# Comparing `tmp/libs_zip-0.0.2-py3-none-any.whl.zip` & `tmp/libs_zip-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 2361 bytes, number of entries: 7
+Zip file size: 4331 bytes, number of entries: 10
+-rw-------  2.0 unx      150 b- defN 24-Apr-17 03:56 libs/__init__.py
+-rw-------  2.0 unx      955 b- defN 24-Apr-17 03:56 libs/data.py
+-rw-------  2.0 unx     1701 b- defN 24-Apr-17 03:56 libs/image.py
 -rw-------  2.0 unx       31 b- defN 24-Apr-16 06:04 libs/test.py
--rw-------  2.0 unx      210 b- defN 24-Apr-16 06:43 libs/web.py
--rw-------  2.0 unx     1067 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/LICENSE
--rw-------  2.0 unx      192 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/WHEEL
--rw-------  2.0 unx        5 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      523 b- defN 24-Apr-16 07:13 libs_zip-0.0.2.dist-info/RECORD
-7 files, 2120 bytes uncompressed, 1433 bytes compressed:  32.4%
+-rw-------  2.0 unx      440 b- defN 24-Apr-17 03:56 libs/web.py
+-rw-------  2.0 unx     1067 b- defN 24-Apr-17 03:58 libs_zip-0.0.3.dist-info/LICENSE
+-rw-------  2.0 unx      332 b- defN 24-Apr-17 03:58 libs_zip-0.0.3.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 24-Apr-17 03:58 libs_zip-0.0.3.dist-info/WHEEL
+-rw-------  2.0 unx        5 b- defN 24-Apr-17 03:58 libs_zip-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      733 b- defN 24-Apr-17 03:58 libs_zip-0.0.3.dist-info/RECORD
+10 files, 5506 bytes uncompressed, 3093 bytes compressed:  43.8%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
+Filename: libs/__init__.py
+Comment: 
+
+Filename: libs/data.py
+Comment: 
+
+Filename: libs/image.py
+Comment: 
+
 Filename: libs/test.py
 Comment: 
 
 Filename: libs/web.py
 Comment: 
 
-Filename: libs_zip-0.0.2.dist-info/LICENSE
+Filename: libs_zip-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: libs_zip-0.0.2.dist-info/METADATA
+Filename: libs_zip-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: libs_zip-0.0.2.dist-info/WHEEL
+Filename: libs_zip-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: libs_zip-0.0.2.dist-info/top_level.txt
+Filename: libs_zip-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: libs_zip-0.0.2.dist-info/RECORD
+Filename: libs_zip-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libs/web.py

```diff
@@ -1,7 +1,19 @@
 import requests
+from selenium import webdriver
 from bs4 import BeautifulSoup
 
+
 def crawl_website(url):
     # 주어진 URL의 웹 페이지를 크롤링하여 HTML 내용을 반환
     response = requests.get(url)
-    return response.content
+    html_content = response.content
+
+    # HTML 문서 파싱
+    soup = BeautifulSoup(html_content, 'html.parser')
+    return soup
+
+def open_url(url):
+    browser = webdriver.Chrome()
+    browser.get(url)
+
+    return browser
```

## Comparing `libs_zip-0.0.2.dist-info/LICENSE` & `libs_zip-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

