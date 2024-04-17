# Comparing `tmp/PyQtUIkit-2.5.1.tar.gz` & `tmp/PyQtUIkit-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.5.1.tar", last modified: Sun Apr 14 10:40:17 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.7.0.tar", last modified: Wed Apr 17 09:09:09 2024, max compression
```

## Comparing `PyQtUIkit-2.5.1.tar` & `PyQtUIkit-2.7.0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.333412 PyQtUIkit-2.5.1/
--rw-rw-rw-   0        0        0     1090 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-14 10:40:17.333412 PyQtUIkit-2.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.286546 PyQtUIkit-2.5.1/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.302162 PyQtUIkit-2.5.1/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.302162 PyQtUIkit-2.5.1/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.317784 PyQtUIkit-2.5.1/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.317784 PyQtUIkit-2.5.1/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1470 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.333412 PyQtUIkit-2.5.1/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1638 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7833 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2788 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    10054 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8253 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     2280 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     4994 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1487 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1424 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4336 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7084 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13348 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16164 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:40:17.302162 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-14 10:40:17.000000 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2525 2024-04-14 10:40:17.000000 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:40:17.000000 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-14 10:40:17.000000 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-14 10:40:17.000000 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-14 10:40:17.000000 PyQtUIkit-2.5.1/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 10:40:17.333412 PyQtUIkit-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-14 10:39:18.000000 PyQtUIkit-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.606049 PyQtUIkit-2.7.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-17 09:09:09.606049 PyQtUIkit-2.7.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.574805 PyQtUIkit-2.7.0/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     2606 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.574805 PyQtUIkit-2.7.0/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.574805 PyQtUIkit-2.7.0/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.590424 PyQtUIkit-2.7.0/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.590424 PyQtUIkit-2.7.0/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     3173 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1762 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/themes/local.py
+-rw-rw-rw-   0        0        0     1470 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.606049 PyQtUIkit-2.7.0/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1654 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3304 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7885 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2739 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    11101 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8328 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     2280 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     5174 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1697 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4336 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7084 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     4021 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13972 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2370 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16164 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:09:09.574805 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-17 09:09:09.000000 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2575 2024-04-17 09:09:09.000000 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 09:09:09.000000 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-17 09:09:09.000000 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 09:09:09.000000 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 09:09:09.000000 PyQtUIkit-2.7.0/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 09:09:09.606049 PyQtUIkit-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-17 09:08:20.000000 PyQtUIkit-2.7.0/setup.py
```

### Comparing `PyQtUIkit-2.5.1/LICENSE` & `PyQtUIkit-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PKG-INFO` & `PyQtUIkit-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.5.1
+Version: 2.7.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/_icons.py` & `PyQtUIkit-2.7.0/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.7.0/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.7.0/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.7.0/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/core/font.py` & `PyQtUIkit-2.7.0/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.7.0/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.7.0/PyQtUIkit/core/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,34 @@
 
         def setter(obj, value: str):
             setattr(obj, self._id, str(value))
 
         super().__init__(getter, setter)
 
 
+class TextProperty(property):
+    def __init__(self, name='', default=''):
+        self._id = '_' + (str(name) or str(uuid4()).replace('-', '_'))
+
+        def getter(obj) -> str:
+            try:
+                res = getattr(obj, self._id)
+                if isinstance(res, str):
+                    return res
+                return res.get(obj._tm)
+            except AttributeError:
+                return default
+
+        def setter(obj, value: str):
+            setattr(obj, self._id, value)
+            obj._apply_lang()
+
+        super().__init__(getter, setter)
+
+
 class IconProperty(property):
     def __init__(self, name=''):
         self._id = '_' + (str(name) or str(uuid4()).replace('-', '_'))
 
         def getter(obj) -> KitIcon | None:
             try:
                 icon = getattr(obj, self._id)
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.7.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.7.0/PyQtUIkit/themes/local.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,67 @@
-from PyQt6.QtGui import QPixmap, QImage, QIcon, QFontDatabase
+class KitLocal:
+    def __init__(self, lang: str, name: str, dct: dict[str: str]):
+        self.__lang = lang
+        self.__name = name
+        self.__dict = dct
 
