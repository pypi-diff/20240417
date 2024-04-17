# Comparing `tmp/tkeasygui-0.2.45.tar.gz` & `tmp/tkeasygui-0.2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.45.tar", last modified: Tue Apr 16 00:08:49 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.46.tar", last modified: Tue Apr 16 15:15:53 2024, max compression
```

## Comparing `tkeasygui-0.2.45.tar` & `tkeasygui-0.2.46.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 00:08:49.133697 tkeasygui-0.2.45/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.45/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-16 00:08:49.133415 tkeasygui-0.2.45/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     2975 2024-04-15 03:34:58.000000 tkeasygui-0.2.45/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 00:08:49.132094 tkeasygui-0.2.45/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.45/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    16604 2024-04-02 14:45:10.000000 tkeasygui-0.2.45/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      188 2024-04-14 12:33:36.000000 tkeasygui-0.2.45/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-16 00:08:47.000000 tkeasygui-0.2.45/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   108336 2024-04-15 23:41:53.000000 tkeasygui-0.2.45/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 00:08:49.133135 tkeasygui-0.2.45/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1346 2024-04-16 00:08:41.000000 tkeasygui-0.2.45/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-16 00:08:49.133753 tkeasygui-0.2.45/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 15:15:53.183107 tkeasygui-0.2.46/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.46/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-16 15:15:53.182860 tkeasygui-0.2.46/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     3578 2024-04-16 00:24:05.000000 tkeasygui-0.2.46/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 15:15:53.180883 tkeasygui-0.2.46/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.46/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    17350 2024-04-16 15:05:05.000000 tkeasygui-0.2.46/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      825 2024-04-16 14:26:56.000000 tkeasygui-0.2.46/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-16 15:15:27.000000 tkeasygui-0.2.46/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   109812 2024-04-16 14:46:52.000000 tkeasygui-0.2.46/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 15:15:53.182578 tkeasygui-0.2.46/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-16 15:10:23.000000 tkeasygui-0.2.46/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-16 15:15:53.183170 tkeasygui-0.2.46/setup.cfg
```

### Comparing `tkeasygui-0.2.45/LICENSE` & `tkeasygui-0.2.46/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.45/PKG-INFO` & `tkeasygui-0.2.46/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.45
+Version: 0.2.46
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -30,22 +30,21 @@
 Project-URL: Documentation, https://github.com/kujirahand/tkeasygui-python/blob/main/README.md
 Project-URL: Repository, https://github.com/kujirahand/tkeasygui-python/
 Project-URL: Issues, https://github.com/kujirahand/tkeasygui-python/issues
 Keywords: GUI,Tkinter,PySimpleGUI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: pyperclip
 
 # TkEasyGUI
 
