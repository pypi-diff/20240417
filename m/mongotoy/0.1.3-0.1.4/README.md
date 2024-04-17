# Comparing `tmp/mongotoy-0.1.3.tar.gz` & `tmp/mongotoy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongotoy-0.1.3.tar", max compression
+gzip compressed data, was "mongotoy-0.1.4.tar", max compression
```

## Comparing `mongotoy-0.1.3.tar` & `mongotoy-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.3/LICENSE
--rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.3/mongotoy/__init__.py
--rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.3/mongotoy/cache.py
--rw-r--r--   0        0        0    49516 2024-04-07 21:04:15.682116 mongotoy-0.1.3/mongotoy/db.py
--rw-r--r--   0        0        0    16382 2024-04-04 16:29:46.366685 mongotoy-0.1.3/mongotoy/documents.py
--rw-r--r--   0        0        0     6693 2024-04-03 17:32:35.942331 mongotoy-0.1.3/mongotoy/errors.py
--rw-r--r--   0        0        0     7719 2024-04-04 15:48:59.159339 mongotoy-0.1.3/mongotoy/expressions.py
--rw-r--r--   0        0        0    11917 2024-04-04 15:54:56.024009 mongotoy-0.1.3/mongotoy/fields.py
--rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.3/mongotoy/geodata.py
--rw-r--r--   0        0        0    37519 2024-04-07 05:47:07.295684 mongotoy-0.1.3/mongotoy/mappers.py
--rw-r--r--   0        0        0     5415 2024-04-04 16:29:08.681600 mongotoy-0.1.3/mongotoy/references.py
--rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.3/mongotoy/sync.py
--rw-r--r--   0        0        0    11819 2024-04-07 21:04:15.689215 mongotoy-0.1.3/mongotoy/types.py
--rw-r--r--   0        0        0      687 2024-04-07 21:21:43.106575 mongotoy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6650 2024-04-07 05:46:30.648934 mongotoy-0.1.3/README.md
--rw-r--r--   0        0        0     7225 1970-01-01 00:00:00.000000 mongotoy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.4/LICENSE
+-rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.4/mongotoy/__init__.py
+-rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.4/mongotoy/cache.py
+-rw-r--r--   0        0        0    49515 2024-04-17 16:33:55.586760 mongotoy-0.1.4/mongotoy/db.py
+-rw-r--r--   0        0        0    16382 2024-04-04 16:29:46.366685 mongotoy-0.1.4/mongotoy/documents.py
+-rw-r--r--   0        0        0     6693 2024-04-03 17:32:35.942331 mongotoy-0.1.4/mongotoy/errors.py
+-rw-r--r--   0        0        0     7731 2024-04-15 16:35:24.067748 mongotoy-0.1.4/mongotoy/expressions.py
+-rw-r--r--   0        0        0    11917 2024-04-04 15:54:56.024009 mongotoy-0.1.4/mongotoy/fields.py
+-rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.4/mongotoy/geodata.py
+-rw-r--r--   0        0        0    40200 2024-04-17 18:30:39.172399 mongotoy-0.1.4/mongotoy/mappers.py
+-rw-r--r--   0        0        0     5415 2024-04-04 16:29:08.681600 mongotoy-0.1.4/mongotoy/references.py
+-rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.4/mongotoy/sync.py
+-rw-r--r--   0        0        0    11992 2024-04-17 17:44:47.007889 mongotoy-0.1.4/mongotoy/types.py
+-rw-r--r--   0        0        0      715 2024-04-17 19:01:28.715731 mongotoy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6484 2024-04-14 05:31:35.928668 mongotoy-0.1.4/README.md
+-rw-r--r--   0        0        0     7128 1970-01-01 00:00:00.000000 mongotoy-0.1.4/PKG-INFO
```

### Comparing `mongotoy-0.1.3/LICENSE` & `mongotoy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/cache.py` & `mongotoy-0.1.4/mongotoy/cache.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/db.py` & `mongotoy-0.1.4/mongotoy/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import datetime
 import functools
 import inspect
-import math
 import mimetypes
 import os
 import typing
 
 import bson
 import gridfs
 import pymongo
@@ -460,15 +459,15 @@
         self,
         *conn,
         ping: bool = False
     ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
         return self._connect(*conn, ping)
 
     @sync.proxy
-    async def migrate(
+    def migrate(
         self,
         document_cls: typing.Type[T],
         session: 'Session' = None
     ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
         return self._migrate(document_cls, session)
 
     @sync.proxy
@@ -1262,62 +1261,68 @@
             self.filename,
             src=src,
             metadata=metadata,
             chunk_size_bytes=self.chunk_size
         )
 
     # noinspection SpellCheckingInspection
-    async def _download(self, fs: FsBucket, dest: typing.IO, revision: int = None):
+    async def _download_to(self, fs: FsBucket, dest: typing.IO, revision: int = 0):
         """
-        Downloads the file from the file system.
+        Downloads a file revision.
+
+        Revision numbers are defined as follows:
+
+            0 = the original stored file
+            1 = the first revision
+            2 = the second revision
+            ...
+            -2 = the second most recent revision
+            -1 = the most recent revision
 
         Args:
             fs (FsBucket): The file system bucket from where the file will be downloaded.
             dest (typing.IO): The destination file object to write the downloaded file contents.
-            revision (int): The revision number of the file to download. If None, download the latest revision.
+            revision (int): The revision number of the file to download.
 
         """
-        if revision is None:
-            await fs._bucket.download_to_stream(
-                file_id=self.id,
-                destination=dest,
-                session=fs._session.driver_session
-            )
-        else:
-            await fs._bucket.download_to_stream_by_name(
-                filename=self.filename,
-                destination=dest,
-                revision=revision,
-                session=fs._session.driver_session
-            )
+        await fs._bucket.download_to_stream_by_name(
+            filename=self.filename,
+            destination=dest,
+            revision=revision,
+            session=fs._session.driver_session
+        )
 
-    async def _stream(self, fs: FsBucket, revision: int = None) -> 'FsOutput':
+    async def _stream(self, fs: FsBucket, revision: int = 0) -> 'FsObjectStream':
         """
         Streams the file from the file system.
 
+        Revision numbers are defined as follows:
+
+            0 = the original stored file
+            1 = the first revision
+            2 = the second revision
+            ...
+            -2 = the second most recent revision
+            -1 = the most recent revision
+
         Args:
             fs (FsBucket): The file system bucket from where the file will be streamed.
-            revision (int, optional): The revision number of the file to stream. If None, streams the latest revision.
+            revision (int, optional): The revision number of the file to stream.
 
         Returns:
-            AsyncIOMotorGridOut: An asynchronous grid file stream.
+            FsObjectStream: An asynchronous file streamer.
 
         """
-        if revision is None:
-            grid_out = await fs._bucket.open_download_stream(
-                file_id=self.id,
-                session=fs._session.driver_session
-            )
-        else:
-            grid_out = await fs._bucket.open_download_stream_by_name(
-                filename=self.filename,
-                revision=revision,
-                session=fs._session.driver_session
-            )
-        return FsOutput(grid_out)
+        grid_out = await fs._bucket.open_download_stream_by_name(
+            filename=self.filename,
+            revision=revision,
+            session=fs._session.driver_session
+        )
+
+        return FsObjectStream(grid_out)
 
     async def _delete(self, fs: FsBucket):
         await fs._bucket.delete(
             file_id=self.id,
             session=fs._session.driver_session
         )
 
@@ -1327,38 +1332,38 @@
         fs: FsBucket,
         src: typing.IO | bytes,
         metadata: dict = None
     ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'FsObject'], 'FsObject']:
         return self._create_revision(fs, src, metadata)
 
     @sync.proxy
