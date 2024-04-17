# Comparing `tmp/ccdt-2.1.95.tar.gz` & `tmp/ccdt-2.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.95.tar", last modified: Mon Apr 15 03:39:48 2024, max compression
+gzip compressed data, was "ccdt-2.1.96.tar", last modified: Wed Apr 17 08:35:42 2024, max compression
```

## Comparing `ccdt-2.1.95.tar` & `ccdt-2.1.96.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.619943 ccdt-2.1.95/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.95/LICENSE
--rw-rw-rw-   0        0        0     4806 2024-04-15 03:39:48.617973 ccdt-2.1.95/PKG-INFO
--rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.95/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.401528 ccdt-2.1.95/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.95/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.417484 ccdt-2.1.95/ccdt/dataset/
--rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.95/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.460370 ccdt-2.1.95/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.95/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.95/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.496273 ccdt-2.1.95/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.95/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0    15199 2023-11-27 03:47:20.000000 ccdt-2.1.95/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0   115264 2024-04-15 03:38:56.000000 ccdt-2.1.95/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.539159 ccdt-2.1.95/ccdt/dataset/base_voc/
--rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.95/ccdt/dataset/base_voc/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.95/ccdt/dataset/base_voc/base_sys.py
--rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.95/ccdt/dataset/base_voc/base_txt.py
--rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.95/ccdt/dataset/base_voc/base_voc.py
--rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.95/ccdt/dataset/base_voc/coco_to_labelme.py
--rw-rw-rw-   0        0        0    23667 2024-03-07 03:40:15.000000 ccdt-2.1.95/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.556113 ccdt-2.1.95/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.95/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.95/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    27068 2024-02-02 07:58:30.000000 ccdt-2.1.95/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.594037 ccdt-2.1.95/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.95/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.95/ccdt/video_tool/intercept.py
--rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.95/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.95/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.616951 ccdt-2.1.95/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4806 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 03:39:48.619943 ccdt-2.1.95/setup.cfg
--rw-rw-rw-   0        0        0     2524 2024-04-15 03:39:24.000000 ccdt-2.1.95/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.608001 ccdt-2.1.95/test/
--rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.95/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.341248 ccdt-2.1.96/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.96/LICENSE
+-rw-rw-rw-   0        0        0     4806 2024-04-17 08:35:42.340251 ccdt-2.1.96/PKG-INFO
+-rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.96/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.190991 ccdt-2.1.96/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.96/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.198969 ccdt-2.1.96/ccdt/dataset/
+-rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.96/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.200964 ccdt-2.1.96/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.96/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.96/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.219072 ccdt-2.1.96/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.96/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0    15439 2024-04-17 03:45:32.000000 ccdt-2.1.96/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0   116306 2024-04-17 03:29:29.000000 ccdt-2.1.96/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.268930 ccdt-2.1.96/ccdt/dataset/base_voc/
+-rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.96/ccdt/dataset/base_voc/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.96/ccdt/dataset/base_voc/base_sys.py
+-rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.96/ccdt/dataset/base_voc/base_txt.py
+-rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.96/ccdt/dataset/base_voc/base_voc.py
+-rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.96/ccdt/dataset/base_voc/coco_to_labelme.py
+-rw-rw-rw-   0        0        0    24241 2024-04-17 02:49:30.000000 ccdt-2.1.96/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.285530 ccdt-2.1.96/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.96/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.96/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    27118 2024-04-17 08:29:52.000000 ccdt-2.1.96/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.316315 ccdt-2.1.96/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.96/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.96/ccdt/video_tool/intercept.py
+-rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.96/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.96/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.339253 ccdt-2.1.96/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4806 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 08:35:42.341248 ccdt-2.1.96/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2024-04-17 08:35:11.000000 ccdt-2.1.96/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.330277 ccdt-2.1.96/test/
+-rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.96/test/test.py
```

### Comparing `ccdt-2.1.95/LICENSE` & `ccdt-2.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/PKG-INFO` & `ccdt-2.1.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.95
+Version: 2.1.96
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.95/README.md` & `ccdt-2.1.96/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.96/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.96/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,24 +93,27 @@
                     obj_path = Path(data_info.get('image_file'))  # 初始化文件为对象
                     # 如果图片名称后缀格式重复多次，就进行重写json文件后保存，重命名图片名称
                     if data_info['image_file'].count(obj_path.suffix) >= 2:
                         file_path = data_info.get('full_path')
                         print(f'图像数据文件格式存在双后缀：{file_path}  请核对数据')
                     else:  # 处理正常数据，包含重构列表原始封装列表
                         if isinstance(judge_dir, str) or isinstance(index, bool) or isinstance(index, str) or isinstance(index, argparse.Namespace):
