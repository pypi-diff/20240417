# Comparing `tmp/qtlink-1.2.2.tar.gz` & `tmp/qtlink-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.2.2.tar", last modified: Wed Apr 17 09:19:12 2024, max compression
+gzip compressed data, was "qtlink-1.2.3.tar", last modified: Wed Apr 17 12:05:42 2024, max compression
```

## Comparing `qtlink-1.2.2.tar` & `qtlink-1.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.401497 qtlink-1.2.2/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      466 2024-04-17 09:19:12.399490 qtlink-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.362972 qtlink-1.2.2/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.2/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.387977 qtlink-1.2.2/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.2/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1730 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0     1357 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1981 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     2019 2024-04-17 09:15:02.000000 qtlink-1.2.2/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.390977 qtlink-1.2.2/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.2/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.394977 qtlink-1.2.2/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.2/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.2/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.397490 qtlink-1.2.2/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.2/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.2/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.2/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.398490 qtlink-1.2.2/qtlink.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 09:19:12.401497 qtlink-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-17 09:16:45.000000 qtlink-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.690459 qtlink-1.2.3/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-17 12:05:42.654404 qtlink-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.623153 qtlink-1.2.3/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.3/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.638778 qtlink-1.2.3/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.3/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1730 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0     1262 2024-04-17 12:03:49.000000 qtlink-1.2.3/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1981 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     2019 2024-04-17 09:15:02.000000 qtlink-1.2.3/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.638778 qtlink-1.2.3/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.3/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.654404 qtlink-1.2.3/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.3/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.3/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.654404 qtlink-1.2.3/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.3/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.3/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.3/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.654404 qtlink-1.2.3/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:05:42.690459 qtlink-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-04-17 12:05:41.000000 qtlink-1.2.3/setup.py
```

### Comparing `qtlink-1.2.2/LICENSE` & `qtlink-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/dialog/dialog_choice.py` & `qtlink-1.2.3/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/dialog/dialog_info.py` & `qtlink-1.2.3/qtlink/dialog/dialog_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QLabel, QPushButton
 
 
-def show_dialog_info(text: str, enable_btn_confirm: bool = False, show_or_exec: str = 'exec'):
+def show_dialog_info(text: str, show_or_exec: str = 'exec', *args, **kwargs):
     """以函数形式直接启动对话框
     :param text: 对话框的消息文本
-    :param enable_btn_confirm: 是否启用确定按钮，默认不启用
     :param show_or_exec: 对话框的运行方式，'exec' or 'show'
     """
-    dialog = DialogInfo(text, enable_btn_confirm)
+    dialog = DialogInfo(text, *args, **kwargs)
     if show_or_exec == 'exec':
         dialog.exec()
     else:
         dialog.show()
 
 
 class DialogInfo(QDialog):
```

### Comparing `qtlink-1.2.2/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.3/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/dialog/dialog_table_display.py` & `qtlink-1.2.3/qtlink/dialog/dialog_table_display.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.3/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/table/table_controller.py` & `qtlink-1.2.3/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.2.3/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/table/table_controller_single_check.py` & `qtlink-1.2.3/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/util.py` & `qtlink-1.2.3/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/widgets/drop_widget.py` & `qtlink-1.2.3/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink/widgets/list_widget.py` & `qtlink-1.2.3/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.3/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.2/setup.py` & `qtlink-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.2.2",
+    version="1.2.3",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6'],
```