-    def download(
+    def download_to(
         self,
         fs: FsBucket,
         dest: typing.IO,
-        revision: int = None
+        revision: int = 0
     ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
-        return self._download(fs, dest, revision)
+        return self._download_to(fs, dest, revision)
 
     @sync.proxy
     def stream(
         self,
         fs: FsBucket,
-        revision: int = None
-    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'FsOutput'], 'FsOutput']:
+        revision: int = 0
+    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'FsObjectStream'], 'FsObjectStream']:
         return self._stream(fs, revision)
 
     @sync.proxy
     def delete(self, fs: FsBucket) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
         return self._delete(fs)
 
 
-class FsOutput:
+class FsObjectStream:
     """
-    Represents a file stored in MongoDB GridFS.
+    Represents the contents of file stored in MongoDB GridFS.
 
     Args:
         grid_out (AsyncIOMotorGridOut): The underlying GridFS file object.
 
     """
 
     def __init__(self, grid_out: AsyncIOMotorGridOut):
```

### Comparing `mongotoy-0.1.3/mongotoy/documents.py` & `mongotoy-0.1.4/mongotoy/documents.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/errors.py` & `mongotoy-0.1.4/mongotoy/errors.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/expressions.py` & `mongotoy-0.1.4/mongotoy/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,42 +35,42 @@
             return other
         return Sort({**self, **other})
 
     def __repr__(self):
         return f'Sort({super().__repr__()})'
 
     @classmethod
-    def Asc(cls, *args) -> 'Sort':
+    def Asc(cls, *fields) -> 'Sort':
         """
         Utility function to create ascending sort expressions.
 
         Args:
-            *args: Variable number of fields to be sorted in ascending order.
+            *fields: Variable number of fields to be sorted in ascending order.
 
         Returns:
             Sort: Resulting ascending sort expression.
         """
         exp = cls()
-        for field in args:
+        for field in fields:
             exp = exp | cls({str(field): pymongo.ASCENDING})
         return exp
 
     @classmethod
-    def Desc(cls, *args) -> 'Sort':
+    def Desc(cls, *fields) -> 'Sort':
         """
         Utility function to create descending sort expressions.
 
         Args:
-            *args: Variable number of field to be sorted in ascending order.
+            *fields: Variable number of field to be sorted in ascending order.
 
         Returns:
             Sort: Resulting ascending sort expression.
         """
         exp = cls()
-        for field in args:
+        for field in fields:
             exp = exp | cls({str(field): pymongo.DESCENDING})
         return exp
 
 
 # noinspection PyPep8Naming
 class Query(dict[str, list | dict]):
     """
```

### Comparing `mongotoy-0.1.3/mongotoy/fields.py` & `mongotoy-0.1.4/mongotoy/fields.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/geodata.py` & `mongotoy-0.1.4/mongotoy/geodata.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/mappers.py` & `mongotoy-0.1.4/mongotoy/mappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -318,17 +318,17 @@
 
         Args:
             mapper (Mapper): The mapper for the list items.
             options (MapperOptions): Mapper configuration params.
 
         """
         self._mapper = mapper
-        # SequenceMapper must be at least empty list not an EmptyValue for ReferencedDocumentMapper
+        # SequenceMapper must be a least an empty sequence not an EmptyValue for ReferencedDocumentMapper
         if options.default is expressions.EmptyValue and isinstance(self.unwrap(), ReferencedDocumentMapper):
-            options.default = []
+            options.default = self.__bind__()
         super().__init__(options)
 
     @property
     def mapper(self) -> Mapper:
         """
         Get the mapper for the list items.
 
@@ -599,56 +599,14 @@
         Returns:
             Any: The dumped value.
 
         """
         return getattr(value, self.ref_field.name)
 
 
-class ListMapper(SequenceMapper, bind=list):
-    """
-    Mapper for handling lists.
-
-    Inherits from ManyMapper and specifies 'list' as the binding type.
-
-    """
-
-
-class TupleMapper(SequenceMapper, bind=tuple):
-    """
-    Mapper for handling tuples.
-
-    Inherits from ManyMapper and specifies 'tuple' as the binding type.
-
-    """
-    def validate(self, value) -> typing.Any:
-        if isinstance(value, list):
-            value = tuple(value)
-        return super().validate(value)
-
-
-class SetMapper(SequenceMapper, bind=set):
-    """
-    Mapper for handling sets.
-
-    Inherits from ManyMapper and specifies 'set' as the binding type.
-
-    """
-
-    def validate(self, value) -> typing.Any:
-        if isinstance(value, list):
-            value = set(value)
-        return super().validate(value)
-
-    def dump_json(self, value, **options) -> typing.Any:
-        return list(value)
-
-    def dump_bson(self, value, **options) -> typing.Any:
-        return list(value)
-
-
 class StrMapper(Mapper, bind=str):
     """
     Mapper for handling string values.
     """
 
     def validate(self, value) -> typing.Any:
         """
@@ -684,14 +642,82 @@
                     raise ValueError(
                         f'Invalid value {value}, required choices={self._options.extra["choices"]}'
                     )
 
         return value
 
 
+class IntMapper(ComparableMapper, bind=int):
+    """
+    Mapper for handling integer values.
+    """
+
+
+class FloatMapper(ComparableMapper, bind=float):
+    """
+    Mapper for handling float values.
+    """
+
+
+class DecimalMapper(ComparableMapper, bind=decimal.Decimal):
+    """
+    Mapper for handling decimal values.
+    """
+
+    def validate(self, value) -> typing.Any:
+        """
+        Validate the decimal value.
+
+        Args:
+            value: The value to be validated.
+
+        Returns:
+            Any: The validated value.
+
+        Raises:
+            TypeError: If validation fails due to incorrect data type.
+
+        """
+        if isinstance(value, bson.Decimal128):
+            value = value.to_decimal()
+        value = super().validate(value)
+        # Ensure decimal limits for MongoDB
+        # https://www.mongodb.com/docs/upcoming/release-notes/3.4/#decimal-type
+        ctx = decimal.Context(prec=34)
+        return ctx.create_decimal(value)
+
+    def dump_json(self, value, **options) -> typing.Any:
+        """
+        Dump the decimal value to a JSON-serializable format.
+
+        Args:
+            value: The value to be dumped.
+            **options: Additional options.
+
+        Returns:
+            Any: The dumped value.
+
+        """
+        return float(value)
+
+    def dump_bson(self, value, **options) -> typing.Any:
+        """
+        Dump the decimal value to BSON.
+
+        Args:
+            value: The value to be dumped.
+            **options: Additional options.
+
+        Returns:
+            Any: The dumped value.
+
+        """
+        return bson.Decimal128(value)
+
+
 class BoolMapper(Mapper, bind=bool):
     """
     Mapper for handling boolean values.
     """
 
     def validate(self, value) -> typing.Any:
         """
