# Comparing `tmp/pyscreeps_arena-0.2.2.tar.gz` & `tmp/pyscreeps_arena-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps_arena-0.2.2.tar", last modified: Wed Apr 17 11:04:17 2024, max compression
+gzip compressed data, was "pyscreeps_arena-0.2a0.tar", last modified: Sun Apr 14 14:14:55 2024, max compression
```

## Comparing `pyscreeps_arena-0.2.2.tar` & `pyscreeps_arena-0.2a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 11:04:17.580000 pyscreeps_arena-0.2.2/
--rw-rw-rw-   0        0        0    46966 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 11:04:17.590000 pyscreeps_arena-0.2.2/pyscreeps_arena/
--rw-rw-rw-   0        0        0      754 2024-04-03 11:07:12.000000 pyscreeps_arena-0.2.2/pyscreeps_arena/__init__.py
--rw-rw-rw-   0        0        0    25914 2024-04-16 17:08:46.000000 pyscreeps_arena-0.2.2/pyscreeps_arena/build.py
--rw-rw-rw-   0        0        0    49317 2024-04-17 11:02:54.000000 pyscreeps_arena-0.2.2/pyscreeps_arena/project.7z
-drwxrwxrwx   0        0        0        0 2024-04-17 11:04:17.600000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0    46966 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       87 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 11:04:18.000000 pyscreeps_arena-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1242 2024-04-17 11:04:06.000000 pyscreeps_arena-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:14:55.120000 pyscreeps_arena-0.2a0/
+-rw-rw-rw-   0        0        0    46966 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 14:14:55.120000 pyscreeps_arena-0.2a0/pyscreeps_arena/
+-rw-rw-rw-   0        0        0      754 2024-04-03 11:07:12.000000 pyscreeps_arena-0.2a0/pyscreeps_arena/__init__.py
+-rw-rw-rw-   0        0        0    25559 2024-04-14 00:04:48.000000 pyscreeps_arena-0.2a0/pyscreeps_arena/build.py
+-rw-rw-rw-   0        0        0    48972 2024-04-14 14:12:44.000000 pyscreeps_arena-0.2a0/pyscreeps_arena/project.7z
+drwxrwxrwx   0        0        0        0 2024-04-14 14:14:55.130000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0    46966 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       87 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 14:14:56.000000 pyscreeps_arena-0.2a0/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2024-04-14 14:14:44.000000 pyscreeps_arena-0.2a0/setup.py
```

### Comparing `pyscreeps_arena-0.2.2/PKG-INFO` & `pyscreeps_arena-0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.2.2
+Version: 0.2a0
 Summary: Python api|interface to play game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps_arena-0.2.2/pyscreeps_arena/__init__.py` & `pyscreeps_arena-0.2a0/pyscreeps_arena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscreeps_arena-0.2.2/pyscreeps_arena/build.py` & `pyscreeps_arena-0.2a0/pyscreeps_arena/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,15 @@
             print()  # 换行
 
         _pre_import_, _pre_imp_detail_ = [], {}  # import
         _pre_sort_ = {}  # sort
         _pre_define_ = {}  # define
         _js_replace_, _insert_id_ = {}, 0  # insert
 
+
         # ----------------------------------- IMPORT ----------------------------------- #
         # 获取所有.py文件中的所有import的内容，并记录下来fname:[imp1, imp2, ...]
         for i, fpath in enumerate(py_fpath):
             fname = py_names[i][:-3] + '.js'
             content = self.auto_read(fpath)
             for i, line in enumerate(content.split('\n')):
                 m = re.search(r'#\s*>\s*import\s+([^\n]+)', line)
@@ -236,28 +237,28 @@
                 if not re.search(r'#\s*>\s*remove', line):
                     new_content += line + '\n'
 
             with open(fpath, 'w', encoding='utf-8') as f:
                 f.write(new_content)
 
         # ------------------------------------ SORT ------------------------------------ #
-        # 获取所有.py文件中的所有# sort的内容，并记录下来(不存在则默认为2^32-1)
+        # 获取所有.py文件中的所有# sort的内容，并记录下来(不存在则默认为65535)
         for i, fpath in enumerate(py_fpath):
             fname = py_names[i][:-3] + '.js'
             content = self.auto_read(fpath)
             m = re.search(r'#\s*>\s*sort\s+(\d+)', content)
             if m:
                 try:
                     sort_num = int(m.group(1))
                 except ValueError:
-                    print(Fore.YELLOW + '[Warn] ' + Fore.RESET + f'sort number error: "{m.group(1)}", use 2^32-1 instead.')
-                    sort_num = 4294967295
+                    print(Fore.YELLOW + '[Warn] ' + Fore.RESET + f'sort number error: "{m.group(1)}", use 65535 instead.')
+                    sort_num = 65535
                 _pre_sort_[fname] = sort_num
             else:
-                _pre_sort_[fname] = 4294967295
+                _pre_sort_[fname] = 65535
 
         # ------------------------------------ DEFINE ------------------------------------ #
         # 扫描所有# define的内容，然后在.py中移除这些行，并记录下来
         for fpath in py_fpath:
             content = self.auto_read(fpath)
             new_content = ""
             for line in content.split('\n'):
@@ -466,29 +467,23 @@
 
         print(Fore.YELLOW + '>>> ' + Fore.RESET + 'generating total main.js ...', end='')
 
         # resort modules
         f_sorts[self.JS_VM] = -1
 
         err_flag = False
-        for i, module in enumerate(usr_modules):
+        for module in usr_modules:
             if module[2:] not in f_sorts:
-                if module[2:6] == 'src.' and module[6:] in f_sorts:
-                    f_sorts[module[2:]] = f_sorts[module[6:]]
-                    # 为了解决这样的问题:
-                    # > import src.creeps.basic
-                    # import src.creeps.basic
+                print(Fore.RED + '\n[Error] ' + Fore.RESET + f'"{module[2:-3]}.py" is not a user module.')
+                imp_detail = t_imps.get(module, None)
+                if imp_detail:
+                    print("\t\t-- May be imported by user in: %s" % imp_detail)
                 else:
-                    print(Fore.RED + '\n[Error] ' + Fore.RESET + f'"{module[2:-3]}.py" is not a user module.')
-                    imp_detail = t_imps.get(module, None)
-                    if imp_detail:
-                        print("\t\t-- May be imported by user in: %s" % imp_detail)
-                    else:
-                        print("\t\t-- Please move this file into the 'src' directory.")
-                    err_flag = True
+                    print("\t\t-- Please move this file into the 'src' directory.")
+                err_flag = True
         if err_flag:
             sys.exit(1)
         for i in range(len(usr_modules)):
             for j in range(i + 1, len(usr_modules)):
                 if f_sorts[usr_modules[i][2:]] > f_sorts[usr_modules[j][2:]]:
                     usr_modules[i], usr_modules[j] = usr_modules[j], usr_modules[i]
```

### Comparing `pyscreeps_arena-0.2.2/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps_arena-0.2a0/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.2.2
+Version: 0.2a0
 Summary: Python api|interface to play game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps_arena-0.2.2/setup.py` & `pyscreeps_arena-0.2a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from setuptools import setup, find_packages
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.2.2',
+    version='0.2.a0',
     description='Python api|interface to play game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
```

