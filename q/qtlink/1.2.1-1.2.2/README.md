# Comparing `tmp/qtlink-1.2.1.tar.gz` & `tmp/qtlink-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.2.1.tar", last modified: Mon Apr 15 06:38:59 2024, max compression
+gzip compressed data, was "qtlink-1.2.2.tar", last modified: Wed Apr 17 09:19:12 2024, max compression
```

## Comparing `qtlink-1.2.1.tar` & `qtlink-1.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.694764 qtlink-1.2.1/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      466 2024-04-15 06:38:59.694764 qtlink-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.569359 qtlink-1.2.1/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.1/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.647878 qtlink-1.2.1/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.1/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1730 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0     1357 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1981 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     1926 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.663514 qtlink-1.2.1/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.1/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.679140 qtlink-1.2.1/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.1/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.1/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.1/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.694764 qtlink-1.2.1/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.1/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.2.1/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.1/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:38:59.694764 qtlink-1.2.1/qtlink.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-15 06:38:59.000000 qtlink-1.2.1/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-15 06:38:59.000000 qtlink-1.2.1/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:38:59.000000 qtlink-1.2.1/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 06:38:59.000000 qtlink-1.2.1/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 06:38:59.000000 qtlink-1.2.1/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 06:38:59.694764 qtlink-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-15 06:38:34.000000 qtlink-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.401497 qtlink-1.2.2/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-17 09:19:12.399490 qtlink-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.362972 qtlink-1.2.2/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.2/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.387977 qtlink-1.2.2/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.2/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1730 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0     1357 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1981 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     2019 2024-04-17 09:15:02.000000 qtlink-1.2.2/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.390977 qtlink-1.2.2/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.2/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.394977 qtlink-1.2.2/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.2/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.2/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.2/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.397490 qtlink-1.2.2/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.2/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.2/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.2/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:19:12.398490 qtlink-1.2.2/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 09:19:12.000000 qtlink-1.2.2/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 09:19:12.401497 qtlink-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-04-17 09:16:45.000000 qtlink-1.2.2/setup.py
```

### Comparing `qtlink-1.2.1/LICENSE` & `qtlink-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/dialog/dialog_choice.py` & `qtlink-1.2.2/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/dialog/dialog_info.py` & `qtlink-1.2.2/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.2/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/dialog/dialog_table_display.py` & `qtlink-1.2.2/qtlink/dialog/dialog_table_display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide6.QtWidgets import QDialog, QTableView, QLabel, QVBoxLayout
+from PySide6.QtWidgets import QDialog, QTableView, QLabel, QVBoxLayout, QAbstractItemView
 
 from qtlink.table.table_controller import TableController
 
 
 def show_dialog_table_display(text: str,
                               table_data: list[dict],
                               show_or_exec: str = 'exec',
@@ -37,13 +37,14 @@
         :param kwargs: 表格控制器可能使用的其他参数
         """
         super().__init__(parent=parent)
         self.v_layout = QVBoxLayout()
         label = QLabel(text, self)
         label.setWordWrap(True)
         self.tableview = QTableView(self)
+        self.tableview.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.v_layout.addWidget(label)
         self.v_layout.addWidget(self.tableview)
 
         self.setLayout(self.v_layout)
         self.table_controller = TableController(tableview=self.tableview)
         self.table_controller.update_table_data(table_data=table_data, *args, **kwargs)
```

### Comparing `qtlink-1.2.1/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.2/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/table/table_controller.py` & `qtlink-1.2.2/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.2.2/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/table/table_controller_single_check.py` & `qtlink-1.2.2/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/util.py` & `qtlink-1.2.2/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink/widgets/list_widget.py` & `qtlink-1.2.2/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.2/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.1/setup.py` & `qtlink-1.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.2.1",
+    version="1.2.2",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6'],
```

