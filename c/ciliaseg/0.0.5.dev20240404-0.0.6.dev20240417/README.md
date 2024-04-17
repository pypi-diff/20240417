# Comparing `tmp/ciliaseg-0.0.5.dev20240404.tar.gz` & `tmp/ciliaseg-0.0.6.dev20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciliaseg-0.0.5.dev20240404.tar", last modified: Thu Apr  4 19:14:30 2024, max compression
+gzip compressed data, was "ciliaseg-0.0.6.dev20240417.tar", last modified: Wed Apr 17 13:57:03 2024, max compression
```

## Comparing `ciliaseg-0.0.5.dev20240404.tar` & `ciliaseg-0.0.6.dev20240417.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.077943 ciliaseg-0.0.5.dev20240404/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-21 17:12:23.000000 ciliaseg-0.0.5.dev20240404/MANIFEST.in
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       64 2024-04-04 19:14:30.077763 ciliaseg-0.0.5.dev20240404/PKG-INFO
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.074915 ciliaseg-0.0.5.dev20240404/ciliaseg/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:26.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      961 2023-11-21 17:12:23.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/__main__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     9878 2024-04-04 19:13:28.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/app.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076053 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:19.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1205 2024-04-04 19:05:36.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/model.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1130 2023-11-13 18:32:23.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/polygon.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076398 ciliaseg-0.0.5.dev20240404/ciliaseg/gui/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:41.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/gui/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    18613 2024-04-04 18:37:17.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/gui/canvas.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076818 ciliaseg-0.0.5.dev20240404/ciliaseg/state/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:31.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/state/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     6120 2024-04-04 19:10:50.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/state/image.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    10063 2024-04-04 18:36:21.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/state/stereocilia.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076949 ciliaseg-0.0.5.dev20240404/ciliaseg/train/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:09.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/train/__init__.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.077148 ciliaseg-0.0.5.dev20240404/ciliaseg/utils/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:52.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/utils/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1091 2023-12-01 18:10:18.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/utils/io.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.077524 ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:33.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    12356 2024-04-04 16:05:51.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/control.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.075701 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       64 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/PKG-INFO
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      607 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/SOURCES.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/dependency_links.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       54 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/entry_points.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      118 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/requires.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        9 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/top_level.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       38 2024-04-04 19:14:30.077992 ciliaseg-0.0.5.dev20240404/setup.cfg
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      446 2024-04-04 19:13:47.000000 ciliaseg-0.0.5.dev20240404/setup.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.695087 ciliaseg-0.0.6.dev20240417/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-21 17:12:23.000000 ciliaseg-0.0.6.dev20240417/MANIFEST.in
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      302 2024-04-17 13:57:03.694671 ciliaseg-0.0.6.dev20240417/PKG-INFO
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.689414 ciliaseg-0.0.6.dev20240417/ciliaseg/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:26.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      961 2023-11-21 17:12:23.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/__main__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     9878 2024-04-04 19:13:28.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/app.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.691641 ciliaseg-0.0.6.dev20240417/ciliaseg/eval/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:19.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/eval/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1205 2024-04-04 19:05:36.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/eval/model.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1130 2023-11-13 18:32:23.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/eval/polygon.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.692062 ciliaseg-0.0.6.dev20240417/ciliaseg/gui/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:41.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/gui/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    19176 2024-04-17 13:48:39.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/gui/canvas.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.693038 ciliaseg-0.0.6.dev20240417/ciliaseg/state/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:31.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/state/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     6434 2024-04-17 13:39:46.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/state/image.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    10147 2024-04-17 13:49:51.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/state/stereocilia.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.693341 ciliaseg-0.0.6.dev20240417/ciliaseg/train/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:09.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/train/__init__.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.693576 ciliaseg-0.0.6.dev20240417/ciliaseg/utils/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:52.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/utils/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1091 2023-12-01 18:10:18.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/utils/io.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.694149 ciliaseg-0.0.6.dev20240417/ciliaseg/widgets/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:33.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/widgets/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    12356 2024-04-04 16:05:51.000000 ciliaseg-0.0.6.dev20240417/ciliaseg/widgets/control.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-17 13:57:03.690813 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      302 2024-04-17 13:57:03.000000 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/PKG-INFO
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      607 2024-04-17 13:57:03.000000 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-17 13:57:03.000000 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       54 2024-04-17 13:57:03.000000 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/entry_points.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      118 2024-04-17 13:57:03.000000 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/requires.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        9 2024-04-17 13:57:03.000000 ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/top_level.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       38 2024-04-17 13:57:03.695132 ciliaseg-0.0.6.dev20240417/setup.cfg
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      446 2024-04-17 13:22:34.000000 ciliaseg-0.0.6.dev20240417/setup.py
```

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/__main__.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/__main__.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/app.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/app.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/eval/model.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/eval/model.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/eval/polygon.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/eval/polygon.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/gui/canvas.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/gui/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         # Interactivity modes --------------
         self.move_mode = True
         self.draw_stereocilia_mode = False
         self.edit_stereocilia_mode = False
 
         # Annotation -----------
-        self._default_stereocilia_label = 'short'  # short middle tall
+        self._default_stereocilia_label = "short"  # short middle tall
         self.polygon_buffer = []
 
         # polygon for stereocila region drawing
         self._draw_mouse_position = None
         self._mouse_position = None
         self._editable_vertex = None
         self._potential_new_vert = None
@@ -66,32 +66,31 @@
         self.scale = 1.0
         self._temp_ratio = (0.0, 0.0)
 
         # where is the mouse?
         self.mouse_position = QPointF()
         self.setMouseTracking(True)
 
-
     def abortAction(self):
         """ gracefully handles when the esc key is pressed """
         self._draw_mouse_position = None
         self._mouse_position = None
         self._editable_vertex = None
         self.polygon_buffer = []
         self.update()
 
-
     def setDefaultClassLabel(self, label):
         self._default_stereocilia_label = label
 
         if self.active_image is not None:
             for stereocilia in self.active_image.get_selected():
                 stereocilia.set_label(label)
 
         self.update()
+
     def disableAllInteractivityModes(self):
         self.move_mode = False
         self.edit_stereocilia_mode = False
         self.draw_stereocilia_mode = False
 
     def enableMoveMode(self):
         self.disableAllInteractivityModes()
@@ -160,21 +159,18 @@
         DOES NOT place the image in the center of the screen. For that, go to self.resetImageToViewport()
         """
         if self.pixmap is not None:
             # get height of the current view and of the pixmap (image)
             w0, h0 = self.pixmap.width(), self.pixmap.height()
             w1, h1 = self.width(), self.height()
 
-            print(w0, w1, h0, h1, end=' ')
-
             if w0 > w1 or h0 > h1:  # zooms out if the image is much smaller
                 _scale = max(w1 / w0, h1 / h0)
             else:  # zooms in otherwise
                 _scale = min(w1 / w0, h1 / h0)
-            print(f'{_scale=}, {w1/w0=}, {h1/h0=}')
         else:
             _scale = 1
 
         self.zoomReset()  # have to reset the zoom first.
         self.zoomBy(_scale)
 
     def _get_viewport_size(self):
@@ -224,25 +220,26 @@
         self.mouse_position_signal.emit([_x, _y])
 
         if not self.active_image:
             return
 
         # Drag the screen around!
         if (
-                event.buttons() == Qt.MiddleButton or event.buttons() == Qt.RightButton
+            event.buttons() == Qt.MiddleButton or event.buttons() == Qt.RightButton
         ) and not self._dragging[0]:
             self._dragging[1] = True
             self._last_drag_pos = event.position()
 
         # This is such that if someone tries to click while already dragging, it just fails..
         if event.buttons() == Qt.LeftButton | Qt.RightButton and self._dragging[1]:
             self._last_drag_pos = QPointF()
             self._dragging[1] = False
         elif (
-                event.buttons() == Qt.MiddleButton | Qt.LeftButton or event.buttons() == Qt.LeftButton | Qt.RightButton
+            event.buttons() == Qt.MiddleButton | Qt.LeftButton
+            or event.buttons() == Qt.LeftButton | Qt.RightButton
         ) and self._dragging[0]:
             self._last_drag_pos = QPointF()
             self._dragging[0] = False
 
         if event.buttons() != Qt.LeftButton:
             self.update()
             return
@@ -256,47 +253,48 @@
 
         if self.edit_stereocilia_mode:
             press = QPointF(_x, _y)
 
             if any(s.is_selected() for s in self.active_image.get_stereocilia()):
                 for s in self.active_image.get_stereocilia():
                     if s.is_selected():
-                        self._editable_vertex: QPointF = s.return_clicked_vertex(press, self.VERTEX_CLICK_TRH)
+                        self._editable_vertex: QPointF = s.return_clicked_vertex(
+                            press, self.VERTEX_CLICK_TRH
+                        )
 
                         if self._editable_vertex is None:
-                            self._potential_new_vert = s.closest_point_on_polygon(press, self.VERTEX_CLICK_TRH*2500)
+                            self._potential_new_vert = s.closest_point_on_polygon(
+                                press, self.VERTEX_CLICK_TRH * 2500
+                            )
                             s.insert_vertex(self._potential_new_vert)
                             self._editable_vertex = self._potential_new_vert
                             self._potential_new_vert = None
 
             if not self._editable_vertex:
-                self.selected_stereocilia.emit('')
+                self.selected_stereocilia.emit("")
                 for s in self.active_image.get_stereocilia():
                     s.deselect()
                 for s in self.active_image.get_stereocilia():
                     if s.is_inside(press):
                         s.select()
                         self.selected_stereocilia.emit(s.get_label_str())
 
-
         self.update()
 
-
-
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
         self.mouse_position = event.position()
         pos = event.position()
         _x = (pos.x() / self.scale) - self._pixmap_offset.x()
         _y = (pos.y() / self.scale) - self._pixmap_offset.y()
 
         # Moves the pixmap around...
         if (
-                (event.buttons() == Qt.LeftButton and self.move_mode)
-                or event.buttons() == Qt.MiddleButton
-                or event.buttons() == Qt.RightButton
+            (event.buttons() == Qt.LeftButton and self.move_mode)
+            or event.buttons() == Qt.MiddleButton
+            or event.buttons() == Qt.RightButton
         ) and any(self._dragging):
             pos = event.position()
             if self._last_drag_pos is not None:
                 self._pixmap_offset += (pos - self._last_drag_pos) / self.scale
                 self._last_drag_pos = pos
             self.zoomBy(1.0)
 
@@ -307,37 +305,40 @@
             self._editable_vertex.setX(_x)
             self._editable_vertex.setY(_y)
 
         if self.edit_stereocilia_mode and not self._editable_vertex:
             selected = self.active_image.get_selected()
             s = selected[0] if selected else None
             if s is not None:
-                self._potential_new_vert = self.active_image.get_selected()[0].closest_point_on_polygon(QPointF(_x, _y), self.VERTEX_CLICK_TRH * 2500)
+                self._potential_new_vert = self.active_image.get_selected()[
+                    0
+                ].closest_point_on_polygon(
+                    QPointF(_x, _y), self.VERTEX_CLICK_TRH * 2500
+                )
 
         self.update()
 
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         self.mouse_position = event.position()
         pos = event.position()
         _x = (pos.x() / self.scale) - self._pixmap_offset.x()
         _y = (pos.y() / self.scale) - self._pixmap_offset.y()
 
         if (
-                event.button() == Qt.MiddleButton or event.button() == Qt.RightButton
-        ) and self._dragging[
-            1
-        ]:  # can always move by pressing the middle button down
+            (event.button() == Qt.MiddleButton or event.button() == Qt.RightButton)
+            and self._dragging[1]
+        ):  # can always move by pressing the middle button down
             pos = event.position()
             if self._last_drag_pos is not None:
                 self._pixmap_offset += pos - self._last_drag_pos
             self._last_drag_pos = QPointF()
             self._dragging[1] = False
 
         if (
-                event.button() == Qt.LeftButton and self.move_mode and self._dragging[0]
+            event.button() == Qt.LeftButton and self.move_mode and self._dragging[0]
         ):  # if you're in move mode then you can click and drag.
             pos = event.position()
             if self._last_drag_pos:  # need to do this to avoid double click bug..
                 self._pixmap_offset += pos - self._last_drag_pos
             self._last_drag_pos = QPointF()
             self._dragging[0] = False
 
@@ -348,24 +349,41 @@
         self.mouse_position = event.position()
         pos = event.position()
         _x = (pos.x() / self.scale) - self._pixmap_offset.x()
         _y = (pos.y() / self.scale) - self._pixmap_offset.y()
 
         if self.draw_stereocilia_mode:
 
-            stereocilia = Stereocilia() \
-                .set_vertices(self.polygon_buffer) \
-                .set_label(self._default_stereocilia_label) \
-                .set_score(1.0) \
+            stereocilia = (
+                Stereocilia()
+                .set_vertices(self.polygon_buffer)
+                .set_label(self._default_stereocilia_label)
+                .set_score(1.0)
                 .set_gt()
+            )
 
             self.active_image.add_stereocilia(stereocilia)
             self.polygon_buffer = []
 
+        if self.edit_stereocilia_mode:
+            # we want to double click outside the region to
+            # end editing...
+
+            if all(
+                not s.is_inside(QPointF(_x, _y))
+                for s in self.active_image.get_selected()
+            ):
+                self.active_image.deselect_all()
+            else:
+                for s in self.active_image.get_stereocilia():
+                    print(s)
+
         self._editable_vertex = None
+        self._potential_new_vert = None
+
         self.update()
 
     def getCurrentWindowCoords(self) -> List[float]:
         x0 = -self._pixmap_offset.x()
         y0 = -self._pixmap_offset.y()
         x1 = self.width() / self.scale + x0
         y1 = self.height() / self.scale + y0
@@ -374,15 +392,14 @@
     def addStereocilia(self):
         raise NotImplemented
 
     def deleteSelected(self):
         if self.active_image is not None:
             self.active_image.delete_selected()
 
-
             self.update()
 
     def setActiveImage(self, image: SEMImage):
         self.active_image = image
         self.setImage(self.active_image.get_image_buffer_as_qimage())
 
         self.resetImageToViewport()
@@ -469,29 +486,29 @@
     def _paint_potential_vert(self):
         if not self._potential_new_vert:
             return
 
         p = self.painter
         pen = QPen()
         pen.setWidthF(6 / self.scale)
-        color = QColor('yellow')
+        color = QColor("yellow")
         pen.setColor(color)
 
         p.setPen(pen)
 
         p.drawPoint(self._potential_new_vert + self._pixmap_offset)
 
     def _paint_polygon_buffer(self):
         if not self.polygon_buffer:
             return
 
         p = self.painter
         pen = QPen()
         pen.setWidthF(2 / self.scale)
-        color = QColor('red')
+        color = QColor("red")
         pen.setColor(color)
 
         verts = [v + self._pixmap_offset for v in self.polygon_buffer]
         if self._draw_mouse_position:
             verts += [self._draw_mouse_position + self._pixmap_offset]
 
         p.setPen(pen)
@@ -512,30 +529,29 @@
             p.drawPoint(point)
 
     def _paint_stereocilia(self):
         if self.pixmap is not None and self.active_image is not None:
             p = self.painter
             pen = QPen()
             pen.setWidthF(2 / self.scale)
-            color = QColor('green')
+            color = QColor("green")
             pen.setColor(color)
             p.setPen(pen)
 
-
             if not self.edit_stereocilia_mode:
                 for s in self.active_image.get_stereocilia():
-                    s.paint(p, self._pixmap_offset, {'scale': self.scale})
+                    s.paint(p, self._pixmap_offset, {"scale": self.scale})
             else:
                 if any(s.is_selected() for s in self.active_image.get_stereocilia()):
                     for s in self.active_image.get_stereocilia():
                         if s.is_selected():
-                            s.paint(p, self._pixmap_offset, {'scale': self.scale})
+                            s.paint(p, self._pixmap_offset, {"scale": self.scale})
                 else:
                     for s in self.active_image.get_stereocilia():
-                        s.paint(p, self._pixmap_offset, {'scale': self.scale})
+                        s.paint(p, self._pixmap_offset, {"scale": self.scale})
 
     def _paint_pixmap(self):
         """paints the image to QLabel"""
         if self.pixmap is not None:
             p = self.painter
             p.drawPixmap(self._pixmap_offset, self.pixmap)
             p.setClipping(True)
```

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/state/image.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/state/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,96 +29,102 @@
     def __init__(self):
 
         self.filepath = None
         self.image = None
         self.sha256_hash_of_image = None
         self.dtype = None
         self.filename = None
