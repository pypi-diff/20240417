# Comparing `tmp/flowmatic-0.1.5.tar.gz` & `tmp/flowmatic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmatic-0.1.5.tar", max compression
+gzip compressed data, was "flowmatic-0.1.6.tar", max compression
```

## Comparing `flowmatic-0.1.5.tar` & `flowmatic-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       46 2023-08-30 06:16:47.937918 flowmatic-0.1.5/README.md
--rw-r--r--   0        0        0     1532 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/Code.png
--rw-r--r--   0        0        0      838 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/File.png
--rw-r--r--   0        0        0     1346 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/Image.png
--rw-r--r--   0        0        0     2210 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/PDF.png
--rw-r--r--   0        0        0     1048 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/Table.png
--rw-r--r--   0        0        0      965 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/Text.png
--rw-r--r--   0        0        0     1207 2023-08-30 06:16:47.937918 flowmatic-0.1.5/assets/icons/Zip.png
--rw-r--r--   0        0        0       51 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/README.md
--rw-r--r--   0        0        0     1830 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/__init__.py
--rw-r--r--   0        0        0     2239 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/flowmatic.py
--rw-r--r--   0        0        0       23 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/flows/__init__.py
--rw-r--r--   0        0        0      911 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/flows/flow.py
--rw-r--r--   0        0        0       61 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/__init__.py
--rw-r--r--   0        0        0      226 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/__init__.py
--rw-r--r--   0        0        0     1207 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/check_box.py
--rw-r--r--   0        0        0     1469 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/date_select.py
--rw-r--r--   0        0        0     1220 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/display.py
--rw-r--r--   0        0        0      655 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/field.py
--rw-r--r--   0        0        0     5818 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/file_field.py
--rw-r--r--   0        0        0     1381 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/radio_group.py
--rw-r--r--   0        0        0     1693 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/fields/text_field.py
--rw-r--r--   0        0        0      665 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/forms/validation.py
--rw-r--r--   0        0        0      176 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/gui/__init__.py
--rw-r--r--   0        0        0      100 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/gui/constants.py
--rw-r--r--   0        0        0       63 2023-08-30 06:16:47.937918 flowmatic-0.1.5/flowmatic/gui/elements/__init__.py
--rw-r--r--   0        0        0      257 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/elements/element_infos.py
--rw-r--r--   0        0        0      861 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/gui.py
--rw-r--r--   0        0        0      278 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/__init__.py
--rw-r--r--   0        0        0     1571 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/element_screen.py
--rw-r--r--   0        0        0     5023 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/form_screen.py
--rw-r--r--   0        0        0      773 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/menu_screen.py
--rw-r--r--   0        0        0     5280 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/result_screen.py
--rw-r--r--   0        0        0     2146 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/screen.py
--rw-r--r--   0        0        0      690 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/screens/title_screen.py
--rw-r--r--   0        0        0       28 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/style/__init__.py
--rw-r--r--   0        0        0       99 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/style/style.py
--rw-r--r--   0        0        0     3102 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/gui/tkgui.py
--rw-r--r--   0        0        0       56 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/server.py
--rw-r--r--   0        0        0      235 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/__init__.py
--rw-r--r--   0        0        0      758 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/exceptions.py
--rw-r--r--   0        0        0     1135 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/icons.py
--rw-r--r--   0        0        0     1687 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/saved_class.py
--rw-r--r--   0        0        0       77 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/settings.py
--rw-r--r--   0        0        0      225 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/singleton.py
--rw-r--r--   0        0        0       73 2023-08-30 06:16:47.941918 flowmatic-0.1.5/flowmatic/util/user.py
--rw-r--r--   0        0        0      431 2023-08-30 06:16:47.941918 flowmatic-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 flowmatic-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1532 2024-04-17 06:42:47.608678 flowmatic-0.1.6/assets/icons/Code.png
+-rw-r--r--   0        0        0      838 2024-04-17 06:42:47.610179 flowmatic-0.1.6/assets/icons/File.png
+-rw-r--r--   0        0        0     1346 2024-04-17 06:42:47.610679 flowmatic-0.1.6/assets/icons/Image.png
+-rw-r--r--   0        0        0     2210 2024-04-17 06:42:47.611680 flowmatic-0.1.6/assets/icons/PDF.png
+-rw-r--r--   0        0        0     1048 2024-04-17 06:42:47.612680 flowmatic-0.1.6/assets/icons/Table.png
+-rw-r--r--   0        0        0      965 2024-04-17 06:42:47.613684 flowmatic-0.1.6/assets/icons/Text.png
+-rw-r--r--   0        0        0     1207 2024-04-17 06:42:47.615180 flowmatic-0.1.6/assets/icons/Zip.png
+-rw-r--r--   0        0        0     1919 2024-04-17 06:42:47.619682 flowmatic-0.1.6/flowmatic/__init__.py
+-rw-r--r--   0        0        0     2317 2024-04-17 06:42:47.620181 flowmatic-0.1.6/flowmatic/flowmatic.py
+-rw-r--r--   0        0        0       24 2024-04-17 06:42:47.622179 flowmatic-0.1.6/flowmatic/flows/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-17 06:42:47.623181 flowmatic-0.1.6/flowmatic/flows/flow.py
+-rw-r--r--   0        0        0       63 2024-04-17 06:42:47.625681 flowmatic-0.1.6/flowmatic/forms/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-17 06:42:47.627182 flowmatic-0.1.6/flowmatic/forms/fields/__init__.py
+-rw-r--r--   0        0        0     1255 2024-04-17 06:42:47.628179 flowmatic-0.1.6/flowmatic/forms/fields/check_box.py
+-rw-r--r--   0        0        0     1527 2024-04-17 06:42:47.629180 flowmatic-0.1.6/flowmatic/forms/fields/date_select.py
+-rw-r--r--   0        0        0     1266 2024-04-17 06:42:47.630179 flowmatic-0.1.6/flowmatic/forms/fields/display.py
+-rw-r--r--   0        0        0      688 2024-04-17 06:42:47.631690 flowmatic-0.1.6/flowmatic/forms/fields/field.py
+-rw-r--r--   0        0        0     6014 2024-04-17 06:42:47.632679 flowmatic-0.1.6/flowmatic/forms/fields/file_field.py
+-rw-r--r--   0        0        0     1433 2024-04-17 06:42:47.633680 flowmatic-0.1.6/flowmatic/forms/fields/radio_group.py
+-rw-r--r--   0        0        0     1755 2024-04-17 06:42:47.634679 flowmatic-0.1.6/flowmatic/forms/fields/text_field.py
+-rw-r--r--   0        0        0      685 2024-04-17 06:42:47.635679 flowmatic-0.1.6/flowmatic/forms/validation.py
+-rw-r--r--   0        0        0      182 2024-04-17 06:42:47.637679 flowmatic-0.1.6/flowmatic/gui/__init__.py
+-rw-r--r--   0        0        0      105 2024-04-17 06:42:47.638688 flowmatic-0.1.6/flowmatic/gui/constants.py
+-rw-r--r--   0        0        0       64 2024-04-17 06:42:47.640679 flowmatic-0.1.6/flowmatic/gui/elements/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-17 06:42:47.641680 flowmatic-0.1.6/flowmatic/gui/elements/element_infos.py
+-rw-r--r--   0        0        0      906 2024-04-17 06:42:47.643181 flowmatic-0.1.6/flowmatic/gui/gui.py
+-rw-r--r--   0        0        0      284 2024-04-17 06:42:47.644680 flowmatic-0.1.6/flowmatic/gui/screens/__init__.py
+-rw-r--r--   0        0        0     1611 2024-04-17 06:42:47.645680 flowmatic-0.1.6/flowmatic/gui/screens/element_screen.py
+-rw-r--r--   0        0        0     5186 2024-04-17 06:42:47.647180 flowmatic-0.1.6/flowmatic/gui/screens/form_screen.py
+-rw-r--r--   0        0        0      799 2024-04-17 06:42:47.648681 flowmatic-0.1.6/flowmatic/gui/screens/menu_screen.py
+-rw-r--r--   0        0        0     5449 2024-04-17 06:42:47.649681 flowmatic-0.1.6/flowmatic/gui/screens/result_screen.py
+-rw-r--r--   0        0        0     2230 2024-04-17 06:42:47.650680 flowmatic-0.1.6/flowmatic/gui/screens/screen.py
+-rw-r--r--   0        0        0      716 2024-04-17 06:42:47.651680 flowmatic-0.1.6/flowmatic/gui/screens/title_screen.py
+-rw-r--r--   0        0        0       29 2024-04-17 06:42:47.654180 flowmatic-0.1.6/flowmatic/gui/style/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-17 06:42:47.655182 flowmatic-0.1.6/flowmatic/gui/style/style.py
+-rw-r--r--   0        0        0     3204 2024-04-17 06:42:47.656182 flowmatic-0.1.6/flowmatic/gui/tkgui.py
+-rw-r--r--   0        0        0       54 2024-04-17 06:42:47.618679 flowmatic-0.1.6/flowmatic/README.md
+-rw-r--r--   0        0        0       61 2024-04-17 06:42:47.657183 flowmatic-0.1.6/flowmatic/server.py
+-rw-r--r--   0        0        0      247 2024-04-17 06:42:47.658679 flowmatic-0.1.6/flowmatic/util/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-17 06:42:47.659681 flowmatic-0.1.6/flowmatic/util/exceptions.py
+-rw-r--r--   0        0        0     1171 2024-04-17 06:42:47.660679 flowmatic-0.1.6/flowmatic/util/icons.py
+-rw-r--r--   0        0        0     1752 2024-04-17 06:42:47.661681 flowmatic-0.1.6/flowmatic/util/saved_class.py
+-rw-r--r--   0        0        0       82 2024-04-17 06:42:47.663182 flowmatic-0.1.6/flowmatic/util/settings.py
+-rw-r--r--   0        0        0      232 2024-04-17 06:42:47.664182 flowmatic-0.1.6/flowmatic/util/singleton.py
+-rw-r--r--   0        0        0       78 2024-04-17 06:42:47.665182 flowmatic-0.1.6/flowmatic/util/user.py
+-rw-r--r--   0        0        0      451 2024-04-17 07:46:43.010183 flowmatic-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-04-17 06:42:47.604181 flowmatic-0.1.6/README.md
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 flowmatic-0.1.6/PKG-INFO
```

### Comparing `flowmatic-0.1.5/assets/icons/Code.png` & `flowmatic-0.1.6/assets/icons/Code.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/assets/icons/File.png` & `flowmatic-0.1.6/assets/icons/File.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/assets/icons/Image.png` & `flowmatic-0.1.6/assets/icons/Image.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/assets/icons/PDF.png` & `flowmatic-0.1.6/assets/icons/PDF.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/assets/icons/Table.png` & `flowmatic-0.1.6/assets/icons/Table.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/assets/icons/Text.png` & `flowmatic-0.1.6/assets/icons/Text.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/assets/icons/Zip.png` & `flowmatic-0.1.6/assets/icons/Zip.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.5/flowmatic/flowmatic.py` & `flowmatic-0.1.6/flowmatic/flowmatic.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from .gui import GUI, TKGUI
-from .gui.screens.screen import Screen
-from .util.settings import Settings
-from .util.user import User
-from .flows.flow import Flow
-
-
-class App:
-    """Singleton for accessing GUI, settings, user and other app-wide objects.
-
-    Attributes:
-        gui (GUI): GUI interface.
-        settings (Settings): Settings.
-        user (User): User.
-
-    Args:
-        title (str, optional): Title of the app. Defaults to "Appy".
-    """
-
-    title: str = "FlowMatic"
-    gui: GUI = None  # type: ignore
-    settings: Settings
-    user: User
-
-    start_screen: Screen
-
-    def __init__(self, start_screen: type[Screen]):
-        self.gui = self.gui or TKGUI(
-            title=self.title, start_screen=start_screen, geometry="1280x720"
-        )
-        self.start_screen = start_screen()
-        self.settings = Settings.load("files/settings.json")
-        self.user = User("")
-
-    def start(self, start_screen: Screen | None = None):
-        """Start app.
-        Args:
-            screen (type[Screen]): Screen to start with."""
-        self.gui.start(start_screen)
-
-    def show_start_screen(self):
-        """Show start screen."""
-        self.gui.switch_screen(self.start_screen)
-
-    def show_screen(self, screen: Screen):
-        """Show start screen.
-        Args:
-            screen (type[Screen]): Screen to show."""
-        self.gui.switch_screen(screen)
-
-    def start_flow(self, flow: Flow):
-        """Start flow.
-        Args:
-            flow (type[Flow]): Flow to start."""
-        self.gui.start_flow(flow)
-
-    def file_dialog(
-        self, title: str, max_files: int, filetypes: list[tuple[str, str]]
-    ) -> tuple[str, ...]:
-        """Open file dialog.
-        Args:
-            title (str): Title of the dialog.
-            max_files (int): Maximum number of files to select.
-            filetypes (list[tuple[str, str]]): Filetypes to show.
-        Returns:
-            str | None: Path to file or None if no file selected."""
-        filenames = self.gui.file_dialog(title, max_files, filetypes)
-
-        if not filenames:
-            return ("",)
-
-        if isinstance(filenames, str):
-            return (filenames,)
-
-        return filenames
-
-    def quit(self):
-        self.gui.quit()
+from .gui import GUI, TKGUI
+from .gui.screens.screen import Screen
+from .util.settings import Settings
+from .util.user import User
+from .flows.flow import Flow
+
+
+class App:
+    """Singleton for accessing GUI, settings, user and other app-wide objects.
+
+    Attributes:
+        gui (GUI): GUI interface.
+        settings (Settings): Settings.
+        user (User): User.
+
+    Args:
+        title (str, optional): Title of the app. Defaults to "Appy".
+    """
+
+    title: str = "FlowMatic"
+    gui: GUI = None  # type: ignore
+    settings: Settings
+    user: User
+
+    start_screen: Screen
+
+    def __init__(self, start_screen: type[Screen]):
+        self.gui = self.gui or TKGUI(
+            title=self.title, start_screen=start_screen, geometry="1280x720"
+        )
+        self.start_screen = start_screen()
+        self.settings = Settings.load("files/settings.json")
+        self.user = User("")
+
+    def start(self, start_screen: Screen | None = None):
+        """Start app.
+        Args:
+            screen (type[Screen]): Screen to start with."""
+        self.gui.start(start_screen)
+
+    def show_start_screen(self):
+        """Show start screen."""
+        self.gui.switch_screen(self.start_screen)
+
+    def show_screen(self, screen: Screen):
+        """Show start screen.
+        Args:
+            screen (type[Screen]): Screen to show."""
+        self.gui.switch_screen(screen)
+
+    def start_flow(self, flow: Flow):
+        """Start flow.
+        Args:
+            flow (type[Flow]): Flow to start."""
+        self.gui.start_flow(flow)
+
+    def file_dialog(
+        self, title: str, max_files: int, filetypes: list[tuple[str, str]]
+    ) -> tuple[str, ...]:
+        """Open file dialog.
+        Args:
+            title (str): Title of the dialog.
+            max_files (int): Maximum number of files to select.
+            filetypes (list[tuple[str, str]]): Filetypes to show.
+        Returns:
+            str | None: Path to file or None if no file selected."""
+        filenames = self.gui.file_dialog(title, max_files, filetypes)
+
+        if not filenames:
+            return ("",)
+
+        if isinstance(filenames, str):
+            return (filenames,)
+
+        return filenames
+
+    def quit(self):
+        self.gui.quit()
```

### Comparing `flowmatic-0.1.5/flowmatic/flows/flow.py` & `flowmatic-0.1.6/flowmatic/flows/flow.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING, Protocol
-
-import flowmatic
-
-if TYPE_CHECKING:
-    from flowmatic.gui.screens.screen import FlowScreen, Screen
-
-
-class Flow(Protocol):
-    steps: list[type[FlowScreen]]
-    screens: list[FlowScreen]
-    return_to: Screen
-    step: int
-
-    def __init__(self) -> None:
-        self.screens = [screen(self) for screen in self.steps]
-        self.step = 0
-
-    def __next__(self) -> None:
-        if self.step == len(self.screens) or self.step < 0:
-            flowmatic.show_screen(self.return_to)
-            return
-        screen = self.screens[self.step]
-        self.step += 1
-        flowmatic.show_screen(screen)
-
-    def start(self):
-        next(self)
-
-    def quit(self):
-        self.step = len(self.screens)
-        next(self)
-
-    def next(self):
-        next(self)
-
-    def previous(self):
-        self.step -= 2
-        next(self)
+from __future__ import annotations
+from typing import TYPE_CHECKING, Protocol
+
+import flowmatic
+
+if TYPE_CHECKING:
+    from flowmatic.gui.screens.screen import FlowScreen, Screen
+
+
+class Flow(Protocol):
+    steps: list[type[FlowScreen]]
+    screens: list[FlowScreen]
+    return_to: Screen
+    step: int
+
+    def __init__(self) -> None:
+        self.screens = [screen(self) for screen in self.steps]
+        self.step = 0
+
+    def __next__(self) -> None:
+        if self.step == len(self.screens) or self.step < 0:
+            flowmatic.show_screen(self.return_to)
+            return
+        screen = self.screens[self.step]
+        self.step += 1
+        flowmatic.show_screen(screen)
+
+    def start(self):
+        next(self)
+
+    def quit(self):
+        self.step = len(self.screens)
+        next(self)
+
+    def next(self):
+        next(self)
+
+    def previous(self):
+        self.step -= 2
+        next(self)
```

### Comparing `flowmatic-0.1.5/flowmatic/forms/fields/check_box.py` & `flowmatic-0.1.6/flowmatic/forms/fields/check_box.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import tkinter as tk
-from typing import Any, Self
-
-import customtkinter as ctk
-
-from flowmatic import gui
-
-
-class CheckBox:
-    master: tk.Frame
-    frame: tk.Frame
-    label: str
-    __value: tk.BooleanVar
-    show: bool
-
-    @property
-    def value(self) -> bool:
-        return self.__value.get()
-
-    @value.setter
-    def value(self, value: bool) -> None:
-        self.__value.set(value)
-
-    def __init__(
-        self,
-        label: str,
-        *,
-        value: bool | None = None,
-    ) -> None:
-        self.label = label
-        self.__value = tk.BooleanVar(value=value)
-
-    def __call__(self, master: tk.Frame) -> Self:
-        self.master = master
-        self.frame = ctk.CTkFrame(
-            self.master,
-            fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
-        )
-        return self
-
-    def build(self, **kwargs: dict[str, Any]) -> Self:
-        self.frame.pack(**gui.pack_defaults)
-        ctk.CTkLabel(master=self.frame, text=self.label).pack(side=tk.LEFT, **kwargs)
-        ctk.CTkCheckBox(self.frame, variable=self.__value).pack(side="left", **kwargs)
-        return self
-
-    def pack(self, element: tk.Widget, **kwargs) -> None:
-        element.pack(**kwargs)
+import tkinter as tk
+from typing import Any, Self
+
+import customtkinter as ctk
+
+from flowmatic import gui
+
+
+class CheckBox:
+    master: tk.Frame
+    frame: tk.Frame
+    label: str
+    __value: tk.BooleanVar
+    show: bool
+
+    @property
+    def value(self) -> bool:
+        return self.__value.get()
+
+    @value.setter
+    def value(self, value: bool) -> None:
+        self.__value.set(value)
+
+    def __init__(
+        self,
+        label: str,
+        *,
+        value: bool | None = None,
+    ) -> None:
+        self.label = label
+        self.__value = tk.BooleanVar(value=value)
+
+    def __call__(self, master: tk.Frame) -> Self:
+        self.master = master
+        self.frame = ctk.CTkFrame(
+            self.master,
+            fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
+        )
+        return self
+
+    def build(self, **kwargs: dict[str, Any]) -> Self:
+        self.frame.pack(**gui.pack_defaults)
+        ctk.CTkLabel(master=self.frame, text=self.label).pack(side=tk.LEFT, **kwargs)
+        ctk.CTkCheckBox(self.frame, variable=self.__value).pack(side="left", **kwargs)
+        return self
+
+    def pack(self, element: tk.Widget, **kwargs) -> None:
+        element.pack(**kwargs)
```

### Comparing `flowmatic-0.1.5/flowmatic/forms/fields/date_select.py` & `flowmatic-0.1.6/flowmatic/forms/fields/text_field.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-import datetime
-import tkinter as tk
-from typing import Self
-import tkcalendar as tkc
-import customtkinter as ctk
-from flowmatic import gui
-
-
-class DateSelect:
-    master: tk.Frame
-    frame: tk.Frame
-    label: str
-    __value: tk.StringVar
-
-    @property
-    def value(self) -> str:
-        return self.__value.get()
-
-    @value.setter
-    def value(self, value: str) -> None:
-        self.__value.set(value)
-
-    def __init__(
-        self,
-        label: str,
-        *,
-        value: str | None = None,
-    ) -> None:
-        self.__value = tk.StringVar(
-            value=value or datetime.date.today().strftime("%d.%m.%Y")
-        )
-        self.label = label
-
-    def __call__(self, master: tk.Frame) -> Self:
-        self.master = master
-        self.frame = ctk.CTkFrame(
-            self.master,
-            fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
-        )
-        return self
-
-    def build(self, **kwargs) -> Self:
-        self.frame.pack()
-        ctk.CTkLabel(master=self.frame, text=self.label).pack(
-            side=tk.LEFT, **gui.pack_defaults
-        )
-        calendar = tkc.Calendar(
-            self.frame,
-            selectmode="day",
-            date_pattern="dd.mm.yyyy",
-            showweeknumbers=True,
-            textvariable=self.__value,
-        )
-        calendar.pack(side=tk.RIGHT, **gui.pack_defaults)
-        return self
-
-    def pack(self, element: tk.Widget, **kwargs) -> None:
-        element.pack(**kwargs)
+import tkinter as tk
+from typing import Any, Self
+
+import customtkinter as ctk
+
+
+class TextField:
+    master: tk.Frame
+    frame: tk.Frame
+    label: str
+    __value: tk.StringVar
+    placeholder_text: str | None
+    show: bool
+
+    @property
+    def value(self) -> str:
+        return self.__value.get()
+
+    @value.setter
+    def value(self, value: str) -> None:
+        self.__value.set(value)
+
+    def __init__(
+        self,
+        label: str,
+        *,
+        value: str | None = None,
+        placeholder_text: str | None = None,
+        show: bool = True
+    ) -> None:
+        self.label = label
+        self.__value = tk.StringVar(value=value)
+        self.placeholder_text = placeholder_text
+        self.show = show
+
+    def __call__(self, master: tk.Frame) -> Self:
+        self.master = master
+        self.frame = ctk.CTkFrame(
+            self.master,
+            fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
+        )
+        return self
+
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, TextField):
+            return False
+        return self.value == __value.value and self.label == __value.label
+
+    def build(self, **kwargs: dict[str, Any]) -> Self:
+        self.frame.pack()
+        ctk.CTkLabel(master=self.frame, text=self.label).pack(side=tk.LEFT, **kwargs)
+        entry = ctk.CTkEntry(
+            self.frame,
+            textvariable=self.__value,
+            placeholder_text=self.placeholder_text,
+            show="•" if not self.show else None,
+        )
+        entry.pack(side=tk.RIGHT, **kwargs)
+        return self
+
+    def pack(self, element: tk.Widget, **kwargs) -> None:
+        element.pack(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flowmatic-0.1.5/flowmatic/forms/fields/display.py` & `flowmatic-0.1.6/flowmatic/forms/fields/display.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import tkinter as tk
-from typing import Any, Self
-import customtkinter as ctk
-from flowmatic import gui
-from flowmatic.gui.elements.element_infos import Element
-
-
-class Display:
-    master: tk.Frame
-    frame: tk.Frame
-    label: str
-    __value: None = None
-    elements: list[Element]
-
-    @property
-    def value(self) -> None:
-        return self.__value
-
-    @value.setter
-    def value(self, value) -> None:
-        pass
-
-    def __init__(self, label: str, elements: list[Element] | None = None) -> None:
-        self.label = label
-        self.elements = elements or []
-
-    def __call__(
-        self,
-        master: tk.Frame,
-    ) -> Self:
-        self.master = master
-        self.frame = ctk.CTkFrame(
-            self.master,
-            # fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
-        )
-        return self
-
-    def build(self, **kwargs: dict[str, Any]) -> Self:
-        self.frame.pack()
-        ctk.CTkLabel(self.frame, text=self.label).pack(**gui.pack_defaults)
-        for element in self.elements:
-            gui.screens.ElementScreen.build_element(element, self.frame)
-        return self
-
-    def pack(self, element: tk.Widget, **kwargs) -> None:
-        element.pack(**kwargs)
+import tkinter as tk
+from typing import Any, Self
+import customtkinter as ctk
+from flowmatic import gui
+from flowmatic.gui.elements.element_infos import Element
+
+
+class Display:
+    master: tk.Frame
+    frame: tk.Frame
+    label: str
+    __value: None = None
+    elements: list[Element]
+
+    @property
+    def value(self) -> None:
+        return self.__value
+
+    @value.setter
+    def value(self, value) -> None:
+        pass
+
+    def __init__(self, label: str, elements: list[Element] | None = None) -> None:
+        self.label = label
+        self.elements = elements or []
+
+    def __call__(
+        self,
+        master: tk.Frame,
+    ) -> Self:
+        self.master = master
+        self.frame = ctk.CTkFrame(
+            self.master,
+            # fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
+        )
+        return self
+
+    def build(self, **kwargs: dict[str, Any]) -> Self:
+        self.frame.pack()
+        ctk.CTkLabel(self.frame, text=self.label).pack(**gui.pack_defaults)
+        for element in self.elements:
+            gui.screens.ElementScreen.build_element(element, self.frame)
+        return self
+
+    def pack(self, element: tk.Widget, **kwargs) -> None:
+        element.pack(**kwargs)
```

### Comparing `flowmatic-0.1.5/flowmatic/forms/validation.py` & `flowmatic-0.1.6/flowmatic/forms/validation.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Callable, Any
-
-
-class FormValidation:
-    field_label: str
-    condition: Callable[[Any], bool]
-    message: str
-
-    def __init__(
-        self, field_label: str, condition: Callable[[Any], bool], message: str
-    ) -> None:
-        self.field_label = field_label
-        self.condition = condition
-        self.message = message
-
-    def validate(self, values: dict[str, int | str | list[str]] | None) -> None:
-        assert values, "Form is empty."
-        value = values.get(self.field_label, None)
-        assert value is not None, f"{self.field_label} is empty."
-        assert self.condition(value), f"{self.field_label}: {self.message}"
+from typing import Callable, Any
+
+
+class FormValidation:
+    field_label: str
+    condition: Callable[[Any], bool]
+    message: str
+
+    def __init__(
+        self, field_label: str, condition: Callable[[Any], bool], message: str
+    ) -> None:
+        self.field_label = field_label
+        self.condition = condition
+        self.message = message
+
+    def validate(self, values: dict[str, int | str | list[str]] | None) -> None:
+        assert values, "Form is empty."
+        value = values.get(self.field_label, None)
+        assert value is not None, f"{self.field_label} is empty."
+        assert self.condition(value), f"{self.field_label}: {self.message}"
```

### Comparing `flowmatic-0.1.5/flowmatic/gui/screens/element_screen.py` & `flowmatic-0.1.6/flowmatic/gui/screens/element_screen.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import customtkinter as ctk
-import tkinter as tk
-from flowmatic import gui
-from flowmatic.gui.elements.element_infos import *  # pylint: disable=wildcard-import, unused-wildcard-import
-from flowmatic.gui.screens.screen import Screen
-
-
-class ElementScreen(Screen):
-    def build(  # pylint: disable=arguments-differ
-        self, elements: list[Element], **kwargs
-    ) -> None:
-        for element in elements:
-            self.build_element(element, self.master, **kwargs)
-
-    @classmethod
-    def build_element(
-        cls, element: Element, master: tk.Frame | tk.Tk, **kwargs
-    ) -> None:
-        match element:
-            case Button():
-                ctk.CTkButton(master, text=element.text, command=element.command).pack(
-                    **(gui.pack_defaults | kwargs),
-                )
-            case Info():
-                ctk.CTkLabel(
-                    master,
-                    text=f"{element.label}: {element.value}",
-                ).pack(**(gui.pack_defaults | kwargs))
-            case ElementFrame():
-                frame = ctk.CTkFrame(master)
-                frame.pack(**gui.pack_defaults)
-                ctk.CTkLabel(frame, text=element.title).pack(
-                    **(gui.pack_defaults | kwargs),
-                )
-                for row in element.rows:
-                    cls.build_element(row, frame, **kwargs)
-            case _:
-                raise NotImplementedError(
-                    f"Unknown element type: {element.__class__.__name__}, extend ElementScreen.build_element() to support it."
-                )
+import customtkinter as ctk
+import tkinter as tk
+from flowmatic import gui
+from flowmatic.gui.elements.element_infos import *  # pylint: disable=wildcard-import, unused-wildcard-import
+from flowmatic.gui.screens.screen import Screen
+
+
+class ElementScreen(Screen):
+    def build(  # pylint: disable=arguments-differ
+        self, elements: list[Element], **kwargs
+    ) -> None:
+        for element in elements:
+            self.build_element(element, self.master, **kwargs)
+
+    @classmethod
+    def build_element(
+        cls, element: Element, master: tk.Frame | tk.Tk, **kwargs
+    ) -> None:
+        match element:
+            case Button():
+                ctk.CTkButton(master, text=element.text, command=element.command).pack(
+                    **(gui.pack_defaults | kwargs),
+                )
+            case Info():
+                ctk.CTkLabel(
+                    master,
+                    text=f"{element.label}: {element.value}",
+                ).pack(**(gui.pack_defaults | kwargs))
+            case ElementFrame():
+                frame = ctk.CTkFrame(master)
+                frame.pack(**gui.pack_defaults)
+                ctk.CTkLabel(frame, text=element.title).pack(
+                    **(gui.pack_defaults | kwargs),
+                )
+                for row in element.rows:
+                    cls.build_element(row, frame, **kwargs)
+            case _:
+                raise NotImplementedError(
+                    f"Unknown element type: {element.__class__.__name__}, extend ElementScreen.build_element() to support it."
+                )
```

### Comparing `flowmatic-0.1.5/flowmatic/gui/screens/form_screen.py` & `flowmatic-0.1.6/flowmatic/gui/screens/form_screen.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-import tkinter as tk
-from typing import Callable, TypeVar, overload
-
-import customtkinter as ctk
-
-import flowmatic
-from flowmatic import gui
-from flowmatic.flows.flow import Flow
-from flowmatic.gui.screens.screen import FlowScreen, Screen
-from ...forms import FormValidation
-from ...forms.fields.field import Field
-from ..elements.element_infos import Button
-
-T = TypeVar("T")
-
-
-class FormScreen(Screen):
-    field_list: list[Field] | None
-    fields: dict[str, Field]
-    validations: list[FormValidation] | None = None
-    __message: tk.StringVar
-
-    @property
-    def message(self) -> str:
-        return self.__message.get()
-
-    @message.setter
-    def message(self, value: str) -> None:
-        """Set message.
-
-        Args:
-            value (str): Message."""
-        self.__message.set(value)
-
-    def __init__(
-        self,
-    ) -> None:
-        self.fields = {}
-        self.__message = tk.StringVar(value="")
-
-    @property
-    def values(self) -> dict[str, str | int | list[str]]:
-        """Get values from fields.
-
-        Returns:
-            dict[str, str]: Values from fields."""
-        return {
-            label: field.value for label, field in self.fields.items() if field.value
-        }
-
-    def validate(self) -> None:
-        if not self.validations:
-            return
-
-        for validation in self.validations:
-            validation.validate(self.values)
-
-    @overload
-    def get(self, __key: str, /) -> str | int | list[str]:
-        ...
-
-    @overload
-    def get(self, __key: str, __default: T) -> str | int | list[str] | T:
-        ...
-
-    @overload
-    def get(self, __key: str, __default: T, __return: type[T]) -> T:
-        ...
-
-    def get(
-        self, __key: str, __default: str | T = "", __return: type[T] | None = None
-    ) -> str | int | list[str] | T:
-        """Get value from field.
-
-        Args:
-            label (str): Label of field.
-
-        Returns:
-            str: Value of field."""
-        value = self.values.get(__key, __default)
-        if __return is not None:
-            if not isinstance(value, __return):
-                raise TypeError(f"Expected {__return} got {type(value)}")
-        return value
-
-    def submit_default(self) -> None:
-        flowmatic.show_start_screen
-
-    def build(  # pylint: disable=arguments-differ
-        self,
-        *,
-        title: str,
-        validations: list[FormValidation] | None = None,
-        submit_button: Button | None = None,
-        back_button: Button | None = None,
-        fields: list[Field] | None = None,
-        field_factory: Callable[..., list[Field]] | None = None,
-    ) -> None:
-        """Build screen.
-
-        Args:
-
-            title (str): Title of screen.
-            validate_command (Callable[[], None]): Command to run when validate button is pressed.
-            validate_text (str, optional): Text of validate button. Defaults to "Submit".
-            back_command (Callable[[], None], optional): Command to run when back button is pressed.
-                 Defaults to None.
-        """
-        # Variables
-        self.field_list = (fields or []) + (field_factory() if field_factory else [])
-        self.validations = validations
-        if not submit_button:
-            submit_button = Button(text="Submit", command=self.submit_default)
-
-        def validate_command() -> None:
-            try:
-                self.validate()
-            except AssertionError as error:
-                self.message = str(error)
-                flowmatic.update_gui()
-            else:
-                submit_button.command()
-
-        # Title
-        ctk.CTkLabel(self.master, text=title).pack(**gui.pack_defaults)
-
-        # Fields
-        if self.field_list:
-            fields_frame = (
-                ctk.CTkScrollableFrame(
-                    self.master, height=gui.HEIGHT - 150, width=gui.WIDTH
-                )
-                if not isinstance(self.master, ctk.CTkScrollableFrame)
-                else ctk.CTkFrame(self.master)
-            )
-            fields_frame.pack(**gui.pack_defaults)
-            for field in self.field_list:
-                self.fields[field.label] = field(fields_frame).build(
-                    **gui.pack_defaults
-                )
-
-        # Message
-        ctk.CTkLabel(self.master, textvariable=self.__message).pack(**gui.pack_defaults)
-
-        # Buttons
-        pack_args = gui.pack_defaults  # | {"pady": (10, 20)}
-        button_frame = ctk.CTkFrame(self.master)
-        button_frame.pack(**pack_args)
-        ctk.CTkButton(
-            button_frame, text=submit_button.text or "Submit", command=validate_command
-        ).pack(**gui.pack_defaults, side=tk.RIGHT)
-        if back_button:
-            ctk.CTkButton(
-                button_frame,
-                text=back_button.text or "Back",
-                command=back_button.command,
-            ).pack(**gui.pack_defaults, side=tk.LEFT)
-
-
-class FlowFormScreen(FormScreen, FlowScreen):
-    def __init__(self, flow: Flow) -> None:
-        self.flow = flow
-        super().__init__()
+import tkinter as tk
+from typing import Callable, TypeVar, overload
+
+import customtkinter as ctk
+
+import flowmatic
+from flowmatic import gui
+from flowmatic.flows.flow import Flow
+from flowmatic.gui.screens.screen import FlowScreen, Screen
+from ...forms import FormValidation
+from ...forms.fields.field import Field
+from ..elements.element_infos import Button
+
+T = TypeVar("T")
+
+
+class FormScreen(Screen):
+    field_list: list[Field] | None
+    fields: dict[str, Field]
+    validations: list[FormValidation] | None = None
+    __message: tk.StringVar
+
+    @property
+    def message(self) -> str:
+        return self.__message.get()
+
+    @message.setter
+    def message(self, value: str) -> None:
+        """Set message.
+
+        Args:
+            value (str): Message."""
+        self.__message.set(value)
+
+    def __init__(
+        self,
+    ) -> None:
+        self.fields = {}
+        self.__message = tk.StringVar(value="")
+
+    @property
+    def values(self) -> dict[str, str | int | list[str]]:
+        """Get values from fields.
+
+        Returns:
+            dict[str, str]: Values from fields."""
+        return {
+            label: field.value for label, field in self.fields.items() if field.value
+        }
+
+    def validate(self) -> None:
+        if not self.validations:
+            return
+
+        for validation in self.validations:
+            validation.validate(self.values)
+
+    @overload
+    def get(self, __key: str, /) -> str | int | list[str]:
+        ...
+
+    @overload
+    def get(self, __key: str, __default: T) -> str | int | list[str] | T:
+        ...
+
+    @overload
+    def get(self, __key: str, __default: T, __return: type[T]) -> T:
+        ...
+
+    def get(
+        self, __key: str, __default: str | T = "", __return: type[T] | None = None
+    ) -> str | int | list[str] | T:
+        """Get value from field.
+
+        Args:
+            label (str): Label of field.
+
+        Returns:
+            str: Value of field."""
+        value = self.values.get(__key, __default)
+        if __return is not None:
+            if not isinstance(value, __return):
+                raise TypeError(f"Expected {__return} got {type(value)}")
+        return value
+
+    def submit_default(self) -> None:
+        flowmatic.show_start_screen
+
+    def build(  # pylint: disable=arguments-differ
+        self,
+        *,
+        title: str,
+        validations: list[FormValidation] | None = None,
+        submit_button: Button | None = None,
+        back_button: Button | None = None,
+        fields: list[Field] | None = None,
+        field_factory: Callable[..., list[Field]] | None = None,
+    ) -> None:
+        """Build screen.
+
+        Args:
+
+            title (str): Title of screen.
+            validate_command (Callable[[], None]): Command to run when validate button is pressed.
+            validate_text (str, optional): Text of validate button. Defaults to "Submit".
+            back_command (Callable[[], None], optional): Command to run when back button is pressed.
+                 Defaults to None.
+        """
+        # Variables
+        self.field_list = (fields or []) + (field_factory() if field_factory else [])
+        self.validations = validations
+        if not submit_button:
+            submit_button = Button(text="Submit", command=self.submit_default)
+
+        def validate_command() -> None:
+            try:
+                self.validate()
+            except AssertionError as error:
+                self.message = str(error)
+                flowmatic.update_gui()
+            else:
+                submit_button.command()
+
+        # Title
+        ctk.CTkLabel(self.master, text=title).pack(**gui.pack_defaults)
+
+        # Fields
+        if self.field_list:
+            fields_frame = (
+                ctk.CTkScrollableFrame(
+                    self.master, height=gui.HEIGHT - 150, width=gui.WIDTH
+                )
+                if not isinstance(self.master, ctk.CTkScrollableFrame)
+                else ctk.CTkFrame(self.master)
+            )
+            fields_frame.pack(**gui.pack_defaults)
+            for field in self.field_list:
+                self.fields[field.label] = field(fields_frame).build(
+                    **gui.pack_defaults
+                )
+
+        # Message
+        ctk.CTkLabel(self.master, textvariable=self.__message).pack(**gui.pack_defaults)
+
+        # Buttons
+        pack_args = gui.pack_defaults  # | {"pady": (10, 20)}
+        button_frame = ctk.CTkFrame(self.master)
+        button_frame.pack(**pack_args)
+        ctk.CTkButton(
+            button_frame, text=submit_button.text or "Submit", command=validate_command
+        ).pack(**gui.pack_defaults, side=tk.RIGHT)
+        if back_button:
+            ctk.CTkButton(
+                button_frame,
+                text=back_button.text or "Back",
+                command=back_button.command,
+            ).pack(**gui.pack_defaults, side=tk.LEFT)
+
+
+class FlowFormScreen(FormScreen, FlowScreen):
+    def __init__(self, flow: Flow) -> None:
+        self.flow = flow
+        super().__init__()
```

### Comparing `flowmatic-0.1.5/flowmatic/gui/screens/menu_screen.py` & `flowmatic-0.1.6/flowmatic/gui/screens/title_screen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import customtkinter as ctk
-
-from flowmatic import gui
-from flowmatic.gui.screens.screen import Screen
-from ...gui.elements import Button
-
-
-class MenuScreen(Screen):
-    """Menu screen. Used for menus.
-
-    Args:
-        master (tk.Tk): Master window."""
-
-    def build(  # pylint: disable=arguments-differ
-        self, title: str, buttons: list[Button]
-    ) -> None:
-        """Build screen.
-
-        Args:
-            title (str): Title of screen.
-            buttons (list[gui.ButtonInfo]): List of buttons to add to screen."""
-        ctk.CTkLabel(self.master, text=title).pack(**gui.pack_defaults)
-        for button in buttons:
-            ctk.CTkButton(self.master, text=button.text, command=button.command).pack(
-                **gui.pack_defaults
-            )
+import customtkinter as ctk
+
+from flowmatic import gui
+from flowmatic.gui.screens.screen import Screen
+from ...gui.elements import Button
+
+
+class TitleScreen(Screen):
+    """Title screen.
+
+    Args:
+        master (tk.Tk): Master of screen."""
+
+    def build(  # pylint: disable=arguments-differ
+        self, title: str, button: Button
+    ) -> None:
+        """Build screen.
+
+        Args:
+            title (str): Title of screen.
+            button (gui.ButtonInfo): Button to show.
+        """
+        ctk.CTkLabel(self.master, text=title).pack(**gui.pack_defaults)
+        ctk.CTkButton(self.master, text=button[0], command=button[1]).pack(
+            **gui.pack_defaults,
+        )
```

### Comparing `flowmatic-0.1.5/flowmatic/util/exceptions.py` & `flowmatic-0.1.6/flowmatic/util/exceptions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""Exceptions used by Appy.
-
-Classes:
-    SavedClassLoadException: Raised when a class cannot be loaded from a saved file."""
-
-
-class SavedClassLoadException(Exception):
-    path: str
-
-    def __init__(self, path: str) -> None:
-        self.path = path
-
-    def __str__(self) -> str:
-        return f"Could not load class from {self.path}"
-
-
-class TooManyFilesError(Exception):
-    max_files: int
-
-    def __init__(self, max_files: int) -> None:
-        self.max_files = max_files
-
-    def __str__(self) -> str:
-        return f"Too many files. Max: {self.max_files}"
-
-
-class NotAFileError(Exception):
-    path: str
-
-    def __init__(self, path: str) -> None:
-        self.path = path
-
-    def __str__(self) -> str:
-        return f"Not a file: {self.path}"
+"""Exceptions used by Appy.
+
+Classes:
+    SavedClassLoadException: Raised when a class cannot be loaded from a saved file."""
+
+
+class SavedClassLoadException(Exception):
+    path: str
+
+    def __init__(self, path: str) -> None:
+        self.path = path
+
+    def __str__(self) -> str:
+        return f"Could not load class from {self.path}"
+
+
+class TooManyFilesError(Exception):
+    max_files: int
+
+    def __init__(self, max_files: int) -> None:
+        self.max_files = max_files
+
+    def __str__(self) -> str:
+        return f"Too many files. Max: {self.max_files}"
+
+
+class NotAFileError(Exception):
+    path: str
+
+    def __init__(self, path: str) -> None:
+        self.path = path
+
+    def __str__(self) -> str:
+        return f"Not a file: {self.path}"
```

### Comparing `flowmatic-0.1.5/flowmatic/util/saved_class.py` & `flowmatic-0.1.6/flowmatic/util/saved_class.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from abc import ABC
-import json
-from typing import Any, Self
-
-from flowmatic.util import SavedClassLoadException
-
-
-class SavedClass(ABC):
-    def __init__(self, path: str):
-        self.path = path
-
-    def set(self, kwargs: dict[str, Any]) -> Self:
-        """Set attributes.
-
-        Args:
-            kwargs (dict[str, Any]): Attributes to set.
-
-        Returns:
-            Self: Self."""
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-        return self
-
-    def items(self):
-        _dict = self.__dict__.copy()
-        _dict.pop("path")
-        return _dict.items()
-
-    def save(self):
-        if self.path:
-            with open(self.path, "w", encoding="utf-8") as file:
-                json.dump(self.__dict__, fp=file)
-
-    def load_from_disk(self) -> None:
-        with open(self.path, "r", encoding="utf-8") as file:
-            try:
-                json_data = json.load(file)
-                for key, value in json_data.items():
-                    setattr(self, key, value)
-            except Exception as exc:
-                raise SavedClassLoadException(self.path) from exc
-
-    def create_file(self) -> None:
-        f = open(self.path, "w", encoding="utf-8")
-        f.close()
-
-    @classmethod
-    def load(cls, path: str) -> Self:
-        """Load the class from disk.
-
-        Args:
-            path (str): Path to load from.
-
-        Returns:
-            Self: The loaded class.
-
-        Raises:
-            SavedClassLoadException: If the class could not be loaded."""
-        self = cls(path)
-        try:
-            self.load_from_disk()
-        except FileNotFoundError:
-            self.create_file()
-
-        return self
+from abc import ABC
+import json
+from typing import Any, Self
+
+from flowmatic.util import SavedClassLoadException
+
+
+class SavedClass(ABC):
+    def __init__(self, path: str):
+        self.path = path
+
+    def set(self, kwargs: dict[str, Any]) -> Self:
+        """Set attributes.
+
+        Args:
+            kwargs (dict[str, Any]): Attributes to set.
+
+        Returns:
+            Self: Self."""
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+        return self
+
+    def items(self):
+        _dict = self.__dict__.copy()
+        _dict.pop("path")
+        return _dict.items()
+
+    def save(self):
+        if self.path:
+            with open(self.path, "w", encoding="utf-8") as file:
+                json.dump(self.__dict__, fp=file)
+
+    def load_from_disk(self) -> None:
+        with open(self.path, "r", encoding="utf-8") as file:
+            try:
+                json_data = json.load(file)
+                for key, value in json_data.items():
+                    setattr(self, key, value)
+            except Exception as exc:
+                raise SavedClassLoadException(self.path) from exc
+
+    def create_file(self) -> None:
+        f = open(self.path, "w", encoding="utf-8")
+        f.close()
+
+    @classmethod
+    def load(cls, path: str) -> Self:
+        """Load the class from disk.
+
+        Args:
+            path (str): Path to load from.
+
+        Returns:
+            Self: The loaded class.
+
+        Raises:
+            SavedClassLoadException: If the class could not be loaded."""
+        self = cls(path)
+        try:
+            self.load_from_disk()
+        except FileNotFoundError:
+            self.create_file()
+
+        return self
```

### Comparing `flowmatic-0.1.5/PKG-INFO` & `flowmatic-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flowmatic
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: aeteseb
 Author-email: 113799213+aeteseb@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ctkmessagebox (>=2.4,<3.0)
 Requires-Dist: customtkinter (>=5.2.0,<6.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: tkcalendar (>=1.6.1,<2.0.0)
 Requires-Dist: tkinterdnd2-universal (>=1.7.3,<2.0.0)
 Description-Content-Type: text/markdown
```