@@ -747,280 +773,406 @@
             Any: The dumped value.
 
         """
         import base64
         return base64.b64encode(value).decode()
 
 
-class ObjectIdMapper(Mapper, bind=bson.ObjectId):
+class UUIDMapper(Mapper, bind=uuid.UUID):
     """
-    Mapper for handling BSON ObjectId values.
+    Mapper for handling UUID values.
     """
 
     def validate(self, value) -> typing.Any:
         """
-        Validate the ObjectId value.
+        Validate the UUID value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
-        if not bson.ObjectId.is_valid(value):
-            raise TypeError(f'Invalid data type {type(value)}, required is {bson.ObjectId}')
-        return bson.ObjectId(value)
+        if not isinstance(value, uuid.UUID):
+            raise TypeError(f'Invalid data type {type(value)}, required is {uuid.UUID}')
+        return value
 
     def dump_json(self, value, **options) -> typing.Any:
         """
-        Dump the ObjectId value to a JSON-serializable format.
+        Dump the UUID value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
         return str(value)
 
 
-class UUIDMapper(Mapper, bind=uuid.UUID):
+class DateTimeMapper(ComparableMapper, bind=datetime.datetime):
     """
-    Mapper for handling UUID values.
+    Mapper for handling datetime values.
+    """
+
+    def dump_json(self, value, **options) -> typing.Any:
+        """
+        Dump the datetime value to a JSON-serializable format.
+
+        Args:
+            value: The value to be dumped.
+            **options: Additional options.
+
+        Returns:
+            Any: The dumped value.
+
+        """
+        return value.isoformat()
+
+
+class DateMapper(ComparableMapper, bind=datetime.date):
+    """
+    Mapper for handling date values.
     """
 
     def validate(self, value) -> typing.Any:
         """
