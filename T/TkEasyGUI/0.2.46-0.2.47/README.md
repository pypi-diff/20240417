# Comparing `tmp/tkeasygui-0.2.46.tar.gz` & `tmp/tkeasygui-0.2.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.46.tar", last modified: Tue Apr 16 15:15:53 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.47.tar", last modified: Wed Apr 17 09:16:08 2024, max compression
```

## Comparing `tkeasygui-0.2.46.tar` & `tkeasygui-0.2.47.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 15:15:53.183107 tkeasygui-0.2.46/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.46/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-16 15:15:53.182860 tkeasygui-0.2.46/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     3578 2024-04-16 00:24:05.000000 tkeasygui-0.2.46/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 15:15:53.180883 tkeasygui-0.2.46/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.46/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    17350 2024-04-16 15:05:05.000000 tkeasygui-0.2.46/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      825 2024-04-16 14:26:56.000000 tkeasygui-0.2.46/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-16 15:15:27.000000 tkeasygui-0.2.46/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   109812 2024-04-16 14:46:52.000000 tkeasygui-0.2.46/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 15:15:53.182578 tkeasygui-0.2.46/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-16 15:15:53.000000 tkeasygui-0.2.46/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-16 15:10:23.000000 tkeasygui-0.2.46/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-16 15:15:53.183170 tkeasygui-0.2.46/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 09:16:08.102162 tkeasygui-0.2.47/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.47/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-17 09:16:08.101961 tkeasygui-0.2.47/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     3578 2024-04-16 00:24:05.000000 tkeasygui-0.2.47/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 09:16:08.099803 tkeasygui-0.2.47/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.47/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    17342 2024-04-16 15:46:28.000000 tkeasygui-0.2.47/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      844 2024-04-16 15:46:10.000000 tkeasygui-0.2.47/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-17 09:16:06.000000 tkeasygui-0.2.47/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   112752 2024-04-17 09:15:28.000000 tkeasygui-0.2.47/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 09:16:08.101695 tkeasygui-0.2.47/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-17 09:16:02.000000 tkeasygui-0.2.47/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-17 09:16:08.102207 tkeasygui-0.2.47/setup.cfg
```

### Comparing `tkeasygui-0.2.46/LICENSE` & `tkeasygui-0.2.47/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.46/PKG-INFO` & `tkeasygui-0.2.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.46
+Version: 0.2.47
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.46/README.md` & `tkeasygui-0.2.47/README.md`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.46/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.47/TkEasyGUI/dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import tkinter.filedialog as filedialog
 import tkinter.messagebox as messagebox
 from datetime import datetime, timedelta
 from tkinter import colorchooser
 from typing import Union
 
-from .utils import WindowType, ElementType, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
+from .utils import Window, Element, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
 from . import widgets as eg
 
 #------------------------------------------------------------------------------
 # Dialogs
 #------------------------------------------------------------------------------
 # like PySimpleGUI
```

### Comparing `tkeasygui-0.2.46/TkEasyGUI/utils.py` & `tkeasygui-0.2.47/TkEasyGUI/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Literal, Union
+from typing import Literal, Union, TypeVar
 import pyperclip
 
 # define TypeAlias
-WindowType = "Window"
-ElementType = "Element"
+Window = TypeVar("Window")
+Element = TypeVar("Element")
 TextAlign = Literal["left", "right", "center"]
 TextVAlign = Literal["top", "bottom", "center"]
 FontType = Union[tuple[str, int], tuple[str, int, str]]
 PointType = Union[tuple[int, int], tuple[float, float]]
 EventMode = Literal["user", "system"]
 OrientationType = Literal["v", "h", "vertical", "horizontal"]
 ListboxSelectMode = Literal["multiple", "browse", "extended", "single"]
