# Comparing `tmp/cypcap-0.5.0.tar.gz` & `tmp/cypcap-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypcap-0.5.0.tar", last modified: Sat Oct 14 17:50:29 2023, max compression
+gzip compressed data, was "cypcap-0.6.0.tar", last modified: Wed Apr 17 15:16:16 2024, max compression
```

## Comparing `cypcap-0.5.0.tar` & `cypcap-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 17:50:29.094152 cypcap-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-10-14 17:50:23.000000 cypcap-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-14 17:50:23.000000 cypcap-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2023-10-14 17:50:23.000000 cypcap-0.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-10-14 17:50:29.094152 cypcap-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-10-14 17:50:23.000000 cypcap-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 17:50:29.094152 cypcap-0.5.0/cypcap/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2557194 2023-10-14 17:50:28.000000 cypcap-0.5.0/cypcap/_cypcap.c
--rw-r--r--   0 runner    (1001) docker     (127)    39839 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/_cypcap.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   346394 2023-10-14 17:50:28.000000 cypcap-0.5.0/cypcap/bpf.c
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/bpf.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/cbpf.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/cpcap.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/csocket.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/npcap.pxi
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2023-10-14 17:50:23.000000 cypcap-0.5.0/cypcap/sockaddr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 17:50:29.094152 cypcap-0.5.0/cypcap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-10-14 17:50:29.000000 cypcap-0.5.0/cypcap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-10-14 17:50:29.000000 cypcap-0.5.0/cypcap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 17:50:29.000000 cypcap-0.5.0/cypcap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 17:50:29.000000 cypcap-0.5.0/cypcap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-14 17:50:29.000000 cypcap-0.5.0/cypcap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-14 17:50:29.000000 cypcap-0.5.0/cypcap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-14 17:50:23.000000 cypcap-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 17:50:29.094152 cypcap-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2023-10-14 17:50:23.000000 cypcap-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:16:16.393904 cypcap-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-17 15:16:07.000000 cypcap-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 15:16:07.000000 cypcap-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-04-17 15:16:07.000000 cypcap-0.6.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-17 15:16:16.393904 cypcap-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-17 15:16:07.000000 cypcap-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:16:16.393904 cypcap-0.6.0/cypcap/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2571852 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap/_cypcap.c
+-rw-r--r--   0 runner    (1001) docker     (127)    40150 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/_cypcap.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   348137 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap/bpf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/bpf.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/cbpf.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/cpcap.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/csocket.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/npcap.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-17 15:16:07.000000 cypcap-0.6.0/cypcap/sockaddr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:16:16.393904 cypcap-0.6.0/cypcap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 15:16:16.000000 cypcap-0.6.0/cypcap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 15:16:07.000000 cypcap-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:16:16.393904 cypcap-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-04-17 15:16:07.000000 cypcap-0.6.0/setup.py
```

### Comparing `cypcap-0.5.0/LICENSE` & `cypcap-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/NOTICE` & `cypcap-0.6.0/NOTICE`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/PKG-INFO` & `cypcap-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cypcap
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Cython based binding for modern libpcap
 Home-page: https://github.com/segevfiner/cypcap
 Author: Segev Finer
 Author-email: segev208@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://segevfiner.github.io/cypcap/
 Project-URL: Issue Tracker, https://github.com/segevfiner/cypcap/issues
```

### Comparing `cypcap-0.5.0/README.rst` & `cypcap-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/cypcap/_cypcap.c` & `cypcap-0.6.0/cypcap/_cypcap.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.3 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "libraries": [
             "pcap"
@@ -49,23 +49,23 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_3" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030003F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -149,14 +149,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -210,14 +212,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -271,60 +275,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -407,14 +434,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -599,26 +629,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -631,15 +662,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -664,15 +694,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -750,16 +780,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -826,14 +861,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -901,27 +938,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -957,15 +994,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1101,14 +1138,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1179,15 +1225,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1207,14 +1253,15 @@
 #define __PYX_HAVE__cypcap___cypcap
 #define __PYX_HAVE_API__cypcap___cypcap
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <stdint.h>
+#include <stddef.h>
 #include "pythread.h"
 
     #ifdef _WIN32
     #include <WinSock2.h>
     #else
     #include <sys/socket.h>
     #endif
@@ -1308,14 +1355,15 @@
         return NULL;
     }
     #endif
     
 
     #ifdef _WIN32
     #include <Windows.h>
+    #include <delayimp.h>
     #include <stdio.h>
     #include <wchar.h>
     static int load_npcap_dlls(void)
     {
         WCHAR npcap_dir[512];
         UINT len;
         len = GetSystemDirectoryW(npcap_dir, 480);
@@ -1326,15 +1374,20 @@
 
         wcscat_s(npcap_dir, 512, L"\\Npcap");
         if (SetDllDirectoryW(npcap_dir) == 0) {
             PyErr_SetFromWindowsErr(0);
             return -1;
         }
 
-        pcap_lib_version();
+        __try {
+            pcap_lib_version();
+        } __except (GetExceptionCode() == VcppException(ERROR_SEVERITY_ERROR, ERROR_MOD_NOT_FOUND)) {
+            PyErr_SetString(PyExc_ImportError, "Failed to load Npcap (Is it installed?)");
+            return -1;
+        }
 
         if (SetDllDirectoryW(NULL) == 0) {
             PyErr_SetFromWindowsErr(0);
             return -1;
         }
 
         return 0;
@@ -1421,32 +1474,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1488,15 +1524,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -2273,29 +2309,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2635,15 +2676,19 @@
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
@@ -2675,15 +2720,19 @@
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
+#else
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+#endif
 
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
 }
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
@@ -2717,15 +2766,19 @@
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
@@ -2816,31 +2869,32 @@
 
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_unsigned_short(unsigned short value, Py_ssize_t width, char padding_char, char format_char);
 
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_unsigned_char(unsigned char value, Py_ssize_t width, char padding_char, char format_char);
 
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod1.proto */
+static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
+
 /* StringJoin.proto */
 #if PY_MAJOR_VERSION < 3
 #define __Pyx_PyString_Join __Pyx_PyBytes_Join
 #define __Pyx_PyBaseString_Join(s, v) (PyUnicode_CheckExact(s) ? PyUnicode_Join(s, v) : __Pyx_PyBytes_Join(s, v))
 #else
 #define __Pyx_PyString_Join PyUnicode_Join
 #define __Pyx_PyBaseString_Join PyUnicode_Join
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
-    #if PY_MAJOR_VERSION < 3
-    #define __Pyx_PyBytes_Join _PyString_Join
-    #else
-    #define __Pyx_PyBytes_Join _PyBytes_Join
-    #endif
-#else
 static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values);
-#endif
 
 /* PyObjectFormat.proto */
 #if CYTHON_USE_UNICODE_WRITER
 static PyObject* __Pyx_PyObject_Format(PyObject* s, PyObject* f);
 #else
 #define __Pyx_PyObject_Format(s, f) PyObject_Format(s, f)
 #endif
@@ -2882,17 +2936,14 @@
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
 /* PyObjectCallNoArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* ValidateBasesTuple.proto */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
@@ -2913,40 +2964,40 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
 #elif CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? PyDict_SetItem(ns, name, value) : PyObject_SetItem(ns, name, value))
 #else
 #define __Pyx_SetNameInClass(ns, name, value)  PyObject_SetItem(ns, name, value)
@@ -3038,15 +3089,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -3088,17 +3139,14 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
-/* PyObjectCall2Args.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
 /* CyFunctionClassCell.proto */
