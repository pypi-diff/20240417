# Comparing `tmp/scrapework-0.4.5.tar.gz` & `tmp/scrapework-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapework-0.4.5.tar", max compression
+gzip compressed data, was "scrapework-0.4.6.tar", max compression
```

## Comparing `scrapework-0.4.5.tar` & `scrapework-0.4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3557 2024-03-29 03:31:11.424327 scrapework-0.4.5/README.md
--rw-r--r--   0        0        0      857 2024-03-29 03:31:23.120306 scrapework-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/__init__.py
--rw-r--r--   0        0        0     2265 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/cache.py
--rw-r--r--   0        0        0        0 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/core/__init__.py
--rw-r--r--   0        0        0      506 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/core/collector.py
--rw-r--r--   0        0        0      567 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/core/context.py
--rw-r--r--   0        0        0      424 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/core/http_client.py
--rw-r--r--   0        0        0      873 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/core/logger.py
--rw-r--r--   0        0        0     2252 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/handlers.py
--rw-r--r--   0        0        0     3729 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/items.py
--rw-r--r--   0        0        0     2810 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/middleware.py
--rw-r--r--   0        0        0      221 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/module.py
--rw-r--r--   0        0        0      194 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/monitors.py
--rw-r--r--   0        0        0      862 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/observer.py
--rw-r--r--   0        0        0      697 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/parsers.py
--rw-r--r--   0        0        0      546 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/processors.py
--rw-r--r--   0        0        0     3258 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/reporter.py
--rw-r--r--   0        0        0     2854 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/request.py
--rw-r--r--   0        0        0     5366 2024-03-29 03:31:11.424327 scrapework-0.4.5/scrapework/scraper.py
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 scrapework-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     4032 2024-04-17 02:34:41.441785 scrapework-0.4.6/README.md
+-rw-r--r--   0        0        0      866 2024-04-17 02:34:53.361707 scrapework-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/cache.py
+-rw-r--r--   0        0        0        0 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/collector.py
+-rw-r--r--   0        0        0      567 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/context.py
+-rw-r--r--   0        0        0      424 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/http_client.py
+-rw-r--r--   0        0        0      873 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/logger.py
+-rw-r--r--   0        0        0     2435 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/handlers.py
+-rw-r--r--   0        0        0     3729 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/items.py
+-rw-r--r--   0        0        0     2810 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/middleware.py
+-rw-r--r--   0        0        0      221 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/module.py
+-rw-r--r--   0        0        0      194 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/monitors.py
+-rw-r--r--   0        0        0      862 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/observer.py
+-rw-r--r--   0        0        0      979 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/parsers.py
+-rw-r--r--   0        0        0      546 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/processors.py
+-rw-r--r--   0        0        0     3258 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/reporter.py
+-rw-r--r--   0        0        0     2854 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/request.py
+-rw-r--r--   0        0        0     5730 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/scraper.py
+-rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 scrapework-0.4.6/PKG-INFO
```

### Comparing `scrapework-0.4.5/README.md` & `scrapework-0.4.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,130 @@
 # Scrapework
 
-Scrapework is a simple and opiniatated scraping framework inspired by Scrapy. It's designed for simple tasks and easy management, allowing you to focus on the scraping logic and not on the boilerplate code.
+Scrapework is a simple and opiniatated framework to extract data from the web. It is inspired by Scrapy and designed for simple tasks and easy management, allowing you to focus on the scraping logic. It is built on top of `parsel` (used by Scrapy) and `httpx` libraries. Some of the key differences are:
 
 - No CLI
 - No twisted framework
 - Designed for in-process usage
 
-## Getting Started
-
-### Installation
+## Installation
 
 First, clone the repository or install as a dependencies:
 
+With pip:
+
 ```sh
-poetry add scrapework
+pip install scrapework
 ```
 
-### Quick Start
-
-Flow:
-
-1. **Request Handling**: Use the `make_request` method to fetch web pages from `start_urls` with the help of `middlewares`.
-2. **Data Extraction**: Implement the `extract` method to parse and extract structured data from the fetched pages using `HTMLBodyParser` or other custom logic.
-3. **Data Processing**: Process and handle the structured data using `handlers` defined in the scraper.
-4. **Reporting**: Generate reports of the scraping process using `reporters`.
+With poetry:
 