-        Validate the UUID value.
+        Validate the date value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
-        if not isinstance(value, uuid.UUID):
-            raise TypeError(f'Invalid data type {type(value)}, required is {uuid.UUID}')
-        return value
+        if isinstance(value, datetime.datetime):
+            value = value.date()
+        return super().validate(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
-        Dump the UUID value to a JSON-serializable format.
+        Dump the date value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return str(value)
+        return value.isoformat()
 
+    def dump_bson(self, value, **options) -> typing.Any:
+        """
+        Dump the date value to BSON.
 
-class IntMapper(ComparableMapper, bind=int):
-    """
-    Mapper for handling integer values.
-    """
+        Args:
+            value: The value to be dumped.
+            **options: Additional options.
 
+        Returns:
+            Any: The dumped value.
 
-class FloatMapper(ComparableMapper, bind=float):
-    """
-    Mapper for handling float values.
-    """
+        """
+        return datetime.datetime.combine(date=value, time=datetime.time.min)
 
 
-class DecimalMapper(ComparableMapper, bind=decimal.Decimal):
+class TimeMapper(ComparableMapper, bind=datetime.time):
     """
-    Mapper for handling decimal values.
+    Mapper for handling time values.
     """
 
     def validate(self, value) -> typing.Any:
         """
-        Validate the decimal value.
+        Validate the time value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
-        if isinstance(value, bson.Decimal128):
-            value = value.to_decimal()
-        value = super().validate(value)
-        # Ensure decimal limits for MongoDB
-        # https://www.mongodb.com/docs/upcoming/release-notes/3.4/#decimal-type
-        ctx = decimal.Context(prec=34)
-        return ctx.create_decimal(value)
+        if isinstance(value, datetime.datetime):
+            value = value.time()
+        return super().validate(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
-        Dump the decimal value to a JSON-serializable format.
+        Dump the time value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return float(value)
+        return value.isoformat()
 
     def dump_bson(self, value, **options) -> typing.Any:
         """
-        Dump the decimal value to BSON.
+        Dump the time value to BSON.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return bson.Decimal128(value)
+        return datetime.datetime.combine(date=datetime.datetime.min, time=value)
 
 
-class DateTimeMapper(ComparableMapper, bind=datetime.datetime):
+class ListMapper(SequenceMapper, bind=list):
     """
-    Mapper for handling datetime values.
+    Mapper for handling lists.
+
+    Inherits from ManyMapper and specifies 'list' as the binding type.
+
+    """
+
+
+class TupleMapper(SequenceMapper, bind=tuple):
+    """
+    Mapper for handling tuples.
+
+    Inherits from ManyMapper and specifies 'tuple' as the binding type.
+
+    """
+    def validate(self, value) -> typing.Any:
+        if isinstance(value, list):
+            value = tuple(value)
+        return super().validate(value)
+
+
+class SetMapper(SequenceMapper, bind=set):
+    """
+    Mapper for handling sets.
+
+    Inherits from ManyMapper and specifies 'set' as the binding type.
+
     """
 
+    def validate(self, value) -> typing.Any:
+        if isinstance(value, list):
+            value = set(value)
+        return super().validate(value)
+
     def dump_json(self, value, **options) -> typing.Any:
+        return list(value)
+
+    def dump_bson(self, value, **options) -> typing.Any:
+        return list(value)
+
+
+class ObjectIdMapper(Mapper, bind=bson.ObjectId):
+    """
+    Mapper for handling BSON ObjectId values.
+    """
+
+    def validate(self, value) -> typing.Any:
         """
-        Dump the datetime value to a JSON-serializable format.
+        Validate the ObjectId value.
+
+        Args:
+            value: The value to be validated.
+
+        Returns:
+            Any: The validated value.
+
+        Raises:
+            TypeError: If validation fails due to incorrect data type.
+
+        """
+        if not bson.ObjectId.is_valid(value):
+            raise TypeError(f'Invalid data type {type(value)}, required is {bson.ObjectId}')
+        return bson.ObjectId(value)
+
+    def dump_json(self, value, **options) -> typing.Any:
+        """
+        Dump the ObjectId value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return value.isoformat()
+        return str(value)
 
 
-class DateMapper(ComparableMapper, bind=datetime.date):
+class Int64Mapper(Mapper, bind=bson.Int64):
     """
-    Mapper for handling date values.
+    Mapper for handling BSON Int64 values.
     """
 
     def validate(self, value) -> typing.Any:
         """
-        Validate the date value.
+        Validate the Int64 value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
-        if isinstance(value, datetime.datetime):
-            value = value.date()
-        return super().validate(value)
+        if not isinstance(value, bson.Int64):
+            raise TypeError(f'Invalid data type {type(value)}, required is {bson.Int64}')
+        return value
 
     def dump_json(self, value, **options) -> typing.Any:
         """
-        Dump the date value to a JSON-serializable format.
+        Dump the Int64 value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return value.isoformat()
+        return int(value)
 
-    def dump_bson(self, value, **options) -> typing.Any:
+
+class Decimal128Mapper(Mapper, bind=bson.Decimal128):
+    """
+    Mapper for handling BSON Decimal128 values.
+    """
+
+    def validate(self, value) -> typing.Any:
         """
-        Dump the date value to BSON.
+        Validate the Decimal128 value.
+
+        Args:
+            value: The value to be validated.
+
+        Returns:
+            Any: The validated value.
+
+        Raises:
+            TypeError: If validation fails due to incorrect data type.
+
+        """
+        if not isinstance(value, bson.Decimal128):
+            raise TypeError(f'Invalid data type {type(value)}, required is {bson.Decimal128}')
+        return value
+
+    def dump_json(self, value, **options) -> typing.Any:
+        """
+        Dump the Decimal128 value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return datetime.datetime.combine(date=value, time=datetime.time.min)
+        return float(value.to_decimal())
 
 
-class TimeMapper(ComparableMapper, bind=datetime.time):
+class RegexMapper(Mapper, bind=bson.Regex):
     """
-    Mapper for handling time values.
+    Mapper for handling BSON Regex values.
     """
 
     def validate(self, value) -> typing.Any:
         """
-        Validate the time value.
+        Validate the Regex value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
-        if isinstance(value, datetime.datetime):
-            value = value.time()
-        return super().validate(value)
+        if not isinstance(value, bson.Regex):
+            value = bson.Regex.from_native(value)
+        return value
 
     def dump_json(self, value, **options) -> typing.Any:
         """
-        Dump the time value to a JSON-serializable format.
+        Dump the Regex value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return value.isoformat()
+        return f'{value.pattern}'
 
-    def dump_bson(self, value, **options) -> typing.Any:
+
+class CodeMapper(Mapper, bind=bson.Code):
+    """
+    Mapper for handling BSON Code values.
+    """
+
+    def validate(self, value) -> typing.Any:
         """
-        Dump the time value to BSON.
+        Validate the Code value.
+
+        Args:
+            value: The value to be validated.
+
+        Returns:
+            Any: The validated value.
+
+        Raises:
+            TypeError: If validation fails due to incorrect data type.
+
+        """
+        if not isinstance(value, bson.Code):
+            raise TypeError(f'Invalid data type {type(value)}, required is {bson.Code}')
+        return value
+
+    def dump_json(self, value, **options) -> typing.Any:
+        """
+        Dump the Decimal128 value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return datetime.datetime.combine(date=datetime.datetime.min, time=value)
+        return str(value)
 
 
 class ConstrainedStrMapper(StrMapper):
     """
     Mapper for handling constrained string values.
     """
 
@@ -1258,40 +1410,14 @@
         try:
             json.dumps(value)
         except Exception as e:
             raise ValueError(f'Invalid JSON data: {str(e)}') from None
 
         return types.Json(value)
 
-    def dump_json(self, value, **options) -> typing.Any:
-        """
-        Dump the JSON data to JSON.
-
-        Args:
-            value: The JSON data to be dumped.
-            **options: Additional options.
-
-        Returns:
-            Any: The dumped JSON data.
-        """
-        return dict(value)
-
-    def dump_bson(self, value, **options) -> typing.Any:
-        """
-        Dump the JSON data to BSON.
-
-        Args:
-            value: The JSON data to be dumped.
-            **options: Additional options.
-
-        Returns:
-            Any: The dumped JSON data.
-        """
-        return dict(value)
-
 
 class BsonMapper(Mapper, bind=types.Bson):
     """
     Mapper for handling BSON data.
 
     This mapper validates and handles BSON data.
     """
@@ -1326,36 +1452,19 @@
         Dump the BSON data to JSON.
 
         Args:
             value: The BSON data to be dumped.
             **options: Additional options.
 
         Returns:
-            Any: The dumped BSON data.
-
-        Raises:
-            NotImplementedError: As BSON data cannot be directly dumped to JSON.
-        """
-        # noinspection SpellCheckingInspection
-        raise NotImplementedError(
-            'mongotoy.types.Bson does not implement dump_json; use mongotoy.types.Json instead'
-        )
-
-    def dump_bson(self, value, **options) -> typing.Any:
-        """
-        Dump the BSON data to BSON.
-
-        Args:
-            value: The BSON data to be dumped.
-            **options: Additional options.
-
-        Returns:
-            Any: The dumped BSON data.
+            Any: The dumped JSON data.
         """
-        return bson.SON(value)
+        from bson import json_util
+        # noinspection PyProtectedMember
+        return json_util._json_convert(value, json_options=json_util.RELAXED_JSON_OPTIONS)
 
 
 class FileMapper(ReferencedDocumentMapper, bind=types.File):
     """
     Mapper for handling file references.
 
     This mapper handles references to files stored in a database.
```

### Comparing `mongotoy-0.1.3/mongotoy/references.py` & `mongotoy-0.1.4/mongotoy/references.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/sync.py` & `mongotoy-0.1.4/mongotoy/sync.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.3/mongotoy/types.py` & `mongotoy-0.1.4/mongotoy/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,20 @@
     Args:
         value (str): The IPv4 address value.
 
     Raises:
         ValueError: If the value is not a valid IPv4 address.
     """
 
+    _regex = re.compile(
+        r'(\b25[0-5]|\b2[0-4][0-9]|\b[01]?[0-9][0-9]?)(\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)){3}'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'(\b25[0-5]|\b2[0-4][0-9]|\b[01]?[0-9][0-9]?)(\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)){3}'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid IPv4 address')
         super().__init__(value)
 
 
 class IpV6(collections.UserString):
     """
     Represents an IPv6 address.
@@ -38,26 +40,28 @@
     Args:
         value (str): The IPv6 address value.
 
     Raises:
         ValueError: If the value is not a valid IPv6 address.
     """
 
+    # noinspection RegExpSimplifiable
+    _regex = re.compile(
+        r'(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:)'
+        r'{1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:)'
+        r'{1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]'
+        r'{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]'
+        r'{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}'
+        r'((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|'
+        r'([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|'
+        r'1{0,1}[0-9]){0,1}[0-9]))'
+    )
+
     def __init__(self, value):
-        # noinspection RegExpSimplifiable
-        if not re.compile(
-            r'(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:)'
-            r'{1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:)'
-            r'{1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]'
-            r'{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]'
-            r'{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}'
-            r'((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|'
-            r'([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|'
-            r'1{0,1}[0-9]){0,1}[0-9]))'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid IPv6 address')
         super().__init__(value)
 
 
 class Port(collections.UserString):
     """
     Represents a port number.
@@ -65,19 +69,21 @@
     Args:
         value (str): The port number value.
 
     Raises:
         ValueError: If the value is not a valid port number.
     """
 
+    _regex = re.compile(
+        r'^((6553[0-5])|(655[0-2][0-9])|(65[0-4][0-9]{2})|(6[0-4][0-9]{3})|([1-5][0-9]{4})|([0-5]{0,5})|'
+        r'([0-9]{1,4}))$'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'^((6553[0-5])|(655[0-2][0-9])|(65[0-4][0-9]{2})|(6[0-4][0-9]{3})|([1-5][0-9]{4})|([0-5]{0,5})|'
-            r'([0-9]{1,4}))$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid port number')
         super().__init__(value)
 
 
 class Mac(collections.UserString):
     """
     Represents a MAC address.
@@ -85,18 +91,20 @@
     Args:
         value (str): The MAC address value.
 
     Raises:
         ValueError: If the value is not a valid MAC address.
     """
 
+    _regex = re.compile(
+        r'^[a-fA-F0-9]{2}(:[a-fA-F0-9]{2}){5}$'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'^[a-fA-F0-9]{2}(:[a-fA-F0-9]{2}){5}$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid MAC address')
         super().__init__(value)
 
 
 class Phone(collections.UserString):
     """
     Represents a phone number.
@@ -104,19 +112,21 @@
     Args:
         value (str): The phone number value.
 
     Raises:
         ValueError: If the value is not a valid phone number.
     """
 
+    # noinspection RegExpRedundantEscape,RegExpSimplifiable
+    _regex = re.compile(
+        r'^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$'
+    )
+
     def __init__(self, value):
-        # noinspection RegExpRedundantEscape,RegExpSimplifiable
-        if not re.compile(
-            r'^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid phone number')
         super().__init__(value)
 
 
 class Email(collections.UserString):
     """
     Represents an email address.
@@ -124,20 +134,22 @@
     Args:
         value (str): The email address value.
 
     Raises:
         ValueError: If the value is not a valid email address.
     """
 
+    _regex = re.compile(
+        r'(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|'
+        r'(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]'
+        r'{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|'
-            r'(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]'
-            r'{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid email address')
         super().__init__(value)
 
 
 class Card(collections.UserString):
     """
     Represents a credit card number.
@@ -145,21 +157,23 @@
     Args:
         value (str): The credit card number value.
 
     Raises:
         ValueError: If the value is not a valid credit card number.
     """
 
+    _regex = re.compile(
+        r'(^4[0-9]{12}(?:[0-9]{3})?$)|(^(?:5[1-5][0-9]{2}|222[1-9]|22'
+        r'[3-9][0-9]|2[3-6][0-9]{2}|27[01][0-9]|2720)[0-9]{12}$)|(3[47][0-9]'
+        r'{13})|(^3(?:0[0-5]|[68][0-9])[0-9]{11}$)|(^6(?:011|5[0-9]{2})[0-9]'
+        r'{12}$)|(^(?:2131|1800|35\d{3})\d{11}$)'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'(^4[0-9]{12}(?:[0-9]{3})?$)|(^(?:5[1-5][0-9]{2}|222[1-9]|22'
-            r'[3-9][0-9]|2[3-6][0-9]{2}|27[01][0-9]|2720)[0-9]{12}$)|(3[47][0-9]'
-            r'{13})|(^3(?:0[0-5]|[68][0-9])[0-9]{11}$)|(^6(?:011|5[0-9]{2})[0-9]'
-            r'{12}$)|(^(?:2131|1800|35\d{3})\d{11}$)'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid credit card number')
         super().__init__(value)
 
 
 class Ssn(collections.UserString):
     """
     Represents a Social Security Number (SSN).
@@ -167,18 +181,20 @@
     Args:
         value (str): The SSN value.
 
     Raises:
         ValueError: If the value is not a valid SSN.
     """
 
+    _regex = re.compile(
+        r'^(?!0{3})(?!6{3})[0-8]\d{2}-(?!0{2})\d{2}-(?!0{4})\d{4}$'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'^(?!0{3})(?!6{3})[0-8]\d{2}-(?!0{2})\d{2}-(?!0{4})\d{4}$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid SSN')
         super().__init__(value)
 
 
 class Hashtag(collections.UserString):
     """
     Represents a hashtag.
@@ -186,18 +202,20 @@
     Args:
         value (str): The hashtag value.
 
     Raises:
         ValueError: If the value is not a valid hashtag.
     """
 
+    _regex = re.compile(
+        r'^#[^ !@#$%^&*(),.?":{}|<>]*$'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'^#[^ !@#$%^&*(),.?":{}|<>]*$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid hashtag')
         super().__init__(value)
 
 
 class Doi(collections.UserString):
     """
     Represents a Digital Object Identifier (DOI).
@@ -205,19 +223,21 @@
     Args:
         value (str): The DOI value.
 
     Raises:
         ValueError: If the value is not a valid DOI.
     """
 
+    # noinspection RegExpRedundantEscape,RegExpSimplifiable
+    _regex = re.compile(
+        r'^(10\.\d{4,5}\/[\S]+[^;,.\s])$'
+    )
+
     def __init__(self, value):
-        # noinspection RegExpRedundantEscape,RegExpSimplifiable
-        if not re.compile(
-            r'^(10\.\d{4,5}\/[\S]+[^;,.\s])$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid DOI')
         super().__init__(value)
 
 
 class Url(collections.UserString):
     """
     Represents a URL.
@@ -225,20 +245,22 @@
     Args:
         value (str): The URL value.
 
     Raises:
         ValueError: If the value is not a valid URL.
     """
 
+    # noinspection RegExpDuplicateCharacterInClass,RegExpRedundantEscape
+    _regex = re.compile(
+        r'https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b'
+        r'([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)'
+    )
+
     def __init__(self, value):
-        # noinspection RegExpDuplicateCharacterInClass,RegExpRedundantEscape
-        if not re.compile(
-            r'https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b'
-            r'([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid URL')
         super().__init__(value)
 
 
 class Version(collections.UserString):
     """
     Represents a Semantic Version Number.
@@ -246,20 +268,22 @@
     Args:
         value (str): The version number value.
 
     Raises:
         ValueError: If the value is not a valid Semantic Version Number.
     """
 
+    _regex = re.compile(
+        r'^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-]'
+        r'[0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+'
+        r'([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$'
+    )
+
     def __init__(self, value):
-        if not re.compile(
-            r'^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-]'
-            r'[0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+'
-            r'([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$'
-        ).fullmatch(value):
+        if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid Semantic Version Number')
         super().__init__(value)
 
 
 class Point(geodata.Position):
     """
     For type "Point", the "coordinates" member is a single position.
@@ -363,37 +387,37 @@
         fs: 'db.FsBucket',
         src: typing.IO | bytes,
         metadata: dict = None
     ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'File'], 'File']:
         pass
 
     # noinspection SpellCheckingInspection
-    def download(
+    def download_to(
         self,
         fs: 'db.FsBucket',
         dest: typing.IO,
         revision: int = None
     ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
         pass
 
     def stream(
         self,
         fs: 'db.FsBucket',
         revision: int = None
-    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, '_FileOut'], '_FileOut']:
+    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'FileStream'], 'FileStream']:
         pass
 
     def delete(self, fs: 'db.FsBucket') -> typing.Coroutine[typing.Any, typing.Any, None] | None:
         pass
 
 
-class _FileOut(typing.Protocol):
+class FileStream(typing.Protocol):
     # noinspection SpellCheckingInspection
     """
-    This is a facade for type mogotoy.db.FsOutput
+    This is a facade for type mogotoy.db.FsObjectStream
     """
 
     def seek(self, pos: int, whence: int = os.SEEK_SET) -> int:
         pass
 
     def seekable(self) -> bool:
         pass
@@ -409,8 +433,7 @@
 
     # noinspection SpellCheckingInspection
     def readchunk(self) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
         pass
 
     def readline(self, size: int = -1) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
         pass
-
```

### Comparing `mongotoy-0.1.3/pyproject.toml` & `mongotoy-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mongotoy"
-version = "0.1.3"
-description = "Async ODM for MongoDB"
+version = "0.1.4"
+description = "Comprehensive ODM for MongoDB"
 license = "Apache-2.0"
 authors = ["gurcuff91 <gf.meneses91@gmail.com>"]
 readme = "README.md"
 homepage = "https://gurcuff91.github.io/mongotoy"
 repository = "https://github.com/gurcuff91/mongotoy"
 keywords = ["mapping", "asyncio", "odm", "mongodb"]
 classifiers = [
@@ -13,13 +13,14 @@
     "Intended Audience :: Developers",
     "Topic :: Database",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-motor = "^3.3.2"
+motor = "^3.4.0"
+pymongo = "^4.6.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mongotoy-0.1.3/README.md` & `mongotoy-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,115 +1,94 @@
 <p align="center">
   <a href="https://github.com/gurcuff91/mongotoy">
     <img src="https://github.com/gurcuff91/mongotoy/blob/master/docs/assets/mongotoy.png" alt="Mongotoy Logo" width="45%" height="auto">
   </a>
 </p>
 
 <p align="center">
-  <i>Async ODM for MongoDB.</i>
+  <i>Comprehensive ODM for MongoDB</i>
 </p>
 
 <p align="center">
   <a href="https://pypi.org/project/mongotoy/">
     <img src="https://img.shields.io/pypi/v/mongotoy?color=%2334D058&label=version" alt="Version"/>
   </a>
   <a href="https://pypi.org/project/mongotoy/">
     <img src="https://img.shields.io/pypi/pyversions/mongotoy.svg?color=%2334D058" alt="Supported Python Versions"/>
   </a>
 </p>
 
 <hr>
 <p align="justify">
-  <b>Mongotoy</b> is a comprehensive asynchronous Object-Document Mapper (ODM) designed to simplify interactions 
-  with MongoDB databases in Python applications. Leveraging the Motor asynchronous MongoDB driver, Mongotoy 
-  seamlessly integrates asynchronous programming with MongoDB, providing developers with a powerful toolset for 
-  building high-performance applications. This integration allows for efficient communication with MongoDB databases,
-  ensuring optimal scalability and responsiveness. With Mongotoy, developers can harness the full potential of 
-  MongoDB's features while enjoying the benefits of asynchronous programming, making it an ideal choice for modern, 
-  data-driven applications
+  Mongotoy is a comprehensive Object-Document Mapper (ODM) that streamlines interactions with MongoDB databases in 
+  Python applications. Powered by <a href="https://github.com/mongodb/motor">Motor</a> driver, Mongotoy seamlessly 
+  integrates with MongoDB, offering a versatile toolkit for constructing high-performance applications. This integration
+  facilitates efficient communication with MongoDB databases, guaranteeing optimal scalability and responsiveness. With 
+  Mongotoy, you can unlock the full potential of MongoDB's features.
 </p>
 <hr>
 
 ## Features
 
 - **Asynchronous Power**: Mongotoy leverages the asynchronous paradigm of Python, enabling efficient management of
 I/O operations for optimal performance and responsiveness in applications.
 
-
-- **Based on Motor Driver**: Mongotoy is built on top of the asynchronous Motor MongoDB driver, ensuring seamless 
-integration with asynchronous Python applications. 
-
+- **Based on Motor Driver**: Mongotoy is built on top of the asynchronous [Motor](https://github.com/mongodb/motor)
+MongoDB driver, ensuring seamless integration with asynchronous Python applications.
 
 - **Schemaless Flexibility**: With a schemaless design, Mongotoy empowers developers to work with MongoDB databases
 without rigid schemas, adapting to evolving data models effortlessly.
 
-
 - **Intuitive API**: Mongotoy features an elegant and straightforward API facilitating common database operations.
 
-
 - **Flexible Configuration Options**: Mongotoy offers extensive configuration options at both the database and 
 document levels, enabling fine-tuning of MongoDB interactions for optimal performance and reliability.
 
-
 - **Custom Data Types Support**: Mongotoy simplifies handling of custom data types and allows defining new types
 through Data Mapper classes, enhancing data integrity and consistency.
 
-
 - **Object-Document Mapping**: Simplifying MongoDB document manipulation, Mongotoy maps Python objects to MongoDB 
 documents seamlessly, enabling intuitive and object-oriented interactions.
 
-
 - **Document Serialization**: Mongotoy supports serialization of documents into JSON, BSON, or Python dictionaries, 
 enabling seamless integration with different parts of an application stack.
 
-
 - **Document Inheritance Support**: Mongotoy provides robust support for document inheritance, enabling the creation
 of hierarchical data models and promoting code reuse and maintainability.
 
-
 - **Python Type Hint Support**: Mongotoy allows developers to define document fields using Python type hints, 
 enhancing code readability and enabling type checking.
 
-
 - **Relationship Management**: Simplifying relationship management between documents, Mongotoy offers robust support
 for references and embedded documents, automating insertions, deletions, and updates.
 
-
 - **Automatic Operation Handling**: Mongotoy automates insertion and deletion management, ensuring data integrity 
 and consistency across related documents.
 
-
 - **Query Building**: Mongotoy provides a powerful query building interface for constructing complex queries using 
 Pythonic syntax.
 
-
 - **Index Management**: Mongotoy simplifies the management of database indexes, optimizing query performance for 
 efficient data retrieval.
 
-
 - **Transactions**: Supporting MongoDB transactions, Mongotoy ensures data consistency and atomicity across multiple
 operations within a single transactional context.
 
-
 - **Geospatial Data Support**: Mongotoy offers robust support for geospatial data types, facilitating storage, 
 querying, and spatial analysis.
 
-
 - **Database Seeding Management**: With built-in support for database seeding, Mongotoy streamlines the 
 initialization of databases with predefined data sets, enhancing developer productivity.
 
-
 - **Support for Capped Collections**: Mongotoy natively supports capped collections in MongoDB, ideal for 
 scenarios requiring fixed-size, ordered datasets.
 
-
 - **Time Series Collections Management**: Mongotoy provides robust support for managing time series data in 
 MongoDB, optimized for storing and querying time-stamped data points.
 
-
 - **GridFS File Handling**: Mongotoy seamlessly integrates with MongoDB's GridFS storage system for efficient
 handling of large files, offering a high-level interface for file management within MongoDB.
 
 ## Minimal Example
 Let's begin with a minimal example by defining a document and performing CRUD operations on the database.
 
 ```python
```

#### html2text {}

```diff
@@ -1,76 +1,75 @@
                                 _[_M_o_n_g_o_t_o_y_ _L_o_g_o_]
-                            Async ODM for MongoDB.
+                         Comprehensive ODM for MongoDB
                      _[_V_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]
 ===============================================================================
-MMoonnggoottooyy is a comprehensive asynchronous Object-Document Mapper (ODM) designed
-to simplify interactions with MongoDB databases in Python applications.
-Leveraging the Motor asynchronous MongoDB driver, Mongotoy seamlessly
-integrates asynchronous programming with MongoDB, providing developers with a
-powerful toolset for building high-performance applications. This integration
-allows for efficient communication with MongoDB databases, ensuring optimal
-scalability and responsiveness. With Mongotoy, developers can harness the full
-potential of MongoDB's features while enjoying the benefits of asynchronous
-programming, making it an ideal choice for modern, data-driven applications
+Mongotoy is a comprehensive Object-Document Mapper (ODM) that streamlines
+interactions with MongoDB databases in Python applications. Powered by _M_o_t_o_r
+driver, Mongotoy seamlessly integrates with MongoDB, offering a versatile
+toolkit for constructing high-performance applications. This integration
+facilitates efficient communication with MongoDB databases, guaranteeing
+optimal scalability and responsiveness. With Mongotoy, you can unlock the full
+potential of MongoDB's features.
 ===============================================================================
 ## Features - **Asynchronous Power**: Mongotoy leverages the asynchronous
 paradigm of Python, enabling efficient management of I/O operations for optimal
 performance and responsiveness in applications. - **Based on Motor Driver**:
-Mongotoy is built on top of the asynchronous Motor MongoDB driver, ensuring
-seamless integration with asynchronous Python applications. - **Schemaless
-Flexibility**: With a schemaless design, Mongotoy empowers developers to work
-with MongoDB databases without rigid schemas, adapting to evolving data models
-effortlessly. - **Intuitive API**: Mongotoy features an elegant and
-straightforward API facilitating common database operations. - **Flexible
-Configuration Options**: Mongotoy offers extensive configuration options at
-both the database and document levels, enabling fine-tuning of MongoDB
-interactions for optimal performance and reliability. - **Custom Data Types
-Support**: Mongotoy simplifies handling of custom data types and allows
-defining new types through Data Mapper classes, enhancing data integrity and
-consistency. - **Object-Document Mapping**: Simplifying MongoDB document
-manipulation, Mongotoy maps Python objects to MongoDB documents seamlessly,
-enabling intuitive and object-oriented interactions. - **Document
-Serialization**: Mongotoy supports serialization of documents into JSON, BSON,
-or Python dictionaries, enabling seamless integration with different parts of
-an application stack. - **Document Inheritance Support**: Mongotoy provides
-robust support for document inheritance, enabling the creation of hierarchical
-data models and promoting code reuse and maintainability. - **Python Type Hint
-Support**: Mongotoy allows developers to define document fields using Python
-type hints, enhancing code readability and enabling type checking. -
-**Relationship Management**: Simplifying relationship management between
-documents, Mongotoy offers robust support for references and embedded
-documents, automating insertions, deletions, and updates. - **Automatic
-Operation Handling**: Mongotoy automates insertion and deletion management,
-ensuring data integrity and consistency across related documents. - **Query
-Building**: Mongotoy provides a powerful query building interface for
-constructing complex queries using Pythonic syntax. - **Index Management**:
-Mongotoy simplifies the management of database indexes, optimizing query
-performance for efficient data retrieval. - **Transactions**: Supporting
-MongoDB transactions, Mongotoy ensures data consistency and atomicity across
-multiple operations within a single transactional context. - **Geospatial Data
-Support**: Mongotoy offers robust support for geospatial data types,
-facilitating storage, querying, and spatial analysis. - **Database Seeding
-Management**: With built-in support for database seeding, Mongotoy streamlines
-the initialization of databases with predefined data sets, enhancing developer
-productivity. - **Support for Capped Collections**: Mongotoy natively supports
-capped collections in MongoDB, ideal for scenarios requiring fixed-size,
-ordered datasets. - **Time Series Collections Management**: Mongotoy provides
-robust support for managing time series data in MongoDB, optimized for storing
-and querying time-stamped data points. - **GridFS File Handling**: Mongotoy
-seamlessly integrates with MongoDB's GridFS storage system for efficient
-handling of large files, offering a high-level interface for file management
-within MongoDB. ## Minimal Example Let's begin with a minimal example by
-defining a document and performing CRUD operations on the database. ```python
-import asyncio from mongotoy import Document, Engine import datetime class
-Person(Document): name: str last_name: str dob: datetime.date # Create database
-engine db = Engine('test-db') async def main(): # Create a new Person instance
-person = Person( name='John', last_name='Doe', dob=datetime.date(1990, 12, 25)
-) # Connect to the MongoDB database await db.connect('mongodb://localhost:
-27017') # Open a database session async with db.session() as session: # Save
-the person to the database await session.save(person) # Fetch all persons from
-database async for c in session.objects(Person): print(c.dump_dict()) # Update
-person dob person.dob=datetime.date(1995, 10, 25) await session.save(person) #
-Delete person from database await session.delete(person) if __name__ ==
-'__main__': asyncio.run(main()) ``` ## Installing To install, just run: ```sh
-pip install mongotoy ``` Or, if using poetry: ```sh poetry add mongotoy ``` ##
-Extras See full documentation at: https://gurcuff91.github.io/mongotoy ### If
-you like this project !!_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+Mongotoy is built on top of the asynchronous [Motor](https://github.com/
+mongodb/motor) MongoDB driver, ensuring seamless integration with asynchronous
+Python applications. - **Schemaless Flexibility**: With a schemaless design,
+Mongotoy empowers developers to work with MongoDB databases without rigid
+schemas, adapting to evolving data models effortlessly. - **Intuitive API**:
+Mongotoy features an elegant and straightforward API facilitating common
+database operations. - **Flexible Configuration Options**: Mongotoy offers
+extensive configuration options at both the database and document levels,
+enabling fine-tuning of MongoDB interactions for optimal performance and
+reliability. - **Custom Data Types Support**: Mongotoy simplifies handling of
+custom data types and allows defining new types through Data Mapper classes,
+enhancing data integrity and consistency. - **Object-Document Mapping**:
+Simplifying MongoDB document manipulation, Mongotoy maps Python objects to
+MongoDB documents seamlessly, enabling intuitive and object-oriented
+interactions. - **Document Serialization**: Mongotoy supports serialization of
+documents into JSON, BSON, or Python dictionaries, enabling seamless
+integration with different parts of an application stack. - **Document
+Inheritance Support**: Mongotoy provides robust support for document
+inheritance, enabling the creation of hierarchical data models and promoting
+code reuse and maintainability. - **Python Type Hint Support**: Mongotoy allows
+developers to define document fields using Python type hints, enhancing code
+readability and enabling type checking. - **Relationship Management**:
+Simplifying relationship management between documents, Mongotoy offers robust
+support for references and embedded documents, automating insertions,
+deletions, and updates. - **Automatic Operation Handling**: Mongotoy automates
+insertion and deletion management, ensuring data integrity and consistency
+across related documents. - **Query Building**: Mongotoy provides a powerful
+query building interface for constructing complex queries using Pythonic
+syntax. - **Index Management**: Mongotoy simplifies the management of database
+indexes, optimizing query performance for efficient data retrieval. -
+**Transactions**: Supporting MongoDB transactions, Mongotoy ensures data
+consistency and atomicity across multiple operations within a single
+transactional context. - **Geospatial Data Support**: Mongotoy offers robust
+support for geospatial data types, facilitating storage, querying, and spatial
+analysis. - **Database Seeding Management**: With built-in support for database
+seeding, Mongotoy streamlines the initialization of databases with predefined
+data sets, enhancing developer productivity. - **Support for Capped
+Collections**: Mongotoy natively supports capped collections in MongoDB, ideal
+for scenarios requiring fixed-size, ordered datasets. - **Time Series
+Collections Management**: Mongotoy provides robust support for managing time
+series data in MongoDB, optimized for storing and querying time-stamped data
+points. - **GridFS File Handling**: Mongotoy seamlessly integrates with
+MongoDB's GridFS storage system for efficient handling of large files, offering
+a high-level interface for file management within MongoDB. ## Minimal Example
+Let's begin with a minimal example by defining a document and performing CRUD
+operations on the database. ```python import asyncio from mongotoy import
+Document, Engine import datetime class Person(Document): name: str last_name:
+str dob: datetime.date # Create database engine db = Engine('test-db') async
+def main(): # Create a new Person instance person = Person( name='John',
+last_name='Doe', dob=datetime.date(1990, 12, 25) ) # Connect to the MongoDB
+database await db.connect('mongodb://localhost:27017') # Open a database
+session async with db.session() as session: # Save the person to the database
+await session.save(person) # Fetch all persons from database async for c in
+session.objects(Person): print(c.dump_dict()) # Update person dob
+person.dob=datetime.date(1995, 10, 25) await session.save(person) # Delete
+person from database await session.delete(person) if __name__ == '__main__':
+asyncio.run(main()) ``` ## Installing To install, just run: ```sh pip install
+mongotoy ``` Or, if using poetry: ```sh poetry add mongotoy ``` ## Extras See
+full documentation at: https://gurcuff91.github.io/mongotoy ### If you like
+this project !!_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

### Comparing `mongotoy-0.1.3/PKG-INFO` & `mongotoy-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,136 +1,116 @@
 Metadata-Version: 2.1
 Name: mongotoy
-Version: 0.1.3
-Summary: Async ODM for MongoDB
+Version: 0.1.4
+Summary: Comprehensive ODM for MongoDB
 Home-page: https://gurcuff91.github.io/mongotoy
 License: Apache-2.0
 Keywords: mapping,asyncio,odm,mongodb
 Author: gurcuff91
 Author-email: gf.meneses91@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: motor (>=3.3.2,<4.0.0)
+Requires-Dist: motor (>=3.4.0,<4.0.0)
+Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/gurcuff91/mongotoy
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/gurcuff91/mongotoy">
     <img src="https://github.com/gurcuff91/mongotoy/blob/master/docs/assets/mongotoy.png" alt="Mongotoy Logo" width="45%" height="auto">
   </a>
 </p>
 
 <p align="center">
-  <i>Async ODM for MongoDB.</i>
+  <i>Comprehensive ODM for MongoDB</i>
 </p>
 
 <p align="center">
   <a href="https://pypi.org/project/mongotoy/">
     <img src="https://img.shields.io/pypi/v/mongotoy?color=%2334D058&label=version" alt="Version"/>
   </a>
   <a href="https://pypi.org/project/mongotoy/">
     <img src="https://img.shields.io/pypi/pyversions/mongotoy.svg?color=%2334D058" alt="Supported Python Versions"/>
   </a>
 </p>
 
 <hr>
 <p align="justify">
-  <b>Mongotoy</b> is a comprehensive asynchronous Object-Document Mapper (ODM) designed to simplify interactions 
-  with MongoDB databases in Python applications. Leveraging the Motor asynchronous MongoDB driver, Mongotoy 
-  seamlessly integrates asynchronous programming with MongoDB, providing developers with a powerful toolset for 
-  building high-performance applications. This integration allows for efficient communication with MongoDB databases,
-  ensuring optimal scalability and responsiveness. With Mongotoy, developers can harness the full potential of 
-  MongoDB's features while enjoying the benefits of asynchronous programming, making it an ideal choice for modern, 
-  data-driven applications
+  Mongotoy is a comprehensive Object-Document Mapper (ODM) that streamlines interactions with MongoDB databases in 
+  Python applications. Powered by <a href="https://github.com/mongodb/motor">Motor</a> driver, Mongotoy seamlessly 
+  integrates with MongoDB, offering a versatile toolkit for constructing high-performance applications. This integration
+  facilitates efficient communication with MongoDB databases, guaranteeing optimal scalability and responsiveness. With 
+  Mongotoy, you can unlock the full potential of MongoDB's features.
 </p>
 <hr>
 
 ## Features
 
 - **Asynchronous Power**: Mongotoy leverages the asynchronous paradigm of Python, enabling efficient management of
 I/O operations for optimal performance and responsiveness in applications.
 
-
-- **Based on Motor Driver**: Mongotoy is built on top of the asynchronous Motor MongoDB driver, ensuring seamless 
-integration with asynchronous Python applications. 
-
+- **Based on Motor Driver**: Mongotoy is built on top of the asynchronous [Motor](https://github.com/mongodb/motor)
+MongoDB driver, ensuring seamless integration with asynchronous Python applications.
 
 - **Schemaless Flexibility**: With a schemaless design, Mongotoy empowers developers to work with MongoDB databases
 without rigid schemas, adapting to evolving data models effortlessly.
 
-
 - **Intuitive API**: Mongotoy features an elegant and straightforward API facilitating common database operations.
 
-
 - **Flexible Configuration Options**: Mongotoy offers extensive configuration options at both the database and 
 document levels, enabling fine-tuning of MongoDB interactions for optimal performance and reliability.
 
-
 - **Custom Data Types Support**: Mongotoy simplifies handling of custom data types and allows defining new types
 through Data Mapper classes, enhancing data integrity and consistency.
 
-
 - **Object-Document Mapping**: Simplifying MongoDB document manipulation, Mongotoy maps Python objects to MongoDB 
 documents seamlessly, enabling intuitive and object-oriented interactions.
 
-
 - **Document Serialization**: Mongotoy supports serialization of documents into JSON, BSON, or Python dictionaries, 
 enabling seamless integration with different parts of an application stack.
 
-
 - **Document Inheritance Support**: Mongotoy provides robust support for document inheritance, enabling the creation
 of hierarchical data models and promoting code reuse and maintainability.
 
-
 - **Python Type Hint Support**: Mongotoy allows developers to define document fields using Python type hints, 
 enhancing code readability and enabling type checking.
 
-
 - **Relationship Management**: Simplifying relationship management between documents, Mongotoy offers robust support
 for references and embedded documents, automating insertions, deletions, and updates.
 
-
 - **Automatic Operation Handling**: Mongotoy automates insertion and deletion management, ensuring data integrity 
 and consistency across related documents.
 
-
 - **Query Building**: Mongotoy provides a powerful query building interface for constructing complex queries using 
 Pythonic syntax.
 
-
 - **Index Management**: Mongotoy simplifies the management of database indexes, optimizing query performance for 
 efficient data retrieval.
 
-
 - **Transactions**: Supporting MongoDB transactions, Mongotoy ensures data consistency and atomicity across multiple
 operations within a single transactional context.
 
-
 - **Geospatial Data Support**: Mongotoy offers robust support for geospatial data types, facilitating storage, 
 querying, and spatial analysis.
 
-
 - **Database Seeding Management**: With built-in support for database seeding, Mongotoy streamlines the 
 initialization of databases with predefined data sets, enhancing developer productivity.
 
-
 - **Support for Capped Collections**: Mongotoy natively supports capped collections in MongoDB, ideal for 
 scenarios requiring fixed-size, ordered datasets.
 
-
 - **Time Series Collections Management**: Mongotoy provides robust support for managing time series data in 
 MongoDB, optimized for storing and querying time-stamped data points.
 
-
 - **GridFS File Handling**: Mongotoy seamlessly integrates with MongoDB's GridFS storage system for efficient
 handling of large files, offering a high-level interface for file management within MongoDB.
 
 ## Minimal Example
 Let's begin with a minimal example by defining a document and performing CRUD operations on the database.
 
 ```python
```