-        self.device = 'cpu'
+        self.device = "cpu"
         self.model_out = None
 
         self.seleted: Stereocilia | None = None
 
         self.adjustments: List[Dict[str, int] | None] = [
-            {"brightness": 0, "contrast": 1, 'channel': 0},
-            {"brightness": 0, "contrast": 1, 'channel': 1},
-            {"brightness": 0, "contrast": 1, 'channel': 2},
+            {"brightness": 0, "contrast": 1, "channel": 0},
+            {"brightness": 0, "contrast": 1, "channel": 1},
+            {"brightness": 0, "contrast": 1, "channel": 2},
         ]
 
         self.stereocilia: List[Stereocilia] = []
         self._candidate_stereocilia = []
 
         self.nms_thr = 0.5
         self.stereocilia_thr = 0.5
 
         self._display_image_buffer = None
 
-    def eval_model(self, model: nn.Module, mean: float = .3717, std: float = .1897):
+    def eval_model(self, model: nn.Module, mean: float = 0.3717, std: float = 0.1897):
         image: Tensor = torch.from_numpy(self.image)  # [X, Y ,3]
         image = image.permute(2, 0, 1).div(255).sub(mean).div(std).float()
 
         with torch.no_grad():
             out = model([image])[0]
 
         self.model_out = out
         print(out)