@@ -3285,17 +3333,14 @@
 #else
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
-/* PyObjectCallMethod1.proto */
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
-
 /* CoroutineBase.proto */
 struct __pyx_CoroutineObject;
 typedef PyObject *(*__pyx_coroutine_body_t)(struct __pyx_CoroutineObject *, PyThreadState *, PyObject *);
 #if CYTHON_USE_EXC_INFO_STACK
 #define __Pyx_ExcInfoStruct  _PyErr_StackItem
 #else
 typedef struct {
@@ -3365,15 +3410,15 @@
 #define __Pyx_Generator_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_GeneratorType)
 #define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
     __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
 static PyObject *__Pyx_Generator_Next(PyObject *self);
 static int __pyx_Generator_init(PyObject *module);
 
 /* CheckBinaryVersion.proto */
-static unsigned long __Pyx_get_runtime_version();
+static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
@@ -3453,14 +3498,16 @@
 
 /* Module declarations from "__builtin__" */
 
 /* Module declarations from "cpython.complex" */
 
 /* Module declarations from "cpython.string" */
 
+/* Module declarations from "libc.stddef" */
+
 /* Module declarations from "cpython.unicode" */
 
 /* Module declarations from "cpython.pyport" */
 
 /* Module declarations from "cpython.dict" */
 
 /* Module declarations from "cpython.instance" */
@@ -3581,38 +3628,39 @@
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k_d[] = "d";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k_x[] = "x";
 static const char __pyx_k_0x[] = "{ 0x";
-  static const char __pyx_k_IN[] = "IN";
-  static const char __pyx_k_UP[] = "UP";
-  static const char __pyx_k__2[] = ".";
-  static const char __pyx_k__3[] = "*";
-  static const char __pyx_k__6[] = "'";
-  static const char __pyx_k__7[] = ")";
-  static const char __pyx_k__9[] = ")>";
-  static const char __pyx_k_gc[] = "gc";
-  static const char __pyx_k_id[] = "id";
-  static const char __pyx_k_jf[] = "jf";
-  static const char __pyx_k_jt[] = "jt";
-  static const char __pyx_k_on[] = " on ";
-  static const char __pyx_k_os[] = "os";
-  static const char __pyx_k_ts[] = "ts";
-  static const char __pyx_k_08x[] = "08x";
-  static const char __pyx_k_OUT[] = "OUT";
-  static const char __pyx_k_PPP[] = "PPP";
-  static const char __pyx_k_RAW[] = "RAW";
-  static const char __pyx_k__12[] = ">";
-  static const char __pyx_k__20[] = ",";
-  static const char __pyx_k__21[] = " ";
-  static const char __pyx_k__22[] = "";
-  static const char __pyx_k__23[] = "\n";
-  static const char __pyx_k__24[] = ", ";
+static const char __pyx_k_IN[] = "IN";
+static const char __pyx_k_UP[] = "UP";
+static const char __pyx_k__2[] = ".";
+static const char __pyx_k__3[] = "*";
+static const char __pyx_k__6[] = "'";
+static const char __pyx_k__7[] = ")";
+static const char __pyx_k__9[] = ")>";
+static const char __pyx_k_gc[] = "gc";
+static const char __pyx_k_id[] = "id";
+static const char __pyx_k_jf[] = "jf";
+static const char __pyx_k_jt[] = "jt";
+static const char __pyx_k_on[] = " on ";
+static const char __pyx_k_os[] = "os";
+static const char __pyx_k_ts[] = "ts";
+static const char __pyx_k_tz[] = "tz";
+static const char __pyx_k_08x[] = "08x";
+static const char __pyx_k_OUT[] = "OUT";
+static const char __pyx_k_PPP[] = "PPP";
+static const char __pyx_k_RAW[] = "RAW";
+static const char __pyx_k__12[] = ">";
+static const char __pyx_k__20[] = ",";
+static const char __pyx_k__21[] = " ";
+static const char __pyx_k__22[] = "";
+static const char __pyx_k__23[] = "\n";
+static const char __pyx_k__24[] = ", ";
 static const char __pyx_k__25[] = " },";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_buf[] = "buf";
 static const char __pyx_k_cnt[] = "cnt";
 static const char __pyx_k_ctx[] = "ctx";
 static const char __pyx_k_dev[] = "dev";
@@ -3640,15 +3688,15 @@
 static const char __pyx_k_Lock[] = "Lock";
 static const char __pyx_k_NANO[] = "NANO";
 static const char __pyx_k_NULL[] = "NULL_";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_Pcap[] = "<Pcap ";
 static const char __pyx_k_SLIP[] = "SLIP";
 static const char __pyx_k_Stat[] = "Stat";
-static const char __pyx_k__158[] = "?";
+static const char __pyx_k__159[] = "?";
 static const char __pyx_k_addr[] = "addr";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_code[] = "code";
 static const char __pyx_k_devs[] = "devs";
 static const char __pyx_k_dict[] = "__dict__";
@@ -3696,14 +3744,15 @@
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_dumps[] = "dumps";
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_float[] = "float";
+static const char __pyx_k_flush[] = "flush";
 static const char __pyx_k_fname[] = "fname";
 static const char __pyx_k_ftell[] = "ftell";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_insns[] = "insns";
 static const char __pyx_k_len_2[] = ", len=";
 static const char __pyx_k_linux[] = "linux";
 static const char __pyx_k_loads[] = "loads";
@@ -3888,14 +3937,15 @@
 static const char __pyx_k_set_snaplen[] = "set_snaplen";
 static const char __pyx_k_set_timeout[] = "set_timeout";
 static const char __pyx_k_setnonblock[] = "setnonblock";
 static const char __pyx_k_tstamp_type[] = "tstamp_type";
 static const char __pyx_k_BPF_too_long[] = "BPF too long";
 static const char __pyx_k_DatalinkType[] = "DatalinkType";
 static const char __pyx_k_Dumper_close[] = "Dumper.close";
+static const char __pyx_k_Dumper_flush[] = "Dumper.flush";
 static const char __pyx_k_Dumper_ftell[] = "Dumper.ftell";
 static const char __pyx_k_Error___init[] = "Error.__init__";
 static const char __pyx_k_HOST_LOWPREC[] = "HOST_LOWPREC";
 static const char __pyx_k_IFACE_NOT_UP[] = "IFACE_NOT_UP";
 static const char __pyx_k_Optional_int[] = "Optional[int]";
 static const char __pyx_k_Optional_str[] = "Optional[str]";
 static const char __pyx_k_Pcap___enter[] = "Pcap.__enter__";
@@ -3982,15 +4032,14 @@
 static const char __pyx_k_Pcap_set_promisc[] = "Pcap.set_promisc";
 static const char __pyx_k_Pcap_set_snaplen[] = "Pcap.set_snaplen";
 static const char __pyx_k_Pcap_set_timeout[] = "Pcap.set_timeout";
 static const char __pyx_k_Pcap_setnonblock[] = "Pcap.setnonblock";
 static const char __pyx_k_Union_str_PcapIf[] = "Union[str, PcapIf]";
 static const char __pyx_k_dump_open_append[] = "dump_open_append";
 static const char __pyx_k_tstamp_precision[] = "tstamp_precision";
-static const char __pyx_k_utcfromtimestamp[] = "utcfromtimestamp";
 static const char __pyx_k_BpfProgram___iter[] = "BpfProgram.__iter__";
 static const char __pyx_k_List_DatalinkType[] = "List[DatalinkType]";
 static const char __pyx_k_NotSupportedError[] = "NotSupportedError";
 static const char __pyx_k_Pcap_set_datalink[] = "Pcap.set_datalink";
 static const char __pyx_k_Pcap_setdirection[] = "Pcap.setdirection";
 static const char __pyx_k_get_selectable_fd[] = "get_selectable_fd";
 static const char __pyx_k_list_tstamp_types[] = "list_tstamp_types";
@@ -4239,17 +4288,18 @@
 static PyObject *__pyx_pf_6cypcap_7_cypcap_10BpfProgram_21__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_BpfProgram *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_6cypcap_7_cypcap_6Dumper___init__(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
 static void __pyx_pf_6cypcap_7_cypcap_6Dumper_2__dealloc__(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_4close(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_6__enter__(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_8__exit__(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_type, CYTHON_UNUSED PyObject *__pyx_v_exc_value, CYTHON_UNUSED PyObject *__pyx_v_exc_tb); /* proto */
 static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_10dump(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self, struct __pyx_obj_6cypcap_7_cypcap_Pkthdr *__pyx_v_pkt_header, PyObject *__pyx_v_pkt_data); /* proto */
-static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_12ftell(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_12flush(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_14ftell(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_6cypcap_7_cypcap_14lib_version(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_Pkthdr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_Stat(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_Pcap(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_BpfProgram(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_Dumper(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap___pyx_scope_struct____iter__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -4388,14 +4438,16 @@
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_6cypcap_7_cypcap_Pkthdr;
   PyObject *__pyx_type_6cypcap_7_cypcap_Stat;
   PyObject *__pyx_type_6cypcap_7_cypcap_Pcap;
   PyObject *__pyx_type_6cypcap_7_cypcap_BpfProgram;
   PyObject *__pyx_type_6cypcap_7_cypcap_Dumper;
   PyObject *__pyx_type_6cypcap_7_cypcap___pyx_scope_struct____iter__;
   PyObject *__pyx_type___pyx_array;
@@ -4466,14 +4518,15 @@
   PyObject *__pyx_n_s_Dumper;
   PyObject *__pyx_n_s_Dumper___enter;
   PyObject *__pyx_n_s_Dumper___exit;
   PyObject *__pyx_n_s_Dumper___reduce_cython;
   PyObject *__pyx_n_s_Dumper___setstate_cython;
   PyObject *__pyx_n_s_Dumper_close;
   PyObject *__pyx_n_s_Dumper_dump;
+  PyObject *__pyx_n_s_Dumper_flush;
   PyObject *__pyx_n_s_Dumper_ftell;
   PyObject *__pyx_n_s_EN10MB;
   PyObject *__pyx_n_s_EN3MB;
   PyObject *__pyx_n_s_ERROR;
   PyObject *__pyx_n_s_Ellipsis;
   PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
   PyObject *__pyx_n_s_Enum;
@@ -4643,15 +4696,15 @@
   PyObject *__pyx_n_s_WARNING_PROMISC_NOTSUP;
   PyObject *__pyx_n_s_WARNING_TSTAMP_TYPE_NOTSUP;
   PyObject *__pyx_n_s_WIRELESS;
   PyObject *__pyx_n_s_Warning;
   PyObject *__pyx_n_s_Warning___init;
   PyObject *__pyx_kp_s_Warning_category_for_libpcap_wa;
   PyObject *__pyx_kp_u__12;
-  PyObject *__pyx_n_s__158;
+  PyObject *__pyx_n_s__159;
   PyObject *__pyx_kp_u__2;
   PyObject *__pyx_kp_s__20;
   PyObject *__pyx_kp_u__20;
   PyObject *__pyx_kp_u__21;
   PyObject *__pyx_kp_s__22;
   PyObject *__pyx_kp_s__23;
   PyObject *__pyx_kp_u__24;
@@ -4738,14 +4791,15 @@
   PyObject *__pyx_n_s_exc_value;
   PyObject *__pyx_n_s_exit;
   PyObject *__pyx_n_s_filter;
   PyObject *__pyx_n_s_filter_2;
   PyObject *__pyx_n_s_findalldevs;
   PyObject *__pyx_n_s_flags;
   PyObject *__pyx_n_s_float;
+  PyObject *__pyx_n_s_flush;
   PyObject *__pyx_n_s_fname;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_n_s_fortran;
   PyObject *__pyx_n_u_fortran;
   PyObject *__pyx_n_s_fromtimestamp;
   PyObject *__pyx_n_s_fsdecode;
   PyObject *__pyx_n_s_fsencode;
@@ -4918,24 +4972,24 @@
   PyObject *__pyx_n_s_to_ms;
   PyObject *__pyx_n_s_ts;
   PyObject *__pyx_n_s_tstamp_precision;
   PyObject *__pyx_n_s_tstamp_type;
   PyObject *__pyx_n_s_tstamp_types;
   PyObject *__pyx_n_s_type;
   PyObject *__pyx_n_s_typing;
+  PyObject *__pyx_n_s_tz;
   PyObject *__pyx_n_s_tzinfo;
   PyObject *__pyx_kp_s_unable_to_allocate_array_data;
   PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
   PyObject *__pyx_kp_u_unclosed_Dumper;
   PyObject *__pyx_kp_u_unclosed_Pcap;
   PyObject *__pyx_kp_u_unknown_type;
   PyObject *__pyx_n_s_unpack;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_utc;
-  PyObject *__pyx_n_s_utcfromtimestamp;
   PyObject *__pyx_n_s_version_info;
   PyObject *__pyx_n_s_warn;
   PyObject *__pyx_n_s_warnings;
   PyObject *__pyx_n_s_win32;
   PyObject *__pyx_n_u_x;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
@@ -5087,14 +5141,15 @@
   PyObject *__pyx_codeobj__151;
   PyObject *__pyx_codeobj__152;
   PyObject *__pyx_codeobj__153;
   PyObject *__pyx_codeobj__154;
   PyObject *__pyx_codeobj__155;
   PyObject *__pyx_codeobj__156;
   PyObject *__pyx_codeobj__157;
+  PyObject *__pyx_codeobj__158;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -5209,14 +5264,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper___enter);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper___exit);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper_dump);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Dumper_flush);
   Py_CLEAR(clear_module_state->__pyx_n_s_Dumper_ftell);
   Py_CLEAR(clear_module_state->__pyx_n_s_EN10MB);
   Py_CLEAR(clear_module_state->__pyx_n_s_EN3MB);
   Py_CLEAR(clear_module_state->__pyx_n_s_ERROR);
   Py_CLEAR(clear_module_state->__pyx_n_s_Ellipsis);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Empty_shape_tuple_for_cython_arr);
   Py_CLEAR(clear_module_state->__pyx_n_s_Enum);
@@ -5386,15 +5442,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_WARNING_PROMISC_NOTSUP);
   Py_CLEAR(clear_module_state->__pyx_n_s_WARNING_TSTAMP_TYPE_NOTSUP);
   Py_CLEAR(clear_module_state->__pyx_n_s_WIRELESS);
   Py_CLEAR(clear_module_state->__pyx_n_s_Warning);
   Py_CLEAR(clear_module_state->__pyx_n_s_Warning___init);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Warning_category_for_libpcap_wa);
   Py_CLEAR(clear_module_state->__pyx_kp_u__12);
-  Py_CLEAR(clear_module_state->__pyx_n_s__158);
+  Py_CLEAR(clear_module_state->__pyx_n_s__159);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_kp_s__20);
   Py_CLEAR(clear_module_state->__pyx_kp_u__20);
   Py_CLEAR(clear_module_state->__pyx_kp_u__21);
   Py_CLEAR(clear_module_state->__pyx_kp_s__22);
   Py_CLEAR(clear_module_state->__pyx_kp_s__23);
   Py_CLEAR(clear_module_state->__pyx_kp_u__24);
@@ -5481,14 +5537,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_exc_value);
   Py_CLEAR(clear_module_state->__pyx_n_s_exit);
   Py_CLEAR(clear_module_state->__pyx_n_s_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_filter_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_findalldevs);
   Py_CLEAR(clear_module_state->__pyx_n_s_flags);
   Py_CLEAR(clear_module_state->__pyx_n_s_float);
+  Py_CLEAR(clear_module_state->__pyx_n_s_flush);
   Py_CLEAR(clear_module_state->__pyx_n_s_fname);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_n_s_fortran);
   Py_CLEAR(clear_module_state->__pyx_n_u_fortran);
   Py_CLEAR(clear_module_state->__pyx_n_s_fromtimestamp);
   Py_CLEAR(clear_module_state->__pyx_n_s_fsdecode);
   Py_CLEAR(clear_module_state->__pyx_n_s_fsencode);
@@ -5661,24 +5718,24 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_to_ms);
   Py_CLEAR(clear_module_state->__pyx_n_s_ts);
   Py_CLEAR(clear_module_state->__pyx_n_s_tstamp_precision);
   Py_CLEAR(clear_module_state->__pyx_n_s_tstamp_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_tstamp_types);
   Py_CLEAR(clear_module_state->__pyx_n_s_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_typing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tz);
   Py_CLEAR(clear_module_state->__pyx_n_s_tzinfo);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unclosed_Dumper);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unclosed_Pcap);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unknown_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_unpack);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_utc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_utcfromtimestamp);
   Py_CLEAR(clear_module_state->__pyx_n_s_version_info);
   Py_CLEAR(clear_module_state->__pyx_n_s_warn);
   Py_CLEAR(clear_module_state->__pyx_n_s_warnings);
   Py_CLEAR(clear_module_state->__pyx_n_s_win32);
   Py_CLEAR(clear_module_state->__pyx_n_u_x);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