-                            save_images_dir = Path(data_info['output_dir'], data_info['image_dir'])
-                            # save_images_dir = os.path.join(data_info['output_dir'], data_info['image_dir'])
-                            os.makedirs(save_images_dir, exist_ok=True)
-                            save_labelme_dir = Path(data_info['output_dir'], data_info['labelme_dir'])
-                            # save_labelme_dir = os.path.join(data_info['output_dir'], data_info['labelme_dir'])
-                            os.makedirs(save_labelme_dir, exist_ok=True)
+                            if custom_label:
+                                save_images_dir = str(Path(data_info['output_dir'], custom_label, data_info['image_dir']))
+                                os.makedirs(save_images_dir, exist_ok=True)
+                                save_labelme_dir = str(Path(data_info['output_dir'], custom_label, data_info['labelme_dir']))
+                                os.makedirs(save_labelme_dir, exist_ok=True)
+                            else:
+                                save_images_dir = Path(data_info['output_dir'], data_info['image_dir'])
+                                os.makedirs(save_images_dir, exist_ok=True)
+                                save_labelme_dir = Path(data_info['output_dir'], data_info['labelme_dir'])
+                                os.makedirs(save_labelme_dir, exist_ok=True)
                             # 图像文件处理，json文件处理
                             if index is True:  # 文件移动
-                                tasks.append(asyncio.create_task(
-                                    self.move_file(data_info['full_path'], save_images_dir)))
+                                tasks.append(asyncio.create_task(self.move_file(data_info['full_path'], save_images_dir)))
                                 if data_info.get('background') is True:  # 不为背景才移动json文件
                                     tasks.append(asyncio.create_task(self.move_file(data_info['original_json_path'], save_labelme_dir)))
                             else:  # 文件拷贝
                                 # 使用 os.path.normpath() 函数，将 Windows 路径转换成标准的跨平台的路径格式
                                 if os.path.normpath(data_info['input_dir']) == os.path.normpath(data_info['output_dir']):
                                     pass
                                 else:
```

### Comparing `ccdt-2.1.95/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.96/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -2029,7 +2029,23 @@
             print(args)
             if dataset.get('labelme_info') is not None:
                 for shape in dataset.get('labelme_info').get('shapes'):
                     for key, value in shape.get("flags").items():
                         if value == args.flags_true:
                             if key in args.filter_flags:
                                 print(key)
+
+    # 按比例划分测试集和训练集,比例一般0.8/0.2或者是0.7/0.3，只实现剪切或移动文件，不能够拷贝，想拷贝需要修改输出的逻辑。
+    def ratio_split(self, args):
+        sublist_test, sublist_train = self.split_list_by_ratio(self.datasets, args.test_ratio, args.train_ratio)
+        self.save_labelme(sublist_test, args.select_cut, "test")  # 保存划分测试集的数据
+        self.save_labelme(sublist_train, args.select_cut, "train")  # 保存划分训练集的数据
+
+    @staticmethod
+    def split_list_by_ratio(lst, ratio_test, ratio_train):
+        total_count = len(lst)
+        sublist_test_count = round(total_count * ratio_test)  # 通过round进行四舍五入计算，保障奇数计算准确
+        sublist_train_count = round(total_count * ratio_train)
+        random.shuffle(lst)
+        sublist_test = lst[:sublist_test_count]
+        sublist_train = lst[sublist_test_count:sublist_test_count + sublist_train_count]
+        return sublist_test, sublist_train
```

### Comparing `ccdt-2.1.95/ccdt/dataset/base_voc/base_sys.py` & `ccdt-2.1.96/ccdt/dataset/base_voc/base_sys.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/base_voc/base_txt.py` & `ccdt-2.1.96/ccdt/dataset/base_voc/base_txt.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/base_voc/base_voc.py` & `ccdt-2.1.96/ccdt/dataset/base_voc/base_voc.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/base_voc/coco_to_labelme.py` & `ccdt-2.1.96/ccdt/dataset/base_voc/coco_to_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/main.py` & `ccdt-2.1.96/ccdt/dataset/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     parser.add_argument('--judging-cross-the-border', type=str, help="检查标注形状是否超越原始图像边界")
     parser.add_argument('--point-number', type=int, help='点标注的数量，用于标注点排序时，追加标注点到列表中然后判断，是否满足标注规则')
     parser.add_argument('--automatic-correction', action="store_true", help="默认False，是否自动矫正标注形状超越图像边界情况。是为True，否为False")
     parser.add_argument('--rectangle-merge', action="store_true", help="默认False，填写参数代表为true，用于判断合并条件，该条件表示矩形框合并。是为True，否为False")
     parser.add_argument('--sync', action="store_true", help="默认False，填写参数代表为true，用于判断是同步处理，还是异步处理。是为True，否为False")
     parser.add_argument('--threshold', type=float, help="阈值参数，模型预测数据集，设定的阈值")
     parser.add_argument('--leak-check', action="store_true", help="默认False，填写参数代表为true，用于筛选漏检出数据。是为True，否为False")
