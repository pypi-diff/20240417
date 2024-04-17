# Comparing `tmp/pomcorn-0.5.0.tar.gz` & `tmp/pomcorn-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomcorn-0.5.0.tar", max compression
+gzip compressed data, was "pomcorn-0.6.0.tar", max compression
```

## Comparing `pomcorn-0.5.0.tar` & `pomcorn-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2024-01-09 13:36:54.865481 pomcorn-0.5.0/LICENSE
--rw-r--r--   0        0        0     5575 2024-01-31 09:56:03.616874 pomcorn-0.5.0/README.rst
--rw-r--r--   0        0        0      362 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/__init__.py
--rw-r--r--   0        0        0     8623 2024-01-31 10:04:31.858940 pomcorn-0.5.0/pomcorn/component.py
--rw-r--r--   0        0        0    12195 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/element.py
--rw-r--r--   0        0        0     1131 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/exceptions.py
--rw-r--r--   0        0        0      708 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/locators/__init__.py
--rw-r--r--   0        0        0     4432 2024-01-24 06:36:06.862654 pomcorn-0.5.0/pomcorn/locators/base_locators.py
--rw-r--r--   0        0        0     6507 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/locators/xpath_locators.py
--rw-r--r--   0        0        0     5239 2024-01-24 06:36:06.862654 pomcorn-0.5.0/pomcorn/page.py
--rw-r--r--   0        0        0        0 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/py.typed
--rw-r--r--   0        0        0     3493 2024-01-09 13:36:54.872148 pomcorn-0.5.0/pomcorn/waits_conditions.py
--rw-r--r--   0        0        0    14179 2024-01-24 06:36:26.579442 pomcorn-0.5.0/pomcorn/web_view.py
--rw-r--r--   0        0        0     4891 2024-01-31 10:08:47.341650 pomcorn-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6644 1970-01-01 00:00:00.000000 pomcorn-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-11-03 07:21:01.198224 pomcorn-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5575 2024-04-17 04:56:14.335184 pomcorn-0.6.0/README.rst
+-rw-r--r--   0        0        0      362 2024-04-17 04:56:14.338518 pomcorn-0.6.0/pomcorn/__init__.py
+-rw-r--r--   0        0        0     8632 2024-04-17 05:35:02.245643 pomcorn-0.6.0/pomcorn/component.py
+-rw-r--r--   0        0        0    12195 2024-04-17 04:56:14.338518 pomcorn-0.6.0/pomcorn/element.py
+-rw-r--r--   0        0        0     1131 2023-12-22 03:42:38.510939 pomcorn-0.6.0/pomcorn/exceptions.py
+-rw-r--r--   0        0        0      708 2023-11-15 05:02:19.832416 pomcorn-0.6.0/pomcorn/locators/__init__.py
+-rw-r--r--   0        0        0     4432 2024-04-09 08:40:32.948820 pomcorn-0.6.0/pomcorn/locators/base_locators.py
+-rw-r--r--   0        0        0     7202 2024-04-17 05:37:54.531002 pomcorn-0.6.0/pomcorn/locators/xpath_locators.py
+-rw-r--r--   0        0        0     5436 2024-04-17 05:37:35.678177 pomcorn-0.6.0/pomcorn/page.py
+-rw-r--r--   0        0        0        0 2023-11-03 07:21:01.218224 pomcorn-0.6.0/pomcorn/py.typed
+-rw-r--r--   0        0        0     3493 2024-04-17 04:56:14.338518 pomcorn-0.6.0/pomcorn/waits_conditions.py
+-rw-r--r--   0        0        0    14179 2024-04-17 04:56:14.338518 pomcorn-0.6.0/pomcorn/web_view.py
+-rw-r--r--   0        0        0     4891 2024-04-17 05:51:27.976730 pomcorn-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6644 1970-01-01 00:00:00.000000 pomcorn-0.6.0/PKG-INFO
```

### Comparing `pomcorn-0.5.0/LICENSE` & `pomcorn-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/README.rst` & `pomcorn-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pomcorn/component.py` & `pomcorn-0.6.0/pomcorn/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         base_locator: locators.XPathLocator | None = None,
         wait_until_visible: bool = True,
     ):
         """Initialize component.
 
         Args:
             page: An instance of the page that uses this component.
-            base_locator: locator: Instance of a class to locate the element in
+            base_locator: Instance of a class to locate the element in
                 the browser. Used in relative element initialization methods
                 and visibility waits. You also can specify it as attribute.
             wait_until_visible: Whether to wait for the component to become
                 visible before completing initialization or not.
 
         """
         super().__init__(page)
@@ -247,15 +247,15 @@
         if (
             base_item := self.init_element(locator=self.base_item_locator)
         ).exists_in_dom:
             base_item.wait_until_visible()
 
         items: list[ListItemType] = []
         for locator in self.iter_locators(self.base_item_locator):