-from PyQtUIkit.themes.builtin_themes import basic_theme, builtin_themes
-from PyQtUIkit.themes.icons import icons
-from PyQtUIkit.themes.svg import SVG
-from PyQtUIkit.themes.theme import KitTheme, KitPalette
-
-
-class ThemeManager:
-    def __init__(self, on_theme_changed):
-        self.__current_theme_name = 'Light'
-        self.__current_theme = basic_theme
-        self.__themes = builtin_themes
-        self.__on_theme_changed = on_theme_changed
-        self.__active = False
-
-        from importlib.resources import files
-        for file in files('PyQtUIkit.fonts').iterdir():
-            QFontDatabase.addApplicationFontFromData(file.read_bytes())
-
-    def add_theme(self, name: str, th: KitTheme):
-        self.__themes[name] = th
-
-    def set_theme(self, new_theme):
-        self.__current_theme = self.__themes.get(new_theme)
-        self.__current_theme_name = new_theme
-        self.__on_theme_changed()
+    def get(self, item):
+        return self.__dict[item]
+
+    def items(self):
+        return self.__dict.items()
 
     @property
-    def current_theme(self):
-        return self.__current_theme_name
+    def lang(self):
+        return self.__lang
 
     @property
-    def active(self):
-        return self.__active
+    def name(self):
+        return self.__name
+
 
-    def _set_active(self):
-        self.__active = KitTheme
+class _KitLocalString:
+    def __init__(self, key: str):
+        self.__key = key
+
+    def __add__(self, other):
+        return _KitLocalStringArray(self, other)
+    
+    def __radd__(self, other):
+        return _KitLocalStringArray(other, self)
+    
+    def get(self, tm):
+        return tm.get_text(self.__key)
+    
+    
+class _KitLocalStringArray:
+    def __init__(self, *args):
+        self.__args = args
+        
+    def get(self, tm):
+        lst = []
+        for el in self.__args:
+            if isinstance(el, _KitLocalString):
+                lst.append(el.get(tm))
+            elif callable(el):
+                lst.append(el(tm))
+            else:
+                lst.append(str(el))
+        return ''.join(lst)
+
+    def __add__(self, other):
+        if isinstance(other, _KitLocalStringArray):
+            return _KitLocalStringArray(*self.__args, *other.__args)
+        return _KitLocalStringArray(*self.__args, other)
+    
+    def __radd__(self, other):
+        if isinstance(other, _KitLocalStringArray):
+            return _KitLocalStringArray(*other.__args, *self.__args)
+        return _KitLocalStringArray(other, *self.__args)
+
+
+class _KitLocalStringClass:
+    def __getattr__(self, item):
+        return _KitLocalString(item)
 
-    def palette(self, key: str):
-        return self.__current_theme.palette(key)
 
