# Comparing `tmp/xtnkk-tools-1.0.0.7.tar.gz` & `tmp/xtnkk-tools-1.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.0.7.tar", last modified: Wed Apr 17 08:41:12 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.0.8.tar", last modified: Wed Apr 17 09:53:36 2024, max compression
```

## Comparing `xtnkk-tools-1.0.0.7.tar` & `xtnkk-tools-1.0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.7/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-17 08:41:04.000000 xtnkk-tools-1.0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/
--rw-rw-rw-   0        0        0     4932 2024-04-17 08:22:51.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     4491 2024-04-17 08:40:50.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-17 09:53:23.000000 xtnkk-tools-1.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/
+-rw-rw-rw-   0        0        0     5484 2024-04-17 09:53:16.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     4491 2024-04-17 08:40:50.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.0.7/setup.py` & `xtnkk-tools-1.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.0.7",  # 版本
+    version="1.0.0.8",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.0.7/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.0.8/xtnkk_tools/MongoDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         return self.db.command(command)
 
     def find(self, coll_name: str, condition: Optional[Dict] = None,
              limit: int = 0, **kwargs) -> List[Dict]:
         """
             find
             coll_name:集合名称
+            condition:查询条件 例如：{"name": "John"}、{"_id": "xxxxx"}
         """
         condition = {} if condition is None else condition
         command = {"find": coll_name, "filter": condition, "limit": limit}
         command.update(kwargs)
         result = self.run_command(command)
         cursor = result["cursor"]
         cursor_id = cursor["id"]
@@ -109,13 +110,28 @@
             data[is_add_create_time_field_name] = get_now_time_int(is_time_10=True)
         collection = self.get_collection(coll_name)
         try:
             collection.insert_one(data)
         except DuplicateKeyError as e:
             if not insert_ignore:
                 raise e
+            return 0
         return 1
 
+    def find_id_is_exist(self, coll_name, _id):
+        """
+            根据id查询id是否存在
+        :param _id:id
+        :return: 存在返回True 否则False
+        """
+        condition = {"_id": _id}
+        status = list(self.find(coll_name, condition))
+        if status:
+            return True
+        return False
+
 
 if __name__ == '__main__':
     mongo_db = MongoDBPro("127.0.0.1", 27017, "spider_pro")
     # mongo_db.add_data_one("test", {"_id": "1", "data": "aaa"})
+    print(mongo_db.find_id_is_exist("test", "1"))
+    print(mongo_db.find_id_is_exist("test", "11"))
```

### Comparing `xtnkk-tools-1.0.0.7/xtnkk_tools/tools.py` & `xtnkk-tools-1.0.0.8/xtnkk_tools/tools.py`

 * *Files identical despite different names*