@@ -5830,14 +5887,15 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__151);
   Py_CLEAR(clear_module_state->__pyx_codeobj__152);
   Py_CLEAR(clear_module_state->__pyx_codeobj__153);
   Py_CLEAR(clear_module_state->__pyx_codeobj__154);
   Py_CLEAR(clear_module_state->__pyx_codeobj__155);
   Py_CLEAR(clear_module_state->__pyx_codeobj__156);
   Py_CLEAR(clear_module_state->__pyx_codeobj__157);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__158);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -5930,14 +5988,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper___enter);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper___exit);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper_dump);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Dumper_flush);
   Py_VISIT(traverse_module_state->__pyx_n_s_Dumper_ftell);
   Py_VISIT(traverse_module_state->__pyx_n_s_EN10MB);
   Py_VISIT(traverse_module_state->__pyx_n_s_EN3MB);
   Py_VISIT(traverse_module_state->__pyx_n_s_ERROR);
   Py_VISIT(traverse_module_state->__pyx_n_s_Ellipsis);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Empty_shape_tuple_for_cython_arr);
   Py_VISIT(traverse_module_state->__pyx_n_s_Enum);
@@ -6107,15 +6166,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_WARNING_PROMISC_NOTSUP);
   Py_VISIT(traverse_module_state->__pyx_n_s_WARNING_TSTAMP_TYPE_NOTSUP);
   Py_VISIT(traverse_module_state->__pyx_n_s_WIRELESS);
   Py_VISIT(traverse_module_state->__pyx_n_s_Warning);
   Py_VISIT(traverse_module_state->__pyx_n_s_Warning___init);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Warning_category_for_libpcap_wa);
   Py_VISIT(traverse_module_state->__pyx_kp_u__12);
-  Py_VISIT(traverse_module_state->__pyx_n_s__158);
+  Py_VISIT(traverse_module_state->__pyx_n_s__159);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_kp_s__20);
   Py_VISIT(traverse_module_state->__pyx_kp_u__20);
   Py_VISIT(traverse_module_state->__pyx_kp_u__21);
   Py_VISIT(traverse_module_state->__pyx_kp_s__22);
   Py_VISIT(traverse_module_state->__pyx_kp_s__23);
   Py_VISIT(traverse_module_state->__pyx_kp_u__24);
@@ -6202,14 +6261,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_exc_value);
   Py_VISIT(traverse_module_state->__pyx_n_s_exit);
   Py_VISIT(traverse_module_state->__pyx_n_s_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_filter_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_findalldevs);
   Py_VISIT(traverse_module_state->__pyx_n_s_flags);
   Py_VISIT(traverse_module_state->__pyx_n_s_float);
+  Py_VISIT(traverse_module_state->__pyx_n_s_flush);
   Py_VISIT(traverse_module_state->__pyx_n_s_fname);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_n_s_fortran);
   Py_VISIT(traverse_module_state->__pyx_n_u_fortran);
   Py_VISIT(traverse_module_state->__pyx_n_s_fromtimestamp);
   Py_VISIT(traverse_module_state->__pyx_n_s_fsdecode);
   Py_VISIT(traverse_module_state->__pyx_n_s_fsencode);
@@ -6382,24 +6442,24 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_to_ms);
   Py_VISIT(traverse_module_state->__pyx_n_s_ts);
   Py_VISIT(traverse_module_state->__pyx_n_s_tstamp_precision);
   Py_VISIT(traverse_module_state->__pyx_n_s_tstamp_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_tstamp_types);
   Py_VISIT(traverse_module_state->__pyx_n_s_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_typing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tz);
   Py_VISIT(traverse_module_state->__pyx_n_s_tzinfo);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unclosed_Dumper);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unclosed_Pcap);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unknown_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_unpack);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_utc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_utcfromtimestamp);
   Py_VISIT(traverse_module_state->__pyx_n_s_version_info);
   Py_VISIT(traverse_module_state->__pyx_n_s_warn);
   Py_VISIT(traverse_module_state->__pyx_n_s_warnings);
   Py_VISIT(traverse_module_state->__pyx_n_s_win32);
   Py_VISIT(traverse_module_state->__pyx_n_u_x);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
@@ -6551,14 +6611,15 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__151);
   Py_VISIT(traverse_module_state->__pyx_codeobj__152);
   Py_VISIT(traverse_module_state->__pyx_codeobj__153);
   Py_VISIT(traverse_module_state->__pyx_codeobj__154);
   Py_VISIT(traverse_module_state->__pyx_codeobj__155);
   Py_VISIT(traverse_module_state->__pyx_codeobj__156);
   Py_VISIT(traverse_module_state->__pyx_codeobj__157);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__158);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -6685,14 +6746,16 @@
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
 #define __pyx_type_6cypcap_7_cypcap_Pkthdr __pyx_mstate_global->__pyx_type_6cypcap_7_cypcap_Pkthdr
 #define __pyx_type_6cypcap_7_cypcap_Stat __pyx_mstate_global->__pyx_type_6cypcap_7_cypcap_Stat
 #define __pyx_type_6cypcap_7_cypcap_Pcap __pyx_mstate_global->__pyx_type_6cypcap_7_cypcap_Pcap
 #define __pyx_type_6cypcap_7_cypcap_BpfProgram __pyx_mstate_global->__pyx_type_6cypcap_7_cypcap_BpfProgram
 #define __pyx_type_6cypcap_7_cypcap_Dumper __pyx_mstate_global->__pyx_type_6cypcap_7_cypcap_Dumper
 #define __pyx_type_6cypcap_7_cypcap___pyx_scope_struct____iter__ __pyx_mstate_global->__pyx_type_6cypcap_7_cypcap___pyx_scope_struct____iter__
 #define __pyx_type___pyx_array __pyx_mstate_global->__pyx_type___pyx_array
@@ -6763,14 +6826,15 @@
 #define __pyx_n_s_Dumper __pyx_mstate_global->__pyx_n_s_Dumper
 #define __pyx_n_s_Dumper___enter __pyx_mstate_global->__pyx_n_s_Dumper___enter
 #define __pyx_n_s_Dumper___exit __pyx_mstate_global->__pyx_n_s_Dumper___exit
 #define __pyx_n_s_Dumper___reduce_cython __pyx_mstate_global->__pyx_n_s_Dumper___reduce_cython
 #define __pyx_n_s_Dumper___setstate_cython __pyx_mstate_global->__pyx_n_s_Dumper___setstate_cython
 #define __pyx_n_s_Dumper_close __pyx_mstate_global->__pyx_n_s_Dumper_close
 #define __pyx_n_s_Dumper_dump __pyx_mstate_global->__pyx_n_s_Dumper_dump
+#define __pyx_n_s_Dumper_flush __pyx_mstate_global->__pyx_n_s_Dumper_flush
 #define __pyx_n_s_Dumper_ftell __pyx_mstate_global->__pyx_n_s_Dumper_ftell
 #define __pyx_n_s_EN10MB __pyx_mstate_global->__pyx_n_s_EN10MB
 #define __pyx_n_s_EN3MB __pyx_mstate_global->__pyx_n_s_EN3MB
 #define __pyx_n_s_ERROR __pyx_mstate_global->__pyx_n_s_ERROR
 #define __pyx_n_s_Ellipsis __pyx_mstate_global->__pyx_n_s_Ellipsis
 #define __pyx_kp_s_Empty_shape_tuple_for_cython_arr __pyx_mstate_global->__pyx_kp_s_Empty_shape_tuple_for_cython_arr
 #define __pyx_n_s_Enum __pyx_mstate_global->__pyx_n_s_Enum
@@ -6940,15 +7004,15 @@
 #define __pyx_n_s_WARNING_PROMISC_NOTSUP __pyx_mstate_global->__pyx_n_s_WARNING_PROMISC_NOTSUP
 #define __pyx_n_s_WARNING_TSTAMP_TYPE_NOTSUP __pyx_mstate_global->__pyx_n_s_WARNING_TSTAMP_TYPE_NOTSUP
 #define __pyx_n_s_WIRELESS __pyx_mstate_global->__pyx_n_s_WIRELESS
 #define __pyx_n_s_Warning __pyx_mstate_global->__pyx_n_s_Warning
 #define __pyx_n_s_Warning___init __pyx_mstate_global->__pyx_n_s_Warning___init
 #define __pyx_kp_s_Warning_category_for_libpcap_wa __pyx_mstate_global->__pyx_kp_s_Warning_category_for_libpcap_wa
 #define __pyx_kp_u__12 __pyx_mstate_global->__pyx_kp_u__12
