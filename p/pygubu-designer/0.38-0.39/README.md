# Comparing `tmp/pygubu-designer-0.38.tar.gz` & `tmp/pygubu_designer-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygubu-designer-0.38.tar", last modified: Sun Feb 11 06:11:04 2024, max compression
+gzip compressed data, was "pygubu_designer-0.39.tar", last modified: Wed Apr 17 00:46:57 2024, max compression
```

## Comparing `pygubu-designer-0.38.tar` & `pygubu_designer-0.39.tar`

### file list

```diff
@@ -1,721 +1,759 @@
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.052385 pygubu-designer-0.38/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       67 2022-06-27 01:27:37.000000 pygubu-designer-0.38/AUTHORS
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5128 2022-09-21 21:46:21.000000 pygubu-designer-0.38/LEEME.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    35064 2022-08-14 23:01:15.000000 pygubu-designer-0.38/LICENSE.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6509 2022-08-14 23:01:15.000000 pygubu-designer-0.38/LISEZMOI.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      248 2022-08-13 03:36:27.000000 pygubu-designer-0.38/MANIFEST.in
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7697 2024-02-11 06:11:04.048385 pygubu-designer-0.38/PKG-INFO
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5007 2022-09-05 01:14:44.000000 pygubu-designer-0.38/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.624378 pygubu-designer-0.38/development/
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)     6434 2023-06-19 23:02:27.000000 pygubu-designer-0.38/development/create-imgs.py
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)     6876 2024-02-11 06:08:43.000000 pygubu-designer-0.38/development/dev-notes.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2186 2023-07-10 01:17:49.000000 pygubu-designer-0.38/development/devtool.py
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)     3885 2023-06-19 23:02:29.000000 pygubu-designer-0.38/development/devtool.sh
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.624378 pygubu-designer-0.38/development/new-designer-icons/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.624378 pygubu-designer-0.38/development/new-designer-icons/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2277 2023-01-16 18:51:44.000000 pygubu-designer-0.38/development/new-designer-icons/__pycache__/testnewiconsapp.cpython-311.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2780 2023-01-16 05:38:47.000000 pygubu-designer-0.38/development/new-designer-icons/main.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.652379 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2129 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/button.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7010 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/button.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3744 2023-01-15 21:44:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/canvas.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4072 2023-01-15 21:44:22.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/canvas.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2101 2023-01-17 02:12:40.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/combobox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     9271 2023-01-17 02:12:35.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/combobox.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1252 2023-01-15 22:41:22.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/default.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4185 2023-01-15 22:13:29.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/default.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      665 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/entry.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3834 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/entry.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1552 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/frame.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6047 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/frame.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1142 2023-01-15 21:09:25.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/label.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5074 2023-01-15 21:10:01.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/label.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1666 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/labelframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6735 2023-01-17 03:53:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/labelframe.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2133 2023-01-17 03:34:34.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/menubutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     8598 2023-01-17 03:34:30.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/menubutton.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      962 2023-01-16 19:11:46.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook-tab.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3043 2023-01-16 19:12:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook-tab.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1060 2023-01-16 20:29:13.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3693 2023-01-16 20:29:02.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      797 2023-01-17 01:34:55.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3257 2023-01-17 01:37:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      782 2023-01-17 01:33:01.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3238 2023-01-17 01:33:20.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1077 2023-01-15 21:28:54.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/progressbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5356 2023-01-15 21:29:31.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/progressbar.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      257 2023-01-15 23:05:13.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/rect848.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1786 2023-01-17 02:48:00.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/spinbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     8481 2023-01-17 02:47:53.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/spinbutton.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1126 2023-01-17 03:00:24.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/textview.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6381 2023-01-17 03:00:15.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/textview.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      867 2023-01-15 21:34:06.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/toplevel.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3229 2023-01-15 21:40:40.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/toplevel.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1068 2023-01-15 22:23:58.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview-col.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5481 2023-01-15 22:24:06.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview-col.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      935 2023-01-15 22:22:00.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4893 2023-01-15 22:21:47.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2489 2023-01-15 22:38:13.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/viewport.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7036 2023-01-15 22:38:17.000000 pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/viewport.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4315 2023-01-15 20:59:40.000000 pygubu-designer-0.38/development/new-designer-icons/template.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7552 2023-01-15 05:57:56.000000 pygubu-designer-0.38/development/new-designer-icons/testnewicons.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      854 2023-01-16 05:38:47.000000 pygubu-designer-0.38/development/new-designer-icons/testnewiconsapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.664379 pygubu-designer-0.38/development/pygubuLogo/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5501 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/Python-logo-notext.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   174121 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/logo_pygubu .ico
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   101863 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/logo_pygubu.icns
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   174121 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/logo_pygubu.ico
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   175900 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/logo_pygubu.xcf
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   124131 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/pyGubu_newLogo.svg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       92 2022-08-14 23:01:14.000000 pygubu-designer-0.38/development/pygubuLogo/rootOfSVGs.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10232 2022-08-13 03:36:28.000000 pygubu-designer-0.38/development/pygubuLogo/tcl-tk.svg
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      627 2023-06-19 23:02:30.000000 pygubu-designer-0.38/development/pygubudesigner_.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       11 2022-08-15 00:47:17.000000 pygubu-designer-0.38/development/requirements.txt
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.676379 pygubu-designer-0.38/examples/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.680379 pygubu-designer-0.38/examples/7guis/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.680379 pygubu-designer-0.38/examples/7guis/01_counter/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1256 2022-07-06 23:05:06.000000 pygubu-designer-0.38/examples/7guis/01_counter/counter.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      798 2022-07-06 23:09:13.000000 pygubu-designer-0.38/examples/7guis/01_counter/counterapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.680379 pygubu-designer-0.38/examples/7guis/02_temperature_converter/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2687 2022-07-07 00:11:21.000000 pygubu-designer-0.38/examples/7guis/02_temperature_converter/tempconv.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1648 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/7guis/02_temperature_converter/tempconvapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.684379 pygubu-designer-0.38/examples/7guis/03_flight_Booker/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2648 2022-07-11 00:53:14.000000 pygubu-designer-0.38/examples/7guis/03_flight_Booker/flight_booker.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3212 2022-08-15 00:05:30.000000 pygubu-designer-0.38/examples/7guis/03_flight_Booker/flightbookerapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.684379 pygubu-designer-0.38/examples/7guis/04_timer/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4089 2022-07-11 03:51:30.000000 pygubu-designer-0.38/examples/7guis/04_timer/timer.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1777 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/7guis/04_timer/timerapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       81 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/7guis/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      347 2022-07-06 22:57:52.000000 pygubu-designer-0.38/examples/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      546 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/binding.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      960 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/button_cb.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2053 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/button_cb.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.580378 pygubu-designer-0.38/examples/canvas/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.684379 pygubu-designer-0.38/examples/canvas/canvas-scrollregion/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      106 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/canvas/canvas-scrollregion/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5196 2022-08-14 21:43:22.000000 pygubu-designer-0.38/examples/canvas/canvas-scrollregion/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5211 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/canvas/canvas-scrollregion/myapp.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      842 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/canvas_example.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.688379 pygubu-designer-0.38/examples/command_properties/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1221 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/command_properties/command_properties.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2641 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/command_properties/command_properties.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1256 2022-08-14 21:43:21.000000 pygubu-designer-0.38/examples/command_properties/command_properties2.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3116 2022-08-14 21:43:22.000000 pygubu-designer-0.38/examples/commands.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    18575 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/commands.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.688379 pygubu-designer-0.38/examples/control_variables/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      584 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/control_variables/controlvariables.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3634 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/control_variables/controlvariables.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.692379 pygubu-designer-0.38/examples/custom_widget/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      436 2022-08-14 23:01:15.000000 pygubu-designer-0.38/examples/custom_widget/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.696380 pygubu-designer-0.38/examples/custom_widget/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      547 2022-03-17 00:59:57.000000 pygubu-designer-0.38/examples/custom_widget/__pycache__/customappwidgets.cpython-38.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      591 2022-08-18 01:16:31.000000 pygubu-designer-0.38/examples/custom_widget/__pycache__/timerappwidgets.cpython-310.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      576 2022-04-15 19:20:34.000000 pygubu-designer-0.38/examples/custom_widget/__pycache__/timerappwidgets.cpython-38.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2301 2022-08-18 01:16:31.000000 pygubu-designer-0.38/examples/custom_widget/__pycache__/timewidget.cpython-310.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2286 2022-04-15 19:20:34.000000 pygubu-designer-0.38/examples/custom_widget/__pycache__/timewidget.cpython-38.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1311 2022-03-27 00:01:32.000000 pygubu-designer-0.38/examples/custom_widget/timer_main.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      515 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/custom_widget/timerapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      287 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/custom_widget/timerappwidgets.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2363 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/custom_widget/timewidget.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.696380 pygubu-designer-0.38/examples/customtkinter/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      174 2023-03-02 04:18:11.000000 pygubu-designer-0.38/examples/customtkinter/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.696380 pygubu-designer-0.38/examples/customtkinter/complex/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    22578 2023-03-02 04:18:11.000000 pygubu-designer-0.38/examples/customtkinter/complex/complex_demo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2365 2023-03-02 04:18:11.000000 pygubu-designer-0.38/examples/customtkinter/complex/complexdemoapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.696380 pygubu-designer-0.38/examples/customtkinter/simple/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6284 2023-03-02 04:18:11.000000 pygubu-designer-0.38/examples/customtkinter/simple/simple_demo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1269 2023-03-02 04:18:11.000000 pygubu-designer-0.38/examples/customtkinter/simple/simpledemoapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.700379 pygubu-designer-0.38/examples/dialogs/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       51 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/dialogs/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.700379 pygubu-designer-0.38/examples/dialogs/demo1/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       73 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/dialogs/demo1/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1178 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/dialogs/demo1/demo.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5699 2022-07-05 02:56:28.000000 pygubu-designer-0.38/examples/dialogs/demo1/demo.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.704380 pygubu-designer-0.38/examples/dialogs/demo2/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       95 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/dialogs/demo2/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1319 2022-08-14 21:43:21.000000 pygubu-designer-0.38/examples/dialogs/demo2/demo.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4523 2022-07-05 02:56:28.000000 pygubu-designer-0.38/examples/dialogs/demo2/demo.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.704380 pygubu-designer-0.38/examples/dialogs/demo3/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       98 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/dialogs/demo3/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4883 2022-08-14 21:43:22.000000 pygubu-designer-0.38/examples/dialogs/demo3/demo.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     9704 2022-07-05 02:56:28.000000 pygubu-designer-0.38/examples/dialogs/demo3/demo.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.708380 pygubu-designer-0.38/examples/dialogs/demo4/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      314 2023-01-18 02:21:28.000000 pygubu-designer-0.38/examples/dialogs/demo4/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.708380 pygubu-designer-0.38/examples/dialogs/demo4/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1835 2023-01-18 00:24:03.000000 pygubu-designer-0.38/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-310.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6987 2023-01-18 00:11:57.000000 pygubu-designer-0.38/examples/dialogs/demo4/settingsdemo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1002 2023-01-18 02:21:28.000000 pygubu-designer-0.38/examples/dialogs/demo4/settingsdemoapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1319 2023-01-18 02:21:28.000000 pygubu-designer-0.38/examples/dialogs/demo4/settingsdialog.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1471 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/example_grid_rc.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1631 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/example_grid_rc_2.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.584378 pygubu-designer-0.38/examples/forms/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.708380 pygubu-designer-0.38/examples/forms/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1276 2023-05-25 03:22:01.000000 pygubu-designer-0.38/examples/forms/__pycache__/formsdemo1base.cpython-310.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1937 2024-01-21 03:00:06.000000 pygubu-designer-0.38/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      723 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/framepad.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.712380 pygubu-designer-0.38/examples/helloworld/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       82 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/helloworld/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      740 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/helloworld/helloworld.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1178 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/helloworld/helloworld.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      755 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/helloworld/holamundo.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1176 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/helloworld/holamundo.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.716380 pygubu-designer-0.38/examples/image_property/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4015 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/image_property/green.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      710 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/image_property/image_property.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1682 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/image_property/image_property.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3270 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/image_property/red.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3572 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/image_property/yellow.gif
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.716380 pygubu-designer-0.38/examples/integration_with_cxFreeze/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      337 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.720380 pygubu-designer-0.38/examples/integration_with_cxFreeze/imgs/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/imgs/ps_circle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/imgs/ps_cross.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/imgs/ps_square.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6612 2022-08-16 20:22:58.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/myapp.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2529 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/integration_with_cxFreeze/setup.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.724380 pygubu-designer-0.38/examples/integration_with_nuitka/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      366 2022-04-15 23:40:48.000000 pygubu-designer-0.38/examples/integration_with_nuitka/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.724380 pygubu-designer-0.38/examples/integration_with_nuitka/imgs/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_nuitka/imgs/MenuIcon4.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_nuitka/imgs/ps_circle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_nuitka/imgs/ps_cross.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_nuitka/imgs/ps_square.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_nuitka/imgs/ps_triangle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6510 2022-08-14 21:43:22.000000 pygubu-designer-0.38/examples/integration_with_nuitka/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.38/examples/integration_with_nuitka/myapp.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.728380 pygubu-designer-0.38/examples/integration_with_py2exe/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      258 2022-04-15 22:25:27.000000 pygubu-designer-0.38/examples/integration_with_py2exe/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.732380 pygubu-designer-0.38/examples/integration_with_py2exe/imgs/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_py2exe/imgs/MenuIcon4.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_py2exe/imgs/ps_circle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_py2exe/imgs/ps_cross.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_py2exe/imgs/ps_square.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_py2exe/imgs/ps_triangle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6602 2022-08-14 21:43:22.000000 pygubu-designer-0.38/examples/integration_with_py2exe/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.38/examples/integration_with_py2exe/myapp.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2731 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/integration_with_py2exe/setup.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.736380 pygubu-designer-0.38/examples/integration_with_pyinstaller/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      291 2022-04-15 22:36:07.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.736380 pygubu-designer-0.38/examples/integration_with_pyinstaller/imgs/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/imgs/ps_circle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/imgs/ps_cross.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/imgs/ps_square.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6602 2022-08-14 21:43:22.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2513 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/myapp.spec
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.38/examples/integration_with_pyinstaller/myapp.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.740380 pygubu-designer-0.38/examples/integration_with_tkcalendar/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      582 2022-08-14 23:01:15.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.740380 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.744380 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      602 2022-04-15 19:22:18.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/__pycache__/tkcalendarwidgets.cpython-38.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1141 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/main.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      526 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       34 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/requirements.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      317 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.744380 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.748380 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      825 2022-08-18 01:20:29.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-310.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      810 2022-04-15 19:24:09.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-38.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1750 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/main.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      547 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       34 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/requirements.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      644 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.748380 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.752380 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/__pycache__/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1607 2022-08-18 01:19:22.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-310.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1596 2022-07-31 21:44:20.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-38.pyc
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2190 2022-07-31 00:06:09.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/main.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      755 2022-07-31 00:06:09.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/myapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       34 2022-07-31 00:06:09.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/requirements.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1975 2022-08-28 07:44:47.000000 pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.752380 pygubu-designer-0.38/examples/integration_with_zipapp/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      365 2022-09-19 01:07:31.000000 pygubu-designer-0.38/examples/integration_with_zipapp/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   355908 2022-09-19 00:05:52.000000 pygubu-designer-0.38/examples/integration_with_zipapp/demoapp.pyz
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.592378 pygubu-designer-0.38/examples/integration_with_zipapp/src/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.756380 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-11 23:06:21.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/__init__.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.760380 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-12 02:32:35.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3445 2022-09-19 00:02:37.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.760380 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/extradata/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-18 01:57:22.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      320 2022-09-19 00:20:17.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4015 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/green.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      556 2022-09-11 22:28:25.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/info.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3270 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/red.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3572 2022-03-19 02:20:06.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1013 2022-09-19 00:20:17.000000 pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/main.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.764381 pygubu-designer-0.38/examples/jpg_image_on_canvas/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      825 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/jpg_image_on_canvas/demoapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1244 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/jpg_image_on_canvas/demoapp.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       14 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/jpg_image_on_canvas/requirements.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    38211 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/jpg_image_on_canvas/seaside400.jpg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3187 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/menubutton.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1347 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/menuexample.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.768380 pygubu-designer-0.38/examples/notebook/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5153 2022-12-10 21:50:50.000000 pygubu-designer-0.38/examples/notebook/demo1.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1379 2022-12-10 21:53:15.000000 pygubu-designer-0.38/examples/notebook/demo1app.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1835 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/panedwindow.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3131 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/panes_and_notebooks.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.768380 pygubu-designer-0.38/examples/pathchooserdemo/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       32 2023-01-01 21:58:08.000000 pygubu-designer-0.38/examples/pathchooserdemo/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.768380 pygubu-designer-0.38/examples/pathchooserdemo/demo1/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1897 2023-01-01 21:36:25.000000 pygubu-designer-0.38/examples/pathchooserdemo/demo1/pathchooserdemo.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3220 2023-01-01 21:36:27.000000 pygubu-designer-0.38/examples/pathchooserdemo/demo1/pathchooserdemo.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.772381 pygubu-designer-0.38/examples/pathchooserdemo/demo2/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2644 2023-01-01 22:13:59.000000 pygubu-designer-0.38/examples/pathchooserdemo/demo2/pathchooserdemo.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10131 2023-01-17 17:00:07.000000 pygubu-designer-0.38/examples/pathchooserdemo/demo2/pathchooserdemo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1840 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/scrollbarhelper.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10765 2021-10-11 04:39:54.000000 pygubu-designer-0.38/examples/scrolledframe-layouts.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     9388 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/scrolledframe.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.772381 pygubu-designer-0.38/examples/scrolledtext/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4030 2022-04-16 00:57:31.000000 pygubu-designer-0.38/examples/scrolledtext/scrolledtext_demo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      977 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/scrolledtext/scrolledtextdemoapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.776381 pygubu-designer-0.38/examples/static_image/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      539 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/static_image/demoapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1676 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/static_image/demoapp.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    23336 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/static_image/logo_253.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       16 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/static_image/requirements.txt
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.596378 pygubu-designer-0.38/examples/text/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.776381 pygubu-designer-0.38/examples/text/logwindowdemo/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3075 2023-01-04 05:41:56.000000 pygubu-designer-0.38/examples/text/logwindowdemo/demo1.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1714 2023-01-04 05:47:58.000000 pygubu-designer-0.38/examples/text/logwindowdemo/demo1app.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.780381 pygubu-designer-0.38/examples/tk_window/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      144 2023-07-10 01:17:49.000000 pygubu-designer-0.38/examples/tk_window/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4015 2023-07-10 01:17:49.000000 pygubu-designer-0.38/examples/tk_window/green.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1354 2023-07-10 01:17:49.000000 pygubu-designer-0.38/examples/tk_window/tkdemo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      600 2023-07-10 01:17:49.000000 pygubu-designer-0.38/examples/tk_window/tkdemoapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.784381 pygubu-designer-0.38/examples/toplevel_centered/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      154 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/toplevel_centered/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1216 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/toplevel_centered/centered_demo1.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1317 2023-06-22 03:13:24.000000 pygubu-designer-0.38/examples/toplevel_centered/centered_demo2.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1020 2023-06-22 03:13:24.000000 pygubu-designer-0.38/examples/toplevel_centered/demo.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.784381 pygubu-designer-0.38/examples/toplevel_menu/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       64 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/toplevel_menu/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1291 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/toplevel_menu/menu.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2470 2022-03-19 02:20:07.000000 pygubu-designer-0.38/examples/toplevel_menu/menu.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.784381 pygubu-designer-0.38/examples/treeview/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       16 2022-12-06 19:21:35.000000 pygubu-designer-0.38/examples/treeview/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.788381 pygubu-designer-0.38/examples/treeview/demo1/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       43 2022-12-06 19:22:00.000000 pygubu-designer-0.38/examples/treeview/demo1/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1496 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/treeview/demo1/treeview.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3473 2022-03-19 02:20:07.000000 pygubu-designer-0.38/examples/treeview/demo1/treeview.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.792381 pygubu-designer-0.38/examples/treeview/demo2/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       64 2022-12-06 19:22:48.000000 pygubu-designer-0.38/examples/treeview/demo2/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    23736 2022-12-06 19:15:41.000000 pygubu-designer-0.38/examples/treeview/demo2/columns_stretching.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2712 2022-12-06 19:24:11.000000 pygubu-designer-0.38/examples/treeview/demo2/columnsstretchingdemo.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.792381 pygubu-designer-0.38/examples/treeview_editable/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       28 2023-07-21 03:20:32.000000 pygubu-designer-0.38/examples/treeview_editable/README.md
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.792381 pygubu-designer-0.38/examples/treeview_editable/demo1/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5044 2023-07-21 03:20:32.000000 pygubu-designer-0.38/examples/treeview_editable/demo1/demoapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7875 2023-07-21 03:20:32.000000 pygubu-designer-0.38/examples/treeview_editable/demo1/demoapp.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.796381 pygubu-designer-0.38/examples/treeview_editable/demo2/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5944 2023-07-21 03:20:32.000000 pygubu-designer-0.38/examples/treeview_editable/demo2/demo2.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3432 2023-07-21 03:20:32.000000 pygubu-designer-0.38/examples/treeview_editable/demo2/demo2app.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.796381 pygubu-designer-0.38/examples/treeview_filterable/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       30 2023-07-21 03:20:33.000000 pygubu-designer-0.38/examples/treeview_filterable/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5404 2023-07-21 03:20:33.000000 pygubu-designer-0.38/examples/treeview_filterable/demo.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2886 2023-07-21 03:20:33.000000 pygubu-designer-0.38/examples/treeview_filterable/demoapp.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.800381 pygubu-designer-0.38/examples/user_input/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-14 23:01:14.000000 pygubu-designer-0.38/examples/user_input/README.md
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       16 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/user_input/requirements.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    28967 2022-09-17 20:39:05.000000 pygubu-designer-0.38/examples/user_input/userinput.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3730 2022-09-17 21:03:37.000000 pygubu-designer-0.38/examples/user_input/userinputapp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      883 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/variables.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4346 2021-01-10 18:38:24.000000 pygubu-designer-0.38/examples/vscrolledframe.ui
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.804381 pygubu-designer-0.38/examples/windowdeleteevent/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      887 2022-07-13 00:05:26.000000 pygubu-designer-0.38/examples/windowdeleteevent/demo1.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1122 2022-03-19 02:20:07.000000 pygubu-designer-0.38/examples/windowdeleteevent/demo1.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      847 2022-07-31 01:37:40.000000 pygubu-designer-0.38/examples/windowdeleteevent/demo2.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1271 2022-07-31 01:37:40.000000 pygubu-designer-0.38/examples/windowdeleteevent/demo2.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)   104249 2022-04-16 04:21:16.000000 pygubu-designer-0.38/pygubu-designer.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2434 2024-02-11 06:09:12.000000 pygubu-designer-0.38/pyproject.toml
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       38 2024-02-11 06:11:04.052385 pygubu-designer-0.38/setup.cfg
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       61 2022-08-13 03:36:27.000000 pygubu-designer-0.38/setup.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.600378 pygubu-designer-0.38/src/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.048385 pygubu-designer-0.38/src/pygubu_designer.egg-info/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7697 2024-02-11 06:11:03.000000 pygubu-designer-0.38/src/pygubu_designer.egg-info/PKG-INFO
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    35797 2024-02-11 06:11:03.000000 pygubu-designer-0.38/src/pygubu_designer.egg-info/SOURCES.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)        1 2024-02-11 06:11:03.000000 pygubu-designer-0.38/src/pygubu_designer.egg-info/dependency_links.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       65 2024-02-11 06:11:03.000000 pygubu-designer-0.38/src/pygubu_designer.egg-info/entry_points.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      443 2024-02-11 06:11:03.000000 pygubu-designer-0.38/src/pygubu_designer.egg-info/requires.txt
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       15 2024-02-11 06:11:03.000000 pygubu-designer-0.38/src/pygubu_designer.egg-info/top_level.txt
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.820381 pygubu-designer-0.38/src/pygubudesigner/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      198 2024-02-11 06:09:12.000000 pygubu-designer-0.38/src/pygubudesigner/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      122 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/__main__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1049 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/actions.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6314 2022-08-14 21:43:22.000000 pygubu-designer-0.38/src/pygubudesigner/bindingseditor.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.824381 pygubu-designer-0.38/src/pygubudesigner/codegen/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       76 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/codegen/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    18807 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/codegen/codebuilder.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    13092 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/codegen/scriptgenerator.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    11033 2022-08-15 00:04:47.000000 pygubu-designer-0.38/src/pygubudesigner/containerlayouteditor.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.608378 pygubu-designer-0.38/src/pygubudesigner/data/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.828381 pygubu-designer-0.38/src/pygubudesigner/data/code_templates/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2945 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/data/code_templates/app.py.mako
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      453 2023-06-03 02:35:17.000000 pygubu-designer-0.38/src/pygubudesigner/data/code_templates/base.py.mako
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1635 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/data/code_templates/customstyles.py.mako
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2033 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/data/code_templates/script.py.mako
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1083 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/data/code_templates/widget.py.mako
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.604378 pygubu-designer-0.38/src/pygubudesigner/data/images/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.840382 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       70 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       71 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       81 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/bin-16.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       85 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       61 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/close.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       73 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/download3-16.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/download3-32.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      230 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/mglass.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      377 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/property_invalid.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      875 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/pygubu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4897 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/pygubu200.gif
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.604378 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.880382 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      107 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      352 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      128 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      224 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      231 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       75 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      327 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1120 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      126 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      100 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      327 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      109 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.920383 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      132 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      197 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      197 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      599 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      129 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      156 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      195 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      133 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      114 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      129 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      142 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      131 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      133 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      156 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.924383 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      592 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      567 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      357 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      572 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.932383 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      194 2023-06-19 23:02:31.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/arrow-left2.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      184 2023-06-19 23:02:32.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/arrow-right2.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      162 2023-06-19 23:02:33.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/bin-16.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      353 2023-06-19 23:02:34.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      334 2023-06-19 23:02:34.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/circle-left.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      333 2023-06-19 23:02:35.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/circle-right.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      170 2023-06-19 23:02:36.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/download3-16.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      214 2023-06-19 23:02:37.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/download3-32.png
--rwxr-xr-x   0 ministerio  (1000) ministerio  (1000)      316 2023-06-19 23:02:37.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/mglass.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      603 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/property_invalid.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4777 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/pygubu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    15896 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/pygubu200.png
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.604378 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.968384 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      488 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      613 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      389 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      480 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      509 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      426 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      480 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      509 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      638 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      488 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1088 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      524 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      356 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      706 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      527 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      334 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      433 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      325 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      508 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      431 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      627 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      426 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      389 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      291 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      638 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      524 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      613 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      356 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      706 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      435 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      545 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      508 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      431 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      293 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      627 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.004384 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      161 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      263 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      169 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      186 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      339 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      148 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      186 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      339 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      181 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      161 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      689 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      179 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      143 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      205 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      202 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      323 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      257 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      206 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      148 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      169 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      116 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      181 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      179 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      263 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      143 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      205 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      175 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      257 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      107 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      206 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.008384 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      705 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      619 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      611 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      673 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.008384 pygubu-designer-0.38/src/pygubudesigner/data/locale/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.604378 pygubu-designer-0.38/src/pygubudesigner/data/locale/de/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.012384 pygubu-designer-0.38/src/pygubudesigner/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3438 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      425 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.608378 pygubu-designer-0.38/src/pygubudesigner/data/locale/es/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.012384 pygubu-designer-0.38/src/pygubudesigner/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12801 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      789 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    57384 2023-07-10 01:17:49.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/pygubu-designer.pot
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    18853 2023-07-10 01:17:49.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/pygubu.pot
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.608378 pygubu-designer-0.38/src/pygubudesigner/data/locale/tr/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.012384 pygubu-designer-0.38/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5317 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      393 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.608378 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_CN/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.016384 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    54371 2024-01-07 01:59:11.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10936 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:03.608378 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_Hans/
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.016384 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    53657 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10937 2024-01-07 00:48:16.000000 pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.020384 pygubu-designer-0.38/src/pygubudesigner/data/ui/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12950 2023-08-21 23:59:06.000000 pygubu-designer-0.38/src/pygubudesigner/data/ui/about_dialog.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     6320 2023-08-21 23:59:06.000000 pygubu-designer-0.38/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10318 2023-08-21 23:59:06.000000 pygubu-designer-0.38/src/pygubudesigner/data/ui/container_layout_editor_base.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    32924 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/data/ui/preferences_dialog.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    84867 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/data/ui/pygubu-ui.ui
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2525 2022-08-13 05:04:19.000000 pygubu-designer-0.38/src/pygubudesigner/dialogs.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2122 2022-09-04 22:12:41.000000 pygubu-designer-0.38/src/pygubudesigner/i18n.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     8470 2022-08-14 21:43:22.000000 pygubu-designer-0.38/src/pygubudesigner/layouteditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2688 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/logpanel.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    33160 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/main.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12425 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/preferences.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.024384 pygubu-designer-0.38/src/pygubudesigner/preview/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)       63 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/preview/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2664 2023-06-24 22:24:14.000000 pygubu-designer-0.38/src/pygubudesigner/preview/builder.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    12465 2023-01-12 04:27:05.000000 pygubu-designer-0.38/src/pygubudesigner/preview/helper.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    16592 2023-01-22 03:21:37.000000 pygubu-designer-0.38/src/pygubudesigner/preview/preview.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.028385 pygubu-designer-0.38/src/pygubudesigner/properties/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      346 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/properties/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1866 2022-11-04 03:45:23.000000 pygubu-designer-0.38/src/pygubudesigner/properties/manager.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    50467 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/properties/predefined.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    31209 2022-12-10 03:26:32.000000 pygubu-designer-0.38/src/pygubudesigner/properties/propertieshelp.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5461 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/propertieseditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1915 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/rfilemanager.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5726 2023-06-03 02:35:17.000000 pygubu-designer-0.38/src/pygubudesigner/stylehandler.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    52147 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/uitreeeditor.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.032384 pygubu-designer-0.38/src/pygubudesigner/util/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5417 2023-03-02 04:18:11.000000 pygubu-designer-0.38/src/pygubudesigner/util/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     4297 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/util/gridcalculator.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1964 2022-08-14 23:43:51.000000 pygubu-designer-0.38/src/pygubudesigner/util/keyboard.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1175 2022-08-31 01:01:59.000000 pygubu-designer-0.38/src/pygubudesigner/util/observable.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1289 2023-06-08 01:20:38.000000 pygubu-designer-0.38/src/pygubudesigner/util/screens.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2798 2022-08-14 23:34:19.000000 pygubu-designer-0.38/src/pygubudesigner/util/selecttool.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     7402 2022-11-04 03:45:24.000000 pygubu-designer-0.38/src/pygubudesigner/widgetdescr.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.044385 pygubu-designer-0.38/src/pygubudesigner/widgets/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1048 2022-09-01 03:11:46.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/__init__.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3063 2023-03-18 00:51:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/bindingeditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3502 2022-08-15 00:27:55.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/colorentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5327 2023-01-11 23:55:19.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/commandentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3943 2023-06-03 02:35:17.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/componentpalette.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5088 2022-08-15 00:07:57.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/containerlayouteditorbase.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     1640 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/cursorentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2681 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/dimensionentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2282 2023-04-23 01:58:21.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/dynamicpropeditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5164 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     8250 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/fontentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    10193 2023-01-18 04:05:01.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/gridselector.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2491 2022-08-14 23:59:02.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/imageentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3046 2023-01-11 23:55:19.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/namedideditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2102 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/pixelcoordinateentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)    11817 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/propertyeditor.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3059 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/relativeentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5174 2022-11-30 02:32:48.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/stickyentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     3255 2023-01-12 05:16:08.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/tkvarentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     5825 2024-02-11 06:08:43.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/toolbarframe.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2488 2022-08-14 21:43:23.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/ttkstyleentry.py
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)     2536 2022-08-13 03:36:28.000000 pygubu-designer-0.38/src/pygubudesigner/widgets/whentry.py
-drwxr-xr-x   0 ministerio  (1000) ministerio  (1000)        0 2024-02-11 06:11:04.044385 pygubu-designer-0.38/tests/
--rw-r--r--   0 ministerio  (1000) ministerio  (1000)      562 2023-06-24 22:22:22.000000 pygubu-designer-0.38/tests/test_plugin_init.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.911082 pygubu_designer-0.39/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       67 2023-09-09 20:40:32.000000 pygubu_designer-0.39/AUTHORS
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5128 2023-09-09 20:40:32.000000 pygubu_designer-0.39/LEEME.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    35064 2023-09-09 20:40:32.000000 pygubu_designer-0.39/LICENSE.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2023-09-09 20:40:32.000000 pygubu_designer-0.39/LISEZMOI.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      248 2023-09-09 20:40:32.000000 pygubu_designer-0.39/MANIFEST.in
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7697 2024-04-17 00:46:57.911082 pygubu_designer-0.39/PKG-INFO
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5007 2023-09-09 20:40:32.000000 pygubu_designer-0.39/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.787082 pygubu_designer-0.39/development/
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6434 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/create-imgs.py
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6817 2024-03-17 20:08:13.000000 pygubu_designer-0.39/development/dev-notes.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2186 2024-04-08 04:51:29.000000 pygubu_designer-0.39/development/devtool.py
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     3885 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/devtool.sh
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.787082 pygubu_designer-0.39/development/gettext/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1037 2024-04-09 23:44:02.000000 pygubu_designer-0.39/development/gettext/pygubu.its
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2024-04-09 23:44:02.000000 pygubu_designer-0.39/development/gettext/pygubu.loc
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.791082 pygubu_designer-0.39/development/new-designer-icons/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2780 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/main.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.799082 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2129 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7010 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3744 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4072 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2101 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9271 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1252 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      665 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3834 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1552 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6047 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1142 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5074 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1666 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6735 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2133 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8598 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      962 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3043 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1060 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3693 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      797 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      782 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3238 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1077 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5356 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/rect848.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1786 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8481 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1126 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6381 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      867 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3229 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1068 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5481 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      935 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4893 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2489 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7036 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4315 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/template.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7552 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/testnewicons.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/testnewiconsapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.799082 pygubu_designer-0.39/development/pygubuLogo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5501 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/Python-logo-notext.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu .ico
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   101863 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.icns
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.ico
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   175900 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.xcf
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   124131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/pyGubu_newLogo.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       92 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/rootOfSVGs.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10232 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/tcl-tk.svg
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubudesigner_.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       11 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/requirements.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/01_counter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/01_counter/counter.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      798 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/01_counter/counterapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/02_temperature_converter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2687 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconv.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1648 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconvapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/03_flight_Booker/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2648 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/03_flight_Booker/flight_booker.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3212 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/03_flight_Booker/flightbookerapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/04_timer/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4089 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/04_timer/timer.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1777 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/04_timer/timerapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      347 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      546 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/binding.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      960 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/button_cb.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2053 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/button_cb.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.775082 pygubu_designer-0.39/examples/canvas/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      106 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5196 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5211 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      842 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas_example.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/command_properties/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1221 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/command_properties/command_properties.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2641 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/command_properties/command_properties.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/command_properties/command_properties2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3116 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/commands.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    18575 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/commands.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/control_variables/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      584 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/control_variables/controlvariables.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3634 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/control_variables/controlvariables.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/custom_widget/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      436 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1311 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timer_main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      515 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timerapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      287 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timerappwidgets.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2363 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timewidget.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/customtkinter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      174 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/customtkinter/complex/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    22578 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/complex/complex_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2365 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/complex/complexdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/customtkinter/simple/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6284 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/simple/simple_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1269 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/simple/simpledemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/dialogs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       51 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/dialogs/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo1/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo1/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5699 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo1/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/dialogs/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       95 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo2/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo2/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4523 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo2/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/dialogs/demo3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       98 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo3/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4883 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo3/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9704 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo3/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/dialogs/demo4/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      314 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/dialogs/demo4/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3373 2023-09-30 23:40:25.000000 pygubu_designer-0.39/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6987 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/settingsdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/settingsdemoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/settingsdialog.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1471 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/example_grid_rc.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1631 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/example_grid_rc_2.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/forms/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/forms/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1939 2024-04-13 02:37:32.000000 pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2087 2024-02-04 03:08:22.000000 pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1156 2024-02-14 15:19:49.000000 pygubu_designer-0.39/examples/forms/__pycache__/project_styles.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12310 2024-04-13 02:36:09.000000 pygubu_designer-0.39/examples/forms/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1635 2024-04-13 02:37:16.000000 pygubu_designer-0.39/examples/forms/formsdemo1app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      796 2024-04-14 01:37:57.000000 pygubu_designer-0.39/examples/forms/formsdemo1appui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      635 2024-02-25 22:14:08.000000 pygubu_designer-0.39/examples/forms/project_styles.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      723 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/framepad.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/helloworld/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       82 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      740 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/helloworld.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/helloworld.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/holamundo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1176 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/holamundo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2303 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1237 2024-02-13 03:45:58.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11576 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/demo-i18n.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1251 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/i18n.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1433 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/demoapp.pot
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.775082 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/image_property/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      710 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/image_property.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1682 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/image_property.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/red.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/yellow.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/integration_with_cxFreeze/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      337 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6612 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2529 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_nuitka/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      366 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6510 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/myapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_py2exe/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      258 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2731 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_pyinstaller/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2513 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.spec
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      582 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1141 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      526 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      317 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1750 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      547 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      644 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2190 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1975 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_zipapp/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      365 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.779082 pygubu_designer-0.39/examples/integration_with_zipapp/src/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/__init__.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3445 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/extradata/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      320 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      556 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/info.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/red.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1013 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/main.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/jpg_image_on_canvas/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      825 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1244 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       14 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    38211 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/seaside400.jpg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3187 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/menubutton.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1347 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/menuexample.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/notebook/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/notebook/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/notebook/demo1app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1835 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/panedwindow.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/panes_and_notebooks.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/pathchooserdemo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       32 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/pathchooserdemo/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1897 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3220 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/pathchooserdemo/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2644 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1840 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrollbarhelper.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/scrolledframe/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/scrolledframe/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      646 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/scrolledframe/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12412 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/scrolledframe/scrolledframe_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10765 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledframe-layouts.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9388 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledframe.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/scrolledtext/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4030 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledtext/scrolledtext_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      977 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledtext/scrolledtextdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/static_image/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      539 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1676 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/demoapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23336 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/logo_253.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/requirements.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.779082 pygubu_designer-0.39/examples/text/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/text/logwindowdemo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3075 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/text/logwindowdemo/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1714 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/text/logwindowdemo/demo1app.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/tk_window/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      144 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1354 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/tkdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      600 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/tkdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/toplevel_centered/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      154 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1216 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/centered_demo1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1317 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/centered_demo2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1020 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/toplevel_menu/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_menu/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1291 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_menu/menu.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2470 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_menu/menu.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       43 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo1/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1496 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo1/treeview.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3473 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo1/treeview.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo2/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23736 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo2/columns_stretching.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2712 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo2/columnsstretchingdemo.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_editable/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       28 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_editable/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5044 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7875 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_editable/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5944 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo2/demo2.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3432 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo2/demo2app.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_filterable/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       30 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_filterable/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5404 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_filterable/demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2886 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_filterable/demoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/user_input/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    28967 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/userinput.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3730 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/userinputapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      883 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/variables.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4346 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/vscrolledframe.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/windowdeleteevent/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      887 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1122 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      847 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1271 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo2.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    88292 2024-04-10 03:51:03.000000 pygubu_designer-0.39/pygubu-designer.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2434 2024-04-11 02:30:33.000000 pygubu_designer-0.39/pyproject.toml
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       38 2024-04-17 00:46:57.911082 pygubu_designer-0.39/setup.cfg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.779082 pygubu_designer-0.39/src/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.907082 pygubu_designer-0.39/src/pygubu_designer.egg-info/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7697 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/PKG-INFO
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    36901 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/SOURCES.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        1 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/dependency_links.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       65 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/entry_points.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      443 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/requires.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       15 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/top_level.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.839082 pygubu_designer-0.39/src/pygubudesigner/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      198 2024-04-11 02:29:26.000000 pygubu_designer-0.39/src/pygubudesigner/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      122 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/__main__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1049 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/actions.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6373 2024-03-12 19:01:57.000000 pygubu_designer-0.39/src/pygubudesigner/bindingseditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.839082 pygubu_designer-0.39/src/pygubudesigner/codegen/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       76 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/codegen/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    19333 2024-04-08 01:37:06.000000 pygubu_designer-0.39/src/pygubudesigner/codegen/codebuilder.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12276 2024-04-08 02:05:57.000000 pygubu_designer-0.39/src/pygubudesigner/codegen/scriptgenerator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11044 2024-03-12 19:01:57.000000 pygubu_designer-0.39/src/pygubudesigner/containerlayouteditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.843082 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2992 2024-03-13 03:14:18.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/app.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2024-03-13 03:28:33.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/appuser.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      453 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/base.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1620 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/customstyles.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2116 2024-04-08 02:11:56.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/script.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      474 2024-04-12 03:50:58.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/scriptuser.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      771 2024-04-08 02:22:55.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widget.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      542 2024-03-06 04:13:52.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widgetbo.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      655 2024-04-12 03:59:49.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widgetuser.py.mako
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/images/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.843082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       70 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       71 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/bin-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       85 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/close.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/download3-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/download3-32.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      230 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/mglass.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/property_invalid.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      875 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4897 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu200.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.859082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      352 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      128 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      224 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      231 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       75 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1120 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      126 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      100 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      109 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.871082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      132 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      599 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      195 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      114 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      142 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.871082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      592 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      567 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      357 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      572 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.871082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      194 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/arrow-left2.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      184 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/arrow-right2.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      162 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/bin-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      353 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/circle-left.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      333 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/circle-right.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      170 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/download3-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      214 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/download3-32.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      316 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/mglass.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      603 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/property_invalid.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4777 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    15896 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu200.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.883082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1088 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      527 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      433 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      325 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      435 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      545 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      293 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.891082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      689 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      202 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      323 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      116 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      175 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      705 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      619 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      611 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      673 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3172 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      425 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13114 2024-04-14 23:23:45.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2024-04-14 23:23:45.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    58684 2024-04-14 23:23:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu-designer.pot
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    20171 2024-04-14 23:23:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu.pot
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4815 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      393 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    53166 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10936 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    52658 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10937 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/data/ui/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13872 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/about_dialog.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6320 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10318 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/container_layout_editor_base.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    16121 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/designer_settings.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4093 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/messagebox.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    45719 2024-04-12 04:11:16.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/project_settings.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    49126 2024-04-12 03:11:36.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/pygubu-ui.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/treecomponent_palette.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4326 2024-04-15 03:30:30.000000 pygubu_designer-0.39/src/pygubudesigner/designerstyles.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2525 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/dialogs.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2122 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/i18n.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8476 2024-03-19 19:06:18.000000 pygubu_designer-0.39/src/pygubudesigner/layouteditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2688 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/logpanel.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    33479 2024-04-13 01:47:41.000000 pygubu_designer-0.39/src/pygubudesigner/main.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4418 2024-04-06 02:39:05.000000 pygubu_designer-0.39/src/pygubudesigner/preferences.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/preview/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       63 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/preview/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2664 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/preview/builder.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13624 2024-04-02 02:28:06.000000 pygubu_designer-0.39/src/pygubudesigner/preview/helper.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    17119 2024-04-01 04:38:44.000000 pygubu_designer-0.39/src/pygubudesigner/preview/preview.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/properties/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      373 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/properties/__init__.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/properties/editors/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/properties/editors/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1027 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/properties/editors/forms.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1866 2024-02-17 03:46:34.000000 pygubu_designer-0.39/src/pygubudesigner/properties/manager.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    50538 2024-04-11 03:47:20.000000 pygubu_designer-0.39/src/pygubudesigner/properties/predefined.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    31209 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/properties/propertieshelp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5528 2024-04-14 01:38:41.000000 pygubu_designer-0.39/src/pygubudesigner/propertieseditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1915 2024-04-07 01:08:23.000000 pygubu_designer-0.39/src/pygubudesigner/rfilemanager.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/services/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1854 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/aboutdialog.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      982 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/aboutdialogui.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/services/builders/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/builders/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3356 2024-03-31 01:41:21.000000 pygubu_designer-0.39/src/pygubudesigner/services/designersettings.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      931 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/designersettingsui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2733 2024-04-14 22:42:58.000000 pygubu_designer-0.39/src/pygubudesigner/services/fieldvalidator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1945 2024-03-07 01:08:46.000000 pygubu_designer-0.39/src/pygubudesigner/services/messagebox.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      843 2024-03-07 01:11:22.000000 pygubu_designer-0.39/src/pygubudesigner/services/messageboxui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4224 2024-04-13 02:03:46.000000 pygubu_designer-0.39/src/pygubudesigner/services/project.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12314 2024-04-14 23:23:05.000000 pygubu_designer-0.39/src/pygubudesigner/services/projectsettings.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1821 2024-04-12 04:13:44.000000 pygubu_designer-0.39/src/pygubudesigner/services/projectsettingsui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6301 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/stylehandler.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4220 2024-03-31 23:43:45.000000 pygubu_designer-0.39/src/pygubudesigner/services/theming.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/services/widgets/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5799 2024-04-08 02:37:37.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpalette.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      450 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpalettebo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3465 2024-04-08 03:06:36.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpaletteui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    59265 2024-04-14 01:49:08.000000 pygubu_designer-0.39/src/pygubudesigner/uitreeeditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/util/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2823 2024-04-01 01:31:03.000000 pygubu_designer-0.39/src/pygubudesigner/util/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4297 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/gridcalculator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1964 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/keyboard.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1175 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/observable.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1289 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/screens.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2798 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/selecttool.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8344 2024-04-14 01:38:14.000000 pygubu_designer-0.39/src/pygubudesigner/widgetdescr.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.907082 pygubu_designer-0.39/src/pygubudesigner/widgets/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3063 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/bindingeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3502 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/colorentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5327 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/commandentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3943 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/componentpalette.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5088 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/containerlayouteditorbase.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1640 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/cursorentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2681 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/dimensionentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2282 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/dynamicpropeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8250 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/fontentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10193 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/gridselector.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2491 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/imageentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3046 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/namedideditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2102 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/pixelcoordinateentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11940 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/propertyeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3059 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/relativeentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5174 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/stickyentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3255 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/tkvarentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5936 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/toolbarframe.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2650 2024-04-02 02:52:39.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/ttkstyleentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2536 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/whentry.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.907082 pygubu_designer-0.39/tests/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      562 2023-09-09 20:40:32.000000 pygubu_designer-0.39/tests/test_plugin_init.py
```

### Comparing `pygubu-designer-0.38/LEEME.md` & `pygubu_designer-0.39/LEEME.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/LICENSE.md` & `pygubu_designer-0.39/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/LISEZMOI.md` & `pygubu_designer-0.39/LISEZMOI.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/PKG-INFO` & `pygubu_designer-0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.38
+Version: 0.39
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
@@ -27,15 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 Requires-Dist: appdirs>=1.4.3
 Requires-Dist: Mako>=1.1.4
 Requires-Dist: screeninfo>=0.8
 Requires-Dist: autopep8>=1.7
-Requires-Dist: pygubu>=0.33
+Requires-Dist: pygubu>=0.35
 Provides-Extra: ttkwidgets
 Requires-Dist: ttkwidgets; extra == "ttkwidgets"
 Provides-Extra: tksheet
 Requires-Dist: tksheet; extra == "tksheet"
 Provides-Extra: tkinterweb
 Requires-Dist: tkinterweb; extra == "tkinterweb"
 Provides-Extra: tkintertable
```

### Comparing `pygubu-designer-0.38/README.md` & `pygubu_designer-0.39/README.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/create-imgs.py` & `pygubu_designer-0.39/development/create-imgs.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/dev-notes.txt` & `pygubu_designer-0.39/development/dev-notes.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 alejandroautalan/pygubu-designer#99
 
 pip install git+https://github.com/alejandroautalan/pygubu git+https://github.com/alejandroautalan/pygubu-designer
 
 
 TODO
 ====
+- BUG: create a pygubu dialog and generate code. Incorrect class hint generated
+  self.mainwindow: pygubu.builder.widgets.dialog = builder.get_object(
+            "settingsdialog", master)
 - Issue: redraw previews on theme change.
-- ttkstyles branch: add optiondb_initializer=None to builder and codebuilder.
-  or name it on_first_widget_cb. Function that will execute only once after
-  the first widget is created, generally the root widget.
 - Customtkinter 5 Issues on designer:
   Can't select SegmentedButton in Preview (can't click it)
   Click on tabview tab does not select tab in treeview.
-  F5 preview of CTk does not show images and shows warning when the
-  preview closes. This is because Ctk is another tk instance running on
-  another thread.
 - Add a mechanism to test code generation.
 - Treeview with scrollHelper. Srollbars are not shown depending on the
   treeview configuration or if columns are set stretch=true
   Investigate the behaviour.
 - FIX: Create a frame frame1, create a frame2 inside, then add a button.
   Create another frame frame3 sibling of frame1, copy frame2 and paste in
   frame3, the content of frame 2 is duplicated in frame3.
@@ -70,42 +67,34 @@
 - Add widget for CanvasPlus
 - Add support to tkinterpp?
 - ADD designer plugin with sun valley ttk theme ?
 - Add button bar. Example: layout section with buttons that will modify
   a group of properties. Example button "Expand": for pack manager will set
   expand=True, fill=both.
 
+- Add notebook, add tab,  add label to tab.
+  Should be displayed on center, y no tab sticky option is set.
+  Problem seems to be, the labels is ejecuting his layout configuration. Should not.
+  Solution 1: add manager type "none" or "parent". If manager of widget is none, the
+    parent widget is in charge of layout configuration.
 
 
 Button Bar
 ==========
 
-New Project, Open Project, Save, UndoButtons, Cut, copy, paste, delete,
-Generate code (generate files in disk, with configured names),
-Buttons for Actions on current layout Manager:
-  Align left, center, Align right, Expand.
-  
+Section: New, Open, Save, Save As
+Section: Cut, copy, paste, delete, UndoButtons?
+Section: Align left, center, Align right, Expand # Buttons for Actions on current layout Manager
+Section: Preview refresh
+Section: Project Properties, Generate code
+
 Example: Click Expand
   Manager Place: set expand=True, fill=both
 
 
-
-
-Project Notes:
-=============
-
-Posible project properties:
-
-name: Project Name
-path: Path to save generated files? Defaults to . (dot), same path as project.
-relative_path: use relative path for external files (eg image files)
-
-
-
-
 Theming notes:
 =============
 
 resources
   - image (name, filename, format, data)
   - named font
   - OptionDatabaseGroup
```

### Comparing `pygubu-designer-0.38/development/devtool.py` & `pygubu_designer-0.39/development/devtool.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/devtool.sh` & `pygubu_designer-0.39/development/devtool.sh`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/main.py` & `pygubu_designer-0.39/development/new-designer-icons/main.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/button.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/button.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/canvas.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/canvas.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/combobox.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/combobox.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/default.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/default.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/entry.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/entry.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/frame.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/frame.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/label.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/label.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/labelframe.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/labelframe.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/menubutton.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/menubutton.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook-tab.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook-tab.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/notebook.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/pannedwindow.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/progressbar.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/progressbar.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/spinbutton.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/spinbutton.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/textview.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/textview.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/toplevel.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/toplevel.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview-col.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview-col.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/treeview.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/viewport.png` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/pygubu-icons/viewport.svg` & `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/template.svg` & `pygubu_designer-0.39/development/new-designer-icons/template.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/testnewicons.ui` & `pygubu_designer-0.39/development/new-designer-icons/testnewicons.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/new-designer-icons/testnewiconsapp.py` & `pygubu_designer-0.39/development/new-designer-icons/testnewiconsapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/Python-logo-notext.svg` & `pygubu_designer-0.39/development/pygubuLogo/Python-logo-notext.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/logo_pygubu .ico` & `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu .ico`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/logo_pygubu.icns` & `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.icns`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/logo_pygubu.ico` & `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.ico`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/logo_pygubu.xcf` & `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.xcf`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/pyGubu_newLogo.svg` & `pygubu_designer-0.39/development/pygubuLogo/pyGubu_newLogo.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubuLogo/tcl-tk.svg` & `pygubu_designer-0.39/development/pygubuLogo/tcl-tk.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/development/pygubudesigner_.py` & `pygubu_designer-0.39/development/pygubudesigner_.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/01_counter/counter.ui` & `pygubu_designer-0.39/examples/7guis/01_counter/counter.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/01_counter/counterapp.py` & `pygubu_designer-0.39/examples/7guis/01_counter/counterapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/02_temperature_converter/tempconv.ui` & `pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconv.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/02_temperature_converter/tempconvapp.py` & `pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconvapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/03_flight_Booker/flight_booker.ui` & `pygubu_designer-0.39/examples/7guis/03_flight_Booker/flight_booker.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/03_flight_Booker/flightbookerapp.py` & `pygubu_designer-0.39/examples/7guis/03_flight_Booker/flightbookerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/04_timer/timer.ui` & `pygubu_designer-0.39/examples/7guis/04_timer/timer.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/7guis/04_timer/timerapp.py` & `pygubu_designer-0.39/examples/7guis/04_timer/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/binding.ui` & `pygubu_designer-0.39/examples/binding.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/button_cb.py` & `pygubu_designer-0.39/examples/button_cb.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/button_cb.ui` & `pygubu_designer-0.39/examples/button_cb.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/canvas/canvas-scrollregion/myapp.py` & `pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/canvas/canvas-scrollregion/myapp.ui` & `pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/canvas_example.ui` & `pygubu_designer-0.39/examples/canvas_example.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/command_properties/command_properties.py` & `pygubu_designer-0.39/examples/command_properties/command_properties.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/command_properties/command_properties.ui` & `pygubu_designer-0.39/examples/command_properties/command_properties.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/command_properties/command_properties2.py` & `pygubu_designer-0.39/examples/command_properties/command_properties2.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/commands.py` & `pygubu_designer-0.39/examples/commands.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/commands.ui` & `pygubu_designer-0.39/examples/commands.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/control_variables/controlvariables.py` & `pygubu_designer-0.39/examples/control_variables/controlvariables.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/control_variables/controlvariables.ui` & `pygubu_designer-0.39/examples/control_variables/controlvariables.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/custom_widget/timer_main.ui` & `pygubu_designer-0.39/examples/custom_widget/timer_main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/custom_widget/timerapp.py` & `pygubu_designer-0.39/examples/custom_widget/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/custom_widget/timewidget.py` & `pygubu_designer-0.39/examples/custom_widget/timewidget.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/customtkinter/complex/complex_demo.ui` & `pygubu_designer-0.39/examples/customtkinter/complex/complex_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/customtkinter/complex/complexdemoapp.py` & `pygubu_designer-0.39/examples/customtkinter/complex/complexdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/customtkinter/simple/simple_demo.ui` & `pygubu_designer-0.39/examples/customtkinter/simple/simple_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/customtkinter/simple/simpledemoapp.py` & `pygubu_designer-0.39/examples/customtkinter/simple/simpledemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo1/demo.py` & `pygubu_designer-0.39/examples/dialogs/demo1/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo1/demo.ui` & `pygubu_designer-0.39/examples/dialogs/demo1/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo2/demo.py` & `pygubu_designer-0.39/examples/dialogs/demo2/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo2/demo.ui` & `pygubu_designer-0.39/examples/dialogs/demo2/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo3/demo.py` & `pygubu_designer-0.39/examples/dialogs/demo3/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo3/demo.ui` & `pygubu_designer-0.39/examples/dialogs/demo3/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo4/settingsdemo.ui` & `pygubu_designer-0.39/examples/dialogs/demo4/settingsdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo4/settingsdemoapp.py` & `pygubu_designer-0.39/examples/dialogs/demo4/settingsdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/dialogs/demo4/settingsdialog.py` & `pygubu_designer-0.39/examples/dialogs/demo4/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/example_grid_rc.ui` & `pygubu_designer-0.39/examples/example_grid_rc.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/example_grid_rc_2.ui` & `pygubu_designer-0.39/examples/example_grid_rc_2.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc` & `pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,265 +1,261 @@
 magic:    0xa70d0d0a
-moddate:  0x54059a65 (Sun Jan  7 01:58:44 2024 UTC)
-files sz: 680
+moddate:  0x99ef1966 (Sat Apr 13 02:36:09 2024 UTC)
+files sz: 800
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01020065006a020000000000
-      0000006503a6010000ab0100000000000000006a0400000000000000005a
-      05650564027a0b00005a0602004700640384006404a6020000ab02000000
-      00000000005a07650864056b0200000000722002006507a6000000ab0000
-      000000000000005a096509a00a0000000000000000000000000000000000
-      000000a6000000ab00000000000000000001006401530064015300
+      0x9700640064016c005a00640064016c015a02640064016c035a03020065
+      006a0400000000000000006505a6010000ab0100000000000000006a0600
+      000000000000005a07650764027a0b00005a08650767015a090200470064
+      0384006404a6020000ab0200000000000000005a0a650b64056b02000000
+      0072200200650aa6000000ab0000000000000000005a0c650ca00d000000
+      0000000000000000000000000000000000a6000000ab0000000000000000
+      0001006401530064015300
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (pathlib)
                  8 STORE_NAME               0 (pathlib)
    
      3          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (pygubu)
-                16 STORE_NAME               1 (pygubu)
+                14 IMPORT_NAME              1 (tkinter)
+                16 STORE_NAME               2 (tk)
    
-     5          18 PUSH_NULL
-                20 LOAD_NAME                0 (pathlib)
-                22 LOAD_ATTR                2 (Path)
-                32 LOAD_NAME                3 (__file__)
-                34 PRECALL                  1
-                38 CALL                     1
-                48 LOAD_ATTR                4 (parent)
-                58 STORE_NAME               5 (PROJECT_PATH)
-   
-     6          60 LOAD_NAME                5 (PROJECT_PATH)
-                62 LOAD_CONST               2 ('demo1.ui')
-                64 BINARY_OP               11 (/)
-                68 STORE_NAME               6 (PROJECT_UI)
-   
-     9          70 PUSH_NULL
-                72 LOAD_BUILD_CLASS
-                74 LOAD_CONST               3 (<code object FormsDemo1Base, file "/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py", line 9>)
-                76 MAKE_FUNCTION            0
-                78 LOAD_CONST               4 ('FormsDemo1Base')
-                80 PRECALL                  2
-                84 CALL                     2
-                94 STORE_NAME               7 (FormsDemo1Base)
-   
-    28          96 LOAD_NAME                8 (__name__)
-                98 LOAD_CONST               5 ('__main__')
-               100 COMPARE_OP               2 (==)
-               106 POP_JUMP_FORWARD_IF_FALSE    32 (to 172)
-   
-    29         108 PUSH_NULL
-               110 LOAD_NAME                7 (FormsDemo1Base)
-               112 PRECALL                  0
-               116 CALL                     0
-               126 STORE_NAME               9 (app)
-   
-    30         128 LOAD_NAME                9 (app)
-               130 LOAD_METHOD             10 (run)
-               152 PRECALL                  0
-               156 CALL                     0
-               166 POP_TOP
-               168 LOAD_CONST               1 (None)
-               170 RETURN_VALUE
+     4          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               1 (None)
+                22 IMPORT_NAME              3 (pygubu)
+                24 STORE_NAME               3 (pygubu)
    
-    28     >>  172 LOAD_CONST               1 (None)
-               174 RETURN_VALUE
+     6          26 PUSH_NULL
+                28 LOAD_NAME                0 (pathlib)
+                30 LOAD_ATTR                4 (Path)
+                40 LOAD_NAME                5 (__file__)
+                42 PRECALL                  1
+                46 CALL                     1
+                56 LOAD_ATTR                6 (parent)
+                66 STORE_NAME               7 (PROJECT_PATH)
+   
+     7          68 LOAD_NAME                7 (PROJECT_PATH)
+                70 LOAD_CONST               2 ('demo1.ui')
+                72 BINARY_OP               11 (/)
+                76 STORE_NAME               8 (PROJECT_UI)
+   
+     8          78 LOAD_NAME                7 (PROJECT_PATH)
+                80 BUILD_LIST               1
+                82 STORE_NAME               9 (RESOURCE_PATHS)
+   
+    11          84 PUSH_NULL
+                86 LOAD_BUILD_CLASS
+                88 LOAD_CONST               3 (<code object FormsDemo1AppUI, file "/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py", line 11>)
+                90 MAKE_FUNCTION            0
+                92 LOAD_CONST               4 ('FormsDemo1AppUI')
+                94 PRECALL                  2
+                98 CALL                     2
+               108 STORE_NAME              10 (FormsDemo1AppUI)
+   
+    29         110 LOAD_NAME               11 (__name__)
+               112 LOAD_CONST               5 ('__main__')
+               114 COMPARE_OP               2 (==)
+               120 POP_JUMP_FORWARD_IF_FALSE    32 (to 186)
+   
+    30         122 PUSH_NULL
+               124 LOAD_NAME               10 (FormsDemo1AppUI)
+               126 PRECALL                  0
+               130 CALL                     0
+               140 STORE_NAME              12 (app)
+   
+    31         142 LOAD_NAME               12 (app)
+               144 LOAD_METHOD             13 (run)
+               166 PRECALL                  0
+               170 CALL                     0
+               180 POP_TOP
+               182 LOAD_CONST               1 (None)
+               184 RETURN_VALUE
+   
+    29     >>  186 LOAD_CONST               1 (None)
+               188 RETURN_VALUE
    consts
       0
       None
       'demo1.ui'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
-            0x970065005a0164005a026406640284015a03640384005a04640484005a
-            05640584005a0664015300
-           9           0 RESUME                   0
+            0x970065005a0164005a026405640284015a03640384005a04640484005a
+            0564015300
+          11           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('FormsDemo1Base')
+                       6 LOAD_CONST               0 ('FormsDemo1AppUI')
                        8 STORE_NAME               2 (__qualname__)
          
-          10          10 LOAD_CONST               6 ((None,))
-                      12 LOAD_CONST               2 (<code object __init__, file "/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py", line 10>)
+          12          10 LOAD_CONST               5 ((None, None))
+                      12 LOAD_CONST               2 (<code object __init__, file "/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py", line 12>)
                       14 MAKE_FUNCTION            1 (defaults)
                       16 STORE_NAME               3 (__init__)
          
-          18          18 LOAD_CONST               3 (<code object run, file "/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py", line 18>)
+          22          18 LOAD_CONST               3 (<code object run, file "/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py", line 22>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               4 (run)
          
-          21          24 LOAD_CONST               4 (<code object on_check_changed, file "/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py", line 21>)
+          25          24 LOAD_CONST               4 (<code object on_submit_clicked, file "/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py", line 25>)
                       26 MAKE_FUNCTION            0
-                      28 STORE_NAME               5 (on_check_changed)
-         
-          24          30 LOAD_CONST               5 (<code object on_submit_clicked, file "/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py", line 24>)
-                      32 MAKE_FUNCTION            0
-                      34 STORE_NAME               6 (on_submit_clicked)
-                      36 LOAD_CONST               1 (None)
-                      38 RETURN_VALUE
+                      28 STORE_NAME               5 (on_submit_clicked)
+                      30 LOAD_CONST               1 (None)
+                      32 RETURN_VALUE
          consts
-            'FormsDemo1Base'
+            'FormsDemo1AppUI'
             None
             code
-               argcount  : 2
+               argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
-                  0x97007401000000000000000000006a010000000000000000a6000000ab
-                  00000000000000000078017c005f0200000000000000007d027c02a00300
-                  000000000000000000000000000000000000007408000000000000000000
-                  00a6010000ab01000000000000000001007c02a005000000000000000000
-                  0000000000000000000000740c00000000000000000000a6010000ab0100
-                  0000000000000001007c02a0070000000000000000000000000000000000
-                  00000064017c01a6020000ab0200000000000000007c005f080000000000
-                  0000007c02a00900000000000000000000000000000000000000007c00a6
-                  010000ab010000000000000000010064005300
-                10           0 RESUME                   0
+                  0x97007401000000000000000000006a0100000000000000007c02ac01a6
+                  010000ab0100000000000000007c005f0200000000000000007c006a0200
+                  00000000000000a003000000000000000000000000000000000000000074
+                  0800000000000000000000a6010000ab01000000000000000001007c006a
+                  020000000000000000a00500000000000000000000000000000000000000
+                  00740c00000000000000000000a6010000ab01000000000000000001007c
+                  006a020000000000000000a0070000000000000000000000000000000000
+                  00000064027c01a6020000ab0200000000000000007c005f080000000000
+                  0000007c006a020000000000000000a00900000000000000000000000000
+                  000000000000007c00a6010000ab010000000000000000010064005300
+                12           0 RESUME                   0
                
-                11           2 LOAD_GLOBAL              1 (NULL + pygubu)
+                13           2 LOAD_GLOBAL              1 (NULL + pygubu)
                             14 LOAD_ATTR                1 (Builder)
-                            24 PRECALL                  0
-                            28 CALL                     0
-                            38 COPY                     1
-                            40 LOAD_FAST                0 (self)
-                            42 STORE_ATTR               2 (builder)
-                            52 STORE_FAST               2 (builder)
-               
-                12          54 LOAD_FAST                2 (builder)
-                            56 LOAD_METHOD              3 (add_resource_path)
-                            78 LOAD_GLOBAL              8 (PROJECT_PATH)
-                            90 PRECALL                  1
-                            94 CALL                     1
-                           104 POP_TOP
-               
-                13         106 LOAD_FAST                2 (builder)
-                           108 LOAD_METHOD              5 (add_from_file)
-                           130 LOAD_GLOBAL             12 (PROJECT_UI)
-                           142 PRECALL                  1
-                           146 CALL                     1
-                           156 POP_TOP
-               
-                15         158 LOAD_FAST                2 (builder)
-                           160 LOAD_METHOD              7 (get_object)
-                           182 LOAD_CONST               1 ('toplevel1')
-                           184 LOAD_FAST                1 (master)
-                           186 PRECALL                  2
-                           190 CALL                     2
-                           200 LOAD_FAST                0 (self)
-                           202 STORE_ATTR               8 (mainwindow)
-               
-                16         212 LOAD_FAST                2 (builder)
-                           214 LOAD_METHOD              9 (connect_callbacks)
-                           236 LOAD_FAST                0 (self)
-                           238 PRECALL                  1
-                           242 CALL                     1
-                           252 POP_TOP
-                           254 LOAD_CONST               0 (None)
-                           256 RETURN_VALUE
+               
+                14          24 LOAD_FAST                2 (on_first_object_cb)
+               
+                13          26 KW_NAMES                 1
+                            28 PRECALL                  1
+                            32 CALL                     1
+                            42 LOAD_FAST                0 (self)
+                            44 STORE_ATTR               2 (builder)
+               
+                15          54 LOAD_FAST                0 (self)
+                            56 LOAD_ATTR                2 (builder)
+                            66 LOAD_METHOD              3 (add_resource_paths)
+                            88 LOAD_GLOBAL              8 (RESOURCE_PATHS)
+                           100 PRECALL                  1
+                           104 CALL                     1
+                           114 POP_TOP
+               
+                16         116 LOAD_FAST                0 (self)
+                           118 LOAD_ATTR                2 (builder)
+                           128 LOAD_METHOD              5 (add_from_file)
+                           150 LOAD_GLOBAL             12 (PROJECT_UI)
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 POP_TOP
+               
+                18         178 LOAD_FAST                0 (self)
+                           180 LOAD_ATTR                2 (builder)
+                           190 LOAD_METHOD              7 (get_object)
+               
+                19         212 LOAD_CONST               2 ('toplevel1')
+                           214 LOAD_FAST                1 (master)
+               
+                18         216 PRECALL                  2
+                           220 CALL                     2
+                           230 LOAD_FAST                0 (self)
+                           232 STORE_ATTR               8 (mainwindow)
+               
+                20         242 LOAD_FAST                0 (self)
+                           244 LOAD_ATTR                2 (builder)
+                           254 LOAD_METHOD              9 (connect_callbacks)
+                           276 LOAD_FAST                0 (self)
+                           278 PRECALL                  1
+                           282 CALL                     1
+                           292 POP_TOP
+                           294 LOAD_CONST               0 (None)
+                           296 RETURN_VALUE
                consts
                   None
+                  ('on_first_object',)
                   'toplevel1'
-               names      ('pygubu', 'Builder', 'builder', 'add_resource_path', 'PROJECT_PATH', 'add_from_file', 'PROJECT_UI', 'get_object', 'mainwindow', 'connect_callbacks')
-               varnames   ('self', 'master', 'builder')
+               names      ('pygubu', 'Builder', 'builder', 'add_resource_paths', 'RESOURCE_PATHS', 'add_from_file', 'PROJECT_UI', 'get_object', 'mainwindow', 'connect_callbacks')
+               varnames   ('self', 'master', 'on_first_object_cb')
                freevars   ()
                cellvars   ()
-               filename   '/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py'
+               filename   '/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py'
                name       '__init__'
-               firstlineno 10
-               lnotab 0x02013401340134023601
+               firstlineno 12
+               lnotab 0x0201160102ff1c023e013e02220104ff1a02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300
-                18           0 RESUME                   0
+                22           0 RESUME                   0
                
-                19           2 LOAD_FAST                0 (self)
+                23           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (mainwindow)
                             14 LOAD_METHOD              1 (mainloop)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 POP_TOP
                             52 LOAD_CONST               0 (None)
                             54 RETURN_VALUE
                consts
                   None
                names      ('mainwindow', 'mainloop')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py'
+               filename   '/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py'
                name       'run'
-               firstlineno 18
-               lnotab 0x0201
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 1
-               flags     : 3
-               code 0x970064005300
-                21           0 RESUME                   0
-               
-                22           2 LOAD_CONST               0 (None)
-                             4 RETURN_VALUE
-               consts
-                  None
-               names      ()
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py'
-               name       'on_check_changed'
-               firstlineno 21
+               firstlineno 22
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                24           0 RESUME                   0
+                25           0 RESUME                   0
                
-                25           2 LOAD_CONST               0 (None)
+                26           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py'
+               filename   '/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py'
                name       'on_submit_clicked'
-               firstlineno 24
+               firstlineno 25
                lnotab 0x0201
-            (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'run', 'on_check_changed', 'on_submit_clicked')
+            (None, None)
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'run', 'on_submit_clicked')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py'
-         name       'FormsDemo1Base'
-         firstlineno 9
-         lnotab 0x0a01080806030603
-      'FormsDemo1Base'
+         filename   '/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py'
+         name       'FormsDemo1AppUI'
+         firstlineno 11
+         lnotab 0x0a01080a0603
+      'FormsDemo1AppUI'
       '__main__'
-   names      ('pathlib', 'pygubu', 'Path', '__file__', 'parent', 'PROJECT_PATH', 'PROJECT_UI', 'FormsDemo1Base', '__name__', 'app', 'run')
+   names      ('pathlib', 'tkinter', 'tk', 'pygubu', 'Path', '__file__', 'parent', 'PROJECT_PATH', 'PROJECT_UI', 'RESOURCE_PATHS', 'FormsDemo1AppUI', '__name__', 'app', 'run')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/ministerio/Privado/projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1base.py'
+   filename   '/home/aautalan/Projects/pygubu-project/pygubu-designer/examples/forms/formsdemo1appui.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0202080108022a010a031a130c0114012cfe
+   lnotab 0x00ff02020801080108022a010a0106031a120c0114012cfe
```

### Comparing `pygubu-designer-0.38/examples/framepad.ui` & `pygubu_designer-0.39/examples/framepad.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/helloworld/helloworld.py` & `pygubu_designer-0.39/examples/helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/helloworld/helloworld.ui` & `pygubu_designer-0.39/examples/helloworld/helloworld.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/helloworld/holamundo.py` & `pygubu_designer-0.39/examples/helloworld/holamundo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/helloworld/holamundo.ui` & `pygubu_designer-0.39/examples/helloworld/holamundo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/image_property/green.gif` & `pygubu_designer-0.39/examples/image_property/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/image_property/image_property.py` & `pygubu_designer-0.39/examples/image_property/image_property.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/image_property/image_property.ui` & `pygubu_designer-0.39/examples/image_property/image_property.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/image_property/red.gif` & `pygubu_designer-0.39/examples/image_property/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/image_property/yellow.gif` & `pygubu_designer-0.39/examples/image_property/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_cxFreeze/myapp.py` & `pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_cxFreeze/myapp.ui` & `pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_cxFreeze/setup.py` & `pygubu_designer-0.39/examples/integration_with_cxFreeze/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_nuitka/myapp.py` & `pygubu_designer-0.39/examples/integration_with_nuitka/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_nuitka/myapp.ui` & `pygubu_designer-0.39/examples/integration_with_nuitka/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_py2exe/myapp.py` & `pygubu_designer-0.39/examples/integration_with_py2exe/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_py2exe/myapp.ui` & `pygubu_designer-0.39/examples/integration_with_py2exe/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_py2exe/setup.py` & `pygubu_designer-0.39/examples/integration_with_py2exe/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_pyinstaller/myapp.py` & `pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_pyinstaller/myapp.spec` & `pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.spec`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_pyinstaller/myapp.ui` & `pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/README.md` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/README.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/main.ui` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp1/myapp.py` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/main.ui` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/myapp.py` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/main.ui` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/myapp.py` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py` & `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui` & `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/green.gif` & `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/info.txt` & `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/info.txt`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/red.gif` & `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/data/yellow.gif` & `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/integration_with_zipapp/src/demoapp/main.py` & `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/main.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/jpg_image_on_canvas/demoapp.py` & `pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/jpg_image_on_canvas/demoapp.ui` & `pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/jpg_image_on_canvas/seaside400.jpg` & `pygubu_designer-0.39/examples/jpg_image_on_canvas/seaside400.jpg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/menubutton.ui` & `pygubu_designer-0.39/examples/menubutton.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/menuexample.ui` & `pygubu_designer-0.39/examples/menuexample.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/notebook/demo1.ui` & `pygubu_designer-0.39/examples/notebook/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/notebook/demo1app.py` & `pygubu_designer-0.39/examples/notebook/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/panedwindow.ui` & `pygubu_designer-0.39/examples/panedwindow.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/panes_and_notebooks.ui` & `pygubu_designer-0.39/examples/panes_and_notebooks.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/pathchooserdemo/demo1/pathchooserdemo.py` & `pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/pathchooserdemo/demo1/pathchooserdemo.ui` & `pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/pathchooserdemo/demo2/pathchooserdemo.py` & `pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/pathchooserdemo/demo2/pathchooserdemo.ui` & `pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/scrollbarhelper.ui` & `pygubu_designer-0.39/examples/scrollbarhelper.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/scrolledframe-layouts.ui` & `pygubu_designer-0.39/examples/scrolledframe-layouts.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/scrolledframe.ui` & `pygubu_designer-0.39/examples/scrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/scrolledtext/scrolledtext_demo.ui` & `pygubu_designer-0.39/examples/scrolledtext/scrolledtext_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/scrolledtext/scrolledtextdemoapp.py` & `pygubu_designer-0.39/examples/scrolledtext/scrolledtextdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/static_image/demoapp.py` & `pygubu_designer-0.39/examples/static_image/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/static_image/demoapp.ui` & `pygubu_designer-0.39/examples/static_image/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/static_image/logo_253.png` & `pygubu_designer-0.39/examples/static_image/logo_253.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/text/logwindowdemo/demo1.ui` & `pygubu_designer-0.39/examples/text/logwindowdemo/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/text/logwindowdemo/demo1app.py` & `pygubu_designer-0.39/examples/text/logwindowdemo/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/tk_window/green.gif` & `pygubu_designer-0.39/examples/tk_window/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/tk_window/tkdemo.ui` & `pygubu_designer-0.39/examples/tk_window/tkdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/tk_window/tkdemoapp.py` & `pygubu_designer-0.39/examples/tk_window/tkdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/toplevel_centered/centered_demo1.py` & `pygubu_designer-0.39/examples/toplevel_centered/centered_demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/toplevel_centered/centered_demo2.py` & `pygubu_designer-0.39/examples/toplevel_centered/centered_demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/toplevel_centered/demo.ui` & `pygubu_designer-0.39/examples/toplevel_centered/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/toplevel_menu/menu.py` & `pygubu_designer-0.39/examples/toplevel_menu/menu.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/toplevel_menu/menu.ui` & `pygubu_designer-0.39/examples/toplevel_menu/menu.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview/demo1/treeview.py` & `pygubu_designer-0.39/examples/treeview/demo1/treeview.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview/demo1/treeview.ui` & `pygubu_designer-0.39/examples/treeview/demo1/treeview.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview/demo2/columns_stretching.ui` & `pygubu_designer-0.39/examples/treeview/demo2/columns_stretching.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview/demo2/columnsstretchingdemo.py` & `pygubu_designer-0.39/examples/treeview/demo2/columnsstretchingdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview_editable/demo1/demoapp.py` & `pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview_editable/demo1/demoapp.ui` & `pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview_editable/demo2/demo2.ui` & `pygubu_designer-0.39/examples/treeview_editable/demo2/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview_editable/demo2/demo2app.py` & `pygubu_designer-0.39/examples/treeview_editable/demo2/demo2app.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview_filterable/demo.ui` & `pygubu_designer-0.39/examples/treeview_filterable/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/treeview_filterable/demoapp.py` & `pygubu_designer-0.39/examples/treeview_filterable/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/user_input/userinput.ui` & `pygubu_designer-0.39/examples/user_input/userinput.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/user_input/userinputapp.py` & `pygubu_designer-0.39/examples/user_input/userinputapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/variables.ui` & `pygubu_designer-0.39/examples/variables.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/vscrolledframe.ui` & `pygubu_designer-0.39/examples/vscrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/windowdeleteevent/demo1.py` & `pygubu_designer-0.39/examples/windowdeleteevent/demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/windowdeleteevent/demo1.ui` & `pygubu_designer-0.39/examples/windowdeleteevent/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/windowdeleteevent/demo2.py` & `pygubu_designer-0.39/examples/windowdeleteevent/demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/examples/windowdeleteevent/demo2.ui` & `pygubu_designer-0.39/examples/windowdeleteevent/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/pyproject.toml` & `pygubu_designer-0.39/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "Topic :: Software Development :: User Interfaces",
 ]
 dependencies = [
     "appdirs >=1.4.3",
     "Mako >=1.1.4",
     "screeninfo >=0.8",
     "autopep8 >=1.7",
-    "pygubu >=0.33"
+    "pygubu >=0.35"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/alejandroautalan/pygubu-designer#readme"
 Issues = "https://github.com/alejandroautalan/pygubu-designer/issues"
 Source = "https://github.com/alejandroautalan/pygubu-designer"
```

### Comparing `pygubu-designer-0.38/src/pygubu_designer.egg-info/PKG-INFO` & `pygubu_designer-0.39/src/pygubu_designer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.38
+Version: 0.39
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
@@ -27,15 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 Requires-Dist: appdirs>=1.4.3
 Requires-Dist: Mako>=1.1.4
 Requires-Dist: screeninfo>=0.8
 Requires-Dist: autopep8>=1.7
-Requires-Dist: pygubu>=0.33
+Requires-Dist: pygubu>=0.35
 Provides-Extra: ttkwidgets
 Requires-Dist: ttkwidgets; extra == "ttkwidgets"
 Provides-Extra: tksheet
 Requires-Dist: tksheet; extra == "tksheet"
 Provides-Extra: tkinterweb
 Requires-Dist: tkinterweb; extra == "tkinterweb"
 Provides-Extra: tkintertable
```

### Comparing `pygubu-designer-0.38/src/pygubu_designer.egg-info/SOURCES.txt` & `pygubu_designer-0.39/src/pygubu_designer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 setup.py
 development/create-imgs.py
 development/dev-notes.txt
 development/devtool.py
 development/devtool.sh
 development/pygubudesigner_.py
 development/requirements.txt
+development/gettext/pygubu.its
+development/gettext/pygubu.loc
 development/new-designer-icons/main.py
 development/new-designer-icons/template.svg
 development/new-designer-icons/testnewicons.ui
 development/new-designer-icons/testnewiconsapp.py
-development/new-designer-icons/__pycache__/testnewiconsapp.cpython-311.pyc
 development/new-designer-icons/pygubu-icons/button.png
 development/new-designer-icons/pygubu-icons/button.svg
 development/new-designer-icons/pygubu-icons/canvas.png
 development/new-designer-icons/pygubu-icons/canvas.svg
 development/new-designer-icons/pygubu-icons/combobox.png
 development/new-designer-icons/pygubu-icons/combobox.svg
 development/new-designer-icons/pygubu-icons/default.png
@@ -104,19 +105,14 @@
 examples/control_variables/controlvariables.py
 examples/control_variables/controlvariables.ui
 examples/custom_widget/README.md
 examples/custom_widget/timer_main.ui
 examples/custom_widget/timerapp.py
 examples/custom_widget/timerappwidgets.py
 examples/custom_widget/timewidget.py
-examples/custom_widget/__pycache__/customappwidgets.cpython-38.pyc
-examples/custom_widget/__pycache__/timerappwidgets.cpython-310.pyc
-examples/custom_widget/__pycache__/timerappwidgets.cpython-38.pyc
-examples/custom_widget/__pycache__/timewidget.cpython-310.pyc
-examples/custom_widget/__pycache__/timewidget.cpython-38.pyc
 examples/customtkinter/README.md
 examples/customtkinter/complex/complex_demo.ui
 examples/customtkinter/complex/complexdemoapp.py
 examples/customtkinter/simple/simple_demo.ui
 examples/customtkinter/simple/simpledemoapp.py
 examples/dialogs/README.md
 examples/dialogs/demo1/README.md
@@ -128,22 +124,34 @@
 examples/dialogs/demo3/README.md
 examples/dialogs/demo3/demo.py
 examples/dialogs/demo3/demo.ui
 examples/dialogs/demo4/README.md
 examples/dialogs/demo4/settingsdemo.ui
 examples/dialogs/demo4/settingsdemoapp.py
 examples/dialogs/demo4/settingsdialog.py
-examples/dialogs/demo4/__pycache__/settingsdialog.cpython-310.pyc
-examples/forms/__pycache__/formsdemo1base.cpython-310.pyc
+examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
+examples/forms/demo1.ui
+examples/forms/formsdemo1app.py
+examples/forms/formsdemo1appui.py
+examples/forms/project_styles.py
+examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
 examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
+examples/forms/__pycache__/project_styles.cpython-311.pyc
 examples/helloworld/README.md
 examples/helloworld/helloworld.py
 examples/helloworld/helloworld.ui
 examples/helloworld/holamundo.py
 examples/helloworld/holamundo.ui
+examples/i18n_gettext_demo/README.md
+examples/i18n_gettext_demo/demo-i18n.ui
+examples/i18n_gettext_demo/demoapp.py
+examples/i18n_gettext_demo/i18n.py
+examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc
+examples/i18n_gettext_demo/locale/demoapp.pot
+examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo
 examples/image_property/green.gif
 examples/image_property/image_property.py
 examples/image_property/image_property.ui
 examples/image_property/red.gif
 examples/image_property/yellow.gif
 examples/integration_with_cxFreeze/README.md
 examples/integration_with_cxFreeze/myapp.py
@@ -181,29 +189,23 @@
 examples/integration_with_pyinstaller/imgs/ps_square.gif
 examples/integration_with_pyinstaller/imgs/ps_triangle.gif
 examples/integration_with_tkcalendar/README.md
 examples/integration_with_tkcalendar/myapp1/main.ui
 examples/integration_with_tkcalendar/myapp1/myapp.py
 examples/integration_with_tkcalendar/myapp1/requirements.txt
 examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
-examples/integration_with_tkcalendar/myapp1/__pycache__/tkcalendarwidgets.cpython-38.pyc
 examples/integration_with_tkcalendar/myapp2/main.ui
 examples/integration_with_tkcalendar/myapp2/myapp.py
 examples/integration_with_tkcalendar/myapp2/requirements.txt
 examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
-examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-310.pyc
-examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-38.pyc
 examples/integration_with_tkcalendar/myapp3/main.ui
 examples/integration_with_tkcalendar/myapp3/myapp.py
 examples/integration_with_tkcalendar/myapp3/requirements.txt
 examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
-examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-310.pyc
-examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-38.pyc
 examples/integration_with_zipapp/README.md
-examples/integration_with_zipapp/demoapp.pyz
 examples/integration_with_zipapp/src/demoapp/__init__.py
 examples/integration_with_zipapp/src/demoapp/main.py
 examples/integration_with_zipapp/src/demoapp/data/__init__.py
 examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
 examples/integration_with_zipapp/src/demoapp/data/green.gif
 examples/integration_with_zipapp/src/demoapp/data/info.txt
 examples/integration_with_zipapp/src/demoapp/data/red.gif
@@ -217,14 +219,17 @@
 examples/notebook/demo1.ui
 examples/notebook/demo1app.py
 examples/pathchooserdemo/README.md
 examples/pathchooserdemo/demo1/pathchooserdemo.py
 examples/pathchooserdemo/demo1/pathchooserdemo.ui
 examples/pathchooserdemo/demo2/pathchooserdemo.py
 examples/pathchooserdemo/demo2/pathchooserdemo.ui
+examples/scrolledframe/README.md
+examples/scrolledframe/demoapp.py
+examples/scrolledframe/scrolledframe_demo.ui
 examples/scrolledtext/scrolledtext_demo.ui
 examples/scrolledtext/scrolledtextdemoapp.py
 examples/static_image/demoapp.py
 examples/static_image/demoapp.ui
 examples/static_image/logo_253.png
 examples/static_image/requirements.txt
 examples/text/logwindowdemo/demo1.ui
@@ -270,33 +275,37 @@
 src/pygubu_designer.egg-info/requires.txt
 src/pygubu_designer.egg-info/top_level.txt
 src/pygubudesigner/__init__.py
 src/pygubudesigner/__main__.py
 src/pygubudesigner/actions.py
 src/pygubudesigner/bindingseditor.py
 src/pygubudesigner/containerlayouteditor.py
+src/pygubudesigner/designerstyles.py
 src/pygubudesigner/dialogs.py
 src/pygubudesigner/i18n.py
 src/pygubudesigner/layouteditor.py
 src/pygubudesigner/logpanel.py
 src/pygubudesigner/main.py
 src/pygubudesigner/preferences.py
 src/pygubudesigner/propertieseditor.py
 src/pygubudesigner/rfilemanager.py
-src/pygubudesigner/stylehandler.py
 src/pygubudesigner/uitreeeditor.py
 src/pygubudesigner/widgetdescr.py
 src/pygubudesigner/codegen/__init__.py
 src/pygubudesigner/codegen/codebuilder.py
 src/pygubudesigner/codegen/scriptgenerator.py
 src/pygubudesigner/data/code_templates/app.py.mako
+src/pygubudesigner/data/code_templates/appuser.py.mako
 src/pygubudesigner/data/code_templates/base.py.mako
 src/pygubudesigner/data/code_templates/customstyles.py.mako
 src/pygubudesigner/data/code_templates/script.py.mako
+src/pygubudesigner/data/code_templates/scriptuser.py.mako
 src/pygubudesigner/data/code_templates/widget.py.mako
+src/pygubudesigner/data/code_templates/widgetbo.py.mako
+src/pygubudesigner/data/code_templates/widgetuser.py.mako
 src/pygubudesigner/data/images/images-gif/arrow-left2.gif
 src/pygubudesigner/data/images/images-gif/arrow-right2.gif
 src/pygubudesigner/data/images/images-gif/bin-16.gif
 src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
 src/pygubudesigner/data/images/images-gif/close.gif
 src/pygubudesigner/data/images/images-gif/download3-16.gif
 src/pygubudesigner/data/images/images-gif/download3-32.gif
@@ -568,24 +577,47 @@
 src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
 src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
 src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
 src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
 src/pygubudesigner/data/ui/about_dialog.ui
 src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
 src/pygubudesigner/data/ui/container_layout_editor_base.ui
-src/pygubudesigner/data/ui/preferences_dialog.ui
+src/pygubudesigner/data/ui/designer_settings.ui
+src/pygubudesigner/data/ui/messagebox.ui
+src/pygubudesigner/data/ui/project_settings.ui
 src/pygubudesigner/data/ui/pygubu-ui.ui
+src/pygubudesigner/data/ui/treecomponent_palette.ui
 src/pygubudesigner/preview/__init__.py
 src/pygubudesigner/preview/builder.py
 src/pygubudesigner/preview/helper.py
 src/pygubudesigner/preview/preview.py
 src/pygubudesigner/properties/__init__.py
 src/pygubudesigner/properties/manager.py
 src/pygubudesigner/properties/predefined.py
 src/pygubudesigner/properties/propertieshelp.py
+src/pygubudesigner/properties/editors/__init__.py
+src/pygubudesigner/properties/editors/forms.py
+src/pygubudesigner/services/__init__.py
+src/pygubudesigner/services/aboutdialog.py
+src/pygubudesigner/services/aboutdialogui.py
+src/pygubudesigner/services/designersettings.py
+src/pygubudesigner/services/designersettingsui.py
+src/pygubudesigner/services/fieldvalidator.py
+src/pygubudesigner/services/messagebox.py
+src/pygubudesigner/services/messageboxui.py
+src/pygubudesigner/services/project.py
+src/pygubudesigner/services/projectsettings.py
+src/pygubudesigner/services/projectsettingsui.py
+src/pygubudesigner/services/stylehandler.py
+src/pygubudesigner/services/theming.py
+src/pygubudesigner/services/builders/__init__.py
+src/pygubudesigner/services/widgets/__init__.py
+src/pygubudesigner/services/widgets/treecomponentpalette.py
+src/pygubudesigner/services/widgets/treecomponentpalettebo.py
+src/pygubudesigner/services/widgets/treecomponentpaletteui.py
 src/pygubudesigner/util/__init__.py
 src/pygubudesigner/util/gridcalculator.py
 src/pygubudesigner/util/keyboard.py
 src/pygubudesigner/util/observable.py
 src/pygubudesigner/util/screens.py
 src/pygubudesigner/util/selecttool.py
 src/pygubudesigner/widgets/__init__.py
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/actions.py` & `pygubu_designer-0.39/src/pygubudesigner/actions.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/bindingseditor.py` & `pygubu_designer-0.39/src/pygubudesigner/bindingseditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import tkinter as tk
 import tkinter.ttk as ttk
 
 from pygubu import builder
 from pygubu.widgets.editabletreeview import InplaceEditor
 
 from .widgets.bindingeditor import EventHandlerEditor, SequenceEditor
+from .widgetdescr import WidgetMeta
+
 
 CLASS_MAP = builder.CLASS_MAP
 
 
 class EventhandlerInplaceEditor(InplaceEditor):
     def __init__(self, master):
         self._editor = e = EventHandlerEditor(master)
@@ -132,15 +134,15 @@
             for item in items:
                 if item != self._adder:
                     values = self.tv.item(item, "values")
                     self._curr_data.add_binding(*values[:3])
 
             # Notify the editor that a change has occurred and the project needs saving.
             # Changed: August 17, 2021
-            self._curr_data.notify(self)
+            self._curr_data.notify(WidgetMeta.BINDING_CHANGED)
 
     def _add_binding(self, bind):
         idx = self.tv.index(self._adder)
         self.tv.insert("", idx, values=bind)
         self.tv.selection_set("")
 
     def edit(self, wdescr):
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/codegen/codebuilder.py` & `pygubu_designer-0.39/src/pygubudesigner/codegen/codebuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pygubu import Builder
 from pygubu.api.v1 import BuilderObject, register_widget
 from pygubu.component.builderobject import CB_TYPES, CLASS_MAP
 from pygubu.component.widgetmeta import WidgetMeta
 from pygubu.plugins.tk.tkstdwidgets import TKToplevel
 from pygubu.stockimage import TK_BITMAP_FORMATS
 
-from pygubudesigner.stylehandler import StyleHandler
+from pygubudesigner.services.stylehandler import StyleHandler
 
 
 class ToplevelOrTk(TKToplevel):
     def code_realize(self, boparent, code_identifier=None):
         if code_identifier is not None:
             self._code_identifier = code_identifier
         lines = []
@@ -64,14 +64,15 @@
     APP_UI_METHOD = 4
     APP_CODE_METHOD = 5
 
 
 class RealizeMode(Enum):
     APP = 1
     METHOD = 2
+    MAIN_MENU = 3
 
 
 class UI2Code(Builder):
     def __init__(self):
         super().__init__()
 
         self._script_type = None
@@ -107,14 +108,15 @@
 
     def _process_options(self, kw):
         kwdef = {
             "as_class": True,
             "tabspaces": 8,
             "script_type": ScriptType.APP_WITH_UI,
             "on_first_object_cb": None,
+            "main_menu": None,
         }
         kwdef.update(kw)
         self._options = kwdef
         self.as_class = self._options["as_class"]
         self.tabspaces = self._options["tabspaces"]
         self._script_type = self._options["script_type"]
         self._on_first_object_cb = self._options["on_first_object_cb"]
@@ -161,21 +163,31 @@
 
         if self._realize_mode == RealizeMode.APP:
             self._current_target = target
 
         if wmeta is not None:
             self._code_realize(builder, wmeta)
 
-    def generate_app_with_ui(self, uidef, target):
+        #
+        # Generate method callback definitions for associated main menu.
+        #
+        main_menu = self._options["main_menu"]
+        if main_menu is not None:
+            wmeta = self.uidefinition.get_widget(main_menu)
+            self._realize_mode = RealizeMode.MAIN_MENU
+            self._code_realize(builder, wmeta)
+
+    def generate_app_with_ui(self, uidef, target, main_menu=None):
         self.generate(
             uidef,
             target,
             as_class=False,
             tabspaces=8,
             script_type=ScriptType.APP_WITH_UI,
+            main_menu=main_menu,
         )
         return self._process_results(target)
 
     def generate_app_code(
         self,
         uidef,
         target,
@@ -332,16 +344,19 @@
             self._tkvariablehints[vname] = var_create.split("(")[0]
             self._import_tk = True
         return self._tkvariables[vname]
 
     def _add_new_code(self, newcode: list):
         if self._realize_mode == RealizeMode.APP:
             self._code.extend(newcode)
-        else:
+        elif self._realize_mode == RealizeMode.METHOD:
             self._methods[self._current_method].extend(newcode)
+        else:
+            # RealizeMode.MAIN_MENU
+            pass
 
     def _get_unique_id(self, wmeta, uniqueid, masterid):
         if self.as_class:
             if wmeta.is_named or self.all_ids_as_attributes:
                 uniqueid = "self." + uniqueid if masterid else "self"
         return uniqueid
 
@@ -502,16 +517,15 @@
         output = name.replace(".", "_")
         output = "".join(x for x in output if x.isalnum() or x == "_")
         return output
 
     def code_translate_str(self, value: str) -> str:
         escaped = BuilderObject.code_escape_str(value)
         if self.with_i18n_support:
-            trval = f"_({escaped})"
-            return trval
+            return f"_({escaped})"
         else:
             return escaped
 
     @property
     def with_i18n_support(self) -> bool:
         return self._with_i18n_support
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/codegen/scriptgenerator.py` & `pygubu_designer-0.39/src/pygubudesigner/codegen/scriptgenerator.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,291 +11,292 @@
 # PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 import keyword
 import logging
 import pathlib
+import tkinter as tk
 from tkinter import filedialog, messagebox
 
 import autopep8
 from mako.lookup import TemplateLookup
 
 from .codebuilder import UI2Code
-from pygubudesigner.stylehandler import StyleHandler
+from pygubudesigner.services.stylehandler import StyleHandler
+from pygubudesigner.services.project import Project
+
 
 logger = logging.getLogger(__name__)
 DATA_DIR = pathlib.Path(__file__).parent.parent / "data"
 TEMPLATE_DIR = DATA_DIR / "code_templates"
 makolookup = TemplateLookup(directories=[TEMPLATE_DIR])
 
 
 class ScriptGenerator:
     def __init__(self, app):
         self.app = app
-        self.builder = builder = app.builder
+        self.builder = app.builder
         self.tree = app.tree_editor
         self.projectname = ""
 
-        self.widgetlist = w = builder.get_object("widgetlist")
-        w.bind("<<ComboboxSelected>>", self._configure_menulist)
-        self.menulist = builder.get_object("menulist")
-
-        self.widgetlistvar = None
-        self.widgetlist_keyvar = None
-        self.template_var = None
-        self.classnamevar = None
-        self.template_desc_var = None
-        self.import_tkvars_var = None
-        self.use_ttkdefs_file_var = None
-        self.add_i18n_var = None
-        self.menulist_keyvar = None
-        myvars = [
-            "widgetlistvar",
-            "widgetlist_keyvar",
-            "template_var",
-            "classnamevar",
-            "template_desc_var",
-            "import_tkvars_var",
-            "use_ttkdefs_file_var",
-            "add_i18n_var",
-            "menulist_keyvar",
-            "all_ids_attributes_var",
-            "add_window_centering_code_var",
-        ]
-        builder.import_variables(self, myvars)
-
-        self.txt_code = builder.get_object("txt_code")
-        self.cb_import_tkvars = builder.get_object("cb_import_tkvars")
-        self.cb_add_i18n = builder.get_object("cb_add_i18n")
-        self.cb_all_ids_attributes = builder.get_object("cb_all_ids_attributes")
-
         _ = self.app.translator
         self.msgtitle = _("Script Generator")
 
-        self.template_desc = {
-            "application": _(
-                "Create a pygubu application script using the UI definition."
-            ),
-            "codescript": _("Create a coded version of the UI definition."),
-            "widget": _("Create a base class for your custom widget."),
-        }
-        self.template_var.set("application")
-        self.import_tkvars_var.set(True)
-        self.use_ttkdefs_file_var.set(False)
+    def _appui_code(self, generator, context):
+        uidef = self.tree.tree_to_uidef()
 
-    def camel_case(self, st):
-        output = "".join(x for x in st.title() if x.isalnum())
-        return output
+        generator.add_import_line("pathlib")
+        # if not main_widget_is_toplevel:
+        generator.add_import_line("tkinter", "tk", priority=1)
+        generator.add_import_line("pygubu", priority=10)
+        target = context["target"]
+        main_menu_id = None
+        if context["set_main_menu"]:
+            main_menu_id = context["main_menu_id"]
+        code = generator.generate_app_with_ui(
+            uidef, target, main_menu=main_menu_id
+        )
 
-    def on_code_generate_clicked(self):
-        if self.form_valid():
-            tree_item = self.widgetlist_keyvar.get()
-            template = self.template_var.get()
-            generator = UI2Code()
-            uidef = self.tree.tree_to_uidef()
-            target = self.tree.get_widget_id(tree_item)
-            target_class = self.tree.get_widget_class(tree_item)
-            class_name = self.classnamevar.get()
-            with_i18n_support = self.add_i18n_var.get()
-            all_ids_attributes = self.all_ids_attributes_var.get()
-            add_window_centering_code = self.add_window_centering_code_var.get()
-
-            main_widget_is_toplevel = False
-            set_main_menu = False
-            main_menu_id = None
-            toplevel_uids = (
-                "tk.Tk",
-                "tk.Toplevel",
-                "customtkinter.CTk",
-                "customtkinter.CTkToplevel",
-            )
+        context["import_lines"] = code["imports"]
+        # Set project paths
+        context["set_project_path"] = True
+
+        # Callbacks
+        context["callbacks"] = code["callbacks"]
+        # Tk Variables
+        if context["import_tk_vars"]:
+            context["tkvariables"] = code["tkvariables"]
+            context["tkvariablehints"] = code["tkvariablehints"]
+
+        bcontext = context.copy()
+        bcontext["class_name"] = context["class_name"] + "UI"
+        tpl = makolookup.get_template("app.py.mako")
+        final_code = tpl.render(**bcontext)
+        final_code = self._format_code(final_code)
+
+        output_dir = context["output_dir"]
+        outfn = output_dir / (context["module_name"] + "ui.py")
+        with open(outfn, "wt") as outfile:
+            outfile.write(final_code)
+            logger.info("Generated code file: %s", outfn)
+
+        context["import_lines"] += (
+            "\nfrom "
+            + context["module_name"]
+            + "ui import "
+            + bcontext["class_name"]
+        )
+        tpl = makolookup.get_template("appuser.py.mako")
+        final_code = tpl.render(**context)
+        final_code = self._format_code(final_code)
+        outfn: pathlib.Path = output_dir / (context["module_name"] + ".py")
+        # DO NOT overwrite user module.
+        if not outfn.exists():
+            with open(outfn, "wt") as outfile:
+                outfile.write(final_code)
+                logger.info("Generated code file: %s", outfn)
+
+    def _script_code(self, generator, context):
+        uidef = self.tree.tree_to_uidef()
+        target = context["target"]
+
+        if not context["main_widget_is_toplevel"]:
+            generator.add_import_line("tkinter", "tk")
+
+        first_object_callback = None
+        if context["has_ttk_styles"]:
+            ttk_styles_module = context["ttk_styles_module"]
+            first_object_callback = f"{ttk_styles_module}.setup_ttk_styles"
+
+        methods = []
+        if context["set_main_menu"]:
+            methods.append(context["main_menu_id"])
+        # Generate code
+        code = generator.generate_app_code(
+            uidef,
+            target,
+            methods_for=methods,
+            on_first_object_cb=first_object_callback,
+        )
+
+        # Prepare template context
+        context["widget_code"] = code[target]
+        context["import_lines"] = code["imports"]
+        context["callbacks"] = code["callbacks"]
+        context["methods"] = code["methods"]
+        context["target_code_id"] = code["target_code_id"]
+
+        bcontext = context.copy()
+        bcontext["class_name"] = context["class_name"] + "UI"
+        tpl = makolookup.get_template("script.py.mako")
+        final_code = tpl.render(**bcontext)
+        final_code = self._format_code(final_code)
+
+        output_dir = context["output_dir"]
+        outfn = output_dir / (context["module_name"] + "ui.py")
+        with open(outfn, "wt") as outfile:
+            outfile.write(final_code)
+
+        tpl = makolookup.get_template("scriptuser.py.mako")
+        final_code = tpl.render(**context)
+        final_code = self._format_code(final_code)
+        outfn: pathlib.Path = output_dir / (context["module_name"] + ".py")
+        # DO NOT overwrite user module.
+        if not outfn.exists():
+            with open(outfn, "wt") as outfile:
+                outfile.write(final_code)
+                logger.info("Generated code file: %s", outfn)
+
+    def _widget_code(self, generator, context):
+        uidef = self.tree.tree_to_uidef()
+        target = context["target"]
+
+        # generator.with_i18n_support = False
+        generator.add_import_line("tkinter", "tk")
+        # Generate code
+        code = generator.generate_app_widget(uidef, target)
+        # Prepare template context
+        context["widget_code"] = code[target]
+        context["import_lines"] = code["imports"]
+        context["callbacks"] = code["callbacks"]
+
+        bcontext = context.copy()
+        bcontext["class_name"] = context["class_name"] + "UI"
+        tpl = makolookup.get_template("widget.py.mako")
+        final_code = tpl.render(**bcontext)
+        final_code = self._format_code(final_code)
+
+        output_dir = context["output_dir"]
+        outfn = output_dir / (context["module_name"] + "ui.py")
+        with open(outfn, "wt") as outfile:
+            outfile.write(final_code)
+            logger.info("Generated code file: %s", outfn)
+
+        tpl = makolookup.get_template("widgetbo.py.mako")
+        final_code = tpl.render(**context)
+        final_code = self._format_code(final_code)
+        output_dir2 = context["output_dir2"]
+        outfn: pathlib.Path = output_dir2 / (context["module_name"] + "bo.py")
+        # DO NOT overwrite user module.
+        if not outfn.exists():
+            with open(outfn, "wt") as outfile:
+                outfile.write(final_code)
+                logger.info("Generated code file: %s", outfn)
+
+        tpl = makolookup.get_template("widgetuser.py.mako")
+        final_code = tpl.render(**context)
+        final_code = self._format_code(final_code)
+        outfn: pathlib.Path = output_dir / (context["module_name"] + ".py")
+        # DO NOT overwrite user module.
+        if not outfn.exists():
+            with open(outfn, "wt") as outfile:
+                outfile.write(final_code)
+                logger.info("Generated code file: %s", outfn)
+
+    def generate_code(self):
+        project = self.app.current_project
+        config = project.get_full_settings()
+        generator = UI2Code()
+        template = config["template"]
+        target = config["main_widget"]
+        itemid = self.tree.get_tree_topitem_byid(target)
+        target_class = self.tree.get_widget_class(itemid)
+
+        toplevel_uids = (
+            "tk.Tk",
+            "tk.Toplevel",
+            "customtkinter.CTk",
+            "customtkinter.CTkToplevel",
+        )
 
-            if target_class in toplevel_uids:
-                main_widget_is_toplevel = True
+        main_widget_is_toplevel = False
+        main_menu_id = ""
+        set_main_menu = False
+        has_ttk_styles = False
+
+        if target_class in toplevel_uids:
+            main_widget_is_toplevel = True
+            # Main menu definition
+            main_menu_id = config["main_menu"]
+            if main_menu_id and template != "widget":
+                set_main_menu = True
+
+        # Style definitions
+        use_ttk_styles = tk.getboolean(config["use_ttk_styledefinition_file"])
+        ttk_styles_module = config["ttk_style_definition_file"]
+
+        use_first_object_cb = use_ttk_styles
+        first_object_func = "None"
+
+        has_ttk_styles = False
+        if use_ttk_styles and ttk_styles_module:
+            has_ttk_styles = True
+            first_object_func = f"{ttk_styles_module}.setup_ttk_styles"
+
+        with_i18n_support = tk.getboolean(config["use_i18n"])
+        import_tk_vars = tk.getboolean(config["import_tkvariables"])
+        add_window_centering_code = tk.getboolean(
+            config["use_window_centering_code"]
+        )
 
-                # Main menu definition
-                menu_item = self.menulist_keyvar.get()
-                if menu_item not in ("empty", "None") and template != "widget":
-                    main_menu_id = self.tree.get_widget_id(menu_item)
-                    set_main_menu = True
-
-            # Style definitions
-            ttk_styles_module = StyleHandler.get_ttk_styles_module()
-            has_ttk_styles = False
-            if self.use_ttkdefs_file_var.get() and ttk_styles_module:
-                has_ttk_styles = True
-
-            context = {
-                "project_name": self.projectname,
-                "class_name": class_name,
-                "main_widget_is_toplevel": main_widget_is_toplevel,
-                "main_widget": target,
-                "widget_base_class": target_class,
-                "widget_code": None,
-                "import_lines": None,
-                "callbacks": "",
-                "tkvariables": [],
-                "has_ttk_styles": has_ttk_styles,
-                "ttk_styles_module": ttk_styles_module,
-                "set_project_path": False,
-                "with_i18n_support": with_i18n_support,
-                "set_main_menu": set_main_menu,
-                "main_menu_id": main_menu_id,
-                "add_window_centering_code": add_window_centering_code,
-            }
-
-            generator.with_i18n_support = with_i18n_support
-            generator.all_ids_as_attributes = all_ids_attributes
-
-            if template == "application":
-                generator.add_import_line("pathlib")
-                # if not main_widget_is_toplevel:
-                generator.add_import_line("tkinter", "tk", priority=1)
-                generator.add_import_line("pygubu", priority=10)
-                code = generator.generate_app_with_ui(uidef, target)
-
-                context["import_lines"] = code["imports"]
-                # Set project paths
-                context["set_project_path"] = True
-
-                # Callbacks
-                context["callbacks"] = code["callbacks"]
-                # Tk Variables
-                if self.import_tkvars_var.get():
-                    context["tkvariables"] = code["tkvariables"]
-                    context["tkvariablehints"] = code["tkvariablehints"]
-                tpl = makolookup.get_template("app.py.mako")
-                final_code = tpl.render(**context)
-                final_code = self._format_code(final_code)
-                self.set_code(final_code)
-            elif template == "widget":
-                generator.with_i18n_support = False
-                generator.add_import_line("tkinter", "tk")
-                # Generate code
-                code = generator.generate_app_widget(uidef, target)
-                # Prepare template context
-                context["widget_code"] = code[target]
-                context["import_lines"] = code["imports"]
-                context["callbacks"] = code["callbacks"]
-
-                tpl = makolookup.get_template("widget.py.mako")
-                final_code = tpl.render(**context)
-                final_code = self._format_code(final_code)
-                self.set_code(final_code)
-            elif template == "codescript":
-                if not main_widget_is_toplevel:
-                    generator.add_import_line("tkinter", "tk")
-
-                first_object_callback = None
-                if has_ttk_styles:
-                    first_object_callback = (
-                        f"{ttk_styles_module}.setup_ttk_styles"
-                    )
-
-                methods = []
-                if set_main_menu:
-                    methods.append(main_menu_id)
-                # Generate code
-                code = generator.generate_app_code(
-                    uidef,
-                    target,
-                    methods_for=methods,
-                    on_first_object_cb=first_object_callback,
-                )
-
-                # Prepare template context
-                context["widget_code"] = code[target]
-                context["import_lines"] = code["imports"]
-                context["callbacks"] = code["callbacks"]
-                context["methods"] = code["methods"]
-                context["target_code_id"] = code["target_code_id"]
-
-                tpl = makolookup.get_template("script.py.mako")
-                final_code = tpl.render(**context)
-                final_code = self._format_code(final_code)
-                self.set_code(final_code)
-
-    def on_code_copy_clicked(self):
-        text = self.get_code()
-        self.txt_code.clipboard_clear()
-        self.txt_code.clipboard_append(text)
+        # calculate output dir
+        uipath = self.app.current_project.fpath.parent
+        output_dir: pathlib.Path = config["output_dir"]
+        if output_dir:
+            output_dir = uipath / output_dir
+        else:
+            output_dir = uipath
+        output_dir2: pathlib.Path = config["output_dir2"]
+        if output_dir2:
+            output_dir2 = uipath / output_dir2
+        else:
+            output_dir2 = uipath
+
+        context = {
+            "output_dir": output_dir,
+            "output_dir2": output_dir2,
+            "target": target,
+            "module_name": config["module_name"],
+            "project_name": self.app.project_name(),
+            "class_name": config["main_classname"],
+            "main_widget_is_toplevel": main_widget_is_toplevel,
+            "main_widget": target,
+            "widget_base_class": target_class,
+            "widget_code": None,
+            "import_lines": None,
+            "callbacks": "",
+            "tkvariables": [],
+            "use_first_object_cb": use_first_object_cb,
+            "first_object_func": first_object_func,
+            "has_ttk_styles": has_ttk_styles,
+            "ttk_styles_module": ttk_styles_module,
+            "set_project_path": False,
+            "with_i18n_support": with_i18n_support,
+            "set_main_menu": set_main_menu,
+            "main_menu_id": main_menu_id,
+            "add_window_centering_code": add_window_centering_code,
+            "import_tk_vars": import_tk_vars,
+        }
 
-        _ = self.app.translator
-        msg = _("Code copied")
-        messagebox.showinfo(
-            title=self.msgtitle,
-            message=msg,
-            parent=self.widgetlist.winfo_toplevel(),
+        generator.with_i18n_support = with_i18n_support
+        generator.all_ids_as_attributes = tk.getboolean(
+            config["all_ids_attributes"]
         )
 
-    def on_code_template_changed(self, clear_code=True):
-        template = self.template_var.get()
-        classname = self.get_classname()
-        import_tkvars_state = "disabled"
-        add_i18n_state = "normal"
-        menulist_state = "normal"
-        all_ids_state = "normal"
         if template == "application":
-            name = f"{classname}App"
-            self.classnamevar.set(name)
-            import_tkvars_state = "normal"
-            all_ids_state = "disabled"
-        elif template == "codescript":
-            name = f"{classname}App"
-            self.classnamevar.set(name)
+            self._appui_code(generator, context)
         elif template == "widget":
-            name = f"{classname}Widget"
-            self.classnamevar.set(name)
-            add_i18n_state = "disabled"
-            menulist_state = "disabled"
-        self.cb_import_tkvars.configure(state=import_tkvars_state)
-        self.cb_add_i18n.configure(state=add_i18n_state)
-        self.cb_all_ids_attributes.configure(state=all_ids_state)
-        self.menulist.configure(state=menulist_state)
-        # Update template description
-        self.template_desc_var.set(self.template_desc[template])
-        if clear_code:
-            self.set_code("")
+            self._widget_code(generator, context)
+        elif template == "codescript":
+            self._script_code(generator, context)
 
-    def on_code_save_clicked(self):
-        _ = self.app.translator
-        filename = (self.classnamevar.get()).lower()
-        options = {
-            "defaultextension": ".py",
-            "filetypes": ((_("Python Script"), "*.py"), (_("All"), "*.*")),
-            "initialfile": f"{filename}.py",
-        }
-        fname = filedialog.asksaveasfilename(**options)
-        if fname:
-            with open(fname, "w") as out:
-                out.write(self.get_code())
-
-    def _configure_menulist(self, event=None):
-        tree_item = self.widgetlist_keyvar.get()
-        target_class = self.tree.get_widget_class(tree_item)
-        newstate = "normal" if target_class == "tk.Toplevel" else "disabled"
-        self.menulist.configure(state=newstate)
-
-    def configure(self):
-        self.projectname = self.app.project_name()
-        # Top level widgets
-        wlist = self.tree.get_top_widget_list()
-        self.widgetlist.configure(values=wlist)
-        self.classnamevar.set(self.get_classname())
-        # Top level menues
-        mlist = self.tree.get_top_menu_list()
-        mlist.insert(0, ("empty", ""))
-        self.menulist.configure(values=mlist)
-        # self.menulist_keyvar.set('None')
-
-        if len(wlist) > 0:
-            key = wlist[0][0]
-            self.widgetlist_keyvar.set(key)
-        self.on_code_template_changed(False)
+    def camel_case(self, st):
+        output = "".join(x for x in st.title() if x.isalnum())
+        return output
 
     def get_classname(self):
         name = pathlib.Path(self.projectname).stem
         return self.camel_case(name)
 
     def form_valid(self):
         valid = True
@@ -327,20 +328,9 @@
             valid = False
             messagebox.showwarning(
                 title=mbtitle, message=_("Invalid classname"), parent=parent
             )
 
         return valid
 
-    def set_code(self, text):
-        self.txt_code.delete("0.0", "end")
-        self.txt_code.insert("0.0", text)
-
-    def get_code(self):
-        return self.txt_code.get("0.0", "end-1c")
-
-    def reset(self):
-        self.set_code("")
-        self.configure()
-
     def _format_code(self, code):
         return autopep8.fix_code(code, options={"aggressive": 1})
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/containerlayouteditor.py` & `pygubu_designer-0.39/src/pygubudesigner/containerlayouteditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             for col in self._current.gridrc_column_indexes():
                 if col == "all":
                     self.gridselector.mark_grid_cols()
                 else:
                     self.gridselector.mark_column(int(col))
 
             # Update the preview now, after the grid rc changes have been made.
-            target.notify("LAYOUT_GRIDRC_CHANGED", target)
+            target.notify(WidgetMeta.LAYOUT_PROPERTY_CHANGED, target)
 
     def _on_gridcell_clicked(self, event=None):
         self._edit_grid_cell(*self.gridselector.selection)
 
     def _edit_grid_cell(self, row, col):
         # Update RC properties editors for cell
         target = self._current
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/code_templates/app.py.mako` & `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/app.py.mako`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 <%inherit file="base.py.mako"/>
 <%block name="project_paths" filter="trim">
 PROJECT_PATH = pathlib.Path(__file__).parent
 PROJECT_UI = PROJECT_PATH / "${project_name}"
+RESOURCE_PATHS = [PROJECT_PATH]
 </%block>
 
 <%block name="class_definition" filter="trim">
 class ${class_name}:
-%if with_i18n_support and has_ttk_styles:
-    def __init__(self, master=None, translator=None):
-        self.builder = builder = pygubu.Builder(
+%if with_i18n_support and use_first_object_cb:
+    def __init__(self, master=None, translator=None, on_first_object_cb=None):
+        self.builder = pygubu.Builder(
             translator=translator,
-            on_first_object=${ttk_styles_module}.setup_ttk_styles)
+            on_first_object=on_first_object_cb)
 %elif with_i18n_support:
     def __init__(self, master=None, translator=None):
-        self.builder = builder = pygubu.Builder(translator)
-%elif has_ttk_styles:
-    def __init__(self, master=None):
-        self.builder = builder = pygubu.Builder(
-            on_first_object=${ttk_styles_module}.setup_ttk_styles)
+        self.builder = pygubu.Builder(translator)
+%elif use_first_object_cb:
+    def __init__(self, master=None, on_first_object_cb=None):
+        self.builder = pygubu.Builder(
+            on_first_object=on_first_object_cb)
 %else:
     def __init__(self, master=None):
-        self.builder = builder = pygubu.Builder()
+        self.builder = pygubu.Builder()
 %endif
-        builder.add_resource_path(PROJECT_PATH)
-        builder.add_from_file(PROJECT_UI)
+        self.builder.add_resource_paths(RESOURCE_PATHS)
+        self.builder.add_from_file(PROJECT_UI)
         # Main widget
-        self.mainwindow:${widget_base_class} = builder.get_object("${main_widget}", master)
+        self.mainwindow:${widget_base_class} = self.builder.get_object("${main_widget}", master)
 %if set_main_menu:
         # Main menu
-        _main_menu = builder.get_object("${main_menu_id}", self.mainwindow)
+        _main_menu = self.builder.get_object("${main_menu_id}", self.mainwindow)
         self.mainwindow.configure(menu=_main_menu)
 %endif
     %if tkvariables:
 
         %for var in tkvariables:
         self.${var}:${tkvariablehints[var]} = None
         %endfor
-        builder.import_variables(self)
+        self.builder.import_variables(self)
 
     %endif
-        builder.connect_callbacks(self)
+        self.builder.connect_callbacks(self)
 
 %if add_window_centering_code:
     def center(self, event):
         wm_min = self.mainwindow.wm_minsize()
         wm_max = self.mainwindow.wm_maxsize()
         screen_w = self.mainwindow.winfo_screenwidth()
         screen_h = self.mainwindow.winfo_screenheight()
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/code_templates/customstyles.py.mako` & `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/customstyles.py.mako`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 import tkinter as tk
 import tkinter.ttk as ttk
 
 
 def setup_ttk_styles(master=None):
     my_font = ("helvetica", 12, "bold")
-    
+
     style = ttk.Style(master)
-    
+
     style.configure("primary.TButton",
                     font=my_font,
                     background="#4582EC",
                     foreground="white")
     style.configure("secondary.TButton",
                     font=my_font,
-                    background="#ADB5BD", 
+                    background="#ADB5BD",
                     foreground="white")
     style.configure("warning.TButton",
                     font=my_font,
-                    background="#F0AD4E", 
-                    foreground="white")    
+                    background="#F0AD4E",
+                    foreground="white")
     style.configure("danger.TButton",
                     font=my_font,
-                    background="#D9534F", 
+                    background="#D9534F",
                     foreground="white")
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/code_templates/script.py.mako` & `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/script.py.mako`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 <%inherit file="base.py.mako"/>
 
 <%block name="class_definition" filter="trim">
-class ${class_name}:
 %if with_i18n_support:
-    def __init__(self, master=None, translator=None):
-        _ = translator
-        if translator is None:
-            _ = lambda x: x
-%else:
-    def __init__(self, master=None):
+# Begin i18n - Setup translator in derived class file
+def i18n_noop(value): return value
+i18n_translator = i18n_noop
+# End i18n
 %endif
+
+class ${class_name}:
+    def __init__(self, master=None):
+        %if with_i18n_support:
+        _ = i18n_translator  # i18n string marker.
+        %endif
         # build ui
 ${widget_code}
         # Main widget
         self.mainwindow = ${target_code_id}
 %if set_main_menu:
         # Main menu
         _main_menu = self.create_${main_menu_id}(self.mainwindow)
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/pygubu.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/pygubu200.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu200.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/property_invalid.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/property_invalid.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/pygubu.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/pygubu200.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu200.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png` & `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -40,32 +40,26 @@
 
 msgid "C"
 msgstr "S"
 
 msgid "Class"
 msgstr "Klasse"
 
-msgid "Class Name:"
-msgstr "Klassenname:"
-
 msgid "Close"
 msgstr "Schließen"
 
 msgid "Close Toplevel previews"
 msgstr "Toplevel-Vorschauen schließen"
 
 msgid "Copy"
 msgstr "Kopieren"
 
 msgid "Custom Widgets"
 msgstr "Benutzerdefinierte Steuerelemente"
 
-msgid "Custom Widgets Builders"
-msgstr "Builders für benutzerdefinierte Steuerelemente"
-
 msgid "Cut"
 msgstr "Ausschneiden"
 
 msgid "Delete items"
 msgstr "Elemente löschen"
 
 msgid "Delete selected items?"
@@ -79,17 +73,14 @@
 
 msgid "File"
 msgstr "Datei"
 
 msgid "General"
 msgstr "Allgemein"
 
-msgid "Generate"
-msgstr "Generieren"
-
 msgid "Help"
 msgstr "Hilfe"
 
 msgid "Item delete"
 msgstr "Element löschen"
 
 msgid "Item down"
@@ -154,17 +145,14 @@
 
 msgid "Quit …"
 msgstr "Beenden …"
 
 msgid "R"
 msgstr "Z"
 
-msgid "Requires restart."
-msgstr "Erfordert Neustart."
-
 msgid "Save"
 msgstr "Speichern"
 
 msgid "Save as …"
 msgstr "Speichern als …"
 
 msgid "Sequence descriptor"
@@ -172,17 +160,14 @@
 
 msgid "Widget grid"
 msgstr "Steuerelementraster"
 
 msgid "Widget tree"
 msgstr "Steuerelementbaum"
 
-msgid "modules"
-msgstr "Module"
-
 msgid "pygubu"
 msgstr "pygubu"
 
 msgid "pygubu ui"
 msgstr "pygubu ui"
 
 msgid "ttk theme"
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygubu 0.7\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-06-27 00:02-0300\n"
+"PO-Revision-Date: 2024-04-14 20:06-0300\n"
 "Last-Translator: Alejandro Autalán <alejandroautalan@gmail.com>\n"
 "Language-Team: \n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 3.2.2\n"
@@ -44,14 +44,17 @@
 
 msgid "Add"
 msgstr "Agregar"
 
 msgid "Add i18n support"
 msgstr "Agregar soporte i18n"
 
+msgid "Add window centering code"
+msgstr "Agregar código de centrado de ventana"
+
 msgid "All"
 msgstr "Todos"
 
 msgid "All Files"
 msgstr "Todos los archivos"
 
 msgid "All IDs as class attributes"
@@ -74,22 +77,19 @@
 
 msgid "Applying ttk style definitions"
 msgstr "Aplicando definiciones de estilos ttk"
 
 msgid "Associated program:"
 msgstr "Programa asociado:"
 
-msgid "Automatically generate code"
-msgstr "Generar código automáticamente"
-
 msgid "Bindings"
 msgstr "Bindings"
 
-msgid "Browse …"
-msgstr "Buscar …"
+msgid "Builder output:"
+msgstr "Directorio del módulo constructor:"
 
 msgid "C"
 msgstr "C"
 
 msgid "Callback:"
 msgstr "Callback:"
 
@@ -107,15 +107,15 @@
 
 msgid "Checking main window visibility."
 msgstr "Verificando visibilidad de la ventana principal."
 
 msgid "Class"
 msgstr "Clase"
 
-msgid "Class Name:"
+msgid "Class name:"
 msgstr "Nombre de la clase:"
 
 msgid "Clear"
 msgstr "Limpiar lista"
 
 msgid "Clear all"
 msgstr "Limpiar todo"
@@ -131,40 +131,37 @@
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Code Script"
 msgstr "Script de codigo"
 
-msgid "Code copied"
-msgstr "Se copió al portapapeles"
-
 msgid "Column index: {0}"
 msgstr "Columna: {0}"
 
 msgid "Column {0} options"
 msgstr "Opciones para columna '{0}'"
 
+msgid "Components"
+msgstr "Componentes"
+
+msgid "Components Palette"
+msgstr "Paleta de componentes"
+
 msgid ""
 "Configuration file at {CONFIG_FILE!s} is corrupted, program may not work as "
 "expected.If you delete this file, configuration will be set to default"
 msgstr ""
 "El archivo de configuración ' {CONFIG_FILE!s}' esta roto, el programa puede "
 "no funcionar como se esperaba.\n"
 "Si elimina este archivo, se iniciará con los ajustes predeterminados"
 
 msgid "Copy"
 msgstr "Copiar"
 
-msgid "Copy to Clipboard"
-msgstr "Copiar al portapapeles"
-
-msgid "Create New …"
-msgstr "Crear Nuevo …"
-
 msgid "Create a base class for your custom widget."
 msgstr "Crear un clase base para su widget personalizado."
 
 msgid "Create a coded version of the UI definition."
 msgstr "Crear un versión en codigo del archivo UI actual."
 
 msgid "Create a pygubu application script using the UI definition."
@@ -172,31 +169,28 @@
 
 msgid "Custom Widget"
 msgstr "Widget Personalizado"
 
 msgid "Custom Widgets"
 msgstr "Widgets Personalizados"
 
-msgid "Custom Widgets Builders"
-msgstr "Constructores Personalizados"
-
 msgid "Cut"
 msgstr "Cortar"
 
 msgid "Delete"
 msgstr "Eliminar"
 
 msgid "Delete items"
 msgstr "Borrar items"
 
 msgid "Delete selected items?"
 msgstr "¿ Borrar items seleccionados ?"
 
-msgid "Design"
-msgstr "Diseño"
+msgid "Description:"
+msgstr "Descripción:"
 
 msgid "Detail"
 msgstr "Detalle"
 
 msgid "Do you want to save the changes before closing?"
 msgstr "¿Quieres guardar los cambios antes de cerrar?"
 
@@ -230,17 +224,14 @@
 msgid ""
 "Faild to parse config file at {CONFIG_FILE!s}, program may not work as "
 "expected."
 msgstr ""
 "Fallo al leer el archivo de configuración '{CONFIG_FILE!s}', el programa "
 "puede no funcionar como se espera."
 
-msgid "Failed to load custom widget module: '{path}'"
-msgstr "Error al cargar modulo de widget personalizado: '{path}'"
-
 msgid "Failed to load widget module: '{_module}'"
 msgstr "Error al cargar modulo de widget: '{_module}'"
 
 msgid "File"
 msgstr "Archivo"
 
 msgid ""
@@ -257,35 +248,29 @@
 
 msgid "GPL3"
 msgstr "GPL3"
 
 msgid "General"
 msgstr "General"
 
-msgid "General preferences"
-msgstr "Preferencias Generales"
-
-msgid "Generate"
-msgstr "Generar"
+msgid "Generate code"
+msgstr "Generar código"
 
 msgid "Go to parent"
 msgstr "Ir al padre"
 
 msgid "Grid"
 msgstr "Grid"
 
 msgid "Grid Row / Column options"
 msgstr "Opciones para columna '{0}'"
 
 msgid "Help"
 msgstr "Ayuda"
 
-msgid "Hidden options"
-msgstr "Opciones ocultas"
-
 msgid "ID"
 msgstr "ID"
 
 msgid "If you don't save the document, all the changes will be lost."
 msgstr "Si no guarda el documento, todos los cambios se perderán."
 
 msgid "Import Tk Variables"
@@ -332,14 +317,23 @@
 
 msgid "Message"
 msgstr "Mensaje"
 
 msgid "Messages"
 msgstr "Mensajes"
 
+msgid "Module name:"
+msgstr "Nombre del módulo:"
+
+msgid "Module output:"
+msgstr "Directorio del módulo:"
+
+msgid "Modules"
+msgstr "Módulos"
+
 msgid "More info."
 msgstr "Más info."
 
 msgid "Move down"
 msgstr "Mover abajo"
 
 msgid "Move left"
@@ -347,14 +341,17 @@
 
 msgid "Move right"
 msgstr "Mover derecha"
 
 msgid "Move up"
 msgstr "Mover arriba"
 
+msgid "Name:"
+msgstr "Nombre:"
+
 msgid "New"
 msgstr "Nuevo"
 
 msgid "No item selected."
 msgstr "No selecciono item."
 
 msgid "No separator (e.g. button1)"
@@ -374,26 +371,26 @@
 
 msgid "Ok"
 msgstr "Aceptar"
 
 msgid "Only {0} children allowed for {1}"
 msgstr "Solo se permiten {0} hijos para {1}"
 
+msgid "Open a project first."
+msgstr "Abre un proyecto primero."
+
 msgid "Open recent …"
 msgstr "Abrir reciente …"
 
 msgid "Open …"
 msgstr "Abrir …"
 
 msgid "Options for {0} container"
 msgstr "Opciones para contenedor {0}"
 
-msgid "Options:"
-msgstr "Opciones:"
-
 msgid "Pack"
 msgstr "Pack"
 
 msgid "Paste"
 msgstr "Pegar"
 
 msgid "Place"
@@ -413,50 +410,59 @@
 
 msgid "Preview"
 msgstr "Previsualización"
 
 msgid "Preview in Toplevel"
 msgstr "Previsualizar en ventana"
 
+msgid "Project"
+msgstr "Proyecto"
+
+msgid "Project Tree"
+msgstr "Árbol del proyecto"
+
+msgid "Project code generated."
+msgstr "Código del proyecto generado."
+
 msgid "Project saved to %s"
 msgstr "Proyecto guardado a %s"
 
+msgid "Project widget builders:"
+msgstr "Constructores personalizados:"
+
 msgid "Properties"
 msgstr "Propiedades"
 
 msgid "Pygubu Designer"
 msgstr "Pygubu Designer"
 
 msgid "Pygubu Preferences"
 msgstr "Preferencias"
 
 msgid "Pygubu wiki"
 msgstr "Wiki de pygubu"
 
-msgid "Python Script"
-msgstr "Python Script"
-
 msgid "Python module"
 msgstr "Módulo python"
 
 msgid "Quit …"
 msgstr "Salir …"
 
 msgid "R"
 msgstr "F"
 
+msgid "Regenerate code when saving the project"
+msgstr "Regenerar el código al guardar el proyecto"
+
 msgid "Remove"
 msgstr "Remover"
 
 msgid "Request new ID and set widget as nameless."
 msgstr "Solicitar nuevo ID y establecer el widget como \"sin  nombre\"."
 
-msgid "Requires restart."
-msgstr "Es necesario reiniciar el programa."
-
 msgid ""
 "Restart Pygubu Designer for\n"
 "changes to take effect."
 msgstr "Reinicia Pygubu Designer para que los cambios tengan efecto."
 
 msgid "Row index: {0}"
 msgstr "Fila: {0}"
@@ -475,39 +481,51 @@
 
 msgid "SaveIcon"
 msgstr "IconoGuardar"
 
 msgid "Script Generator"
 msgstr "Generador de Script"
 
+msgid "Select a valid choice."
+msgstr "Seleccione una opción válida."
+
+msgid "Select a widget builder file"
+msgstr "Seleccione un archivo constructor"
+
 msgid "Select all"
 msgstr "Seleccionar todo"
 
+msgid "Select output directory"
+msgstr "Seleccione directorio de salida"
+
+msgid "Select style definitions file"
+msgstr "Seleccione archivo de definición de estilos"
+
 msgid "Select template"
 msgstr "Seleccione plantilla"
 
 msgid "Select widget"
 msgstr "Seleccione widget"
 
 msgid "Send widget ID"
 msgstr "Enviar widget ID"
 
 msgid "Sequence descriptor"
 msgstr "Descriptor de secuencia"
 
+msgid "Settings"
+msgstr "Ajustes"
+
 msgid "Simple"
 msgstr "Simple"
 
-msgid "Single section widgets toolbar (requires restart)"
-msgstr "Paleta de widgets de selección única (requiere reiniciar)"
-
 msgid "Specifies the current value of the widget."
 msgstr "El valor nuevo/actual del widget."
 
-msgid "Style Definition File:"
+msgid "Style definition file:"
 msgstr "Archivo de definición de estilos:"
 
 msgid "Styles"
 msgstr "Estilos"
 
 msgid "Template description here."
 msgstr "Descripción de la plantilla AQUI."
@@ -523,35 +541,35 @@
 
 msgid "The name of the entry widget."
 msgstr "El nombre del widget entry."
 
 msgid "The new/current value of the entry."
 msgstr "El valor nuevo/actual del entry."
 
+msgid "The path must exist."
+msgstr "La ruta debe existir."
+
 msgid "The text string being inserted/deleted."
 msgstr "La cadena de texto que se inserta/elimina."
 
 msgid "The validation condition that triggered the callback."
 msgstr "La condición de validación que originó la llamada."
 
 msgid "This does not affect previously generated names."
 msgstr "Esto no afecta los nombres generados previamente."
 
 msgid "This program:"
 msgstr "Este programa:"
 
+msgid "This value should be a valid python identifier."
+msgstr "Este valor debe ser un identificador de python válido."
+
 msgid "Tk image formats"
 msgstr "Formatos de imagen Tk"
 
-msgid "Tree"
-msgstr "Arbol"
-
-msgid "Ttk Styles"
-msgstr "Estilos ttk"
-
 msgid "Type of action."
 msgstr "Tipo de acción."
 
 msgid "Uppercase first letter (e.g. Button…)"
 msgstr "Primera letra en mayúscula (ej. Button1)"
 
 msgid "Use \"_\" as separator (e.g. button_1)"
@@ -568,26 +586,17 @@
 
 msgid "Widget naming"
 msgstr "Nombre de widgets"
 
 msgid "Widget tree"
 msgstr "Arbol de widgets"
 
-msgid "Window geometry:"
-msgstr "Geometría de la ventana:"
-
-msgid "modules"
-msgstr "módulos"
-
 msgid "newproject"
 msgstr "nuevo_proyecto"
 
-msgid "on property change"
-msgstr "al cambiar una propiedad"
-
 msgid "pygubu"
 msgstr "pygubu"
 
 msgid "pygubu ui"
 msgstr "archivos de pygubu"
 
 msgid "pygubu-designer"
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/pygubu-designer.pot` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu-designer.pot`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: pygubudesigner\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-26 23:52-0300\n"
+"POT-Creation-Date: 2024-04-14 19:58-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -73,42 +73,42 @@
 msgstr ""
 
 #: src/pygubudesigner/data/ui/about_dialog.ui:261
 msgid "Close"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:7
-#: src/pygubudesigner/main.py:614
+#: src/pygubudesigner/main.py:585
 msgid "Save Changes"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:36
+#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:37
 msgid "SaveIcon"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:59
+#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:58
 msgid "Message"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:70
+#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:68
 msgid "Detail"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:98
 msgid "Don't Save"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:114
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:558
+#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:112
+#: src/pygubudesigner/data/ui/designer_settings.ui:248
+#: src/pygubudesigner/data/ui/project_settings.ui:748
 msgid "Cancel"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:129
+#: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:125
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:46
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:1096
 msgid "Save"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/container_layout_editor_base.ui:25
 #: src/pygubudesigner/containerlayouteditor.py:42
 #, python-brace-format
 msgid "Options for {0} container"
@@ -130,129 +130,191 @@
 msgid "Row {0} options"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/container_layout_editor_base.ui:212
 msgid "Column {0} options"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:9
+#: src/pygubudesigner/data/ui/designer_settings.ui:9
 msgid "Pygubu Preferences"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:34
+#: src/pygubudesigner/data/ui/designer_settings.ui:42
+#: src/pygubudesigner/data/ui/project_settings.ui:64
 msgid "General"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:50
-msgid "General preferences"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:66
+#: src/pygubudesigner/data/ui/designer_settings.ui:68
 msgid "Preferred widget set:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:85
+#: src/pygubudesigner/data/ui/designer_settings.ui:88
 msgid "Preferred ttk theme:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:106
+#: src/pygubudesigner/data/ui/designer_settings.ui:108
 msgid "Preferred layout manager:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:129
+#: src/pygubudesigner/data/ui/designer_settings.ui:130
 msgid "Center toplevel preview window"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:143
-msgid "Automatically generate code"
+#: src/pygubudesigner/data/ui/designer_settings.ui:152
+msgid "Widget naming"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:157
-msgid "on property change"
+#: src/pygubudesigner/data/ui/designer_settings.ui:176
+msgid "Separator:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:171
-msgid "Single section widgets toolbar (requires restart)"
+#: src/pygubudesigner/data/ui/designer_settings.ui:198
+msgid "Uppercase first letter (e.g. Button…)"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:187
-msgid "Widget naming"
+#: src/pygubudesigner/data/ui/designer_settings.ui:212
+msgid "This does not affect previously generated names."
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:200
-msgid "No separator (e.g. button1)"
+#: src/pygubudesigner/data/ui/designer_settings.ui:230
+msgid "Widget"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:212
-msgid "Use \"_\" as separator (e.g. button_1)"
+#: src/pygubudesigner/data/ui/designer_settings.ui:260
+#: src/pygubudesigner/data/ui/messagebox.ui:64
+#: src/pygubudesigner/data/ui/project_settings.ui:758
+msgid "Ok"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:226
-msgid "Uppercase first letter (e.g. Button…)"
+#: src/pygubudesigner/data/ui/messagebox.ui:8
+msgid "Dialog"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:238
-msgid "This does not affect previously generated names."
+#: src/pygubudesigner/data/ui/project_settings.ui:78
+msgid "Name:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:253
-msgid "Hidden options"
+#: src/pygubudesigner/data/ui/project_settings.ui:111
+msgid "Description:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:265
-msgid "Window geometry:"
+#: src/pygubudesigner/data/ui/project_settings.ui:158
+msgid "Code"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:291
-msgid "Custom Widgets"
+#: src/pygubudesigner/data/ui/project_settings.ui:182
+msgid "Module name:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:319
-msgid "Custom Widgets Builders"
+#: src/pygubudesigner/data/ui/project_settings.ui:214
+msgid "Template:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:351
-msgid "modules"
+#: src/pygubudesigner/data/ui/project_settings.ui:237
+msgid "Template description here."
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:380
-msgid "Requires restart."
+#: src/pygubudesigner/data/ui/project_settings.ui:249
+msgid "Main widget:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:392
-msgid "-"
+#: src/pygubudesigner/data/ui/project_settings.ui:282
+msgid "Class name:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:405
-msgid "+"
+#: src/pygubudesigner/data/ui/project_settings.ui:313
+msgid "Main menu:"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:346
+msgid "Module output:"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:377
+#: src/pygubudesigner/data/ui/project_settings.ui:434
+#: src/pygubudesigner/data/ui/project_settings.ui:577
+msgid "…"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:378
+#: src/pygubudesigner/data/ui/project_settings.ui:435
+msgid "Select output directory"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:426
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:453
-msgid "Ttk Styles"
+#: src/pygubudesigner/data/ui/project_settings.ui:403
+msgid "Builder output:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:478
-msgid "Style Definition File:"
+#: src/pygubudesigner/data/ui/project_settings.ui:471
+msgid "Import Tk Variables"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:511
-msgid "Browse …"
+#: src/pygubudesigner/data/ui/project_settings.ui:481
+msgid "Use ttk style definitions file"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:521
+#: src/pygubudesigner/data/ui/project_settings.ui:491
+msgid "Add i18n support"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:501
+msgid "All IDs as class attributes"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:511
+msgid "Regenerate code when saving the project"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:521
+msgid "Add window centering code"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:538
+#: src/pygubudesigner/services/projectsettings.py:286
+#: src/pygubudesigner/services/projectsettings.py:306
+#: src/pygubudesigner/services/projectsettings.py:316
+msgid "Styles"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:547
+msgid "Style definition file:"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:578
+#: src/pygubudesigner/data/ui/project_settings.ui:593
+msgid "Select style definitions file"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:592
+#: src/pygubudesigner/data/ui/project_settings.ui:705
+msgid "+"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:617
 msgid "Remove"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:531
-msgid "Create New …"
+#: src/pygubudesigner/data/ui/project_settings.ui:643
+msgid "Custom Widgets"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/preferences_dialog.ui:570
-msgid "Ok"
+#: src/pygubudesigner/data/ui/project_settings.ui:654
+msgid "Project widget builders:"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:683
+msgid "Modules"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:706
+msgid "Select a widget builder file"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/project_settings.ui:719
+msgid "-"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:7
 msgid "File"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:14
@@ -271,39 +333,39 @@
 msgid "Clear list"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:52
 msgid "Save as …"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:62 src/pygubudesigner/main.py:178
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:62 src/pygubudesigner/main.py:180
 msgid "Quit …"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:69
 msgid "Edit"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:76
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:238
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:260
 msgid "Copy"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:83
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:244
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:266
 msgid "Paste"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:90
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:250
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:272
 msgid "Cut"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:97
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:265
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:287
 msgid "Duplicate"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:105
 msgid "Widget tree"
 msgstr ""
 
@@ -340,231 +402,163 @@
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:172
 msgid "Preferences"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/pygubu-ui.ui:179
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:506
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:1032
+msgid "Project"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:185
+msgid "Settings"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:194
+msgid "Generate code"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:201
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:651
 msgid "Preview"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:186
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:208
 msgid "Preview in Toplevel"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:193
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:215
 msgid "Close Toplevel previews"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:198
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:220
 msgid "ttk theme"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:206
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:228
 msgid "Help"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:212
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:234
 msgid "Pygubu wiki"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:218
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:240
 msgid "About Pygubu"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:229
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:251
 msgid "Go to parent"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:256
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:278
 msgid "Delete"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:273
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:296 src/pygubudesigner/main.py:150
 msgid "Pygubu Designer"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:314
-msgid "Design"
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:339
+msgid "Components Palette"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:356
-msgid "Tree"
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:360
+msgid "Project Tree"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:376
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:381
+#: src/pygubudesigner/data/ui/treecomponent_palette.ui:25
+#: src/pygubudesigner/services/widgets/treecomponentpaletteui.py:29
 msgid "Filter:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:397
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:403
 msgid "✖"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:427
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:432
 msgid "ID"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:439
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:444
 msgid "Class"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:451
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:456
 msgid "R"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:463
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:468
 msgid "C"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:475
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:480
 msgid " "
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:556
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:496
 msgid "Properties"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:578
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:521
 msgid "Appearance"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:597
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:540
 msgid "Layout"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:615
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:558
 msgid "Bindings"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:649
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:592
 msgid "Sequence descriptor"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:661
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:604
 msgid "Event Handler"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:673
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:616
 msgid "Add"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:713
-msgid "Code"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:733
-msgid "Template description here."
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:745
-msgid "Template:"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:756
-msgid "Application"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:778
-msgid "Code Script"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:800
-msgid "Custom Widget"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:835
-msgid "Options:"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:869
-msgid "Main widget:"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:892
-msgid "Class Name:"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:923
-msgid "Main menu:"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:958
-msgid "Import Tk Variables"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:969
-msgid "Use ttk style definitions file"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:980
-msgid "Add i18n support"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:991
-msgid "All IDs as class attributes"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:1076
-msgid "Generate"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:1086
-msgid "Copy to Clipboard"
-msgstr ""
-
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:1178
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:755
 msgid "Messages"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:72
-msgid "Script Generator"
+#: src/pygubudesigner/data/ui/treecomponent_palette.ui:73
+#: src/pygubudesigner/services/widgets/treecomponentpaletteui.py:52
+msgid "tk"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:76
-msgid "Create a pygubu application script using the UI definition."
-msgstr ""
-
-#: src/pygubudesigner/codegen/scriptgenerator.py:78
-msgid "Create a coded version of the UI definition."
+#: src/pygubudesigner/data/ui/treecomponent_palette.ui:116
+#: src/pygubudesigner/services/widgets/treecomponentpaletteui.py:75
+msgid "Components"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:79
-msgid "Create a base class for your custom widget."
-msgstr ""
-
-#: src/pygubudesigner/codegen/scriptgenerator.py:220
-msgid "Code copied"
-msgstr ""
-
-#: src/pygubudesigner/codegen/scriptgenerator.py:261
-msgid "Python Script"
-msgstr ""
-
-#: src/pygubudesigner/codegen/scriptgenerator.py:261
-#: src/pygubudesigner/main.py:657 src/pygubudesigner/main.py:702
-#: src/pygubudesigner/preferences.py:308 src/pygubudesigner/preferences.py:341
-#: src/pygubudesigner/preferences.py:391
-msgid "All"
+#: src/pygubudesigner/codegen/scriptgenerator.py:43
+msgid "Script Generator"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:306
+#: src/pygubudesigner/codegen/scriptgenerator.py:311
 msgid "Select widget"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:312
+#: src/pygubudesigner/codegen/scriptgenerator.py:317
 msgid "Select template"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:318
+#: src/pygubudesigner/codegen/scriptgenerator.py:323
 msgid "Enter classname"
 msgstr ""
 
-#: src/pygubudesigner/codegen/scriptgenerator.py:325
+#: src/pygubudesigner/codegen/scriptgenerator.py:330
 msgid "Invalid classname"
 msgstr ""
 
 #: src/pygubudesigner/containerlayouteditor.py:43
 #, python-brace-format
 msgid "Row index: {0}"
 msgstr ""
@@ -599,110 +593,91 @@
 msgid "Change manager from {0} to {1}?"
 msgstr ""
 
 #: src/pygubudesigner/layouteditor.py:180
 msgid "All container widgets will be updated."
 msgstr ""
 
-#: src/pygubudesigner/main.py:73
+#: src/pygubudesigner/main.py:84
 #, python-brace-format
 msgid "Failed to load widget module: '{_module}'"
 msgstr ""
 
-#: src/pygubudesigner/main.py:74 src/pygubudesigner/main.py:94
-#: src/pygubudesigner/main.py:650 src/pygubudesigner/main.py:689
-#: src/pygubudesigner/preferences.py:102 src/pygubudesigner/preferences.py:108
+#: src/pygubudesigner/main.py:86 src/pygubudesigner/main.py:627
+#: src/pygubudesigner/main.py:676 src/pygubudesigner/main.py:921
+#: src/pygubudesigner/preferences.py:106 src/pygubudesigner/preferences.py:112
 msgid "Error"
 msgstr ""
 
-#: src/pygubudesigner/main.py:93
-#, python-brace-format
-msgid "Failed to load custom widget module: '{path}'"
-msgstr ""
-
-#: src/pygubudesigner/main.py:578
+#: src/pygubudesigner/main.py:548
 msgid "Checking main window visibility."
 msgstr ""
 
-#: src/pygubudesigner/main.py:580
+#: src/pygubudesigner/main.py:550
 msgid "Main window is not visible in current monitors."
 msgstr ""
 
-#: src/pygubudesigner/main.py:584
+#: src/pygubudesigner/main.py:554
 msgid "Main window position fixed."
 msgstr ""
 
-#: src/pygubudesigner/main.py:617
+#: src/pygubudesigner/main.py:588
 msgid "If you don't save the document, all the changes will be lost."
 msgstr ""
 
-#: src/pygubudesigner/main.py:631
+#: src/pygubudesigner/main.py:602
 msgid "Do you want to save the changes before closing?"
 msgstr ""
 
-#: src/pygubudesigner/main.py:647
+#: src/pygubudesigner/main.py:618
 #, python-format
 msgid "Project saved to %s"
 msgstr ""
 
-#: src/pygubudesigner/main.py:657 src/pygubudesigner/main.py:701
+#: src/pygubudesigner/main.py:637 src/pygubudesigner/main.py:688
 msgid "pygubu ui"
 msgstr ""
 
-#: src/pygubudesigner/main.py:694
+#: src/pygubudesigner/main.py:637 src/pygubudesigner/main.py:689
+#: src/pygubudesigner/services/projectsettings.py:33
+msgid "All"
+msgstr ""
+
+#: src/pygubudesigner/main.py:681
 msgid "Do you want to save the changes before opening?"
 msgstr ""
 
-#: src/pygubudesigner/main.py:712
+#: src/pygubudesigner/main.py:699
 msgid "Do you want to save the changes before creating?"
 msgstr ""
 
-#: src/pygubudesigner/main.py:888
+#: src/pygubudesigner/main.py:840
+msgid "Open a project first."
+msgstr ""
+
+#: src/pygubudesigner/main.py:866
+msgid "Project code generated."
+msgstr ""
+
+#: src/pygubudesigner/main.py:881
 msgid "newproject"
 msgstr ""
 
-#: src/pygubudesigner/preferences.py:99
+#: src/pygubudesigner/preferences.py:103
 msgid ""
 "Configuration file at {CONFIG_FILE!s} is corrupted, program may not work as "
 "expected.If you delete this file, configuration will be set to default"
 msgstr ""
 
-#: src/pygubudesigner/preferences.py:106
+#: src/pygubudesigner/preferences.py:110
 msgid ""
 "Faild to parse config file at {CONFIG_FILE!s}, program may not work as "
 "expected."
 msgstr ""
 
-#: src/pygubudesigner/preferences.py:308 src/pygubudesigner/preferences.py:341
-#: src/pygubudesigner/preferences.py:391
-msgid "Python module"
-msgstr ""
-
-#: src/pygubudesigner/preferences.py:323
-msgid ""
-"File saved.\n"
-"\n"
-"Please edit the style definition file."
-msgstr ""
-
-#: src/pygubudesigner/preferences.py:324 src/pygubudesigner/preferences.py:331
-#: src/pygubudesigner/preferences.py:362
-msgid "Styles"
-msgstr ""
-
-#: src/pygubudesigner/preferences.py:330
-msgid "Error saving template file."
-msgstr ""
-
-#: src/pygubudesigner/preferences.py:361
-msgid ""
-"Restart Pygubu Designer for\n"
-"changes to take effect."
-msgstr ""
-
 #: src/pygubudesigner/properties/propertieshelp.py:5
 msgid "Object class name."
 msgstr ""
 
 #: src/pygubudesigner/properties/propertieshelp.py:6
 msgid "Object unique identifier."
 msgstr ""
@@ -1826,61 +1801,126 @@
 
 #: src/pygubudesigner/properties/propertieshelp.py:559
 msgid ""
 "When a non-empty value is supplied, places the row in a uniform group with "
 "other rows that have the same value for uniform."
 msgstr ""
 
-#: src/pygubudesigner/stylehandler.py:79
+#: src/pygubudesigner/services/designersettings.py:32
+msgid "No separator (e.g. button1)"
+msgstr ""
+
+#: src/pygubudesigner/services/designersettings.py:33
+msgid "Use \"_\" as separator (e.g. button_1)"
+msgstr ""
+
+#: src/pygubudesigner/services/fieldvalidator.py:10
+msgid "This value should be a valid python identifier."
+msgstr ""
+
+#: src/pygubudesigner/services/fieldvalidator.py:35
+msgid "Select a valid choice."
+msgstr ""
+
+#: src/pygubudesigner/services/fieldvalidator.py:60
+msgid "The path must exist."
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:33
+msgid "Python module"
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:55
+msgid "Create a pygubu application script using the UI definition."
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:57
+msgid "Create a coded version of the UI definition."
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:58
+msgid "Create a base class for your custom widget."
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:61
+msgid "Application"
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:62
+msgid "Code Script"
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:63
+msgid "Custom Widget"
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:285
+msgid ""
+"Restart Pygubu Designer for\n"
+"changes to take effect."
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:304
+msgid ""
+"File saved.\n"
+"\n"
+"Please edit the style definition file."
+msgstr ""
+
+#: src/pygubudesigner/services/projectsettings.py:315
+msgid "Error saving template file."
+msgstr ""
+
+#: src/pygubudesigner/services/stylehandler.py:78
 msgid "Applying ttk style definitions"
 msgstr ""
 
-#: src/pygubudesigner/stylehandler.py:101
+#: src/pygubudesigner/services/stylehandler.py:101
 #, python-format
 msgid "ttk style definition error: %s"
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:173
+#: src/pygubudesigner/uitreeeditor.py:221
 msgid "Delete items"
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:174
+#: src/pygubudesigner/uitreeeditor.py:222
 msgid "Delete selected items?"
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:463
+#: src/pygubudesigner/uitreeeditor.py:518
 msgid "No item selected."
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:701
+#: src/pygubudesigner/uitreeeditor.py:758
 #, python-format
 msgid "Allowed children: %s."
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:711
+#: src/pygubudesigner/uitreeeditor.py:768
 #, python-brace-format
 msgid "Only {0} children allowed for {1}"
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:726
+#: src/pygubudesigner/uitreeeditor.py:784
 #, python-brace-format
 msgid "{0} not allowed as parent of {1}"
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:736
+#: src/pygubudesigner/uitreeeditor.py:794
 #, python-format
 msgid "Not allowed, %s is not a container."
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:748
+#: src/pygubudesigner/uitreeeditor.py:806
 #, python-format
 msgid "%s not allowed at root level"
 msgstr ""
 
-#: src/pygubudesigner/uitreeeditor.py:758
+#: src/pygubudesigner/uitreeeditor.py:816
 #, python-format
 msgid "Not allowed at root level, %s is not a container."
 msgstr ""
 
 #: src/pygubudesigner/widgets/commandentry.py:103
 msgid "Callback:"
 msgstr ""
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/pygubu.pot` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,592 +4,629 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: pygubu\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-26 23:52-0300\n"
+"POT-Creation-Date: 2024-04-14 19:58-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/__init__.py:6
-msgid "tkcalendar"
+#: ../pygubu/src/pygubu/forms/validation/constraint/form.py:8
+msgid "This value is required."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:72
-msgid "intinitially displayed year, default is current year."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:22
+msgid "button color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:77
-msgid "initially displayed month, default is current month."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:25
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:63
+msgid "text color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:86
-msgid "first day of the week"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:61
+msgid "background color \"should match parent bg\""
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:92
-msgid "minimum allowed date (string with format yyyy-mm-dd)"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:68
+msgid "indicator ring background \"fill color\""
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:97
-msgid "maximum allowed date (string with format yyyy-mm-dd)"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:74
+msgid "indicator outline / ring color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:105
-msgid "whether to display week numbers"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:77
+msgid "check mark color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:115
-msgid ""
-"whether to display the last days of the previous month and the first of the "
-"next month."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:30
+msgid "color of frame"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:132
-msgid "date pattern used to format the date as a string."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:76
+msgid "use vertical scrollbar"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:143
-msgid "connect the currently selected date to the variable."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:85
+msgid "use horizontal scrollbar"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:175
-msgid "tooltip opacity between 0 and 1"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:94
+msgid "auto scroll to bottom if new items added to frame"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:181
-msgid "delay in ms before displaying the tooltip"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:98
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:55
+msgid "background color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/widgets.py:308
-msgid ""
-"Specifies the list of values to display. In code you can pass any iterable. "
-"In Designer, a json like list: [\"item1\", \"item2\"]"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:102
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:96
+msgid "color of scrollbars' slider"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/tabview.py:94
-msgid "The 'name' argument of method: CTkTabview.add(self, name: str)"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:109
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:102
+msgid "color of scrollbars' trough, default to frame's background"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/__init__.py:6
-msgid "CustomTkinter"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:116
+#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:123
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:108
+msgid "vertical scrollbar width"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/ctkbase.py:133
-msgid "Color behind the widget if it has rounded corners."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/__init__.py:5
+msgid "AwesomeTkinter"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/ctkbase.py:159
-msgid "Main color of the widget."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/label.py:41
+msgid "milliseconds"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/ctkbase.py:232
-msgid "Default color theme."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:48
+msgid "color of base ring"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/windows.py:104
-msgid "Set the maximum window size."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:54
+msgid "color of indicator ring"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/customtkinter/windows.py:105
-msgid "Set the minimum window size."
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:60
+msgid "percentage text color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:63
-msgid "width of the canvas in pixels"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:66
+msgid "tkinter font for percentage text"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:69
-msgid "height of the canvas in pixels"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:76
+msgid ""
+"font size to progressbar width ratio, e.g. for a progressbar size 100 "
+"pixels, a 0.1 ratio means font size 10"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:76
-msgid ""
-"callback for when an item is created, with args: (int item, int rectangle)"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:83
+msgid "base image for progressbar"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:84
-msgid ""
-"callback for when an item is deleted, with args: (int item, int rectangle)"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:89
+msgid "indicator image for progressbar"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:92
-msgid ""
-"callback for when an item is moved, with args: (int item, int rectangle, int "
-"x, int y)"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:95
+msgid "color of parent container"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:100
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:58
+msgid "foreground color"
+msgstr ""
+
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:61
+msgid "border width"
+msgstr ""
+
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:69
+msgid "include vertical scrollbar"
+msgstr ""
+
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:77
+msgid "include horizontal scrollbar"
+msgstr ""
+
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:85
+msgid "automatic vertical scrolling"
+msgstr ""
+
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:92
 msgid ""
-"user defined function for when an item is created, with arg (add_item).\n"
-"Where add_item is a function of this widget."
+"maximum characters allowed in Text widget, text will be truncated from the "
+"beginning to match the max chars"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:62
-msgid "side the scrollbar should be on"
+#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:114
+msgid "horizontal scrollbar width"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:124
-msgid "position of the toggle arrow compared to the text"
+#: ../pygubu/src/pygubu/plugins/customtkinter/ctkbase.py:210
+msgid "Color behind the widget if it has rounded corners."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:132
-msgid "width of the closed ToggledFrame (in characters)"
+#: ../pygubu/src/pygubu/plugins/customtkinter/ctkbase.py:220
+msgid "Main color of the widget."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:138
-msgid "text to display next to the toggle arrow"
+#: ../pygubu/src/pygubu/plugins/customtkinter/ctkbase.py:298
+msgid "Default color theme."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:42
-msgid "calendar locale (defines the language, date formatting)"
+#: ../pygubu/src/pygubu/plugins/customtkinter/__init__.py:6
+msgid "CustomTkinter"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:50
-msgid "first day of the week, 0 is monday"
+#: ../pygubu/src/pygubu/plugins/customtkinter/tabview.py:95
+msgid "The 'name' argument of method: CTkTabview.add(self, name: str)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:53
-msgid "year to display"
+#: ../pygubu/src/pygubu/plugins/customtkinter/widgets.py:323
+msgid ""
+"Specifies the list of values to display. In code you can pass any iterable. "
+"In Designer, a json like list: [\"item1\", \"item2\"]"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:61
-msgid "month to display"
+#: ../pygubu/src/pygubu/plugins/customtkinter/windows.py:104
+msgid "Set the maximum window size."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:67
-msgid "background color of the selected day"
+#: ../pygubu/src/pygubu/plugins/customtkinter/windows.py:105
+msgid "Set the minimum window size."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:73
-msgid "selectforeground color of the selected day"
+#: ../pygubu/src/pygubu/plugins/pygubu/accordionframe.py:27
+#: ../pygubu/src/pygubu/plugins/pygubu/accordionframe.py:71
+#: ../pygubu/src/pygubu/plugins/pygubu/calendarframe.py:41
+#: ../pygubu/src/pygubu/plugins/pygubu/colorinputbo.py:23
+#: ../pygubu/src/pygubu/plugins/pygubu/combobox.py:27
+#: ../pygubu/src/pygubu/plugins/pygubu/dialog.py:51
+#: ../pygubu/src/pygubu/plugins/pygubu/dockfw.py:32
+#: ../pygubu/src/pygubu/plugins/pygubu/dockfw.py:78
+#: ../pygubu/src/pygubu/plugins/pygubu/dockfw.py:132
+#: ../pygubu/src/pygubu/plugins/pygubu/editabletreeview.py:31
+#: ../pygubu/src/pygubu/plugins/pygubu/filterabletreeview.py:29
+#: ../pygubu/src/pygubu/plugins/pygubu/hideableframe.py:17
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:88
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:127
+#: ../pygubu/src/pygubu/plugins/pygubu/scrolledframe.py:71
+#: ../pygubu/src/pygubu/plugins/pygubu/tkscrolledframe.py:84
+msgid "Pygubu Widgets"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/tickscale.py:54
-msgid "increment by which the slider can be moved. 0 means continuous sliding."
+#: ../pygubu/src/pygubu/plugins/pygubu/combobox.py:31
+msgid ""
+"In designer: json list of key, value pairs\n"
+"    Example: [[\"A\", \"Option 1 Label\"], [\"B\", \"Option 2 Label\"]]\n"
+"In code: an iterable of key, value pairs"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/tickscale.py:61
-msgid "if not 0, display ticks with the given interval"
+#: ../pygubu/src/pygubu/plugins/pygubu/dialog.py:54
+msgid "Determines if dialog is run in normal or modal mode."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/tickscale.py:82
-msgid "if tickinterval is not 0, position of the ticks"
+#: ../pygubu/src/pygubu/plugins/pygubu/dockfw.py:85
+msgid "The weight value for the pane."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:27
-msgid "link to be opened"
+#: ../pygubu/src/pygubu/plugins/pygubu/dockfw.py:147
+msgid "The weight value of the widget in the pane"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:33
-msgid "text color when widget is created"
+#: ../pygubu/src/pygubu/plugins/pygubu/forms/base.py:7
+msgid "Pygubu Forms"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:39
-msgid "text color when hovering over the widget"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:36
+msgid "Dialog type"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:45
-msgid "text color when link is clicked"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:47
+msgid "Initial path value."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:67
-msgid "side the Entry must be on."
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:51
+msgid ""
+"Dialog option. Determines if path must exist for directory and file dialogs. "
+"The default value is True."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:76
-msgid "scale orientation"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:63
+msgid "Dialog option. Sets initial directory."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:84
-msgid "width of the Scale in pixels"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:66
+msgid "Dialog option. Sets dialog title."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:90
-msgid "width of the Entry in characters"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:69
+msgid "Dialog option. Sets default file extension."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:93
-msgid "start value of the scale"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:97
+msgid "Image for the button."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:96
-msgid "end value of the scale"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:100
+msgid "Tk variable associated to the path property."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:102
-msgid "space between the entry and the scale"
+#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:103
+msgid "Path entry state."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/__init__.py:5
-msgid "ttkwidgets"
+#: ../pygubu/src/pygubu/plugins/pygubu/scrollbarhelper.py:60
+#: ../pygubu/src/pygubu/plugins/pygubu/tkscrollbarhelper.py:76
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1439
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1484
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1529
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:501
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:567
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:669
+msgid "Pygubu Helpers"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:51
-msgid "initially selected alpha value (between 0 and 255)"
+#: ../pygubu/src/pygubu/plugins/pygubu/tkinterscrolledtext.py:17
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:187
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:271
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:320
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:380
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:439
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:480
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:578
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:669
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:700
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:745
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:778
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:854
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:896
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1544
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:69
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:89
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:112
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:136
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:177
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:193
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:204
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:230
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:252
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:274
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:289
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:369
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:478
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:709
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:745
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:774
+msgid "Control & Display"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:54
-msgid "gradient color"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:72
+msgid "intinitially displayed year, default is current year."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:60
-msgid "variable linked to the alpha value"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:77
+msgid "initially displayed month, default is current month."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:123
-msgid "hue (between 0 and 360) of the color square gradient"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:86
+msgid "first day of the week"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:126
-msgid "initially selected color"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:92
+msgid "minimum allowed date (string with format yyyy-mm-dd)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:168
-msgid "initially selected hue value (between 0 and 360)"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:97
+msgid "maximum allowed date (string with format yyyy-mm-dd)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:174
-msgid "variable linked to the hue value"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:105
+msgid "whether to display week numbers"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:44
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:171
-msgid "Values separated by space. In code you can pass a full list"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:115
+msgid ""
+"whether to display the last days of the previous month and the first of the "
+"next month."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:110
-msgid "font in entry and listbox"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:132
+msgid "date pattern used to format the date as a string."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:118
-msgid "whether the user is allowed to enter values not in the list"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:143
+msgid "connect the currently selected date to the variable."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:126
-msgid "whether to automatically export selected text to the clipboard"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:175
+msgid "tooltip opacity between 0 and 1"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:134
-msgid "text alignment in entry and listbox"
+#: ../pygubu/src/pygubu/plugins/tkcalendar/basecalendar.py:181
+msgid "delay in ms before displaying the tooltip"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:141
-msgid "Values separated by space. In code you can pass a full python list."
+#: ../pygubu/src/pygubu/plugins/tkcalendar/__init__.py:6
+msgid "tkcalendar"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:58
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:117
-msgid "name of the callback function with one argument: the font family name"
+#: ../pygubu/src/pygubu/plugins/tkintermapview/__init__.py:7
+msgid "TkinterMapView"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:156
-msgid ""
-"name of the callback function with arguments: (family: str, size: int, bold: "
-"bool, italic: bool, underline: bool)"
+#: ../pygubu/src/pygubu/plugins/tkintertable/__init__.py:7
+msgid "tkintertable"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:197
-msgid ""
-"name of the callback function with arguments: (bold: bool, italic: bool, "
-"underline: bool, overstrike: bool)"
+#: ../pygubu/src/pygubu/plugins/tkinterweb/__init__.py:6
+msgid "TkinterWeb"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:207
-msgid "Show/hide Header label"
+#: ../pygubu/src/pygubu/plugins/tksheet/__init__.py:6
+msgid "tksheet"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:213
-msgid "size of the font on the buttons"
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:65
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:120
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:150
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:220
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:611
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:43
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:307
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:324
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:338
+msgid "Containers"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:257
-msgid "name of the callback function on click with single argument: size: int"
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:668
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:990
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1335
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1348
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1372
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1395
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1413
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1529
+#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:368
+msgid "Menu"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/table.py:41
-msgid "whether columns are draggable"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:44
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:171
+msgid "Values separated by space. In code you can pass a full list"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/table.py:49
-msgid "whether rows are draggable"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:110
+msgid "font in entry and listbox"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttkwidgets/table.py:58
-msgid ""
-"whether columns are sortable by clicking on their headings. The sorting "
-"order depends on the type of data (str, float, ...) which can be set with "
-"the column method."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:118
+msgid "whether the user is allowed to enter values not in the list"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:30
-msgid "color of frame"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:126
+msgid "whether to automatically export selected text to the clipboard"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:76
-msgid "use vertical scrollbar"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:134
+msgid "text alignment in entry and listbox"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:85
-msgid "use horizontal scrollbar"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:141
+msgid "Values separated by space. In code you can pass a full python list."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:94
-msgid "auto scroll to bottom if new items added to frame"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:42
+msgid "calendar locale (defines the language, date formatting)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:98
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:55
-msgid "background color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:50
+msgid "first day of the week, 0 is monday"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:102
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:96
-msgid "color of scrollbars' slider"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:53
+msgid "year to display"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:109
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:102
-msgid "color of scrollbars' trough, default to frame's background"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:61
+msgid "month to display"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:116
-#: ../pygubu/src/pygubu/plugins/awesometkinter/frame.py:123
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:108
-msgid "vertical scrollbar width"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:67
+msgid "background color of the selected day"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/label.py:41
-msgid "milliseconds"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/calendar.py:73
+msgid "selectforeground color of the selected day"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/__init__.py:5
-msgid "AwesomeTkinter"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:51
+msgid "initially selected alpha value (between 0 and 255)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:58
-msgid "foreground color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:54
+msgid "gradient color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:61
-msgid "border width"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:60
+msgid "variable linked to the alpha value"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:69
-msgid "include vertical scrollbar"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:123
+msgid "hue (between 0 and 360) of the color square gradient"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:77
-msgid "include horizontal scrollbar"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:126
+msgid "initially selected color"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:85
-msgid "automatic vertical scrolling"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:168
+msgid "initially selected hue value (between 0 and 360)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:92
-msgid ""
-"maximum characters allowed in Text widget, text will be truncated from the "
-"beginning to match the max chars"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/color.py:174
+msgid "variable linked to the hue value"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/text.py:114
-msgid "horizontal scrollbar width"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:58
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:117
+msgid "name of the callback function with one argument: the font family name"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:22
-msgid "button color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:156
+msgid ""
+"name of the callback function with arguments: (family: str, size: int, bold: "
+"bool, italic: bool, underline: bool)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:25
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:63
-msgid "text color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:197
+msgid ""
+"name of the callback function with arguments: (bold: bool, italic: bool, "
+"underline: bool, overstrike: bool)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:61
-msgid "background color \"should match parent bg\""
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:207
+msgid "Show/hide Header label"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:68
-msgid "indicator ring background \"fill color\""
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:213
+msgid "size of the font on the buttons"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:74
-msgid "indicator outline / ring color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/font.py:257
+msgid "name of the callback function on click with single argument: size: int"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/button.py:77
-msgid "check mark color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:62
+msgid "side the scrollbar should be on"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:48
-msgid "color of base ring"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:124
+msgid "position of the toggle arrow compared to the text"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:54
-msgid "color of indicator ring"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:132
+msgid "width of the closed ToggledFrame (in characters)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:60
-msgid "percentage text color"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/frames.py:138
+msgid "text to display next to the toggle arrow"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:66
-msgid "tkinter font for percentage text"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/__init__.py:5
+msgid "ttkwidgets"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:76
-msgid ""
-"font size to progressbar width ratio, e.g. for a progressbar size 100 "
-"pixels, a 0.1 ratio means font size 10"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:63
+msgid "width of the canvas in pixels"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:83
-msgid "base image for progressbar"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:69
+msgid "height of the canvas in pixels"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:89
-msgid "indicator image for progressbar"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:76
+msgid ""
+"callback for when an item is created, with args: (int item, int rectangle)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/awesometkinter/progressbar.py:95
-msgid "color of parent container"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:84
+msgid ""
+"callback for when an item is deleted, with args: (int item, int rectangle)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkintertable/__init__.py:7
-msgid "tkintertable"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:92
+msgid ""
+"callback for when an item is moved, with args: (int item, int rectangle, int "
+"x, int y)"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tksheet/__init__.py:6
-msgid "tksheet"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/itemscanvas.py:100
+msgid ""
+"user defined function for when an item is created, with arg (add_item).\n"
+"Where add_item is a function of this widget."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkinterweb/__init__.py:6
-msgid "TkinterWeb"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:27
+msgid "link to be opened"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/dialog.py:51
-#: ../pygubu/src/pygubu/plugins/pygubu/combobox.py:24
-#: ../pygubu/src/pygubu/plugins/pygubu/tkscrolledframe.py:78
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:43
-#: ../pygubu/src/pygubu/plugins/pygubu/calendarframe.py:41
-#: ../pygubu/src/pygubu/plugins/pygubu/editabletreeview.py:31
-#: ../pygubu/src/pygubu/plugins/pygubu/scrolledframe.py:65
-msgid "Pygubu Widgets"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:33
+msgid "text color when widget is created"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/dialog.py:54
-msgid "Determines if dialog is run in normal or modal mode."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:39
+msgid "text color when hovering over the widget"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:57
-msgid "Initial path value."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/linklabel.py:45
+msgid "text color when link is clicked"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:60
-msgid "Image for the button."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:67
+msgid "side the Entry must be on."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:63
-msgid "Tk variable associated to the path property."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:76
+msgid "scale orientation"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:66
-msgid "Path entry state."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:84
+msgid "width of the Scale in pixels"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:77
-msgid ""
-"Dialog option. Determines if path must exist for directory and file dialogs. "
-"The default value is True."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:90
+msgid "width of the Entry in characters"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:89
-msgid "Dialog option. Sets initial directory."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:93
+msgid "start value of the scale"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:92
-msgid "Dialog option. Sets dialog title."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:96
+msgid "end value of the scale"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:95
-msgid "Dialog option. Sets default file extension."
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/scaleentry.py:102
+msgid "space between the entry and the scale"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/tkscrollbarhelper.py:76
-#: ../pygubu/src/pygubu/plugins/pygubu/scrollbarhelper.py:60
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:483
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:549
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:651
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1464
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1509
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1554
-msgid "Pygubu Helpers"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/table.py:41
+msgid "whether columns are draggable"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/pygubu/tkinterscrolledtext.py:17
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:68
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:87
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:110
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:134
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:175
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:188
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:199
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:224
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:245
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:266
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:277
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:354
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:460
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:688
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:724
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:753
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:215
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:299
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:347
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:406
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:465
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:506
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:604
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:695
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:726
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:771
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:804
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:880
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:922
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1569
-msgid "Control & Display"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/table.py:49
+msgid "whether rows are draggable"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tkintermapview/__init__.py:7
-msgid "TkinterMapView"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/table.py:58
+msgid ""
+"whether columns are sortable by clicking on their headings. The sorting "
+"order depends on the type of data (str, float, ...) which can be set with "
+"the column method."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:43
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:295
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:309
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:323
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:148
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:178
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:248
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:637
-msgid "Containers"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/tickscale.py:54
+msgid "increment by which the slider can be moved. 0 means continuous sliding."
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:353
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:694
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1016
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1360
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1373
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1397
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1420
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1438
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1554
-msgid "Menu"
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/tickscale.py:61
+msgid "if not 0, display ticks with the given interval"
+msgstr ""
+
+#: ../pygubu/src/pygubu/plugins/ttkwidgets/tickscale.py:82
+msgid "if tickinterval is not 0, position of the ticks"
 msgstr ""
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -112,26 +112,20 @@
 
 msgid "Applying ttk style definitions"
 msgstr "正在运用 ttk 样式定义"
 
 msgid "Associated program:"
 msgstr "相关程序："
 
-msgid "Automatically generate code"
-msgstr "自动生成代码"
-
 msgid "Background color to use when drawing the proxy."
 msgstr "绘制代理时要使用的背景颜色。"
 
 msgid "Bindings"
 msgstr "绑定"
 
-msgid "Browse …"
-msgstr "浏览 …"
-
 msgid "C"
 msgstr "C"
 
 msgid "Callback:"
 msgstr "回调:"
 
 msgid "Cancel"
@@ -148,17 +142,14 @@
 
 msgid "Checking main window visibility."
 msgstr "检查主窗口的可见性"
 
 msgid "Class"
 msgstr "类"
 
-msgid "Class Name:"
-msgstr "类名:"
-
 msgid "Clear"
 msgstr "清除"
 
 msgid "Clear all"
 msgstr "清除所有"
 
 msgid "Clear list"
@@ -172,17 +163,14 @@
 
 msgid "Code"
 msgstr "代码"
 
 msgid "Code Script"
 msgstr "代码脚本"
 
-msgid "Code copied"
-msgstr "代码被复制"
-
 msgid "Column index: {0}"
 msgstr "列索引： {0}"
 
 msgid "Column {0} options"
 msgstr "第'{0}'列的选项"
 
 msgid ""
@@ -197,20 +185,14 @@
 
 msgid "Controls how the built-in class bindings manage the selection."
 msgstr "控制内置类绑定如何管理选项。"
 
 msgid "Copy"
 msgstr "复制"
 
-msgid "Copy to Clipboard"
-msgstr "复制到剪切板"
-
-msgid "Create New …"
-msgstr "新建 …"
-
 msgid "Create a base class for your custom widget."
 msgstr "给你的自定义控件创建一个基类"
 
 msgid "Create a coded version of the UI definition."
 msgstr "创建一个用户界面定义的代码版本。"
 
 msgid "Create a pygubu application script using the UI definition."
@@ -218,32 +200,26 @@
 
 msgid "Custom Widget"
 msgstr "自定义控件"
 
 msgid "Custom Widgets"
 msgstr "自定义控件"
 
-msgid "Custom Widgets Builders"
-msgstr "自定义建设者控件"
-
 msgid "Cut"
 msgstr "剪切"
 
 msgid "Delete"
 msgstr "删除"
 
 msgid "Delete items"
 msgstr "删除项"
 
 msgid "Delete selected items?"
 msgstr "删除被选项？"
 
-msgid "Design"
-msgstr "设计"
-
 msgid "Detail"
 msgstr "详细"
 
 msgid "Determines if the window can be resized."
 msgstr "确定窗口是否可以调整。"
 
 msgid "Determines scroll type for the widget."
@@ -299,17 +275,14 @@
 msgstr "事件处理"
 
 msgid ""
 "Faild to parse config file at {CONFIG_FILE!s}, program may not work as "
 "expected."
 msgstr "未能解析\"{CONFIG_FILE!s}\"的配置文件，程序可能无法按预期工作。"
 
-msgid "Failed to load custom widget module: '{path}'"
-msgstr "加载自定义控件模块失败： '{path}'"
-
 msgid "Failed to load widget module: '{_module}'"
 msgstr "加载控件模块失败： '{_module}'"
 
 msgid "File"
 msgstr "文件"
 
 msgid ""
@@ -351,35 +324,26 @@
 
 msgid "GPL3"
 msgstr "GNU 通用公共许可证 第3版"
 
 msgid "General"
 msgstr "常用"
 
-msgid "General preferences"
-msgstr "首选项"
-
-msgid "Generate"
-msgstr "生成"
-
 msgid "Go to parent"
 msgstr "到父控件"
 
 msgid "Grid"
 msgstr "Grid"
 
 msgid "Grid Row / Column options"
 msgstr "表格行列选项："
 
 msgid "Help"
 msgstr "帮助"
 
-msgid "Hidden options"
-msgstr "隐藏选项"
-
 msgid "ID"
 msgstr "ID"
 
 msgid "If True, set this column as the tree column #0"
 msgstr "如果是True，将此列设置为树列 #0"
 
 msgid ""
@@ -590,17 +554,14 @@
 
 msgid "Open …"
 msgstr "打开 …"
 
 msgid "Options for {0} container"
 msgstr "{0} 容器的选项"
 
-msgid "Options:"
-msgstr "可选项:"
-
 msgid "Pack"
 msgstr "Pack"
 
 msgid "Paste"
 msgstr "粘贴"
 
 msgid "Place"
@@ -635,17 +596,14 @@
 
 msgid "Pygubu Preferences"
 msgstr "首选项"
 
 msgid "Pygubu wiki"
 msgstr "pygubu 百科"
 
-msgid "Python Script"
-msgstr "Python 脚本"
-
 msgid "Python module"
 msgstr "Python 模块"
 
 msgid "Quit …"
 msgstr "退出 …"
 
 msgid "R"
@@ -677,17 +635,14 @@
 "Requests additional space below each text line in the widget, using any of "
 "the standard forms for screen distances. If a line wraps, this option only "
 "applies to the last line on the display."
 msgstr ""
 "使用屏幕距离的任何标准形式，控制控件中每个文本行上方的额外空间。如果换行，此"
 "选项仅适用于屏幕上的第一行。"
 
-msgid "Requires restart."
-msgstr "需要重启应用。"
-
 msgid ""
 "Restart Pygubu Designer for\n"
 "changes to take effect."
 msgstr ""
 "重新启动 pygubu-designer\n"
 "改动将生效。"
 
@@ -759,17 +714,14 @@
 
 msgid "Sets the window title."
 msgstr "设置窗口标题。"
 
 msgid "Simple"
 msgstr "简易"
 
-msgid "Single section widgets toolbar (requires restart)"
-msgstr "独立小部件工具栏(需要重新启动)"
-
 msgid ""
 "Some interactions with the scale cause its value to change by \"large\" "
 "increments; this option specifies the size of the large increments."
 msgstr ""
 "与缩放的一些交互作用导致其值以 \"large\" 增量变化; 此选项指定大增量的大小。"
 
 msgid "Specifies a background color to use when the button is selected."
@@ -1425,17 +1377,14 @@
 "selected by the x, y, relx, and rely options."
 msgstr "指定在 x、y、relx 和依赖选项选择的 （x，y） 位置定位哪个窗口点。"
 
 msgid ""
 "Specifies which side of the container the content will be packed against."
 msgstr "指定内容将包装在容器的哪一侧。"
 
-msgid "Style Definition File:"
-msgstr "样式定义文件："
-
 msgid "Styles"
 msgstr "样式"
 
 msgid "Template description here."
 msgstr "模板描述."
 
 msgid "Template:"
@@ -1508,20 +1457,14 @@
 
 msgid "This program:"
 msgstr "此程序："
 
 msgid "Tk image formats"
 msgstr "Tk图片格式"
 
-msgid "Tree"
-msgstr "树状图"
-
-msgid "Ttk Styles"
-msgstr "Ttk 样式"
-
 msgid "Type of action."
 msgstr "Action类型"
 
 msgid "Uppercase first letter (e.g. Button…)"
 msgstr "首字母大写(像这样: Button1)"
 
 msgid "Use \"_\" as separator (e.g. button_1)"
@@ -1564,26 +1507,17 @@
 
 msgid "Widget naming"
 msgstr "控件命名"
 
 msgid "Widget tree"
 msgstr "控件树状图"
 
-msgid "Window geometry:"
-msgstr "窗口大小："
-
-msgid "modules"
-msgstr "模块"
-
 msgid "newproject"
 msgstr "新项目"
 
-msgid "on property change"
-msgstr "关属性更改"
-
 msgid "pygubu"
 msgstr "pygubu"
 
 msgid "pygubu ui"
 msgstr "pygubu 用户界面"
 
 msgid "pygubu-designer"
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -118,17 +118,14 @@
 
 msgid "Background color to use when drawing the proxy."
 msgstr "绘制代理时要使用的背景颜色。"
 
 msgid "Bindings"
 msgstr "绑定"
 
-msgid "Browse …"
-msgstr "浏览 ..."
-
 msgid "C"
 msgstr "C"
 
 msgid "Callback:"
 msgstr "回调:"
 
 msgid "Cancel"
@@ -142,17 +139,14 @@
 
 msgid "Change manager from {0} to {1}?"
 msgstr "转换{0}布局管理器为{1}布局管理器?"
 
 msgid "Class"
 msgstr "类"
 
-msgid "Class Name:"
-msgstr "类名:"
-
 msgid "Clear"
 msgstr "清除"
 
 msgid "Clear all"
 msgstr "清除所有"
 
 msgid "Clear list"
@@ -166,17 +160,14 @@
 
 msgid "Code"
 msgstr "代码"
 
 msgid "Code Script"
 msgstr "代码脚本"
 
-msgid "Code copied"
-msgstr "代码被复制"
-
 msgid "Column index: {0}"
 msgstr "列索引： {0}"
 
 msgid "Column {0} options"
 msgstr "第'{0}'列的选项"
 
 msgid ""
@@ -191,20 +182,14 @@
 
 msgid "Controls how the built-in class bindings manage the selection."
 msgstr "控制内置类绑定如何管理选项。"
 
 msgid "Copy"
 msgstr "复制"
 
-msgid "Copy to Clipboard"
-msgstr "复制到剪切板"
-
-msgid "Create New …"
-msgstr "新建 ..."
-
 msgid "Create a base class for your custom widget."
 msgstr "给你的自定义控件创建一个base类"
 
 msgid "Create a coded version of the UI definition."
 msgstr "创建一个用户界面定义的代码版本。"
 
 msgid "Create a pygubu application script using the UI definition."
@@ -212,32 +197,26 @@
 
 msgid "Custom Widget"
 msgstr "自定义控件"
 
 msgid "Custom Widgets"
 msgstr "自定义控件"
 
-msgid "Custom Widgets Builders"
-msgstr "自定义控件Builders"
-
 msgid "Cut"
 msgstr "剪切"
 
 msgid "Delete"
 msgstr "删除"
 
 msgid "Delete items"
 msgstr "删除项"
 
 msgid "Delete selected items?"
 msgstr "删除被选项？"
 
-msgid "Design"
-msgstr "设计"
-
 msgid "Detail"
 msgstr "详细"
 
 msgid "Determines if the window can be resized."
 msgstr "确定窗口是否可以调整。"
 
 msgid "Determines scroll type for the widget."
@@ -293,17 +272,14 @@
 msgstr "事件处理"
 
 msgid ""
 "Faild to parse config file at {CONFIG_FILE!s}, program may not work as "
 "expected."
 msgstr "未能解析\"{CONFIG_FILE!s}\"的配置文件，程序可能无法按预期工作。"
 
-msgid "Failed to load custom widget module: '{path}'"
-msgstr "加载自定义控件模块失败： '{path}'"
-
 msgid "Failed to load widget module: '{_module}'"
 msgstr "加载控件模块失败： '{_module}'"
 
 msgid "File"
 msgstr "文件"
 
 msgid ""
@@ -345,35 +321,26 @@
 
 msgid "GPL3"
 msgstr "GNU 通用公共许可证 第3版"
 
 msgid "General"
 msgstr "常用"
 
-msgid "General preferences"
-msgstr "首选项"
-
-msgid "Generate"
-msgstr "生成"
-
 msgid "Go to parent"
 msgstr "到父控件"
 
 msgid "Grid"
 msgstr "Grid"
 
 msgid "Grid Row / Column options"
 msgstr "表格行列选项："
 
 msgid "Help"
 msgstr "帮助"
 
-msgid "Hidden options"
-msgstr "被隐藏选项"
-
 msgid "ID"
 msgstr "ID"
 
 msgid "If True, set this column as the tree column #0"
 msgstr "如果是True，将此列设置为树列 #0"
 
 msgid ""
@@ -578,17 +545,14 @@
 
 msgid "Open …"
 msgstr "打开 …"
 
 msgid "Options for {0} container"
 msgstr "{0} 容器的选项"
 
-msgid "Options:"
-msgstr "可选项:"
-
 msgid "Pack"
 msgstr "Pack"
 
 msgid "Paste"
 msgstr "粘贴"
 
 msgid "Place"
@@ -623,17 +587,14 @@
 
 msgid "Pygubu Preferences"
 msgstr "首选项"
 
 msgid "Pygubu wiki"
 msgstr "pygubu 百科"
 
-msgid "Python Script"
-msgstr "Python脚本"
-
 msgid "Python module"
 msgstr "Python 模块"
 
 msgid "Quit …"
 msgstr "退出 …"
 
 msgid "R"
@@ -665,17 +626,14 @@
 "Requests additional space below each text line in the widget, using any of "
 "the standard forms for screen distances. If a line wraps, this option only "
 "applies to the last line on the display."
 msgstr ""
 "使用屏幕距离的任何标准形式，控制控件中每个文本行上方的额外空间。如果换行，此"
 "选项仅适用于屏幕上的第一行。"
 
-msgid "Requires restart."
-msgstr "需要重启应用。"
-
 msgid ""
 "Restart Pygubu Designer for\n"
 "changes to take effect."
 msgstr ""
 "重新启动 pygubu-designer\n"
 "更改将生效。"
 
@@ -1407,17 +1365,14 @@
 "selected by the x, y, relx, and rely options."
 msgstr "指定在 x、y、relx 和依赖选项选择的 （x，y） 位置定位哪个窗口点。"
 
 msgid ""
 "Specifies which side of the container the content will be packed against."
 msgstr "指定内容将包装在容器的哪一侧。"
 
-msgid "Style Definition File:"
-msgstr "样式定义文件："
-
 msgid "Styles"
 msgstr "样式"
 
 msgid "Template description here."
 msgstr "模板描述."
 
 msgid "Template:"
@@ -1490,20 +1445,14 @@
 
 msgid "This program:"
 msgstr "此程序："
 
 msgid "Tk image formats"
 msgstr "Tk图片格式"
 
-msgid "Tree"
-msgstr "树"
-
-msgid "Ttk Styles"
-msgstr "Ttk 样式"
-
 msgid "Type of action."
 msgstr "Action类型"
 
 msgid "Uppercase first letter (e.g. Button…)"
 msgstr "首字母大写(像这样: Button1)"
 
 msgid "Use \"_\" as separator (e.g. button_1)"
@@ -1546,20 +1495,14 @@
 
 msgid "Widget naming"
 msgstr "控件命名"
 
 msgid "Widget tree"
 msgstr "控件树"
 
-msgid "Window geometry:"
-msgstr "窗口大小："
-
-msgid "modules"
-msgstr "模块"
-
 msgid "newproject"
 msgstr "新项目"
 
 msgid "pygubu"
 msgstr "pygubu"
 
 msgid "pygubu ui"
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/ui/about_dialog.ui` & `pygubu_designer-0.39/examples/scrolledframe/scrolledframe_demo.ui`

 * *Files 19% similar despite different names*

#### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/ui/about_dialog.ui` & `pygubu_designer-0.39/examples/scrolledframe/scrolledframe_demo.ui`

```diff
@@ -1,271 +1,269 @@
 <?xml version="1.0" encoding="utf-8"?>
 <interface version="1.3">
-  <object class="pygubu.builder.widgets.dialog" id="aboutdialog">
-    <property name="geometry">420x550</property>
-    <property name="height">100</property>
-    <property name="modal">False</property>
+  <object class="tk.Toplevel" id="toplevel1">
+    <property name="geometry">480x400</property>
+    <property name="height">200</property>
     <property name="resizable">both</property>
-    <property name="title" translatable="yes">About</property>
+    <property name="title" translatable="yes">ScrolledFrame demo using grid manager</property>
     <property name="width">200</property>
+    <containerlayout manager="grid">
+      <property type="col" id="0" name="weight">1</property>
+      <property type="row" id="0" name="weight">1</property>
+    </containerlayout>
     <child>
       <object class="ttk.Frame" id="frame1">
-        <property name="height">250</property>
+        <property name="height">200</property>
         <property name="padding">5</property>
-        <property name="width">400</property>
-        <layout manager="pack">
-          <property name="expand">true</property>
-          <property name="fill">both</property>
+        <property name="width">200</property>
+        <layout manager="grid">
+          <property name="column">0</property>
+          <property name="row">0</property>
+          <property name="sticky">nsew</property>
         </layout>
+        <containerlayout manager="grid">
+          <property type="col" id="0" name="weight">1</property>
+          <property type="row" id="1" name="weight">1</property>
+        </containerlayout>
         <child>
-          <object class="ttk.Frame" id="Frame_1">
+          <object class="ttk.Frame" id="frame3">
             <property name="height">200</property>
             <property name="width">200</property>
-            <layout manager="pack">
-              <property name="expand">true</property>
-              <property name="fill">both</property>
-              <property name="side">top</property>
+            <layout manager="grid">
+              <property name="column">0</property>
+              <property name="row">0</property>
+              <property name="sticky">nsew</property>
             </layout>
             <child>
-              <object class="ttk.Label" id="logo">
-                <property name="anchor">e</property>
-                <property name="font">Sans 18 bold</property>
-                <property name="image">pygubu200</property>
-                <property name="text" translatable="yes">pygubu</property>
-                <layout manager="pack">
-                  <property name="pady">0 20</property>
+              <object class="ttk.Label" id="label1">
+                <property name="text" translatable="yes">A scrolledframe with size limited by a &quot;framesizer&quot;.
+A framesizer is a frame with propagate=False.
+It will maintain a size of 350x80 pixels</property>
+                <property name="wraplength">450</property>
+                <layout manager="grid">
+                  <property name="column">0</property>
+                  <property name="pady">5</property>
+                  <property name="row">0</property>
+                  <property name="sticky">ew</property>
                 </layout>
               </object>
             </child>
             <child>
-              <object class="ttk.Frame" id="frame2">
-                <property name="height">200</property>
-                <property name="width">200</property>
-                <layout manager="pack">
-                  <property name="fill">both</property>
-                  <property name="pady">0 10</property>
-                  <property name="side">top</property>
+              <object class="ttk.Frame" id="framesizer" named="True">
+                <property name="height">80</property>
+                <property name="width">350</property>
+                <layout manager="grid">
+                  <property name="column">0</property>
+                  <property name="row">1</property>
                 </layout>
+                <containerlayout manager="grid">
+                  <property name="propagate">False</property>
+                  <property type="col" id="0" name="weight">1</property>
+                  <property type="row" id="0" name="weight">1</property>
+                </containerlayout>
                 <child>
-                  <object class="ttk.Frame" id="frame4">
-                    <property name="height">200</property>
+                  <object class="pygubu.builder.widgets.scrolledframe" id="scrolledframe_1">
+                    <property name="height">50</property>
+                    <property name="scrolltype">both</property>
                     <property name="width">200</property>
-                    <layout manager="pack">
-                      <property name="side">top</property>
+                    <layout manager="grid">
+                      <property name="column">0</property>
+                      <property name="row">0</property>
+                      <property name="sticky">nsew</property>
                     </layout>
+                    <containerlayout manager="grid">
+                      <property type="col" id="0" name="weight">1</property>
+                      <property type="row" id="0" name="weight">1</property>
+                    </containerlayout>
                     <child>
-                      <object class="ttk.Label" id="label1">
-                        <property name="font">{sans} 12 {bold}</property>
-                        <property name="text" translatable="yes">This program:</property>
-                        <layout manager="pack">
-                          <property name="anchor">center</property>
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
-                    <child>
-                      <object class="ttk.Label" id="label2">
-                        <property name="font">{sans} 12 {bold}</property>
-                        <property name="text" translatable="yes">pygubu-designer</property>
-                        <layout manager="pack">
-                          <property name="anchor">center</property>
-                          <property name="padx">5 0</property>
-                          <property name="side">left</property>
+                      <object class="tk.Text" id="Text_1">
+                        <property name="height">50</property>
+                        <property name="text" translatable="yes">Very long long long long long long long long text</property>
+                        <property name="width">50</property>
+                        <layout manager="grid">
+                          <property name="column">0</property>
+                          <property name="row">0</property>
+                          <property name="sticky">nsew</property>
                         </layout>
                       </object>
                     </child>
                   </object>
                 </child>
+              </object>
+            </child>
+          </object>
+        </child>
+        <child>
+          <object class="ttk.Frame" id="frame4">
+            <property name="height">200</property>
+            <property name="width">200</property>
+            <layout manager="grid">
+              <property name="column">0</property>
+              <property name="pady">10 0</property>
+              <property name="row">1</property>
+              <property name="sticky">nsew</property>
+            </layout>
+            <containerlayout manager="grid">
+              <property type="col" id="0" name="weight">1</property>
+              <property type="row" id="1" name="weight">1</property>
+            </containerlayout>
+            <child>
+              <object class="ttk.Label" id="label2">
+                <property name="text" translatable="yes">A scrolledframe with with no restriction.</property>
+                <property name="wraplength">450</property>
+                <layout manager="grid">
+                  <property name="column">0</property>
+                  <property name="pady">5</property>
+                  <property name="row">0</property>
+                  <property name="sticky">ew</property>
+                </layout>
+              </object>
+            </child>
+            <child>
+              <object class="pygubu.builder.widgets.scrolledframe" id="scrolledframe1">
+                <property name="height">50</property>
+                <property name="scrolltype">both</property>
+                <property name="width">200</property>
+                <layout manager="grid">
+                  <property name="column">0</property>
+                  <property name="row">1</property>
+                  <property name="sticky">nsew</property>
+                </layout>
                 <child>
-                  <object class="ttk.Label" id="label3">
-                    <property name="font">{Sans} 10 {}</property>
-                    <property name="justify">center</property>
-                    <property name="text" translatable="yes">A visual design tool for tkinter that generates Python code for the user interface portion of your desktop application.</property>
-                    <property name="wraplength">420</property>
-                    <layout manager="pack">
-                      <property name="fill">both</property>
-                      <property name="pady">2</property>
-                      <property name="side">top</property>
+                  <object class="tk.Canvas" id="canvas1">
+                    <property name="background">#00d9d9</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">0</property>
+                      <property name="row">0</property>
                     </layout>
                   </object>
                 </child>
                 <child>
-                  <object class="ttk.Label" id="designer_version">
-                    <property name="font">{sans} 10 {}</property>
-                    <property name="text" translatable="yes">Version: %version%</property>
-                    <layout manager="pack">
-                      <property name="side">top</property>
+                  <object class="tk.Canvas" id="canvas2">
+                    <property name="background">#0080d9</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">1</property>
+                      <property name="row">0</property>
                     </layout>
                   </object>
                 </child>
                 <child>
-                  <object class="ttk.Frame" id="frame7">
+                  <object class="tk.Canvas" id="canvas3">
+                    <property name="background">#0023d9</property>
                     <property name="height">200</property>
                     <property name="width">200</property>
-                    <layout manager="pack">
-                      <property name="side">top</property>
+                    <layout manager="grid">
+                      <property name="column">2</property>
+                      <property name="row">0</property>
                     </layout>
-                    <child>
-                      <object class="ttk.Label" id="label7">
-                        <property name="font">{sans} 10 {}</property>
-                        <property name="text" translatable="yes">License:</property>
-                        <layout manager="pack">
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
-                    <child>
-                      <object class="ttk.Label" id="licence_link">
-                        <property name="anchor">center</property>
-                        <property name="cursor">hand2</property>
-                        <property name="font">{Sans} 10 {}</property>
-                        <property name="foreground">#143ee3</property>
-                        <property name="text" translatable="yes">GPL3</property>
-                        <bind sequence="&lt;Button-1&gt;" handler="on_gpl3_clicked" add=""/>
-                        <layout manager="pack">
-                          <property name="padx">5 0</property>
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
                   </object>
                 </child>
-              </object>
-            </child>
-            <child>
-              <object class="ttk.Frame" id="frame3">
-                <property name="height">200</property>
-                <property name="width">200</property>
-                <layout manager="pack">
-                  <property name="fill">both</property>
-                  <property name="side">top</property>
-                </layout>
                 <child>
-                  <object class="ttk.Frame" id="frame5">
+                  <object class="tk.Canvas" id="canvas7">
+                    <property name="background">#0000d9</property>
                     <property name="height">200</property>
                     <property name="width">200</property>
-                    <layout manager="pack">
-                      <property name="side">top</property>
+                    <layout manager="grid">
+                      <property name="column">3</property>
+                      <property name="row">0</property>
+                    </layout>
+                  </object>
+                </child>
+                <child>
+                  <object class="tk.Canvas" id="canvas4">
+                    <property name="background">#00ff00</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">0</property>
+                      <property name="row">1</property>
                     </layout>
-                    <child>
-                      <object class="ttk.Label" id="label4">
-                        <property name="font">{sans} 11 {bold}</property>
-                        <property name="text" translatable="yes">Associated program:</property>
-                        <layout manager="pack">
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
-                    <child>
-                      <object class="ttk.Label" id="label5">
-                        <property name="font">{sans} 11 {bold}</property>
-                        <property name="text" translatable="yes">pygubu</property>
-                        <layout manager="pack">
-                          <property name="padx">5 0</property>
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
                   </object>
                 </child>
                 <child>
-                  <object class="ttk.Label" id="label6">
-                    <property name="font">{sans} 10 {}</property>
-                    <property name="justify">center</property>
-                    <property name="text" translatable="yes">A run-time library that the designer requires. It is optional for your application.</property>
-                    <property name="wraplength">420</property>
-                    <layout manager="pack">
-                      <property name="fill">both</property>
-                      <property name="pady">2</property>
-                      <property name="side">top</property>
+                  <object class="tk.Canvas" id="canvas5">
+                    <property name="background">#00a600</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">1</property>
+                      <property name="row">1</property>
                     </layout>
                   </object>
                 </child>
                 <child>
-                  <object class="ttk.Label" id="version">
-                    <property name="font">{Sans} 10 {}</property>
-                    <property name="text" translatable="yes">Version: %version%</property>
-                    <layout manager="pack"/>
+                  <object class="tk.Canvas" id="canvas6">
+                    <property name="background">#004900</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">2</property>
+                      <property name="row">1</property>
+                    </layout>
                   </object>
                 </child>
                 <child>
-                  <object class="ttk.Frame" id="frame8">
+                  <object class="tk.Canvas" id="canvas8">
+                    <property name="background">#002400</property>
                     <property name="height">200</property>
                     <property name="width">200</property>
-                    <layout manager="pack">
-                      <property name="side">top</property>
+                    <layout manager="grid">
+                      <property name="column">3</property>
+                      <property name="row">1</property>
                     </layout>
-                    <child>
-                      <object class="ttk.Label" id="label10">
-                        <property name="font">{sans} 10 {}</property>
-                        <property name="text" translatable="yes">License:</property>
-                        <layout manager="pack">
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
-                    <child>
-                      <object class="ttk.Label" id="label11">
-                        <property name="anchor">center</property>
-                        <property name="cursor">hand2</property>
-                        <property name="font">{Sans} 10 {}</property>
-                        <property name="foreground">#143ee3</property>
-                        <property name="text" translatable="yes">MIT</property>
-                        <bind sequence="&lt;Button-1&gt;" handler="on_mit_clicked" add=""/>
-                        <layout manager="pack">
-                          <property name="padx">5 0</property>
-                          <property name="side">left</property>
-                        </layout>
-                      </object>
-                    </child>
                   </object>
                 </child>
-              </object>
-            </child>
-            <child>
-              <object class="ttk.Frame" id="frame6">
-                <property name="height">200</property>
-                <property name="width">200</property>
-                <layout manager="pack">
-                  <property name="pady">10 0</property>
-                  <property name="side">top</property>
-                </layout>
                 <child>
-                  <object class="ttk.Label" id="label9">
-                    <property name="anchor">center</property>
-                    <property name="cursor">hand2</property>
-                    <property name="font">{Sans} 10 {}</property>
-                    <property name="foreground">#143ee3</property>
-                    <property name="text" translatable="yes">More info.</property>
-                    <bind sequence="&lt;Button-1&gt;" handler="on_moreinfo_clicked" add=""/>
-                    <layout manager="pack">
-                      <property name="pady">10 0</property>
-                      <property name="side">top</property>
+                  <object class="tk.Canvas" id="canvas9">
+                    <property name="background">#ff0000</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">0</property>
+                      <property name="row">2</property>
+                    </layout>
+                  </object>
+                </child>
+                <child>
+                  <object class="tk.Canvas" id="canvas10">
+                    <property name="background">#b90000</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">1</property>
+                      <property name="row">2</property>
+                    </layout>
+                  </object>
+                </child>
+                <child>
+                  <object class="tk.Canvas" id="canvas11">
+                    <property name="background">#6e0000</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">2</property>
+                      <property name="row">2</property>
+                    </layout>
+                  </object>
+                </child>
+                <child>
+                  <object class="tk.Canvas" id="canvas12">
+                    <property name="background">#390000</property>
+                    <property name="height">200</property>
+                    <property name="width">200</property>
+                    <layout manager="grid">
+                      <property name="column">3</property>
+                      <property name="row">2</property>
                     </layout>
                   </object>
                 </child>
-              </object>
-            </child>
-          </object>
-        </child>
-        <child>
-          <object class="ttk.Frame" id="bottom">
-            <property name="height"/>
-            <property name="padding">0 10 0 0</property>
-            <property name="width"/>
-            <layout manager="pack">
-              <property name="fill">x</property>
-            </layout>
-            <child>
-              <object class="ttk.Button" id="close_btn">
-                <property name="command" type="command" cbtype="simple" args="">on_ok_execute</property>
-                <property name="text" translatable="yes">Close</property>
-                <layout manager="pack">
-                  <property name="side">right</property>
-                </layout>
               </object>
             </child>
           </object>
         </child>
       </object>
     </child>
   </object>
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui` & `pygubu_designer-0.39/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/ui/container_layout_editor_base.ui` & `pygubu_designer-0.39/src/pygubudesigner/data/ui/container_layout_editor_base.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/ui/pygubu-ui.ui` & `pygubu_designer-0.39/src/pygubudesigner/data/ui/project_settings.ui`

 * *Files 21% similar despite different names*

#### Comparing `pygubu-designer-0.38/src/pygubudesigner/data/ui/pygubu-ui.ui` & `pygubu_designer-0.39/src/pygubudesigner/data/ui/project_settings.ui`

```diff
@@ -1,1205 +1,769 @@
 <?xml version="1.0" encoding="utf-8"?>
-<interface version="1.3">
-  <object class="tk.Menu" id="mainmenu">
-    <property name="tearoff">0</property>
-    <child>
-      <object class="tk.Menuitem.Submenu" id="filemenu">
-        <property name="label" translatable="yes">File</property>
-        <property name="tearoff">0</property>
-        <property name="underline">0</property>
-        <child>
-          <object class="tk.Menuitem.Command" id="FILE_NEW">
-            <property name="accelerator">Ctrl+N</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_file_menuitem_clicked</property>
-            <property name="label" translatable="yes">New</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="FILE_OPEN">
-            <property name="accelerator">Ctrl+O</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_file_menuitem_clicked</property>
-            <property name="label" translatable="yes">Open …</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Submenu" id="file_recent_menu">
-            <property name="label" translatable="yes">Open recent …</property>
-            <property name="tearoff">false</property>
-            <child>
-              <object class="tk.Menuitem.Separator" id="file_recent_sep1"/>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Command" id="FILE_RECENT_CLEAR">
-                <property name="command" type="command" cbtype="with_wid" args="">on_file_menuitem_clicked</property>
-                <property name="label" translatable="yes">Clear list</property>
-              </object>
-            </child>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Separator" id="file_sep2"/>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="FILE_SAVE">
-            <property name="accelerator">Ctrl+S</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_file_menuitem_clicked</property>
-            <property name="label" translatable="yes">Save</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="FILE_SAVEAS">
-            <property name="command" type="command" cbtype="with_wid" args="">on_file_menuitem_clicked</property>
-            <property name="label" translatable="yes">Save as …</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Separator" id="file_sep1"/>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="FILE_QUIT">
-            <property name="accelerator">Ctrl+Q</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_file_menuitem_clicked</property>
-            <property name="label" translatable="yes">Quit …</property>
-          </object>
-        </child>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Submenu" id="editmenu">
-        <property name="label" translatable="yes">Edit</property>
-        <property name="tearoff">0</property>
-        <property name="underline">0</property>
-        <child>
-          <object class="tk.Menuitem.Command" id="TREE_ITEM_COPY">
-            <property name="accelerator">Ctrl+C</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-            <property name="label" translatable="yes">Copy</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="TREE_ITEM_PASTE">
-            <property name="accelerator">Ctrl+V</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-            <property name="label" translatable="yes">Paste</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="TREE_ITEM_CUT">
-            <property name="accelerator">Ctrl+X</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-            <property name="label" translatable="yes">Cut</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="TREE_ITEM_DUPLICATE">
-            <property name="accelerator">Ctrl+D</property>
-            <property name="command" type="command" cbtype="with_wid">on_edit_menuitem_clicked</property>
-            <property name="label" translatable="yes">Duplicate</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Separator" id="edit_Separator1"/>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Submenu" id="edit_widget">
-            <property name="label" translatable="yes">Widget tree</property>
-            <property name="tearoff">0</property>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_MOVE_UP">
-                <property name="accelerator">Ctrl+I</property>
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Item up</property>
-              </object>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_MOVE_DOWN">
-                <property name="accelerator">Ctrl+K</property>
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Item down</property>
-              </object>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Separator" id="edit_sep2"/>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_DELETE">
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Item delete</property>
-              </object>
-            </child>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Submenu" id="edit_widget_grid">
-            <property name="label" translatable="yes">Widget grid</property>
-            <property name="tearoff">0</property>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_GRID_UP">
-                <property name="accelerator">Alt+I</property>
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Move up</property>
-              </object>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_GRID_DOWN">
-                <property name="accelerator">Alt+K</property>
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Move down</property>
-              </object>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_GRID_LEFT">
-                <property name="accelerator">Alt+J</property>
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Move left</property>
-              </object>
-            </child>
-            <child>
-              <object class="tk.Menuitem.Command" id="TREE_ITEM_GRID_RIGHT">
-                <property name="accelerator">Alt+L</property>
-                <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-                <property name="label" translatable="yes">Move right</property>
-              </object>
-            </child>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Separator" id="edit_Separator2"/>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="edit_preferences">
-            <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
-            <property name="label" translatable="yes">Preferences</property>
-          </object>
-        </child>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Submenu" id="previewmenu">
-        <property name="label" translatable="yes">Preview</property>
-        <property name="tearoff">0</property>
-        <property name="underline">0</property>
-        <child>
-          <object class="tk.Menuitem.Command" id="TREE_ITEM_PREVIEW_TOPLEVEL">
-            <property name="accelerator">F5</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_previewmenu_action</property>
-            <property name="label" translatable="yes">Preview in Toplevel</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="PREVIEW_TOPLEVEL_CLOSE_ALL">
-            <property name="accelerator">F6</property>
-            <property name="command" type="command" cbtype="with_wid" args="">on_previewmenu_action</property>
-            <property name="label" translatable="yes">Close Toplevel previews</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Submenu" id="preview_themes_submenu">
-            <property name="label" translatable="yes">ttk theme</property>
-            <property name="tearoff">0</property>
-          </object>
-        </child>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Submenu" id="helpmenu">
-        <property name="label" translatable="yes">Help</property>
-        <property name="tearoff">0</property>
-        <property name="underline">0</property>
-        <child>
-          <object class="tk.Menuitem.Command" id="help_online">
-            <property name="command" type="command" cbtype="with_wid" args="">on_help_menuitem_clicked</property>
-            <property name="label" translatable="yes">Pygubu wiki</property>
-          </object>
-        </child>
-        <child>
-          <object class="tk.Menuitem.Command" id="help_about">
-            <property name="command" type="command" cbtype="with_wid" args="">on_help_menuitem_clicked</property>
-            <property name="label" translatable="yes">About Pygubu</property>
-          </object>
-        </child>
-      </object>
-    </child>
-  </object>
-  <object class="tk.Menu" id="context_menu">
-    <property name="tearoff">false</property>
-    <child>
-      <object class="tk.Menuitem.Command" id="menu_go_to_parent">
-        <property name="command" type="command" cbtype="simple">on_context_menu_go_to_parent_clicked</property>
-        <property name="label" translatable="yes">Go to parent</property>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Separator" id="sep_context"/>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Command" id="menu_copy">
-        <property name="command" type="command" cbtype="simple">on_context_menu_copy_clicked</property>
-        <property name="label" translatable="yes">Copy</property>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Command" id="menu_paste">
-        <property name="command" type="command" cbtype="simple">on_context_menu_paste_clicked</property>
-        <property name="label" translatable="yes">Paste</property>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Command" id="menu_cut">
-        <property name="command" type="command" cbtype="simple">on_context_menu_cut_clicked</property>
-        <property name="label" translatable="yes">Cut</property>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Command" id="menu_delete">
-        <property name="command" type="command" cbtype="simple">on_context_menu_delete_clicked</property>
-        <property name="label" translatable="yes">Delete</property>
-      </object>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Separator" id="context_sep1"/>
-    </child>
-    <child>
-      <object class="tk.Menuitem.Command" id="menu_duplicate">
-        <property name="command" type="command" cbtype="simple">on_context_menu_duplicate_clicked</property>
-        <property name="label" translatable="yes">Duplicate</property>
-      </object>
-    </child>
-  </object>
-  <object class="tk.Toplevel" id="mainwindow">
-    <property name="geometry">640x480</property>
-    <property name="height">200</property>
-    <property name="resizable">both</property>
-    <property name="title" translatable="yes">Pygubu Designer</property>
+<interface version="1.4" author="PygubuDesigner 0.39">
+  <project>
+    <settings>
+      <setting id="name">Project settings dialog</setting>
+      <setting id="description">Designer Project Settings dialog.</setting>
+      <setting id="module_name">projectsettings</setting>
+      <setting id="template">application</setting>
+      <setting id="main_widget">settingsdialog</setting>
+      <setting id="main_classname">ProjectSettings</setting>
+      <setting id="main_menu"/>
+      <setting id="output_dir">../../services</setting>
+      <setting id="output_dir2"/>
+      <setting id="import_tkvariables">True</setting>
+      <setting id="use_ttk_styledefinition_file">False</setting>
+      <setting id="use_i18n">True</setting>
+      <setting id="all_ids_attributes">False</setting>
+      <setting id="generate_code_onsave">True</setting>
+      <setting id="use_window_centering_code">False</setting>
+      <setting id="ttk_style_definition_file"/>
+    </settings>
+    <customwidgets/>
+  </project>
+  <object class="pygubu.builder.widgets.dialog" id="settingsdialog" named="True">
+    <property name="geometry">680x580</property>
+    <property name="height">100</property>
+    <property name="modal">true</property>
     <property name="width">200</property>
+    <bind sequence="&lt;&lt;DialogClose&gt;&gt;" handler="on_dialog_close" add="True"/>
     <child>
-      <object class="ttk.Frame" id="mainframe">
-        <property name="padding">2</property>
+      <object class="ttk.Frame" id="frame8">
+        <property name="height">200</property>
+        <property name="padding">4</property>
+        <property name="width">200</property>
         <layout manager="pack">
           <property name="expand">true</property>
           <property name="fill">both</property>
           <property name="side">top</property>
         </layout>
         <child>
-          <object class="ttk.Panedwindow" id="mainpw">
+          <object class="ttk.Frame" id="frame9">
             <property name="height">200</property>
-            <property name="orient">vertical</property>
             <property name="width">200</property>
             <layout manager="pack">
               <property name="expand">true</property>
               <property name="fill">both</property>
               <property name="side">top</property>
             </layout>
             <child>
-              <object class="ttk.Panedwindow.Pane" id="mainpw_top">
-                <property name="weight">1</property>
+              <object class="ttk.Notebook" id="notebook1">
+                <property name="height">200</property>
+                <property name="style">ProjectSettings.TNotebook</property>
+                <property name="width">200</property>
+                <layout manager="pack">
+                  <property name="expand">true</property>
+                  <property name="fill">both</property>
+                  <property name="side">top</property>
+                </layout>
                 <child>
-                  <object class="ttk.Frame" id="newmain">
-                    <layout manager="pack">
-                      <property name="expand">true</property>
-                      <property name="fill">both</property>
-                      <property name="side">top</property>
-                    </layout>
+                  <object class="ttk.Notebook.Tab" id="tab2">
+                    <property name="compound">left</property>
+                    <property name="image">mglass.png</property>
+                    <property name="sticky">nsew</property>
+                    <property name="text" translatable="yes">General</property>
                     <child>
-                      <object class="ttk.Notebook" id="nbmain">
-                        <bind sequence="&lt;&lt;NotebookTabChanged&gt;&gt;" handler="nbmain_tab_changed" add=""/>
+                      <object class="pygubu.forms.ttkwidget.FrameFormBuilder" id="frm_general" named="True">
+                        <property name="padding">5</property>
+                        <layout manager="pack">
+                          <property name="side">top</property>
+                        </layout>
+                        <containerlayout manager="grid">
+                          <property type="col" id="1" name="weight">1</property>
+                          <property type="col" id="all" name="pad">10</property>
+                          <property type="row" id="all" name="pad">10</property>
+                        </containerlayout>
+                        <child>
+                          <object class="ttk.Label" id="label6">
+                            <property name="text" translatable="yes">Name:</property>
+                            <layout manager="grid">
+                              <property name="column">0</property>
+                              <property name="row">0</property>
+                              <property name="sticky">ew</property>
+                            </layout>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="pygubu.forms.ttkwidget.Entry" id="entryfield4">
+                            <property name="field_name">name</property>
+                            <property name="style">EntryField.TEntry</property>
+                            <layout manager="grid">
+                              <property name="column">1</property>
+                              <property name="ipady">3</property>
+                              <property name="row">0</property>
+                              <property name="sticky">ew</property>
+                            </layout>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo6">
+                            <property name="field_name">name</property>
+                            <property name="style">LabelFieldInfo.TLabel</property>
+                            <layout manager="grid">
+                              <property name="column">1</property>
+                              <property name="row">1</property>
+                              <property name="sticky">ew</property>
+                            </layout>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="ttk.Label" id="label7">
+                            <property name="text" translatable="yes">Description:</property>
+                            <layout manager="grid">
+                              <property name="column">0</property>
+                              <property name="row">2</property>
+                              <property name="sticky">ew</property>
+                            </layout>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="pygubu.builder.widgets.scrollbarhelper" id="scrollbarhelper2">
+                            <property name="scrolltype">both</property>
+                            <property name="usemousewheel">false</property>
+                            <layout manager="grid">
+                              <property name="column">0</property>
+                              <property name="columnspan">2</property>
+                              <property name="row">3</property>
+                              <property name="sticky">ew</property>
+                            </layout>
+                            <child>
+                              <object class="pygubu.forms.tkwidget.Text" id="textfield1">
+                                <property name="field_name">description</property>
+                                <property name="height">8</property>
+                                <property name="width">32</property>
+                                <layout manager="pack"/>
+                              </object>
+                            </child>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo7">
+                            <property name="field_name">description</property>
+                            <property name="style">LabelFieldInfo.TLabel</property>
+                            <layout manager="grid">
+                              <property name="column">0</property>
+                              <property name="columnspan">2</property>
+                              <property name="row">4</property>
+                              <property name="sticky">ew</property>
+                            </layout>
+                          </object>
+                        </child>
+                      </object>
+                    </child>
+                  </object>
+                </child>
+                <child>
+                  <object class="ttk.Notebook.Tab" id="tab1">
+                    <property name="sticky">nsew</property>
+                    <property name="text" translatable="yes">Code</property>
+                    <child>
+                      <object class="pygubu.forms.ttkwidget.FrameFormBuilder" id="frm_code" named="True">
+                        <property name="padding">5 5 50 5</property>
                         <layout manager="pack">
                           <property name="expand">true</property>
                           <property name="fill">both</property>
                           <property name="side">top</property>
                         </layout>
                         <child>
-                          <object class="ttk.Notebook.Tab" id="tab_design">
-                            <property name="sticky">nsew</property>
-                            <property name="text" translatable="yes">Design</property>
-                            <child>
-                              <object class="ttk.Frame" id="designer_main">
-                                <property name="height">100</property>
-                                <property name="width">100</property>
-                                <layout manager="pack">
-                                  <property name="expand">true</property>
-                                  <property name="fill">both</property>
-                                  <property name="side">top</property>
+                          <object class="ttk.Frame" id="frame1">
+                            <property name="height">200</property>
+                            <property name="width">200</property>
+                            <layout manager="pack">
+                              <property name="fill">x</property>
+                              <property name="side">top</property>
+                            </layout>
+                            <containerlayout manager="grid">
+                              <property type="col" id="1" name="weight">1</property>
+                              <property type="col" id="all" name="pad">5</property>
+                              <property type="row" id="all" name="pad">8</property>
+                            </containerlayout>
+                            <child>
+                              <object class="ttk.Label" id="label3">
+                                <property name="text" translatable="yes">Module name:</property>
+                                <layout manager="grid">
+                                  <property name="column">0</property>
+                                  <property name="row">0</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Entry" id="module_name" named="True">
+                                <property name="style">EntryField.TEntry</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="ipady">3</property>
+                                  <property name="row">0</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo4">
+                                <property name="field_name">module_name</property>
+                                <property name="style">LabelFieldInfo.TLabel</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">1</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="lbl_template">
+                                <property name="text" translatable="yes">Template:</property>
+                                <layout manager="grid">
+                                  <property name="column">0</property>
+                                  <property name="row">2</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.pygubuwidget.PygubuCombobox" id="template" named="True">
+                                <property name="style">ComboboxField.TCombobox</property>
+                                <bind sequence="&lt;&lt;ComboboxSelected&gt;&gt;" handler="on_template_change" add=""/>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="ipady">3</property>
+                                  <property name="row">2</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="label5">
+                                <property name="font">TkSmallCaptionFont</property>
+                                <property name="text" translatable="yes">Template description here.</property>
+                                <property name="textvariable">string:template_desc_var</property>
+                                <property name="wraplength">500</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">3</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="lbl_wlist">
+                                <property name="text" translatable="yes">Main widget:</property>
+                                <layout manager="grid">
+                                  <property name="column">0</property>
+                                  <property name="row">4</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.pygubuwidget.PygubuCombobox" id="main_widget" named="True">
+                                <property name="state">readonly</property>
+                                <property name="style">ComboboxField.TCombobox</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="ipady">3</property>
+                                  <property name="row">4</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo1">
+                                <property name="field_name">main_widget</property>
+                                <property name="style">LabelFieldInfo.TLabel</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">5</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="label_2">
+                                <property name="text" translatable="yes">Class name:</property>
+                                <layout manager="grid">
+                                  <property name="row">6</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Entry" id="main_classname" named="True">
+                                <property name="style">EntryField.TEntry</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="ipady">3</property>
+                                  <property name="row">6</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo2">
+                                <property name="field_name">main_classname</property>
+                                <property name="style">LabelFieldInfo.TLabel</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">7</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="label2">
+                                <property name="text" translatable="yes">Main menu:</property>
+                                <layout manager="grid">
+                                  <property name="column">0</property>
+                                  <property name="row">8</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.pygubuwidget.PygubuCombobox" id="main_menu" named="True">
+                                <property name="state">readonly</property>
+                                <property name="style">ComboboxField.TCombobox</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="ipady">3</property>
+                                  <property name="row">8</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo3">
+                                <property name="field_name">main_menu</property>
+                                <property name="style">LabelFieldInfo.TLabel</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">9</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="label4">
+                                <property name="text" translatable="yes">Module output:</property>
+                                <layout manager="grid">
+                                  <property name="column">0</property>
+                                  <property name="row">10</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Frame" id="frame3">
+                                <property name="height">200</property>
+                                <property name="width">200</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">10</property>
+                                  <property name="sticky">ew</property>
                                 </layout>
                                 <child>
-                                  <object class="ttk.Frame" id="fpalette">
-                                    <property name="height">50</property>
+                                  <object class="pygubu.forms.ttkwidget.Entry" id="output_dir" named="True">
+                                    <property name="style">EntryField.TEntry</property>
                                     <layout manager="pack">
+                                      <property name="expand">true</property>
                                       <property name="fill">x</property>
-                                      <property name="side">top</property>
+                                      <property name="ipady">3</property>
+                                      <property name="side">left</property>
                                     </layout>
                                   </object>
                                 </child>
                                 <child>
-                                  <object class="ttk.Panedwindow" id="designerpw">
-                                    <property name="orient">horizontal</property>
+                                  <object class="pygubu.widgets.PathChooserButton" id="btn_path_chooser" named="True">
+                                    <property name="image">mglass.png</property>
+                                    <property name="text" translatable="yes">…</property>
+                                    <property name="title" translatable="yes">Select output directory</property>
+                                    <property name="type">directory</property>
+                                    <property name="width">4</property>
+                                    <bind sequence="&lt;&lt;PathChooserPathChanged&gt;&gt;" handler="output_dir_changed" add=""/>
                                     <layout manager="pack">
-                                      <property name="expand">true</property>
-                                      <property name="fill">both</property>
-                                      <property name="side">top</property>
+                                      <property name="padx">10 0</property>
+                                      <property name="side">left</property>
                                     </layout>
-                                    <child>
-                                      <object class="ttk.Panedwindow.Pane" id="otree1">
-                                        <property name="weight">0</property>
-                                        <child>
-                                          <object class="ttk.Frame" id="addwframe1">
-                                            <property name="padding">0 0 0 2</property>
-                                            <layout manager="pack">
-                                              <property name="expand">true</property>
-                                              <property name="fill">both</property>
-                                              <property name="side">top</property>
-                                            </layout>
-                                            <child>
-                                              <object class="ttk.Label" id="lblottitle">
-                                                <property name="padding">1</property>
-                                                <property name="style">PanelTitle.TLabel</property>
-                                                <property name="text" translatable="yes">Tree</property>
-                                                <layout manager="pack">
-                                                  <property name="fill">x</property>
-                                                  <property name="pady">0 2</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                              </object>
-                                            </child>
-                                            <child>
-                                              <object class="ttk.Frame" id="filter_frame">
-                                                <property name="height">200</property>
-                                                <property name="padding">0 0 0 6</property>
-                                                <property name="width">200</property>
-                                                <layout manager="pack">
-                                                  <property name="fill">x</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <child>
-                                                  <object class="ttk.Label" id="lblfilter">
-                                                    <property name="font">TkSmallCaptionFont</property>
-                                                    <property name="text" translatable="yes">Filter:</property>
-                                                    <layout manager="pack">
-                                                      <property name="side">left</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="ttk.Entry" id="filter_entry">
-                                                    <property name="textvariable">filtervar</property>
-                                                    <property name="validate">none</property>
-                                                    <layout manager="pack">
-                                                      <property name="expand">true</property>
-                                                      <property name="fill">x</property>
-                                                      <property name="side">left</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="ttk.Button" id="filterclear_btn">
-                                                    <property name="image">close.gif</property>
-                                                    <property name="style">FilterClearButton.Toolbutton</property>
-                                                    <property name="text" translatable="yes">✖</property>
-                                                    <layout manager="pack">
-                                                      <property name="side">right</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                            <child>
-                                              <object class="pygubu.builder.widgets.scrollbarhelper" id="sbh1">
-                                                <property name="scrolltype">both</property>
-                                                <property name="usemousewheel">true</property>
-                                                <layout manager="pack">
-                                                  <property name="expand">true</property>
-                                                  <property name="fill">both</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <child>
-                                                  <object class="pygubu.widgets.FilterableTreeview" id="project_tree" named="True">
-                                                    <layout manager="pack">
-                                                      <property name="side">top</property>
-                                                    </layout>
-                                                    <child>
-                                                      <object class="ttk.Treeview.Column" id="treecolumn">
-                                                        <property name="column_anchor">w</property>
-                                                        <property name="heading_anchor">w</property>
-                                                        <property name="minwidth">200</property>
-                                                        <property name="stretch">true</property>
-                                                        <property name="text" translatable="yes">ID</property>
-                                                        <property name="tree_column">True</property>
-                                                        <property name="visible">True</property>
-                                                        <property name="width">200</property>
-                                                      </object>
-                                                    </child>
-                                                    <child>
-                                                      <object class="ttk.Treeview.Column" id="class">
-                                                        <property name="column_anchor">w</property>
-                                                        <property name="heading_anchor">w</property>
-                                                        <property name="minwidth">100</property>
-                                                        <property name="stretch">false</property>
-                                                        <property name="text" translatable="yes">Class</property>
-                                                        <property name="tree_column">False</property>
-                                                        <property name="visible">false</property>
-                                                        <property name="width">120</property>
-                                                      </object>
-                                                    </child>
-                                                    <child>
-                                                      <object class="ttk.Treeview.Column" id="row">
-                                                        <property name="column_anchor">w</property>
-                                                        <property name="heading_anchor">w</property>
-                                                        <property name="minwidth">20</property>
-                                                        <property name="stretch">false</property>
-                                                        <property name="text" translatable="yes">R</property>
-                                                        <property name="tree_column">False</property>
-                                                        <property name="visible">True</property>
-                                                        <property name="width">20</property>
-                                                      </object>
-                                                    </child>
-                                                    <child>
-                                                      <object class="ttk.Treeview.Column" id="col">
-                                                        <property name="column_anchor">w</property>
-                                                        <property name="heading_anchor">w</property>
-                                                        <property name="minwidth">20</property>
-                                                        <property name="stretch">false</property>
-                                                        <property name="text" translatable="yes">C</property>
-                                                        <property name="tree_column">False</property>
-                                                        <property name="visible">True</property>
-                                                        <property name="width">20</property>
-                                                      </object>
-                                                    </child>
-                                                    <child>
-                                                      <object class="ttk.Treeview.Column" id="space_trick">
-                                                        <property name="column_anchor">w</property>
-                                                        <property name="heading_anchor">w</property>
-                                                        <property name="minwidth">20</property>
-                                                        <property name="stretch">False</property>
-                                                        <property name="text" translatable="yes"/>
-                                                        <property name="tree_column">False</property>
-                                                        <property name="visible">True</property>
-                                                        <property name="width">20</property>
-                                                      </object>
-                                                    </child>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                          </object>
-                                        </child>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Panedwindow.Pane" id="previewpane">
-                                        <property name="weight">2</property>
-                                        <child>
-                                          <object class="ttk.Frame" id="Frame_1">
-                                            <property name="height">250</property>
-                                            <property name="padding">1</property>
-                                            <property name="width">250</property>
-                                            <layout manager="pack">
-                                              <property name="expand">true</property>
-                                              <property name="fill">both</property>
-                                              <property name="side">top</property>
-                                            </layout>
-                                            <child>
-                                              <object class="ttk.Label" id="lblpreview">
-                                                <property name="padding">1</property>
-                                                <property name="style">PanelTitle.TLabel</property>
-                                                <property name="text" translatable="yes">Preview</property>
-                                                <layout manager="pack">
-                                                  <property name="fill">x</property>
-                                                  <property name="pady">0 2</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                              </object>
-                                            </child>
-                                            <child>
-                                              <object class="pygubu.builder.widgets.scrollbarhelper" id="scrollbarhelper_1">
-                                                <property name="scrolltype">both</property>
-                                                <property name="usemousewheel">true</property>
-                                                <layout manager="pack">
-                                                  <property name="expand">true</property>
-                                                  <property name="fill">both</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <child>
-                                                  <object class="tk.Canvas" id="preview_canvas">
-                                                    <property name="highlightthickness">0</property>
-                                                    <property name="takefocus">true</property>
-                                                    <layout manager="pack">
-                                                      <property name="expand">true</property>
-                                                      <property name="fill">both</property>
-                                                      <property name="side">top</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                          </object>
-                                        </child>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Panedwindow.Pane" id="objectproppane">
-                                        <property name="weight">0</property>
-                                        <child>
-                                          <object class="ttk.Frame" id="frame_1">
-                                            <property name="height">200</property>
-                                            <property name="width">200</property>
-                                            <layout manager="pack">
-                                              <property name="expand">true</property>
-                                              <property name="fill">both</property>
-                                              <property name="side">top</property>
-                                            </layout>
-                                            <child>
-                                              <object class="ttk.Label" id="lbltitle2">
-                                                <property name="padding">1</property>
-                                                <property name="style">PanelTitle.TLabel</property>
-                                                <property name="text" translatable="yes">Properties</property>
-                                                <layout manager="pack">
-                                                  <property name="fill">x</property>
-                                                  <property name="pady">0 2</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                              </object>
-                                            </child>
-                                            <child>
-                                              <object class="ttk.Notebook" id="notebook1">
-                                                <property name="height">200</property>
-                                                <property name="padding">0 2 0 0</property>
-                                                <property name="width">375</property>
-                                                <layout manager="pack">
-                                                  <property name="expand">true</property>
-                                                  <property name="fill">both</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <child>
-                                                  <object class="ttk.Notebook.Tab" id="generaltab">
-                                                    <property name="padding">2 6 2 6</property>
-                                                    <property name="sticky">nsew</property>
-                                                    <property name="text" translatable="yes">Appearance</property>
-                                                    <child>
-                                                      <object class="pygubu.builder.widgets.scrolledframe" id="propertiesframe">
-                                                        <property name="padding">5</property>
-                                                        <property name="scrolltype">both</property>
-                                                        <property name="usemousewheel">true</property>
-                                                        <layout manager="pack">
-                                                          <property name="expand">true</property>
-                                                          <property name="fill">both</property>
-                                                          <property name="side">top</property>
-                                                        </layout>
-                                                      </object>
-                                                    </child>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="ttk.Notebook.Tab" id="layouttab">
-                                                    <property name="padding">2 6 2 6</property>
-                                                    <property name="sticky">nsew</property>
-                                                    <property name="text" translatable="yes">Layout</property>
-                                                    <child>
-                                                      <object class="pygubu.builder.widgets.scrolledframe" id="layoutframe">
-                                                        <property name="padding">5</property>
-                                                        <property name="scrolltype">both</property>
-                                                        <property name="usemousewheel">true</property>
-                                                        <layout manager="pack">
-                                                          <property name="expand">true</property>
-                                                          <property name="fill">both</property>
-                                                          <property name="side">top</property>
-                                                        </layout>
-                                                      </object>
-                                                    </child>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="ttk.Notebook.Tab" id="bindingtab">
-                                                    <property name="padding">2 6 2 6</property>
-                                                    <property name="text" translatable="yes">Bindings</property>
-                                                    <child>
-                                                      <object class="ttk.Frame" id="bindingscontainer">
-                                                        <property name="height">200</property>
-                                                        <property name="padding">2</property>
-                                                        <property name="width">200</property>
-                                                        <layout manager="pack">
-                                                          <property name="expand">true</property>
-                                                          <property name="fill">both</property>
-                                                          <property name="side">top</property>
-                                                        </layout>
-                                                        <child>
-                                                          <object class="pygubu.builder.widgets.scrollbarhelper" id="bindingsframe">
-                                                            <property name="scrolltype">both</property>
-                                                            <property name="usemousewheel">true</property>
-                                                            <layout manager="pack">
-                                                              <property name="expand">true</property>
-                                                              <property name="fill">both</property>
-                                                              <property name="side">top</property>
-                                                            </layout>
-                                                            <child>
-                                                              <object class="pygubu.builder.widgets.editabletreeview" id="bindingstree">
-                                                                <property name="show">headings</property>
-                                                                <layout manager="pack">
-                                                                  <property name="expand">true</property>
-                                                                  <property name="fill">both</property>
-                                                                  <property name="side">top</property>
-                                                                </layout>
-                                                                <child>
-                                                                  <object class="ttk.Treeview.Column" id="sequence">
-                                                                    <property name="column_anchor">w</property>
-                                                                    <property name="heading_anchor">w</property>
-                                                                    <property name="minwidth">20</property>
-                                                                    <property name="stretch">True</property>
-                                                                    <property name="text" translatable="yes">Sequence descriptor</property>
-                                                                    <property name="tree_column">False</property>
-                                                                    <property name="visible">True</property>
-                                                                    <property name="width">200</property>
-                                                                  </object>
-                                                                </child>
-                                                                <child>
-                                                                  <object class="ttk.Treeview.Column" id="handler">
-                                                                    <property name="column_anchor">w</property>
-                                                                    <property name="heading_anchor">w</property>
-                                                                    <property name="minwidth">20</property>
-                                                                    <property name="stretch">True</property>
-                                                                    <property name="text" translatable="yes">Event Handler</property>
-                                                                    <property name="tree_column">False</property>
-                                                                    <property name="visible">True</property>
-                                                                    <property name="width">200</property>
-                                                                  </object>
-                                                                </child>
-                                                                <child>
-                                                                  <object class="ttk.Treeview.Column" id="add">
-                                                                    <property name="column_anchor">w</property>
-                                                                    <property name="heading_anchor">w</property>
-                                                                    <property name="minwidth">50</property>
-                                                                    <property name="stretch">True</property>
-                                                                    <property name="text" translatable="yes">Add</property>
-                                                                    <property name="tree_column">False</property>
-                                                                    <property name="visible">True</property>
-                                                                    <property name="width">50</property>
-                                                                  </object>
-                                                                </child>
-                                                                <child>
-                                                                  <object class="ttk.Treeview.Column" id="actions">
-                                                                    <property name="column_anchor">w</property>
-                                                                    <property name="heading_anchor">w</property>
-                                                                    <property name="minwidth">50</property>
-                                                                    <property name="stretch">True</property>
-                                                                    <property name="tree_column">False</property>
-                                                                    <property name="visible">True</property>
-                                                                    <property name="width">50</property>
-                                                                  </object>
-                                                                </child>
-                                                              </object>
-                                                            </child>
-                                                          </object>
-                                                        </child>
-                                                      </object>
-                                                    </child>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                          </object>
-                                        </child>
-                                      </object>
-                                    </child>
                                   </object>
                                 </child>
                               </object>
                             </child>
-                          </object>
-                        </child>
-                        <child>
-                          <object class="ttk.Notebook.Tab" id="tab_code">
-                            <property name="sticky">nsew</property>
-                            <property name="text" translatable="yes">Code</property>
                             <child>
-                              <object class="ttk.Frame" id="fcodemain">
+                              <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo5">
+                                <property name="field_name">output_dir</property>
+                                <property name="style">LabelFieldInfo.TLabel</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">11</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Label" id="label9">
+                                <property name="text" translatable="yes">Builder output:</property>
+                                <layout manager="grid">
+                                  <property name="column">0</property>
+                                  <property name="row">12</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Frame" id="frame5">
                                 <property name="height">200</property>
-                                <property name="padding">4</property>
                                 <property name="width">200</property>
-                                <layout manager="pack">
-                                  <property name="side">top</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">12</property>
+                                  <property name="sticky">ew</property>
                                 </layout>
                                 <child>
-                                  <object class="ttk.Frame" id="templatechoices">
-                                    <property name="height">200</property>
-                                    <property name="width">200</property>
+                                  <object class="pygubu.forms.ttkwidget.Entry" id="output_dir2" named="True">
+                                    <property name="style">EntryField.TEntry</property>
                                     <layout manager="pack">
+                                      <property name="expand">true</property>
                                       <property name="fill">x</property>
-                                      <property name="side">top</property>
+                                      <property name="ipady">3</property>
+                                      <property name="side">left</property>
                                     </layout>
-                                    <child>
-                                      <object class="ttk.Label" id="lbl_tpldesc">
-                                        <property name="font">{Default} 10 {bold}</property>
-                                        <property name="text" translatable="yes">Template description here.</property>
-                                        <property name="textvariable">string:template_desc_var</property>
-                                        <property name="wraplength">500</property>
-                                        <layout manager="pack">
-                                          <property name="fill">x</property>
-                                          <property name="pady">5 10</property>
-                                          <property name="side">bottom</property>
-                                        </layout>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Label" id="lbl_template">
-                                        <property name="text" translatable="yes">Template:</property>
-                                        <layout manager="pack">
-                                          <property name="padx">0 5</property>
-                                          <property name="side">left</property>
-                                        </layout>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Radiobutton" id="Radiobutton_1">
-                                        <property name="command" type="command" cbtype="simple" args="">on_code_template_changed</property>
-                                        <property name="style">Template.Toolbutton</property>
-                                        <property name="text" translatable="yes">Application</property>
-                                        <property name="value">application</property>
-                                        <property name="variable">string:template_var</property>
-                                        <layout manager="pack">
-                                          <property name="side">left</property>
-                                        </layout>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Separator" id="Separator_1">
-                                        <property name="orient">vertical</property>
-                                        <layout manager="pack">
-                                          <property name="fill">y</property>
-                                          <property name="padx">5</property>
-                                          <property name="side">left</property>
-                                        </layout>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Radiobutton" id="Radiobutton_2">
-                                        <property name="command" type="command" cbtype="simple" args="">on_code_template_changed</property>
-                                        <property name="style">Template.Toolbutton</property>
-                                        <property name="text" translatable="yes">Code Script</property>
-                                        <property name="value">codescript</property>
-                                        <property name="variable">string:template_var</property>
-                                        <layout manager="pack">
-                                          <property name="side">left</property>
-                                        </layout>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Separator" id="Separator_2">
-                                        <property name="orient">vertical</property>
-                                        <layout manager="pack">
-                                          <property name="fill">y</property>
-                                          <property name="padx">5</property>
-                                          <property name="side">left</property>
-                                        </layout>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Radiobutton" id="Radiobutton_3">
-                                        <property name="command" type="command" cbtype="simple" args="">on_code_template_changed</property>
-                                        <property name="style">Template.Toolbutton</property>
-                                        <property name="text" translatable="yes">Custom Widget</property>
-                                        <property name="value">widget</property>
-                                        <property name="variable">string:template_var</property>
-                                        <layout manager="pack">
-                                          <property name="side">left</property>
-                                        </layout>
-                                      </object>
-                                    </child>
                                   </object>
                                 </child>
                                 <child>
-                                  <object class="ttk.Panedwindow" id="panedwindow1">
-                                    <property name="height">200</property>
-                                    <property name="orient">horizontal</property>
-                                    <property name="width">200</property>
+                                  <object class="pygubu.widgets.PathChooserButton" id="btn_path2_chooser" named="True">
+                                    <property name="image">mglass.png</property>
+                                    <property name="text" translatable="yes">…</property>
+                                    <property name="title" translatable="yes">Select output directory</property>
+                                    <property name="type">directory</property>
+                                    <property name="width">4</property>
+                                    <bind sequence="&lt;&lt;PathChooserPathChanged&gt;&gt;" handler="output_dir2_changed" add=""/>
                                     <layout manager="pack">
-                                      <property name="expand">true</property>
-                                      <property name="fill">both</property>
-                                      <property name="side">top</property>
+                                      <property name="padx">10 0</property>
+                                      <property name="side">left</property>
                                     </layout>
-                                    <child>
-                                      <object class="ttk.Panedwindow.Pane" id="pane1">
-                                        <property name="weight">1</property>
-                                        <child>
-                                          <object class="ttk.Frame" id="newtop">
-                                            <property name="height">200</property>
-                                            <property name="width">200</property>
-                                            <layout manager="pack">
-                                              <property name="fill">x</property>
-                                              <property name="side">top</property>
-                                            </layout>
-                                            <child>
-                                              <object class="ttk.Labelframe" id="codeoptions">
-                                                <property name="height">130</property>
-                                                <property name="padding">4</property>
-                                                <property name="text" translatable="yes">Options:</property>
-                                                <property name="width">100</property>
-                                                <layout manager="pack">
-                                                  <property name="expand">true</property>
-                                                  <property name="fill">both</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <containerlayout manager="pack">
-                                                  <property name="propagate">False</property>
-                                                </containerlayout>
-                                                <child>
-                                                  <object class="pygubu.builder.widgets.scrolledframe" id="scrolledframe1">
-                                                    <property name="scrolltype">both</property>
-                                                    <property name="usemousewheel">false</property>
-                                                    <layout manager="pack">
-                                                      <property name="expand">true</property>
-                                                      <property name="fill">both</property>
-                                                      <property name="side">top</property>
-                                                    </layout>
-                                                    <child>
-                                                      <object class="ttk.Frame" id="frame1">
-                                                        <property name="height">200</property>
-                                                        <property name="width">200</property>
-                                                        <layout manager="pack">
-                                                          <property name="fill">x</property>
-                                                          <property name="side">top</property>
-                                                        </layout>
-                                                        <containerlayout manager="grid">
-                                                          <property type="col" id="0" name="pad">5</property>
-                                                          <property type="row" id="0" name="pad">5</property>
-                                                          <property type="row" id="1" name="pad">5</property>
-                                                        </containerlayout>
-                                                        <child>
-                                                          <object class="ttk.Label" id="lbl_wlist">
-                                                            <property name="text" translatable="yes">Main widget:</property>
-                                                            <layout manager="grid">
-                                                              <property name="column">0</property>
-                                                              <property name="row">0</property>
-                                                              <property name="sticky">ew</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="pygubu.builder.widgets.combobox" id="widgetlist">
-                                                            <property name="keyvariable">string:widgetlist_keyvar</property>
-                                                            <property name="textvariable">string:widgetlistvar</property>
-                                                            <property name="validate">focusin</property>
-                                                            <property name="validatecommand" type="command" cbtype="entry_validate" args="">on_code_template_property_changed</property>
-                                                            <layout manager="grid">
-                                                              <property name="column">1</property>
-                                                              <property name="row">0</property>
-                                                              <property name="sticky">ew</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Label" id="label_2">
-                                                            <property name="text" translatable="yes">Class Name:</property>
-                                                            <layout manager="grid">
-                                                              <property name="row">1</property>
-                                                              <property name="sticky">ew</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Entry" id="classname">
-                                                            <property name="textvariable">string:classnamevar</property>
-                                                            <property name="validate">focusout</property>
-                                                            <property name="validatecommand" type="command" cbtype="entry_validate" args="">on_code_template_property_changed</property>
-                                                            <layout manager="grid">
-                                                              <property name="column">1</property>
-                                                              <property name="row">1</property>
-                                                              <property name="sticky">ew</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Frame" id="spacerframe1">
-                                                            <property name="height">10</property>
-                                                            <property name="width">10</property>
-                                                            <layout manager="grid">
-                                                              <property name="column">2</property>
-                                                              <property name="row">1</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Label" id="label2">
-                                                            <property name="text" translatable="yes">Main menu:</property>
-                                                            <layout manager="grid">
-                                                              <property name="column">0</property>
-                                                              <property name="row">2</property>
-                                                              <property name="sticky">ew</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="pygubu.builder.widgets.combobox" id="menulist">
-                                                            <property name="keyvariable">string:menulist_keyvar</property>
-                                                            <property name="textvariable">string:menulist_var</property>
-                                                            <property name="validate">focusin</property>
-                                                            <property name="validatecommand" type="command" cbtype="entry_validate" args="">on_code_template_property_changed</property>
-                                                            <layout manager="grid">
-                                                              <property name="column">1</property>
-                                                              <property name="row">2</property>
-                                                              <property name="sticky">ew</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                      </object>
-                                                    </child>
-                                                    <child>
-                                                      <object class="ttk.Frame" id="frame2">
-                                                        <property name="height">200</property>
-                                                        <property name="padding">0 5 0 0</property>
-                                                        <property name="width">200</property>
-                                                        <layout manager="pack">
-                                                          <property name="fill">x</property>
-                                                          <property name="side">top</property>
-                                                        </layout>
-                                                        <child>
-                                                          <object class="ttk.Checkbutton" id="cb_import_tkvars">
-                                                            <property name="command" type="command" cbtype="simple">on_code_template_property_changed</property>
-                                                            <property name="text" translatable="yes">Import Tk Variables</property>
-                                                            <property name="variable">boolean:import_tkvars_var</property>
-                                                            <layout manager="pack">
-                                                              <property name="anchor">w</property>
-                                                              <property name="side">top</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Checkbutton" id="cb_use_ttk_definitions">
-                                                            <property name="command" type="command" cbtype="simple">on_code_template_property_changed</property>
-                                                            <property name="text" translatable="yes">Use ttk style definitions file</property>
-                                                            <property name="variable">boolean:use_ttkdefs_file_var</property>
-                                                            <layout manager="pack">
-                                                              <property name="anchor">w</property>
-                                                              <property name="side">top</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Checkbutton" id="cb_add_i18n">
-                                                            <property name="command" type="command" cbtype="simple">on_code_template_property_changed</property>
-                                                            <property name="text" translatable="yes">Add i18n support</property>
-                                                            <property name="variable">boolean:add_i18n_var</property>
-                                                            <layout manager="pack">
-                                                              <property name="anchor">w</property>
-                                                              <property name="side">top</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Checkbutton" id="cb_all_ids_attributes" named="True">
-                                                            <property name="command" type="command" cbtype="simple">on_code_template_property_changed</property>
-                                                            <property name="text" translatable="yes">All IDs as class attributes</property>
-                                                            <property name="variable">boolean:all_ids_attributes_var</property>
-                                                            <layout manager="pack">
-                                                              <property name="anchor">w</property>
-                                                              <property name="side">top</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                        <child>
-                                                          <object class="ttk.Checkbutton" id="cb_window_centering_code" named="True">
-                                                            <property name="command" type="command" cbtype="simple">on_code_template_property_changed</property>
-                                                            <property name="text" translatable="yes">Add window centering code</property>
-                                                            <property name="variable">boolean:add_window_centering_code_var</property>
-                                                            <layout manager="pack">
-                                                              <property name="anchor">w</property>
-                                                              <property name="side">top</property>
-                                                            </layout>
-                                                          </object>
-                                                        </child>
-                                                      </object>
-                                                    </child>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                          </object>
-                                        </child>
-                                      </object>
-                                    </child>
-                                    <child>
-                                      <object class="ttk.Panedwindow.Pane" id="pane2">
-                                        <property name="weight">2</property>
-                                        <child>
-                                          <object class="ttk.Frame" id="codepreview">
-                                            <property name="height">200</property>
-                                            <property name="width">200</property>
-                                            <layout manager="pack">
-                                              <property name="expand">true</property>
-                                              <property name="fill">both</property>
-                                              <property name="side">top</property>
-                                            </layout>
-                                            <child>
-                                              <object class="ttk.Frame" id="Frame_5">
-                                                <property name="height">200</property>
-                                                <property name="width">200</property>
-                                                <layout manager="pack">
-                                                  <property name="expand">true</property>
-                                                  <property name="fill">both</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <child>
-                                                  <object class="ttk.Label" id="Label_1">
-                                                    <property name="text" translatable="yes">Preview</property>
-                                                    <layout manager="pack">
-                                                      <property name="fill">x</property>
-                                                      <property name="side">top</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="pygubu.builder.widgets.scrollbarhelper" id="scrollbarhelper_2">
-                                                    <property name="scrolltype">both</property>
-                                                    <property name="usemousewheel">true</property>
-                                                    <layout manager="pack">
-                                                      <property name="expand">true</property>
-                                                      <property name="fill">both</property>
-                                                      <property name="side">top</property>
-                                                    </layout>
-                                                    <child>
-                                                      <object class="tk.Text" id="txt_code">
-                                                        <property name="font">TkFixedFont</property>
-                                                        <property name="height">10</property>
-                                                        <property name="width">40</property>
-                                                        <layout manager="pack">
-                                                          <property name="expand">true</property>
-                                                          <property name="fill">both</property>
-                                                          <property name="side">top</property>
-                                                        </layout>
-                                                      </object>
-                                                    </child>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                            <child>
-                                              <object class="ttk.Frame" id="btnbar2">
-                                                <property name="height">200</property>
-                                                <property name="padding">2</property>
-                                                <property name="width">200</property>
-                                                <layout manager="pack">
-                                                  <property name="fill">x</property>
-                                                  <property name="side">top</property>
-                                                </layout>
-                                                <child>
-                                                  <object class="ttk.Button" id="btn_generate">
-                                                    <property name="command" type="command" cbtype="simple" args="">on_code_generate_clicked</property>
-                                                    <property name="text" translatable="yes">Generate</property>
-                                                    <layout manager="pack">
-                                                      <property name="padx">0 10</property>
-                                                      <property name="side">left</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="ttk.Button" id="btn_toclipboard">
-                                                    <property name="command" type="command" cbtype="simple" args="">on_code_copy_clicked</property>
-                                                    <property name="text" translatable="yes">Copy to Clipboard</property>
-                                                    <layout manager="pack">
-                                                      <property name="padx">0 10</property>
-                                                      <property name="side">left</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                                <child>
-                                                  <object class="ttk.Button" id="btn_save">
-                                                    <property name="command" type="command" cbtype="simple" args="">on_code_save_clicked</property>
-                                                    <property name="text" translatable="yes">Save</property>
-                                                    <layout manager="pack">
-                                                      <property name="side">left</property>
-                                                    </layout>
-                                                  </object>
-                                                </child>
-                                              </object>
-                                            </child>
-                                          </object>
-                                        </child>
-                                      </object>
-                                    </child>
                                   </object>
                                 </child>
                               </object>
                             </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelwidgetinfo1">
+                                <property name="field_name">output_dir2</property>
+                                <property name="style">LabelFieldInfo.TLabel</property>
+                                <layout manager="grid">
+                                  <property name="column">1</property>
+                                  <property name="row">13</property>
+                                  <property name="sticky">ew</property>
+                                </layout>
+                              </object>
+                            </child>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="ttk.Frame" id="frame2">
+                            <property name="height">200</property>
+                            <property name="padding">0 5 0 0</property>
+                            <property name="width">200</property>
+                            <layout manager="pack">
+                              <property name="fill">x</property>
+                              <property name="side">top</property>
+                            </layout>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Checkbutton" id="import_tkvariables" named="True">
+                                <property name="text" translatable="yes">Import Tk Variables</property>
+                                <property name="variable">boolean:import_tkvariables_var</property>
+                                <layout manager="pack">
+                                  <property name="anchor">w</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Checkbutton" id="use_ttk_styledefinition_file" named="True">
+                                <property name="text" translatable="yes">Use ttk style definitions file</property>
+                                <property name="variable">boolean:use_ttk_style_var</property>
+                                <layout manager="pack">
+                                  <property name="anchor">w</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Checkbutton" id="use_i18n" named="True">
+                                <property name="text" translatable="yes">Add i18n support</property>
+                                <property name="variable">boolean:use_i18n_var</property>
+                                <layout manager="pack">
+                                  <property name="anchor">w</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Checkbutton" id="all_ids_attributes" named="True">
+                                <property name="text" translatable="yes">All IDs as class attributes</property>
+                                <property name="variable">boolean:all_ids_attr_var</property>
+                                <layout manager="pack">
+                                  <property name="anchor">w</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Checkbutton" id="generate_code_onsave" named="True">
+                                <property name="text" translatable="yes">Regenerate code when saving the project</property>
+                                <property name="variable">boolean:generate_code_onsave_var</property>
+                                <layout manager="pack">
+                                  <property name="anchor">w</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.forms.ttkwidget.Checkbutton" id="use_window_centering_code" named="True">
+                                <property name="text" translatable="yes">Add window centering code</property>
+                                <property name="variable">boolean:use_windowcenter_code_var</property>
+                                <layout manager="pack">
+                                  <property name="anchor">w</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
                           </object>
                         </child>
                       </object>
                     </child>
                   </object>
                 </child>
-              </object>
-            </child>
-            <child>
-              <object class="ttk.Panedwindow.Pane" id="mainpw_bottom">
-                <property name="weight">0</property>
                 <child>
-                  <object class="ttk.Frame" id="bpanel">
-                    <property name="height">200</property>
-                    <property name="width">200</property>
-                    <layout manager="pack">
-                      <property name="side">top</property>
-                    </layout>
+                  <object class="ttk.Notebook.Tab" id="tab3">
+                    <property name="sticky">nsew</property>
+                    <property name="text" translatable="yes">Styles</property>
                     <child>
-                      <object class="ttk.Frame" id="bp_container">
-                        <property name="height">200</property>
-                        <property name="width">200</property>
+                      <object class="pygubu.forms.ttkwidget.FrameFormBuilder" id="frm_style" named="True">
+                        <property name="padding">5</property>
                         <layout manager="pack">
-                          <property name="expand">true</property>
-                          <property name="fill">both</property>
                           <property name="side">top</property>
                         </layout>
                         <child>
-                          <object class="pygubu.builder.widgets.scrollbarhelper" id="scrollbarhelper_3">
-                            <property name="scrolltype">both</property>
-                            <property name="usemousewheel">false</property>
+                          <object class="ttk.Label" id="label1">
+                            <property name="text" translatable="yes">Style definition file:</property>
                             <layout manager="pack">
-                              <property name="expand">true</property>
-                              <property name="fill">both</property>
+                              <property name="anchor">w</property>
+                              <property name="side">top</property>
+                            </layout>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="ttk.Frame" id="frame4">
+                            <property name="height">200</property>
+                            <property name="width">200</property>
+                            <layout manager="pack">
+                              <property name="fill">x</property>
                               <property name="side">top</property>
                             </layout>
                             <child>
-                              <object class="tk.Text" id="txt_log">
-                                <property name="font">TkFixedFont</property>
-                                <property name="height">8</property>
-                                <property name="state">disabled</property>
-                                <property name="width">50</property>
+                              <object class="pygubu.forms.ttkwidget.Entry" id="ttk_style_definition_file" named="True">
+                                <property name="style">EntryField.TEntry</property>
                                 <layout manager="pack">
-                                  <property name="side">top</property>
+                                  <property name="expand">true</property>
+                                  <property name="fill">x</property>
+                                  <property name="ipady">3</property>
+                                  <property name="side">left</property>
                                 </layout>
                               </object>
                             </child>
+                            <child>
+                              <object class="pygubu.widgets.PathChooserButton" id="btn_stylepath_find" named="True">
+                                <property name="defaultextension">.py</property>
+                                <property name="image">mglass.png</property>
+                                <property name="text" translatable="yes">…</property>
+                                <property name="title" translatable="yes">Select style definitions file</property>
+                                <property name="type">file</property>
+                                <property name="width">4</property>
+                                <bind sequence="&lt;&lt;PathChooserPathChanged&gt;&gt;" handler="on_style_new_selected" add=""/>
+                                <layout manager="pack">
+                                  <property name="padx">10 0</property>
+                                  <property name="side">left</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="pygubu.widgets.PathChooserButton" id="btn_stylepath_new" named="True">
+                                <property name="defaultextension">.py</property>
+                                <property name="mustexist">false</property>
+                                <property name="text" translatable="yes">+</property>
+                                <property name="title" translatable="yes">Select style definitions file</property>
+                                <property name="type">file</property>
+                                <property name="width">3</property>
+                                <bind sequence="&lt;&lt;PathChooserPathChanged&gt;&gt;" handler="on_style_new_create" add=""/>
+                                <layout manager="pack">
+                                  <property name="padx">5 0</property>
+                                  <property name="side">left</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Separator" id="separator1">
+                                <property name="orient">vertical</property>
+                                <layout manager="pack">
+                                  <property name="fill">y</property>
+                                  <property name="padx">5</property>
+                                  <property name="side">left</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Button" id="button2">
+                                <property name="command" type="command" cbtype="simple">on_style_remove</property>
+                                <property name="image">bin-16.png</property>
+                                <property name="text" translatable="yes">Remove</property>
+                                <layout manager="pack">
+                                  <property name="side">left</property>
+                                </layout>
+                              </object>
+                            </child>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="pygubu.forms.ttkwidget.LabelWidgetInfo" id="labelfieldinfo8">
+                            <property name="field_name">ttk_style_definition_file</property>
+                            <property name="style">LabelFieldInfo.TLabel</property>
+                            <layout manager="pack">
+                              <property name="fill">x</property>
+                              <property name="pady">0 5</property>
+                              <property name="side">top</property>
+                            </layout>
                           </object>
                         </child>
                       </object>
                     </child>
+                  </object>
+                </child>
+                <child>
+                  <object class="ttk.Notebook.Tab" id="tab4">
+                    <property name="sticky">nsew</property>
+                    <property name="text" translatable="yes">Custom Widgets</property>
                     <child>
-                      <object class="ttk.Frame" id="bp_buttons">
+                      <object class="ttk.Frame" id="frame13">
                         <property name="height">200</property>
-                        <property name="padding">1</property>
+                        <property name="padding">5</property>
                         <property name="width">200</property>
                         <layout manager="pack">
-                          <property name="fill">x</property>
-                          <property name="side">bottom</property>
+                          <property name="side">top</property>
                         </layout>
                         <child>
-                          <object class="ttk.Checkbutton" id="btn_messages">
-                            <property name="command" type="command" cbtype="simple" args="">on_bpanel_button_clicked</property>
-                            <property name="offvalue">0</property>
-                            <property name="onvalue">messages</property>
-                            <property name="style">Toolbutton</property>
-                            <property name="text" translatable="yes">Messages</property>
-                            <property name="variable">string:bpanel_buttonsvar</property>
+                          <object class="ttk.Label" id="label8">
+                            <property name="text" translatable="yes">Project widget builders:</property>
                             <layout manager="pack">
+                              <property name="anchor">w</property>
+                              <property name="pady">5</property>
+                              <property name="side">top</property>
+                            </layout>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="pygubu.builder.widgets.scrollbarhelper" id="scrollbarhelper1">
+                            <property name="scrolltype">both</property>
+                            <property name="usemousewheel">false</property>
+                            <layout manager="pack">
+                              <property name="expand">true</property>
+                              <property name="fill">both</property>
                               <property name="side">left</property>
                             </layout>
+                            <child>
+                              <object class="ttk.Treeview" id="cwtree" named="True">
+                                <property name="selectmode">extended</property>
+                                <layout manager="pack">
+                                  <property name="side">left</property>
+                                </layout>
+                                <child>
+                                  <object class="ttk.Treeview.Column" id="column1">
+                                    <property name="column_anchor">w</property>
+                                    <property name="heading_anchor">center</property>
+                                    <property name="minwidth">20</property>
+                                    <property name="stretch">true</property>
+                                    <property name="text" translatable="yes">Modules</property>
+                                    <property name="tree_column">true</property>
+                                    <property name="visible">true</property>
+                                    <property name="width">200</property>
+                                  </object>
+                                </child>
+                              </object>
+                            </child>
+                          </object>
+                        </child>
+                        <child>
+                          <object class="ttk.Frame" id="frame7">
+                            <property name="height">200</property>
+                            <property name="padding">4 0 4 0</property>
+                            <property name="width">200</property>
+                            <layout manager="pack">
+                              <property name="fill">y</property>
+                              <property name="side">left</property>
+                            </layout>
+                            <child>
+                              <object class="pygubu.widgets.PathChooserButton" id="btn_cwadd_module" named="True">
+                                <property name="defaultextension">.py</property>
+                                <property name="text" translatable="yes">+</property>
+                                <property name="title" translatable="yes">Select a widget builder file</property>
+                                <property name="type">file</property>
+                                <property name="width">-3</property>
+                                <bind sequence="&lt;&lt;PathChooserPathChanged&gt;&gt;" handler="btn_cwadd_clicked" add=""/>
+                                <layout manager="pack">
+                                  <property name="pady">0 8</property>
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
+                            <child>
+                              <object class="ttk.Button" id="btn_cwremove" named="True">
+                                <property name="command" type="command" cbtype="simple">btn_cwremove_clicked</property>
+                                <property name="text" translatable="yes">-</property>
+                                <property name="width">-3</property>
+                                <layout manager="pack">
+                                  <property name="side">top</property>
+                                </layout>
+                              </object>
+                            </child>
                           </object>
                         </child>
                       </object>
                     </child>
                   </object>
                 </child>
               </object>
             </child>
           </object>
         </child>
+        <child>
+          <object class="ttk.Frame" id="frame10">
+            <property name="height">200</property>
+            <property name="width">200</property>
+            <layout manager="pack">
+              <property name="anchor">e</property>
+              <property name="pady">5 0</property>
+              <property name="side">top</property>
+            </layout>
+            <child>
+              <object class="ttk.Button" id="button7">
+                <property name="command" type="command" cbtype="simple">btn_cancel_clicked</property>
+                <property name="text" translatable="yes">Cancel</property>
+                <layout manager="pack">
+                  <property name="padx">0 10</property>
+                  <property name="side">left</property>
+                </layout>
+              </object>
+            </child>
+            <child>
+              <object class="ttk.Button" id="button6">
+                <property name="command" type="command" cbtype="simple">btn_apply_clicked</property>
+                <property name="text" translatable="yes">Ok</property>
+                <layout manager="pack">
+                  <property name="side">left</property>
+                </layout>
+              </object>
+            </child>
+          </object>
+        </child>
       </object>
     </child>
   </object>
 </interface>
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/dialogs.py` & `pygubu_designer-0.39/src/pygubudesigner/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/i18n.py` & `pygubu_designer-0.39/src/pygubudesigner/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/layouteditor.py` & `pygubu_designer-0.39/src/pygubudesigner/layouteditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,18 +131,18 @@
                     else:
                         label.grid_remove()
                         widget.grid_remove()
         else:
             self._fprop.grid_remove()
 
         # determine if show container layout options
-        has_children = self._container_options.get("has_children", False)
+        # has_children = self._container_options.get("has_children", False)
         children_grid_dim = self._container_options.get("grid_dim", None)
 
-        if is_container and allow_container_layout and has_children:
+        if is_container and allow_container_layout:  # and has_children:
             self._cleditor.grid()
             cmanager = wdescr.container_manager
             self._cleditor.edit(wdescr, cmanager, children_grid_dim)
         else:
             self._cleditor.grid_remove()
 
         self._sframe.reposition()
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/logpanel.py` & `pygubu_designer-0.39/src/pygubudesigner/logpanel.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/main.py` & `pygubu_designer-0.39/src/pygubudesigner/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,39 +21,50 @@
 import importlib
 import logging
 import pkgutil
 import platform
 import sys
 import tkinter as tk
 import webbrowser
+import traceback
 from pathlib import Path
 from tkinter import filedialog, messagebox
 
 import pygubu
 from pygubu import builder
 from pygubu.component.plugin_manager import PluginManager
 from pygubu.stockimage import StockImage, StockImageException
 
 import pygubudesigner
 import pygubudesigner.actions as actions
+import pygubudesigner.designerstyles as designerstyles
+
 from pygubudesigner import preferences as pref
+from pygubudesigner.services.project import Project
+from pygubudesigner.services.designersettings import DesignerSettings
+from pygubudesigner.services.projectsettings import ProjectSettings
+from pygubudesigner.services.aboutdialog import AboutDialog
 from pygubudesigner.codegen import ScriptGenerator
 from pygubudesigner.dialogs import AskSaveChangesDialog, ask_save_changes
 from pygubudesigner.widgets.componentpalette import ComponentPalette
 from pygubudesigner.widgets.toolbarframe import ToolbarFrame
 
 from .i18n import translator
 from .logpanel import LogPanelManager
 from .preview import PreviewHelper
 from .properties import load_custom_properties
 from .rfilemanager import RecentFilesManager
 from .uitreeeditor import WidgetsTreeEditor
-from .util import get_ttk_style, menu_iter_children, virtual_event
+from .util import menu_iter_children, virtual_event, enable_dpi
 from .util.keyboard import Key, key_bind
 from .util.screens import is_visible_in_screens, parse_geometry
+from .services.stylehandler import StyleHandler
+from .services.messagebox import show_error
+from .services.theming import get_ttk_style
+
 
 # Initialize logger
 logger = logging.getLogger(__name__)
 
 
 # translator function
 _ = translator
@@ -67,36 +78,20 @@
         all_modules.extend(plugin.get_all_modules())
     for _module in all_modules:
         try:
             importlib.import_module(_module)
         except (ModuleNotFoundError, ImportError) as e:
             logger.exception(e)
             msg = _(f"Failed to load widget module: '{_module}'")
-            messagebox.showerror(_("Error"), msg)
+            det = traceback.format_exc()
+            show_error(None, _("Error"), msg, det)
 
     # Initialize designer plugins
     PluginManager.load_designer_plugins()
 
-    # initialize custom widgets
-    for path in map(Path, pref.get_custom_widgets()):
-        if not path.match("*.py"):
-            continue
-
-        dirname = str(path.parent)
-        modulename = path.name[:-3]
-        if dirname not in sys.path:
-            sys.path.append(dirname)
-
-        try:
-            importlib.import_module(modulename)
-        except Exception as e:
-            logger.exception(e)
-            msg = _(f"Failed to load custom widget module: '{path}'")
-            messagebox.showerror(_("Error"), msg)
-
     # Register custom properties
     load_custom_properties()
 
 
 # Initialize images
 DATA_DIR = Path(__file__).parent / "data"
 
@@ -141,24 +136,31 @@
     def __init__(self):
         """Creates all gui widgets"""
 
         self.translator = translator
         self.preview = None
         self.about_dialog = None
         self.preferences = None
-        self.script_generator = None
-        self.builder = pygubu.Builder(translator)
-        self.currentfile = None
+        self.project_settings = None
+        self.builder = pygubu.Builder(
+            translator, on_first_object=designerstyles.setup_ttk_styles
+        )
+        self.current_project = None
         self.is_changed = False
         self.current_title = "new"
+        self.mbox_title = _("Pygubu Designer")
 
         self.builder.add_from_file(str(DATA_DIR / "ui" / "pygubu-ui.ui"))
         self.builder.add_resource_path(str(DATA_DIR / "images"))
 
         in_macos = sys.platform == "darwin"
+
+        # Enable DPI aware
+        enable_dpi()
+
         # build main ui
         self.mainwindow = self.builder.get_object("mainwindow")
         self.main_menu = self.builder.get_object("mainmenu", self.mainwindow)
         self.context_menu = self.builder.get_object(
             "context_menu", self.mainwindow
         )
 
@@ -201,22 +203,14 @@
         )
 
         # Bottom Panel
         self.setup_bottom_panel()
 
         self.builder.connect_callbacks(self)
 
-        # setup app preferences
-        self.setup_app_preferences()
-
-        #
-        # Setup tkk styles
-        #
-        self._setup_styles()
-
         # Customize OpenFiledialog window
         if sys.platform == "linux":
             file_dialog_hack = """
 # Show button and hide hidden files
 catch {tk_getOpenFile -badoption}
 set ::tk::dialog::file::showHiddenBtn 1
 set ::tk::dialog::file::showHiddenVar 0
@@ -242,33 +236,48 @@
         except StockImageException:
             pass
 
         # Load all widgets before creating the component pallete
         init_pygubu_widgets()
 
         # _pallete
-        self.fpalette = self.builder.get_object("fpalette")
-        self.create_component_palette(self.fpalette)
+        # self.fpalette = self.builder.get_object("fpalette")
+        # self.create_component_palette(self.fpalette)
+
+        # Tree palette
+        self.tree_palette = self.builder.get_object("tree_palette")
+        self.tree_palette.on_add_widget = self.on_add_widget_event
+        self.tree_palette.build_tree()
 
         # tree editor
         self.tree_editor = WidgetsTreeEditor(self)
-
-        # Tab Code
-        self.script_generator = ScriptGenerator(self)
-
+        # code generator
+        self.script_generator: ScriptGenerator = ScriptGenerator(self)
         # App bindings
         self._setup_app_bindings()
 
+        # setup app preferences
+        self.setup_app_preferences()
+
+        # project settings
+        self.project_settings = ProjectSettings(self.mainwindow, translator)
+        self.project_settings.on_settings_changed = (
+            self._on_project_settings_changed
+        )
+        # load maindock state
+        self.load_dockframe_layout()
+
     def run(self):
         self.mainwindow.protocol("WM_DELETE_WINDOW", self.__on_window_close)
         self.mainwindow.mainloop()
 
     def __on_window_close(self):
         """Manage WM_DELETE_WINDOW protocol."""
         if self.on_close_execute():
+            self.previewer.close_toplevel_previews()
             self.mainwindow.withdraw()
             self.mainwindow.destroy()
 
     def quit(self):
         """Exit the app if it is ready for quit."""
         self.__on_window_close()
 
@@ -412,50 +421,14 @@
         w.bind(actions.FILE_SAVE, self.on_file_save)
         w.bind(actions.FILE_SAVEAS, lambda e: self.do_save_as())
         w.bind(actions.FILE_QUIT, lambda e: self.quit())
         w.bind(actions.FILE_RECENT_CLEAR, lambda e: self.rfiles_manager.clear())
         # On preferences save binding
         w.bind("<<PygubuDesignerPreferencesSaved>>", self.on_preferences_saved)
 
-    def _setup_styles(self):
-        self.mainwindow.option_add("*Dialog.msg.width", 34)
-        self.mainwindow.option_add("*Dialog.msg.wrapLength", "6i")
-
-        s = get_ttk_style()
-        s.configure(
-            "ColorSelectorButton.Toolbutton", image=StockImage.get("mglass")
-        )
-        s.configure(
-            "ImageSelectorButton.Toolbutton", image=StockImage.get("mglass")
-        )
-        s.configure("ComponentPalette.Toolbutton", font="TkSmallCaptionFont")
-        s.configure("ComponentPalette.TNotebook.Tab", font="TkSmallCaptionFont")
-        s.configure(
-            "PanelTitle.TLabel",
-            background="#808080",
-            foreground="white",
-            font="TkSmallCaptionFont",
-        )
-        s.configure("Template.Toolbutton", padding=5)
-        # ToolbarFrame scroll buttons
-        s.configure(
-            ToolbarFrame.BTN_LEFT_STYLE, image=StockImage.get("arrow-left2")
-        )
-        s.configure(
-            ToolbarFrame.BTN_RIGHT_STYLE, image=StockImage.get("arrow-right2")
-        )
-        # Preview panel, Selection indicator color
-        s.configure("PreviewIndicator.TFrame", background="red")
-
-        if sys.platform == "linux":
-            # change background of comboboxes
-            color = s.lookup("TEntry", "fieldbackground")
-            s.map("TCombobox", fieldbackground=[("readonly", color)])
-            s.map("TSpinbox", fieldbackground=[("readonly", color)])
-
     def _setup_theme_menu(self):
         menu = self.builder.get_object("preview_themes_submenu")
         s = get_ttk_style()
         styles = sorted(s.theme_names())
         self.__theme_var = var = tk.StringVar()
         theme = pref.get_option("ttk_theme")
         var.set(theme)
@@ -565,18 +538,14 @@
 
     def setup_app_preferences(self):
         # Restore windows position and size
         geom = pref.get_window_size()
         self.mainwindow.geometry(geom)
         self.mainwindow.after_idle(self._check_window_visibility)
 
-        # Load preferred ttk theme
-        theme = pref.get_option("ttk_theme")
-        self._change_ttk_theme(theme)
-
     def _check_window_visibility(self):
         geom = pref.get_window_size()
         window_visible = is_visible_in_screens(geom)
         logger.debug(_("Checking main window visibility."))
         if not window_visible:
             msg = _("Main window is not visible in current monitors.")
             logger.debug(msg)
@@ -589,15 +558,16 @@
             self.mainwindow.geometry(geom)
             self.mainwindow.deiconify()
 
     def _change_ttk_theme(self, theme):
         s = get_ttk_style()
         try:
             s.theme_use(theme)
-            self._setup_styles()
+            logger.debug("ttk theme changed to: %s", theme)
+            designerstyles.setup_ttk_styles(self.mainwindow, theme)
             event_name = "<<PygubuDesignerTtkThemeChanged>>"
             self.mainwindow.event_generate(event_name)
         except tk.TclError:
             logger.exception("Invalid ttk theme.")
 
     def on_preferences_saved(self, event=None):
         # Setup ttk theme if changed
@@ -643,55 +613,71 @@
     def do_save(self, fname):
         saved = False
         try:
             self.save_file(fname)
             self.set_changed(False)
             logger.info(_("Project saved to %s"), fname)
             saved = True
+            if self.generate_code_on_save():
+                self._project_code_generate()
         except Exception as e:
-            messagebox.showerror(_("Error"), str(e), parent=self.mainwindow)
+            msg = str(e)
+            det = traceback.format_exc()
+            show_error(
+                self.mainwindow,
+                _("Error"),
+                msg,
+                det,
+            )
         return saved
 
     def do_save_as(self):
         saved = False
         options = {
             "defaultextension": ".ui",
             "filetypes": ((_("pygubu ui"), "*.ui"), (_("All"), "*.*")),
         }
         fname = filedialog.asksaveasfilename(**options)
         if fname:
             saved = self.do_save(fname)
         return saved
 
     def save_file(self, filename):
-        uidefinition = self.tree_editor.tree_to_uidef()
-        uidefinition.save(filename)
-        self.currentfile = filename
+        project = self.current_project
+        if project is None:
+            project = Project()
+        project.uidefinition = self.tree_editor.tree_to_uidef()
+        project.save(filename)
+        self.current_project = project
         title = self.project_name()
         self.set_title(title)
-        self.rfiles_manager.addfile(filename)
+        self.rfiles_manager.addfile(str(filename))
 
     def set_changed(self, newvalue=True):
         if newvalue and not self.is_changed:
             self.set_title(f"{self.current_title} (*)")
         self.is_changed = newvalue
 
     def load_file(self, filename):
         """Load xml into treeview"""
 
         try:
-            self.tree_editor.load_file(filename)
-            self.currentfile = filename
+            fpath = Path(filename).resolve()
+            project = Project.load(fpath)
+            self.tree_editor.load_file(project)
+            self.current_project = project
             title = self.project_name()
             self.set_title(title)
             self.set_changed(False)
-            self.rfiles_manager.addfile(filename)
-            self.script_generator.reset()
+            self.rfiles_manager.addfile(str(fpath))
+            self.reload_component_palette()
         except Exception as e:
-            messagebox.showerror(_("Error"), str(e), parent=self.mainwindow)
+            msg = str(e)
+            det = traceback.format_exc()
+            show_error(self.mainwindow, _("Error"), msg, det)
 
     def do_file_open(self, filename=None):
         openfile = True
         if self.is_changed:
             msg = _("Do you want to save the changes before opening?")
             openfile = self.ask_save_changes(msg)
         if openfile:
@@ -711,24 +697,24 @@
         new = True
         if self.is_changed:
             msg = _("Do you want to save the changes before creating?")
             new = self.ask_save_changes(msg)
         if new:
             self.previewer.remove_all()
             self.tree_editor.remove_all()
-            self.currentfile = None
+            self.current_project = None
             self.set_changed(False)
             self.set_title(self.project_name())
-            self.script_generator.reset()
+            StyleHandler.clear_definition_file()
 
     def on_file_save(self, event=None):
         file_saved = False
-        if self.currentfile:
+        if self.current_project:
             if self.is_changed:
-                file_saved = self.do_save(self.currentfile)
+                file_saved = self.do_save(self.current_project.fpath)
         else:
             file_saved = self.do_save_as()
         return file_saved
 
     # File Menu
     def on_file_menuitem_clicked(self, itemid):
         action = f"<<ACTION_{itemid}>>"
@@ -738,14 +724,21 @@
     def on_edit_menuitem_clicked(self, itemid):
         if itemid == "edit_preferences":
             self._edit_preferences()
         else:
             action = f"<<ACTION_{itemid}>>"
             self.mainwindow.event_generate(action)
 
+    # Project menu
+    def on_project_menuitem_clicked(self, itemid):
+        if itemid == "project_settings":
+            self._edit_project_settings()
+        if itemid == "project_codegen":
+            self._project_code_generate()
+
     # preview menu
     def on_previewmenu_action(self, itemid):
         action = f"<<ACTION_{itemid}>>"
         self.mainwindow.event_generate(action)
 
     # Help menu
     def on_help_menuitem_clicked(self, itemid):
@@ -827,103 +820,73 @@
 
     def on_context_menu_duplicate_clicked(self):
         """
         Duplicate was clicked from the context menu.
         """
         self.mainwindow.event_generate(actions.TREE_ITEM_DUPLICATE)
 
-    def _create_about_dialog(self):
-        builder = pygubu.Builder(translator)
-        builder.add_from_file(str(DATA_DIR / "ui" / "about_dialog.ui"))
-        builder.add_resource_path(str(DATA_DIR / "images"))
-
-        dialog = builder.get_object("aboutdialog", self.mainwindow)
-        entry = builder.get_object("version")
-        txt = entry.cget("text")
-        txt = txt.replace("%version%", str(pygubu.__version__))
-        entry.configure(text=txt)
-        entry = builder.get_object("designer_version")
-        txt = entry.cget("text")
-        txt = txt.replace("%version%", str(pygubudesigner.__version__))
-        entry.configure(text=txt)
-
-        def on_ok_execute():
-            dialog.close()
-
-        def on_gpl3_clicked(e):
-            url = "https://www.gnu.org/licenses/gpl-3.0.html"
-            webbrowser.open_new_tab(url)
-
-        def on_mit_clicked(e):
-            url = "https://opensource.org/licenses/MIT"
-            webbrowser.open_new_tab(url)
-
-        def on_moreinfo_clicked(e):
-            url = "https://github.com/alejandroautalan/pygubu-designer"
-            webbrowser.open_new_tab(url)
-
-        dialog_callbacks = {
-            "on_ok_execute": on_ok_execute,
-            "on_gpl3_clicked": on_gpl3_clicked,
-            "on_mit_clicked": on_mit_clicked,
-            "on_moreinfo_clicked": on_moreinfo_clicked,
-        }
-        builder.connect_callbacks(dialog_callbacks)
-
-        return dialog
-
     def show_about_dialog(self):
         if self.about_dialog is None:
-            self.about_dialog = self._create_about_dialog()
-            self.about_dialog.run()
-        else:
-            self.about_dialog.show()
+            self.about_dialog = AboutDialog(self.mainwindow, translator)
+        self.about_dialog.run()
 
     def _edit_preferences(self):
         if self.preferences is None:
-            self.preferences = pref.PreferencesUI(self.mainwindow, translator)
-        self.preferences.dialog.run()
+            # self.preferences = pref.PreferencesUI(self.mainwindow, translator)
+            self.preferences = DesignerSettings(self.mainwindow, translator)
+        self.preferences.run()
+
+    def _require_project_open(self):
+        if self.current_project is None:
+            msg = _("Open a project first.")
+            messagebox.showinfo(self.mbox_title, msg, parent=self.mainwindow)
+        return self.current_project is not None
+
+    def _edit_project_settings(self):
+        if not self._require_project_open():
+            return
+        options = self.tree_editor.get_options_for_project_settings()
+        self.project_settings.setup(options)
+        self.project_settings.edit(self.current_project)
+        self.project_settings.run()
+
+    def _on_project_settings_changed(self, new_settings: dict):
+        self.current_project.set_full_settings(new_settings)
+        self.set_changed()
+        self.reload_component_palette()
+
+    def _project_code_generate(self):
+        if not self._require_project_open():
+            return
+        options = self.tree_editor.get_options_for_project_settings()
+        self.project_settings.setup(options)
+        self.project_settings.edit(self.current_project)
+        valid = self.project_settings.validate_for_codegen()
+        if valid:
+            self.script_generator.generate_code()
+            msg = _("Project code generated.")
+            logger.info(msg)
+        else:
+            self.project_settings.run()
+
+    def generate_code_on_save(self):
+        return (
+            False
+            if self.current_project is None
+            else self.current_project.generate_code_onsave
+        )
 
     def project_name(self):
         name = None
-        if self.currentfile is None:
+        if self.current_project is None:
             name = _("newproject")
         else:
-            name = Path(self.currentfile).name
+            name = self.current_project.fpath.name
         return name
 
-    def nbmain_tab_changed(self, event):
-        if event.widget.index("current") == 1:  # Index 1 is the code-tab
-            self.script_generator.configure()
-            if pref.get_option("auto_generate_code") == "yes":
-                self.on_code_generate_clicked()
-
-    # Tab code management
-    def on_code_generate_clicked(self):
-        self.script_generator.on_code_generate_clicked()
-
-    def on_code_copy_clicked(self):
-        self.script_generator.on_code_copy_clicked()
-
-    def on_code_template_changed(self):
-        self.script_generator.on_code_template_changed()
-        if pref.get_option("auto_generate_code") == "yes":
-            self.on_code_generate_clicked()
-
-    def on_code_template_property_changed(self):
-        if (
-            pref.get_option("auto_generate_code") == "yes"
-            and pref.get_option("auto_generate_code_on_prop_change") == "yes"
-        ):
-            self.on_code_generate_clicked()
-        return True
-
-    def on_code_save_clicked(self):
-        self.script_generator.on_code_save_clicked()
-
     def setup_bottom_panel(self):
         self.log_panel = LogPanelManager(self)
         self.setup_logger_handler()
 
     def on_bpanel_button_clicked(self):
         self.log_panel.on_bpanel_button_clicked()
 
@@ -933,14 +896,52 @@
         # handler.setLevel(logging.INFO)
         # add handler to the root logger:
         logging.getLogger().addHandler(handler)
 
     def log_message(self, msg, level):
         self.log_panel.log_message(msg, level)
 
+    def reload_component_palette(self):
+        """Reload palette with project custom widgets."""
+        project = self.current_project
+        prefixes = [Path(cw).stem for cw in project.custom_widgets]
+        current_prefixes = self.tree_palette.project_custom_widget_prefixes
+
+        prefixes.sort()
+        current_prefixes.sort()
+        if prefixes != current_prefixes:
+            try:
+                project.load_custom_widgets()
+                self.tree_palette.project_custom_widget_prefixes = prefixes
+                self.tree_palette.build_tree()
+            except Exception as e:
+                msg = str(e)
+                det = traceback.format_exc()
+                show_error(
+                    self.mainwindow,
+                    _("Error"),
+                    msg,
+                    det,
+                )
+
+    def on_dockframe_changed(self, event=None):
+        """Save current layout of maindock widget."""
+        dock = self.builder.get_object("maindock")
+        dock_layout = dock.save_layout()
+        pref.save_maindock_layout(dock_layout)
+
+    def load_dockframe_layout(self):
+        """Load layout for maindock widget."""
+        layout = pref.get_maindock_layout()
+        try:
+            dock = self.builder.get_object("maindock")
+            dock.load_layout(layout)
+        except Exception:
+            logger.debug("Error loading maindock layout")
+
 
 def start_pygubu():
     print(f"python: {platform.python_version()} on {sys.platform}")
     print(f"tk: {tk.TkVersion}")
     print(f"pygubu: {pygubu.__version__}")
     print(f"pygubu-designer: {pygubudesigner.__version__}")
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/preview/builder.py` & `pygubu_designer-0.39/src/pygubudesigner/preview/builder.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/preview/helper.py` & `pygubu_designer-0.39/src/pygubudesigner/preview/helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from collections import OrderedDict
 from functools import partial
 
 from pygubu.stockimage import StockImage
 
 import pygubudesigner.actions as actions
 from pygubudesigner.widgets.ttkstyleentry import TtkStylePropertyEditor
-
+from pygubudesigner.services.theming import ThemeChangedMonitor
+from ..preferences import get_preview_indicator_color
 from .preview import MenuPreview, Preview
 
 logger = logging.getLogger(__name__)
 
 
 class PreviewHelper:
     indicators_tag = ("top", "bottom", "left", "right")
@@ -67,14 +68,22 @@
         self.style.configure("PreviewFrame.TFrame", background="lightgreen")
 
         self.selected_widget = None
         canvas.bind_all(
             actions.PREVIEW_TOPLEVEL_CLOSE_ALL,
             lambda e: self.close_toplevel_previews(),
         )
+        # monitor theme change to maintain selector color
+        self.tcmonitor = ThemeChangedMonitor(
+            canvas, self.update_indicators_color
+        )
+
+    def update_indicators_color(self):
+        for key, frame in self.indicators.items():
+            frame.configure(background=get_preview_indicator_color())
 
     def add_resource_path(self, path):
         self.resource_paths.append(path)
 
     def motion_handler(self, event):
         if not self._moving:
             c = event.widget
@@ -200,20 +209,21 @@
             self.bind_preview_widget(widget, callback)
 
     def _create_indicators(self):
         # selected indicators
         anchors = {"top": tk.SW, "bottom": tk.NW, "left": tk.NE, "right": tk.NW}
         self.indicators = {}
         for tag in anchors:
-            frame = ttk.Frame(
+            frame = tk.Frame(
                 self.canvas,
-                style="PreviewIndicator.TFrame",
+                class_="PreviewIndicatorFrame",
                 width=1,
                 height=1,
                 borderwidth=0,
+                background=get_preview_indicator_color(),
             )
             self.canvas.create_window(
                 -10, -10, window=frame, anchor=anchors[tag], tags=tag
             )
             self.indicators[tag] = frame
 
     def _update_indicator_coords(self, tag, widget):
@@ -278,14 +288,28 @@
             widget = preview.get_widget_by_id(selected_id)
             for tag in self.indicators:
                 self._update_indicator_coords(tag, widget)
             self._update_style_editor(widget)
         self._sel_id = identifier
         self._sel_widget = selected_id
 
+    def preview_for_widget(self, preview_id, widget_id):
+        """Returns the live widget preview of widget_id."""
+        if preview_id in self.previews:
+            preview = self.previews[preview_id]
+            widget = preview.get_widget_by_id(widget_id)
+            return widget
+        return None
+
+    def update_preview_bbox(self, preview_id):
+        """Updates the preview to the requested size of
+        the widget inside."""
+        if preview_id in self.previews:
+            self.previews[preview_id].update_window_bbox()
+
     def delete(self, identifier):
         if identifier in self.previews:
             preview = self.previews[identifier]
             preview.erase()
             del self.previews[identifier]
             self.reset_selected(identifier)
             self.move_previews()
@@ -307,15 +331,19 @@
 
         # Check if we should center the preview window
         if self.center_window_check():
             Preview.center_window_active_monitor(top)
 
     def close_toplevel_previews(self):
         for top in self.toplevel_previews:
-            top.destroy()
+            try:
+                top.destroy()
+            except tk.TclError:
+                # the user closed the window.
+                pass
         self.toplevel_previews = []
 
     def preview_click_handler(self, preview_id, event=None):
         preview = self.previews[preview_id]
         wid = preview.builder.get_widget_id(event.widget)
         if wid is not None:
             self.selected_widget = wid
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/preview/preview.py` & `pygubu_designer-0.39/src/pygubudesigner/preview/preview.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,27 @@
             self.draw()
             self._resize_preview_window()
 
     def _resize_preview_window(self):
         if self.canvas_window:
             self.canvas_window.configure(width=self.w, height=self.h)
 
+    def update_window_bbox(self):
+        """Update the canvas window to the requested
+        size of the widget."""
+        if self.canvas_window:
+            # do one update before recalculation
+            self.canvas.update_idletasks()
+            self.min_w = self._get_wreqwidth()
+            self.min_h = self._get_wreqheight()
+            self.w = self.min_w * 2
+            self.h = self.min_h * 2
+            # print("request new size to", self.min_w, self.min_h)
+            self.resize_to(self.min_w, self.min_h)
+
     def update(self, widget_id, uidefinition):
         # delete current preview
         # FIXME maybe do something to update preview without re-creating all ?
         del self.builder
         self.builder = None
         self.canvas.itemconfigure(self.shapes["window"], window="")
         if self.canvas_window:
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/properties/manager.py` & `pygubu_designer-0.39/src/pygubudesigner/properties/manager.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/properties/predefined.py` & `pygubu_designer-0.39/src/pygubudesigner/properties/predefined.py`

 * *Files 0% similar despite different names*

```diff
@@ -1223,14 +1223,15 @@
             }
         },
     },
     "style": {
         "editor": "dynamic",
         "params": {"mode": "ttkstylechoice"},
         "ttk.Button": {"params": {"values": ("", "Toolbutton")}},
+        "ttk.Checkbutton": {"params": {"values": ("", "Toolbutton")}},
         "help": help_for("style"),
     },
     "tabs": {  # FIXME see tk.Text tab property
         "editor": "dynamic",
         "params": {"mode": "entry"},
         "help": help_for("tabs"),
     },
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/properties/propertieshelp.py` & `pygubu_designer-0.39/src/pygubudesigner/properties/propertieshelp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/propertieseditor.py` & `pygubu_designer-0.39/src/pygubudesigner/propertieseditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from pygubu import builder
 from pygubu.widgets.simpletooltip import create as create_tooltip
 
 from pygubudesigner.i18n import translator as _
 from pygubudesigner.widgets.propertyeditor import create_editor
 from .widgets import NamedIDPropertyEditor
-from .stylehandler import StyleHandler
+from .services.stylehandler import StyleHandler
 from pygubudesigner.properties.manager import PropertiesManager
 
 logger = logging.getLogger(__name__)
 CLASS_MAP = builder.CLASS_MAP
 
 
 class PropertiesEditor:
@@ -102,14 +102,15 @@
 
         # Setup name placeholder
         params = pdescr["params"]
         if pname == "id" and params["mode"] == "namedid":
             params["placeholder"] = wdescr.start_id
 
         # Configure editor
+        logger.debug("Setting editor mode for %s", pname)
         editor.parameters(**params)
 
         # Setup tooltip
         help = pdescr.get("help", None)
         if isinstance(help, dict):
             found_match = False
             for k, v in help.items():
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/rfilemanager.py` & `pygubu_designer-0.39/src/pygubudesigner/rfilemanager.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/stylehandler.py` & `pygubu_designer-0.39/src/pygubudesigner/services/stylehandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 import sys
 import importlib
 import logging
 from pathlib import Path
 from tkinter import ttk
 
-from pygubudesigner import preferences as pref
 from pygubudesigner.widgets.ttkstyleentry import TtkStylePropertyEditor
-
-from .i18n import translator as _
+from ..i18n import translator as _
 
 logger = logging.getLogger(__name__)
 
 
 # StyleRegister
 # This class y used to capture the styles defined by the user.
 #
@@ -46,14 +44,15 @@
 
     def configure(self, style, query_opt=None, **kw):
         self._add_style(style)
         super().configure(style, query_opt, **kw)
 
 
 class StyleHandler:
+    current_definition_file = None
     last_definition_file = None
     last_modified_time = None
     required_function_name = "setup_ttk_styles"
 
     def __init__(self, mframe, reselect_item_func):
         self.mframe = mframe
         self.after_token = None
@@ -86,67 +85,79 @@
                 )
                 module = importlib.util.module_from_spec(spec)
 
                 sys.modules[module_name] = module
                 spec.loader.exec_module(module)
 
                 if hasattr(module, self.required_function_name):
-                    module.setup_ttk_styles()
+                    master = self.mframe.winfo_toplevel()
+                    module.setup_ttk_styles(master)
                 else:
                     msg = "Styles definition file does not have the required function: %s"
                     logger.info(msg, self.required_function_name)
 
                 new_styles = self.style.registered_styles()
                 TtkStylePropertyEditor.set_global_style_list(new_styles)
         except Exception as e:
             msg = _("ttk style definition error: %s")
             logger.error(msg, e)
 
     @classmethod
     def get_ttk_styles_module(cls):
         module = None
-        style_definition_path = Path(pref.get_option("v_style_definition_file"))
-
-        if style_definition_path.is_file():
-            module = style_definition_path.stem
+        if cls.current_definition_file is not None:
+            if cls.current_definition_file.is_file():
+                module = cls.current_definition_file.stem
         return module
 
+    @classmethod
+    def set_definition_file(cls, filepath):
+        if not isinstance(filepath, Path):
+            raise ValueError()
+        cls.current_definition_file = filepath
+        logger.debug("New definitions file %s", str(filepath))
+
+    @classmethod
+    def clear_definition_file(cls):
+        StyleRegister.STYLE_DEFINITIONS.clear()
+        TtkStylePropertyEditor.set_global_style_list([])
+        cls.current_definition_file = None
+
     def check_definition_file(self, force_reload=False):
-        # print('checking definitions')
         # Get the path to the style definition file.
-        style_definition_path = Path(pref.get_option("v_style_definition_file"))
-
-        do_reload = False
-        has_definition_file = False
-        is_new_file = False
-        if style_definition_path.is_file():
-            has_definition_file = True
-            file_mtime = style_definition_path.stat().st_mtime
-            if StyleHandler.last_definition_file != style_definition_path:
-                do_reload = True
-                is_new_file = True
-                StyleHandler.last_definition_file = style_definition_path
-                StyleHandler.last_modified_time = file_mtime
-            if not is_new_file:
-                if file_mtime > StyleHandler.last_modified_time:
+        style_definition_path = self.current_definition_file
+        if style_definition_path is not None:
+            do_reload = False
+            has_definition_file = False
+            is_new_file = False
+            if style_definition_path.is_file():
+                has_definition_file = True
+                file_mtime = style_definition_path.stat().st_mtime
+                if StyleHandler.last_definition_file != style_definition_path:
                     do_reload = True
+                    is_new_file = True
+                    StyleHandler.last_definition_file = style_definition_path
                     StyleHandler.last_modified_time = file_mtime
-        if do_reload or (has_definition_file and force_reload):
-            # Clear and reload all the definitions.
-
-            # Reason: so that definitions that are no longer in the definition file
-            # will no longer populate in the style combobox.
-            StyleRegister.STYLE_DEFINITIONS.clear()
-
-            self._run_styles_module(style_definition_path)
-
-            # Re-select the selected item so the style combobox
-            # will show the latest styles from the definition file.
-            if self.reselect_item_func is not None:
-                self.reselect_item_func()
+                if not is_new_file:
+                    if file_mtime > StyleHandler.last_modified_time:
+                        do_reload = True
+                        StyleHandler.last_modified_time = file_mtime
+            if do_reload or (has_definition_file and force_reload):
+                # Clear and reload all the definitions.
+
+                # Reason: so that definitions that are no longer in the definition file
+                # will no longer populate in the style combobox.
+                StyleRegister.STYLE_DEFINITIONS.clear()
+
+                self._run_styles_module(style_definition_path)
+
+                # Re-select the selected item so the style combobox
+                # will show the latest styles from the definition file.
+                if self.reselect_item_func is not None:
+                    self.reselect_item_func()
 
         # schedule new check
         self.after_token = self.mframe.after(1000, self.check_definition_file)
 
 
 # Patch ttk module, so designer can "see" style changes.
 if not hasattr(ttk, "_style_original"):
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/uitreeeditor.py` & `pygubu_designer-0.39/src/pygubudesigner/uitreeeditor.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 import json
 import logging
 import os
 import tkinter as tk
 import xml.etree.ElementTree as ET
-from collections import Counter
+from collections import Counter, OrderedDict
 from functools import partial
 from tkinter import messagebox
 
 from pygubu.builder import CLASS_MAP
 from pygubu.component.uidefinition import UIDefinition
 from pygubu.stockimage import StockImage, StockImageException
 
@@ -38,14 +38,22 @@
 import pygubudesigner.actions as action
 from .bindingseditor import BindingsEditor
 from .i18n import translator as _
 from .layouteditor import LayoutEditor
 from .propertieseditor import PropertiesEditor
 from .util import trlog
 from .widgetdescr import WidgetMeta
+from pygubu.forms.widget import FieldWidget
+from pygubudesigner.properties.editors.forms import (
+    FormFieldNameEntry,
+    FormFieldNameSelector,
+)
+from pygubudesigner.services.project import Project
+from pygubu.component.plugin_manager import PluginManager
+
 
 logger = logging.getLogger("pygubu.designer")
 
 
 class WidgetsTreeEditor:
     GRID_UP = 0
     GRID_DOWN = 1
@@ -57,14 +65,19 @@
         self.treeview = app.treeview
         self.previewer = app.previewer
         self.treedata = {}
         self.counter = Counter()
         self.virtual_clipboard_for_duplicate = None
         self.duplicating = False
         self.duplicate_parent_iid = None
+        self.update_builders = {}
+        self.preview_update_cbid = None
+        self.scheduled_widget_updates = []
+        self._stretch_cb = None
+        self.treeview.bind("<Configure>", self._on_tree_configure)
 
         self.treeview.filter_func = self.filter_match
 
         # Get the default layout manager based on the user's configuration.
         self.__preferred_layout_manager_var = tk.StringVar()
         current_default_layout = pref.get_option("default_layout_manager")
         if not current_default_layout:
@@ -98,14 +111,16 @@
         # set global validator for IDs
         IdentifierPropertyEditor.global_validator = self.is_id_unique
         NamedIDPropertyEditor.global_validator = self.is_id_unique
         # set global validator for commands
         CommandPropertyBase.global_validator = self.is_command_valid
         # set global validator for bindings commands
         EventHandlerEditor.global_validator = self.is_binding_valid
+        # set global validator for form field name entry
+        FormFieldNameEntry.global_validator = self.is_form_fieldname_valid
 
         # Widget Editor
         pframe = app.builder.get_object("propertiesframe")
         lframe = app.builder.get_object("layoutframe")
         bframe = app.builder.get_object("bindingsframe")
         bindingstree = app.builder.get_object("bindingstree")
         self.properties_editor = PropertiesEditor(
@@ -164,14 +179,37 @@
         tree.bind_all(action.TREE_ITEM_MOVE_DOWN, self.on_item_move_down)
         tree.bind_all(action.TREE_NAV_UP, self.on_item_nav_up)
         tree.bind_all(action.TREE_NAV_DOWN, self.on_item_nav_down)
         tree.bind_all(
             action.TREE_ITEM_PREVIEW_TOPLEVEL, self.on_preview_in_toplevel
         )
 
+    def _on_tree_configure(self, event):
+        if self._stretch_cb is not None:
+            self.treeview.after_cancel(self._stretch_cb)
+        self._stretch_cb = self.treeview.after(350, self._stretch_main_column)
+
+    def _stretch_main_column(self):
+        w = self.treeview.winfo_width()
+        stretch_col = "#0"
+        stretch_col_cwidth = 0
+        cols = [stretch_col]
+        cols.extend(self.treeview.cget("displaycolumns"))
+        csum = 0
+        for col in cols:
+            cwidth = self.treeview.column(col, "width")
+            if col == stretch_col:
+                stretch_col_cwidth = cwidth
+            csum += cwidth
+        space_left = w - csum - 4
+        if space_left > 0:
+            stretch_col_cwidth += space_left
+            self.treeview.column(stretch_col, width=stretch_col_cwidth)
+        self._stretch_cb = None
+
     def filter_match(self, tree, itemid, filter_value):
         txt = tree.item(itemid, "text").lower()
         match_found = filter_value in txt
         if not match_found:
             class_txt = self.treedata[itemid].classname.lower()
             match_found = filter_value in class_txt
         return match_found
@@ -398,21 +436,28 @@
             if "pack" == cm:
                 manager_options.remove("grid")
         logger.debug(manager_options)
 
         # Prepare container layout options
         cinfo = self.get_container_info(item)
         cmanager = cinfo["manager"]
-        if cmanager is not None and cmanager != wdescr.container_manager:
+        if cmanager is None:
+            # Allow simple propagate option.
+            wdescr.container_manager = "pack"
+        elif cmanager != wdescr.container_manager:
             # Update widged description
             wdescr.container_manager = cmanager
 
+        # Prepare field name values
+        FormFieldNameSelector.FIELD_NAMES = self.get_form_fieldname_list()
+
         self.properties_editor.edit(wdescr)
         self.layout_editor.edit(wdescr, manager_options, cinfo)
         self.bindings_editor.edit(wdescr)
+        self.get_form_fieldname_list()
 
     def editor_hide_all(self):
         self.properties_editor.hide_all()
         self.layout_editor.hide_all()
         self.bindings_editor.hide_all()
 
     def config_filter(self):
@@ -560,16 +605,15 @@
         for child in item_children:
             self.delete_item_data(child)
 
         del self.treedata[item]
 
     def new_uidefinition(self):
         author = f"PygubuDesigner {pygubudesigner.__version__}"
-        uidef = UIDefinition(wmetaclass=WidgetMeta)
-        uidef.author = author
+        uidef = UIDefinition(wmetaclass=WidgetMeta, author=author)
         return uidef
 
     def tree_to_uidef(self, treeitem=None):
         """Traverses treeview and generates a ElementTree object"""
 
         # Need to remove filter or hidden items will not be saved.
         self.treeview.filter_remove(remember=True)
@@ -700,52 +744,56 @@
 
         new_boclass = CLASS_MAP[classname].builder
         root = root_item
         if root:
             root_classname = self.treedata[root].classname
             root_boclass = CLASS_MAP[root_classname].builder
             allowed_children = root_boclass.allowed_children
-            if allowed_children:
-                if classname not in allowed_children:
-                    if show_warnings:
-                        str_children = ", ".join(allowed_children)
-                        msg = _("Allowed children: %s.")
-                        logger.warning(msg, str_children)
-                    is_valid = False
-                    return is_valid
+            allowed_children = (
+                [] if allowed_children is None else allowed_children
+            )
+            canbe_parent = root_boclass.canbe_parent_of(new_boclass, classname)
+            if not canbe_parent:
+                if show_warnings:
+                    str_children = ", ".join(allowed_children)
+                    msg = _("Allowed children: %s.")
+                    logger.warning(msg, str_children)
+                is_valid = False
+                return is_valid
 
             children_count = len(self.treeview.get_children(root))
             maxchildren = root_boclass.maxchildren
             if maxchildren is not None and children_count >= maxchildren:
                 if show_warnings:
                     msg = trlog(
                         _("Only {0} children allowed for {1}"),
                         maxchildren,
                         root_classname,
                     )
                     logger.warning(msg)
                 is_valid = False
                 return is_valid
 
-            allowed_parents = new_boclass.allowed_parents
-            if (
-                allowed_parents is not None
-                and root_classname not in allowed_parents
-            ):
+            # allowed_parents = new_boclass.allowed_parents
+            # if (
+            #    allowed_parents is not None
+            #    and root_classname not in allowed_parents
+            # ):
+            if not new_boclass.canbe_child_of(root_boclass, root_classname):
                 if show_warnings:
                     msg = trlog(
                         _("{0} not allowed as parent of {1}"),
                         root_classname,
                         classname,
                     )
                     logger.warning(msg)
                 is_valid = False
                 return is_valid
 
-            if allowed_children is None and root_boclass.container is False:
+            if not canbe_parent and root_boclass.container is False:
                 if show_warnings:
                     msg = _("Not allowed, %s is not a container.")
                     logger.warning(msg, root_classname)
                 is_valid = False
                 return is_valid
 
         else:
@@ -949,27 +997,25 @@
             self.treeview.delete(*children)
         self.editor_hide_all()
         self.counter.clear()  # Reset the widget counter (August 19, 2021)
         self.current_edit = (
             None  # We no longer have a selected item in the treeview
         )
 
-    def load_file(self, filename):
+    def load_file(self, project: Project):
         """Load file into treeview"""
 
         self.counter.clear()
-        uidef = UIDefinition(wmetaclass=WidgetMeta)
-        uidef.load_file(filename)
-
         self.remove_all()
         self.previewer.remove_all()
         self.editor_hide_all()
 
-        dirname = os.path.dirname(os.path.abspath(filename))
+        dirname = project.fpath.parent
         self.previewer.resource_paths.append(dirname)
+        uidef = project.uidefinition
         for widget in uidef.widgets():
             self.populate_tree("", uidef, widget, from_file=True)
 
         children = self.treeview.get_children("")
         for child in children:
             self.draw_widget(child)
         self.previewer.show_selected(None, None)
@@ -1103,39 +1149,112 @@
             self.editor_hide_all()
 
         # Check if some menu items (such as 'Duplicate') should be disabled or not.
         # The reason is: the treeview selection has changed, so we need to evaluate
         # whether it makes sense to have some menus enabled or not.
         self.app.evaluate_menu_states()
 
-    def update_event(self, hint, obj):
+    def update_tree_data_display(self, item, data):
         """Updates tree colums when itemdata is changed."""
+        tree = self.treeview
+        item_text = self._treeitem_label(data)
+        if item_text != tree.item(item, "text"):
+            tree.item(item, text=item_text)
+        # if tree.parent(item) != '' and 'layout' in data:
+        if tree.parent(item) != "" and data.layout_required:
+            if data.manager == "grid":
+                row = data.layout_property("row")
+                col = data.layout_property("column")
+                values = tree.item(item, "values")
+                if row != values[1] or col != values[2]:
+                    values = (data.classname, row, col)
+                tree.item(item, values=values)
+
+    def preview_widget_update(self, item, hint, data):
+        """Update widget preview.
+        If posible, it will update widget properties live.
+        Otherwise, a full widget redraw is done.
+        """
+
+        full_redraw = (
+            (hint & WidgetMeta.PROPERTY_RO_CHANGED)
+            | (hint & WidgetMeta.LAYOUT_MANAGER_CHANGED)
+            | (hint & WidgetMeta.PROPERTY_BLANKED)
+        )
+
+        # FIXME: A full redraw is done when a property is blanked.
+        #        Maybe this can be improved in the future?
+
+        if full_redraw:
+            # Needs full redraw.
+            self.draw_widget(item)
+        else:
+            # Maybe just needs update.
+            preview_id = self.get_toplevel_parent(item)
+
+            widget_id = data.identifier
+            bclass = data.classname
+            widget = self.previewer.preview_for_widget(preview_id, widget_id)
+            if bclass not in self.update_builders:
+                builder = PluginManager.get_preview_builder_for(bclass)
+                builder = (
+                    CLASS_MAP[bclass].builder if builder is None else builder
+                )
+                self.update_builders[bclass] = builder(None, data)
+            builder = self.update_builders[bclass]
+            # Use copy here because preview builders can change data for preview
+            meta_copy = WidgetMeta(bclass, widget_id)
+            meta_copy.copy_properties(data)
+            builder.wmeta = meta_copy
+            builder.widget = widget
+
+            if hint & WidgetMeta.PROPERTY_CHANGED:
+                builder.configure()
+            if hint & WidgetMeta.LAYOUT_PROPERTY_CHANGED:
+                builder.layout()
+                # FIXME: When propagate property is changed
+                # calculations are not correct unless a property
+                # is reconfigured ?
+                builder.configure()
+            if hint & WidgetMeta.BINDING_CHANGED:
+                # Do nothing now
+                pass
+            self.previewer.update_preview_bbox(preview_id)
+            self.previewer.show_selected(preview_id, widget_id)
+
+    def update_event(self, hint, data):
+        """Manages notify event when data is changed."""
 
         if not self._listen_object_updates:
             return
 
-        tree = self.treeview
-        data = obj
-        item = self.get_item_by_data(obj)
-        item_text = self._treeitem_label(data)
+        item = self.get_item_by_data(data)
         if item:
-            if item_text != tree.item(item, "text"):
-                tree.item(item, text=item_text)
-            # if tree.parent(item) != '' and 'layout' in data:
-            if tree.parent(item) != "" and data.layout_required:
-                if data.manager == "grid":
-                    row = data.layout_property("row")
-                    col = data.layout_property("column")
-                    values = tree.item(item, "values")
-                    if row != values[1] or col != values[2]:
-                        values = (data.classname, row, col)
-                    tree.item(item, values=values)
-            self.draw_widget(item)
+            self.update_tree_data_display(item, data)
+            self.preview_widget_update(item, hint, data)
             self.app.set_changed()
 
+    def schedule_preview_update(self, item):
+        """Schedule a preview update.
+        Helps to reduce full redraw when moving widget in treeview with keyboard.
+        """
+        if item not in self.scheduled_widget_updates:
+            self.scheduled_widget_updates.append(item)
+        if self.preview_update_cbid is not None:
+            self.treeview.after_cancel(self.preview_update_cbid)
+        self.preview_update_cbid = self.treeview.after(
+            950, self.schedule_preview_update_execute
+        )
+
+    def schedule_preview_update_execute(self):
+        for item in self.scheduled_widget_updates:
+            self.draw_widget(item)
+        self.scheduled_widget_updates.clear()
+        self.preview_update_cbid = None
+
     def get_item_by_data(self, data):
         skey = None
         for key, value in self.treedata.items():
             if value == data:
                 skey = key
                 break
         return skey
@@ -1193,15 +1312,16 @@
                 manager = item_data.manager
                 layout_required = item_data.layout_required
                 self.app.set_changed()
 
                 # Always refresh preview for objects that don't
                 # require a layout, such as menus and notebook tabs.
                 if manager in ("pack", "place") or not layout_required:
-                    self.draw_widget(item)
+                    # self.draw_widget(item)
+                    self.schedule_preview_update(item)
             self.treeview.filter_restore()
 
     def on_item_move_down(self, event):
         tree = self.treeview
         sel = tree.selection()
         if sel:
             self.treeview.filter_remove(remember=True)
@@ -1215,15 +1335,16 @@
                 manager = item_data.manager
                 layout_required = item_data.layout_required
                 self.app.set_changed()
 
                 # Always refresh preview for objects that don't
                 # require a layout, such as menus and notebook tabs.
                 if manager in ("pack", "place") or not layout_required:
-                    self.draw_widget(item)
+                    # self.draw_widget(item)
+                    self.schedule_preview_update(item)
             self.treeview.filter_restore()
 
     #
     # Item grid move functions
     #
     def on_item_grid_move(self, direction):
         tree = self.treeview
@@ -1247,26 +1368,41 @@
                     if current_col > 0:
                         new_col = current_col - 1
                 elif direction == self.GRID_RIGHT:
                     new_col = current_col + 1
 
                 if current_row != new_row:
                     data.layout_property("row", str(new_row))
-                    data.notify()
+                    data.notify(WidgetMeta.LAYOUT_PROPERTY_CHANGED)
                 if current_col != new_col:
                     data.layout_property("column", str(new_col))
-                    data.notify()
+                    data.notify(WidgetMeta.LAYOUT_PROPERTY_CHANGED)
             self.treeview.filter_restore()
 
     def _top_widget_iterator(self):
         children = self.treeview.get_children("")
         for item in children:
             data = self.treedata[item]
             yield (item, data)
 
+    def _data_iterator(self, root=None):
+        start = "" if root is None else root
+        children = self.treeview.get_children(start)
+        for item in children:
+            data = self.treedata[item]
+            yield (item, data)
+        for item in children:
+            yield from self._data_iterator(item)
+
+    def get_tree_topitem_byid(self, wid):
+        for item, data in self._top_widget_iterator():
+            if data.identifier == wid:
+                return item
+        return None
+
     def get_top_widget_list(self):
         wlist = []
         for item, data in self._top_widget_iterator():
             if data.classname != "tk.Menu":
                 label = f"{data.identifier} ({data.classname})"
                 element = (item, label)
                 wlist.append(element)
@@ -1277,14 +1413,25 @@
         for item, data in self._top_widget_iterator():
             if data.classname == "tk.Menu":
                 label = f"{data.identifier} ({data.classname})"
                 element = (item, label)
                 wlist.append(element)
         return wlist
 
+    def get_options_for_project_settings(self):
+        main_widget = OrderedDict()
+        main_menu = OrderedDict()
+        for item, data in self._top_widget_iterator():
+            label = f"{data.identifier} ({data.classname})"
+            if data.classname == "tk.Menu":
+                main_menu[data.identifier] = label
+            else:
+                main_widget[data.identifier] = label
+        return dict(main_widget=main_widget, main_menu=main_menu)
+
     def get_widget_class(self, item):
         return self.treedata[item].classname
 
     def get_widget_id(self, item):
         return self.treedata[item].identifier
 
     def select_by_id(self, widget_id):
@@ -1417,7 +1564,38 @@
         wmeta.identifier = newid
         wmeta.is_named = False
 
         self._listen_object_updates = True
         self.editor_edit(item, wmeta)
         self.draw_widget(item)
         self.app.set_changed()
+
+    def _is_form_field_class(self, classname: str):
+        builder = CLASS_MAP[classname].builder
+        if builder.class_ is not None:
+            return issubclass(builder.class_, FieldWidget)
+        return False
+
+    def _is_form_filedname_defined(self, fieldname: str):
+        is_defined = False
+        for item, data in self._data_iterator():
+            if self._is_form_field_class(data.classname):
+                fname = data.widget_property("field_name")
+                if not fname:
+                    fname = data.identifier
+                if fname == fieldname:
+                    is_defined = True
+                    break
+        return is_defined
+
+    def get_form_fieldname_list(self):
+        flist = []
+        for item, data in self._data_iterator():
+            if self._is_form_field_class(data.classname):
+                fname = data.widget_property("field_name")
+                if not fname:
+                    fname = data.identifier
+                flist.append(fname)
+        return flist
+
+    def is_form_fieldname_valid(self, fieldname: str):
+        return not self._is_form_filedname_defined(fieldname)
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/util/__init__.py` & `pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpalette.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,214 +1,178 @@
-#
-# Copyright 2012-2022 Alejandro Autalán
-#
-# This program is free software: you can redistribute it and/or modify it
-# under the terms of the GNU General Public License version 3, as published
-# by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranties of
-# MERCHANTABILITY, SATISFACTORY QUALITY, or FITNESS FOR A PARTICULAR
-# PURPOSE.  See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-import sys
 import tkinter as tk
 import tkinter.ttk as ttk
-
-
-# in-place prettyprint formatter
-def indent(elem, level=0):
-    i = "\n" + level * "  "
-    if len(elem):
-        if not elem.text or not elem.text.strip():
-            elem.text = i + "  "
-        if not elem.tail or not elem.tail.strip():
-            elem.tail = i
-        for elem in elem:
-            indent(elem, level + 1)
-        if not elem.tail or not elem.tail.strip():
-            elem.tail = i
-    else:
-        if level and (not elem.tail or not elem.tail.strip()):
-            elem.tail = i
-
-
-def treeview_print(tree, root=""):
-    def tree_print(tree, root):
-        children = tree.get_children(root)
-        if root != "" and children:
-            print(root)
-        for item in children:
-            tree_print(tree, item)
-
-    tree_print(tree, root)
-
-
-class BraceMessage:
-    """Helper class to use braces {} in log messages"""
-
-    def __init__(self, fmt, *args, **kwargs):
-        self.fmt = fmt
-        self.args = args
-        self.kwargs = kwargs
-
-    def __str__(self):
-        return self.fmt.format(*self.args, **self.kwargs)
-
-
-# Helper to translate log messages with braces
-trlog = BraceMessage
-
-
-def virtual_event(event_name):
-    """Generate virtual event event_name"""
-
-    def virtual_event_gen(event):
-        event.widget.event_generate(event_name)
-
-    return virtual_event_gen
-
-
-def menu_iter_children(menu):
-    """Iterates all menu items (including submenus).
-    Returns (menu, itemtype, index)"""
-    count = menu.index(tk.END)
-    if count is not None:
-        cascades = []
-        for i in range(0, count + 1):
-            itemtype = menu.type(i)
-            if itemtype == "cascade":
-                cascade = menu.nametowidget(menu.entrycget(i, "menu"))
-                cascades.append(cascade)
-            yield (menu, itemtype, i)
-        for m in cascades:
-            yield from menu_iter_children(m)
-
-
-__style = None
-
-has_sv_ttk = False
-has_ttkthemes = False
-has_ttkbootsrap = False
-
-
-class ThemeModule:
-    def theme_names(self) -> list:
-        raise NotImplementedError
-
-    def theme_use(self, name):
-        raise NotImplementedError
-
-    def can_handle(self, name) -> bool:
-        return False
-
-
-class SunValleyModule(ThemeModule):
-    sv_themes = {"sun-valley-dark": "dark", "sun-valley-light": "light"}
-
-    def __init__(self):
-        sv_ttk.get_theme()
-
-    def theme_names(self) -> list:
-        return []
-
-    def theme_use(self, name):
-        sv_ttk.set_theme(self.sv_themes[name])
-
-    def can_handle(self, name) -> bool:
-        return name in self.sv_themes
-
-
-class ttkthemesModule(ThemeModule):
-    def __init__(self):
-        self.style = ThemedStyle()
-        self.definitions = list(self.style.theme_names())
-
-    def theme_names(self) -> list:
-        return self.definitions
-
-    def theme_use(self, name):
-        self.style.theme_use(name)
-
-    def can_handle(self, name):
-        return name in self.definitions
-
-
-class ttkbModule(ThemeModule):
-    def __init__(self):
-        self.style = ttkb.Style()
-        self.definitions = list(self.style.theme_names())
-
-    def theme_names(self) -> list:
-        return self.definitions
-
-    def theme_use(self, name):
-        self.style.theme_use(name)
-
-    def can_handle(self, name):
-        return name in self.definitions
-
-
-class MultipleThemeModuleManager(ttk.Style):
-    modules = []
-    theme_list = None
-
-    def theme_names(self):
-        if self.theme_list is None:
-            MultipleThemeModuleManager.theme_list = list(super().theme_names())
-            for m in self.modules:
-                themes = m.theme_names()
-                for t in themes:
-                    if t not in self.theme_list:
-                        self.theme_list.append(t)
-        return self.theme_list
-
-    def theme_use(self, name):
-        theme_set = False
-        for m in self.modules:
-            if m.can_handle(name):
-                m.theme_use(name)
-                theme_set = True
-                break
-        if not theme_set:
-            super().theme_use(name)
-
-
-try:
-    import ttkbootstrap as ttkb
-
-    has_ttkbootsrap = True
-except ImportError:
-    pass
-
-try:
-    import sv_ttk
-
-    has_sv_ttk = True
-except ImportError:
-    pass
-try:
-    from ttkthemes.themed_style import ThemedStyle
-
-    has_ttkthemes = True
-except ImportError:
-    pass
-
-
-def get_ttk_style():
-    """Use ttkthemes if module is installed"""
-    global __style
-    if __style is None:
-        manager = MultipleThemeModuleManager()
-        if has_ttkthemes:
-            manager.modules.append(ttkthemesModule())
-        if has_sv_ttk:
-            manager.modules.append(SunValleyModule())
-        if has_ttkbootsrap:
-            manager.modules.append(ttkbModule())
-
-        __style = manager
-
-    return __style
+import pygubu
+import pygubu.widgets.simpletooltip as tooltip
+import pygubudesigner.services.widgets.treecomponentpaletteui as baseui
+from pygubudesigner.i18n import translator
+from pygubu.stockimage import StockImage, StockImageException
+
+
+baseui.i18n_translator = translator
+
+
+class TreeVisualState:
+    def __init__(self, tree: ttk.Treeview):
+        self.tree: ttk.Treeview = tree
+        self.expanded_nodes = []
+        self.focus = None
+
+    def save(self):
+        self.expanded_nodes = []
+        for item in self.tree.get_children():
+            if self.tree.item(item, "open"):
+                self.expanded_nodes.append(item)
+        self.focus = self.tree.focus()
+
+    def restore(self):
+        for item in self.expanded_nodes:
+            if self.tree.exists(item):
+                self.tree.item(item, open=True)
+        if self.focus and self.tree.exists(self.focus):
+            self.tree.see(self.focus)
+
+
+class TreeComponentPalette(baseui.TreeComponentPaletteUI):
+    KEY_PRESS_CB_MILISECONDS = 800
+
+    def __init__(self, master=None, **kw):
+        super().__init__(master, **kw)
+
+        self.on_add_widget = None  # callback to call on double click.
+        self._keypress_cbid = None
+        self.cptree.filter_func = self.custom_filter
+        tooltip.create(self.fb_show_alltk, "Show all Tk widgets")
+        self.setup_styles()
+        self.visual_state = TreeVisualState(self.cptree)
+        btn_image = StockImage.get("cancel-circle-16")
+        self.btn_filter_cancel.configure(image=btn_image)
+        self.project_custom_widget_prefixes = []
+
+    def setup_styles(self):
+        s = ttk.Style(self)
+        s.configure("TreeComponentPalette.Treeview", rowheight=30)
+
+    def custom_filter(
+        self, tree: ttk.Treeview, itemid: str, fvalue: str
+    ) -> bool:
+        txt = tree.item(itemid, "text").lower()
+        match_found = fvalue in txt
+        return match_found
+
+    def on_filter_keypress(self, event=None):
+        if self._keypress_cbid is not None:
+            self.after_cancel(self._keypress_cbid)
+        self._keypress_cbid = self.after(
+            self.KEY_PRESS_CB_MILISECONDS, self._on_filter_keypress_after
+        )
+
+    def _on_filter_keypress_after(self, event=None):
+        self.on_do_filter(event)
+        self._cbid = None
+
+    def on_do_filter(self, event=None):
+        self.cptree.filter_by(self.filter_text_var.get())
+
+    def on_filter_clear(self):
+        self.filter_text_var.set("")
+        self.cptree.filter_by("")
+
+    def on_show_alltk(self):
+        self.build_tree()
+
+    def build_tree(self):
+        self.visual_state.save()
+        self.cptree.filter_remove()
+        items = self.cptree.get_children()
+        self.cptree.delete(*items)
+        self.create_treeview_widget_list()
+        self.cptree.filter_by(self.filter_text_var.get())
+        self.visual_state.restore()
+
+    def create_treelist(self):
+        omit_tagset = {"tk", "ttk"}
+
+        # create unique tag set
+        tagset: set = set()
+        for c in pygubu.builder.CLASS_MAP.keys():
+            wc = pygubu.builder.CLASS_MAP[c]
+            tagset.update((str(tag) for tag in wc.tags))
+        tagset.difference_update(omit_tagset)
+
+        # Put every class in defined sections
+        treelist = []
+        for c in pygubu.builder.CLASS_MAP.keys():
+            wc = pygubu.builder.CLASS_MAP[c]
+
+            is_tk_only = "tk" in wc.tags and "ttk" not in wc.tags
+            if is_tk_only and not self.var_show_alltk.get():
+                continue
+
+            if wc.public is False:
+                show_widget = False
+                for prefix in self.project_custom_widget_prefixes:
+                    if c.startswith(prefix):
+                        show_widget = True
+                        break
+                if show_widget is False:
+                    continue
+            ctags = set((str(tag) for tag in wc.tags)) - omit_tagset
+            sections = tagset & ctags
+            for s in sections:
+                treelist.append((s, wc))
+
+        # sort tags by group and label
+        def by_label(t):
+            return f"{t[0]}{t[1].group}{t[1].label}"
+
+        treelist.sort(key=by_label)
+        return treelist
+
+    def create_treeview_widget_list(self):
+        treelist = self.create_treelist()
+        widgetlisttv = self.cptree
+
+        # Default widget image:
+        default_image = ""
+        try:
+            default_image = StockImage.get("22x22-tk.default")
+        except StockImageException:
+            pass
+
+        # Start building widget tree selector
+        sections = {}
+        for key, wc in treelist:
+            section = key
+            # insert section
+            if section not in sections:
+                sections[section] = widgetlisttv.insert(
+                    "", "end", iid=hash(section), text=section
+                )
+            # insert widget
+            w_image = default_image
+            try:
+                w_image = StockImage.get("22x22-{0}".format(wc.classname))
+            except StockImageException:
+                pass
+
+            label = f" {wc.label}"
+            widgetlisttv.insert(
+                sections[section],
+                "end",
+                text=label,
+                image=w_image,
+                tags="widget",
+                values=(wc.classname,),
+            )
+        widgetlisttv.tag_bind("widget", "<Double-1>", self.on_widgetlist_dclick)
+
+    def on_widgetlist_dclick(self, event):
+        tv = event.widget
+        sel = tv.selection()
+        if sel:
+            item = sel[0]
+            classname = tv.item(item, "values")[0]
+            self.on_add_widget_event(classname)
+
+    def on_add_widget_event(self, cname):
+        if self.on_add_widget:
+            self.on_add_widget(cname)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/util/gridcalculator.py` & `pygubu_designer-0.39/src/pygubudesigner/util/gridcalculator.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/util/keyboard.py` & `pygubu_designer-0.39/src/pygubudesigner/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/util/observable.py` & `pygubu_designer-0.39/src/pygubudesigner/util/observable.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/util/screens.py` & `pygubu_designer-0.39/src/pygubudesigner/util/screens.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/util/selecttool.py` & `pygubu_designer-0.39/src/pygubudesigner/util/selecttool.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgetdescr.py` & `pygubu_designer-0.39/src/pygubudesigner/widgetdescr.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 )
 from .util.observable import Observable
 
 logger = logging.getLogger(__name__)
 
 
 class WidgetMeta(WidgetMetaBase, Observable):
+    LAYOUT_MANAGER_CHANGED = 1
+    LAYOUT_PROPERTY_CHANGED = 2
+    PROPERTY_CHANGED = 4
+    PROPERTY_RO_CHANGED = 8
+    BINDING_CHANGED = 16
+    PROPERTY_BLANKED = 32  # Will use this when a property is unset.
+
     def __init__(
         self,
         cname,
         identifier,
         manager=None,
         properties_defaults=None,
         layout_defaults=None,
@@ -59,69 +66,80 @@
     def is_named(self, value: bool):
         if self.start_named is None:
             self.start_named = value
         super(WidgetMeta, type(self)).is_named.fset(self, value)
 
     def apply_layout_defaults(self):
         super().apply_layout_defaults()
-        self.notify("LAYOUT_CHANGED", self)
+        self.notify(self.LAYOUT_PROPERTY_CHANGED, self)
 
     def widget_property(self, name, value=None):
         if value is None:
             if name == "id":
                 return self.identifier
             elif name == "class":
                 return self.classname
             else:
                 return self.properties.get(name, "")
         else:
+            event_type = self.PROPERTY_CHANGED
             # Setter
             if name == "id":
                 self.identifier = value
+                event_type = event_type | self.PROPERTY_RO_CHANGED
             elif name == "class":
                 self.classname = value
+                event_type = event_type | self.PROPERTY_RO_CHANGED
             else:
                 if value:
                     self.properties[name] = value
                 else:
                     # remove if no value set
+                    event_type = event_type | self.PROPERTY_BLANKED
                     self.properties.pop(name, None)
-            self.notify("PROPERTY_CHANGED", self)
+                builder = CLASS_MAP[self.classname].builder
+                if name in builder.ro_properties:
+                    event_type = event_type | self.PROPERTY_RO_CHANGED
+            self.notify(event_type, self)
 
     def layout_property(self, name, value=None):
         if value is None:
             # Getter
             default = ""
             if name in ("row", "column"):
                 default = "0"
             return self.layout_properties.get(name, default)
         else:
+            event_type = self.LAYOUT_PROPERTY_CHANGED
             # Setter
             if value:
                 self.layout_properties[name] = value
             else:
                 # remove if no value set
+                event_type = event_type | self.PROPERTY_BLANKED
                 self.layout_properties.pop(name, None)
-            self.notify("LAYOUT_CHANGED", self)
+            self.notify(event_type, self)
 
     def container_property(self, name, value=None):
         if value is None:
             # Getter
             return self.container_properties.get(name, "")
         else:
+            event_type = self.LAYOUT_PROPERTY_CHANGED
             # do not save propagate if value is True
             if name == "propagate" and value.lower() == "true":
                 value = None
             # Setter
             if value:
                 self.container_properties[name] = value
             else:
                 # remove if no value set
+                event_type = event_type | self.PROPERTY_BLANKED
                 self.container_properties.pop(name, None)
-            self.notify("LAYOUT_CHANGED", self)
+            self.notify(event_type, self)
 
     def gridrc_property(self, type_, num, pname, value=None):
         if value is None:
             # Getter
             default = "0"
             if pname == "uniform":
                 default = ""
@@ -131,15 +149,15 @@
         else:
             # Setter
             self.set_gridrc_value(type_, num, pname, value)
 
     def gridrc_clear(self, notify_change=True):
         self.gridrc_properties = []
         if notify_change:
-            self.notify("LAYOUT_CHANGED")
+            self.notify(self.LAYOUT_PROPERTY_CHANGED)
 
     def gridrc_row_indexes(self):
         rows = set()
         for line in self.gridrc_properties:
             if line.rctype == "row":
                 rows.add(line.rcid)
         return list(rows)
@@ -156,15 +174,16 @@
         return self._manager
 
     @manager.setter
     def manager(self, value):
         if self._manager != value:
             self._manager = value
             self.clear_layout()
-        self.notify("LAYOUT_CHANGED", self)
+            self.notify(self.LAYOUT_MANAGER_CHANGED, self)
+        # self.notify("LAYOUT_CHANGED", self)
 
     def get_bindings(self):
         blist = []
         for v in self.bindings:
             blist.append((v.sequence, v.handler, v.add))
         return blist
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/__init__.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/bindingeditor.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/bindingeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/colorentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/colorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/commandentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/commandentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/componentpalette.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/componentpalette.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/containerlayouteditorbase.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/containerlayouteditorbase.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/cursorentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/cursorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/dimensionentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/dimensionentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/dynamicpropeditor.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/dynamicpropeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/entryvalidatecommandeditor.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/entryvalidatecommandeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/fontentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/fontentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/gridselector.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/gridselector.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/imageentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/imageentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/namedideditor.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/namedideditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/pixelcoordinateentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/pixelcoordinateentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/propertyeditor.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/propertyeditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,25 @@
 import tkinter as tk
 import tkinter.ttk as ttk
 
 from pygubu.widgets.combobox import Combobox
 from pygubu.widgets.scrollbarhelper import ScrollbarHelper
 
 EDITORS = {}
-KEY_PRESS_CB_MILISECONDS = 500
+KEY_PRESS_CB_MILISECONDS = 850
 
 
 def register_editor(name, class_):
     EDITORS[name] = class_
 
 
 def create_editor(name, *args, **kw):
+    if name not in EDITORS:
+        msg = f"Trying to use an unregister editor named: {name}"
+        raise Exception(msg)
     editor = EDITORS[name](*args, **kw)
     return editor
 
 
 class PropertyEditor(ttk.Frame):
     style_initialized = False
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/relativeentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/relativeentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/stickyentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/stickyentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/tkvarentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/tkvarentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/toolbarframe.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/toolbarframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,40 +57,62 @@
         self.controls_required = False
         self._scrollRecurse = 0
         self.timer = None
         self.fcontrols = fcontrols
         self.fvport = fvport
         self.fcontent = fcontent
         self.fcstart = 0
+        self._xvstatus = [1.0, 1.0]
         self.SCROLL_INCREMENT = 50
         fvport.bind("<Configure>", self._reposition)
         fcontent.bind("<Configure>", self._reposition)
         self._configure_mousewheel()
 
     def child_master(self):
         return self.fcontent
 
     def _configure_mousewheel(self):
         BindManager.init_mousewheel_binding(self)
-        self.bind(
-            "<Enter>",
-            lambda event: BindManager.mousewheel_bind(self),
-            add="+",
-        )
-        self.bind(
-            "<Leave>", lambda event: BindManager.mousewheel_unbind(), add="+"
-        )
+        BindManager.mousewheel_bind(self)
         self.on_mousewheel = BindManager.make_onmousewheel_cb(self, "x", 2)
 
     def xview(self, mode=None, value=None, units=None):
         if mode == "scroll":
-            if value > 0:
-                self.scroll_right()
-            else:
-                self.scroll_left()
+            vp_width = self.fvport.winfo_width()
+            content_width = self.fcontent.winfo_reqwidth()
+            if content_width > vp_width:
+                if value > 0:
+                    self.scroll_right()
+                else:
+                    self.scroll_left()
+        if mode is None and value is None:
+            return self._xvstatus
+
+    def scroll_right(self):
+        newstart = self.fcstart - self.SCROLL_INCREMENT
+        cw = self.fcontent.winfo_reqwidth()
+        f_width = self.fvport.winfo_width()
+        limit = cw - f_width
+        if newstart > -(limit):
+            self.fcstart = newstart
+        elif self.fcstart != -limit:
+            self.fcstart = -limit
+            self._xvstatus[0] = 0
+            self._xvstatus[1] = 1
+        self.fcontent.place(x=self.fcstart)
+
+    def scroll_left(self):
+        newstart = self.fcstart + self.SCROLL_INCREMENT
+        if newstart <= 0:
+            self.fcstart = newstart
+        elif self.fcstart < 0:
+            self.fcstart = 0
+            self._xvstatus[0] = 1
+            self._xvstatus[1] = 0
+        self.fcontent.place(x=self.fcstart)
 
     def toggle_controls(self):
         self.controls_visible = not self.controls_visible
         if self.controls_visible:
             self.fcontrols.pack(side="left", fill="y")
         else:
             self.fcontrols.pack_forget()
@@ -133,34 +155,13 @@
             if self.fcstart != 0:
                 self.fcstart = 0
                 self.fcontent.place(x=self.fcstart)
 
         if self.controls_required != self.controls_visible:
             self.toggle_controls()
 
-    def scroll_right(self):
-        newstart = self.fcstart - self.SCROLL_INCREMENT
-        cw = self.fcontent.winfo_reqwidth()
-        f_width = self.fvport.winfo_width()
-        limit = cw - f_width
-        if newstart > -(limit):
-            self.fcstart = newstart
-            self.fcontent.place(x=self.fcstart)
-        elif self.fcstart != -limit:
-            self.fcstart = -limit
-            self.fcontent.place(x=self.fcstart)
-
-    def scroll_left(self):
-        newstart = self.fcstart + self.SCROLL_INCREMENT
-        if newstart <= 0:
-            self.fcstart = newstart
-            self.fcontent.place(x=self.fcstart)
-        elif self.fcstart < 0:
-            self.fcstart = 0
-            self.fcontent.place(x=self.fcstart)
-
 
 if __name__ == "__main__":
     root = tk.Tk()
     widget = ToolbarFrame(root)
     widget.pack(expand=True, fill="both")
     root.mainloop()
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/ttkstyleentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/ttkstyleentry.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
 import tkinter as tk
 import tkinter.ttk as ttk
+from pygubu.theming.bootstrap.style import Style as BootstrapStyle
 
 from pygubudesigner.widgets.propertyeditor import (
     ChoicePropertyEditor,
     register_editor,
 )
 
 
@@ -46,23 +47,25 @@
     @classmethod
     def set_filter_hints(cls, hints):
         cls.STYLES_FILTER_HINTS = hints
 
     @classmethod
     def set_global_style_list(cls, style_list):
         cls.STYLES = style_list
+        cls.STYLES.extend(BootstrapStyle.get_generated_styles())
 
     def _create_style_options(self, styles):
-        new_list = [] if styles is None else list(styles)
+        new_list: list = [] if styles is None else list(styles)
         if self.STYLES_FILTER_HINTS:
             for s in self.STYLES:
                 for hint in self.STYLES_FILTER_HINTS:
                     if s.endswith(hint):
                         new_list.append(s)
                         break
+        new_list.sort()
         return new_list
 
 
 register_editor("ttkstylechoice", TtkStylePropertyEditor)
 
 
 if __name__ == "__main__":
```

### Comparing `pygubu-designer-0.38/src/pygubudesigner/widgets/whentry.py` & `pygubu_designer-0.39/src/pygubudesigner/widgets/whentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.38/tests/test_plugin_init.py` & `pygubu_designer-0.39/tests/test_plugin_init.py`

 * *Files identical despite different names*

