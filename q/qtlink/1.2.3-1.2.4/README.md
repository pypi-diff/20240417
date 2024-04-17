# Comparing `tmp/qtlink-1.2.3.tar.gz` & `tmp/qtlink-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.2.3.tar", last modified: Wed Apr 17 12:05:42 2024, max compression
+gzip compressed data, was "qtlink-1.2.4.tar", last modified: Wed Apr 17 13:09:35 2024, max compression
```

## Comparing `qtlink-1.2.3.tar` & `qtlink-1.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.690459 qtlink-1.2.3/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      466 2024-04-17 12:05:42.654404 qtlink-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.623153 qtlink-1.2.3/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.3/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.638778 qtlink-1.2.3/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.3/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1730 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0     1262 2024-04-17 12:03:49.000000 qtlink-1.2.3/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1981 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     2019 2024-04-17 09:15:02.000000 qtlink-1.2.3/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.638778 qtlink-1.2.3/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.3/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.654404 qtlink-1.2.3/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.3/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.3/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.3/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.654404 qtlink-1.2.3/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.3/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.3/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.3/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:05:42.654404 qtlink-1.2.3/qtlink.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 12:05:42.000000 qtlink-1.2.3/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 12:05:42.690459 qtlink-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-17 12:05:41.000000 qtlink-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.452337 qtlink-1.2.4/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-17 13:09:35.452337 qtlink-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.421098 qtlink-1.2.4/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.4/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.436711 qtlink-1.2.4/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.4/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1620 2024-04-17 13:09:04.000000 qtlink-1.2.4/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0     1403 2024-04-17 13:05:04.000000 qtlink-1.2.4/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.4/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.4/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.436711 qtlink-1.2.4/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.4/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.4/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.452337 qtlink-1.2.4/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.4/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.4/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.4/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.4/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.4/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.452337 qtlink-1.2.4/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.4/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.4/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.4/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:35.452337 qtlink-1.2.4/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-17 13:09:35.000000 qtlink-1.2.4/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-17 13:09:35.000000 qtlink-1.2.4/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:09:35.000000 qtlink-1.2.4/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 13:09:35.000000 qtlink-1.2.4/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 13:09:35.000000 qtlink-1.2.4/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:09:35.452337 qtlink-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-04-17 13:09:04.000000 qtlink-1.2.4/setup.py
```

### Comparing `qtlink-1.2.3/LICENSE` & `qtlink-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/dialog/dialog_choice.py` & `qtlink-1.2.4/qtlink/dialog/dialog_choice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QLabel, QPushButton, QHBoxLayout
 
 
-def show_dialog_choice(text: str, click_btn_confirm, show_or_exec: str = 'exec', parent=None):
+def show_dialog_choice(text: str, show_or_exec: str = 'exec', *args, **kwargs):
     """以函数形式直接启动对话框
     :param text: 对话框的消息文本
-    :param click_btn_confirm: 点击确定按钮后自动调用的函数
     :param show_or_exec: 对话框的运行方式，'exec' or 'show'
-    :param parent: 对话框所属的父类
     """
-    dialog = DialogChoice(text, click_btn_confirm=click_btn_confirm, parent=parent)
+    dialog = DialogChoice(text, *args, **kwargs)
     if show_or_exec == 'exec':
         dialog.exec()
     else:
         dialog.show()
 
 
 class DialogChoice(QDialog):
     """带有确定/取消按钮的对话框类"""
 
-    def __init__(self, text: str, click_btn_confirm, parent=None):
+    def __init__(self, text: str, click_btn_confirm, parent=None, title: str = '提示'):
         """
         :param text: 对话框的文本消息
         :param click_btn_confirm: 点击确定按钮后自动调用的函数
         :param parent: 对话框所属的父类
         """
         super().__init__(parent=parent)
         vLayout = QVBoxLayout()
@@ -37,12 +35,13 @@
         hLayout.addWidget(btn_confirm)
 
         btn_cancel = QPushButton('取消', self)
         btn_cancel.clicked.connect(self.close)
         hLayout.addWidget(btn_cancel)
         vLayout.addLayout(hLayout)
 
+        self.setWindowTitle(title)
         self.setLayout(vLayout)
 
     def on_clicked_btn_confirm(self):
         self.click_btn_confirm()
         self.close()