-For more details see [Design](docs/Design.md).
-
-### Scraper Configuration
+```sh
+poetry add scrapework
+```
 
-- `start_urls`: A list of URLs to start scraping from.
-- request middleware to configure the request handling.
-- parsers: comes with various extractors (plain body, smart extractors, markedown.)
-- handlers: comes with various handlers (log, save to file, save to database.)
-- reporters
+## Quick Start
 
-### Creating a Spider
+### Create a Scraper
 
-A Spider is a class that defines how to navigate a website and extract data. Here's how you can create a Spider:
+First, create a Scraper class to define how extract data and optionally navigate a website. Here's how you can create a simple Scraper:
 
 ```python
-from scrapework.spider import Spider
+from scrapework.scraper import Scraper
 
-class MyScraper(Scraper):
-    start_urls = ['http://quotes.toscrape.com']
+class SimpleScraper(Scraper):
+    name = "simple_scraper"
 
-    def parse(self, response):
-        for quote in response.css('div.quote'):
+    def extract(self, ctx, selector):
+        for quote in selector.css('div.quote'):
             yield {
                 'text': quote.css('span.text::text').get(),
                 'author': quote.css('span small::text').get(),
             }
+
+    def process(self, items, config):
+        for item in items:
+            print(f"Quote: {item['text']}, Author: {item['author']}")
+```
+
+Similar to Scrapy `parse`, the `extract` method is an expected and this is where you define your scraping logic. It's called with the HTTP response of the initial URL.
+
+### Run the Scraper
+
+To run the Scraper, you need to create an instance and call the `run` method passing the URLs to scrape:
+
+```python
+scraper = SimpleScraper()
+scraper.run(['http://quotes.toscrape.com'])
 ```
 
-The `parse` method is where you define your scraping logic. It's called with the HTTP response of the initial URL.
+### Modules Configuration
+
+Scrapework can be extended using various modules:
+
+- `middleware` to configure the request handling (chache, proxy, ...).
+- `handlers`: comes with various handlers (log, save to file, save to database.)
+- `reporters`: to export and log the scraping events and metadata.
+
+## Flow
+
+The scraping flow consists of the following steps:
+
+1. **Webpage downloading**: Fetch the webpages using `httpx`. Optionally, use `middleware` to handle requests.
+2. **Extract data**: Extract structured data from the HTML using `parsers`.
+3. **Export data**: Use `handlers` to store or export the structured data.
+4. **Reporting**: Generate reports and logs of the scraping process using `reporters`.
+
+For more details see [Design](docs/Design.md).
+
+## Advanced Usage
+
+For more advanced usage, you can override other methods in the Scraper, Parser, and Pipeline classes. Check the source code for more details.
 
-### Creating an Extractor
+### Add Parser
 
-An Extractor is a class that defines how to extract data from a webpage. Here's how you can create an Extractor:
+Alternatively, you can create a Parser class to define how to extract data from a webpage. Here's how you can create an Parser and configure it in the Scraper:
 
 ```python
-from scrapework.extractors import Extractor
+from scrapework.parsers import Parser, Scraper
+
+class SimpleScraper(Scraper):
+    name = "simple_scraper"
+    parser = SimpleParser()
 
-class MyExtractor(Extractor):
-    def extract(self, selector):
+class SimpleParser(Parser):
+    def extract(self, ctx, selector):
         return {
             'text': selector.css('span.text::text').get(),
             'author': selector.css('span small::text').get(),
         }
 ```
 
-The `extract` method is where you define your extraction logic. It's called with a `parsel.Selector` object that you can use to extract data from the HTML.
+The `extract` method is where you define your extraction logic. It's called passing a `parsel.Selector` object that you can use to extract data from the HTML using `css` or `xpath`.
 
-### Creating a Pipeline
+### Add a data handler
 
-A Pipeline is a class that defines how to process and store the data. Here's how you can create a Pipeline:
+Similar to a pipeline, an `handler` defines how to process and store the data:
 
 ```python
-from scrapework.pipelines import ItemPipeline
+from scrapework.handlers import Handler
 
-class MyPipeline(ItemPipeline):
+class SimpleHandler(Handler):
     def process_items(self, items, config):
         for item in items:
             print(f"Quote: {item['text']}, Author: {item['author']}")
 ```
 