-    def font(self, font):
-        return self.__current_theme.font(font)
-
-    def border(self):
-        return self.__current_theme.border()
-
-    def pixmap(self, name, color, size=None):
-        icon = SVG(icons[name])
-        icon.change_color(color)
-        if size:
-            icon.resize(*size)
-        return QPixmap.fromImage(QImage.fromData(icon.bytes()))
-
-    def icon(self, name, color=None, size=None):
-        return QIcon(self.pixmap(name, color, size))
-
-    @staticmethod
-    def add_icon(icon: str, name: str):
-        """
-        Add icon (from .svg file or from data)
-        :param icon: path to file or data
-        :param name: icon name, str
-        :return:
-        """
-        if icon.endswith('.svg'):
-            with open(icon, encoding='utf-8') as f:
-                icon = f.read()
-        icons[name] = icon
+KitLocalString = _KitLocalStringClass()
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.7.0/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.7.0/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.7.0/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.7.0/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.button import KitButton, KitIconButton, KitLayoutButton
 from PyQtUIkit.widgets.line_edit import KitLineEdit
 from PyQtUIkit.widgets.list_widget import KitListWidget, KitListWidgetItem
 from PyQtUIkit.widgets.main_window import KitMainWindow
 from PyQtUIkit.widgets.spin_box import KitSpinBox
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.combo_box import KitComboBox, KitComboBoxItem
+from PyQtUIkit.widgets.combo_box import KitComboBox, KitComboBoxItem, KitLanguageBox
 from PyQtUIkit.widgets.checkbox import KitCheckBox
 from PyQtUIkit.widgets.toggle import KitToggle
 from PyQtUIkit.widgets.tab_bar import KitTabBar, KitTab
 from PyQtUIkit.widgets.spinner import KitSpinner
 from PyQtUIkit.widgets.progress_bar import KitProgressBar
 from PyQtUIkit.widgets.tree_widget import KitTreeWidget, KitTreeWidgetItem
 from PyQtUIkit.widgets.menu import KitMenu
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-from typing import Callable
-
-from PyQtUIkit.builder import BUILDER
 from PyQtUIkit.core.properties import PaletteProperty, IntProperty
 from PyQtUIkit.themes import ThemeManager
 
 
 class _KitWidget:
     main_palette = PaletteProperty('main_palette')
     border_palette = PaletteProperty('border_palette', 'Border')
 
     def __init__(self):
         self._tm: ThemeManager = None
         self._add_child_func = lambda x: None
 
-    def _build_from_kui(self):
-        BUILDER.build_from_file(self, self._add_child_func)
-
-    def _build_from_kui_as_child(self, _class, vars):
-        BUILDER.build(_class, self, self._add_child_func, vars)
-
     def _set_tm(self, tm: ThemeManager):
         self._tm = tm
         if tm and tm.active:
             self._apply_theme()
+            self._apply_lang()
 
     @property
     def theme_manager(self):
         return self._tm
 
     def _apply_theme(self):
         pass
 
+    def _apply_lang(self):
+        pass
+
 
 class KitGroup:
     NO_GROUP = 0
     HORIZONTAL = 1
     VERTICAL = 2
     FIRST = 3
     MIDDLE = 4
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/button.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, QMargins
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QHBoxLayout, QWidget
 
 from PyQtUIkit.core import IconProperty, EnumProperty, PaletteProperty, KitFont, FontProperty, \
-    SignalProperty, MethodsProperty
+    SignalProperty, MethodsProperty, TextProperty
 from PyQtUIkit.themes import ThemeManager
 from PyQtUIkit.widgets import KitIconWidget
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     icon = IconProperty('icon')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
     on_click = SignalProperty('on_click', 'clicked')
+    text = TextProperty('text')
 
     def __init__(self, text='', icon=None):
         super().__init__()
         self.__widgets = []
         self.setCursor(Qt.CursorShape.PointingHandCursor)
 
-        self.setText(text)
+        self._text = text
         self._icon = icon
 