-#define __pyx_n_s__158 __pyx_mstate_global->__pyx_n_s__158
+#define __pyx_n_s__159 __pyx_mstate_global->__pyx_n_s__159
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_kp_s__20 __pyx_mstate_global->__pyx_kp_s__20
 #define __pyx_kp_u__20 __pyx_mstate_global->__pyx_kp_u__20
 #define __pyx_kp_u__21 __pyx_mstate_global->__pyx_kp_u__21
 #define __pyx_kp_s__22 __pyx_mstate_global->__pyx_kp_s__22
 #define __pyx_kp_s__23 __pyx_mstate_global->__pyx_kp_s__23
 #define __pyx_kp_u__24 __pyx_mstate_global->__pyx_kp_u__24
@@ -7035,14 +7099,15 @@
 #define __pyx_n_s_exc_value __pyx_mstate_global->__pyx_n_s_exc_value
 #define __pyx_n_s_exit __pyx_mstate_global->__pyx_n_s_exit
 #define __pyx_n_s_filter __pyx_mstate_global->__pyx_n_s_filter
 #define __pyx_n_s_filter_2 __pyx_mstate_global->__pyx_n_s_filter_2
 #define __pyx_n_s_findalldevs __pyx_mstate_global->__pyx_n_s_findalldevs
 #define __pyx_n_s_flags __pyx_mstate_global->__pyx_n_s_flags
 #define __pyx_n_s_float __pyx_mstate_global->__pyx_n_s_float
+#define __pyx_n_s_flush __pyx_mstate_global->__pyx_n_s_flush
 #define __pyx_n_s_fname __pyx_mstate_global->__pyx_n_s_fname
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_n_s_fortran __pyx_mstate_global->__pyx_n_s_fortran
 #define __pyx_n_u_fortran __pyx_mstate_global->__pyx_n_u_fortran
 #define __pyx_n_s_fromtimestamp __pyx_mstate_global->__pyx_n_s_fromtimestamp
 #define __pyx_n_s_fsdecode __pyx_mstate_global->__pyx_n_s_fsdecode
 #define __pyx_n_s_fsencode __pyx_mstate_global->__pyx_n_s_fsencode
@@ -7215,24 +7280,24 @@
 #define __pyx_n_s_to_ms __pyx_mstate_global->__pyx_n_s_to_ms
 #define __pyx_n_s_ts __pyx_mstate_global->__pyx_n_s_ts
 #define __pyx_n_s_tstamp_precision __pyx_mstate_global->__pyx_n_s_tstamp_precision
 #define __pyx_n_s_tstamp_type __pyx_mstate_global->__pyx_n_s_tstamp_type
 #define __pyx_n_s_tstamp_types __pyx_mstate_global->__pyx_n_s_tstamp_types
 #define __pyx_n_s_type __pyx_mstate_global->__pyx_n_s_type
 #define __pyx_n_s_typing __pyx_mstate_global->__pyx_n_s_typing
+#define __pyx_n_s_tz __pyx_mstate_global->__pyx_n_s_tz
 #define __pyx_n_s_tzinfo __pyx_mstate_global->__pyx_n_s_tzinfo
 #define __pyx_kp_s_unable_to_allocate_array_data __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_array_data
 #define __pyx_kp_s_unable_to_allocate_shape_and_str __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_shape_and_str
 #define __pyx_kp_u_unclosed_Dumper __pyx_mstate_global->__pyx_kp_u_unclosed_Dumper
 #define __pyx_kp_u_unclosed_Pcap __pyx_mstate_global->__pyx_kp_u_unclosed_Pcap
 #define __pyx_kp_u_unknown_type __pyx_mstate_global->__pyx_kp_u_unknown_type
 #define __pyx_n_s_unpack __pyx_mstate_global->__pyx_n_s_unpack
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_utc __pyx_mstate_global->__pyx_n_s_utc
-#define __pyx_n_s_utcfromtimestamp __pyx_mstate_global->__pyx_n_s_utcfromtimestamp
 #define __pyx_n_s_version_info __pyx_mstate_global->__pyx_n_s_version_info
 #define __pyx_n_s_warn __pyx_mstate_global->__pyx_n_s_warn
 #define __pyx_n_s_warnings __pyx_mstate_global->__pyx_n_s_warnings
 #define __pyx_n_s_win32 __pyx_mstate_global->__pyx_n_s_win32
 #define __pyx_n_u_x __pyx_mstate_global->__pyx_n_u_x
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
@@ -7384,14 +7449,15 @@
 #define __pyx_codeobj__151 __pyx_mstate_global->__pyx_codeobj__151
 #define __pyx_codeobj__152 __pyx_mstate_global->__pyx_codeobj__152
 #define __pyx_codeobj__153 __pyx_mstate_global->__pyx_codeobj__153
 #define __pyx_codeobj__154 __pyx_mstate_global->__pyx_codeobj__154
 #define __pyx_codeobj__155 __pyx_mstate_global->__pyx_codeobj__155
 #define __pyx_codeobj__156 __pyx_mstate_global->__pyx_codeobj__156
 #define __pyx_codeobj__157 __pyx_mstate_global->__pyx_codeobj__157
+#define __pyx_codeobj__158 __pyx_mstate_global->__pyx_codeobj__158
 /* #### Code section: module_code ### */
 
 /* "View.MemoryView":131
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
@@ -21015,70 +21081,70 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -24630,15 +24696,15 @@
 }
 
 /* "cypcap/_cypcap.pyx":337
  *         self.ts = ts_datetime.timestamp()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def ts_utcdatetime(self) -> datetime:
- *         """Timestamp as a naive UTC datetime."""
+ *         """Timestamp as a UTC aware datetime."""
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6cypcap_7_cypcap_6Pkthdr_14ts_utcdatetime_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_6cypcap_7_cypcap_6Pkthdr_14ts_utcdatetime_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
@@ -24655,86 +24721,83 @@
 static PyObject *__pyx_pf_6cypcap_7_cypcap_6Pkthdr_14ts_utcdatetime___get__(struct __pyx_obj_6cypcap_7_cypcap_Pkthdr *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "cypcap/_cypcap.pyx":340
  *     def ts_utcdatetime(self) -> datetime:
- *         """Timestamp as a naive UTC datetime."""
- *         return datetime.utcfromtimestamp(self.ts)             # <<<<<<<<<<<<<<
+ *         """Timestamp as a UTC aware datetime."""
+ *         return datetime.fromtimestamp(self.ts, tz=timezone.utc)             # <<<<<<<<<<<<<<
  * 
  *     @ts_utcdatetime.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_datetime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fromtimestamp); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_utcfromtimestamp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_timezone); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_utc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_tz, __pyx_t_5) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ts); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_5 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "cypcap/_cypcap.pyx":337
  *         self.ts = ts_datetime.timestamp()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def ts_utcdatetime(self) -> datetime:
- *         """Timestamp as a naive UTC datetime."""
+ *         """Timestamp as a UTC aware datetime."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("cypcap._cypcap.Pkthdr.ts_utcdatetime.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cypcap/_cypcap.pyx":342
- *         return datetime.utcfromtimestamp(self.ts)
+ *         return datetime.fromtimestamp(self.ts, tz=timezone.utc)
  * 
  *     @ts_utcdatetime.setter             # <<<<<<<<<<<<<<
  *     def ts_utcdatetime(self, ts_utcdatetime: datetime):
  *         if ts_utcdatetime.tzinfo is None:
  */
 
 /* Python wrapper */
@@ -24845,15 +24908,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ts, __pyx_t_5) < 0) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cypcap/_cypcap.pyx":342
- *         return datetime.utcfromtimestamp(self.ts)
+ *         return datetime.fromtimestamp(self.ts, tz=timezone.utc)
  * 
  *     @ts_utcdatetime.setter             # <<<<<<<<<<<<<<
  *     def ts_utcdatetime(self, ts_utcdatetime: datetime):
  *         if ts_utcdatetime.tzinfo is None:
  */
 
   /* function exit code */
@@ -43347,15 +43410,15 @@
   __pyx_t_1 = ((struct __pyx_vtabstruct_6cypcap_7_cypcap_Dumper *)__pyx_v_self->__pyx_vtab)->_check_closed(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1279, __pyx_L1_error)
 
   /* "cypcap/_cypcap.pyx":1281
  *         self._check_closed()
  * 
  *         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)             # <<<<<<<<<<<<<<
  * 
- *     def ftell(self) -> int:
+ *     def flush(self):
  */
   __pyx_t_2 = __Pyx_PyObject_AsUString(__pyx_v_pkt_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 1281, __pyx_L1_error)
   pcap_dump(((unsigned char *)__pyx_v_self->dumper), (&__pyx_v_pkt_header->pkthdr), __pyx_t_2);
 
   /* "cypcap/_cypcap.pyx":1277
  *         self.close()
  * 
@@ -43375,30 +43438,215 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cypcap/_cypcap.pyx":1283
  *         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)
  * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         """Flush the packets to the capture file."""
+ *         self._check_closed()
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_13flush(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6cypcap_7_cypcap_6Dumper_12flush, "Flush the packets to the capture file.");
+static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_13flush = {"flush", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_13flush, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_12flush};
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_13flush(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("flush (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("flush", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "flush", 0))) return NULL;
+  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_12flush(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_12flush(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self) {
+  int __pyx_v_result;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  char const *__pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("flush", 1);
+
+  /* "cypcap/_cypcap.pyx":1285
+ *     def flush(self):
+ *         """Flush the packets to the capture file."""
+ *         self._check_closed()             # <<<<<<<<<<<<<<
+ * 
+ *         result = cpcap.pcap_dump_flush(self.dumper)
+ */
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6cypcap_7_cypcap_Dumper *)__pyx_v_self->__pyx_vtab)->_check_closed(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1285, __pyx_L1_error)
+
+  /* "cypcap/_cypcap.pyx":1287
+ *         self._check_closed()
+ * 
+ *         result = cpcap.pcap_dump_flush(self.dumper)             # <<<<<<<<<<<<<<
+ *         if result == cpcap.PCAP_ERROR:
+ *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
+ */
+  __pyx_v_result = pcap_dump_flush(__pyx_v_self->dumper);
+
+  /* "cypcap/_cypcap.pyx":1288
+ * 
+ *         result = cpcap.pcap_dump_flush(self.dumper)
+ *         if result == cpcap.PCAP_ERROR:             # <<<<<<<<<<<<<<
+ *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_result == PCAP_ERROR);
+  if (unlikely(__pyx_t_2)) {
+
+    /* "cypcap/_cypcap.pyx":1289
+ *         result = cpcap.pcap_dump_flush(self.dumper)
+ *         if result == cpcap.PCAP_ERROR:
+ *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())             # <<<<<<<<<<<<<<
+ * 
+ *         return result
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = pcap_statustostr(((int)__pyx_v_result));
+    __pyx_t_7 = __Pyx_ssize_strlen(__pyx_t_6); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_decode_c_string(__pyx_t_6, 0, __pyx_t_7, NULL, NULL, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = NULL;
+    __pyx_t_1 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_9);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_t_5, __pyx_t_8};
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 2+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1289, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    }
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(0, 1289, __pyx_L1_error)
+
+    /* "cypcap/_cypcap.pyx":1288
+ * 
+ *         result = cpcap.pcap_dump_flush(self.dumper)
+ *         if result == cpcap.PCAP_ERROR:             # <<<<<<<<<<<<<<
+ *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
+ * 
+ */
+  }
+
+  /* "cypcap/_cypcap.pyx":1291
+ *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
+ * 
+ *         return result             # <<<<<<<<<<<<<<
+ * 
+ *     def ftell(self) -> int:
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1291, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "cypcap/_cypcap.pyx":1283
+ *         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)
+ * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         """Flush the packets to the capture file."""
+ *         self._check_closed()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("cypcap._cypcap.Dumper.flush", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "cypcap/_cypcap.pyx":1293
+ *         return result
+ * 
  *     def ftell(self) -> int:             # <<<<<<<<<<<<<<
  *         """Get the current file offset for a savefile being written."""
  *         self._check_closed()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_13ftell(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_15ftell(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_6cypcap_7_cypcap_6Dumper_12ftell, "Get the current file offset for a savefile being written.");
-static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_13ftell = {"ftell", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_13ftell, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_12ftell};
-static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_13ftell(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_6cypcap_7_cypcap_6Dumper_14ftell, "Get the current file offset for a savefile being written.");
+static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_15ftell = {"ftell", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_15ftell, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_14ftell};
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_15ftell(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -43415,22 +43663,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("ftell", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "ftell", 0))) return NULL;
-  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_12ftell(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_14ftell(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_12ftell(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self) {
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_14ftell(struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self) {
   int64_t __pyx_v_result;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -43440,56 +43688,56 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ftell", 1);
 
-  /* "cypcap/_cypcap.pyx":1285
+  /* "cypcap/_cypcap.pyx":1295
  *     def ftell(self) -> int:
  *         """Get the current file offset for a savefile being written."""
  *         self._check_closed()             # <<<<<<<<<<<<<<
  * 
  *         result = cpcap.pcap_dump_ftell64(self.dumper)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6cypcap_7_cypcap_Dumper *)__pyx_v_self->__pyx_vtab)->_check_closed(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6cypcap_7_cypcap_Dumper *)__pyx_v_self->__pyx_vtab)->_check_closed(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1295, __pyx_L1_error)
 
-  /* "cypcap/_cypcap.pyx":1287
+  /* "cypcap/_cypcap.pyx":1297
  *         self._check_closed()
  * 
  *         result = cpcap.pcap_dump_ftell64(self.dumper)             # <<<<<<<<<<<<<<
  *         if result == cpcap.PCAP_ERROR:
  *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
  */
   __pyx_v_result = pcap_dump_ftell64(__pyx_v_self->dumper);
 
