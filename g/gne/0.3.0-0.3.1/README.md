# Comparing `tmp/gne-0.3.0.tar.gz` & `tmp/gne-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gne-0.3.0.tar", last modified: Thu Oct  7 07:01:28 2021, max compression
+gzip compressed data, was "gne-0.3.1.tar", last modified: Wed Apr 17 14:45:33 2024, max compression
```

## Comparing `gne-0.3.0.tar` & `gne-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 kingname   (501) staff       (20)        0 2021-10-07 07:01:28.948066 gne-0.3.0/
--rw-r--r--   0 kingname   (501) staff       (20)     4979 2021-10-07 06:14:18.000000 gne-0.3.0/CHANGELOG.md
--rw-r--r--   0 kingname   (501) staff       (20)      107 2019-12-31 15:04:16.000000 gne-0.3.0/MANIFEST.in
--rw-r--r--   0 kingname   (501) staff       (20)     1728 2021-10-07 07:01:28.949495 gne-0.3.0/PKG-INFO
--rw-r--r--   0 kingname   (501) staff       (20)     8701 2021-10-07 06:39:43.000000 gne-0.3.0/README.md
-drwxr-xr-x   0 kingname   (501) staff       (20)        0 2021-10-07 07:01:28.918562 gne-0.3.0/gne/
--rw-r--r--   0 kingname   (501) staff       (20)     2201 2021-10-07 02:36:16.000000 gne-0.3.0/gne/__init__.py
--rw-r--r--   0 kingname   (501) staff       (20)     5624 2020-10-06 14:55:19.000000 gne-0.3.0/gne/defaults.py
-drwxr-xr-x   0 kingname   (501) staff       (20)        0 2021-10-07 07:01:28.945420 gne-0.3.0/gne/extractor/
--rw-r--r--   0 kingname   (501) staff       (20)      691 2020-02-13 15:03:08.000000 gne-0.3.0/gne/extractor/AuthorExtractor.py
--rw-r--r--   0 kingname   (501) staff       (20)     8200 2021-10-07 06:39:43.000000 gne-0.3.0/gne/extractor/ContentExtractor.py
--rw-r--r--   0 kingname   (501) staff       (20)     1406 2020-08-02 08:47:26.000000 gne-0.3.0/gne/extractor/ListExtractor.py
--rw-r--r--   0 kingname   (501) staff       (20)     1756 2020-02-21 13:42:44.000000 gne-0.3.0/gne/extractor/TimeExtractor.py
--rw-r--r--   0 kingname   (501) staff       (20)     2665 2021-10-04 01:18:12.000000 gne-0.3.0/gne/extractor/TitleExtractor.py
--rw-r--r--   0 kingname   (501) staff       (20)      216 2020-07-26 14:09:21.000000 gne-0.3.0/gne/extractor/__init__.py
--rw-r--r--   0 kingname   (501) staff       (20)     5033 2021-10-04 01:18:12.000000 gne-0.3.0/gne/utils.py
-drwxr-xr-x   0 kingname   (501) staff       (20)        0 2021-10-07 07:01:28.932970 gne-0.3.0/gne.egg-info/
--rw-r--r--   0 kingname   (501) staff       (20)     1728 2021-10-07 07:01:28.000000 gne-0.3.0/gne.egg-info/PKG-INFO
--rw-r--r--   0 kingname   (501) staff       (20)      432 2021-10-07 07:01:28.000000 gne-0.3.0/gne.egg-info/SOURCES.txt
--rw-r--r--   0 kingname   (501) staff       (20)        1 2021-10-07 07:01:28.000000 gne-0.3.0/gne.egg-info/dependency_links.txt
--rw-r--r--   0 kingname   (501) staff       (20)       18 2021-10-07 07:01:28.000000 gne-0.3.0/gne.egg-info/requires.txt
--rw-r--r--   0 kingname   (501) staff       (20)        4 2021-10-07 07:01:28.000000 gne-0.3.0/gne.egg-info/top_level.txt
--rw-r--r--   0 kingname   (501) staff       (20)      950 2019-12-31 16:25:21.000000 gne-0.3.0/pypi_desc.md
--rw-r--r--   0 kingname   (501) staff       (20)       84 2021-10-07 07:01:28.954267 gne-0.3.0/setup.cfg
--rw-r--r--   0 kingname   (501) staff       (20)      834 2021-10-07 06:11:08.000000 gne-0.3.0/setup.py
+drwxr-xr-x   0 kingname   (501) staff       (20)        0 2024-04-17 14:45:33.897374 gne-0.3.1/
+-rw-r--r--   0 kingname   (501) staff       (20)     5180 2024-04-17 14:41:41.000000 gne-0.3.1/CHANGELOG.md
+-rw-r--r--   0 kingname   (501) staff       (20)    35149 2022-08-23 15:52:24.000000 gne-0.3.1/LICENSE
+-rw-r--r--   0 kingname   (501) staff       (20)      107 2022-08-23 15:52:24.000000 gne-0.3.1/MANIFEST.in
+-rw-r--r--   0 kingname   (501) staff       (20)     1593 2024-04-17 14:45:33.897468 gne-0.3.1/PKG-INFO
+-rw-r--r--   0 kingname   (501) staff       (20)     8910 2023-09-03 02:33:47.000000 gne-0.3.1/README.md
+drwxr-xr-x   0 kingname   (501) staff       (20)        0 2024-04-17 14:45:33.894397 gne-0.3.1/gne/
+-rw-r--r--   0 kingname   (501) staff       (20)     2633 2024-04-17 14:39:53.000000 gne-0.3.1/gne/__init__.py
+-rw-r--r--   0 kingname   (501) staff       (20)     5818 2024-04-17 14:22:58.000000 gne-0.3.1/gne/defaults.py
+-rw-r--r--   0 kingname   (501) staff       (20)       45 2022-09-22 14:53:09.000000 gne-0.3.1/gne/exceptions.py
+drwxr-xr-x   0 kingname   (501) staff       (20)        0 2024-04-17 14:45:33.897157 gne-0.3.1/gne/extractor/
+-rw-r--r--   0 kingname   (501) staff       (20)      691 2022-08-23 15:52:24.000000 gne-0.3.1/gne/extractor/AuthorExtractor.py
+-rw-r--r--   0 kingname   (501) staff       (20)     8201 2022-09-12 08:39:47.000000 gne-0.3.1/gne/extractor/ContentExtractor.py
+-rw-r--r--   0 kingname   (501) staff       (20)     1406 2022-08-23 15:52:24.000000 gne-0.3.1/gne/extractor/ListExtractor.py
+-rw-r--r--   0 kingname   (501) staff       (20)      871 2022-09-18 14:00:12.000000 gne-0.3.1/gne/extractor/MetaExtractor.py
+-rw-r--r--   0 kingname   (501) staff       (20)     1756 2022-08-23 15:52:24.000000 gne-0.3.1/gne/extractor/TimeExtractor.py
+-rw-r--r--   0 kingname   (501) staff       (20)     2665 2022-08-23 15:52:24.000000 gne-0.3.1/gne/extractor/TitleExtractor.py
+-rw-r--r--   0 kingname   (501) staff       (20)      258 2022-09-18 14:00:12.000000 gne-0.3.1/gne/extractor/__init__.py
+-rw-r--r--   0 kingname   (501) staff       (20)     5394 2024-04-17 14:38:09.000000 gne-0.3.1/gne/utils.py
+drwxr-xr-x   0 kingname   (501) staff       (20)        0 2024-04-17 14:45:33.895280 gne-0.3.1/gne.egg-info/
+-rw-r--r--   0 kingname   (501) staff       (20)     1593 2024-04-17 14:45:33.000000 gne-0.3.1/gne.egg-info/PKG-INFO
+-rw-r--r--   0 kingname   (501) staff       (20)      489 2024-04-17 14:45:33.000000 gne-0.3.1/gne.egg-info/SOURCES.txt
+-rw-r--r--   0 kingname   (501) staff       (20)        1 2024-04-17 14:45:33.000000 gne-0.3.1/gne.egg-info/dependency_links.txt
+-rw-r--r--   0 kingname   (501) staff       (20)       18 2024-04-17 14:45:33.000000 gne-0.3.1/gne.egg-info/requires.txt
+-rw-r--r--   0 kingname   (501) staff       (20)        4 2024-04-17 14:45:33.000000 gne-0.3.1/gne.egg-info/top_level.txt
+-rw-r--r--   0 kingname   (501) staff       (20)      845 2023-09-03 02:33:47.000000 gne-0.3.1/pypi_desc.md
+-rw-r--r--   0 kingname   (501) staff       (20)       84 2024-04-17 14:45:33.897713 gne-0.3.1/setup.cfg
+-rw-r--r--   0 kingname   (501) staff       (20)     1729 2023-09-03 02:33:47.000000 gne-0.3.1/setup.py
```

### Comparing `gne-0.3.0/CHANGELOG.md` & `gne-0.3.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # General News Extractor Changelog
 