-        self._build_from_kui()
-
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
@@ -56,15 +55,18 @@
     subcontrol-origin: padding;
     padding-right: 5px;
     subcontrol-position: right;
 }}""")
         if self.icon is not None:
             self.setIcon(self.icon.icon(self.main_palette.text))
 
-    text = MethodsProperty(QPushButton.text, QPushButton.setText)
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        self.setText(self.text)
 
 
 class KitIconButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     icon = IconProperty('icon')
     on_click = SignalProperty('on_click', 'clicked')
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/checkbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,35 +6,37 @@
 from PyQtUIkit.widgets.button import KitIconButton
 
 
 class KitCheckBox(QWidget, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    text = TextProperty('text')
 
     stateChanged = pyqtSignal(bool)
     stateEdited = pyqtSignal(bool)
 
     def __init__(self, text=''):
         super().__init__()
         self.__state = False
+        self._text = text
         self.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Minimum)
 
         main_layout = QHBoxLayout()
         main_layout.setAlignment(Qt.AlignmentFlag.AlignLeft)
         main_layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(main_layout)
 
         self.__button = KitIconButton()
         self.__button.setCheckable(True)
         self.__button.clicked.connect(self._on_clicked)
         self.__button.size = 16
         main_layout.addWidget(self.__button)
 
-        self.__label = QPushButton(text)
+        self.__label = QPushButton()
         self.__label.clicked.connect(self._on_clicked)
         main_layout.addWidget(self.__label)
         if not text:
             self.__label.hide()
 
     def _on_clicked(self):
         self.__state = not self.__state
@@ -49,20 +51,14 @@
     def isChecked(self):
         return self.__state
 
     def setChecked(self, state):
         self.__state = bool(state)
         self.__on_state_changed()
 
-    def setText(self, text):
-        self.__label.setText(text)
-
-    def getText(self):
-        return self.__label.text()
-
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__button._set_tm(tm)
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
@@ -72,11 +68,13 @@
         self.__label.setStyleSheet(f"""
         QPushButton {{
             color: {self.main_palette.text};
             background-color: transparent;
             text-align: left;
         }}""")
 
+    def _apply_lang(self):
+        self.__label.setText(self.text)
+
     state = MethodsProperty(isChecked, setChecked)
-    text = MethodsProperty(getText, setText)
     on_state_changed = SignalProperty('on_state_changed', 'stateChanged')
     on_state_edited = SignalProperty('on_state_edited', 'stateEdited')
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/combo_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from PyQt6.QtCore import pyqtSignal, Qt, QPoint, QPropertyAnimation, QEasingCurve, QSize, QParallelAnimationGroup
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QMenu, QHBoxLayout, QApplication
 
 from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty, \
-    MethodsProperty
+    MethodsProperty, TextProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget, KitGroupItem as _KitGroupItem
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.layout import KitVBoxLayout
 from PyQtUIkit.widgets.button import KitLayoutButton
 
 
 class KitComboBoxItem(QPushButton, _KitWidget):
     selected = pyqtSignal(object)
     icon = IconProperty('icon')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    text = TextProperty('text')
 
     def __init__(self, name='', value=None, icon=''):
         super().__init__()
-        self._name = name
+        self._text = name
         self._value = value if value is not None else name
         self._icon = icon
         self.setCheckable(True)
         self.clicked.connect(self._on_clicked)
-        self.setText(self._name)
         self.setFixedHeight(24)
         self.setCursor(Qt.CursorShape.PointingHandCursor)
 
     def _on_clicked(self, flag):
         if not flag:
             self.setChecked(True)
         self.selected.emit(self)
@@ -55,15 +55,16 @@
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
 }}""")
         if self.icon is not None:
             self.setIcon(self.icon.icon(self.main_palette.text))
 