-  /* "cypcap/_cypcap.pyx":1288
+  /* "cypcap/_cypcap.pyx":1298
  * 
  *         result = cpcap.pcap_dump_ftell64(self.dumper)
  *         if result == cpcap.PCAP_ERROR:             # <<<<<<<<<<<<<<
  *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
  * 
  */
   __pyx_t_2 = (__pyx_v_result == PCAP_ERROR);
   if (unlikely(__pyx_t_2)) {
 
-    /* "cypcap/_cypcap.pyx":1289
+    /* "cypcap/_cypcap.pyx":1299
  *         result = cpcap.pcap_dump_ftell64(self.dumper)
  *         if result == cpcap.PCAP_ERROR:
  *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())             # <<<<<<<<<<<<<<
  * 
  *         return result
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = pcap_statustostr(((int)__pyx_v_result));
-    __pyx_t_7 = __Pyx_ssize_strlen(__pyx_t_6); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1289, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_decode_c_string(__pyx_t_6, 0, __pyx_t_7, NULL, NULL, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1289, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_ssize_strlen(__pyx_t_6); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1299, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_decode_c_string(__pyx_t_6, 0, __pyx_t_7, NULL, NULL, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_9)) {
@@ -43503,48 +43751,48 @@
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_t_5, __pyx_t_8};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 2+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1289, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 1289, __pyx_L1_error)
+    __PYX_ERR(0, 1299, __pyx_L1_error)
 
-    /* "cypcap/_cypcap.pyx":1288
+    /* "cypcap/_cypcap.pyx":1298
  * 
  *         result = cpcap.pcap_dump_ftell64(self.dumper)
  *         if result == cpcap.PCAP_ERROR:             # <<<<<<<<<<<<<<
  *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
  * 
  */
   }
 
-  /* "cypcap/_cypcap.pyx":1291
+  /* "cypcap/_cypcap.pyx":1301
  *             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
  * 
  *         return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1291, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 1291, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 1301, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "cypcap/_cypcap.pyx":1283
- *         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)
+  /* "cypcap/_cypcap.pyx":1293
+ *         return result
  * 
  *     def ftell(self) -> int:             # <<<<<<<<<<<<<<
  *         """Get the current file offset for a savefile being written."""
  *         self._check_closed()
  */
 
   /* function exit code */