-The `process_items` method is where you define your processing logic. It's called with the items extracted by the Extractor and a `PipelineConfig` object.
-
-### Running the Spider
-
-To run the Spider, you need to create an instance of it and call the `start_requests` method:
+The `process_items` method is where you define your processing logic. It's called with the items extracted by the Parser and a `PipelineConfig` object.
 
 ```python
-spider = MySpider()
-spider.start_requests()
-```
-
-## Advanced Usage
+scraper = SimpleScraper()
 
-For more advanced usage, you can override other methods in the Spider, Extractor, and Pipeline classes. Check the source code for more details.
+scraper.use(SimpleHandler())
+```
 
 ## Testing
 
 To run the tests, use the following command:
 
 ```sh
 pytest tests/
```

### Comparing `scrapework-0.4.5/pyproject.toml` & `scrapework-0.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapework"
-version = "v0.4.5"
+version = "v0.4.6"
 description = "simple scraping framework"
 authors = ["Stéphane Busso <stephane.busso@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sbusso/scrapework"
 homepage = "https://github.com/sbusso/scrapework"
 
@@ -14,15 +14,15 @@
 python-dotenv = "^1.0.1"
 boto3 = "^1.34.68"
 pydantic = "^2.6.4"
 parsel = "^1.9.0"
 courlan = "^1.0.0"
 trafilatura = "^1.8.0"
 httpx = "^0.27.0"
-hishel = "^0.0.24"
+hishel = ">=0.0.24,<0.0.27"
 rich = "^13.7.1"
 fake-useragent = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
 ruff = "^0.3.4"
```

### Comparing `scrapework-0.4.5/scrapework/cache.py` & `scrapework-0.4.6/scrapework/cache.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/core/context.py` & `scrapework-0.4.6/scrapework/core/context.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/core/logger.py` & `scrapework-0.4.6/scrapework/core/logger.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/handlers.py` & `scrapework-0.4.6/scrapework/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import json
 import logging
 from abc import abstractmethod
 from dataclasses import asdict, is_dataclass
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Iterable, Union
 
 import boto3
 from pydantic import BaseModel, Field
 
 from scrapework.core.context import Context
 from scrapework.module import Module
 
 
 class Handler(Module):
+    """Handler Processes and handles the structured data
+
+    Processes and handls the structured data, such as saving it to a file or uploading it to a cloud storage service.
+    """
+
     logger: logging.Logger
 
     @abstractmethod
     def process_items(
         self,
         ctx: Context,
-        items: Union[Dict[str, Any], List[Dict[str, Any]]],
+        items: Union[Dict[str, Any], Iterable[Dict[str, Any]]],
     ):
         pass
 
 
 def encode_items(items: Union[Dict[str, Any], Iterable[Dict[str, Any]]]):
     if isinstance(items, BaseModel):
         items = items.model_dump()
```

### Comparing `scrapework-0.4.5/scrapework/items.py` & `scrapework-0.4.6/scrapework/items.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/middleware.py` & `scrapework-0.4.6/scrapework/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/observer.py` & `scrapework-0.4.6/scrapework/observer.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/parsers.py` & `scrapework-0.4.6/scrapework/parsers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from typing import Any, Dict, Iterable, Union
 
+from parsel import Selector
 from trafilatura import bare_extraction
 
+from scrapework.core.context import Context
+
 
 class Parser:
-    def extract(self, selector) -> Union[Dict[str, Any], Iterable[Dict[str, Any]]]:
+    def extract(
+        self, ctx: Context, selector: Selector
+    ) -> Union[Dict[str, Any], Iterable[Dict[str, Any]]]:
         raise NotImplementedError
 
 
+class EmptyParser(Parser):
+    def extract(self, _ctx: Context, _selector: Selector) -> Dict[str, str]:
+        return {}
+
+
 class HTMLBodyParser(Parser):
-    def extract(self, selector) -> Dict[str, str]:
+    def extract(self, _: Context, selector: Selector) -> Dict[str, str]:
         body = selector.xpath("//body/text()").get()
 
         if not body:
             raise ValueError("Body not found")
 
         return {"body": body}
 
 
 class ArticleParser(Parser):
-    def extract(self, selector) -> Dict[str, str]:
+    def extract(self, _ctx: Context, selector: Selector) -> Dict[str, str]:
         article = bare_extraction(selector)
 
         if not article:
             raise ValueError("Article not found")
 
         return {"text": article.text}
```

### Comparing `scrapework-0.4.5/scrapework/processors.py` & `scrapework-0.4.6/scrapework/processors.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/reporter.py` & `scrapework-0.4.6/scrapework/reporter.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/request.py` & `scrapework-0.4.6/scrapework/request.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.5/scrapework/scraper.py` & `scrapework-0.4.6/scrapework/scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import datetime
-from abc import ABC, abstractmethod
+from abc import ABC
 from dataclasses import dataclass
 from typing import Any, Callable, ClassVar, Dict, Iterable, List, Optional, Union
 
 from httpx import Response
 from parsel import Selector
 
 from scrapework.core.collector import JobCollector, MetadataCollector
 from scrapework.core.context import Context
 from scrapework.core.logger import Logger
 from scrapework.handlers import Handler
 from scrapework.middleware import RequestMiddleware
 from scrapework.module import Module
-from scrapework.parsers import HTMLBodyParser
+from scrapework.parsers import Parser
 from scrapework.reporter import LoggerReporter, Reporter
 from scrapework.request import Request
 
 
 # Class to handle url associated with a parser callback, using the default parser if none is provided
 @dataclass
 class ExtractCallback:
@@ -35,17 +35,20 @@
     urls_to_visit: List[ExtractCallback] = []
     base_url: str = ""
     filename: str = ""
     callback: Optional[
         Callable[[Context, Response], Union[Dict[str, Any], Iterable[Dict[str, Any]]]]
     ] = None
 
+    parser: Parser = Parser()
+
     handlers: List[Handler] = []
     middlewares: List[RequestMiddleware] = []
     reporters: List[Reporter] = []
+
     modules: List[Module] = [LoggerReporter()]
 
     def __init__(self, **args):
 
         if not self.__class__.name:
             raise ValueError("Subclass must provide a name attribute")
 
@@ -60,47 +63,48 @@
         return []
 
     def configuration(self) -> None:
 
         for module in [*self.modules, *self.use_modules()]:
             self.use(module)
 
-    def use(self, module: Module) -> None:
+    def variables(self):
+        return {
+            "name": self.name,
+        }
+
+    def use(self, module: Module | List[Module]) -> None:
+        if isinstance(module, list):
+            for m in module:
+                self.use(m)
         match module:
             case RequestMiddleware():
                 self.middlewares.append(module)
             case Handler():
                 self.handlers.append(module)
             case Reporter():
                 self.reporters.append(module)
 
     def build_start_urls(self, input) -> List[str]:
         return []
 
-    @abstractmethod
     def extract(
         self, ctx: Context, selector: Selector
     ) -> Union[Dict[str, Any], Iterable[Dict[str, Any]]]:
-        HTMLBodyParser().extract(selector)
+        return self.parser.extract(ctx, selector)
 
-    def variables(self):
-        return {
-            "name": self.name,
-        }
-
-    def to_visit(
-        self, url: str, extract: Optional[Callable] = None, force=False
-    ) -> None:
-        if url in self.visited_urls and not force:
-            return
-
-        if not extract:
-            extract = self.extract
+    def process(
+        self, ctx: Context, items: Union[Dict[str, Any], Iterable[Dict[str, Any]]]
+    ):
+        for handler in self.handlers:
+            handler.process_items(ctx, items)
 
-        self.urls_to_visit.append(ExtractCallback(url, extract))
+    def report(self, ctx: Context):
+        for reporter in self.reporters:
+            reporter.report(ctx)
 
     def run(self, start_urls: Optional[List[str]] = None, input: Optional[Any] = None):
         self.logger.info("Scraping started")
 
         if not start_urls and not input:
             raise ValueError("Either start_urls or input must be provided")
 
@@ -132,38 +136,50 @@
             if response.status_code != 200:
                 raise ValueError(
                     f"Request failed with status code {response.status_code}"
                 )
 
             self.visited_urls.append(url_with_callback.url)
 
-            new_items = list(url_with_callback.extract(ctx, Selector(response.text)))
-            items += new_items
+            new_items = url_with_callback.extract(ctx, Selector(response.text))
+
+            # TODO: self.process(ctx, new_items)
+
+            items += list(new_items)
 
             iter_end_time = datetime.datetime.now()
             items_count = len(items)
             ctx.collector.set("items_count", items_count)
             ctx.collector.jobs.append(
                 JobCollector(
                     url=url_with_callback.url,
                     duration=iter_end_time - iter_begin_time,
-                    items_count=len(new_items),
+                    items_count=len(list(new_items)),
                 )
             )
 
-        for handler in self.handlers:
-            handler.process_items(ctx, items)
+        self.process(ctx, items)
 
         end_time = datetime.datetime.now()
 
         ctx.collector.set("duration", end_time - begin_time)
         self.logger.info("Scraping complete")
 
-        for reporter in self.reporters:
-            reporter.report(ctx)
+        self.report(ctx)
+
+    def to_visit(
+        self, url: str, extract: Optional[Callable] = None, force=False
+    ) -> None:
+        if url in self.visited_urls and not force:
+            return
+
+        if not extract:
+            extract = self.extract
+
+        self.urls_to_visit.append(ExtractCallback(url, extract))
 
     def make_request(self, ctx: Context, url: str) -> Optional[Response]:
         request = Request(url=url, logger=self.logger)
 
         self.logger.info(f"Making request to {url}")
 
         for middleware in self.middlewares:
```

### Comparing `scrapework-0.4.5/PKG-INFO` & `scrapework-0.4.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,157 @@
 Metadata-Version: 2.1
 Name: scrapework
-Version: 0.4.5
+Version: 0.4.6
 Summary: simple scraping framework
 Home-page: https://github.com/sbusso/scrapework
 License: MIT
 Author: Stéphane Busso
 Author-email: stephane.busso@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.68,<2.0.0)
 Requires-Dist: courlan (>=1.0.0,<2.0.0)
 Requires-Dist: fake-useragent (>=1.5.1,<2.0.0)