```

### Comparing `qtlink-1.2.3/qtlink/dialog/dialog_info.py` & `qtlink-1.2.4/qtlink/dialog/dialog_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QLabel, QPushButton
 
 
 def show_dialog_info(text: str, show_or_exec: str = 'exec', *args, **kwargs):
     """以函数形式直接启动对话框
     :param text: 对话框的消息文本
     :param show_or_exec: 对话框的运行方式，'exec' or 'show'
+    :param args: Dialog的其他参数
+    :param kwargs: Dialog的其他参数
     """
     dialog = DialogInfo(text, *args, **kwargs)
     if show_or_exec == 'exec':
         dialog.exec()
     else:
         dialog.show()
 
 
 class DialogInfo(QDialog):
     """仅显示文本消息的对话框类"""
 
-    def __init__(self, text: str, enable_btn_confirm: bool = False, parent=None):
+    def __init__(self, text: str, enable_btn_confirm: bool = False, parent=None, title: str = '提示'):
         """
         :param text: 对话框的文本消息
         :param enable_btn_confirm: 是否启用确定按钮（只有关闭对话框的作用），默认不启用
         :param parent: 对话框所属的父类
         """
         super().__init__(parent=parent)
         vLayout = QVBoxLayout()
@@ -30,8 +32,9 @@
         vLayout.addWidget(label)
 
         if enable_btn_confirm:
             btn_confirm = QPushButton('确定', self)
             btn_confirm.clicked.connect(self.close)
             vLayout.addWidget(btn_confirm)
 
+        self.setWindowTitle(title)
         self.setLayout(vLayout)
```

### Comparing `qtlink-1.2.3/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.4/qtlink/dialog/dialog_table_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 class DialogTableCheck(DialogTableDisplay):
     """可以显示并选择表格数据的对话框"""
 
     def __init__(self, text: str,
                  table_data: list[dict],
                  check_type: str = 'single',
                  parent=None,
+                 title: str = '选择',
                  *args, **kwargs):
         """
         :param text: 对话框的消息文本
         :param table_data: 表格数据
         :param check_type: 表格数据的选择方式，单选：'single'，多选：'multiple'
         :param parent: 对话框所属的父类
         :param args: 表格控制器可能使用的其他参数
         :param kwargs: 表格控制器可能使用的其他参数
         """
         super().__init__(text=text, table_data=table_data, parent=parent)
 
         self.btn_ok = QPushButton('确定')
         self.v_layout.addWidget(self.btn_ok)
+
+        self.setWindowTitle(title)
         self.setLayout(self.v_layout)
 
         if check_type == 'single':
             self.table_controller = TableControllerSingleCheck(tableview=self.tableview)
         elif check_type == 'multiple':
             self.table_controller = TableControllerMultipleCheck(tableview=self.tableview)
         else:
```

### Comparing `qtlink-1.2.3/qtlink/dialog/dialog_table_display.py` & `qtlink-1.2.4/qtlink/dialog/dialog_table_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 class DialogTableDisplay(QDialog):
     """可以显示表格数据的对话框"""
 
     def __init__(self, text: str,
                  table_data: list[dict],
                  parent=None,
+                 title: str = '提示',
                  *args, **kwargs):
         """
         :param text: 对话框的文本消息
         :param table_data: 表格数据
         :param parent: 对话框所属的父类
         :param args: 表格控制器可能使用的其他参数
         :param kwargs: 表格控制器可能使用的其他参数
@@ -41,10 +42,11 @@
         label = QLabel(text, self)
         label.setWordWrap(True)
         self.tableview = QTableView(self)
         self.tableview.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.v_layout.addWidget(label)
         self.v_layout.addWidget(self.tableview)
 
+        self.setWindowTitle(title)
         self.setLayout(self.v_layout)
         self.table_controller = TableController(tableview=self.tableview)
         self.table_controller.update_table_data(table_data=table_data, *args, **kwargs)
```

### Comparing `qtlink-1.2.3/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.4/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/table/table_controller.py` & `qtlink-1.2.4/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.2.4/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/table/table_controller_single_check.py` & `qtlink-1.2.4/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/util.py` & `qtlink-1.2.4/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/widgets/drop_widget.py` & `qtlink-1.2.4/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink/widgets/list_widget.py` & `qtlink-1.2.4/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.4/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.3/setup.py` & `qtlink-1.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.2.3",
+    version="1.2.4",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6'],
```