+    parser.add_argument('--randomize', action="store_true", help="默认False，填写参数代表为true，用于列表随机化。是为True，否为False")
+    parser.add_argument('--test-ratio', type=float, default=0.2, help='默认测试集比例值')
+    parser.add_argument('--train-ratio', type=float, default=0.8, help='默认训练集比例值')
     parser.add_argument('--error-check', action="store_true", help="默认False，填写参数代表为true，用于筛选误检出数据。是为True，否为False")
     parser.add_argument('--right-check', action="store_true", help="默认False，填写参数代表为true，用于筛选正确检出数据。是为True，否为False")
     parser.add_argument('--coco-to-bbox', action="store_true", help="默认False，填写参数代表为true，用于判断多边形转矩形框。是为True，否为False")
     parser.add_argument('--background', action="store_true", help="默认False，填写参数代表为true，用于把系统输出的json转换为labelme对应的json。是为True，否为False")
     parser.add_argument('--is-PCA', action="store_true",
                         help="默认False，填写参数代表为true，用于直方图降维条件判断。是为True，但会造成信息丢失，否为False，信息更准确")
     parser.add_argument('--delete', action="store_true", help="默认False，填写参数代表为true，用于删除勾选数据。是为True，否为False")
@@ -152,14 +155,16 @@
         return args
     elif args.function == 'move':  # 移动文件，临时功能
         return args
     elif args.function == 'modify_flags':  # 修改flags字典值
         return args
     elif args.function == 'filter_flags_true':  # 筛选flags字典值为真的数据
         return args
+    elif args.function == 'ratio':  # 筛选flags字典值为真的数据
+        return args
     else:
         assert not args.function, '传入的操作功能参数不对:{}'.format(args.function)
 
 
 def main():
     # async def main():
     args = parser_args()
@@ -299,13 +304,15 @@
         #     dataset.image_check(args)
         elif args.function == 'move':  # 自定义格式把文件重命名
             dataset.move_file(args)
         elif args.function == 'modify_flags':  # 修改falgs值
             dataset.modify_flags(args)
         elif args.function == 'filter_flags_true':  # 筛选falgs值为真的标注
             dataset.select_flags_true(args)
+        elif args.function == 'ratio':  # 按比例划分测试集和训练集
+            dataset.ratio_split(args)
 
 
 if __name__ == '__main__':
     main()
     # 使用了asyncio.run()函数来启动，协程事件循环，则不需要手动关闭事件循环
     # asyncio.run(main())