```

### Comparing `tkeasygui-0.2.46/TkEasyGUI/widgets.py` & `tkeasygui-0.2.47/TkEasyGUI/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 """
 import io
 import os
 import platform
 import sys
 import tkinter as tk
 import tkinter.font as tkfont
+from tkinter import font as tkinter_font
 from tkinter import scrolledtext
 from datetime import datetime
 from queue import Queue
 from tkinter import ttk
 from typing import Any, Literal, Union
 # from typing import TypeAlias
 
 from PIL import Image as PILImage
 from PIL import ImageTk
 
 from . import utils
-from .utils import WindowType, ElementType, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
+from .utils import Window, Element, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
 from . import dialogs
 
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
@@ -148,39 +149,39 @@
     """Get ttk style"""
     global _ttk_style
     if _ttk_style is None:
         _ttk_style = ttk.Style()
     return _ttk_style
 
 # active window
-_window_list: list[WindowType] = []
+_window_list: list[Window] = []
 def _get_active_window() -> Union[tk.Toplevel, None]:
     """Get the active window."""
     if len(_window_list) == 0:
         return None
     return _window_list[-1].window
 
-def _window_push(win: WindowType) -> None:
+def _window_push(win: Window) -> None:
     """Push a window to the list."""
     _window_list.append(win)
 
-def _window_pop(win: WindowType) -> None:
+def _window_pop(win: Window) -> None:
     """Pop a window from the list."""
     i = _window_list.index(win)
     if i >= 0:
         _window_list.pop()
 
 class Window:
     """
     Main window object in TkEasyGUI
     """
     def __init__(
                 self,
                 title: str,
-                layout: list[list[ElementType]],
+                layout: list[list[Element]],
                 size: Union[tuple[str, int], None] = None, 
                 resizable:bool = False,
                 font: Union[FontType, None] = None,
                 modal: bool = False, 
                 keep_on_top:bool = False, # keep on top
                 no_titlebar: bool = False, # hide titlebar
                 grab_anywhere: bool = False, # can move window by dragging anywhere
@@ -199,15 +200,15 @@
         self.timeout_key: str = WINDOW_TIMEOUT
         self.timeout_id: Union[str, None] = None
         self.focus_timer_id: Union[str, None] = None
         self.events: Queue = Queue()
         self.key_elements: dict[str, Element] = {}
         self.last_values: dict[str, Any] = {}
         self.flag_alive: bool = True # Pressing the close button will turn this flag to False.
-        self.layout: list[list[ElementType]] = layout
+        self.layout: list[list[Element]] = layout
         self._event_hooks: dict[str, list[callable]] = {}
         self.font: Union[FontType, None] = font
         self.radio_group_dict: dict[str, list[tk.IntVar, int]] = {}
         self.minimized: bool = False
         self.maximized: bool = False
         self.is_hidden: bool = False
         self._keep_on_top: bool = keep_on_top
@@ -217,14 +218,15 @@
         self._start_x: Union[int, None] = None
         self._start_y: Union[int, None] = None
         self._mouse_x: Union[int, None] = None
         self._mouse_y: Union[int, None] = None
         self.alpha_channel: float = alpha_channel
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
+        self.font_size_average: tuple[int, int] = (12, 10)
         # Frame
         self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         if size is not None:
             self.window.geometry(f"{size[0]}x{size[1]}")
@@ -238,14 +240,16 @@
             self.window.attributes("-topmost", True)
         if no_titlebar:
             self.hide_titlebar(True)
         if grab_anywhere:
             self.set_grab_anywhere(True)
         if alpha_channel < 1.0:
             self.set_alpha_channel(alpha_channel)
+        # font
+        self.calc_font_size(font)
         # bind events
         if self.enable_key_events:
             self.window.bind("<Key>", lambda e: self._event_handler(
                 WINDOW_KEY_EVENT,
                 {"event": e, "key": e.keysym, "event_type": "key"}))
         if self.return_keyboard_events: # for compatibility with PySimpleGUI
             self.window.bind("<Key>", lambda e: self._event_handler(
@@ -376,26 +380,43 @@
                     row_prop["pady"] = elem.pady
             # add row
             frame_row.pack(**row_prop)
         # end of create
         if self.need_focus_widget is not None:
             self.need_focus_widget.focus_set()
 
+    def calc_font_size(self, font: FontType) -> None:
+        """Calculate font size."""
+        font_obj = tkinter_font.Font()
+        if font is not None:
+            if len(font) >= 2:
+                font_obj = tkinter_font.Font(family=font[0], size=font[1])
+            elif len(font) == 1:
+                font_obj = tkinter_font.Font(family=font[0])
+        # calc measure
+        # The letter 'M' is commonly used to represent the average width of a font in typography. This is because the 'M' is relatively wide, making it suitable for indicating width in comparison to other characters, especially in fixed-width (monospace) fonts.
+        m_size = font_obj.measure("M")
+        s_size = font_obj.measure("s")
+        a_size = font_obj.measure("A")
+        w = (m_size + s_size + a_size) // 3
+        h = font_obj.metrics("linespace")
+        self.font_size_average = (w, h)
+ 
     def move_to_center(self) -> None:
         """Move the window to the center of the screen."""
         if isinstance(self.window, tk.Tk):
             self.window.eval('tk::PlaceWindow . center')
 
-    def get_element_by_key(self, key: str) -> Union[ElementType, None]:
+    def get_element_by_key(self, key: str) -> Union[Element, None]:
         """Get an element by its key."""
         return self.key_elements[key] if key in self.key_elements else None
     
-    def get_elements_by_type(self, element_type: str) -> list[ElementType]:
+    def get_elements_by_type(self, element_type: str) -> list[Element]:
         """Get elements by type."""
-        result: list[ElementType] = []
+        result: list[Element] = []
         for rows in self.layout:
             for elem in rows:
                 if elem.element_type.lower() == element_type.lower():
                     result.append(elem)
         return result
 
     def read(self, timeout: Union[int, None] = None, timeout_key: str="-TIMEOUT-") -> tuple[str, dict[str, Any]]:
@@ -879,15 +900,15 @@
         return result
 
     def set_disabled(self, disabled: bool) -> None:
         self.disabled = disabled
         state = tk.DISABLED if disabled else tk.NORMAL
         self.widget_update(state=state)
 
-    def bind_events(self, events: dict[str, str], event_mode: EventMode="user") -> ElementType:
+    def bind_events(self, events: dict[str, str], event_mode: EventMode="user") -> Element:
         """
         Bind user events
         **Example**
         ```
         # (1) bind events in the constructor
         eg.Canvas(key="-canvas-", bind_events={"<ButtonPress>": "on", "<ButtonRelease>": "off"})
         # (2) bind events in the method
@@ -2040,64 +2061,111 @@
     """Output element. (alias of Multiline) TODO: implement"""
     pass
 
 class Slider(Element):
     """Slider element."""
     def __init__(
                 self,
-                key: Union[str, None] = None,
                 range: tuple[float, float] = (1, 10),
-                orientation: OrientationType = "horizontal",
-                resolution: Union[float, None] = None,
                 default_value: Union[float, None] = None,
-                enable_events: bool = False,
+                resolution: Union[float, None] = None,
+                orientation: OrientationType = "horizontal",
+                tick_interval: Union[float, None] = None, # tick marks interval on the scale
+                enable_events: bool = False, # enable changing events
+                enable_changed_events: bool = False, # enable changed event
+                disable_number_display: bool = False,
+                size: Union[tuple[int, int], None] = None, # horizontal: (bar_length, thumb_size), vertical: (thumb_size, bar_length)
+                key: Union[str, None] = None,
                 # other
+                default: Union[float, None] = None, # same as default_value
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         style_name = "Horizontal.TScale" if (orientation == "h" or orientation == "horizontal") else "Vertical.TScale"
         super().__init__("Slider", style_name, key, True, metadata, **kw)
+        # common parameters
         self.has_value = True
         self.has_font_prop = False
+        # range and resolution
         self.range = range
         self.resolution = resolution # dummy @see Slider.create
+        if tick_interval is not None:
+            self.props["tickinterval"] = tick_interval
+        # set default_value or default
         self.default_value = default_value if default_value is not None else range[0]
+        if default is not None:
+            self.default_value = default
         # check orientation
-        self.orientation: OrientationType = orientation
         if orientation == "v":
-            self.props["orient"] = "vertical"
+            orientation = "vertical"
         elif orientation == "h":
-            self.props["orient"] = "horizontal"
-        elif orientation == "vertical" or orientation == "horizontal":
-            self.props["orient"] = orientation
-        # event
-        if enable_events:
+            orientation = "horizontal"
+        self.orientation: OrientationType = orientation
+        self.props["orient"] = orientation
+        # size
+        self.slider_size = size
+        # look
+        if disable_number_display:
+            self.props["showvalue"] = 0 # hide number
+        # events
+        self.enable_events = enable_events
+        if enable_changed_events:
             self.bind_events({
                 "<ButtonRelease-1>": "release"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
+        """Create the widget."""
+        # bar size
+        if (self.slider_size is not None) and (len(self.slider_size) == 2):
+            size = self.slider_size
+            if self.orientation == "horizontal":
+                length = size[0] * win.font_size_average[0]
+                width = size[1] * win.font_size_average[1]
+            else:
+                width = size[0] * win.font_size_average[0]
+                length = size[1] * win.font_size_average[1]
+            self.props["width"] = width
+            self.props["length"] = length
+        # var
         self.scale_var = tk.DoubleVar()
         self.scale_var.set(self.default_value)
-        self.widget = ttk.Scale(
+        # command
+        command = None
+        if self.enable_events:
+            command = lambda *event: self.disptach_event({"event_type": "change", "event": event})
+        # widget
+        self.widget = tk.Scale(
             parent,
+            from_=self.range[0],
+            to=self.range[1],
+            resolution=self.resolution,
+            command=command,
             variable=self.scale_var,
-            from_=self.range[0], to=self.range[1],
-            # resolution=self.resolution, # (memo) ttk.Scale does not support resolution
             **self.props)
         return self.widget
-    
+
     def get(self) -> Any:
         """Return Widget"""
+        print(f"@[{self.key}].get=", self.scale_var.get())
         return self.scale_var.get()
+    
+    def set(self, value: float) -> None:
+        """Set the value of the widget."""
+        self._value = value
+        self.widget.set(value)
 
-    def update(self, value: Union[float, None]=None, **kw) -> None:
+    def update(self,
+               value: Union[float, None]=None,
+               disable_number_display: Union[bool, None]=None,
+               **kw) -> None:
         """Update the widget."""
+        if disable_number_display is not None:
+            self.props["showvalue"] = 0 if disable_number_display else 1
         if value is not None:
-            self.scale_var.set(value)
-            self.disptach_event()
+            self.set(value)
         else:
             self.widget_update(**kw)
 
 class Canvas(Element):
     """Canvas element."""
     def __init__(
                 self,
```

### Comparing `tkeasygui-0.2.46/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.47/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.46
+Version: 0.2.47
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.46/pyproject.toml` & `tkeasygui-0.2.47/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.46"
+version = "0.2.47"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