@@ -120,25 +119,36 @@
 
 ## Samples
 
 We have prepared a selection of samples to demonstrate simple usage. Please check them out.
 
 - [samples](https://github.com/kujirahand/tkeasygui-python/tree/main/tests).
 
+Running `tests/file_viewer.py` allows all samples to be easily launched.
+
 ## Documents
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
 ## About the relationship with PySimpleGUI
 
 - When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
 - The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
 - This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
 - We are not considering full compatibility with PySimpleGUI.
 
+### TkEasyGUI features:
+
+- Using a `for` loop and `window.event_iter()` enables straightforward event processing.
+- Custom popup dialogs, such as a color selection dialog (`eg.popup_color`), are available.
+- The `Image` class supports not only PNG but also JPEG formats.
+- Convenient event hooks and features for bulk event registration are provided - [docs/custom_events](docs/custom_events.md).
+- Methods such as Copy, Paste, and Cut are added to text boxes (Multiline/Input).
+- The system's default color scheme is utilized.
+
 ## Link
 
 - [pypi.org > TkEasyGUI](https://pypi.org/project/tkeasygui/)
 - [GitHub > TkEasyGUI](https://github.com/kujirahand/tkeasygui-python/)
```

### Comparing `tkeasygui-0.2.45/README.md` & `tkeasygui-0.2.46/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -71,25 +71,36 @@
 
 ## Samples
 
 We have prepared a selection of samples to demonstrate simple usage. Please check them out.
 
 - [samples](https://github.com/kujirahand/tkeasygui-python/tree/main/tests).
 
+Running `tests/file_viewer.py` allows all samples to be easily launched.
+
 ## Documents
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
 ## About the relationship with PySimpleGUI
 
 - When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
 - The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
 - This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
 - We are not considering full compatibility with PySimpleGUI.
 
+### TkEasyGUI features:
+
+- Using a `for` loop and `window.event_iter()` enables straightforward event processing.
+- Custom popup dialogs, such as a color selection dialog (`eg.popup_color`), are available.
+- The `Image` class supports not only PNG but also JPEG formats.
+- Convenient event hooks and features for bulk event registration are provided - [docs/custom_events](docs/custom_events.md).
+- Methods such as Copy, Paste, and Cut are added to text boxes (Multiline/Input).
+- The system's default color scheme is utilized.
+
 ## Link
 
 - [pypi.org > TkEasyGUI](https://pypi.org/project/tkeasygui/)
 - [GitHub > TkEasyGUI](https://github.com/kujirahand/tkeasygui-python/)
```

### Comparing `tkeasygui-0.2.45/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.46/TkEasyGUI/dialogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 TkEasyGUI dialogs
 """
 import subprocess
 import tkinter.filedialog as filedialog
 import tkinter.messagebox as messagebox
 from datetime import datetime, timedelta
 from tkinter import colorchooser
-from typing import Any
+from typing import Union
 
-import TkEasyGUI as eg
+from .utils import WindowType, ElementType, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
+from . import widgets as eg
 
 #------------------------------------------------------------------------------
 # Dialogs
 #------------------------------------------------------------------------------
 # like PySimpleGUI
 
 def popup_buttons(message: str, title: str = "Question", buttons: list[str] = ["OK", "Cancel"], 
@@ -111,20 +112,20 @@
     """Display a message in a popup window with Yes and No buttons. Return "Yes" or "No" or "Cancel"."""
     return popup_buttons(message, title, buttons=["Yes", "No", "Cancel"])
 
 def popup_cancel(message: str, title: str="") -> str:
     """Display a message in a popup window with OK and Cancel buttons. Return "OK" or "Cancel"."""
     return popup_buttons(message, title, buttons=["Cancel"])
 
-def popup_get_text(message: str, title: str = "", default: str = "", font: tuple[Any]|None=None) -> (str|None):
+def popup_get_text(message: str, title: str = "", default: str = "", font: eg.FontType=None) -> Union[str, None]:
     """Display a message in a popup window with a text entry. Return the text entered."""
     # return simpledialog.askstring(title, message, initialvalue=default)
     return popup_input(message, title, default, font=font)
 
-def popup_input(message: str, title: str = "", default: str = "", font: tuple[Any]|None=None) -> (str|None):
+def popup_input(message: str, title: str = "", default: str = "", font: eg.FontType=None) -> Union[str, None]:
     """Display a message in a popup window with a text entry. Return the text entered."""
     result = None
     win = eg.Window(title, layout=[
         [eg.Text(message)],
         [eg.Input(default, key="-user-", width=40)],
         [eg.Button("OK", width=9), eg.Button("Cancel", width=9)]
     ], modal=True, font=font)
@@ -147,15 +148,23 @@
     """Display a message in a popup window with an warning icon."""
     messagebox.showwarning(title, message)
 
 def popup_info(message: str, title: str="Warning") -> None:
     """Display a message in a popup window with an warning icon."""
     messagebox.showwarning(title, message)
 
-def popup_get_file(message: str="", title: str|None=None, initial_folder: str="", save_as: bool=False, multiple_files: bool=False, file_types: tuple[tuple[str, str]]=(("All Files", "*.*"),), no_window: bool|None=None, **kw) -> (str|tuple[str]|None):
+def popup_get_file(
+        message: str="",
+        title: Union[str, None] = None,
+        initial_folder: str = "",
+        save_as: bool = False, # show `save as` dialog
+        multiple_files: bool = False, # can select multiple files
+        file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
+        no_window: Union[bool, None] = None, # for compatibility
+        **kw) -> Union[str, tuple[str], None]:
     """Popup a file selection dialog. Return the file selected."""
     if title is None:
         title = message
     if save_as:
         result = filedialog.asksaveasfilename(
             title=title,
             initialdir=initial_folder,
@@ -166,21 +175,33 @@
             title=title, 
             initialdir=initial_folder,
             filetypes=file_types,
             multiple=multiple_files, # type: ignore
             **kw)
     return result
 
-def popup_get_folder(message: str="", title: str|None=None, default_path: str="", no_window: bool|None=None, **kw) -> (str|None):
+def popup_get_folder(
+            message: str = "",
+            title: Union[str, None] = None,
+            default_path: str = "",
+            no_window: Union[bool, None] = None, # for compatibility
+            **kw
+            ) -> Union[str, None]:
     """Popup a folder selection dialog. Return the folder selected."""
     if title is None:
         title = message
     return filedialog.askdirectory(title=title, initialdir=default_path, **kw)
 
-def popup_scrolled(message: str, title: str = "", size: tuple[int,int]=[40, 5], readonly: bool=False, font: tuple[str, int]|None=None) -> str|None:
+def popup_scrolled(
+            message: str,
+            title: str = "",
+            size: tuple[int,int] = [40, 5],
+            readonly: bool = False,
+            font: Union[FontType, None] = None
+            ) -> Union[str, None]:
     """Display a message in a popup window with a text entry. Return the text entered."""
     win = eg.Window(title, layout=[
         [eg.Multiline(message, key="-text-", size=size, readonly=readonly, font=font)],
         [eg.Button("OK", width=9), eg.Button("Cancel", width=5)]
     ], modal=True)
     result = None
     while win.is_alive():
@@ -189,15 +210,20 @@
             result = win["-text-"].get()
             break
         if event == "Cancel":
             break
     win.close()
     return result
 
-def popup_get_date(message: str = "", title: str = "", current_date:datetime|None=None, font: tuple[str, int]|None=None) -> datetime|None:
+def popup_get_date(
+        message: str = "",
+        title: str = "",
+        current_date: Union[datetime, None] = None,
+        font: Union[tuple[str, int], None] = None
+        ) -> Union[datetime, None]:
     """Display a calendar in a popup window. Return the datetime entered or None."""
     if current_date is None:
         current_date = datetime.now()
     # week names
     week_names = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
     week_colors = [None, None, None, None, None, "blue", "red"]
     # set
@@ -337,22 +363,29 @@
 '''
     # Execute PowerShell
     subprocess.run(["powershell", "-Command", powershell_script])
 
 #------------------------------------------------------------------------------
 # TkEasyGUI original dialogs
 
-def popup_color(title: str="", default_color: str|None=None) -> (str|None):
+def popup_color(title: str="", default_color: Union[str, None]=None) -> (Union[str, None]):
     """Popup a color selection dialog. Return the color selected."""
     col = colorchooser.askcolor(title=title, color=default_color)
     if col[1] is None:
         return default_color
     return f"{col[1]}".upper()
 
-def popup_listbox(items: list[str], message: str = "", title: str = "", size: tuple[int,int]=(20, 7), font: tuple[str, int]|None=None, multiple:bool = False) -> str|None:
+def popup_listbox(
+        items: list[str], # list of items
+        message: str = "",
+        title: str = "",
+        size: tuple[int,int] = (20, 7),
+        font: Union[FontType, None] = None,
+        multiple:bool = False # multiple selection
+        ) -> Union[str, None]:
     """Display Listbox in a popup window"""
     select_mode = eg.LISTBOX_SELECT_MODE_BROWSE if multiple is False else eg.LISTBOX_SELECT_MODE_MULTIPLE
     win = eg.Window(title, layout=[
         [eg.Text(message)],
         [eg.Listbox(values=items, key="-list-", size=size, font=font, select_mode=select_mode)],
         [eg.Button("OK", width=9), eg.Button("Cancel", width=5)]
     ], modal=True)
```

### Comparing `tkeasygui-0.2.45/TkEasyGUI/widgets.py` & `tkeasygui-0.2.46/TkEasyGUI/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 import sys
 import tkinter as tk
 import tkinter.font as tkfont
 from tkinter import scrolledtext
 from datetime import datetime
 from queue import Queue
 from tkinter import ttk
-from typing import Any, Literal, TypeAlias, Union, Generator
+from typing import Any, Literal, Union
+# from typing import TypeAlias
+
 from PIL import Image as PILImage
 from PIL import ImageTk
 
 from . import utils
+from .utils import WindowType, ElementType, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
 from . import dialogs
 
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
@@ -31,27 +34,14 @@
 LISTBOX_SELECT_MODE_EXTENDED: str = "extended"
 LISTBOX_SELECT_MODE_SINGLE: str = "single"
 TABLE_SELECT_MODE_NONE: str = tk.NONE
 TABLE_SELECT_MODE_BROWSE: str = tk.BROWSE
 TABLE_SELECT_MODE_EXTENDED: str = tk.EXTENDED
 EG_SWAP_EVENT_NAME: str = "--swap_event_name--"
 
-# type
-WindowType: TypeAlias = "Window"
-ElementType: TypeAlias = "Element"
-TextAlign: TypeAlias = Literal["left", "right", "center"]
-TextVAlign: TypeAlias = Literal["top", "bottom", "center"]
-FontType: TypeAlias = tuple[str, int] | tuple[str, int, str]
-PointType: TypeAlias = tuple[int, int] | tuple[float, float]
-EventMode: TypeAlias = Literal["user", "system"]
-OrientationType: TypeAlias = Literal["v", "h", "vertical", "horizontal"]
-ListboxSelectMode: TypeAlias = Literal["multiple", "browse", "extended", "single"]
-PadType: TypeAlias = int | tuple[int, int] | tuple[tuple[int, int], tuple[int, int]]
-ReliefType: TypeAlias = Literal["flat", "groove", "raised", "ridge", "solid", "sunken"]
-
 # about color (Thanks)
 # https://kuroro.blog/python/YcZ6Yh4PswqUzaQXwnG2/
 
 #------------------------------------------------------------------------------
 # utility
 def get_platform() -> str:
     """get platform"""
@@ -121,16 +111,16 @@
 _compatibility: bool = True
 def set_PySimpleGUI_compatibility(flag: bool=True) -> None:
     """Set compatibility with PySimpleGUI (Default=True)"""
     global _compatibility
     _compatibility = flag
 
 # only one root element
-_root_window: tk.Tk|None = None
-_ttk_style: ttk.Style|None = None
+_root_window: Union[tk.Tk, None] = None
+_ttk_style: Union[ttk.Style, None] = None
 def get_root_window() -> tk.Tk:
     """Get root window."""
     global _root_window
     if _root_window is None:
         _root_window = tk._get_default_root() # tk.Tk()
         _root_window.eval('tk::PlaceWindow . center')
         _root_window.attributes('-alpha', 0)
@@ -159,15 +149,15 @@
     global _ttk_style
     if _ttk_style is None:
         _ttk_style = ttk.Style()
     return _ttk_style
 
 # active window
 _window_list: list[WindowType] = []
-def _get_active_window() -> tk.Toplevel|None:
+def _get_active_window() -> Union[tk.Toplevel, None]:
     """Get the active window."""
     if len(_window_list) == 0:
         return None
     return _window_list[-1].window
 
 def _window_push(win: WindowType) -> None:
     """Push a window to the list."""
@@ -183,55 +173,55 @@
     """
     Main window object in TkEasyGUI
     """
     def __init__(
                 self,
                 title: str,
                 layout: list[list[ElementType]],
-                size: tuple[str, int]|None=None, 
-                resizable:bool=False,
-                font:FontType|None=None,
-                modal: bool=False, 
-                keep_on_top:bool=False, # keep on top
-                no_titlebar: bool=False, # hide titlebar
-                grab_anywhere: bool=False, # can move window by dragging anywhere
-                alpha_channel: float=1.0,
-                enable_key_events: bool=False, # enable keyboard events
-                return_keyboard_events: bool=False, # enable keyboard events (for compatibility)
+                size: Union[tuple[str, int], None] = None, 
+                resizable:bool = False,
+                font: Union[FontType, None] = None,
+                modal: bool = False, 
+                keep_on_top:bool = False, # keep on top
+                no_titlebar: bool = False, # hide titlebar
+                grab_anywhere: bool = False, # can move window by dragging anywhere
+                alpha_channel: float = 1.0,
+                enable_key_events: bool = False, # enable keyboard events
+                return_keyboard_events: bool = False, # enable keyboard events (for compatibility)
                 **kw) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = _get_active_window()
         if active_win is None:
             active_win = get_root_window()
         self.window: tk.Toplevel = tk.Toplevel(master=active_win)
-        self.timeout: int|None = None
+        self.timeout: Union[int, None] = None
         self.timeout_key: str = WINDOW_TIMEOUT
-        self.timeout_id: str|None = None
-        self.focus_timer_id: str|None = None
+        self.timeout_id: Union[str, None] = None
+        self.focus_timer_id: Union[str, None] = None
         self.events: Queue = Queue()
         self.key_elements: dict[str, Element] = {}
         self.last_values: dict[str, Any] = {}
         self.flag_alive: bool = True # Pressing the close button will turn this flag to False.
         self.layout: list[list[ElementType]] = layout
         self._event_hooks: dict[str, list[callable]] = {}
-        self.font: FontType|None = font
+        self.font: Union[FontType, None] = font
         self.radio_group_dict: dict[str, list[tk.IntVar, int]] = {}
         self.minimized: bool = False
         self.maximized: bool = False
         self.is_hidden: bool = False
         self._keep_on_top: bool = keep_on_top
         self._no_titlebar: bool = no_titlebar
         self._grab_anywhere: bool = grab_anywhere
         self._grab_flag: bool = False
-        self._start_x: int|None = None
-        self._start_y: int|None = None
-        self._mouse_x: int|None = None
-        self._mouse_y: int|None = None
+        self._start_x: Union[int, None] = None
+        self._start_y: Union[int, None] = None
+        self._mouse_x: Union[int, None] = None
+        self._mouse_y: Union[int, None] = None
         self.alpha_channel: float = alpha_channel
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
         # Frame
         self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
         # set window properties
         self.window.title(title)
@@ -404,15 +394,15 @@
         result: list[ElementType] = []
         for rows in self.layout:
             for elem in rows:
                 if elem.element_type.lower() == element_type.lower():
                     result.append(elem)
         return result
 
-    def read(self, timeout: int|None=None, timeout_key: str="-TIMEOUT-") -> tuple[str, dict[str, Any]]:
+    def read(self, timeout: Union[int, None] = None, timeout_key: str="-TIMEOUT-") -> tuple[str, dict[str, Any]]:
         """ [Window.read] Read events from the window."""
         self.timeout = timeout
         self.timeout_key = timeout_key
         time_id = time_checker_start()
         while True:
             # set timeout
             if self.timeout_id is not None:
@@ -438,15 +428,15 @@
         if key in self._event_hooks:
             flag_stop = self._dispatch_event_hooks(key, values)
             if flag_stop:
                 key = f"{key}-stopped" # change event name
                 values = self.get_values() # collect values again
         return (key, values)
     
-    def event_iter(self, timeout: int|None=None, timeout_key: str=TIMEOUT_KEY) -> Any:
+    def event_iter(self, timeout: Union[int, None] = None, timeout_key: str=TIMEOUT_KEY) -> Any:
         """
         Return generator with event and values
         **Example**
         ```py
         import TkEasyGUI as eg
         # create a window
         with eg.Window("test", layout=[[eg.Button("Hello")]]) as window:
@@ -527,15 +517,15 @@
         self.last_values = values
         return values
 
     def _window_idle_handler(self) -> None:
         """Handle window idle event."""
         _exit_mainloop()
 
-    def _event_handler(self, key: str, values: dict[str, Any]|None) -> None:
+    def _event_handler(self, key: str, values: Union[dict[str, Any], None]) -> None:
         """Handle an event."""
         # set value
         if values is None:
             values = {}
         for k, v in self.get_values().items():
             values[k] = v
         # check EG_SWAP_EVENT_NAME
@@ -714,17 +704,17 @@
 }
 class Element:
     """Element class."""
     def __init__(
             self,
             element_type: str, # element type
             ttk_style_name: str, # tkinter widget type
-            key: str|None, # key
+            key: Union[str, None], # key
             has_value: bool, # has value
-            metadata: dict[str, Any]|None=None, # meta data
+            metadata: Union[dict[str, Any], None] = None, # meta data
             **kw) -> None:
         """Create an element."""
         # define properties
         self.has_value: bool = has_value
         self.key: str|int|None = key
         if self.key is not None:
             register_element_key(self.key) # for checking unique key
@@ -735,26 +725,26 @@
         self.use_ttk: bool = True if ttk_style_name != "" else False
         self.metadata = metadata
         self.style_name: str = self._generate_style_name(key)
         self.props: dict[str, Any] = kw
         self.widget: Any|None = None
         self.expand_x: bool = False
         self.expand_y: bool = False
-        self.anchor: str|None = None
+        self.anchor: Union[str, None] = None
         self.has_children: bool = False
         self.prev_element: Element|None = None
         self.next_element: Element|None = None
         self.window: Window|None = None
         self.parent: tk.Widget|None = None
         self._bind_dict: dict[str, tuple[str, bool, EventMode]] = {}
         self.user_bind_event: tk.Event|None = None # when bind event fired then set this value
         self.vertical_alignment: TextVAlign = "center"
         self.padx: int|tuple[int,int]|None = 1
         self.pady: int|tuple[int,int]|None = None
-        self.font: FontType|None = None
+        self.font: Union[FontType, None] = None
         self.has_font_prop: bool = True
         self.col_no: int = -1
         self.row_no: int = -1
     
     def get_name(self) -> str:
         """Get element name."""
         if self.key is None:
@@ -765,15 +755,15 @@
         """
         Bind event. @see `Window.bind`
         """
         self._bind_dict[event_name] = (handle_name, propagate, event_mode)
         if self.window is not None:
             self.window.bind(self, event_name, handle_name, propagate=propagate, event_mode=event_mode)
 
-    def disptach_event(self, values: dict[str, Any]|None=None) -> None:
+    def disptach_event(self, values: Union[dict[str, Any], None] = None) -> None:
         """Dispatch event"""
         if values is None:
             values = {}
         if self.window is not None:
             self.window._event_handler(self.key, values)
     
     def _justify_to_anchor(self, justify: TextAlign) -> str:
@@ -781,16 +771,16 @@
         if justify == "left":
             return "w"
         if justify == "right":
             return "e"
         return "center"
 
     def _set_pack_props(self,
-                expand_x: bool|None=None,
-                expand_y: bool|None=None,
+                expand_x: Union[bool, None] = None,
+                expand_y: Union[bool, None] = None,
                 pad: PadType=None) ->None:
         """Set pack properties"""
         if expand_x is not None:
             self.expand_x = expand_x
         if expand_y is not None:
             self.expand_y = expand_y
         if pad is not None:
@@ -800,19 +790,19 @@
                 self.padx = pad[0]
                 self.pady = pad[1]
             else:
                 self.padx = pad[0][0]
                 self.pady = pad[0][1]
 
     def _set_text_props(self,
-                font: FontType|None=None,
-                text_align: TextAlign|None=None,
-                color: str|None=None,
-                text_color: str|None=None,
-                background_color: str|None=None) ->None:
+                font: Union[FontType, None] = None,
+                text_align: Union[TextAlign, None] = None,
+                color: Union[str, None] = None,
+                text_color: Union[str, None] = None,
+                background_color: Union[str, None] = None) -> None:
         """set default props style"""
         if font is not None:
             self.props["font"] = font
             self.font = font
         if text_align is not None:
             self.props["justify"] = text_align
         if color is not None:
@@ -952,15 +942,15 @@
             if "justify" in self.props:
                 anchor = self._justify_to_anchor(self.props.pop("justify"))
                 style.configure(style_name, anchor=anchor)
             if "height" in self.props:
                 height = self.props.pop("height")
                 self.pady = (height-1)//2
     
-    def _generate_style_name(self, style_key: str|None) -> str:
+    def _generate_style_name(self, style_key: Union[str, None]) -> str:
         """generate style name"""
         if style_key is None or style_key == "":
             style_key = generate_element_style_key(self.element_type)
         if "." in self.ttk_style_name:
             return f"{self.ttk_style_name}"
         else:
             return f"{style_key}.{self.ttk_style_name}"
@@ -985,15 +975,15 @@
         kw = self.convert_props(kw)
         try:
             if (self.widget is not None)and(len(kw) > 0):
                 self.widget.configure(**kw)
         except Exception as e:
             print(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}", file=sys.stderr)
 
-    def get_prev_widget(self, target_key: str|None=None) -> tk.Widget:
+    def get_prev_widget(self, target_key: Union[str, None] = None) -> tk.Widget:
         """Get the previous widget."""
         # check target_key
         target: tk.Widget = None
         if target_key:
             if target_key in self.window.key_elements:
                 target = self.window.key_elements[target_key]
                 return target
@@ -1025,28 +1015,28 @@
 class Frame(Element):
     """Frame element."""
     def __init__(
                 self,
                 title: str,
                 layout: list[list[Element]],
                 key: str = "",
-                size: tuple[int, int]|None=None,
+                size: Union[tuple[int, int], None] = None,
                 relief: ReliefType="groove",
                 # text props
-                font: FontType|None=None, # font
-                color: str|None=None,
-                text_color: str|None=None,
-                background_color: str|None=None,
+                font: Union[FontType, None] = None, # font
+                color: Union[str, None] = None,
+                text_color: Union[str, None] = None,
+                background_color: Union[str, None] = None,
                 label_outside: bool=False,
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                metadata: dict[str, Any]|None=None,
+                metadata: Union[dict[str, Any], None] = None,
                 use_ttk: bool=False,
                 **kw) -> None:
         style_name = "TLabelframe" if use_ttk else ""
         super().__init__("Frame", style_name, key, False, metadata, **kw)
         self.has_children = True
         self.layout = layout
         self.label_outside = label_outside
@@ -1087,25 +1077,25 @@
 
 class Column(Element):
     """Frame element."""
     def __init__(
                 self,
                 layout: list[list[Element]],
                 key: str = "",
-                background_color: str|None=None,
+                background_color: Union[str, None] = None,
                 vertical_alignment: TextVAlign="top",
-                size: tuple[int, int]|None=None,
+                size: Union[tuple[int, int], None] = None,
                 # text props
-                text_align: TextAlign|None="left", # text align
+                text_align: Union[TextAlign, None]="left", # text align
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                metadata: dict[str, Any]|None=None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Column", "TFrame", key, False, metadata, **kw)
         self.has_children = True
         self.layout = layout
         self.vertical_alignment = vertical_alignment
         self.has_font_prop = False
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
@@ -1136,29 +1126,29 @@
         return super().__getattr__(name)
 
 class Text(Element):
     """Text element."""
     def __init__(
                 self,
                 text: str = "",
-                key: str|None=None,
+                key: Union[str, None] = None,
                 enable_events: bool=False, # enabled events (click)
-                wrap_length: int|None=None, # wrap length(unit=pixel)
+                wrap_length: Union[int, None] = None, # wrap length(unit=pixel)
                 # text props
-                text_align: TextAlign|None="left", # text align
-                font: FontType|None=None, # font
-                color: str|None=None, # text color
-                text_color: str|None=None, # same as color
-                background_color: str|None=None, # background color
+                text_align: Union[TextAlign, None]="left", # text align
+                font: Union[FontType, None] = None, # font
+                color: Union[str, None] = None, # text color
+                text_color: Union[str, None] = None, # same as color
+                background_color: Union[str, None] = None, # background color
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                metadata: dict[str, Any]|None=None, # user metadata
+                metadata: Union[dict[str, Any], None] = None, # user metadata
                 **kw
                 ) -> None:
         key = text if (key is None) or (key == "") else key
         super().__init__("Text", "", key, False, metadata, **kw)
         self.props["text"] = text
         self._set_text_props(font=font, text_align=text_align, color=color, text_color=text_color, background_color=background_color)
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
@@ -1185,15 +1175,15 @@
         return self.props["text"]
     
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
         self.widget_update(text=text)
 
-    def update(self, text: str|None=None, *args, **kw) -> None:
+    def update(self, text: Union[str, None] = None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         self.widget_update(**kw)
 
 class Label(Text):
     """
@@ -1214,18 +1204,18 @@
     **Note**
     - "!label" is disabled
     - "label::-event_name-" is set event name
     - "---" is separator
     """
     def __init__(
                 self,
-                items:Any|None=None,
-                menu_definition:list[list[str|list[Any]]]|None=None,
-                key: str|None=None,
-                metadata: dict[str, Any]|None=None,
+                items: Union[Any, None] = None,
+                menu_definition: Union[list[list[Union[str,list[Any]]]], None] = None,
+                key: Union[str, None] = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Menu", "", key, False, metadata, **kw)
         self.items = menu_definition
         if items is not None:
             self.items = items
     
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
@@ -1250,15 +1240,15 @@
         if "::" in label:
             label, key = label.split("::")
         parent.add_command(
             label=label, 
             state=state,
             command=lambda : self.disptach_event({EG_SWAP_EVENT_NAME: key}))
 
-    def _create_menu(self, parent: tk.Menu, items: list[list[str|list[Any]]], level:int = 0) -> None:
+    def _create_menu(self, parent: tk.Menu, items: list[list[Union[str, list[Any]]]], level:int = 0) -> None:
         i = 0
         while i < len(items):
             item = items[i]
             if isinstance(item, int) or isinstance(item, float):
                 item = str(item)
             if isinstance(item, str):
                 # check next item
@@ -1289,43 +1279,43 @@
         return self.props["text"]
     
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
         self.widget_update(text=text)
 
-    def update(self, text: str|None=None, *args, **kw) -> None:
+    def update(self, text: Union[str, None] = None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         self.widget_update(**kw)
 
 class Button(Element):
     """Button element."""
     def __init__(
                 self,
-                button_text: str="",
-                key: str|None = None,
-                disabled: bool=None,
-                size: tuple[int, int]|None=None,
-                use_ttk_buttons: bool=False,
-                tooltip: str|None=None, # (TODO) tooltip
-                button_color: str|tuple[str, str]|None=None,
+                button_text: str = "",
+                key: Union[str, None] = None,
+                disabled: bool = None,
+                size: Union[tuple[int, int], None] = None,
+                use_ttk_buttons: bool = False,
+                tooltip: Union[str, None] = None, # (TODO) tooltip
+                button_color: Union[str, tuple[str, str], None] = None,
                 # text props
-                text_align: TextAlign|None="left", # text align
-                font: FontType|None=None, # font
-                color: str|None=None, # text color
-                text_color: str|None=None, # same as color
-                background_color: str|None=None, # background color
+                text_align: Union[TextAlign, None] = "left", # text align
+                font: Union[FontType, None] = None, # font
+                color: Union[str, None] = None, # text color
+                text_color: Union[str, None] = None, # same as color
+                background_color: Union[str, None] = None, # background color
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                metadata: dict[str, Any]|None=None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         key = button_text if (key is None) or (key == "") else key
         super().__init__("Button", "TButton", key, False, metadata, **kw)
         self.use_ttk = use_ttk_buttons # can select ttk or tk button
         self.disabled = False
         if disabled is not None:
@@ -1353,15 +1343,15 @@
         else:
             self.widget = tk.Button(
                 parent,
                 command=lambda: self.disptach_event({"event_type": "command"}),
                 **self.props)
         return self.widget
 
-    def set_button_color(self, button_color: str|tuple[str,str], update: bool=True) -> None:
+    def set_button_color(self, button_color: Union[str, tuple[str,str]], update: bool = True) -> None:
         """Set the button color."""
         props = {}
         if isinstance(button_color, tuple):
             if len(button_color) == 2:
                 props["text_color"] = button_color[0]
                 props["background_color"] = button_color[1]
             elif len(button_color) == 1:
@@ -1379,15 +1369,19 @@
         """Set the text of the widget."""
         self.props["text"] = text
         self.widget_update(text=text)
     
     def get_text(self) -> str:
         return self.props["text"]
 
-    def update(self, text: str|None=None, disabled: bool|None=None, button_color: str|tuple[str,str]|None=None, **kw) -> None:
+    def update(self,
+               text: Union[str, None] = None, 
+               disabled: Union[bool, None] = None,
+               button_color: Union[str, tuple[str,str], None] = None,
+               **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.props["text"] = text
             self.widget_update(text=text)
         if disabled is not None:
             self.set_disabled(disabled)
         if button_color is not None:
@@ -1409,18 +1403,18 @@
     pass
 
 class Checkbox(Element):
     """Checkbox element."""
     def __init__(
                 self, text: str="",
                 default: bool=False,
-                key: str|None = None,
+                key: Union[str, None] = None,
                 enable_events: bool=False,
                 # other
-                metadata: dict[str, Any]|None=None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         if key is None or key == "":
             key = text
         super().__init__("Checkbox", "TCheckbutton", key, True, metadata, **kw)
         self.default_value = default
         self.props["text"] = text
         if enable_events:
@@ -1463,20 +1457,20 @@
             self.set_value(kw.pop("value"))
         self.widget_update(**kw)
 
 class Radio(Element):
     """Checkbox element."""
     def __init__(
                 self, text: str="",
-                group_id: int|str="group",
-                default: bool=False,
-                key: str|None = None,
-                enable_events: bool=False,
+                group_id: Union[int, str] = "group",
+                default: bool = False,
+                key: Union[str, None] = None,
+                enable_events: bool = False,
                 # other
-                metadata: dict[str, Any]|None=None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         if key is None or key == "":
             key = text
         super().__init__("Radio", "TRadiobutton", key, True, metadata, **kw)
         self.default_value = default
         self.value: int = 0
         self.props["text"] = text
@@ -1522,47 +1516,47 @@
         return self.is_selected()
 
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
         self.widget_update(text=text)
 
-    def update(self, text: str|None=None, **kw) -> None:
+    def update(self, text: Union[str, None] = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         self.widget_update(**kw)
 
 class Input(Element):
     """
     Text input element.
     """
     def __init__(
                 self,
                 text: str = "", # default text
-                key: str|None = None, # key
-                default_text: str|None = None, # same as text
+                key: Union[str, None] = None, # key
+                default_text: Union[str, None] = None, # same as text
                 enable_events: bool = False, # enabled events ([enter] or [change])
                 enable_key_events: bool = False,  # enabled key events
                 enable_focus_events: bool = False, # enabled focus events
-                readonly_background_color: str|None = "silver",
-                password_char: str|None = None, # if you want to use it as a password input box, set "*"
+                readonly_background_color: Union[str, None] = "silver",
+                password_char: Union[str, None] = None, # if you want to use it as a password input box, set "*"
                 readonly: bool = False, # read only box
                 # text props
-                text_align: TextAlign|None = "left", # text align
-                font: FontType|None = None, # font
-                color: str|None = None, # text color
-                text_color: str|None = None, # same as color
-                background_color: str|None = None, # background color
+                text_align: Union[TextAlign, None] = "left", # text align
+                font: Union[FontType, None] = None, # font
+                color: Union[str, None] = None, # text color
+                text_color: Union[str, None] = None, # same as color
+                background_color: Union[str, None] = None, # background color
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("Input", "TEntry", key, True, metadata, **kw)
         self.readonly: bool = readonly
         self.enable_events: bool = enable_events
         if default_text is not None: # compatibility with PySimpleGUI
             text = default_text
@@ -1648,15 +1642,15 @@
 
     def set_readonly(self, readonly: bool) -> None:
         """set readonly"""
         self.readonly = readonly
         state = "readonly" if self.readonly else "normal"
         self.widget_update(state=state)
 
-    def update(self, text: str|None=None, readonly: bool|None=None, **kw) -> None:
+    def update(self, text: Union[str, None] = None, readonly: Union[bool, None] = None, **kw) -> None:
         """Update the widget."""
         if self.widget is None:
             return
         # check readonly
         if readonly is not None:
             self.set_readonly(readonly)
         # text
@@ -1769,33 +1763,33 @@
     pass
 
 class Multiline(Element):
     """Multiline text input element."""
     def __init__(
                 self,
                 text: str = "", # default text
-                default_text: str|None = None, # same as text
-                key: str|None = None, # key
+                default_text: Union[str, None] = None, # same as text
+                key: Union[str, None] = None, # key
                 readonly: bool = False,
                 enable_events: bool = False, 
                 enable_key_events: bool = False,
                 enable_focus_events: bool = False,
                 size: tuple[int, int] = (50, 10), # element size (unit=character)
                 # text props
-                font: FontType|None = None, # font
-                color: str|None = None, # text color
-                text_color: str|None = None, # same as color
-                background_color: str|None = None, # background color
+                font: Union[FontType, None] = None, # font
+                color: Union[str, None] = None, # text color
+                text_color: Union[str, None] = None, # same as color
+                background_color: Union[str, None] = None, # background color
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                readonly_background_color: str|None = None,
-                metadata: dict[str, Any]|None = None,
+                readonly_background_color: Union[str, None] = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("Multiline", "", key, True, metadata, **kw)
         if default_text is not None:
             text = default_text
         self.props["text"] = text
         self.props["size"] = size
@@ -1881,15 +1875,15 @@
             return
         text = ""
         if self.widget.tag_ranges(tk.SEL):
             text = self.copy()
             self.widget.delete(tk.SEL_FIRST, tk.SEL_LAST)
         return text
 
-    def update(self, text: str|None = None, readonly: bool|None = None, **kw) -> None:
+    def update(self, text: Union[str, None] = None, readonly: Union[bool, None] = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         if readonly is not None:
             self.set_readonly(readonly)
         self.widget_update(**kw)
 
@@ -2018,15 +2012,15 @@
             return
         text: tk.Text = self.widget
         text.tag_add(tk.SEL, "1.0", tk.END)
         text.mark_set(tk.INSERT, '1.0')
         self.widget.see(tk.INSERT)
         print("@select_all")
 
-    def print(self, text: str, text_color: str|None=None, background_color: str|None=None, end:str="\n") -> None:
+    def print(self, text: str, text_color: Union[str, None] = None, background_color: Union[str, None] = None, end:str="\n") -> None:
         """Print text."""
         text += end
         if self.widget is None:
             return
         tags: list[str] = []
         if text_color is not None:
             tag = generate_element_style_key("--multiline-text_color")
@@ -2046,22 +2040,22 @@
     """Output element. (alias of Multiline) TODO: implement"""
     pass
 
 class Slider(Element):
     """Slider element."""
     def __init__(
                 self,
-                key: str|None = None,
+                key: Union[str, None] = None,
                 range: tuple[float, float] = (1, 10),
                 orientation: OrientationType = "horizontal",
-                resolution: float|None = None,
-                default_value: float|None = None,
+                resolution: Union[float, None] = None,
+                default_value: Union[float, None] = None,
                 enable_events: bool = False,
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         style_name = "Horizontal.TScale" if (orientation == "h" or orientation == "horizontal") else "Vertical.TScale"
         super().__init__("Slider", style_name, key, True, metadata, **kw)
         self.has_value = True
         self.has_font_prop = False
         self.range = range
         self.resolution = resolution # dummy @see Slider.create
@@ -2091,32 +2085,32 @@
             **self.props)
         return self.widget
     
     def get(self) -> Any:
         """Return Widget"""
         return self.scale_var.get()
 
-    def update(self, value: float|None=None, **kw) -> None:
+    def update(self, value: Union[float, None]=None, **kw) -> None:
         """Update the widget."""
         if value is not None:
             self.scale_var.set(value)
             self.disptach_event()
         else:
             self.widget_update(**kw)
 
 class Canvas(Element):
     """Canvas element."""
     def __init__(
                 self,
-                key: str|None = None,
+                key: Union[str, None] = None,
                 enable_events: bool = False,
-                background_color: str|None = None,
+                background_color: Union[str, None] = None,
                 size: tuple[int, int] = (300, 300),
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Canvas", "", key, False, metadata, **kw)
         self.props["size"] = size
         self.has_font_prop = False
         if background_color:
             self.props["background"] = background_color
         if enable_events:
@@ -2143,22 +2137,22 @@
         if name in ["Widget", "tk_canvas", "TKCanvas"]: # compatibility with PySimpleGUI
             return self.widget
         return super().__getattr__(name)
 
 class Graph(Element):
     """Graph element."""
     def __init__(
-            self, key: str|None = None,
-            background_color: str|None = None,
+            self, key: Union[str, None] = None,
+            background_color: Union[str, None] = None,
             size: tuple[int, int]=(300, 300),
-            canvas_size: tuple[int, int]|None = None,
-            graph_bottom_left: tuple[int, int]|None = None,
-            graph_top_right: tuple[int, int]|None = None,
+            canvas_size: Union[tuple[int, int], None] = None,
+            graph_bottom_left: Union[tuple[int, int], None] = None,
+            graph_top_right: Union[tuple[int, int], None] = None,
             # other
-            metadata: dict[str, Any]|None = None,
+            metadata: Union[dict[str, Any], None] = None,
             **kw) -> None:
         super().__init__("Graph", "", key, False, metadata, **kw)
         self.has_font_prop = False
         # <Coordinate> graph_Declared for compatibility, but not yet implemented.
         self.graph_bottom_left = graph_bottom_left
         self.graph_top_right = graph_top_right
         # </Coordinate>
@@ -2200,68 +2194,68 @@
     
     def draw_point(self, point: PointType, size: int = 2, color: str = 'black') -> int:
         """Draw a point."""
         x, y = point
         size2: float = size / 2
         return self.widget.create_oval(x-size2, y-size2, x+size2, y+size2, fill=color)
     
-    def draw_circle(self, center_location: PointType, radius: int|float, fill_color: str|None = None, line_color: str|None = 'black', line_width: int = 1) -> int:
+    def draw_circle(self, center_location: PointType, radius: Union[int, float], fill_color: Union[str, None] = None, line_color: Union[str, None] = 'black', line_width: int = 1) -> int:
         """Draw a circle."""
         x, y = center_location
         return self.widget.create_oval(x-radius, y-radius, x+radius, y+radius, fill=fill_color, outline=line_color, width=line_width)
 
-    def draw_oval(self, top_left: PointType, bottom_right: PointType, fill_color: str|None = None, line_color: str|None = None, line_width: int = 1):
+    def draw_oval(self, top_left: PointType, bottom_right: PointType, fill_color: Union[str, None] = None, line_color: Union[str, None] = None, line_width: int = 1):
         """Draw an oval."""
         return self.widget.create_oval(top_left, bottom_right, fill=fill_color, outline=line_color, width=line_width)
     
-    def draw_arc(self, top_left: PointType, bottom_right: PointType, extent: int|None = None, start_angle: int|None = None, style: str|None = None, arc_color: str|None = 'black', line_width: int = 1, fill_color: str|None = None) -> int:
+    def draw_arc(self, top_left: PointType, bottom_right: PointType, extent: Union[int, None] = None, start_angle: Union[int, None] = None, style: Union[str, None] = None, arc_color: Union[str, None] = 'black', line_width: int = 1, fill_color: Union[str, None] = None) -> int:
         """Draw an arc."""
         return self.widget.create_arc(top_left, bottom_right, extent=extent, start=start_angle, style=style, outline=arc_color, width=line_width, fill=fill_color)
     
     def erase(self) -> None:
         """Delete all"""
         self.widget.delete("all")
     
-    def draw_rectangle(self, top_left: PointType, bottom_right: PointType, fill_color: str|None=None, line_color: str|None=None, line_width: int|None=None) -> int:
+    def draw_rectangle(self, top_left: PointType, bottom_right: PointType, fill_color: Union[str, None] = None, line_color: Union[str, None] = None, line_width: Union[int, None] = None) -> int:
         """Draw rectangle"""
         return self.widget.create_rectangle(top_left[0], top_left[1], bottom_right[0], bottom_right[1], fill=fill_color, outline=line_color, width=line_width)
     
-    def draw_polygon(self, points: list[PointType], fill_color: str|None=None, line_color: str|None=None, line_width: int|None=None) -> None:
+    def draw_polygon(self, points: list[PointType], fill_color: Union[str, None] = None, line_color: Union[str, None] = None, line_width: Union[int, None] = None) -> None:
         """Draw polygon"""
         return self.widget.create_polygon(points, fill=fill_color, outline=line_color, width=line_width)
     
-    def draw_text(self, text: str, location: PointType, color: str|None='black', font: FontType=None, angle: float|str|None=0, text_location: TextAlign=tk.CENTER) -> int:
+    def draw_text(self, text: str, location: PointType, color: Union[str, None]='black', font: FontType = None, angle: Union[float, str, None] = 0, text_location: TextAlign = tk.CENTER) -> int:
         """Draw text"""
         x, y = location
         anchor = {"left": "w", "right": "e", "center": "center"}[text_location]
         return self.widget.create_text(x, y, text=text, font=font, fill=color, angle=angle, anchor=anchor)
     
-    def draw_image(self, filename: str|None=None, data: bytes|None=None, location: PointType|None=None) -> int:
+    def draw_image(self, filename: Union[str, None] = None, data: Union[bytes, None] = None, location: Union[PointType, None] = None) -> int:
         """Draw image"""
         # check location
         if location is None:
             location = (0, 0)
         # load image
         image: tk.PhotoImage|None = get_image_tk(filename=filename, data=data)
         # important
         self.widget.image = image # type: ignore
         return self.widget.create_image(location, image=image, anchor=tk.NW)
 
 class Image(Element):
     """Image element."""
     def __init__(
                 self,
-                source: bytes|str|None = None, # image source
+                source: Union[bytes, str, None] = None, # image source
                 filename = None, # filen ame
                 data: bytes = None, # image data
-                key: str|None = None,
-                background_color: str|None = None,
+                key: Union[str, None] = None,
+                background_color: Union[str, None] = None,
                 size: tuple[int, int] = (300, 300),
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Image", "", key, False, metadata, **kw)
         self.has_font_prop = False
         self.source = source
         self.filename = filename
         self.data = data
         self.size = self.props["size"] = size
@@ -2281,29 +2275,37 @@
         """Return Widget"""
         return self.widget
 
     def erase(self) -> None:
         """Erase image"""
         self.widget.delete("all")
 
-    def set_image(self, source: bytes|str=None, filename: str|None=None, data: bytes|None=None) -> None:
+    def set_image(self,
+            source: Union[bytes, str, None] = None,
+            filename: Union[str, None] = None,
+            data: Union[bytes, None]=None) -> None:
         if self.widget is None:
             return
         # set 
         self.filename = filename
         self.data = data
         # erase
         self.erase()
         # load
         photo = get_image_tk(source, filename, data, self.size)
         if photo is not None:
             self.widget.create_image(0, 0, image=photo, anchor="nw")
             self.widget.photo = photo # type ignore
 
-    def update(self, source: bytes|str=None, filename: str|None=None, data: bytes|None=None, size: tuple[int,int]|None=None, **kw) -> None:
+    def update(self,
+               source: Union[bytes, str, None] = None,
+               filename: Union[str, None] = None,
+               data: Union[bytes, None] = None,
+               size: Union[tuple[int,int], None] = None,
+               **kw) -> None:
         """Update the widget."""
         if size is not None:
             self.size = size
             self.widget.configure(width=size[0], height=size[1])
         if (source is not None) or (filename is not None) or (data is not None):
             self.set_image(source, filename, data)
         self.widget_update(**kw)
@@ -2314,20 +2316,20 @@
             return self.widget
         return super().__getattr__(name)
 
 class VSeparator(Element):
     """VSeparator element."""
     def __init__(
                 self,
-                key: str|None = None,
-                background_color: str|None = None,
+                key: Union[str, None] = None,
+                background_color: Union[str, None] = None,
                 pad: PadType = 5,
                 size: tuple[int, int]=(5, 100),
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("VSeparator", "TSeparator", key, False, metadata, **kw)
         size = (pad, size[1])
         self.size = self.props["size"] = size
         self.props["padx"] = pad
         if background_color is not None:
             self.props["background"] = background_color
@@ -2337,20 +2339,20 @@
         self.widget = ttk.Separator(parent, orient="vertical")
         return self.widget
 
 class HSeparator(Element):
     """HSeparator element."""
     def __init__(
                 self,
-                key: str|None = None,
-                background_color: str|None = None,
+                key: Union[str, None] = None,
+                background_color: Union[str, None] = None,
                 pad: PadType = 5,
                 size: tuple[int, int] = (100, 5),
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("HSeparator", "TSeparator", key, False, metadata, **kw)
         size = (size[1], pad)
         self.size = self.props["size"] = size
         self.props["pady"] = pad
         if background_color is not None:
             self.props["background"] = background_color
@@ -2363,19 +2365,19 @@
 
 class Listbox(Element):
     """Listbox element."""
     def __init__(
                 self,
                 values: list[str] = [],
                 default_values: list[str] = [],
-                key: str|None = None,
+                key: Union[str, None] = None,
                 enable_events: bool = False,
                 select_mode: ListboxSelectMode = LISTBOX_SELECT_MODE_BROWSE,
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Listbox", "", key, True, metadata, **kw)
         self.values = values
         self.select_mode = select_mode
         self.default_values = default_values
         # event
         if enable_events:
@@ -2439,18 +2441,18 @@
 
 class Combo(Element):
     """Combo element."""
     def __init__(
                 self,
                 values: list[str]=[],
                 default_value: str="",
-                key: str|None = None,
+                key: Union[str, None] = None,
                 enable_events: bool = False,
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Combo", "TCombobox", key, True, metadata, **kw)
         self.values = values
         self.value: tk.StringVar|None = None
         self.default_value = default_value
         # event
         if enable_events:
@@ -2495,34 +2497,34 @@
 
 class Table(Element):
     """Table element."""
     def __init__(
                 self,
                 values: list[list[str]] = [],
                 headings: list[str] = [],
-                key: str|None = None,
+                key: Union[str, None] = None,
                 justification: TextAlign = "center",
                 auto_size_columns: bool = True,
                 max_col_width: int = 0,
-                col_widths: list[int]|None = None,
+                col_widths: Union[list[int], None] = None,
                 enable_events: bool = False,
-                event_returns_values: bool|None = None, # Returns the table value if set to True, otherwise returns the index.
+                event_returns_values: Union[bool, None] = None, # Returns the table value if set to True, otherwise returns the index.
                 select_mode: str="browse",
                 # text props
-                text_align: TextAlign|None = "left", # text align
-                font: FontType|None = None, # font
-                color: str|None = None, # text color
-                text_color: str|None = None, # same as color
-                background_color: str|None = None, # background color
+                text_align: Union[TextAlign, None] = "left", # text align
+                font: Union[FontType, None] = None, # font
+                color: Union[str, None] = None, # text color
+                text_color: Union[str, None] = None, # same as color
+                background_color: Union[str, None] = None, # background color
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
-                pad: PadType|None = None,
+                pad: Union[PadType, None] = None,
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         """Create a table."""
         # super().__init__("Table", "Treeview", key, metadata, **kw)
         super().__init__("Table", "", key, True, metadata, **kw)
         self.values = values
         self.headings = headings
         self.enable_events = enable_events
@@ -2649,23 +2651,23 @@
 #------------------------------------------------------------------------------
 # Browse elements
 
 class FileBrowse(Element):
     """FileBrowse element."""
     def __init__(
                 self, button_text: str="...",
-                key: str|None = None,
+                key: Union[str, None] = None,
                 title: str = "",
-                target_key: str|None = None,
+                target_key: Union[str, None] = None,
                 file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
                 multiple_files: bool = False,
-                initial_folder: str|None = None,
+                initial_folder: Union[str, None] = None,
                 save_as: bool = False,
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("FileBrowse", "", key, False, metadata, **kw)
         self.target_key = target_key
         self.title = title
         self.file_types = file_types
         self.save_as = save_as
@@ -2694,15 +2696,15 @@
                 target_text = str(target.get())
             except Exception:
                 target_text = ""
             if target_text != "":
                 init_dir = os.path.dirname(target_text)
         return init_dir
 
-    def show_dialog(self, *args) -> str|None:
+    def show_dialog(self, *args) -> Union[str, None]:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # get initial directory
         init_dir = self._get_initial_directory()
         # popup
         result = dialogs.popup_get_file(
             title=self.title,
@@ -2718,31 +2720,31 @@
         return result
     
     def set_text(self, text: str) -> None:
         """Set the text of the button."""
         self.props["text"] = text
         self.widget_update(text=text)
 
-    def update(self, text: str|None=None, **kw) -> None:
+    def update(self, text: Union[str, None] = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         self.widget_update(**kw)
 
 class FilesBrowse(FileBrowse):
     """FilesBrowse element."""
     def __init__(
                 self,
                 button_text: str = "...",
-                key: str|None = None,
-                target_key: str|None = None,
+                key: Union[str, None] = None,
+                target_key: Union[str, None] = None,
                 title: str="",
                 file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("FilesBrowse", "", key, False, metadata, **kw)
         self.target_key = target_key
         self.title = title
         self.file_types = file_types
         self.props["text"] = button_text
@@ -2751,20 +2753,20 @@
         self.save_as = False
 
 class FileSaveAsBrowse(FileBrowse):
     """FileSaveAsBrowse element."""
     def __init__(
                 self,
                 button_text: str="...",
-                key: str|None = None,
-                target_key: str|None = None,
+                key: Union[str, None] = None,
+                target_key: Union[str, None] = None,
                 title: str = "",
                 file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("FileSaveAsBrowse", "", key, False, metadata, **kw)
         self.target_key = target_key
         self.title = title
         self.file_types = file_types
         self.props["text"] = button_text
@@ -2777,29 +2779,29 @@
     pass
 
 class FolderBrowse(FileBrowse):
     """FolderBrowse element."""
     def __init__(
                 self,
                 button_text: str="...",
-                key: str|None = None,
-                target_key: str|None = None,
-                default_path: str|None = None,
+                key: Union[str, None] = None,
+                target_key: Union[str, None] = None,
+                default_path: Union[str, None] = None,
                 title: str = "",
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("FolderBrowse", "", key, False, metadata, **kw)
         self.target_key = target_key
         self.title = title
         self.default_path = default_path
         self.props["text"] = button_text
     
-    def show_dialog(self, *args) -> str|None:
+    def show_dialog(self, *args) -> Union[str, None]:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # popup
         result = dialogs.popup_get_folder(
             title=self.title,
             default_path=self.default_path,
         )
@@ -2808,29 +2810,29 @@
         return result
 
 class ColorBrowse(FileBrowse):
     """FolderBrowse element."""
     def __init__(
                 self,
                 button_text: str="...",
-                key: str|None = None,
-                target_key: str|None = None,
-                default_color: str|None = None,
+                key: Union[str, None] = None,
+                target_key: Union[str, None] = None,
+                default_color: Union[str, None] = None,
                 title: str="",
                 # other
-                metadata: dict[str, Any]|None = None,
+                metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("FolderBrowse", "", key, False, metadata, **kw)
         self.target_key = target_key
         self.title = title
         self.default_color = default_color
         self.props["text"] = button_text
     
-    def show_dialog(self, *args) -> str|None:
+    def show_dialog(self, *args) -> Union[str, None]:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # popup
         result = dialogs.popup_color(
             title=self.title,
             default_color=self.default_color,
         )
@@ -2887,15 +2889,19 @@
     if size[0] < size[1]:
         r = size[0] / img.size[0]
     else:
         r = size[1] / img.size[1]
     w, h = size[0], int(img.size[1] * r)
     return img.resize(size=(w, h))
 
-def get_image_tk(source: bytes|str|None=None, filename: str|None = None, data: bytes|None = None, size: tuple[int, int]|None = None) -> tk.PhotoImage|None:
+def get_image_tk(
+        source: Union[bytes, Union[str, None]] = None,
+        filename: Union[str, None] = None,
+        data: Union[bytes, None] = None,
+        size: Union[tuple[int, int], None] = None) -> Union[tk.PhotoImage, None]:
     """Get Image for tk"""
     # if source is bytes, set data
     if source is not None:
         if isinstance(source, str): # is filename
             filename = source
         else: # is data
             data = source
```

### Comparing `tkeasygui-0.2.45/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.46/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.45
+Version: 0.2.46
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -30,22 +30,21 @@
 Project-URL: Documentation, https://github.com/kujirahand/tkeasygui-python/blob/main/README.md
 Project-URL: Repository, https://github.com/kujirahand/tkeasygui-python/
 Project-URL: Issues, https://github.com/kujirahand/tkeasygui-python/issues
 Keywords: GUI,Tkinter,PySimpleGUI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: pyperclip
 
 # TkEasyGUI
 
@@ -120,25 +119,36 @@
 
 ## Samples
 
 We have prepared a selection of samples to demonstrate simple usage. Please check them out.
 
 - [samples](https://github.com/kujirahand/tkeasygui-python/tree/main/tests).
 
+Running `tests/file_viewer.py` allows all samples to be easily launched.
+
 ## Documents
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
 ## About the relationship with PySimpleGUI
 
 - When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
 - The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
 - This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
 - We are not considering full compatibility with PySimpleGUI.
 
+### TkEasyGUI features:
+
+- Using a `for` loop and `window.event_iter()` enables straightforward event processing.
+- Custom popup dialogs, such as a color selection dialog (`eg.popup_color`), are available.
+- The `Image` class supports not only PNG but also JPEG formats.
+- Convenient event hooks and features for bulk event registration are provided - [docs/custom_events](docs/custom_events.md).
+- Methods such as Copy, Paste, and Cut are added to text boxes (Multiline/Input).
+- The system's default color scheme is utilized.
+
 ## Link
 
 - [pypi.org > TkEasyGUI](https://pypi.org/project/tkeasygui/)
 - [GitHub > TkEasyGUI](https://github.com/kujirahand/tkeasygui-python/)
```

### Comparing `tkeasygui-0.2.45/pyproject.toml` & `tkeasygui-0.2.46/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.45"
+version = "0.2.46"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
 ]
 maintainers = [
  { name="kujirahand", email="web@kujirahand.com" },
 ]
 description = "TkEasyGUI is simple GUI Library for Python3 with Tkinter"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["GUI", "Tkinter", "PySimpleGUI"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: User Interfaces",
 ]
```