+## 0.3.1 (2024-04-17)
+
+### Bug fix
+
+有一些网站源代码不规范，在html中间突然出现</html>。末尾又出现一次</html>.这种情况下，会导致解析出错。现在已经修复。
+
 ## 0.3.0 (2021-10-07)
 
 ### New Feature
 
 1. 基于可视化区域，更准确地识别正文
 
 ### Bug fix
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
-# General News Extractor Changelog ## 0.3.0 (2021-10-07) ### New Feature 1.
+# General News Extractor Changelog ## 0.3.1 (2024-04-17) ### Bug fix
+æä¸äºç½ç«æºä»£ç ä¸è§èï¼å¨htmlä¸­é´çªç¶åºç°
+ãæ«å°¾ååºç°ä¸æ¬¡
+.è¿ç§æåµä¸ï¼ä¼å¯¼è´è§£æåºéãç°å¨å·²ç»ä¿®å¤ã ## 0.3.0
+(2021-10-07) ### New Feature 1.
 åºäºå¯è§ååºåï¼æ´åç¡®å°è¯å«æ­£æ ### Bug fix *
 ä¿®å¤ä¸é¢è¿ç§æåµæ¶ï¼æ æ³æ­£ç¡®å¯»æ¾æ­£æç bug ```html
 ææ¯æ­£æææ¯æ­£æææ¯æ­£æ_å__³_é__®_è_¯__1ææ¯æ­£æææ¯æ­£æææ¯æ­£æææ¯æ­£æ
 ææ¯æ­£æææ¯æ­£æææ¯æ­£æææ¯æ­£æææ¯æ­£æ_å__³_é__®_è_¯__2ææ¯æ­£æææ¯æ­£æ
 ææ¯æ­£æ
 ``` * ç»è®¡ä¸ä¸ªæ ç­¾ä¸é¢ç p
 æ ç­¾çæ¶åï¼åºè¯¥æè¿ä¸ªæ ç­¾ä¸é¢çç´æ¥ææ¡£æ°ä¹ç»è®¡è¿å»