-    name = MethodsProperty(QPushButton.text, QPushButton.setText)
+    def _apply_lang(self):
+        self.setText(self.text)
 
 
 class KitComboBox(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     type = IntProperty('type', 1)
     icon = IconProperty('icon')
     font = FontProperty('font')
@@ -90,15 +91,14 @@
         self._arrow.setFixedSize(16, 12)
         layout.addWidget(self._arrow)
 
         for el in values:
             self.addItem(el)
 
         self._add_child_func = self.addItem
-        self._build_from_kui()
 
     def addItem(self, item: str | KitComboBoxItem, value=None):
         if not isinstance(item, KitComboBoxItem):
             item = KitComboBoxItem(item, value)
         item.selected.connect(self._on_item_selected)
         self.__widgets.append(item)
         self.__menu.add_item(item)
@@ -123,27 +123,30 @@
         self.setText('')
 
     def currentItem(self):
         if not self.__widgets:
             return None
         return self.__widgets[self.__current]
 
+    def count(self):
+        return len(self.__widgets)
+
     def currentValue(self):
         if not self.__widgets:
             return None
         return self.__widgets[self.__current].value
 
     def setCurrentIndex(self, index):
         if self.__current is not None:
             self.__widgets[self.__current].setChecked(False)
         self.__current = index
         self.__widgets[self.__current].setChecked(True)
 
         if self.__current is not None:
-            self.setText(self.__widgets[self.__current].text())
+            self.setText(self.__widgets[self.__current].text)
             if self.__widgets[self.__current].icon is not None and self._tm and self._tm.active:
                 self.setIcon(self.__widgets[self.__current].icon.icon(self.main_palette.text))
         self.currentValueChanged.emit(self.currentValue())
         self.currentIndexChanged.emit(self.__current)
 
     def _show_menu(self):
         pos = QPoint(0, self.height() if self.type == 1 else self.height() // 2)
@@ -188,14 +191,22 @@
     border: {self.border}px solid {self.border_palette.selected};
 }}""")
         if self.__current is not None and self.__widgets[self.__current].icon is not None:
             self.setIcon(self.__widgets[self.__current].icon.icon(self.main_palette.text))
         self.__menu._apply_theme()
         self._arrow._apply_theme()
 
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        item = self.currentItem()
+        self.setText('' if not item else item.text)
+        for el in self.__widgets:
+            el._apply_lang()
+
 
 class _ComboBoxMenu(QMenu, _KitWidget):
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self):
         super().__init__()
@@ -273,7 +284,33 @@
 
         self.__anim = QParallelAnimationGroup()
         self.__anim.addAnimation(pos_anim)
         self.__anim.addAnimation(height_anim)
         self.__anim.start()
 
         self.exec()
+
+
+class KitLanguageBox(KitComboBox):
+    langChanged = pyqtSignal(str)
+
+    def __init__(self):
+        super().__init__()
+        self.__loading = False
+        self.currentValueChanged.connect(self._on_value_changed)
+
+    def _on_value_changed(self, value):
+        if self.__loading:
+            return
+        self.theme_manager.set_lang(value)
+        self.langChanged.emit(value)
+
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        self.__loading = True
+        self.clear()
+        for lang, name in self.theme_manager.get_languages():
+            self.addItem(KitComboBoxItem(name, lang))
+            if lang == self.theme_manager.lang:
+                self.setCurrentIndex(self.count() - 1)
+        self.__loading = False
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QDialog, QVBoxLayout, QLabel
 
-from PyQtUIkit.core.properties import PaletteProperty, BoolProperty, StringProperty, IconProperty
+from PyQtUIkit.core.properties import PaletteProperty, BoolProperty, StringProperty, IconProperty, TextProperty
 from PyQtUIkit.widgets import KitIconButton, KitHBoxLayout, KitVBoxLayout, KitButton, KitIconWidget, KitLabel
 from PyQtUIkit.widgets.form import KitForm
 from PyQtUIkit.widgets._widget import _KitWidget
 
 
 class KitDialog(QDialog, _KitWidget):
     header_palette = PaletteProperty('header_palette', 'Menu')
     button_close = BoolProperty('button_close', True)
-    name = StringProperty('name', '')
+    name = TextProperty('name')
 
     def __init__(self, parent):
         super().__init__()
         self._main_palette = 'Bg'
         self._parent = parent
         self.setWindowFlag(Qt.WindowType.FramelessWindowHint)
 
@@ -69,25 +69,28 @@
     def _apply_theme(self):
         self.__top_widget.main_palette = self.header_palette
         self.__button_close.main_palette = self.header_palette
         self.__button_close.setHidden(not self.button_close)
         self.__label.setHidden(not self.name)
         self.__top_widget.setHidden(not self.button_close and not self.name)
 
-        self.__label.setText(self.name)
         css = f"""color: {self.main_palette.text};
                   background-color: {self.main_palette.main};
                   border: 1px solid {self.border_palette.main};
                   border-radius: 5px;"""
         self.setStyleSheet(css)
 
         self.__top_widget._set_tm(self._parent._tm)
         self.__widget._set_tm(self._parent._tm)
         super()._apply_theme()
 
+    def _apply_lang(self):
+        self.__label.setText(self.name)
+        self.__widget._apply_lang()
+
     @staticmethod
     def question(parent, question: str, answers=('No', 'Yes'), default='No'):
         dialog = _KitAskDialog(parent, question, answers, default)
         dialog.exec()
         return dialog.answer
 
     @staticmethod
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/label.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from PyQt6.QtWidgets import QLabel
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
+from PyQtUIkit.core import IntProperty, PaletteProperty, EnumProperty, KitFont, FontProperty, TextProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitLabel(QLabel, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Transparent')
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    text = TextProperty('text')
 
     def __init__(self, text=''):
-        super().__init__(text)
+        super().__init__()
+        self._text = text
         self._use_text_only = True
-        self._build_from_kui()
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
         QWidget {{
             color: {self.main_palette.text_only if self._use_text_only else self.main_palette.text};
             background-color: transparent;
             border: none;
         }}""")
 