@@ -43565,23 +43813,23 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_15__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_17__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_15__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_15__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_15__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_17__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_17__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -43598,22 +43846,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_14__reduce_cython__(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_16__reduce_cython__(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self) {
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
@@ -43645,23 +43893,23 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_17__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_19__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_17__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_17__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_17__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_6cypcap_7_cypcap_6Dumper_19__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6cypcap_7_cypcap_6Dumper_19__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
@@ -43727,28 +43975,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("cypcap._cypcap.Dumper.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_16__setstate_cython__(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_6cypcap_7_cypcap_6Dumper_18__setstate_cython__(((struct __pyx_obj_6cypcap_7_cypcap_Dumper *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_6cypcap_7_cypcap_6Dumper_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6cypcap_7_cypcap_Dumper *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
@@ -43772,15 +44020,15 @@
   __Pyx_AddTraceback("cypcap._cypcap.Dumper.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cypcap/_cypcap.pyx":1294
+/* "cypcap/_cypcap.pyx":1304
  * 
  * 
  * def lib_version() -> str:             # <<<<<<<<<<<<<<
  *     """Get the version information for libpcap."""
  *     return cpcap.pcap_lib_version().decode()
  */
 
@@ -43808,31 +44056,31 @@
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lib_version", 1);
 
-  /* "cypcap/_cypcap.pyx":1296
+  /* "cypcap/_cypcap.pyx":1306
  * def lib_version() -> str:
  *     """Get the version information for libpcap."""
  *     return cpcap.pcap_lib_version().decode()             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = pcap_lib_version();
-  __pyx_t_2 = __Pyx_ssize_strlen(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1296, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_1, 0, __pyx_t_2, NULL, NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1296, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ssize_strlen(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1306, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_1, 0, __pyx_t_2, NULL, NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(PyString_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("str", __pyx_t_3))) __PYX_ERR(0, 1296, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("str", __pyx_t_3))) __PYX_ERR(0, 1306, __pyx_L1_error)
   __Pyx_INCREF(__pyx_t_3);
   __pyx_r = ((PyObject*)__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "cypcap/_cypcap.pyx":1294
+  /* "cypcap/_cypcap.pyx":1304
  * 
  * 
  * def lib_version() -> str:             # <<<<<<<<<<<<<<
  *     """Get the version information for libpcap."""
  *     return cpcap.pcap_lib_version().decode()
  */
 
@@ -43844,25 +44092,27 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static struct __pyx_vtabstruct_6cypcap_7_cypcap_Pkthdr __pyx_vtable_6cypcap_7_cypcap_Pkthdr;
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_6cypcap_7_cypcap_Pkthdr *__pyx_freelist_6cypcap_7_cypcap_Pkthdr[8];
 static int __pyx_freecount_6cypcap_7_cypcap_Pkthdr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_Pkthdr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6cypcap_7_cypcap_Pkthdr *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_6cypcap_7_cypcap_Pkthdr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_6cypcap_7_cypcap_Pkthdr)) & (int)(!__Pyx_PyType_HasFeature(t, (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE))))) {
     o = (PyObject*)__pyx_freelist_6cypcap_7_cypcap_Pkthdr[--__pyx_freecount_6cypcap_7_cypcap_Pkthdr];
     memset(o, 0, sizeof(struct __pyx_obj_6cypcap_7_cypcap_Pkthdr));
     (void) PyObject_INIT(o, t);
   } else
   #endif
   {
@@ -43883,15 +44133,15 @@
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_6cypcap_7_cypcap_Pkthdr) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_6cypcap_7_cypcap_Pkthdr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6cypcap_7_cypcap_Pkthdr)) & (int)(!__Pyx_PyType_HasFeature(Py_TYPE(o), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE))))) {
     __pyx_freelist_6cypcap_7_cypcap_Pkthdr[__pyx_freecount_6cypcap_7_cypcap_Pkthdr++] = ((struct __pyx_obj_6cypcap_7_cypcap_Pkthdr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -43984,15 +44234,15 @@
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Pkthdr_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_6cypcap_7_cypcap_Pkthdr[] = {
   {(char *)"ts", __pyx_getprop_6cypcap_7_cypcap_6Pkthdr_ts, __pyx_setprop_6cypcap_7_cypcap_6Pkthdr_ts, (char *)PyDoc_STR("Timestamp."), 0},
   {(char *)"ts_datetime", __pyx_getprop_6cypcap_7_cypcap_6Pkthdr_ts_datetime, __pyx_setprop_6cypcap_7_cypcap_6Pkthdr_ts_datetime, (char *)PyDoc_STR("Timestamp as a naive local datetime."), 0},
-  {(char *)"ts_utcdatetime", __pyx_getprop_6cypcap_7_cypcap_6Pkthdr_ts_utcdatetime, __pyx_setprop_6cypcap_7_cypcap_6Pkthdr_ts_utcdatetime, (char *)PyDoc_STR("Timestamp as a naive UTC datetime."), 0},
+  {(char *)"ts_utcdatetime", __pyx_getprop_6cypcap_7_cypcap_6Pkthdr_ts_utcdatetime, __pyx_setprop_6cypcap_7_cypcap_6Pkthdr_ts_utcdatetime, (char *)PyDoc_STR("Timestamp as a UTC aware datetime."), 0},
   {(char *)"caplen", __pyx_getprop_6cypcap_7_cypcap_6Pkthdr_caplen, __pyx_setprop_6cypcap_7_cypcap_6Pkthdr_caplen, (char *)PyDoc_STR("Length of portion present."), 0},
   {(char *)"len", __pyx_getprop_6cypcap_7_cypcap_6Pkthdr_len, __pyx_setprop_6cypcap_7_cypcap_6Pkthdr_len, (char *)PyDoc_STR("Length of this packet (off wire)."), 0},
   {0, 0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_6cypcap_7_cypcap_Pkthdr_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_6cypcap_7_cypcap_Pkthdr},
@@ -44091,24 +44341,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_6cypcap_7_cypcap_Stat *__pyx_freelist_6cypcap_7_cypcap_Stat[8];
 static int __pyx_freecount_6cypcap_7_cypcap_Stat = 0;
+#endif
 
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap_Stat(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_6cypcap_7_cypcap_Stat > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_6cypcap_7_cypcap_Stat)) & (int)(!__Pyx_PyType_HasFeature(t, (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE))))) {
     o = (PyObject*)__pyx_freelist_6cypcap_7_cypcap_Stat[--__pyx_freecount_6cypcap_7_cypcap_Stat];
     memset(o, 0, sizeof(struct __pyx_obj_6cypcap_7_cypcap_Stat));
     (void) PyObject_INIT(o, t);
   } else
   #endif
   {
@@ -44127,15 +44379,15 @@
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_6cypcap_7_cypcap_Stat) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_6cypcap_7_cypcap_Stat < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6cypcap_7_cypcap_Stat)) & (int)(!__Pyx_PyType_HasFeature(Py_TYPE(o), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE))))) {
     __pyx_freelist_6cypcap_7_cypcap_Stat[__pyx_freecount_6cypcap_7_cypcap_Stat++] = ((struct __pyx_obj_6cypcap_7_cypcap_Stat *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -44755,17 +45007,18 @@
   #endif
 }
 
 static PyMethodDef __pyx_methods_6cypcap_7_cypcap_Dumper[] = {
   {"__enter__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_7__enter__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"__exit__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_9__exit__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"dump", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_11dump, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_10dump},
-  {"ftell", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_13ftell, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_12ftell},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_15__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_17__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"flush", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_13flush, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_12flush},
+  {"ftell", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_15ftell, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6cypcap_7_cypcap_6Dumper_14ftell},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6cypcap_7_cypcap_6Dumper_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_6cypcap_7_cypcap_Dumper_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_6cypcap_7_cypcap_Dumper},
   {Py_tp_doc, (void *)PyDoc_STR("Dumper represents a capture savefile.")},
   {Py_tp_methods, (void *)__pyx_methods_6cypcap_7_cypcap_Dumper},
@@ -44860,24 +45113,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_6cypcap_7_cypcap___pyx_scope_struct____iter__ *__pyx_freelist_6cypcap_7_cypcap___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_6cypcap_7_cypcap___pyx_scope_struct____iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_6cypcap_7_cypcap___pyx_scope_struct____iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_6cypcap_7_cypcap___pyx_scope_struct____iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_6cypcap_7_cypcap___pyx_scope_struct____iter__)))) {
     o = (PyObject*)__pyx_freelist_6cypcap_7_cypcap___pyx_scope_struct____iter__[--__pyx_freecount_6cypcap_7_cypcap___pyx_scope_struct____iter__];
     memset(o, 0, sizeof(struct __pyx_obj_6cypcap_7_cypcap___pyx_scope_struct____iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -44896,15 +45151,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_6cypcap_7_cypcap___pyx_scope_struct____iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_6cypcap_7_cypcap___pyx_scope_struct____iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6cypcap_7_cypcap___pyx_scope_struct____iter__)))) {
     __pyx_freelist_6cypcap_7_cypcap___pyx_scope_struct____iter__[__pyx_freecount_6cypcap_7_cypcap___pyx_scope_struct____iter__++] = ((struct __pyx_obj_6cypcap_7_cypcap___pyx_scope_struct____iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -46038,14 +46293,15 @@
     {&__pyx_n_s_Dumper, __pyx_k_Dumper, sizeof(__pyx_k_Dumper), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper___enter, __pyx_k_Dumper___enter, sizeof(__pyx_k_Dumper___enter), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper___exit, __pyx_k_Dumper___exit, sizeof(__pyx_k_Dumper___exit), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper___reduce_cython, __pyx_k_Dumper___reduce_cython, sizeof(__pyx_k_Dumper___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper___setstate_cython, __pyx_k_Dumper___setstate_cython, sizeof(__pyx_k_Dumper___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper_close, __pyx_k_Dumper_close, sizeof(__pyx_k_Dumper_close), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper_dump, __pyx_k_Dumper_dump, sizeof(__pyx_k_Dumper_dump), 0, 0, 1, 1},
+    {&__pyx_n_s_Dumper_flush, __pyx_k_Dumper_flush, sizeof(__pyx_k_Dumper_flush), 0, 0, 1, 1},
     {&__pyx_n_s_Dumper_ftell, __pyx_k_Dumper_ftell, sizeof(__pyx_k_Dumper_ftell), 0, 0, 1, 1},
     {&__pyx_n_s_EN10MB, __pyx_k_EN10MB, sizeof(__pyx_k_EN10MB), 0, 0, 1, 1},
     {&__pyx_n_s_EN3MB, __pyx_k_EN3MB, sizeof(__pyx_k_EN3MB), 0, 0, 1, 1},
     {&__pyx_n_s_ERROR, __pyx_k_ERROR, sizeof(__pyx_k_ERROR), 0, 0, 1, 1},
     {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
     {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
     {&__pyx_n_s_Enum, __pyx_k_Enum, sizeof(__pyx_k_Enum), 0, 0, 1, 1},
@@ -46215,15 +46471,15 @@
     {&__pyx_n_s_WARNING_PROMISC_NOTSUP, __pyx_k_WARNING_PROMISC_NOTSUP, sizeof(__pyx_k_WARNING_PROMISC_NOTSUP), 0, 0, 1, 1},
     {&__pyx_n_s_WARNING_TSTAMP_TYPE_NOTSUP, __pyx_k_WARNING_TSTAMP_TYPE_NOTSUP, sizeof(__pyx_k_WARNING_TSTAMP_TYPE_NOTSUP), 0, 0, 1, 1},
     {&__pyx_n_s_WIRELESS, __pyx_k_WIRELESS, sizeof(__pyx_k_WIRELESS), 0, 0, 1, 1},
     {&__pyx_n_s_Warning, __pyx_k_Warning, sizeof(__pyx_k_Warning), 0, 0, 1, 1},
     {&__pyx_n_s_Warning___init, __pyx_k_Warning___init, sizeof(__pyx_k_Warning___init), 0, 0, 1, 1},
     {&__pyx_kp_s_Warning_category_for_libpcap_wa, __pyx_k_Warning_category_for_libpcap_wa, sizeof(__pyx_k_Warning_category_for_libpcap_wa), 0, 0, 1, 0},
     {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
-    {&__pyx_n_s__158, __pyx_k__158, sizeof(__pyx_k__158), 0, 0, 1, 1},
+    {&__pyx_n_s__159, __pyx_k__159, sizeof(__pyx_k__159), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
     {&__pyx_kp_s__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 0, 1, 0},
     {&__pyx_kp_u__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 1, 0, 0},
     {&__pyx_kp_u__21, __pyx_k__21, sizeof(__pyx_k__21), 0, 1, 0, 0},
     {&__pyx_kp_s__22, __pyx_k__22, sizeof(__pyx_k__22), 0, 0, 1, 0},
     {&__pyx_kp_s__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 0, 1, 0},
     {&__pyx_kp_u__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 1, 0, 0},
@@ -46310,14 +46566,15 @@
     {&__pyx_n_s_exc_value, __pyx_k_exc_value, sizeof(__pyx_k_exc_value), 0, 0, 1, 1},
     {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
     {&__pyx_n_s_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 0, 1, 1},
     {&__pyx_n_s_filter_2, __pyx_k_filter_2, sizeof(__pyx_k_filter_2), 0, 0, 1, 1},
     {&__pyx_n_s_findalldevs, __pyx_k_findalldevs, sizeof(__pyx_k_findalldevs), 0, 0, 1, 1},
     {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
     {&__pyx_n_s_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 0, 1, 1},
+    {&__pyx_n_s_flush, __pyx_k_flush, sizeof(__pyx_k_flush), 0, 0, 1, 1},
     {&__pyx_n_s_fname, __pyx_k_fname, sizeof(__pyx_k_fname), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
     {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
     {&__pyx_n_s_fromtimestamp, __pyx_k_fromtimestamp, sizeof(__pyx_k_fromtimestamp), 0, 0, 1, 1},
     {&__pyx_n_s_fsdecode, __pyx_k_fsdecode, sizeof(__pyx_k_fsdecode), 0, 0, 1, 1},
     {&__pyx_n_s_fsencode, __pyx_k_fsencode, sizeof(__pyx_k_fsencode), 0, 0, 1, 1},
@@ -46490,24 +46747,24 @@
     {&__pyx_n_s_to_ms, __pyx_k_to_ms, sizeof(__pyx_k_to_ms), 0, 0, 1, 1},
     {&__pyx_n_s_ts, __pyx_k_ts, sizeof(__pyx_k_ts), 0, 0, 1, 1},
     {&__pyx_n_s_tstamp_precision, __pyx_k_tstamp_precision, sizeof(__pyx_k_tstamp_precision), 0, 0, 1, 1},
     {&__pyx_n_s_tstamp_type, __pyx_k_tstamp_type, sizeof(__pyx_k_tstamp_type), 0, 0, 1, 1},
     {&__pyx_n_s_tstamp_types, __pyx_k_tstamp_types, sizeof(__pyx_k_tstamp_types), 0, 0, 1, 1},
     {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
     {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
+    {&__pyx_n_s_tz, __pyx_k_tz, sizeof(__pyx_k_tz), 0, 0, 1, 1},
     {&__pyx_n_s_tzinfo, __pyx_k_tzinfo, sizeof(__pyx_k_tzinfo), 0, 0, 1, 1},
     {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
     {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
     {&__pyx_kp_u_unclosed_Dumper, __pyx_k_unclosed_Dumper, sizeof(__pyx_k_unclosed_Dumper), 0, 1, 0, 0},
     {&__pyx_kp_u_unclosed_Pcap, __pyx_k_unclosed_Pcap, sizeof(__pyx_k_unclosed_Pcap), 0, 1, 0, 0},
     {&__pyx_kp_u_unknown_type, __pyx_k_unknown_type, sizeof(__pyx_k_unknown_type), 0, 1, 0, 0},
     {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_utc, __pyx_k_utc, sizeof(__pyx_k_utc), 0, 0, 1, 1},
-    {&__pyx_n_s_utcfromtimestamp, __pyx_k_utcfromtimestamp, sizeof(__pyx_k_utcfromtimestamp), 0, 0, 1, 1},
     {&__pyx_n_s_version_info, __pyx_k_version_info, sizeof(__pyx_k_version_info), 0, 0, 1, 1},
     {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
     {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
     {&__pyx_n_s_win32, __pyx_k_win32, sizeof(__pyx_k_win32), 0, 0, 1, 1},
     {&__pyx_n_u_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 1, 0, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
@@ -47520,43 +47777,52 @@
  *         self._check_closed()
  */
   __pyx_codeobj__153 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__142, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cypcap__cypcap_pyx, __pyx_n_s_dump, 1277, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__153)) __PYX_ERR(0, 1277, __pyx_L1_error)
 
   /* "cypcap/_cypcap.pyx":1283
  *         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)
  * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         """Flush the packets to the capture file."""
+ *         self._check_closed()
+ */
+  __pyx_codeobj__154 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__89, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cypcap__cypcap_pyx, __pyx_n_s_flush, 1283, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__154)) __PYX_ERR(0, 1283, __pyx_L1_error)
+
+  /* "cypcap/_cypcap.pyx":1293
+ *         return result
+ * 
  *     def ftell(self) -> int:             # <<<<<<<<<<<<<<
  *         """Get the current file offset for a savefile being written."""
  *         self._check_closed()
  */
-  __pyx_codeobj__154 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__89, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cypcap__cypcap_pyx, __pyx_n_s_ftell, 1283, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__154)) __PYX_ERR(0, 1283, __pyx_L1_error)
+  __pyx_codeobj__155 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__89, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cypcap__cypcap_pyx, __pyx_n_s_ftell, 1293, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__155)) __PYX_ERR(0, 1293, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__155 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__155)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__156 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__156)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  */
-  __pyx_codeobj__156 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__156)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__157 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__157)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "cypcap/_cypcap.pyx":1294
+  /* "cypcap/_cypcap.pyx":1304
  * 
  * 
  * def lib_version() -> str:             # <<<<<<<<<<<<<<
  *     """Get the version information for libpcap."""
  *     return cpcap.pcap_lib_version().decode()
  */
-  __pyx_codeobj__157 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cypcap__cypcap_pyx, __pyx_n_s_lib_version, 1294, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__157)) __PYX_ERR(0, 1294, __pyx_L1_error)
+  __pyx_codeobj__158 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cypcap__cypcap_pyx, __pyx_n_s_lib_version, 1304, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__158)) __PYX_ERR(0, 1304, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -47951,31 +48217,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_3(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_3); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_3(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_3); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -48191,30 +48457,28 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_cypcap", __pyx_methods, __pyx_k_This_module_is_a_Cython_based_b, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _cypcap pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_cypcap" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
@@ -48945,20 +49209,20 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_ImportFrom(__pyx_t_7, __pyx_n_s_Callable); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Callable, __pyx_t_4) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "cypcap/npcap.pxi":45
+  /* "cypcap/npcap.pxi":51
  * 
  * 
  * load_npcap_dlls()             # <<<<<<<<<<<<<<
  */
-  __pyx_t_9 = load_npcap_dlls(); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(6, 45, __pyx_L1_error)
+  __pyx_t_9 = load_npcap_dlls(); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(6, 51, __pyx_L1_error)
 
   /* "cypcap/_cypcap.pyx":29
  * 
  * # TODO This is a really big enumeration, add more values as requested
  * class DatalinkType(enum.IntEnum):             # <<<<<<<<<<<<<<
  *     """Datalink types."""
  *     NULL_ = cpcap.DLT_NULL
@@ -51629,65 +51893,78 @@
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_6cypcap_7_cypcap_Dumper, __pyx_n_s_dump, __pyx_t_7) < 0) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   PyType_Modified(__pyx_ptype_6cypcap_7_cypcap_Dumper);
 
   /* "cypcap/_cypcap.pyx":1283
  *         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)
  * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         """Flush the packets to the capture file."""
+ *         self._check_closed()
+ */
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_13flush, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper_flush, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__154)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1283, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_6cypcap_7_cypcap_Dumper, __pyx_n_s_flush, __pyx_t_7) < 0) __PYX_ERR(0, 1283, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  PyType_Modified(__pyx_ptype_6cypcap_7_cypcap_Dumper);
+
+  /* "cypcap/_cypcap.pyx":1293
+ *         return result
+ * 
  *     def ftell(self) -> int:             # <<<<<<<<<<<<<<
  *         """Get the current file offset for a savefile being written."""
  *         self._check_closed()
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1283, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 1283, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_13ftell, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper_ftell, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__154)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1283, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 1293, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_15ftell, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper_ftell, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__155)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_6cypcap_7_cypcap_Dumper, __pyx_n_s_ftell, __pyx_t_4) < 0) __PYX_ERR(0, 1283, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_6cypcap_7_cypcap_Dumper, __pyx_n_s_ftell, __pyx_t_4) < 0) __PYX_ERR(0, 1293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   PyType_Modified(__pyx_ptype_6cypcap_7_cypcap_Dumper);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_15__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper___reduce_cython, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__155)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper___reduce_cython, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__156)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.dumper cannot be converted to a Python object for pickling"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_17__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper___setstate_cython, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__156)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_6Dumper_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Dumper___setstate_cython, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__157)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_4) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cypcap/_cypcap.pyx":1294
+  /* "cypcap/_cypcap.pyx":1304
  * 
  * 
  * def lib_version() -> str:             # <<<<<<<<<<<<<<
  *     """Get the version information for libpcap."""
  *     return cpcap.pcap_lib_version().decode()
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1294, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 1294, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_15lib_version, 0, __pyx_n_s_lib_version, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__157)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1294, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 1304, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_6cypcap_7_cypcap_15lib_version, 0, __pyx_n_s_lib_version, NULL, __pyx_n_s_cypcap__cypcap, __pyx_d, ((PyObject *)__pyx_codeobj__158)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lib_version, __pyx_t_7) < 0) __PYX_ERR(0, 1294, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lib_version, __pyx_t_7) < 0) __PYX_ERR(0, 1304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "cypcap/_cypcap.pyx":1
  * # cython: language_level=3str, binding=True             # <<<<<<<<<<<<<<
  * """
  * This module is a Cython based binding for modern libpcap.
  */
@@ -51881,33 +52158,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -52115,20 +52399,38 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
+}
+#endif
 #endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
@@ -52214,15 +52516,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -52233,15 +52535,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -52265,15 +52567,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -52552,17 +52854,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -52631,16 +52939,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -52651,16 +52964,21 @@
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
     self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -52717,15 +53035,15 @@
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
     if (kwargs == NULL) {
         #if CYTHON_VECTORCALL
-        #if Py_VERSION_HEX < 0x03090000
+        #if PY_VERSION_HEX < 0x03090000
         vectorcallfunc f = _PyVectorcall_Function(func);
         #else
         vectorcallfunc f = PyVectorcall_Function(func);
         #endif
         if (f) {
             return f(func, args, (size_t)nargs, NULL);
         }
@@ -53042,15 +53360,15 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if PY_VERSION_HEX >= 0x030D0000
+            #if PY_VERSION_HEX >= 0x030d0000
             if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
             #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
@@ -53171,15 +53489,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -53206,15 +53524,17 @@
     }
     return NULL;
 }
 static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
     __Pyx_TypeName obj_type_name;
     if (likely(PyType_Check(obj))) {
         PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (meth) {
+        if (!meth) {
+            PyErr_Clear();
+        } else {
             PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
             Py_DECREF(meth);
             return result;
         }
     }
     obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
@@ -53315,36 +53635,43 @@
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
 /* GetAttr3 */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
     Py_INCREF(d);
     return d;
 }
+#endif
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r;
-#if CYTHON_USE_TYPE_SLOTS
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    int res = PyObject_GetOptionalAttr(o, n, &r);
+    return (res != 0) ? r : __Pyx_NewRef(d);
+#else
+  #if CYTHON_USE_TYPE_SLOTS
     if (likely(PyString_Check(n))) {
         r = __Pyx_PyObject_GetAttrStrNoError(o, n);
         if (unlikely(!r) && likely(!PyErr_Occurred())) {
             r = __Pyx_NewRef(d);
         }
         return r;
     }
-#endif
+  #endif
     r = PyObject_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+#endif
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -53374,15 +53701,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -54046,19 +54373,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_ass_item(o, i, v);
         }
     }
 #else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