```

### Comparing `ccdt-2.1.95/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.96/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.96/ccdt/dataset/utils/labelme_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,34 +212,34 @@
         2、使用数据库：将文件数据导入数据库，然后使用数据库查询来处理数据。数据库可以优化大规模数据的存储和检索。（最优推荐）
         """
         obj_path = Path(file_path)
         if obj_path.suffix in self.parameter.file_formats:
             # 设计规则，根据图片文件查找json文件，同时根据约定的目录规则封装labelme数据集
             if file_path.count('00.images') == 1 or self.parameter.output_format == 'voc' or self.parameter.output_format == 'sys':
                 # relative_path = os.path.join('..', obj_path.parent.name, obj_path.name)
-                relative_path = Path('..', obj_path.parent.name, obj_path.name)
+                relative_path = str(Path('..', obj_path.parent.name, obj_path.name))
                 # image_dir = str(obj_path.parent).replace('\\', '/').replace(root_dir, '').strip('\\/')
                 image_dir = obj_path.parent.relative_to(root_dir)
-                labelme_dir = Path(image_dir.parent, '01.labelme')
+                labelme_dir = str(Path(image_dir.parent, '01.labelme'))
                 # labelme_dir = os.path.join(image_dir.replace('00.images', '').strip('\\/'), '01.labelme')
                 labelme_file = obj_path.stem + '.json'
                 json_path = None
-                output_dir = Path(self.parameter.output_dir)
+                output_dir = str(Path(self.parameter.output_dir))
                 if self.parameter.output_dir:
                     # 打印的时候不需要用到，非打印功能，都会用到
-                    json_path = Path(self.parameter.output_dir, labelme_dir, labelme_file)
-                original_json_path = Path(root_dir, labelme_dir, labelme_file)
+                    json_path = str(Path(self.parameter.output_dir, labelme_dir, labelme_file))
+                original_json_path = str(Path(root_dir, labelme_dir, labelme_file))
                 md5_value = await self.calculate_file_md5_async(file_path)  # 如果不是图像，这里获取MD5值是无法获取的，会直接跳转，存在未知图像后缀格式数据的逻辑
                 if self.parameter.output_dir:  # 如果有输出路径，则自定义错误输出目录
-                    self.group_error_path = Path(self.parameter.output_dir, 'group_error_path')
-                    self.out_of_bounds_path = Path(self.parameter.output_dir, 'out_of_bounds_path')
-                    self.error_path = Path(self.parameter.output_dir, 'error_path')
+                    self.group_error_path = str(Path(self.parameter.output_dir, 'group_error_path'))
+                    self.out_of_bounds_path = str(Path(self.parameter.output_dir, 'out_of_bounds_path'))
+                    self.error_path = str(Path(self.parameter.output_dir, 'error_path'))
                 image = Image.open(file_path)
                 # image, check = self.is_valid_image(file_path)  # 暂时不用
-                data_path = dict(image_dir=image_dir,  # 封装图像目录相对路径，方便后期路径重组及拼接
+                data_path = dict(image_dir=str(image_dir),  # 封装图像目录相对路径，方便后期路径重组及拼接
                                  image_file=obj_path.name,  # 封装图像文件名称
                                  image_width=image.width,  # 封装图像宽度
                                  image_height=image.height,  # 封装图像高度
                                  labelme_dir=labelme_dir,  # 封装json文件相对目录
                                  labelme_file=labelme_file,  # 封装json文件名称
                                  input_dir=root_dir,  # 封装输入路径目录
                                  output_dir=output_dir,  # 封装输出路径目录
@@ -248,15 +248,15 @@
                                  error_path=self.error_path,  # 错误数据存放总目录，不分错误类别
                                  http_url=self.parameter.http_url,  # 封装http对象存储服务访问服务地址
                                  point_number=self.parameter.point_number,
                                  # 封装数据处理类型，包含base_labelme基类和coco基类
                                  data_type=self.type_args[0].get('type'),
                                  labelme_info=None,  # 封装一张图像标注属性信息
                                  background=True,  # 封装一张图像属于负样本还是正样本，默认为True，正样本，有标注
-                                 full_path=obj_path,  # 封装一张图像绝对路径
+                                 full_path=str(obj_path),  # 封装一张图像绝对路径
                                  json_path=json_path,  # 封装一张图像对应json文件绝对路径，用于输出时写文件的路径使用
                                  original_json_path=original_json_path,  # 封装原始json文件绝对路径
                                  md5_value=md5_value,  # 封装一张图像MD5值，用于唯一性判断
                                  relative_path=relative_path,
                                  # check=check,  # 图像校验结果记录，true为合格图像，false为不合格图像
                                  # 封装图像使用标注工具读取相对路径，格式为：..\\00.images\\000000000419.jpg
                                  only_annotation=False, )  # 封装是图像还是处理图像对应标注内容的判断条件，默认图片和注释文件一起处理
```

### Comparing `ccdt-2.1.95/ccdt/video_tool/intercept.py` & `ccdt-2.1.96/ccdt/video_tool/intercept.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/video_tool/split.py` & `ccdt-2.1.96/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt/video_tool/video_main.py` & `ccdt-2.1.96/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.96/ccdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.95
+Version: 2.1.96
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.95/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.96/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.95/setup.py` & `ccdt-2.1.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.95',
+    version='2.1.96',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ccdt-2.1.95/test/test.py` & `ccdt-2.1.96/test/test.py`

 * *Files identical despite different names*

