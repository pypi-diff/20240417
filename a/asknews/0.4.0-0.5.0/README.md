# Comparing `tmp/asknews-0.4.0-py3-none-any.whl.zip` & `tmp/asknews-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 21865 bytes, number of entries: 24
+Zip file size: 22019 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4442 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      170 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     7443 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
 -rw-r--r--  2.0 unx    11705 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
 -rw-r--r--  2.0 unx    10375 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    15904 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
--rw-r--r--  2.0 unx     1744 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
+-rw-r--r--  2.0 unx     2424 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     3381 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      606 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1284 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      552 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
--rw-r--r--  2.0 unx     4144 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
+-rw-r--r--  2.0 unx     4166 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6302 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5248 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1583 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3185 b- defN 80-Jan-01 00:00 asknews-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.4.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.4.0.dist-info/RECORD
-24 files, 83984 bytes uncompressed, 18831 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3185 b- defN 80-Jan-01 00:00 asknews-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.5.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.5.0.dist-info/RECORD
+24 files, 84686 bytes uncompressed, 18985 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.4.0.dist-info/LICENSE
+Filename: asknews-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.4.0.dist-info/METADATA
+Filename: asknews-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.4.0.dist-info/WHEEL
+Filename: asknews-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.4.0.dist-info/RECORD
+Filename: asknews-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/dto/base.py

```diff
@@ -7,24 +7,49 @@
 from uuid import UUID
 
 
 class BaseSchema(BaseModel):
     __content_type__: ClassVar[str] = "application/json"
 
 
-class Entities(BaseModel):
+class RedditEntities(BaseModel):
     DATE: list[str] = []
     EVENT: list[str] = []
     GPE: list[str] = []
     ORG: list[str] = []
     PERSON: list[str] = []
     NORP: list[str] = []
     CARDINAL: list[str] = []
 
 
+class Entities(BaseModel):
+    Person: list[str] = []
+    Organization: list[str] = []
+    Location: list[str] = []
+    Nationality: list[str] = []
+    Event: list[str] = []
+    Money: list[str] = []
+    Law: list[str] = []
+    Quantity: list[str] = []
+    Time: list[str] = []
+    Sports: list[str] = []
+    Politics: list[str] = []
+    Title: list[str] = []
+    Number: list[str] = []
+    Arms: list[str] = []
+    Product: list[str] = []
+    Media: list[str] = []
+    Transportation: list[str] = []
+    Religion: list[str] = []
+    Technology: list[str] = []
+    Space: list[str] = []
+    Medicine: list[str] = []
+    Language: list[str] = []
+    Science: list[str] = []
+
 class Article(BaseModel):
     article_id: Annotated[UUID, Field(title='Article Id')]
     article_url: Annotated[AnyUrl, Field(title='Article Url')]
     classification: Annotated[list[str], Field(title='Classification')]
     country: Annotated[str, Field(title='Country')]
     source_id: Annotated[str, Field(title='Source Id')]
     page_rank: Annotated[int, Field(title='Page Rank')]
```

## asknews_sdk/dto/stories.py

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Annotated
 from datetime import datetime
 from uuid import UUID
 from pydantic import AnyUrl, BaseModel, Field
 
-from asknews_sdk.dto.base import BaseSchema, Article, Entities
+from asknews_sdk.dto.base import BaseSchema, Article, Entities, RedditEntities
 
 
 class RedditPerspective(BaseModel):
     sentiment: int
     relevant: bool
     summary: str
 
@@ -19,15 +19,15 @@
     author_comment_karma: int
     author_link_karma: int
     body: str
     classification: list[str]
     comments: list[RedditComment]
     comments_count: int
     date: datetime
-    entities: Entities
+    entities: RedditEntities
     id: UUID
     key_takeaways: list[str]
     keywords: list[str]
     sentiment: int
     subreddit_name: str
     subreddit_url: str
     summary: str