+    if (is_list || !PyMapping_Check(o))
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
@@ -54115,14 +54438,15 @@
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* HasAttr */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
@@ -54131,14 +54455,15 @@
         PyErr_Clear();
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
+#endif
 
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
@@ -54193,15 +54518,17 @@
         Py_DECREF(s);
         return result;
     }
     #endif
     return __Pyx_PyObject_FormatAndDecref(s, f);
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f) {
-    PyObject *result = PyObject_Format(s, f);
+    PyObject *result;
+    if (unlikely(!s)) return NULL;
+    result = PyObject_Format(s, f);
     Py_DECREF(s);
     return result;
 }
 
 /* ModFloat[double] */
 static CYTHON_INLINE double __Pyx_mod_double(double a, double b) {
     double r = fmod(a, b);
@@ -54288,17 +54615,18 @@
   PyGILState_Release(_save);
   #endif
   return err;
 }
 
 /* UnpackUnboundCMethod */
 static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
     PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
     if (unlikely(!selfless_args)) return NULL;
-    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    result = PyObject_Call(method, selfless_args, kwargs);
     Py_DECREF(selfless_args);
     return result;
 }
 static PyMethodDef __Pyx_UnboundCMethod_Def = {
      "CythonUnboundCMethod",
      __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
      METH_VARARGS | METH_KEYWORDS,
@@ -54447,17 +54775,18 @@
         return PyUnicode_FromOrdinal(*dpos);
     }
     return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -54543,25 +54872,27 @@
         return NULL;
     }
     new_len = left_len + right_len;
     if (__Pyx_unicode_modifiable(left)
             && PyUnicode_CheckExact(right)
             && PyUnicode_KIND(right) <= PyUnicode_KIND(left)
             && !(PyUnicode_IS_ASCII(left) && !PyUnicode_IS_ASCII(right))) {
+        int ret;
         __Pyx_GIVEREF(*p_left);
-        if (unlikely(PyUnicode_Resize(p_left, new_len) != 0)) {
-            __Pyx_GOTREF(*p_left);
+        ret = PyUnicode_Resize(p_left, new_len);
+        __Pyx_GOTREF(*p_left);
+        if (unlikely(ret != 0))
             return NULL;
-        }
-        __Pyx_INCREF(*p_left);
-        #if PY_VERSION_HEX >= 0x030D0000
+        #if PY_VERSION_HEX >= 0x030d0000
         if (unlikely(PyUnicode_CopyCharacters(*p_left, left_len, right, 0, right_len) < 0)) return NULL;
         #else
         _PyUnicode_FastCopyCharacters(*p_left, left_len, right, 0, right_len);
         #endif
+        __Pyx_INCREF(*p_left);
+        __Pyx_GIVEREF(*p_left);
         return *p_left;
     } else {
         return __Pyx_PyUnicode_Concat(left, right);
     }
   }
 #endif
 
@@ -54707,20 +55038,160 @@
     }
     if (ulength == 1) {
         return PyUnicode_FromOrdinal(*dpos);
     }
     return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
 }
 
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod1 */
+#if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
+static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
+    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
+    Py_DECREF(method);
+    return result;
+}
+#endif
+static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
+#if CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2
+    PyObject *args[2] = {obj, arg};
+    (void) __Pyx_PyObject_GetMethod;
+    (void) __Pyx_PyObject_CallOneArg;
+    (void) __Pyx_PyObject_Call2Args;
+    return PyObject_VectorcallMethod(method_name, args, 2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
+#else
+    PyObject *method = NULL, *result;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_Call2Args(method, obj, arg);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) return NULL;
+    return __Pyx__PyObject_CallMethod1(method, arg);
+#endif
+}
+
 /* StringJoin */