-        self.model_out['polygons'] = [
-            ciliaseg.eval.polygon.find_contours(out['masks'][i, 0, ...].permute(1,0).numpy()) for i in range(out['scores'].shape[0])]
+        self.model_out["polygons"] = [
+            ciliaseg.eval.polygon.find_contours(
+                out["masks"][i, 0, ...].permute(1, 0).numpy()
+            )
+            for i in range(out["scores"].shape[0])
+        ]
         return self
 
     def update_polygons(self, polygon_threshold: float = 0.25):
         if self.model_out is None:
             return
 
-        self.model_out['polygons-downsampled'] = [
-            ciliaseg.eval.polygon.approximate_polygon(c, tolerance=polygon_threshold) for c in self.model_out['polygons']]
+        self.model_out["polygons-downsampled"] = [
+            ciliaseg.eval.polygon.approximate_polygon(c, tolerance=polygon_threshold)
+            for c in self.model_out["polygons"]
+        ]
 
         return self
 
     def populate_stereocilia_from_model_out(self):
         if not self.model_out:
             return
 
-
         to_delete = [s for s in self.get_stereocilia() if not s.is_ground_truth()]
         self.set_stereocilia([s for s in self.get_stereocilia() if s.is_ground_truth()])
         del to_delete
 
-        scores = self.model_out['scores']
-        masks = self.model_out['masks']  # [N, 1, X, Y]
-        labels = self.model_out['labels']
-        boxes = self.model_out['boxes']
-        polygons = self.model_out['polygons-downsampled']
+        scores = self.model_out["scores"]
+        masks = self.model_out["masks"]  # [N, 1, X, Y]
+        labels = self.model_out["labels"]
+        boxes = self.model_out["boxes"]
+        polygons = self.model_out["polygons-downsampled"]
 
         ind = torchvision.ops.nms(boxes, scores, self.nms_thr)
 
         for i in range(masks.shape[0]):
             if scores[i] < self.stereocilia_thr or i not in ind:
                 continue
 
             _mask = masks[i, 0, ...]  # x, y
             poly = polygons[i]
             poly: List[QPointF] = ciliaseg.eval.polygon.polygon_to_qt(poly)
 