-Requires-Dist: hishel (>=0.0.24,<0.0.25)
+Requires-Dist: hishel (>=0.0.24,<0.0.27)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: parsel (>=1.9.0,<2.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: trafilatura (>=1.8.0,<2.0.0)
 Project-URL: Repository, https://github.com/sbusso/scrapework
 Description-Content-Type: text/markdown
 
 # Scrapework
 
-Scrapework is a simple and opiniatated scraping framework inspired by Scrapy. It's designed for simple tasks and easy management, allowing you to focus on the scraping logic and not on the boilerplate code.
+Scrapework is a simple and opiniatated framework to extract data from the web. It is inspired by Scrapy and designed for simple tasks and easy management, allowing you to focus on the scraping logic. It is built on top of `parsel` (used by Scrapy) and `httpx` libraries. Some of the key differences are:
 
 - No CLI
 - No twisted framework
 - Designed for in-process usage
 
-## Getting Started
-
-### Installation
+## Installation
 
 First, clone the repository or install as a dependencies:
 
+With pip:
+
 ```sh
-poetry add scrapework
+pip install scrapework
 ```
 
-### Quick Start
-
-Flow:
-
-1. **Request Handling**: Use the `make_request` method to fetch web pages from `start_urls` with the help of `middlewares`.
-2. **Data Extraction**: Implement the `extract` method to parse and extract structured data from the fetched pages using `HTMLBodyParser` or other custom logic.
-3. **Data Processing**: Process and handle the structured data using `handlers` defined in the scraper.
-4. **Reporting**: Generate reports of the scraping process using `reporters`.
+With poetry:
 
-For more details see [Design](docs/Design.md).
-
-### Scraper Configuration
+```sh
+poetry add scrapework
+```
 
-- `start_urls`: A list of URLs to start scraping from.
-- request middleware to configure the request handling.
-- parsers: comes with various extractors (plain body, smart extractors, markedown.)
-- handlers: comes with various handlers (log, save to file, save to database.)
-- reporters
+## Quick Start
 
-### Creating a Spider
+### Create a Scraper
 
-A Spider is a class that defines how to navigate a website and extract data. Here's how you can create a Spider:
+First, create a Scraper class to define how extract data and optionally navigate a website. Here's how you can create a simple Scraper:
 
 ```python
-from scrapework.spider import Spider
+from scrapework.scraper import Scraper
 
-class MyScraper(Scraper):
-    start_urls = ['http://quotes.toscrape.com']
+class SimpleScraper(Scraper):
+    name = "simple_scraper"
 
-    def parse(self, response):
-        for quote in response.css('div.quote'):
+    def extract(self, ctx, selector):
+        for quote in selector.css('div.quote'):
             yield {
                 'text': quote.css('span.text::text').get(),
                 'author': quote.css('span small::text').get(),
             }
+
+    def process(self, items, config):
+        for item in items:
+            print(f"Quote: {item['text']}, Author: {item['author']}")
+```
+
+Similar to Scrapy `parse`, the `extract` method is an expected and this is where you define your scraping logic. It's called with the HTTP response of the initial URL.
+
+### Run the Scraper
+
+To run the Scraper, you need to create an instance and call the `run` method passing the URLs to scrape:
+
+```python
+scraper = SimpleScraper()
+scraper.run(['http://quotes.toscrape.com'])
 ```
 
-The `parse` method is where you define your scraping logic. It's called with the HTTP response of the initial URL.
+### Modules Configuration
+
+Scrapework can be extended using various modules:
+
+- `middleware` to configure the request handling (chache, proxy, ...).
+- `handlers`: comes with various handlers (log, save to file, save to database.)
+- `reporters`: to export and log the scraping events and metadata.
+
+## Flow
+
+The scraping flow consists of the following steps:
+
+1. **Webpage downloading**: Fetch the webpages using `httpx`. Optionally, use `middleware` to handle requests.
+2. **Extract data**: Extract structured data from the HTML using `parsers`.
+3. **Export data**: Use `handlers` to store or export the structured data.
+4. **Reporting**: Generate reports and logs of the scraping process using `reporters`.
+
+For more details see [Design](docs/Design.md).
+
+## Advanced Usage
+
+For more advanced usage, you can override other methods in the Scraper, Parser, and Pipeline classes. Check the source code for more details.
 
-### Creating an Extractor
+### Add Parser
 
-An Extractor is a class that defines how to extract data from a webpage. Here's how you can create an Extractor:
+Alternatively, you can create a Parser class to define how to extract data from a webpage. Here's how you can create an Parser and configure it in the Scraper:
 
 ```python
-from scrapework.extractors import Extractor
+from scrapework.parsers import Parser, Scraper
+
+class SimpleScraper(Scraper):
+    name = "simple_scraper"
+    parser = SimpleParser()
 
-class MyExtractor(Extractor):
-    def extract(self, selector):
+class SimpleParser(Parser):
+    def extract(self, ctx, selector):
         return {
             'text': selector.css('span.text::text').get(),
             'author': selector.css('span small::text').get(),
         }
 ```
 
-The `extract` method is where you define your extraction logic. It's called with a `parsel.Selector` object that you can use to extract data from the HTML.
+The `extract` method is where you define your extraction logic. It's called passing a `parsel.Selector` object that you can use to extract data from the HTML using `css` or `xpath`.
 
-### Creating a Pipeline
+### Add a data handler
 
-A Pipeline is a class that defines how to process and store the data. Here's how you can create a Pipeline:
+Similar to a pipeline, an `handler` defines how to process and store the data:
 
 ```python
-from scrapework.pipelines import ItemPipeline
+from scrapework.handlers import Handler
 
-class MyPipeline(ItemPipeline):
+class SimpleHandler(Handler):
     def process_items(self, items, config):
         for item in items:
             print(f"Quote: {item['text']}, Author: {item['author']}")
 ```
 
-The `process_items` method is where you define your processing logic. It's called with the items extracted by the Extractor and a `PipelineConfig` object.
-
-### Running the Spider
-
-To run the Spider, you need to create an instance of it and call the `start_requests` method:
+The `process_items` method is where you define your processing logic. It's called with the items extracted by the Parser and a `PipelineConfig` object.
 
 ```python
-spider = MySpider()
-spider.start_requests()
-```
-
-## Advanced Usage
+scraper = SimpleScraper()
 
-For more advanced usage, you can override other methods in the Spider, Extractor, and Pipeline classes. Check the source code for more details.
+scraper.use(SimpleHandler())
+```
 
 ## Testing
 
 To run the tests, use the following command:
 
 ```sh
 pytest tests/
```

