# Comparing `tmp/q1pulse-0.9.1.tar.gz` & `tmp/q1pulse-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1pulse-0.9.1.tar", last modified: Fri Jul 28 13:45:15 2023, max compression
+gzip compressed data, was "dist\q1pulse-0.9.2.tar", last modified: Mon Jul 31 11:39:07 2023, max compression
```

## Comparing `q1pulse-0.9.1.tar` & `q1pulse-0.9.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/
--rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.9.1/LICENSE
--rw-rw-rw-   0        0        0      193 2023-07-28 13:45:15.000000 q1pulse-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    14959 2023-07-24 12:53:33.000000 q1pulse-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/
--rw-rw-rw-   0        0        0      139 2023-07-28 13:45:07.000000 q1pulse-0.9.1/q1pulse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/assembler/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/assembler/__init__.py
--rw-rw-rw-   0        0        0    31856 2023-07-26 15:23:50.000000 q1pulse-0.9.1/q1pulse/assembler/generator.py
--rw-rw-rw-   0        0        0     1813 2023-07-11 13:10:59.000000 q1pulse-0.9.1/q1pulse/assembler/generator_data.py
--rw-rw-rw-   0        0        0    10258 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/assembler/instruction_queue.py
--rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.9.1/q1pulse/assembler/registers.py
--rw-rw-rw-   0        0        0    12183 2023-07-27 12:31:40.000000 q1pulse-0.9.1/q1pulse/instrument.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/lang/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/lang/__init__.py
--rw-rw-rw-   0        0        0      148 2023-07-20 15:51:39.000000 q1pulse-0.9.1/q1pulse/lang/base.py
--rw-rw-rw-   0        0        0     6677 2023-07-26 14:18:22.000000 q1pulse-0.9.1/q1pulse/lang/conditions.py
--rw-rw-rw-   0        0        0     1575 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/exceptions.py
--rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.9.1/q1pulse/lang/expression.py
--rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.9.1/q1pulse/lang/flow_statements.py
--rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.9.1/q1pulse/lang/generator.py
--rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.9.1/q1pulse/lang/loops.py
--rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.9.1/q1pulse/lang/math_expressions.py
--rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.9.1/q1pulse/lang/register.py
--rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.9.1/q1pulse/lang/register_statements.py
--rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.9.1/q1pulse/lang/registers.py
--rw-rw-rw-   0        0        0     2682 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/sequence.py
--rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.9.1/q1pulse/lang/simulator_statements.py
--rw-rw-rw-   0        0        0     4697 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/timed_statements.py
--rw-rw-rw-   0        0        0     1014 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/timeline.py
--rw-rw-rw-   0        0        0      431 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/triggers.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/modules/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/modules/__init__.py
--rw-rw-rw-   0        0        0     9514 2023-07-27 12:32:31.000000 q1pulse-0.9.1/q1pulse/modules/modules.py
--rw-rw-rw-   0        0        0     3028 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/modules/sequencer_states.py
--rw-rw-rw-   0        0        0     7011 2023-07-27 12:36:42.000000 q1pulse-0.9.1/q1pulse/program.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/sequencer/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/sequencer/__init__.py
--rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.9.1/q1pulse/sequencer/builderbase.py
--rw-rw-rw-   0        0        0    14380 2023-07-28 13:37:14.000000 q1pulse-0.9.1/q1pulse/sequencer/control.py
--rw-rw-rw-   0        0        0     6414 2023-07-27 12:37:02.000000 q1pulse-0.9.1/q1pulse/sequencer/readout.py
--rw-rw-rw-   0        0        0    12984 2023-07-27 13:36:41.000000 q1pulse-0.9.1/q1pulse/sequencer/sequencer.py
--rw-rw-rw-   0        0        0     3395 2023-07-11 15:30:18.000000 q1pulse-0.9.1/q1pulse/sequencer/sequencer_data.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/util/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/util/__init__.py
--rw-rw-rw-   0        0        0      690 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/util/qblox_version.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse.egg-info/
--rw-rw-rw-   0        0        0      193 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-28 13:45:15.000000 q1pulse-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-07-28 13:45:07.000000 q1pulse-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/
+-rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-07-31 11:39:07.000000 q1pulse-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14959 2023-07-24 12:53:33.000000 q1pulse-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse/
+-rw-rw-rw-   0        0        0      139 2023-07-31 11:38:46.000000 q1pulse-0.9.2/q1pulse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse/assembler/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.2/q1pulse/assembler/__init__.py
+-rw-rw-rw-   0        0        0    32490 2023-07-30 15:01:53.000000 q1pulse-0.9.2/q1pulse/assembler/generator.py
+-rw-rw-rw-   0        0        0     1911 2023-07-30 15:01:53.000000 q1pulse-0.9.2/q1pulse/assembler/generator_data.py
+-rw-rw-rw-   0        0        0     9973 2023-07-30 15:01:53.000000 q1pulse-0.9.2/q1pulse/assembler/instruction_queue.py
+-rw-rw-rw-   0        0        0     2649 2023-07-30 15:01:53.000000 q1pulse-0.9.2/q1pulse/assembler/registers.py
+-rw-rw-rw-   0        0        0     3362 2023-07-29 12:35:59.000000 q1pulse-0.9.2/q1pulse/assembler/registers_orig.py
+-rw-rw-rw-   0        0        0    12183 2023-07-27 12:31:40.000000 q1pulse-0.9.2/q1pulse/instrument.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse/lang/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.2/q1pulse/lang/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-07-20 15:51:39.000000 q1pulse-0.9.2/q1pulse/lang/base.py
+-rw-rw-rw-   0        0        0     6677 2023-07-26 14:18:22.000000 q1pulse-0.9.2/q1pulse/lang/conditions.py
+-rw-rw-rw-   0        0        0     1575 2023-07-24 12:53:33.000000 q1pulse-0.9.2/q1pulse/lang/exceptions.py
+-rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.9.2/q1pulse/lang/expression.py
+-rw-rw-rw-   0        0        0     3640 2023-07-29 18:20:56.000000 q1pulse-0.9.2/q1pulse/lang/flow_statements.py
+-rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.9.2/q1pulse/lang/generator.py
+-rw-rw-rw-   0        0        0     3559 2023-07-29 18:09:04.000000 q1pulse-0.9.2/q1pulse/lang/loops.py
+-rw-rw-rw-   0        0        0     8055 2023-07-29 16:28:27.000000 q1pulse-0.9.2/q1pulse/lang/math_expressions.py
+-rw-rw-rw-   0        0        0      690 2023-07-30 12:32:20.000000 q1pulse-0.9.2/q1pulse/lang/register.py
+-rw-rw-rw-   0        0        0     1011 2023-07-30 12:32:55.000000 q1pulse-0.9.2/q1pulse/lang/register_statements.py
+-rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.9.2/q1pulse/lang/registers.py
+-rw-rw-rw-   0        0        0     2682 2023-07-30 10:55:23.000000 q1pulse-0.9.2/q1pulse/lang/sequence.py
+-rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.9.2/q1pulse/lang/simulator_statements.py
+-rw-rw-rw-   0        0        0     4697 2023-07-30 10:55:19.000000 q1pulse-0.9.2/q1pulse/lang/timed_statements.py
+-rw-rw-rw-   0        0        0     1014 2023-07-24 12:53:33.000000 q1pulse-0.9.2/q1pulse/lang/timeline.py
+-rw-rw-rw-   0        0        0      431 2023-07-24 12:53:33.000000 q1pulse-0.9.2/q1pulse/lang/triggers.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse/modules/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.2/q1pulse/modules/__init__.py
+-rw-rw-rw-   0        0        0     9514 2023-07-27 12:32:31.000000 q1pulse-0.9.2/q1pulse/modules/modules.py
+-rw-rw-rw-   0        0        0     3028 2023-07-24 12:53:33.000000 q1pulse-0.9.2/q1pulse/modules/sequencer_states.py
+-rw-rw-rw-   0        0        0     7531 2023-07-30 15:01:53.000000 q1pulse-0.9.2/q1pulse/program.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse/sequencer/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.2/q1pulse/sequencer/__init__.py
+-rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.9.2/q1pulse/sequencer/builderbase.py
+-rw-rw-rw-   0        0        0    14860 2023-07-30 10:12:33.000000 q1pulse-0.9.2/q1pulse/sequencer/control.py
+-rw-rw-rw-   0        0        0     6414 2023-07-28 13:45:37.000000 q1pulse-0.9.2/q1pulse/sequencer/readout.py
+-rw-rw-rw-   0        0        0    13057 2023-07-29 17:05:17.000000 q1pulse-0.9.2/q1pulse/sequencer/sequencer.py
+-rw-rw-rw-   0        0        0     3395 2023-07-29 10:05:08.000000 q1pulse-0.9.2/q1pulse/sequencer/sequencer_data.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse/util/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.2/q1pulse/util/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-07-24 12:53:33.000000 q1pulse-0.9.2/q1pulse/util/qblox_version.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:39:07.000000 q1pulse-0.9.2/q1pulse.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-31 11:39:06.000000 q1pulse-0.9.2/q1pulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1260 2023-07-31 11:39:06.000000 q1pulse-0.9.2/q1pulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:39:06.000000 q1pulse-0.9.2/q1pulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-31 11:39:06.000000 q1pulse-0.9.2/q1pulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 11:39:06.000000 q1pulse-0.9.2/q1pulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-31 11:39:07.000000 q1pulse-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      310 2023-07-31 11:38:46.000000 q1pulse-0.9.2/setup.py
```

### Comparing `q1pulse-0.9.1/LICENSE` & `q1pulse-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/README.md` & `q1pulse-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/assembler/generator.py` & `q1pulse-0.9.2/q1pulse/assembler/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import math
 from functools import wraps
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from typing import List
 
 from .generator_data import GeneratorData