-    text = MethodsProperty(QLabel.text, QLabel.setText)
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        self.setText(self.text)
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
         self.__layout = QVBoxLayout() if orientation == Qt.Orientation.Vertical else QHBoxLayout()
         self.__layout.setContentsMargins(0, 0, 0, 0)
         self.__layout.setSpacing(0)
         strange_widget.setLayout(self.__layout)
 
         self._add_child_func = self.addWidget
-        self._build_from_kui()
 
     def addWidget(self, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.addWidget(widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.addWidget(widget, stretch)
         else:
@@ -114,14 +113,21 @@
         QWidget {{
             background-color: {self.main_palette.main};
             border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
 
+    def _apply_lang(self):
+        if not self._tm or not self._tm.active:
+            return
+        for el in self._widgets:
+            if hasattr(el, '_apply_theme'):
+                el._apply_lang()
+
     padding = MethodsProperty(getContentsMargins, _set_margins)
     spacing = MethodsProperty(getSpacing, setSpacing)
     alignment = MethodsProperty(getAlignment, setAlignment)
     max_width = MethodsProperty(QWidget.maximumWidth, QWidget.setMaximumWidth)
     min_width = MethodsProperty(QWidget.minimumWidth, QWidget.setMinimumWidth)
     max_height = MethodsProperty(QWidget.maximumHeight, QWidget.setMaximumHeight)
     min_height = MethodsProperty(QWidget.minimumHeight, QWidget.setMinimumHeight)
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/line_edit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from PyQt6.QtWidgets import QLineEdit
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty, SignalProperty
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty, SignalProperty, \
+    TextProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitLineEdit(QLineEdit, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
     font = FontProperty('font')
+    placeholder_text = TextProperty('placeholder_text')
 
     def __init__(self, text=''):
         super().__init__(text)
         self.__widgets = []
         self.border = 1
         self.radius = 4
 
@@ -32,10 +34,15 @@
     background-color: {self.main_palette.hover};
 }}
 QLineEdit:focus {{
     border: {self.border}px solid {self.border_palette.selected};
     background-color: {self.main_palette.hover};
 }}""")
 
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        self.setPlaceholderText(self.placeholder_text)
+
     text = MethodsProperty(QLineEdit.text, QLineEdit.setText)
     on_text_changed = SignalProperty('on_text_changed', 'textChanged')
     on_text_edited = SignalProperty('on_text_edited', 'textEdited')
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/main_window.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from PyQtUIkit.themes import ThemeManager
 
 
 class KitMainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
-        self._tm = ThemeManager(self._apply_theme)
+        self._tm = ThemeManager(self._apply_theme, self._apply_lang)
         self.__menu_bar = None
 
     @property
     def theme_manager(self):
         return self._tm
 
     def _apply_theme(self):
@@ -20,14 +20,23 @@
             return
         cw = self.centralWidget()
         if hasattr(cw, '_apply_theme'):
             cw._apply_theme()
         if hasattr(self.__menu_bar, '_apply_theme'):
             self.__menu_bar._apply_theme()
 
+    def _apply_lang(self):
+        if not self._tm.active:
+            return
+        cw = self.centralWidget()
+        if hasattr(cw, '_apply_lang'):
+            cw._apply_lang()
+        if hasattr(self.__menu_bar, '_apply_lang'):
+            self.__menu_bar._apply_lang()
+
     def setCentralWidget(self, widget: typing.Optional[QWidget]) -> None:
         super().setCentralWidget(widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
             widget.main_palette = 'Bg'
             widget.radius = 0
 
@@ -38,12 +47,13 @@
             menubar._set_tm(self._tm)
 
     def show(self) -> None:
         super().show()
         if not self._tm.active:
             self._tm._set_active()
             self._apply_theme()
+            self._apply_lang()
 
     def set_theme(self, theme):
         self._tm.set_theme(theme)
         if self._tm.active:
             self._apply_theme()
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/scroll_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,7 +115,12 @@
     subcontrol-position: left;
     subcontrol-origin: margin;
 }}
 """)
         widget = self.widget()
         if hasattr(widget, '_apply_theme'):
             widget._apply_theme()
+
+    def _apply_lang(self):
+        widget = self.widget()
+        if hasattr(widget, '_apply_lang'):
+            widget._apply_lang()
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/tab_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,20 @@
         self.__button_close.radius = 8
         self.__button_close.hide()
         self.__button_close.on_click = self.closeRequested.emit
         layout.addWidget(self.__button_close)
 
         self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
+    def currentIndex(self):
+        return self.__tabs.index(self.__current)
+
+    def currentTab(self):
+        return self.__current
+
     def _set_checked(self, flag):
         self.__checked = flag
         self._apply_theme()
 
     def mousePressEvent(self, e) -> None:
         super().mousePressEvent(e)
         if e.button() == Qt.MouseButton.LeftButton:
@@ -129,15 +135,15 @@
 
         self.__label._apply_theme()
         self.__icon_widget.setHidden(not self.icon)
         self.__icon_widget.icon = self.icon
         self.__button_close._apply_theme()
 
 
-class KitTabBar(KitHBoxLayout, _KitWidget):
+class KitTabBar(KitHBoxLayout):
     tabs_palette = PaletteProperty('tabs_palette', 'Main')
     height = IntProperty('height', 26)
     radius_top = IntProperty('radius_top', 6)
     radius_bottom = IntProperty('radius_bottom', 0)
 
     currentChanged = pyqtSignal(object)
     tabCloseRequested = pyqtSignal(int)
@@ -150,47 +156,64 @@
         self.__tabs_closable = False
         self.__tabs_movable = False
         self.setContentsMargins(0, 0, 0, 0)
         self.radius = 0
         self.setSpacing(0)
         self._main_palette = 'Bg'
 
-        self.__button_left = KitButton(icon='line-chevron-left')
+        self.__button_left = KitButton(icon='line-chevron-back')
         self.__button_left.border = 0
         self.__button_left.setFixedWidth(20)
         self.__button_left.clicked.connect(self._scroll_left)
         self.addWidget(self.__button_left)
 
         self.__scroll_area = KitScrollArea()
         self.addWidget(self.__scroll_area)
         self.__layout = _TabLayout(self.__tabs)
         self.__scroll_area.setWidget(self.__layout)
         self.__layout.tabMoved.connect(self.tabMoved.emit)
         self.__scroll_area.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 
-        self.__button_right = KitButton(icon='line-chevron-right')
+        self.__button_right = KitButton(icon='line-chevron-forward')
         self.__button_right.border = 0
         self.__button_right.setFixedWidth(20)
         self.__button_right.clicked.connect(self._scroll_right)
         self.addWidget(self.__button_right)
 
+    def currentIndex(self):
+        return self.__tabs.index(self.__current)
+
+    def currentTab(self):
+        return self.__current
+
+    def tab(self, index):
+        return self.__tabs[index]
+
     def addTab(self, tab: str | KitTab):
         self.insertTab(len(self.__tabs), tab)
 
     def insertTab(self, index, tab: str | KitTab):
         if isinstance(tab, str):
             tab = KitTab(tab)
         tab._set_closable(self.__tabs_closable)
+
+        if self._tm and self._tm.active:
+            tab.main_palette = self.tabs_palette
+            tab.radius_top = self.radius_top
+            tab.radius_bottom = self.radius_bottom
+            tab.setFixedHeight(self.height)
+
         tab._set_tm(self._tm)
         tab.selected.connect(lambda: self.setCurrentTab(tab))
         tab.closeRequested.connect(lambda: self._close_requested(tab))
         tab._mousePress.connect(self.__layout.on_mouse_press)
         tab._mouseRelease.connect(self.__layout.on_mouse_release)
         self.__tabs.insert(index, tab)
         self.__layout.update_tabs()
+        tab.show()
         if self.__current is None:
             self.__current = tab
             tab._set_checked(True)
 
     def _scroll_left(self):
         self.__scroll_area.scroll(-50)
 
@@ -223,14 +246,15 @@
         self.currentChanged.emit(None if tab is None else self.__tabs.index(tab))
 
     def tabsCount(self):
         return len(self.__tabs)
 
     def removeTab(self, index):
         tab = self.__tabs.pop(index)
+        tab.setParent(None)
         self.__layout.update_tabs()
         if self.__current == tab:
             self.setCurrentTab(min(index, self.tabsCount() - 1))
         self.__button_left.setHidden(self.__layout.width() <= self.width())
         self.__button_right.setHidden(self.__layout.width() <= self.width())
 
     def _set_tm(self, tm):
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/text_edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from PyQt6.QtWidgets import QTextEdit
 
 from PyQtUIkit.core import KitFont
-from PyQtUIkit.core.properties import IntProperty, PaletteProperty, EnumProperty, FontProperty
+from PyQtUIkit.core.properties import IntProperty, PaletteProperty, EnumProperty, FontProperty, TextProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitTextEdit(QTextEdit, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    placeholder_text = TextProperty('placeholder_text')
 
     def __init__(self):
         super().__init__()
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
@@ -66,7 +67,12 @@
 QTextEdit QScrollBar::sub-line, QScrollBar::add-line {{
     background: none;
     height: 0px;
     subcontrol-position: left;
     subcontrol-origin: margin;
 }}
 """)
+
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        self.setPlaceholderText(self.placeholder_text)
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.7.0/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.7.0/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.5.1
+Version: 2.7.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.5.1/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.7.0/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 setup.py
 PyQtUIkit/__init__.py
 PyQtUIkit/_icons.py
+PyQtUIkit/_translate.py
 PyQtUIkit.egg-info/PKG-INFO
 PyQtUIkit.egg-info/SOURCES.txt
 PyQtUIkit.egg-info/dependency_links.txt
 PyQtUIkit.egg-info/entry_points.txt
 PyQtUIkit.egg-info/requires.txt
 PyQtUIkit.egg-info/top_level.txt
 PyQtUIkit/builder/__init__.py
@@ -41,14 +42,15 @@
 PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
 PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
 PyQtUIkit/fonts/RobotoMono-Thin.ttf
 PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
 PyQtUIkit/themes/__init__.py
 PyQtUIkit/themes/builtin_themes.py
 PyQtUIkit/themes/icons.py
+PyQtUIkit/themes/local.py
 PyQtUIkit/themes/svg.py
 PyQtUIkit/themes/theme.py
 PyQtUIkit/widgets/__init__.py
 PyQtUIkit/widgets/_widget.py
 PyQtUIkit/widgets/application.py
 PyQtUIkit/widgets/button.py
 PyQtUIkit/widgets/checkbox.py
```

### Comparing `PyQtUIkit-2.5.1/setup.py` & `PyQtUIkit-2.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         package_dir={'PyQtUIkit': 'PyQtUIkit'},
         packages=find_packages(include=['PyQtUIkit*']),
         package_data={
             '': ['fonts/*.ttf'],
         },
         entry_points={
             'console_scripts': [
-                'kit-icons = PyQtUIkit._icons:main'
+                'kit-icons = PyQtUIkit._icons:main',
+                'kit-translator = PyQtUIkit._translate:main'
             ]
         },
         description='A PyQtUIkit package.',
         install_requires=requirements(),
         python_requires='>=3.10'
     )
```