-            items.append(self.item_class(self.page, locator))
+            items.append(self.item_class(page=self.page, base_locator=locator))
         return items
 
     def get_item_by_text(self, text: str) -> ListItemType:
         """Get list item by text."""
         locator = self.base_item_locator.extend_query(
             extra_query=f"[contains(.,'{text}')]",
         )
```

### Comparing `pomcorn-0.5.0/pomcorn/element.py` & `pomcorn-0.6.0/pomcorn/element.py`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pomcorn/exceptions.py` & `pomcorn-0.6.0/pomcorn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pomcorn/locators/__init__.py` & `pomcorn-0.6.0/pomcorn/locators/__init__.py`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pomcorn/locators/base_locators.py` & `pomcorn-0.6.0/pomcorn/locators/base_locators.py`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pomcorn/locators/xpath_locators.py` & `pomcorn-0.6.0/pomcorn/locators/xpath_locators.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,30 +196,57 @@
                 must match exactly. By default, the search is based on a
                 partial match of the value.
 
         """
         super().__init__(text=text, element="button", exact=exact)
 
 
-class InputByLabelLocator(XPathLocator):
+class InputInLabelLocator(XPathLocator):
     """Locator to looking for input with label by XPath.
 
     Specify the query as the string
     ``//label[contains(., "label")]//input``, where ``label`` is the text of
     the input label.
 
+    Example:
+        <label>Title</label>
+            <input value="Value">
+        </label>
+
     """
 
     def __init__(self, label: str):
         """Init XPathLocator."""
         super().__init__(
             query=f'//label[contains(., "{label}")]//input',
         )
 
 
+class InputByLabelLocator(XPathLocator):
+    """Locator to looking for input next to label by XPath.
+
+    Specify the query as the string
+    ``//label[contains(., "label")]/following-sibling::input``, where ``label``
+    is the text of the input label.
+
+    Example:
+        <div>
+            <label for="InputWithLabel">Title</label>
+            <input id="InputWithLabel" value="Value">
+        </div>
+
+    """
+
+    def __init__(self, label: str):
+        """Init XPathLocator."""
+        super().__init__(
+            query=f'//label[contains(., "{label}")]/following-sibling::input',
+        )
+
+
 class TextAreaByLabelLocator(XPathLocator):
     """Locator to looking for textarea with label by XPath.
 
     Specify the query as the string
     ``//*[label[contains(text(), "{label}")]]/textarea``, where ``label``
     is the text of the textarea label.
```

### Comparing `pomcorn-0.5.0/pomcorn/page.py` & `pomcorn-0.6.0/pomcorn/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Self
 
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.remote.webdriver import WebDriver
 
-from . import locators
 from .exceptions import PageDidNotLoadedError
 from .web_view import WebView
 
 
 class Page(WebView):
     """The class for representing a web page.
 
@@ -142,22 +141,27 @@
             relative_url (str): Relative URL
 
         """
         self.webdriver.get(
             self._get_full_relative_url(self.app_root, relative_url),
         )
 
-    def click_on_page(self):
-        """Click on page `html` tag.
+    def click_on_page(self) -> None:
+        """Click on (1, 1) coordinates in the upper left corner of the page.
 
         Allows you to move focus away from an element, for example, if it
         is currently unavailable for interaction.
 
         """
-        self.init_element(locator=locators.TagNameLocator("html")).click()
+        from selenium.webdriver.common.action_chains import ActionChains
+
+        ActionChains(self.webdriver).move_by_offset(
+            xoffset=1,  # cspell:disable-line
+            yoffset=1,  # cspell:disable-line
+        ).click().perform()
 
     @staticmethod
     def _get_full_relative_url(app_root: str, relative_url: str) -> str:
         """Add relative URL to application root URL.
 
         Args:
             relative_url (str): Relative URL
```

### Comparing `pomcorn-0.5.0/pomcorn/waits_conditions.py` & `pomcorn-0.6.0/pomcorn/waits_conditions.py`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pomcorn/web_view.py` & `pomcorn-0.6.0/pomcorn/web_view.py`

 * *Files identical despite different names*

### Comparing `pomcorn-0.5.0/pyproject.toml` & `pomcorn-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pomcorn"
-version = "0.5.0"
+version = "0.6.0"
 description = "Base implementation of Page Object Model"
 authors = [
   "Saritasa <pypi@saritasa.com>",
 ]
 maintainers = [
     "Anton Oboleninov <anton.oboleninov@saritasa.com>",
 ]
```

### Comparing `pomcorn-0.5.0/PKG-INFO` & `pomcorn-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomcorn
-Version: 0.5.0
+Version: 0.6.0
 Summary: Base implementation of Page Object Model
 Home-page: https://pypi.org/project/pomcorn/
 License: MIT
 Keywords: python,selenium,webdriver,autotests,page object model,page object pattern,page object,pom,parsing,browser
 Author: Saritasa
 Author-email: pypi@saritasa.com
 Maintainer: Anton Oboleninov
```