-            s = Stereocilia() \
-                .set_score(scores[i]) \
-                .set_label(int(labels[i]) - 1) \
+            s = (
+                Stereocilia()
+                .set_score(scores[i])
+                .set_label(int(labels[i]) - 1)
                 .set_vertices(poly)
+            )
 
             self.add_stereocilia(s)
 
         return self
 
     def load_image(self, filepath):
         self.filepath = filepath
         _image = io.imread(filepath)
 
         if _image.ndim == 2:
-            _image = _image[:, :, np.newaxis][:,:,[0,0,0]]
-
+            _image = _image[:, :, np.newaxis][:, :, [0, 0, 0]]
 
         if _image.max() > 256:
 
             const = 2 ** 15 if _image.max() < 2 ** 15 else 2 ** 16
             if _image.max() < 2 ** 13:
                 const = 2 ** 13
 
@@ -127,15 +133,17 @@
             _image = np.round(_image).astype(np.uint8)
 
         if _image.shape[0] < 5:  # sometimes the channel is first i guess..
             _image = _image.transpose(1, 2, 0)
 
         while _image.shape[-1] < 3:
             x, y, _ = _image.shape
-            _image = np.concatenate((_image, np.zeros((x, y, 1), dtype=np.uint8)), axis=-1)
+            _image = np.concatenate(
+                (_image, np.zeros((x, y, 1), dtype=np.uint8)), axis=-1
+            )
 
         _image = np.ascontiguousarray(_image[:, :, -3::].astype(np.uint8))
 
         self.image = _image
         self._display_image_buffer = _image.copy()
 
         return self