-from .instruction_queue import InstructionQueue, Instruction
+from .instruction_queue import InstructionQueue, Instruction, PendingUpdate
 from .registers import SequencerRegisters
 from ..lang.math_expressions import get_dtype, Expression, Operand
 from ..lang.generator import GeneratorBase
 from ..lang.register import Register
 from ..lang.exceptions import (
         Q1ValueError, Q1TypeError,
         Q1Exception, Q1CompileError
@@ -41,86 +41,104 @@
 
 
 def register_args(signature):
     '''
         Signature:
         I: integer only; Evaluate expression, allow label.
         f: float or int: Evaluate expression, if one float, then all float; label counts as int
-        F: float only: Evaluate expressoin, convert to i16
-        t: time. No register. No conversion.
+        F: float only: Evaluate expression, convert to i16
+        t: time. integer, No register. No conversion.
         o: object. No register. No conversion.
     '''
+    def arg_I(generator, i, arg, conversion_comments):
+        # translate reg, expr. to asm register
+        if isinstance(arg, Operand):
+            if arg.dtype != int:
+                raise Q1TypeError(f'Argument {i} must be of type int ({arg})')
+            asm_reg = generator._to_asm_reg(arg)
+            if conversion_comments is not None:
+                conversion_comments += [f'{arg} -> {asm_reg}']
+            return asm_reg
+        elif isinstance(arg, str):
+            # label or 'Rxx'
+            return arg
+        else:
+            # make unsigned
+            return _int_u32(arg)
+
+    def arg_f(generator, i, arg, conversion_comments):
+        # Note: label has dtype int
+#        dtype = get_dtype(arg)
+        # check optional all float or all int
+#        if opt_type is None:
+#            opt_type = dtype
+#        elif dtype is not None and dtype != opt_type:
+#            raise Q1TypeError(f'Float/int argument mismatch {dtype}<>{opt_type}')
+
+        if isinstance(arg,str):
+            # label or 'Rxx'
+            return arg
+        elif isinstance(arg, Operand):
+            asm_reg = generator._to_asm_reg(arg)
+            if conversion_comments is not None:
+                conversion_comments += [f'{arg} -> {asm_reg}']
+            return asm_reg
+        elif get_dtype(arg) == float:
+            value = _float_to_f32(arg)
+            if conversion_comments is not None:
+                conversion_comments += [f'{arg} -> {asm_reg}']
+            return value
+        else:
+            # make unsigned
+            return _int_u32(arg)
+
+    def arg_F(generator, i, arg, conversion_comments):
+        if arg is None:
+            return arg
+        elif isinstance(arg, Operand):
+            if arg.dtype != float:
+                raise Q1TypeError(f'Argument {i} must be of type float ({arg})')
+            asm_reg = generator._oper_to_f16(arg)
+            if conversion_comments is not None:
+                conversion_comments += [f'{arg} -> {asm_reg}']
+            return asm_reg
+        else:
+            value = _float_to_f16(arg)
+            if conversion_comments is not None:
+                conversion_comments += [f'{arg} -> {value}']
+            return value
+
+    arg_conv = []
+    for i,atype in enumerate(signature):
+        if atype in 'to':
+            # argument is time or object. Nothing to translate
+            continue
+        elif atype == 'I':
+            arg_conv.append((i, arg_I))
+        elif atype == 'f':
+            arg_conv.append((i, arg_f))
+        elif atype == 'F':
+            arg_conv.append((i, arg_F))
+
+
     def decorator_register_args(func):
         @wraps(func)
         def func_wrapper(self, *args, **kwargs):
             try:
                 # print(f'{func.__name__} {args}')
                 args = list(args)
                 self._registers.enter_scope()
-                comments = []
-                opt_type = None
-                for i,(arg,atype) in enumerate(zip(args,signature)): # @@@ optimize: atype to index?
-                    converted = False
-                    if atype in 'to':
-                        # argument is time or object. Nothing to translate
-                        continue
-                    elif atype == 'I':
-                        # translate reg, expr. to asm register
-                        if isinstance(arg, Operand):
-                            if arg.dtype != int:
-                                raise Q1TypeError(f'Argument {i} must be of type int ({args[i]})')
-                            asm_reg = self._to_asm_reg(arg)
-                            args[i] = asm_reg
-                            converted = True
-                        elif isinstance(arg,str):
-                            # label or 'Rxx'
-                            pass
-                        else:
-                            # make unsigned
-                            args[i] = _int_u32(arg)
-                    elif atype == 'f':
-                        # Note: label has dtype int
-                        dtype = get_dtype(arg)
-                        # check optional all float or all int
-                        if opt_type is None:
-                            opt_type = dtype
-                        elif dtype is not None and dtype != opt_type:
-                            raise Q1TypeError(f'Float/int argument mismatch {dtype}<>{opt_type}')
-                        if isinstance(arg, Operand):
-                            asm_reg = self._to_asm_reg(arg)
-                            args[i] = asm_reg
-                            converted = True
-                        elif dtype == float:
-                            args[i] = _float_to_f32(arg)
-                            converted = True
-                        elif isinstance(arg,str):
-                            # label or 'Rxx'
-                            pass
-                        else:
-                            # make unsigned
-                            args[i] = _int_u32(arg)
-                    elif atype == 'F':
-                        if arg is None:
-                            pass
-                        elif isinstance(arg, Operand):
-                            if arg.dtype != float:
-                                raise Q1TypeError(f'Argument {i} must be of type float ({args[i]})')
-                            asm_reg = self._to_asm_reg(arg)
-                            asm_reg = self._reg_to_f16(asm_reg)
-                            args[i] = asm_reg
-                            converted = True
-                        else:
-                            args[i] = _float_to_f16(arg)
-                            converted = True
 
-                    if self._show_arg_conversions and converted:
-                        comments += [f'{arg} -> {args[i]}']
+                conversion_comments = [] if self._show_arg_conversions else None
+                for i,conv_func in arg_conv:
+                    arg = args[i]
+                    args[i] = conv_func(self, i, arg, conversion_comments)
 
-                if self._show_arg_conversions and len(comments) > 0:
-                    self.add_comment(' -- args: ' + ', '.join(comments))
+                if self._show_arg_conversions and len(conversion_comments) > 0:
+                    self.add_comment(' -- args: ' + ', '.join(conversion_comments))
                 res = func(self, *args, **kwargs)
                 self._registers.exit_scope()
                 return res
             except Q1Exception as ex:
                 msg = f'in call\n    {func.__name__}({",".join(str(arg) for arg in args)})'
                 raise Q1CompileError(msg) from ex
 
@@ -133,33 +151,47 @@
 class ConditionalBlockState:
     rt_time_start: int = 0
     n_rt_instruction_start: int = 0
     last_rt_instructions: List[Instruction] = field(default_factory=list)
     rt_end_times: List[int] = field(default_factory=list)
 
 
+@dataclass
+class LastRtSettings:
+    awg_offs_time: int = -1
+    awg_offs_instr: Instruction = None
+    awg_gain_time: int = -1
+    awg_gain_instr: Instruction = None
+
+    def clear(self):
+        self.awg_gain_time = -1
+        self.awg_offs_time = -1
+
+
 class Q1asmGenerator(InstructionQueue, GeneratorBase):
     def __init__(self, add_comments=False, list_registers=True,
                  line_numbers=True, comment_arg_conversions=False,
                  optimize=1):
         super().__init__(add_comments=add_comments)
         self._list_registers = list_registers
         self._line_numbers = line_numbers
         self._show_arg_conversions = comment_arg_conversions
         self._optimize = optimize
         self.q1asm = None
         self._repetitions = 1
-        self._last_rt_settings = {}
+        self._last_rt_settings = LastRtSettings()
         self._conditional_block_state = None
         self._data = GeneratorData()
         self._registers = SequencerRegisters(self._add_reg_comment if add_comments else None)
         # counter for signed ASR emulation
         self._asr_jumps = 0
         self.modifies_frequency = False
         self.add_comment('--INIT--', init_section=True)
+        self._zero_reg = self.allocate_reg('_zero')
+        self.move(0, self._zero_reg, init_section=True)
 
 
     @property
     def repetitions(self):
         return self._repetitions
 
     @repetitions.setter
@@ -178,39 +210,36 @@
 
         if self._repetitions > 1:
             self.repetitions_reg = self.allocate_reg('_repetitions')
             self.move(self._repetitions, self.repetitions_reg,
                       init_section=True)
 
     def end_main(self, time):
-        if self._finalized:
-            return
         self._wait_till(time)
         self.block_end()
         self.add_comment('--END--')
         if self._repetitions > 1:
             self.loop(self.repetitions_reg, '@_start')
             # Last start/stop to ensure that pending update is set at end of program
             self.block_start()
             self.block_end()
         self._flush_pending_update()
         self._add_instruction('stop')
-        self._finalized = True
 
     def block_start(self):
         # Pending updates of the previous block must be updated now.
         # So, updates scheduled at the end of the loop will be updated
         # at the start of the loop or immediately after the loop.
         self._schedule_update(self._rt_time)
         # rt_settings may not be overwritten across block boundary
-        self._last_rt_settings = {}
+        self._last_rt_settings.clear()
 
     def block_end(self):
         # NOTE pending update will move to next block start.
-        self._last_rt_settings = {}
+        self._last_rt_settings.clear()
 
     def enter_conditional(self, time):
         self._flush_pending_update()
         self._wait_till(time)
         self.add_comment('Start conditional block')
         self._conditional_block_state = ConditionalBlockState()
 
@@ -219,15 +248,15 @@
         self._add_instruction('set_cond', 1, mask, operator, 4)
         # Store rt state at start to set the time after the block.
         self._conditional_block_state.n_rt_instruction_start = self._n_rt_instructions
         self._conditional_block_state.rt_time_start = self._rt_time
 
     def exit_condition(self):
         self._flush_pending_update()
-        self._last_rt_settings = {}
+        self._last_rt_settings.clear()
         cbs = self._conditional_block_state
         # add wait command if there is no pending rt command with wait_after time
         if self._last_rt_command is None:
             self._add_rt_command('wait', time=self._rt_time)
         else_time = 4*(self._n_rt_instructions - cbs.n_rt_instruction_start)
         self.add_comment(f'End condition. total wait_else {else_time} ns (t_end={self._rt_time})')
         # update end times of previous branches with time spent in else-wait.
@@ -273,54 +302,54 @@
 
     @register_args(signature='II')
     def loop(self, register, label):
         self._add_instruction('loop', register, label)
 
     @register_args(signature='ff')
     def move(self, source, destination, init_section=False):
-        self._add_instruction('move', source, destination,
-                              init_section=init_section)
+        self._add_reg_instruction('move', source, destination,
+                                  init_section=init_section)
 
     @register_args(signature='fff')
     def add(self, lhs, rhs, destination):
         if isinstance(lhs, int):
             # swap arguments. 1st argument cannot be immediate value
             lhs,rhs = rhs,lhs
-        self._add_instruction('add', lhs, rhs, destination)
+        self._add_reg_instruction('add', lhs, rhs, destination)
 
     @register_args(signature='fff')
     def sub(self, lhs, rhs, destination):
         # q1asm has no instruction for sub imm,reg,reg. Use sub reg,reg,reg instead
         if isinstance(lhs, Number):
             with self._registers.temp_regs(1) as temp:
                 self.move(lhs, temp)
-                self._add_instruction('sub', temp, rhs, destination)
+                self._add_reg_instruction('sub', temp, rhs, destination)
         else:
-            self._add_instruction('sub', lhs, rhs, destination)
+            self._add_reg_instruction('sub', lhs, rhs, destination)
 
     @register_args(signature='fIf')
     def asl(self, lhs, rhs, destination):
         # q1asm has no instruction for asl imm,reg,reg. Use asl reg,reg,reg instead
         if isinstance(lhs, Number):
             with self._registers.temp_regs(1) as temp:
                 self.move(lhs, temp)
-                self._add_instruction('asl', temp, rhs, destination)
+                self._add_reg_instruction('asl', temp, rhs, destination)
         else:
-            self._add_instruction('asl', lhs, rhs, destination)
+            self._add_reg_instruction('asl', lhs, rhs, destination)
 
     @register_args(signature='fIf')
     def lsr(self, lhs, rhs, destination):
         # NOTE: q1asm asr is unsigned, so actually it is an logical shift right
         if isinstance(lhs, Number):
             # q1asm has no instruction for asr imm,reg,reg. Use asr reg,reg,reg instead
             with self._registers.temp_regs(1) as temp:
                 self.move(lhs, temp)
-                self._add_instruction('asr', temp, rhs, destination)
+                self._add_reg_instruction('asr', temp, rhs, destination)
         else:
-            self._add_instruction('asr', lhs, rhs, destination)
+            self._add_reg_instruction('asr', lhs, rhs, destination)
 
     @register_args(signature='fIf')
     def asr(self, lhs, rhs, destination):
         with self.scope():
             if isinstance(lhs, Number):
                 # q1asm has no instruction for asr imm,reg,reg. Use asr reg,reg,reg instead
                 temp = self.get_temp_reg()
@@ -334,94 +363,95 @@
                     # It is more efficient than the other emulation below.
                     label = f'asr_end{self._asr_jumps}'
                     self._asr_jumps += 1
                     sign = self.get_temp_reg()
                     # get sign of lhs
                     self.bits_and(lhs, 0x8000_0000, sign)
                     # actual ASR
-                    self._add_instruction('asr', lhs, rhs, destination)
+                    self._add_reg_instruction('asr', lhs, rhs, destination)
                     # add sign extension bits if negative (highest bit set)
                     self.jlt(sign, 0x8000_0000, '@'+label)
                     sign_extension = 0xFFFF_FFFF << (31-rhs)
                     sign_extension &= 0xFFFF_FFFF
                     self.bits_or(destination, sign_extension, destination)
                     self.set_label(label)
                 else:
                     # This emulation adds 6 instructions: AND, ASR, NOP, SUB, NOP, OR
                     sign = self.get_temp_reg()
                     sign_extension = self.get_temp_reg()
                     # get sign of lhs (highest bit)
                     self.bits_and(lhs, 0x8000_0000, sign)
                     # actual ASR
-                    self._add_instruction('asr', lhs, rhs, destination)
+                    self._add_reg_instruction('asr', lhs, rhs, destination)
                     # compute sign extension bits
                     self.lsr(sign, rhs, sign) # explicit unsigned shift
-                    zero = self.get_zero_reg()
+                    zero = self._zero_reg
                     self.sub(zero, sign, sign_extension)
                     self.bits_or(destination, sign_extension, destination)
             else:
-                self._add_instruction('asr', lhs, rhs, destination)
-
+                self._add_reg_instruction('asr', lhs, rhs, destination)
 
     @register_args(signature='II')
     def bits_not(self, source, destination):
-        self._add_instruction('not', source, destination)
+        self._add_reg_instruction('not', source, destination)
 
     @register_args(signature='III')
     def bits_and(self, lhs, rhs, destination):
         if isinstance(lhs, int):
             # swap arguments. 1st argument cannot be immediate value
             lhs,rhs = rhs,lhs
-        self._add_instruction('and', lhs, rhs, destination)
+        self._add_reg_instruction('and', lhs, rhs, destination)
 
     @register_args(signature='III')
     def bits_or(self, lhs, rhs, destination):
         if isinstance(lhs, int):
             # swap arguments. 1st argument cannot be immediate value
             lhs,rhs = rhs,lhs
-        self._add_instruction('or', lhs, rhs, destination)
+        self._add_reg_instruction('or', lhs, rhs, destination)
 
     @register_args(signature='III')
     def bits_xor(self, lhs, rhs, destination):
         if isinstance(lhs, int):
             # swap arguments. 1st argument cannot be immediate value
             lhs,rhs = rhs,lhs
-        self._add_instruction('xor', lhs, rhs, destination)
+        self._add_reg_instruction('xor', lhs, rhs, destination)
 
     @register_args(signature='tI')
     def set_mrk(self, time, value):
         self._add_rt_setting('set_mrk', value, time=time)
         self._contains_io_instr = True
 
     @register_args(signature='t')
     def reset_phase(self, time):
         self._add_rt_setting('reset_ph', time=time)
 
     @register_args(signature='tFF')
     def awg_offset(self, time, offset0, offset1):
         offset0, offset1 = self._both_reg_or_imm(offset0, offset1)
-        last = self._last_rt_settings.get('set_awg_offs')
-        if last is not None and last[0] == time:
+        last_rt_settings = self._last_rt_settings
+        if last_rt_settings.awg_offs_time == time:
             self.add_comment(f'-- Overwrites set_awg_offs at {time} --')
-            self._overwrite_rt_setting(last[1])
+            self._overwrite_rt_setting(last_rt_settings.awg_offs_instr)
         instr = self._add_rt_setting('set_awg_offs', offset0, offset1,
                                      time=time)
-        self._last_rt_settings['set_awg_offs'] = (time, instr)
+        last_rt_settings.awg_offs_time = time
+        last_rt_settings.awg_offs_instr = instr
         self._contains_io_instr = True
 
     @register_args(signature='tFF')
     def awg_gain(self, time, gain0, gain1):
         gain0, gain1 = self._both_reg_or_imm(gain0, gain1)
-        last = self._last_rt_settings.get('set_awg_gain')
-        if last is not None and last[0] == time:
+        last_rt_settings = self._last_rt_settings
+        if last_rt_settings.awg_gain_time == time:
             self.add_comment(f'-- Overwrites set_awg_gain at {time} --')
-            self._overwrite_rt_setting(last[1])
+            self._overwrite_rt_setting(last_rt_settings.awg_gain_instr)
         instr = self._add_rt_setting('set_awg_gain', gain0, gain1,
                                      time=time)
-        self._last_rt_settings['set_awg_gain'] = (time, instr)
+        last_rt_settings.awg_gain_time = time
+        last_rt_settings.awg_gain_instr = instr
 
 #    @register_args(signature='tI') -- handled in _convert_frequency()
     def set_freq(self, time, frequency):
         ifreq = self._convert_frequency(frequency)
         self._add_rt_setting('set_freq', ifreq, time=time)
         self.modifies_frequency = True
 
@@ -437,18 +467,20 @@
             iphase = self._convert_phase(delta, hires_regs)
             # @@@ accumulate phase shifts at same time
             self._add_rt_setting('set_ph_delta', iphase, time=time)
 
     @register_args(signature='tI')
     def wait_reg(self, time, register):
         # Note: wait_reg also effectively contains a block_end and block_start.
-        elapsed = self._wait_till(time, pending_update='flush', return_negative=True)
+        elapsed = self._wait_till(time,
+                                  pending_update=PendingUpdate.FLUSH,
+                                  return_negative=True)
         self._add_wait_reg(register, elapsed)
         # rt_settings may not be overwritten across wait_reg boundary
-        self._last_rt_settings = {}
+        self._last_rt_settings.clear()
 
 #    @register_args(signature='too') # -- effectively translates nothing
     def play(self, time, wave0, wave1):
         # if one of them is None, then play same wave as other.
         if wave0 is None:
             wave0 = wave1
         elif wave1 is None:
@@ -497,25 +529,19 @@
     @contextmanager
     def unsigned_registers(self):
         emulate_signed = self.emulate_signed
         self.emulate_signed = False
         yield
         self.emulate_signed = emulate_signed
 
-    def enter_scope(self):
-        self._registers.enter_scope()
-
-    def exit_scope(self):
-        self._registers.exit_scope()
-
     @contextmanager
     def scope(self):
-        self.enter_scope()
+        self._registers.enter_scope()
         yield
-        self.exit_scope()
+        self._registers.exit_scope()
 
     def get_temp_reg(self):
         ''' Allocates an assembler register for temporary use within scope. '''
         return self._registers.get_temp_reg()
 
     def temp_regs(self, n):
         return self._registers.temp_regs(n)
@@ -526,21 +552,22 @@
     def _add_reg_comment(self, comment):
         if self._list_registers:
             self._reg_comment = comment
 
     def _both_reg_or_imm(self, value1, value2):
         # Note: There is an older implementation with for loops that is
         #       much shorter, but this version is mucch faster.
+        # Not checked combination: None, None
         if value1 is None:
             if isinstance(value2, int):
                 res1 = 0
                 res2 = value2
             else:
                 # None,reg => reg,reg
-                res1 = self.get_zero_reg()
+                res1 = self._zero_reg
                 res2 = value2
         elif isinstance(value1, int):
             if value2 is None:
                 res1 = value1
                 res2 = 0
             elif isinstance(value2, int):
                 res1 = value1
@@ -552,51 +579,53 @@
                 res1 = temp
                 res2 = value2
         else:
             # value1 is reg
             if value2 is None:
                 # reg,None => reg,reg
                 res1 = value1
-                res2 = self.get_zero_reg()
+                res2 = self._zero_reg
             elif isinstance(value2, int):
                 # reg,imm => reg,reg
                 temp = self._registers.get_temp_reg()
                 self.move(value2, temp)
                 res1 = value1
                 res2 = temp
             else:
                 # reg,reg
                 res1 = value1
                 res2 = value2
         return res1,res2
 
-    def get_zero_reg(self):
-        asm_reg, init_reg = self._registers.get_zero_reg()
-        if init_reg:
-            self._add_instruction('move', 0, asm_reg, init_section=True)
-        return asm_reg
-
     def _to_asm_reg(self, operand):
         if isinstance(operand, Register):
             asm_reg = self._registers.get_asm_reg(operand.name)
         elif isinstance(operand, Expression):
             asm_reg = operand.evaluate(self)
         else:
             raise Q1TypeError(f'Illegal operand {operand}')
         return asm_reg
 
     def _translate_reg(self, value_or_reg):
         if isinstance(value_or_reg, Register):
             return self._registers.get_asm_reg(value_or_reg.name)
         return value_or_reg
 
-    def _reg_to_f16(self, reg):
-        temp_reg = self.get_temp_reg()
-        self._add_instruction('asr', reg, 16, temp_reg)
-        return temp_reg
+    def _oper_to_f16(self, operand):
+        if isinstance(operand, Register):
+            asm_reg = self._registers.get_asm_reg(operand.name)
+            temp_reg = self.get_temp_reg()
+            self._add_reg_instruction('asr', asm_reg, 16, temp_reg)
+            return temp_reg
+        elif isinstance(operand, Expression):
+            asm_reg = operand.evaluate(self)
+            self._add_reg_instruction('asr', asm_reg, 16, asm_reg)
+            return asm_reg
+        else:
+            raise Q1TypeError(f'Illegal operand {operand}')
 
     def _convert_frequency(self, frequency):
         if isinstance(frequency, Operand):
             dtype = get_dtype(frequency)
             if dtype is not int:
                 raise Exception(f'frequency must be an integer value')
             if isinstance(frequency, Expression):
```

### Comparing `q1pulse-0.9.1/q1pulse/assembler/generator_data.py` & `q1pulse-0.9.2/q1pulse/assembler/generator_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,25 @@
         self.weights = {}
         self.acquisitions = {}
 
     def translate_wave(self, wave):
         if not isinstance(wave, Wave):
             raise Q1TypeError(f'Unsupported type for wave: {wave}')
 
-        if wave.name not in self.waveforms:
-            self.waveforms[wave.name] = {
+        waveforms = self.waveforms
+        try:
+            entry = waveforms[wave.name]
+            return entry['index']
+        except KeyError:
+            index = len(waveforms)
+            waveforms[wave.name] = {
                     'data':list(wave.data),
-                    'index':len(self.waveforms)
+                    'index':index
                     }
-
-        return self.waveforms[wave.name]['index']
+            return index
 
     def translate_acquisition(self, acquisition):
         if not isinstance(acquisition, AcquisitionBins):
             raise Q1TypeError(f'Unsupported type for acquisition: {acquisition}')
 
         if acquisition.name not in self.acquisitions:
             self.acquisitions[acquisition.name] = {
```

### Comparing `q1pulse-0.9.1/q1pulse/assembler/instruction_queue.py` & `q1pulse-0.9.2/q1pulse/assembler/instruction_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 from ..lang.exceptions import (
-        Q1StateError,
         Q1InternalError,
         Q1TimingError
         )
 
 @dataclass
 class Instruction:
     mnemonic: str
@@ -14,44 +13,41 @@
     comment: Optional[str] = None
     label: Optional[str] = None
     wait_after: Optional[int] = None
     overwritten: bool = False
 
 @dataclass
 class PendingUpdate:
-    index: str
+    KEEP = 0
+    MERGE = 1
+    FLUSH = 2
+    index: int
     time: int
 
 
 RT_RESOLUTION = 4
 MAX_WAIT = (1<<16)-RT_RESOLUTION
 
 class InstructionQueue:
     _check_time_reg = True
     emulate_signed = True
 
     def __init__(self, add_comments=False):
-        super().__init__()
         self.add_comments = add_comments
         self._init_section = []
         self._instructions = []
         self._reg_comment = None
         self._wait_loop_cnt = 0
         self._rt_time = 0
         self._pending_update = None
         self._last_rt_command = None
         self._n_rt_instructions = 0
-        self._finalized = False
         self._updating_reg = None
 
     def add_comment(self, line, init_section=False):
-        if not self.add_comments:
-            return
-        if self._finalized:
-            raise Q1StateError('Sequence already finalized')
         if init_section:
             self._init_section.append(line)
         else:
             self._instructions.append(line)
 
     def set_label(self, label):
         '''
@@ -59,55 +55,54 @@
         '''
         self._instructions.append(Instruction(None, label=label))
 
     def adjust_time(self, duration):
         self._rt_time += duration
 
     def __append_instruction(self, instruction):
-        if self._finalized:
-            raise Q1StateError('Sequence already finalized')
-        self._wait_register_updates(instruction.mnemonic, instruction.args)
+        self._wait_register_updates(instruction)
         self._instructions.append(instruction)
 
-    def _add_instruction(self, mnemonic, *args, comment=None, init_section=False):
-        if self._finalized:
-            raise Q1StateError('Sequence already finalized')
+    def _add_reg_instruction(self, mnemonic, *args, init_section=False):
         if self._reg_comment:
-            comment = self._reg_comment if not comment else comment + ' ' + self._reg_comment
+            comment = self._reg_comment
             self._reg_comment = None
+        else:
+            comment = None
         instruction = Instruction(mnemonic, args, comment=comment)
         if init_section:
             self._init_section.append(instruction)
             return
         self.__append_instruction(instruction)
-        if mnemonic in ['move','not','add','sub','and','or','xor','asl','asr']:
-            self._updating_reg = args[-1]
+        self._updating_reg = args[-1]
+
+    def _add_instruction(self, mnemonic, *args, comment=None):
+        instruction = Instruction(mnemonic, args, comment=comment)
+        self.__append_instruction(instruction)
 
     def _add_rt_setting(self, mnemonic, *args, time=None):
         if self.add_comments:
             comment = f'@ {time}'
         else:
             comment = None
         instruction = Instruction(mnemonic, args, comment=comment)
         self.__append_instruction(instruction)
         self._schedule_update(time)
         return instruction
 
-    def _add_rt_command(self, mnemonic, *args, time=None, index=None, updating=False):
-        self._wait_till(time, pending_update='merge' if updating else 'flush')
+    def _add_rt_command(self, mnemonic, *args, time=None, updating=False):
+        self._wait_till(time,
+                        pending_update=PendingUpdate.MERGE if updating else PendingUpdate.FLUSH)
         wait_after = RT_RESOLUTION
         if self.add_comments:
             comment = f't={time}'
         else:
             comment = None
         instruction = Instruction(mnemonic, args, comment=comment, wait_after=wait_after)
-        if index is None:
-            self.__append_instruction(instruction)
-        else:
-            self._instructions.insert(index, instruction)
+        self.__append_instruction(instruction)
         self._last_rt_command = instruction
         self._n_rt_instructions += 1
         self._rt_time += wait_after
 
     def _overwrite_rt_setting(self, instruction):
         instruction.overwritten = True
         if self.add_comments:
@@ -121,77 +116,77 @@
 
     def _schedule_update(self, time):
         self._wait_till(time)
         # put new update immediately after rt_setting (but get index after previous pending has been added)
         index_update = len(self._instructions)
         self._pending_update = PendingUpdate(index_update, time)
 
-    def _wait_till(self, time, pending_update='keep', return_negative=False):
-        if (self._pending_update is not None
-            and time == self._pending_update.time):
-            if pending_update == 'keep':
-                return
-            elif pending_update == 'merge':
-                # merge pending update with RT command that follows
-                self._pending_update = None
-                self._last_rt_command = None
-                self._rt_time = time
-                return
-            elif pending_update != 'flush':
-                Q1InternalError(f'Unknown {pending_update}')
-        self._flush_pending_update()
+    def _wait_till(self, time, pending_update=PendingUpdate.KEEP, return_negative=False):
+        if self._pending_update is not None:
+            if time == self._pending_update.time:
+                if pending_update == PendingUpdate.KEEP:
+                    return
+                elif pending_update == PendingUpdate.MERGE:
+                    # merge pending update with RT command that follows
+                    self._pending_update = None
+                    self._last_rt_command = None
+                    self._rt_time = time
+                    return
+                elif pending_update != PendingUpdate.FLUSH:
+                    Q1InternalError(f'Unknown {pending_update}')
+            self._flush_pending_update()
         wait_time = time - self._rt_time
-        if wait_time < 0:
-            if return_negative:
-                # time will be compensated in register
-                self._rt_time = time
-                return -wait_time
-            raise Q1TimingError(f'Too short wait time of {wait_time} ns at t={self._rt_time}')
         if wait_time > 0:
-            if wait_time > 50000:
-                self.add_comment(f'wait {wait_time} (t={time})')
             if self._last_rt_command is not None:
                 if self._last_rt_command.wait_after + wait_time < MAX_WAIT:
                     self._last_rt_command.wait_after += wait_time
                 else:
                     rem_wait_time = wait_time - MAX_WAIT + self._last_rt_command.wait_after
                     self._last_rt_command.wait_after = MAX_WAIT
                     self.__add_wait_instruction(rem_wait_time)
             else:
                 self.__add_wait_instruction(wait_time)
+        elif wait_time < 0:
+            if return_negative:
+                # time will be compensated in register
+                self._rt_time = time
+                return -wait_time
+            raise Q1TimingError(f'Too short wait time of {wait_time} ns at t={self._rt_time}')
         self._last_rt_command = None
         self._rt_time = time
         return 0
 
     def _flush_pending_update(self):
         pending_update = self._pending_update
         if pending_update is not None:
             wait_after = RT_RESOLUTION
-            instruction = Instruction('upd_param',  wait_after=wait_after, comment=f't={pending_update.time}')
+            if self.add_comments:
+                comment = f't={pending_update.time}'
+            else:
+                comment = None
+            instruction = Instruction('upd_param',  wait_after=wait_after, comment=comment)
             self._instructions.insert(pending_update.index, instruction)
             self._n_rt_instructions += 1
             self._pending_update = None
             self._last_rt_command = instruction
             self._rt_time += wait_after
 
     def __add_wait_instruction(self, time):
-        if time < 0:
-            raise Q1InternalError(f'Illegal wait time {time}')
         if time < MAX_WAIT:
             self._add_instruction('wait', time)
             self._n_rt_instructions += 1
         else:
             n_max,rem_wait = divmod(time, MAX_WAIT)
             if n_max <= 2:
                 for _ in range(n_max):
                     self._add_instruction('wait', MAX_WAIT)
             else:
                 self._wait_loop_cnt += 1
                 with self.temp_regs(1) as wait_reg:
-                    self._add_instruction('move', n_max, wait_reg)
+                    self._add_reg_instruction('move', n_max, wait_reg)
                     label = f'wait{self._wait_loop_cnt}'
                     self.set_label(label)
                     self._add_instruction('wait', MAX_WAIT)
                     self._add_instruction('loop', wait_reg, '@'+label)
             self._n_rt_instructions += n_max
             if rem_wait > 0:
                 self._add_instruction('wait', rem_wait)
@@ -202,26 +197,26 @@
         if less_then_65us and elapsed == 0 and not self._check_time_reg:
             # single instruction for short simple wait
             self._add_instruction('wait', time_reg)
             return
 
         wait_reg = self.allocate_reg('_waittime')
         if elapsed > 0:
-            self._add_instruction('sub', time_reg, elapsed, wait_reg)
+            self._add_reg_instruction('sub', time_reg, elapsed, wait_reg)
         else:
-            self._add_instruction('move', time_reg, wait_reg)
+            self._add_reg_instruction('move', time_reg, wait_reg)
         self._wait_loop_cnt += 1
 
         if self._check_time_reg:
             self.add_comment('         --- check for negative wait time')
             continue_label = f'waitc{self._wait_loop_cnt}'
             if self.emulate_signed:
                 self.add_comment('         --- emulate signed wait time')
                 with self.temp_regs(1) as temp_reg:
-                    self._add_instruction('xor', wait_reg, 0x8000_0000, temp_reg)
+                    self._add_reg_instruction('xor', wait_reg, 0x8000_0000, temp_reg)
                     self._add_instruction('jge', temp_reg, 0x8000_0000 + RT_RESOLUTION, '@'+continue_label)
             else:
                 self._add_instruction('jge', wait_reg, RT_RESOLUTION, '@'+continue_label)
             self._add_instruction('illegal', comment='negative wait time')
             if less_then_65us:
                 self._add_instruction('jlt', wait_reg, MAX_WAIT, '@'+continue_label)
                 self._add_instruction('illegal', comment='larger than 65 us')
@@ -229,22 +224,23 @@
 
         if not less_then_65us:
             loop_label = f'wait{self._wait_loop_cnt}'
             end_label = f'endwait{self._wait_loop_cnt}'
             self._add_instruction('jlt', wait_reg, MAX_WAIT, '@'+end_label)
             self.set_label(loop_label)
             self._add_instruction('wait', MAX_WAIT-RT_RESOLUTION)
-            self._add_instruction('sub', wait_reg, MAX_WAIT-RT_RESOLUTION, wait_reg)
+            self._add_reg_instruction('sub', wait_reg, MAX_WAIT-RT_RESOLUTION, wait_reg)
             self._add_instruction('jge', wait_reg, MAX_WAIT, '@'+loop_label)
             self.set_label(end_label)
 
         self._add_instruction('wait', wait_reg)
 
-    def _wait_register_updates(self, mnemonic, args):
+    def _wait_register_updates(self, instruction):
         '''
         Inserts a NOP when one of the arguments is a register which
         has been modified by the previous instruction.
         Registers are modified by the arithmetic instructions.
         '''
-        if self._updating_reg is not None and self._updating_reg in args:
-            self._add_instruction('nop', comment=f' {mnemonic} wait for {self._updating_reg}')
+        if self._updating_reg is not None and self._updating_reg in instruction.args:
+            self._add_instruction('nop',
+                                  comment=f' {instruction.mnemonic} wait for {self._updating_reg}')
         self._updating_reg = None
```

### Comparing `q1pulse-0.9.1/q1pulse/assembler/registers.py` & `q1pulse-0.9.2/q1pulse/assembler/registers_orig.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/instrument.py` & `q1pulse-0.9.2/q1pulse/instrument.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/conditions.py` & `q1pulse-0.9.2/q1pulse/lang/conditions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/exceptions.py` & `q1pulse-0.9.2/q1pulse/lang/exceptions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/flow_statements.py` & `q1pulse-0.9.2/q1pulse/lang/flow_statements.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
     @property
     def sequence(self):
         return self._sequence
 
 
 def _assign_reg(generator, register, value, allocate=True):
-    statement = register.assign(value, allocate=allocate)
-    statement.write_instruction(generator)
+    if allocate:
+        generator.allocate_reg(register.name)
+    generator.move(value, register)
 
 def _increment_reg(generator, register, incr):
-    statement = register.assign(register + incr)
-    statement.write_instruction(generator)
+    generator.add(register, incr, register)
 
 class LoopStatement(BranchStatement):
     def __init__(self, time, sequence, loop):
         super().__init__(time, sequence, loop.label)
         self._loop = loop
 
     def __repr__(self):
```

### Comparing `q1pulse-0.9.1/q1pulse/lang/generator.py` & `q1pulse-0.9.2/q1pulse/lang/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/loops.py` & `q1pulse-0.9.2/q1pulse/lang/loops.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 raise Q1TypeError('Array values must all be same type')
         if dtype == float:
             literal_values = [value for value in values if isinstance(value, Number)]
             if max(literal_values) > 1.0 or min(literal_values) < -1.0:
                 raise Q1ValueError('value out of range [-1.0, 1.0]')
 
         self._table_label = f'_table{self._loop_number}'
-        self._data_ptr = Register(f'_ptr{self._loop_number}')
+        self._data_ptr = Register(f'_ptr{self._loop_number}', dtype=int)
 
     @property
     def loopvar(self):
         return self._loopvar
 
     def __repr__(self):
         return f'loop_array({self.values}):{self.loopvar}'
```

### Comparing `q1pulse-0.9.1/q1pulse/lang/math_expressions.py` & `q1pulse-0.9.2/q1pulse/lang/math_expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 
     def __sub__(self, rhs):
         return Subtraction(self, rhs)
 
     def __rsub__(self, lhs):
         return Subtraction(lhs, self)
 
+    def __neg__(self):
+        if self.dtype == int:
+            return Subtraction(0, self)
+        if self.dtype == float:
+            return Subtraction(0.0, self)
+        return NotImplemented
+
     def __lshift__(self, rhs):
         return Asl(self, rhs)
 
     def __rshift__(self, rhs):
         return Asr(self, rhs)
 
     def __and__(self, rhs):
```

### Comparing `q1pulse-0.9.1/q1pulse/lang/register.py` & `q1pulse-0.9.2/q1pulse/lang/register.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/register_statements.py` & `q1pulse-0.9.2/q1pulse/lang/register_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/registers.py` & `q1pulse-0.9.2/q1pulse/lang/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/sequence.py` & `q1pulse-0.9.2/q1pulse/lang/sequence.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/simulator_statements.py` & `q1pulse-0.9.2/q1pulse/lang/simulator_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/timed_statements.py` & `q1pulse-0.9.2/q1pulse/lang/timed_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/lang/timeline.py` & `q1pulse-0.9.2/q1pulse/lang/timeline.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/modules/modules.py` & `q1pulse-0.9.2/q1pulse/modules/modules.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/modules/sequencer_states.py` & `q1pulse-0.9.2/q1pulse/modules/sequencer_states.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/program.py` & `q1pulse-0.9.2/q1pulse/program.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
+import time
+import logging
 from contextlib import contextmanager
 from numbers import Number
 
 from .lang.conditions import CounterFlags
 from .lang.exceptions import Q1InternalError, Q1ValueError
 from .lang.triggers import TriggerCounter, Trigger
 from .lang.math_expressions import Expression
 from .lang.timeline import Timeline
 from .lang.registers import Registers
 from .lang.register import Register
 from .lang.register_statements import RegisterAssignment
 from .lang.loops import RangeLoop, LinspaceLoop, ArrayLoop
 from .assembler.generator import Q1asmGenerator
 
+logger = logging.getLogger(__name__)
 
 class Program:
     def __init__(self, path=None):
         self.sequence_builders = {}
         self.path = path if path is not None else os.path.join('q1','_prog')
         self.R = Registers(self, local=False)
         self.repetitions = 1
@@ -46,22 +49,32 @@
         return os.path.join(self.path, f'q1seq_{name}.json')
 
     def compile(self, annotate=False, add_comments=True,
                 listing=False, json=True, optimize=1):
         # store compiled sequences
         self._q1asm = {}
 
+        start_compile = time.perf_counter()
         for builder in self.sequence_builders.values():
             g = Q1asmGenerator(add_comments=add_comments,
                                optimize=optimize)
             g.repetitions = self.repetitions
+            start = time.perf_counter()
             builder.compile(g, annotate=annotate)
+            end = time.perf_counter()
+            d1 = (end-start)*1000
+            start = end
             filename = self.seq_filename(builder.name) if listing or json else None
             g.assemble(listing=listing, json_output=json, filename=filename)
             self._q1asm[builder.name] = g.q1asm
+            end = time.perf_counter()
+            d2 = (end-start)*1000
+            logger.debug(f'compile {builder.name} {d1:5.2f} {d2:5.2f}')
+        duration = time.perf_counter() - start_compile
+        logger.debug(f'Total compilation {duration*1000:5.2f}')
 
     def q1asm(self, name):
         return self._q1asm[name]
 
     def _add_statement(self, statement, init_section=False):
         if not isinstance(statement, RegisterAssignment):
             raise Q1InternalError(f'Illegal statement for program {statement}')
```

### Comparing `q1pulse-0.9.1/q1pulse/sequencer/control.py` & `q1pulse-0.9.2/q1pulse/sequencer/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,19 +312,28 @@
             raise Q1ValueError('No output paths enabled')
 
         if len(self._enabled_paths) == 1:
             path = self._enabled_paths[0]
             if arg1 is None:
                 return (arg0, None) if path == 0 else (None, arg0)
             else:
-                return (arg0, arg1) if path == 0 else (-arg1, arg0)
+                if path == 1:
+                    # NOTE:
+                    # if 1 path is enabled and 2 arguments are passed, then
+                    # IQ should be rotated over pi/2, i.e. multiplied with [[0,1],[-1,0]]
+                    # This rotation is applied to gain and offset.
+                    # The amplitude of the waveform is multiplied by the gain.
+                    # The waveforms only have to be swapped.
+                    if isinstance(arg1, Wave):
+                        return (arg1, arg0)
+                    else:
+                        return (-arg1, arg0)
+                return (arg0, arg1)
 
-        # channels could be swapped
-        args = (arg0, arg1)
-        return (args[i] for i in self._enabled_paths)
+        return (arg0, arg1)
 
     def _translate_wave(self, wave):
         if wave is None:
             return None
         if isinstance(wave, str):
             return self._waves[wave]
         if isinstance(wave, Wave):
```

### Comparing `q1pulse-0.9.1/q1pulse/sequencer/readout.py` & `q1pulse-0.9.2/q1pulse/sequencer/readout.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/sequencer/sequencer.py` & `q1pulse-0.9.2/q1pulse/sequencer/sequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,34 +41,36 @@
     '''
 
     def __init__(self, name):
         self.name = name
         self._local_loop_cnt = 0
         self.Rs = Registers(self, local=True)
         self._sequence_stack = []
+        self.sequence = None
         self._local_time = 0
         self._local_time_active = False
         self._compiled = False
         self._init_sequence = Sequence(None)
         self._last_timed_statement = None
         self._conditional_block = None
         self._in_condition = False
         self._trigger_counters = []
 
     def start_sequence(self, program, timeline):
         self._program = program
         self._timeline = timeline
-        self._start_sequence()
+        self._sequence_push(Sequence(self._timeline))
 
-    def _start_sequence(self):
-        self._sequence_stack.append(Sequence(self._timeline))
+    def _sequence_push(self, sequence):
+        self._sequence_stack.append(sequence)
+        self.sequence = sequence
 
-    @property
-    def sequence(self):
-        return self._sequence_stack[-1]
+    def _sequence_pop(self):
+        self._sequence_stack.pop()
+        self.sequence = self._sequence_stack[-1]
 
     def _add_statement(self, statement, init_section=False):
         self._check_time(statement)
         if SequenceBuilder.add_traceback_to_instructions and not isinstance(statement, str):
             self._add_traceback(statement)
         if self._compiled:
             raise Q1StateError('Program cannot be changed after compilation')
@@ -220,25 +222,25 @@
         if isinstance(loop, (RangeLoop, LinspaceLoop)):
             loop_statement = LoopStatement(self.end_time, loop_sequence, loop)
         elif isinstance(loop, ArrayLoop):
             loop_statement = ArrayLoopStatement(self.end_time, loop_sequence, loop)
         else:
             raise Q1InternalError('Unknown loop')
         self._add_statement(loop_statement)
-        self._sequence_stack.append(loop_sequence)
+        self._sequence_push(loop_sequence)
 
     def exit_loop(self, loop):
         if isinstance(loop, (RangeLoop, LinspaceLoop)):
             loop_end_statement = EndLoopStatement(self.end_time, loop)
         elif isinstance(loop, ArrayLoop):
             loop_end_statement = EndArrayLoopStatement(self.end_time, loop)
         else:
             raise Q1InternalError('Unknown loop')
         self._add_statement(loop_end_statement)
-        self._sequence_stack.pop()
+        self._sequence_pop()
 
     @contextmanager
     def _seq_repeat(self, n):
         ''' repeat loop not synchronizing with other sequencers. '''
         if n == 0:
             raise ValueError('n must be > 0')
         if n == 1:
@@ -246,23 +248,23 @@
         else:
             t_start = self.current_time
             loop = Loop(self._local_loop_cnt, n, local=True)
             self._local_loop_cnt += 1
             loop_sequence = Sequence(self._timeline)
             loop_statement = LoopStatement(self.current_time, loop_sequence, loop)
             self._add_statement(loop_statement)
-            self._sequence_stack.append(loop_sequence)
+            self._sequence_push(loop_sequence)
 
             yield
 
             loop_end_statement = EndLoopStatement(self.current_time, loop)
             self._add_statement(loop_end_statement)
             t_loop = self.current_time - t_start
             self._add_statement(LoopDurationStatement(n, t_loop))
-            self._sequence_stack.pop()
+            self._sequence_pop()
             self.set_pulse_end(t_start + n * t_loop)
 
     def _add_reg_wait(self, reg):
         self._add_statement(WaitRegStatement(self.end_time, reg))
 
     @property
     def trigger_counters(self):
@@ -321,19 +323,19 @@
             raise Q1SyntaxError('Conditions must be wrapped in `conditional` section.')
         if self._in_condition:
             raise Q1SyntaxError('Conditions cannot be nested')
         self._in_condition = True
         timeline = copy(self._timeline)
         branch = BranchSequence(timeline, operator)
         self._conditional_block.add_branch(branch)
-        self._sequence_stack.append(branch)
+        self._sequence_push(branch)
 
     def exit_condition(self, end_time=None):
         if end_time is None:
             end_time = self.end_time
         self.add_comment(f'Condition end time: {end_time}')
         self._conditional_block.set_end_time(end_time)
         self._in_condition = False
-        self._sequence_stack.pop()
+        self._sequence_pop()
         self._last_timed_statement = self._conditional_block
```

### Comparing `q1pulse-0.9.1/q1pulse/sequencer/sequencer_data.py` & `q1pulse-0.9.2/q1pulse/sequencer/sequencer_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse/util/qblox_version.py` & `q1pulse-0.9.2/q1pulse/util/qblox_version.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.9.1/q1pulse.egg-info/SOURCES.txt` & `q1pulse-0.9.2/q1pulse.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 q1pulse.egg-info/requires.txt
 q1pulse.egg-info/top_level.txt
 q1pulse/assembler/__init__.py
 q1pulse/assembler/generator.py
 q1pulse/assembler/generator_data.py
 q1pulse/assembler/instruction_queue.py
 q1pulse/assembler/registers.py
+q1pulse/assembler/registers_orig.py
 q1pulse/lang/__init__.py
 q1pulse/lang/base.py
 q1pulse/lang/conditions.py
 q1pulse/lang/exceptions.py
 q1pulse/lang/expression.py
 q1pulse/lang/flow_statements.py
 q1pulse/lang/generator.py
```