```

## Comparing `asknews-0.4.0.dist-info/LICENSE` & `asknews-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.4.0.dist-info/METADATA` & `asknews-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python SDK for AskNews
 Home-page: https://gitlab.com/emergentmethods/asknews/python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.4.0.dist-info/RECORD` & `asknews-0.5.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 asknews_sdk/api/analytics.py,sha256=Pdri83YjVS8JkwqDyCYVIlIa0FqL-brrQ2KJm_SniCY,4442
 asknews_sdk/api/base.py,sha256=Zwg4Cy9FDUt2wywKUmVnZIex7NB9oUrdRR0BM8Yll7A,170
 asknews_sdk/api/chat.py,sha256=3Q8GU-Hkv9i66pYq2dv_KN0mNdeSLHWAbyU3wFsiRwY,7443
 asknews_sdk/api/news.py,sha256=GSv_6U4_7uo49ZrUHGseITA2yCj26e0KrqF4ob0g7ig,11705
 asknews_sdk/api/stories.py,sha256=OHM5wJjnE4KttlqPovRqKVk9oG0ESAEDsQDhbm127DU,10375
 asknews_sdk/client.py,sha256=Lj7akBppXJI7XUNDgkbQhEbcGDP58P5noEA_ncXjeYM,15904
 asknews_sdk/dto/__init__.py,sha256=tNRL7YBHo76LAeTADE9qIj5xR0eQywJHpuer7QSuJXY,740
-asknews_sdk/dto/base.py,sha256=fegkjcrPidJ8ql4iyOSQyqlT_tx-Mi_urgwdutNgoZw,1744
+asknews_sdk/dto/base.py,sha256=B5FJzeaKDNg9GE14cI7TdE_6vTQ1_HUhzY0RToVh-bw,2424
 asknews_sdk/dto/chat.py,sha256=AvRpnpGGaW3wCItqn77L-YtIg9OMCc-isuaeJyFEm80,3381
 asknews_sdk/dto/error.py,sha256=XhOo_lgl9vVHbhUVQiFIUXVaXAexUULjr7Hph5b6Ovc,606
 asknews_sdk/dto/news.py,sha256=vI3CC3rljq9I7T5ivp97KZpbvSeJJzel7b5N3qFEqyo,1284
 asknews_sdk/dto/sentiment.py,sha256=m6d-5mQ0dd4vewj7wF3-IZGLknXHkaKRmdYbyUaYI50,552
-asknews_sdk/dto/stories.py,sha256=UnM4rYq-j81hI4Bvvlu4SORIdqKfu0sDVqyG1C01Usk,4144
+asknews_sdk/dto/stories.py,sha256=91vsZukWukCrBR3GM4LkgT5Pn0NydU8Ec8hUb37uPRc,4166
 asknews_sdk/errors.py,sha256=F7VncOcrCxM1mYGCqV2NUGDnDnqQWgxhhmXd__-5bK8,1414
 asknews_sdk/sdk.py,sha256=etSaKeGiUIQ2qd1Ek_m86eKTEe7FbAYacUq1UdY1Nd4,6302
 asknews_sdk/security.py,sha256=C3_-lQMwHNx9E-4GC4LedXofJ2ybZLGQGxIh55nVvks,5248
 asknews_sdk/utils.py,sha256=YAk-0ANXWu7J9PlKCyptXZnlvle4cLXuQWXxjxxWojQ,1583
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.4.0.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.4.0.dist-info/METADATA,sha256=ZwmnxFqhQcTb-fxXYhH1im8BTXImMebogjw_Lina5G4,3185
-asknews-0.4.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.4.0.dist-info/RECORD,,
+asknews-0.5.0.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.5.0.dist-info/METADATA,sha256=t57msDyGwFhD8qQqSWR4OpHI-ulGmV_6dB86Tzw4cJg,3185
+asknews-0.5.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.5.0.dist-info/RECORD,,
```

