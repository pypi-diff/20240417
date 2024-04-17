# Comparing `tmp/zlutils-0.1.6.tar.gz` & `tmp/zlutils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlutils-0.1.6.tar", last modified: Wed Apr 10 18:19:19 2024, max compression
+gzip compressed data, was "zlutils-0.2.0.tar", last modified: Wed Apr 17 02:52:17 2024, max compression
```

## Comparing `zlutils-0.1.6.tar` & `zlutils-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:19:19.739838 zlutils-0.1.6/
--rw-r--r--   0 zlols     (1000) zlols     (1000)      367 2024-04-10 18:19:19.739838 zlutils-0.1.6/PKG-INFO
--rw-r--r--   0 zlols     (1000) zlols     (1000)        2 2024-03-20 17:14:30.000000 zlutils-0.1.6/README.md
--rw-r--r--   0 zlols     (1000) zlols     (1000)       38 2024-04-10 18:19:19.739838 zlutils-0.1.6/setup.cfg
--rw-r--r--   0 zlols     (1000) zlols     (1000)      599 2024-04-10 14:52:27.000000 zlutils-0.1.6/setup.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:19:19.739838 zlutils-0.1.6/zlutils/
--rw-r--r--   0 zlols     (1000) zlols     (1000)       46 2024-04-10 10:31:55.000000 zlutils-0.1.6/zlutils/__init__.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1897 2024-04-10 15:07:09.000000 zlutils-0.1.6/zlutils/const.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1119 2024-04-10 15:09:05.000000 zlutils-0.1.6/zlutils/event.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     5258 2024-03-30 03:58:57.000000 zlutils-0.1.6/zlutils/shared.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)      371 2024-03-31 05:47:19.000000 zlutils-0.1.6/zlutils/wrapper.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:19:19.739838 zlutils-0.1.6/zlutils.egg-info/
--rw-r--r--   0 zlols     (1000) zlols     (1000)      367 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/PKG-INFO
--rw-r--r--   0 zlols     (1000) zlols     (1000)      233 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/SOURCES.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)        1 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/dependency_links.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)        8 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 02:52:17.380649 zlutils-0.2.0/
+-rw-rw-rw-   0        0        0      419 2024-04-17 02:52:17.380649 zlutils-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2024-04-16 12:11:00.000000 zlutils-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:52:17.381648 zlutils-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      623 2024-04-16 16:48:37.000000 zlutils-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:52:17.371226 zlutils-0.2.0/zlutils/
+-rw-rw-rw-   0        0        0       54 2024-04-16 16:49:13.000000 zlutils-0.2.0/zlutils/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-16 12:11:00.000000 zlutils-0.2.0/zlutils/const.py
+-rw-rw-rw-   0        0        0     1154 2024-04-16 12:11:00.000000 zlutils-0.2.0/zlutils/event.py
+-rw-rw-rw-   0        0        0     5415 2024-04-16 12:11:00.000000 zlutils-0.2.0/zlutils/shared.py
+-rw-rw-rw-   0        0        0     3135 2024-04-16 18:31:30.000000 zlutils-0.2.0/zlutils/view.py
+-rw-rw-rw-   0        0        0      384 2024-04-16 12:11:00.000000 zlutils-0.2.0/zlutils/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:52:17.379666 zlutils-0.2.0/zlutils.egg-info/
+-rw-rw-rw-   0        0        0      419 2024-04-17 02:52:17.000000 zlutils-0.2.0/zlutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-17 02:52:17.000000 zlutils-0.2.0/zlutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:52:17.000000 zlutils-0.2.0/zlutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 02:52:17.000000 zlutils-0.2.0/zlutils.egg-info/top_level.txt
```

### Comparing `zlutils-0.1.6/setup.py` & `zlutils-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import setuptools
-
-discription = "a package of utils"
-
-setuptools.setup(
-  name="zlutils",
-  version='0.1.6',
-  python_requires=">=3.6",
-  author="zlols",
-  author_email="zlols@foxmail.com",
-  description=discription,
-  long_description=discription,
-  long_description_content_type="text/markdown",
-  url="https://github.com/zlolss/zlutils.py.git",
-  py_modules=['zlutils'],
-  install_requires=[
-    ],
-  packages=setuptools.find_packages(),
-  classifiers=[
-  "Programming Language :: Python :: 3 :: Only",
-  "License :: OSI Approved :: MIT License",
-  #"Operating System :: OS Independent",
-  ],
-)
+import setuptools
+
+discription = "a package of utils"
+
+setuptools.setup(
+  name="zlutils",
+  version='0.2.0',
+  python_requires=">=3.6",
+  author="zlols",
+  author_email="zlols@foxmail.com",
+  description=discription,
+  long_description=discription,
+  long_description_content_type="text/markdown",
+  url="https://github.com/zlolss/zlutils.py.git",
+  py_modules=['zlutils'],
+  install_requires=[
+    ],
+  packages=setuptools.find_packages(),
+  classifiers=[
+  "Programming Language :: Python :: 3 :: Only",
+  "License :: OSI Approved :: MIT License",
+  #"Operating System :: OS Independent",
+  ],
+)
```

### Comparing `zlutils-0.1.6/zlutils/const.py` & `zlutils-0.2.0/zlutils/const.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-
-#  =============================================== 常量类
-class _常量类(type):
-    '''常量不能以下划线_开头'''
-
-    def __new__(元类, 类名, 所有基类, 类变量):
-        类变量[f'_{类名}__allconsts'] = [变量名 for 变量名 in 类变量.keys() if 变量名[:1]!='_']
-        return super().__new__(元类, 类名, 所有基类, 类变量)
-
-
-    def __setattr__(类, 变量名, 想要设置的值):
-        #if 变量名 not in vars(类):
-        raise RuntimeError('这是一只固态只因因此不能改变结构')
-        #try:
-        #    vars(类)[变量名].赋值(想要设置的值)
-        #except:
-        #    super().__setattr__(变量名, 想要设置的值)
-
-    def __iter__(类):
-        return super().__getattribute__(f'_{类.__name__}__allconsts').__iter__()
-
-
-class 常量类(metaclass=_常量类):
-
-    def __init__(我):
-        raise TypeError(f'{我.__class__.__name__}不允许实例化')
-
-
-# =============================================== 模式类
-class _模式类(_常量类):
-    '''
-应用样例:
-from zlutils.const import 模式类
-class m(模式类):
-    gtt = 0
-    add = 0
-
-print(m.gtt)
-输出:gtt
-
-'gtt' in m
-输出:True
-
-list(m)
-输出:['gtt', 'add']
-
-'''
-
-    def __contains__(类, 常量):
-        try:
-            super().__getattribute__(常量)
-            return True
-        except:
-            return False
-
-
-    def __getattribute__(类, 常量名):
-        取值 = super().__getattribute__(常量名)
-        if  '_' == 常量名[:1]:
-            return 取值
-        return str(常量名)
-
-
-class 模式类(metaclass=_模式类):
-    '''用于区分不同的模式'''
-    样例 = 0 # 等于号后的值不生效,可任意设置
-
-    def __init__(我):
-        raise TypeError(f'{我.__class__.__name__}不允许实例化')
-
-
-# =============================================== 字段类
-class 字段类:
-    pass
-
+
+#  =============================================== 常量类
+class _常量类(type):
+    '''常量不能以下划线_开头'''
+
+    def __new__(元类, 类名, 所有基类, 类变量):
+        类变量[f'_{类名}__allconsts'] = [变量名 for 变量名 in 类变量.keys() if 变量名[:1]!='_']
+        return super().__new__(元类, 类名, 所有基类, 类变量)
+
+
+    def __setattr__(类, 变量名, 想要设置的值):
+        #if 变量名 not in vars(类):
+        raise RuntimeError('这是一只固态只因因此不能改变结构')
+        #try:
+        #    vars(类)[变量名].赋值(想要设置的值)
+        #except:
+        #    super().__setattr__(变量名, 想要设置的值)
+
+    def __iter__(类):
+        return super().__getattribute__(f'_{类.__name__}__allconsts').__iter__()
+
+
+class 常量类(metaclass=_常量类):
+
+    def __init__(我):
+        raise TypeError(f'{我.__class__.__name__}不允许实例化')
+
+
+# =============================================== 模式类
+class _模式类(_常量类):
+    '''
+应用样例:
+from zlutils.const import 模式类
+class m(模式类):
+    gtt = 0
+    add = 0
+
+print(m.gtt)
+输出:gtt
+
+'gtt' in m
+输出:True
+
+list(m)
+输出:['gtt', 'add']
+
+'''
+
+    def __contains__(类, 常量):
+        try:
+            super().__getattribute__(常量)
+            return True
+        except:
+            return False
+
+
+    def __getattribute__(类, 常量名):
+        取值 = super().__getattribute__(常量名)
+        if  '_' == 常量名[:1]:
+            return 取值
+        return str(常量名)
+
+
+class 模式类(metaclass=_模式类):
+    '''用于区分不同的模式'''
+    样例 = 0 # 等于号后的值不生效,可任意设置
+
+    def __init__(我):
+        raise TypeError(f'{我.__class__.__name__}不允许实例化')
+
+
+# =============================================== 字段类
+class 字段类:
+    pass
+
```

### Comparing `zlutils-0.1.6/zlutils/shared.py` & `zlutils-0.2.0/zlutils/shared.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-'''
-v0.1 2024-03-22
-# 共享列表在linux,py310环境下有bug,当创建者断开时丢失
-'''
-
-import logging, time
-日志 = logging.getLogger()
-
-_默认字符串编码 = 'utf-8'
-_允许的数据类型 = [int, float, str]
-
-
-class _共享列表映射:
-        def __init__(我, 共享列表, 列表索引):
-            我.列表索引 = 列表索引
-            我.共享列表 = 共享列表
-        def 取值(我):
-            return 我.共享列表[我.列表索引]
-        def __get__(我, 实例, 甲方):
-            return 我.取值()
-        def 赋值(我, 值):
-            if type(值) not in _允许的数据类型:
-                raise RuntimeError(f"赋值类型{type(值)}不在许可范围({_允许的数据类型})中")
-            我.共享列表[我.列表索引] = 值
-        def __repr__(我):
-            return f'{我.__class__.__name__}({我.取值()})'
-
-
-class _只因(type):
-
-    心 = 0.0
-
-    def __new__(元类, 类名, 所有基类, 类变量):
-        if 类名=='公鸡':
-            return super().__new__(元类, 类名, 所有基类, 类变量)
-        import base64
-
-        共享列表名 = 'zls_'+ base64.b64encode(类名.encode(_默认字符串编码)).decode(_默认字符串编码)
-        变量名列表 = [变量名 for 变量名 in 类变量 if (type(类变量[变量名]) in _允许的数据类型)and(变量名[:1]!='_')]
-        类变量_元类 = vars(元类)
-        变量名列表_元类 = [变量名 for 变量名 in 类变量_元类 if (type(类变量_元类[变量名]) in _允许的数据类型)and(变量名[:1]!='_')]
-        变量名列表_合成 = 变量名列表 + 变量名列表_元类
-        from multiprocessing import shared_memory
-        try:
-            共享列表 = shared_memory.ShareableList( name=共享列表名 )
-            日志.info("载入共享列表, 覆盖默认值")
-        except Exception as e:
-            日志.warning(e)
-            值列表 = [ 类变量[变量名] for 变量名 in 变量名列表 ]
-            值列表_元类 = [类变量_元类[变量名] for 变量名 in 变量名列表_元类]
-            值列表_合成 = 值列表+值列表_元类
-            共享列表 = shared_memory.ShareableList( sequence = 值列表_合成, name=共享列表名 )
-            日志.info("以默认值创建共享列表")
-        类变量[f'_{类名}___共享列表'] = 共享列表
-        for 索引值, 变量名 in enumerate(变量名列表_合成):
-            类变量[变量名] = _共享列表映射(共享列表, 索引值)
-        return super().__new__(元类, 类名, 所有基类, 类变量)
-
-    def __setattr__(类, 变量名, 想要设置的值):
-        if 变量名 not in vars(类):
-            raise RuntimeError('这是一只固态的只因不能改变结构')
-        try:
-            vars(类)[变量名].赋值(想要设置的值)
-        except:
-            super().__setattr__(变量名, 想要设置的值)
-
-
-import threading
-class 公鸡(metaclass=_只因):
-    '''使用说明:
-派生类类中的类变量将通过内存共享给本环境中的所有的python程序.
-以派生类的名称为唯一标识.
-类变量值仅支持基本数据类型:int,float,str.
-_开头的类变量会被忽略
-已存在的赋值会覆盖默认值
-不支持自定义方法
-当所有类被释放后共享内存将被释放
-
-派生类定义模板如下:
-
-class 不会下蛋的( 公鸡 ):
-    描述 = "默认值"
-    食量 = 0
-
-# 赋值
-不会下蛋的.食量 = 1
-# 取值
-print(不会下蛋的.食量)
-'''
-
-    心 = 0.0
-
-    def __new__(cls, *_, **__):
-        raise RuntimeError("冷知识: 公鸡不能自我繁殖")
-
-
-class 鸡心管理器:
-
-    def __init__(我, 一只只因, 标准心律=120):
-        我.给自己绑定一只只因(一只只因)
-        我.标准心律 = 标准心律
-
-    def 给自己绑定一只只因(我, 一只只因):
-        if isinstance(一只只因, _只因):
-            我.只因 = 一只只因
-        else:
-            try:
-                _ = 一只只因.心
-                一只只因.心 = time.time()
-                我.只因 = 一只只因
-                日志.warning('虽然不是只因, 但勉强能用吧?...大概')
-            except:
-                日志.error('没有心吗?(꒪⌓꒪)')
-                raise RuntimeError(f"你确定这玩意儿({一只只因})是只因?")
-
-    @property
-    def 心跳间隔(我):
-        return 1 / 我.标准心律
-
-    @property
-    def 心跳检测间隔(我):
-        return 1.5 / 我.标准心律
-
-    def 跳一下(我):
-        我.只因.心 = time.time()
-
-    @property
-    def 有心跳(我):
-        return (time.time()-我.只因.心) <= 我.心跳检测间隔
-
-    def 一直跳(我):
-        我.跳一下()
-        我.准备跳 = threading.Timer(我.心跳间隔 ,我.一直跳)
-        我.准备跳.start()
-
-    def 一颗成熟的心要学会自己跳(我):
-        我.准备跳 = threading.Timer(我.心跳间隔 ,我.一直跳)
-        我.准备跳.start()
-
-    def 似了(我):
-        我.准备跳.cancel()
-
-    def 复活(我):
-        我.准备跳 = threading.Timer(我.心跳间隔 ,我.一直跳)
-        我.准备跳.start()
-
-    def 这次真的似了(我):
-        我.准备跳.cancel()
-
-
-
-
-
-
-
-
-
+'''
+v0.1 2024-03-22
+# 共享列表在linux,py310环境下有bug,当创建者断开时丢失
+'''
+
+import logging, time
+日志 = logging.getLogger()
+
+_默认字符串编码 = 'utf-8'
+_允许的数据类型 = [int, float, str]
+
+
+class _共享列表映射:
+        def __init__(我, 共享列表, 列表索引):
+            我.列表索引 = 列表索引
+            我.共享列表 = 共享列表
+        def 取值(我):
+            return 我.共享列表[我.列表索引]
+        def __get__(我, 实例, 甲方):
+            return 我.取值()
+        def 赋值(我, 值):
+            if type(值) not in _允许的数据类型:
+                raise RuntimeError(f"赋值类型{type(值)}不在许可范围({_允许的数据类型})中")
+            我.共享列表[我.列表索引] = 值
+        def __repr__(我):
+            return f'{我.__class__.__name__}({我.取值()})'
+
+
+class _只因(type):
+
+    心 = 0.0
+
+    def __new__(元类, 类名, 所有基类, 类变量):
+        if 类名=='公鸡':
+            return super().__new__(元类, 类名, 所有基类, 类变量)
+        import base64
+
+        共享列表名 = 'zls_'+ base64.b64encode(类名.encode(_默认字符串编码)).decode(_默认字符串编码)
+        变量名列表 = [变量名 for 变量名 in 类变量 if (type(类变量[变量名]) in _允许的数据类型)and(变量名[:1]!='_')]
+        类变量_元类 = vars(元类)
+        变量名列表_元类 = [变量名 for 变量名 in 类变量_元类 if (type(类变量_元类[变量名]) in _允许的数据类型)and(变量名[:1]!='_')]
+        变量名列表_合成 = 变量名列表 + 变量名列表_元类
+        from multiprocessing import shared_memory
+        try:
+            共享列表 = shared_memory.ShareableList( name=共享列表名 )
+            日志.info("载入共享列表, 覆盖默认值")
+        except Exception as e:
+            日志.warning(e)
+            值列表 = [ 类变量[变量名] for 变量名 in 变量名列表 ]
+            值列表_元类 = [类变量_元类[变量名] for 变量名 in 变量名列表_元类]
+            值列表_合成 = 值列表+值列表_元类
+            共享列表 = shared_memory.ShareableList( sequence = 值列表_合成, name=共享列表名 )
+            日志.info("以默认值创建共享列表")
+        类变量[f'_{类名}___共享列表'] = 共享列表
+        for 索引值, 变量名 in enumerate(变量名列表_合成):
+            类变量[变量名] = _共享列表映射(共享列表, 索引值)
+        return super().__new__(元类, 类名, 所有基类, 类变量)
+
+    def __setattr__(类, 变量名, 想要设置的值):
+        if 变量名 not in vars(类):
+            raise RuntimeError('这是一只固态的只因不能改变结构')
+        try:
+            vars(类)[变量名].赋值(想要设置的值)
+        except:
+            super().__setattr__(变量名, 想要设置的值)
+
+
+import threading
+class 公鸡(metaclass=_只因):
+    '''使用说明:
+派生类类中的类变量将通过内存共享给本环境中的所有的python程序.
+以派生类的名称为唯一标识.
+类变量值仅支持基本数据类型:int,float,str.
+_开头的类变量会被忽略
+已存在的赋值会覆盖默认值
+不支持自定义方法
+当所有类被释放后共享内存将被释放
+
+派生类定义模板如下:
+
+class 不会下蛋的( 公鸡 ):
+    描述 = "默认值"
+    食量 = 0
+
+# 赋值
+不会下蛋的.食量 = 1
+# 取值
+print(不会下蛋的.食量)
+'''
+
+    心 = 0.0
+
+    def __new__(cls, *_, **__):
+        raise RuntimeError("冷知识: 公鸡不能自我繁殖")
+
+
+class 鸡心管理器:
+
+    def __init__(我, 一只只因, 标准心律=120):
+        我.给自己绑定一只只因(一只只因)
+        我.标准心律 = 标准心律
+
+    def 给自己绑定一只只因(我, 一只只因):
+        if isinstance(一只只因, _只因):
+            我.只因 = 一只只因
+        else:
+            try:
+                _ = 一只只因.心
+                一只只因.心 = time.time()
+                我.只因 = 一只只因
+                日志.warning('虽然不是只因, 但勉强能用吧?...大概')
+            except:
+                日志.error('没有心吗?(꒪⌓꒪)')
+                raise RuntimeError(f"你确定这玩意儿({一只只因})是只因?")
+
+    @property
+    def 心跳间隔(我):
+        return 1 / 我.标准心律
+
+    @property
+    def 心跳检测间隔(我):
+        return 1.5 / 我.标准心律
+
+    def 跳一下(我):
+        我.只因.心 = time.time()
+
+    @property
+    def 有心跳(我):
+        return (time.time()-我.只因.心) <= 我.心跳检测间隔
+
+    def 一直跳(我):
+        我.跳一下()
+        我.准备跳 = threading.Timer(我.心跳间隔 ,我.一直跳)
+        我.准备跳.start()
+
+    def 一颗成熟的心要学会自己跳(我):
+        我.准备跳 = threading.Timer(我.心跳间隔 ,我.一直跳)
+        我.准备跳.start()
+
+    def 似了(我):
+        我.准备跳.cancel()
+
+    def 复活(我):
+        我.准备跳 = threading.Timer(我.心跳间隔 ,我.一直跳)
+        我.准备跳.start()
+
+    def 这次真的似了(我):
+        我.准备跳.cancel()
+
+
+
+
+
+
+
+
+
```