@@ -144,15 +152,15 @@
         h, w, _ = self._display_image_buffer.shape
 
         _image = self._display_image_buffer[:, :, 0:3]
         _image = np.ascontiguousarray(_image.astype(np.uint8))
 
         return QImage(_image.data, w, h, 3 * w, QImage.Format_RGB888)
 
-    def get_selected(self):
+    def get_selected(self) -> List[Stereocilia]:
         selected = []
         for stereocilia in self.get_stereocilia():
             if stereocilia.is_selected():
                 selected.append(stereocilia)
         return selected
 
     def delete_selected(self):
@@ -198,7 +206,13 @@
         return self
 
     def clear_stereocilia(self):
         self.seleted = None
         self.stereocilia = []
         self._candidate_stereocilia = []
         return self
+
+    def deselect_all(self):
+        for s in self._candidate_stereocilia:
+            s.deselect()
+        for s in self.stereocilia:
+            s.deselect()
```

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/state/stereocilia.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/state/stereocilia.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     vertex_point_smaller_size: int
     unselected_border_thickness: int
     selected_border_thickness: int
     scale: float
 
 
 default_style: StyleDict = {
-    'row1_border_color': QColor(255, 0, 0, 128),
-    'row1_fill_color': QColor(255, 0, 0, 50),
-    'row2_border_color': QColor(0, 255, 0, 128),
-    'row2_fill_color': QColor(0, 255, 0, 50),
-    'row3_border_color': QColor(0, 0, 255, 128),
-    'row3_fill_color': QColor(0, 0, 255, 50),
-    'vertex_point_larger_size': 8,
-    'vertex_point_smaller_size': 5,
-    'unselected_border_thickness': 1,
-    'selected_border_thickness': 3,
-    'scale': 1
+    "row1_border_color": QColor(255, 0, 0, 128),
+    "row1_fill_color": QColor(255, 0, 0, 50),
+    "row2_border_color": QColor(0, 255, 0, 128),
+    "row2_fill_color": QColor(0, 255, 0, 50),
+    "row3_border_color": QColor(0, 0, 255, 128),
+    "row3_fill_color": QColor(0, 0, 255, 50),
+    "vertex_point_larger_size": 8,
+    "vertex_point_smaller_size": 5,
+    "unselected_border_thickness": 1,
+    "selected_border_thickness": 3,
+    "scale": 1,
 }
 
 
 class Stereocilia:
     """
     Object which can be drawn on a hair bundle
     """
@@ -83,75 +83,78 @@
 
     def set_vertices(self, vertices: List[QPointF]):
         self.vertices = vertices
         return self
 
     def set_vertex_at_index(self, vertex: QPointF, index: int):
         assert index < len(
-            self.vertices), f'stereocilia {self} has {len(self.vertices)}, but tried to access vertex at index: {index}'
-        raise RuntimeError('not needed')
+            self.vertices
+        ), f"stereocilia {self} has {len(self.vertices)}, but tried to access vertex at index: {index}"
+        raise RuntimeError("not needed")
 
         self.vertices[index] = vertex
 
     def get_vertices(self):
         return self.vertices
 
     def clear_vertices(self):
         self.vertices = []
         return self
 
     def set_label(self, label: str | int):
-        _valid = {'short': 0, 'middle': 1, 'tall': 2}
+        _valid = {"short": 0, "middle": 1, "tall": 2}
         if isinstance(label, str):
             self.label = _valid[label]
         elif isinstance(label, int) and label in [0, 1, 2]:
             self.label = label
         else:
-            raise ValueError(f'cannot self.label to invalid value: {label}')
+            raise ValueError(f"cannot self.label to invalid value: {label}")
 
         return self
 
     def get_label(self):
         return self.label
 
     def get_label_str(self):
-        _valid = {0: 'short', 1: 'middle', 2: 'tall'}
-        return _valid[self.label] if self.label is not None else ''
+        _valid = {0: "short", 1: "middle", 2: "tall"}
+        return _valid[self.label] if self.label is not None else ""
 
     def clear_label(self):
         self.label = None
         return self
 
     def paint(self, painter: QPainter, offset: QPointF, style: StyleDict):
         oldpen = painter.pen()
 
         style_dict = copy(self.default_style_dict)
         for k, v in style.items():
             style_dict[k] = v
 
         if self.label == 0:
-            border_color = style_dict['row1_border_color']
-            fill_color = style_dict['row1_fill_color']
+            border_color = style_dict["row1_border_color"]
+            fill_color = style_dict["row1_fill_color"]
         elif self.label == 1:
-            border_color = style_dict['row2_border_color']
-            fill_color = style_dict['row2_fill_color']
+            border_color = style_dict["row2_border_color"]
+            fill_color = style_dict["row2_fill_color"]
         elif self.label == 2:
-            border_color = style_dict['row3_border_color']
-            fill_color = style_dict['row3_fill_color']
+            border_color = style_dict["row3_border_color"]
+            fill_color = style_dict["row3_fill_color"]
         else:
             border_color = QColor(100, 100, 100, 255)
             fill_color = QColor(100, 100, 100, 255)
 
         pen = QPen()
         pen.setColor(border_color)
 
         if self.is_selected():
-            pen.setWidthF(style_dict['selected_border_thickness'] / style_dict['scale'])
+            pen.setWidthF(style_dict["selected_border_thickness"] / style_dict["scale"])
         else:
-            pen.setWidthF(style_dict['unselected_border_thickness'] / style_dict['scale'])
+            pen.setWidthF(
+                style_dict["unselected_border_thickness"] / style_dict["scale"]
+            )
 
         painter.setPen(pen)
 
         brush = QBrush()
         brush.setStyle(Qt.SolidPattern)
         brush.setColor(fill_color)
         painter.setBrush(brush)
@@ -159,35 +162,35 @@
         verts = [v + offset for v in self.vertices]
         polygon = QPolygonF(verts)
         painter.drawPolygon(polygon)
 
         if self.is_selected():
             pen = QPen()
             pen.setCapStyle(Qt.RoundCap)
-            pen.setWidthF(style_dict['vertex_point_larger_size'] / style_dict['scale'])
-            pen.setColor('white')
+            pen.setWidthF(style_dict["vertex_point_larger_size"] / style_dict["scale"])
+            pen.setColor("white")
             painter.setPen(pen)
             for v in verts:
                 painter.drawPoint(v)
 
-            pen.setWidthF(style_dict['vertex_point_smaller_size'] / style_dict['scale'])
-            pen.setColor('black')
+            pen.setWidthF(style_dict["vertex_point_smaller_size"] / style_dict["scale"])
+            pen.setColor("black")
             painter.setPen(pen)
             for v in verts:
                 painter.drawPoint(v)
 
         painter.setPen(oldpen)
 
     def is_inside(self, point: QPointF) -> bool:
         " returns true if the coordinate x,y is inside the polygon "
         return self.is_point_inside_polygon(point, self.vertices)
 
     def return_clicked_vertex(self, point: QPointF, thr: float) -> QPointF | None:
         distances = [self._dist(vert, point) for vert in self.vertices]
-        mindist = float('inf')
+        mindist = float("inf")
         mindist_index = -1
         for i, dist in enumerate(distances):
             if dist < thr:
                 mindist_index = i if dist <= mindist else mindist_index
                 mindist = min(dist, mindist)
         if mindist_index == -1:
             return None
@@ -195,16 +198,15 @@
             return self.vertices[mindist_index]
 
     @staticmethod
     def _dist(a: QPointF, b: QPointF) -> float:
         return sqrt((b.x() - a.x()) ** 2 + (b.y() - a.y()) ** 2)
 
     @staticmethod
-    def is_point_inside_polygon(point: QPointF,
-                                vertices: List[QPointF]) -> bool:
+    def is_point_inside_polygon(point: QPointF, vertices: List[QPointF]) -> bool:
         """
         Calculates if a point is inside a polygon.
             ien.setColor(color)
 
         :param point: [x0, y0]
         :param vertices: List[[x0, y0], ...]
 
@@ -212,18 +214,21 @@
         """
         # Implementation of the Ray Casting Algorithm
         # Source: https://stackoverflow.com/a/21337692
         x, y = point.x(), point.y()
         inside = False
         for i in range(len(vertices)):
             j = (i + 1) % len(vertices)
-            if ((vertices[i].y() > y) != (vertices[j].y() > y) and
-                    (x < (vertices[j].x() - vertices[i].x()) * (y - vertices[i].y()) / (
-                            vertices[j].y() - vertices[i].y()) +
-                     vertices[i].x())):
+            if (vertices[i].y() > y) != (vertices[j].y() > y) and (
+                x
+                < (vertices[j].x() - vertices[i].x())
+                * (y - vertices[i].y())
+                / (vertices[j].y() - vertices[i].y())
+                + vertices[i].x()
+            ):
                 inside = not inside
         return inside
 
     def x(self) -> List[float]:
         return [p.x() for p in self.vertices]
 
     def y(self) -> List[float]:
@@ -257,25 +262,25 @@
 
         def _fast_dist(x0, y0, x1, y1) -> float:
             return (x1 - x0) ** 2 + (y1 - y0) ** 2
 
         mouse_x, mouse_y = point.x(), point.y()
 
         _line = [
-            _fit_line(self.vertices[i].x(), self.vertices[i].y(), self.vertices[i-1].x(), self.vertices[i-1].y())
-            for i
-            in range(len(self.vertices))
-        ]
-        _close = [
-            _closest_to_line(mouse_x, mouse_y, m, b) for (m, b) in _line
+            _fit_line(
+                self.vertices[i].x(),
+                self.vertices[i].y(),
+                self.vertices[i - 1].x(),
+                self.vertices[i - 1].y(),
+            )
+            for i in range(len(self.vertices))
         ]
+        _close = [_closest_to_line(mouse_x, mouse_y, m, b) for (m, b) in _line]
 
-        dist = [
-            _fast_dist(mouse_x, mouse_y, x0, y0) for (x0, y0) in _close
-        ]
+        dist = [_fast_dist(mouse_x, mouse_y, x0, y0) for (x0, y0) in _close]
 
         ind = np.argmin(dist)
 
         if dist[ind] > thr:
             return None
 
         v0 = self.vertices[ind]
@@ -290,18 +295,21 @@
 
         _x0 = min(x0, x1)
         _x1 = max(x0, x1)
 
         vert_x = min(max(vert_x, _x0), _x1)
         vert_y = vert_x * m + b
 
-        print(f'{vert_y=} = {m=} * {vert_x=} + {b=}')
         return QPointF(vert_x, vert_y)
 
-    def insert_vertex(self, vertex: QPointF):
+    def insert_vertex(self, vertex: QPointF | None):
+
+        if vertex is None:
+            return
+
         def _fit_line(x0, y0, x1, y1) -> Tuple[float, float]:
             m = (y1 - y0) / (x1 - x0 + 1e-8)
             b = y1 - m * x1
             return m, b
 
         def _closest_to_line(x, y, m, b):
             vert_x = (x + m * (y - b)) / (1 + m ** 2)
@@ -310,24 +318,23 @@
             return vert_x, vert_y
 
         def _fast_dist(x0, y0, x1, y1) -> float:
             return (x1 - x0) ** 2 + (y1 - y0) ** 2
 
         mouse_x, mouse_y = vertex.x(), vertex.y()
 
-
         _line = [
-            _fit_line(self.vertices[i].x(), self.vertices[i].y(), self.vertices[i-1].x(), self.vertices[i-1].y())
-            for i
-            in range(len(self.vertices))
-        ]
-        _close = [
-            _closest_to_line(mouse_x, mouse_y, m, b) for (m, b) in _line
+            _fit_line(
+                self.vertices[i].x(),
+                self.vertices[i].y(),
+                self.vertices[i - 1].x(),
+                self.vertices[i - 1].y(),
+            )
+            for i in range(len(self.vertices))
         ]
+        _close = [_closest_to_line(mouse_x, mouse_y, m, b) for (m, b) in _line]
 
-        dist = [
-            _fast_dist(mouse_x, mouse_y, x0, y0) for (x0, y0) in _close
-        ]
+        dist = [_fast_dist(mouse_x, mouse_y, x0, y0) for (x0, y0) in _close]
 
         ind = np.argmin(dist)
 
         self.vertices.insert(ind, vertex)
```

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/utils/io.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/utils/io.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/control.py` & `ciliaseg-0.0.6.dev20240417/ciliaseg/widgets/control.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/SOURCES.txt` & `ciliaseg-0.0.6.dev20240417/ciliaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