```

### Comparing `gne-0.3.0/README.md` & `gne-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # GNE
 
 ![](https://github.com/GeneralNewsExtractor/GeneralNewsExtractor/raw/master/screenshots/logo.png)
 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=GeneralNewsExtractor/GeneralNewsExtractor&type=Date)](https://star-history.com/#GeneralNewsExtractor/GeneralNewsExtractor&Date)
+
+
 ## 项目起源
 
 开发这个项目，源自于我在知网发现了一篇关于自动化抽取新闻类网站正文的算法论文——[《基于文本及符号密度的网页正文提取方法》](https://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFDLAST2019&filename=GWDZ201908029&v=MDY4MTRxVHJXTTFGckNVUkxPZmJ1Wm5GQ2poVXJyQklqclBkTEc0SDlqTXA0OUhiWVI4ZVgxTHV4WVM3RGgxVDM=)）
 
 这篇论文中描述的算法看起来简洁清晰，并且符合逻辑。但由于论文中只讲了算法原理，并没有具体的语言实现，所以我使用 Python 根据论文实现了这个抽取器。并分别使用今日头条、网易新闻、游民星空、观察者网、凤凰网、腾讯新闻、ReadHub、新浪新闻做了测试，发现提取效果非常出色，几乎能够达到100%的准确率。
 
 ## 项目现状
```

### Comparing `gne-0.3.0/gne/__init__.py` & `gne-0.3.1/gne/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,62 @@
-from .utils import pre_parse, remove_noise_node, config, html2element, normalize_text
-from gne.extractor import ContentExtractor, TitleExtractor, TimeExtractor, AuthorExtractor, ListExtractor
+from .exceptions import NoContentException
+from .utils import pre_parse, remove_noise_node, config, html2element, normalize_text, fix_html
+from gne.extractor import ContentExtractor, TitleExtractor, TimeExtractor, AuthorExtractor, ListExtractor, MetaExtractor
+
+__version__ = "0.3.1"
+__author__ = "Kingname"
 
 
 class GeneralNewsExtractor:
     def extract(self,
                 html,
                 title_xpath='',
                 author_xpath='',
                 publish_time_xpath='',
                 host='',
                 body_xpath='',
+                normalize=False,
                 noise_node_list=None,
                 with_body_html=False,
                 use_visiable_info=False):
 
         # 对 HTML 进行预处理可能会破坏 HTML 原有的结构，导致根据原始 HTML 编写的 XPath 不可用
         # 因此，如果指定了 title_xpath/author_xpath/publish_time_xpath，那么需要先提取再进行
         # 预处理
-        normal_html = normalize_text(html)
+        html = fix_html(html)
+        if normalize:
+            normal_html = normalize_text(html)
+        else:
+            normal_html = html
         element = html2element(normal_html)
+        meta_content = MetaExtractor().extract(element)
         title = TitleExtractor().extract(element, title_xpath=title_xpath)
         publish_time = TimeExtractor().extractor(element, publish_time_xpath=publish_time_xpath)
         author = AuthorExtractor().extractor(element, author_xpath=author_xpath)
         element = pre_parse(element)
         remove_noise_node(element, noise_node_list)
         content = ContentExtractor().extract(element,
                                              host=host,
                                              with_body_html=with_body_html,
                                              body_xpath=body_xpath,
                                              use_visiable_info=use_visiable_info)
+        if not content:
+            raise NoContentException('无法提取正文！')
         result = {'title': title,
                   'author': author,
                   'publish_time': publish_time,
                   'content': content[0][1]['text'],
-                  'images': content[0][1]['images']
+                  'images': content[0][1]['images'],
+                  'meta': meta_content
                   }
         if with_body_html or config.get('with_body_html', False):
             result['body_html'] = content[0][1]['body_html']
         return result
 
 
 class ListPageExtractor:
     def extract(self, html, feature):
         normalize_html = normalize_text(html)
         element = html2element(normalize_html)
         extractor = ListExtractor()
         return extractor.extract(element, feature)
+
```

### Comparing `gne-0.3.0/gne/defaults.py` & `gne-0.3.1/gne/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,23 @@
                 'disclaimer',
                 'recommend',
                 'related',
                 'footer',
                 'comment',
                 'social',
                 'submeta',
-                'report-infor'
+                'report-infor',
+                'header_toolbar'
                 }
 
 
 HIGH_WEIGHT_ARRT_KEYWORD = ['content',
                             'article',
                             'news_txt',
+                            'pages_content',
                             'post_text']
 
 
 PUBLISH_TIME_META = [  # 部分特别规范的新闻网站，可以直接从 HTML 的 meta 数据中获得发布时间
     '//meta[starts-with(@property, "rnews:datePublished")]/@content',
     '//meta[starts-with(@property, "article:published_time")]/@content',
     '//meta[starts-with(@property, "og:published_time")]/@content',
@@ -97,7 +99,12 @@
     '//meta[starts-with(@name, "publishdate")]/@content',
     '//meta[starts-with(@name, "PubDate")]/@content',
     '//meta[starts-with(@name, "pubtime")]/@content',
     '//meta[starts-with(@name, "_pubtime")]/@content',
     '//meta[starts-with(@name, "weibo: article:create_at")]/@content',
     '//meta[starts-with(@pubdate, "pubdate")]/@content',
 ]
+
+# 满足下面的XPath，极有可能是文章详情页
+ARTICLE_XPATH = [
+    '//*[@class="article__content"]',
+]
```

### Comparing `gne-0.3.0/gne/extractor/AuthorExtractor.py` & `gne-0.3.1/gne/extractor/AuthorExtractor.py`

 * *Files identical despite different names*

### Comparing `gne-0.3.0/gne/extractor/ContentExtractor.py` & `gne-0.3.1/gne/extractor/ContentExtractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             body = selector.xpath('//body')[0]
         for node in iter_node(body):
             if use_visiable_info:
                 if not node.attrib.get('is_visiable', True):
                     continue
                 coordinate_json = node.attrib.get('coordinate', '{}')
                 coordinate = json.loads(coordinate_json)
+
                 if coordinate.get('height', 0) < 150:  # 正文块的高度应该要大于150px
                     continue
             node_hash = hash(node)
             density_info = self.calc_text_density(node)
             text_density = density_info['density']
             ti_text = density_info['ti_text']
             text_tag_count = self.count_text_tag(node, tag='p')
```

### Comparing `gne-0.3.0/gne/extractor/ListExtractor.py` & `gne-0.3.1/gne/extractor/ListExtractor.py`

 * *Files identical despite different names*

### Comparing `gne-0.3.0/gne/extractor/TimeExtractor.py` & `gne-0.3.1/gne/extractor/TimeExtractor.py`

 * *Files identical despite different names*

### Comparing `gne-0.3.0/gne/extractor/TitleExtractor.py` & `gne-0.3.1/gne/extractor/TitleExtractor.py`

 * *Files identical despite different names*

### Comparing `gne-0.3.0/gne/utils.py` & `gne-0.3.1/gne/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -169,14 +169,26 @@
                 matrix[index_of_str1][index_of_str2] = 0
     return str1[start_position: start_position + max_length]
 
 
 def normalize_text(html):
     """
     使用 NFKC 对网页源代码进行归一化，把特殊符号转换为普通符号
+    注意，中文标点符号可能会被转换成英文标点符合。
     :param html:
     :return:
     """
     return unicodedata.normalize('NFKC', html)
 
 
+def fix_html(html):
+    """
+    有一些网站的HTML不规范，比如</html>出现在源代码的中间。这个时候需要修复一下。
+    :param html:
+    :return: html
+    """
+    new_html = html.replace('</html>', '')
+    new_html = f'{new_html}</html>'
+    return new_html
+
+
 config = read_config()
```

### Comparing `gne-0.3.0/pypi_desc.md` & `gne-0.3.1/pypi_desc.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # GNE: 通用新闻网站正文抽取器
 
 GeneralNewsExtractor（GNE）是一个通用新闻网站正文抽取模块，输入一篇新闻网页的 HTML， 输出正文内容、标题、作者、发布时间、正文中的图片地址和正文所在的标签源代码。GNE在提取今日头条、网易新闻、游民星空、 观察者网、凤凰网、腾讯新闻、ReadHub、新浪新闻等数百个中文新闻网站上效果非常出色，几乎能够达到100%的准确率。
 
 使用方式也非常简单：
 
 ```python
-
 from gne import GeneralNewsExtractor
 
 extractor = GeneralNewsExtractor()
 html = '网站源代码'
 result = extractor.extract(html)
 print(result)
 ```
 
 ## 安装
 
-```bash
+```
 pip install gne
 ```
 
 ## 文档
 
-[https://generalnewsextractor.readthedocs.io/](https://generalnewsextractor.readthedocs.io/)
+https://generalnewsextractor.readthedocs.io/
 
 ## 帮助 GNE 变得更好
 
-[https://github.com/kingname/GeneralNewsExtractor](https://github.com/kingname/GeneralNewsExtractor)
+https://github.com/kingname/GeneralNewsExtractor
```