-#if !CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
-    return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
-}
+    (void) __Pyx_PyObject_CallMethod1;
+#if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION < 3
+    return _PyString_Join(sep, values);
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000
+    return _PyBytes_Join(sep, values);
+#else
+    return __Pyx_PyObject_CallMethod1(sep, __pyx_n_s_join, values);
 #endif
+}
 
 /* PyObjectFormat */
 #if CYTHON_USE_UNICODE_WRITER
 static PyObject* __Pyx_PyObject_Format(PyObject* obj, PyObject* format_spec) {
     int ret;
     _PyUnicodeWriter writer;
     if (likely(PyFloat_CheckExact(obj))) {
@@ -55066,115 +55537,14 @@
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
     PyObject *arg[2] = {NULL, NULL};
     return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    __Pyx_TypeName type_name;
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
-        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
-#elif PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (likely(descr != NULL)) {
-        *method = descr;
-        return 0;
-    }
-    type_name = __Pyx_PyType_GetName(tp);
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
-                 type_name, name);
-#else
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
-                 type_name, PyString_AS_STRING(name));
-#endif
-    __Pyx_DECREF_TypeName(type_name);
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
-}
-
 /* PyObjectCallMethod0 */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
     PyObject *method = NULL, *result = NULL;
     int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
     if (likely(is_method)) {
         result = __Pyx_PyObject_CallOneArg(method, obj);
         Py_DECREF(method);
@@ -55228,46 +55598,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -55553,18 +55923,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_3
-#define __PYX_HAVE_RT_ImportType_3_0_3
-static PyTypeObject *__Pyx_ImportType_3_0_3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -55610,23 +55980,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -55752,18 +56122,15 @@
     }
     Py_INCREF((PyObject*) metaclass);
     return (PyObject*) metaclass;
 }
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -56739,15 +57106,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -56930,20 +57297,14 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
-/* PyObjectCall2Args */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args[3] = {NULL, arg1, arg2};
-    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
 /* Py3ClassCreate */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
                                            PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
     PyObject *ns;
     if (metaclass) {
         PyObject *prep = __Pyx_PyObject_GetAttrStrNoError(metaclass, __pyx_n_s_prepare);
         if (prep) {
@@ -57334,16 +57695,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -57355,14 +57716,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -57452,15 +57815,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -58610,38 +58973,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_pcap_direction_t(pcap_direction_t value) {
@@ -58672,38 +59037,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(pcap_direction_t),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(pcap_direction_t));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_bpf_u_int32(bpf_u_int32 value) {
@@ -58734,38 +59101,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(bpf_u_int32),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(bpf_u_int32));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
@@ -58933,15 +59302,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -59069,38 +59438,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned short),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned short));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE bpf_u_int32 __Pyx_PyInt_As_bpf_u_int32(PyObject *x) {
@@ -59268,15 +59639,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -59404,38 +59775,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
@@ -59466,38 +59839,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
@@ -59665,15 +60040,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -59980,38 +60355,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned char),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned char));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
@@ -60042,38 +60419,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE unsigned short __Pyx_PyInt_As_unsigned_short(PyObject *x) {
@@ -60241,15 +60620,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -60514,15 +60893,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -60650,38 +61029,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int64_t),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int64_t));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
@@ -60849,15 +61230,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -61122,15 +61503,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -61235,38 +61616,20 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__158);
+        name = __Pyx_NewRef(__pyx_n_s__159);
     }
     return name;
 }
 #endif
 
-/* PyObjectCallMethod1 */
-  static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
-    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
-    Py_DECREF(method);
-    return result;
-}
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
-    PyObject *method = NULL, *result;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_Call2Args(method, obj, arg);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) return NULL;
-    return __Pyx__PyObject_CallMethod1(method, arg);
-}
-
 /* CoroutineBase */
   #include <frameobject.h>
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
@@ -61544,17 +61907,30 @@
             assert(result == Py_None);
             PyErr_SetNone(PyExc_StopAsyncIteration);
         }
         else if (result == Py_None) {
             PyErr_SetNone(PyExc_StopIteration);
         }
         else {
+#if PY_VERSION_HEX < 0x030d00A1
             _PyGen_SetStopIterationValue(result);
+#else
+            if (!PyTuple_Check(result) && !PyExceptionInstance_Check(result)) {
+                PyErr_SetObject(PyExc_StopIteration, result);
+            } else {
+                PyObject *exc = __Pyx_PyObject_CallOneArg(PyExc_StopIteration, result);
+                if (likely(exc != NULL)) {
+                    PyErr_SetObject(PyExc_StopIteration, exc);
+                    Py_DECREF(exc);
+                }
+            }
+#endif
         }
-        Py_CLEAR(result);
+        Py_DECREF(result);
+        result = NULL;
     }
     return result;
 #endif
 }
 #endif
 static CYTHON_INLINE
 PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
@@ -62327,15 +62703,15 @@
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
-  static unsigned long __Pyx_get_runtime_version() {
+  static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
     unsigned long factor = 0x01000000UL;
     unsigned int digit = 0;
```

### Comparing `cypcap-0.5.0/cypcap/_cypcap.pyx` & `cypcap-0.6.0/cypcap/_cypcap.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -332,16 +332,16 @@
 
     @ts_datetime.setter
     def ts_datetime(self, ts_datetime: datetime):
         self.ts = ts_datetime.timestamp()
 
     @property
     def ts_utcdatetime(self) -> datetime:
-        """Timestamp as a naive UTC datetime."""
-        return datetime.utcfromtimestamp(self.ts)
+        """Timestamp as a UTC aware datetime."""
+        return datetime.fromtimestamp(self.ts, tz=timezone.utc)
 
     @ts_utcdatetime.setter
     def ts_utcdatetime(self, ts_utcdatetime: datetime):
         if ts_utcdatetime.tzinfo is None:
             ts_utcdatetime = ts_utcdatetime.replace(tzinfo=timezone.utc)
 
         self.ts = ts_utcdatetime.timestamp()
@@ -1276,14 +1276,24 @@
 
     def dump(self, Pkthdr pkt_header: Pkthdr, pkt_data) -> None:
         """Write a packet to a capture file."""
         self._check_closed()
 
         cpcap.pcap_dump(<unsigned char*>self.dumper, &pkt_header.pkthdr, pkt_data)
 
+    def flush(self):
+        """Flush the packets to the capture file."""
+        self._check_closed()
+
+        result = cpcap.pcap_dump_flush(self.dumper)
+        if result == cpcap.PCAP_ERROR:
+            raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
+
+        return result
+
     def ftell(self) -> int:
         """Get the current file offset for a savefile being written."""
         self._check_closed()
 
         result = cpcap.pcap_dump_ftell64(self.dumper)
         if result == cpcap.PCAP_ERROR:
             raise Error(result, cpcap.pcap_statustostr(<int>result).decode())
```

### Comparing `cypcap-0.5.0/cypcap/bpf.c` & `cypcap-0.6.0/cypcap/bpf.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.3 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "libraries": [
             "pcap"
         ],
@@ -30,23 +30,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_3" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030003F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -130,14 +130,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -191,14 +193,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -252,60 +256,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -388,14 +415,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -580,26 +610,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -612,15 +643,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -645,15 +675,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -731,16 +761,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -807,14 +842,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -882,27 +919,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -938,15 +975,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1082,14 +1119,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1160,15 +1206,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1265,32 +1311,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1332,15 +1361,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1573,29 +1602,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -1732,15 +1766,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -1944,15 +1978,15 @@
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
-static unsigned long __Pyx_get_runtime_version();
+static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 
@@ -4395,30 +4429,28 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("bpf", __pyx_methods, __pyx_k_BPF_Constants_and_utility_funct, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to bpf pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "bpf" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
@@ -5381,21 +5413,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
@@ -5454,15 +5504,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -5473,15 +5523,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -5505,15 +5555,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -5698,18 +5748,15 @@
 #endif
     return 0;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -6699,15 +6746,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -7019,33 +7066,40 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 #endif
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
@@ -7188,16 +7242,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -7209,14 +7263,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -7306,15 +7362,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -7410,38 +7466,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE unsigned short __Pyx_PyInt_As_unsigned_short(PyObject *x) {
@@ -7609,15 +7667,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -7745,38 +7803,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned short),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned short));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* FormatTypeName */
 #if CYTHON_COMPILING_IN_LIMITED_API
@@ -7823,38 +7883,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
@@ -8022,15 +8084,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -8295,15 +8357,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -8515,15 +8577,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-static unsigned long __Pyx_get_runtime_version() {
+static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
     unsigned long factor = 0x01000000UL;
     unsigned int digit = 0;
```

### Comparing `cypcap-0.5.0/cypcap/bpf.pyx` & `cypcap-0.6.0/cypcap/bpf.pyx`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/cypcap/cbpf.pxd` & `cypcap-0.6.0/cypcap/cbpf.pxd`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/cypcap/cpcap.pxd` & `cypcap-0.6.0/cypcap/cpcap.pxd`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/cypcap/npcap.pxi` & `cypcap-0.6.0/cypcap/npcap.pxi`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from . cimport cpcap
 
 cdef extern from *:
     """
     #ifdef _WIN32
     #include <Windows.h>
+    #include <delayimp.h>
     #include <stdio.h>
     #include <wchar.h>
     static int load_npcap_dlls(void)
     {
         WCHAR npcap_dir[512];
         UINT len;
         len = GetSystemDirectoryW(npcap_dir, 480);
@@ -18,15 +19,20 @@
 
         wcscat_s(npcap_dir, 512, L"\\\\Npcap");
         if (SetDllDirectoryW(npcap_dir) == 0) {
             PyErr_SetFromWindowsErr(0);
             return -1;
         }
 
-        pcap_lib_version();
+        __try {
+            pcap_lib_version();
+        } __except (GetExceptionCode() == VcppException(ERROR_SEVERITY_ERROR, ERROR_MOD_NOT_FOUND)) {
+            PyErr_SetString(PyExc_ImportError, "Failed to load Npcap (Is it installed?)");
+            return -1;
+        }
 
         if (SetDllDirectoryW(NULL) == 0) {
             PyErr_SetFromWindowsErr(0);
             return -1;
         }
 
         return 0;
```

### Comparing `cypcap-0.5.0/cypcap/sockaddr.c` & `cypcap-0.6.0/cypcap/sockaddr.c`

 * *Files identical despite different names*

### Comparing `cypcap-0.5.0/cypcap.egg-info/PKG-INFO` & `cypcap-0.6.0/cypcap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cypcap
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Cython based binding for modern libpcap
 Home-page: https://github.com/segevfiner/cypcap
 Author: Segev Finer
 Author-email: segev208@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://segevfiner.github.io/cypcap/
 Project-URL: Issue Tracker, https://github.com/segevfiner/cypcap/issues
```

### Comparing `cypcap-0.5.0/setup.py` & `cypcap-0.6.0/setup.py`

 * *Files identical despite different names*

