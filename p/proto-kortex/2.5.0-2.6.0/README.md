# Comparing `tmp/proto_kortex-2.5.0.tar.gz` & `tmp/proto_kortex-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto_kortex-2.5.0.tar", max compression
+gzip compressed data, was "proto_kortex-2.6.0.tar", max compression
```

## Comparing `proto_kortex-2.5.0.tar` & `proto_kortex-2.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      431 2024-02-18 21:02:23.140752 proto_kortex-2.5.0/LICENSE.txt
--rw-r--r--   0        0        0      942 2024-02-18 21:02:23.140752 proto_kortex-2.5.0/README.md
--rw-r--r--   0        0        0       17 2024-02-18 21:06:19.109028 proto_kortex-2.5.0/gen/python/proto_kortex/hstp/__init__.py
--rw-r--r--   0        0        0       53 2024-02-18 21:06:19.109028 proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/__init__.py
--rw-r--r--   0        0        0    15630 2024-02-18 21:06:19.089027 proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.py
--rw-r--r--   0        0        0    18738 2024-02-18 21:06:19.089027 proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.pyi
--rw-r--r--   0        0        0    18524 2024-02-18 21:06:19.089027 proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/hstp_pb2_grpc.py
--rw-r--r--   0        0        0      414 2024-02-18 21:06:15.356839 proto_kortex-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 proto_kortex-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      431 2024-04-17 16:25:05.570873 proto_kortex-2.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      942 2024-04-17 16:25:05.570873 proto_kortex-2.6.0/README.md
+-rw-r--r--   0        0        0       17 2024-04-17 16:29:13.668443 proto_kortex-2.6.0/gen/python/proto_kortex/hstp/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-17 16:29:13.668443 proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/__init__.py
+-rw-r--r--   0        0        0    15679 2024-04-17 16:29:13.652443 proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.py
+-rw-r--r--   0        0        0    18777 2024-04-17 16:29:13.652443 proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.pyi
+-rw-r--r--   0        0        0    18524 2024-04-17 16:29:13.652443 proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/hstp_pb2_grpc.py
+-rw-r--r--   0        0        0      414 2024-04-17 16:29:10.468425 proto_kortex-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 proto_kortex-2.6.0/PKG-INFO
```

### Comparing `proto_kortex-2.5.0/README.md` & `proto_kortex-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.py` & `proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12hstp/v1/hstp.proto\x12\x07hstp.v1\"@\n\x11GetAuthUrlRequest\x12+\n\x08provider\x18\x01 \x01(\x0e\x32\x19.hstp.v1.IdentityProvider\"R\n\x08\x41uthInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x16\n\x0e\x63over_verifier\x18\x02 \x01(\t\x12\x12\n\ncsrf_token\x18\x03 \x01(\t\x12\r\n\x05nonce\x18\x04 \x01(\t\"m\n\x12GetAuthUrlResponse\x12&\n\tauth_info\x18\x01 \x01(\x0b\x32\x11.hstp.v1.AuthInfoH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"\x1e\n\x0e\x41rchiveRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"T\n\x0f\x41rchiveResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"@\n\x13\x42\x61tchArchiveRequest\x12)\n\x08requests\x18\x01 \x03(\x0b\x32\x17.hstp.v1.ArchiveRequest\"C\n\x14\x42\x61tchArchiveResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.hstp.v1.ArchiveResponse\"\x1b\n\x0bReadRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"Q\n\x0cReadResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\":\n\x10\x42\x61tchReadRequest\x12&\n\x08requests\x18\x01 \x03(\x0b\x32\x14.hstp.v1.ReadRequest\"=\n\x11\x42\x61tchReadResponse\x12(\n\tresponses\x18\x01 \x03(\x0b\x32\x15.hstp.v1.ReadResponse\"W\n\rUpsertRequest\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\x36\n\x12\x63ollision_strategy\x18\x02 \x01(\x0e\x32\x1a.hstp.v1.CollisionStrategy\"S\n\x0eUpsertResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\">\n\x12\x42\x61tchUpsertRequest\x12(\n\x08requests\x18\x01 \x03(\x0b\x32\x16.hstp.v1.UpsertRequest\"A\n\x13\x42\x61tchUpsertResponse\x12*\n\tresponses\x18\x01 \x03(\x0b\x32\x17.hstp.v1.UpsertResponse\"\x1e\n\x0eRestoreRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"T\n\x0fRestoreResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"@\n\x13\x42\x61tchRestoreRequest\x12)\n\x08requests\x18\x01 \x03(\x0b\x32\x17.hstp.v1.RestoreRequest\"C\n\x14\x42\x61tchRestoreResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.hstp.v1.RestoreResponse\"\x1c\n\x05Point\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\"m\n\x0eNearestRequest\x12\x0e\n\x04swid\x18\x01 \x01(\tH\x00\x12\x1f\n\x05point\x18\x02 \x01(\x0b\x32\x0e.hstp.v1.PointH\x00\x12\x12\n\nspace_swid\x18\x03 \x01(\t\x12\x0c\n\x04topk\x18\x04 \x01(\x04\x42\x08\n\x06target\"2\n\x0e\x45ntityDistance\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\x10\n\x08\x64istance\x18\x02 \x01(\x01\"?\n\x12\x45ntityDistanceList\x12)\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x17.hstp.v1.EntityDistance\"\x1e\n\nEntityList\x12\x10\n\x08\x65ntities\x18\x01 \x03(\t\"\xa8\x01\n\x0fNearestResponse\x12+\n\x08\x65ntities\x18\x01 \x01(\x0b\x32\x13.hstp.v1.EntityListB\x02\x18\x01H\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x12\x37\n\x10\x65ntity_distances\x18\x03 \x01(\x0b\x32\x1b.hstp.v1.EntityDistanceListH\x00\x42\n\n\x08response\"@\n\x13\x42\x61tchNearestRequest\x12)\n\x08requests\x18\x01 \x03(\x0b\x32\x17.hstp.v1.NearestRequest\"C\n\x14\x42\x61tchNearestResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.hstp.v1.NearestResponse\"@\n\rListenRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\x12!\n\x04type\x18\x02 \x01(\x0e\x32\x13.hstp.v1.ListenType\"\xae\x01\n\x0eListenResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x12%\n\x04type\x18\x03 \x01(\x0e\x32\x13.hstp.v1.ListenTypeB\x02\x18\x01\x12\x32\n\rresponse_type\x18\x04 \x01(\x0e\x32\x1b.hstp.v1.ListenResponseTypeB\n\n\x08response\">\n\x12\x42\x61tchListenRequest\x12(\n\x08requests\x18\x01 \x03(\x0b\x32\x16.hstp.v1.ListenRequest\"A\n\x13\x42\x61tchListenResponse\x12*\n\tresponses\x18\x01 \x03(\x0b\x32\x17.hstp.v1.ListenResponse\"\x1c\n\x0cLinksRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"a\n\rLinksResponse\x12\x1f\n\x05links\x18\x01 \x01(\x0b\x32\x0e.hstp.v1.LinksH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"<\n\x11\x42\x61tchLinksRequest\x12\'\n\x08requests\x18\x01 \x03(\x0b\x32\x15.hstp.v1.LinksRequest\"?\n\x12\x42\x61tchLinksResponse\x12)\n\tresponses\x18\x01 \x03(\x0b\x32\x16.hstp.v1.LinksResponse\"X\n\rIngestRequest\x12$\n\x07\x64octype\x18\x01 \x01(\x0e\x32\x13.hstp.v1.IngestType\x12\x10\n\x08\x64ocument\x18\x02 \x01(\t\x12\x0f\n\x07\x64ry_run\x18\x03 \x01(\x08\"A\n\rIngestSuccess\x12\x16\n\x0eingested_swids\x18\x01 \x03(\t\x12\x18\n\x10ingested_schemas\x18\x02 \x03(\t\"H\n\x13IngestDryRunSuccess\x12\x16\n\x0eprocessed_data\x18\x01 \x03(\t\x12\x19\n\x11generated_schemas\x18\x02 \x03(\t\"\xa5\x01\n\x0eIngestResponse\x12)\n\x07success\x18\x01 \x01(\x0b\x32\x16.hstp.v1.IngestSuccessH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x12\x37\n\x0f\x64ry_run_success\x18\x03 \x01(\x0b\x32\x1c.hstp.v1.IngestDryRunSuccessH\x00\x42\n\n\x08response\"\x1d\n\x0cQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"R\n\rQueryResponse\x12\x10\n\x06result\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"\"\n\x11ParseQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"^\n\x12ParseQueryResponse\x12\x17\n\rresponse_type\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"\x8d\x01\n\x05Links\x12\x0c\n\x04swid\x18\x01 \x01(\t\x12:\n\x1blinks_with_this_swid_as_dst\x18\x02 \x03(\x0b\x32\x15.hstp.v1.ReadResponse\x12:\n\x1blinks_with_this_swid_as_src\x18\x03 \x03(\x0b\x32\x15.hstp.v1.ReadResponse\"\x1c\n\x08\x45ntities\x12\x10\n\x08\x65ntities\x18\x01 \x03(\t\"L\n\tHSTPError\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.hstp.v1.ErrorCode\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0c\n\x04swid\x18\x03 \x01(\t*\x88\x01\n\nListenType\x12\x14\n\x10LISTEN_TYPE_NONE\x10\x00\x12\x13\n\x0fLISTEN_TYPE_ADD\x10\x01\x12\x16\n\x12LISTEN_TYPE_REMOVE\x10\x02\x12\x19\n\x15LISTEN_TYPE_LINKS_ADD\x10\x03\x12\x1c\n\x18LISTEN_TYPE_LINKS_REMOVE\x10\x04*\x8d\x02\n\x12ListenResponseType\x12\x1d\n\x19LISTEN_RESPONSE_TYPE_NONE\x10\x00\x12\x1e\n\x1aLISTEN_RESPONSE_TYPE_ADDED\x10\x01\x12 \n\x1cLISTEN_RESPONSE_TYPE_REMOVED\x10\x02\x12 \n\x1cLISTEN_RESPONSE_TYPE_UPDATED\x10\x03\x12$\n LISTEN_RESPONSE_TYPE_LINKS_ADDED\x10\x04\x12&\n\"LISTEN_RESPONSE_TYPE_LINKS_REMOVED\x10\x05\x12&\n\"LISTEN_RESPONSE_TYPE_LINKS_UPDATED\x10\x06*\xb5\x01\n\x11\x43ollisionStrategy\x12\x1b\n\x17\x43OLLISION_STRATEGY_NONE\x10\x00\x12\x1b\n\x17\x43OLLISION_STRATEGY_FAIL\x10\x01\x12\x1c\n\x18\x43OLLISION_STRATEGY_MERGE\x10\x02\x12 \n\x1c\x43OLLISION_STRATEGY_OVERWRITE\x10\x03\x12&\n\"COLLISION_STRATEGY_FORCE_OVERWRITE\x10\x04*M\n\nIngestType\x12\x14\n\x10INGEST_TYPE_NONE\x10\x00\x12\x14\n\x10INGEST_TYPE_JSON\x10\x01\x12\x13\n\x0fINGEST_TYPE_CSV\x10\x02*\xb9\x08\n\tErrorCode\x12\x13\n\x0f\x45RROR_CODE_NONE\x10\x00\x12\x1f\n\x1b\x45RROR_CODE_MISSING_PROPERTY\x10\x01\x12 \n\x1c\x45RROR_CODE_SCHEMA_VALIDATION\x10\x02\x12\x1f\n\x1b\x45RROR_CODE_ENTITY_NOT_FOUND\x10\x03\x12\x1d\n\x19\x45RROR_CODE_INVALID_ENTITY\x10\x04\x12\x1b\n\x17\x45RROR_CODE_IMMUDB_ERROR\x10\x05\x12!\n\x1d\x45RROR_CODE_ENTITY_PARSE_ERROR\x10\x06\x12%\n!ERROR_CODE_ENTITY_SERIALIZE_ERROR\x10\x07\x12\x1f\n\x1b\x45RROR_CODE_UPSERT_COLLISION\x10\x08\x12 \n\x1c\x45RROR_CODE_PARSE_QUERY_ERROR\x10\t\x12\'\n#ERROR_CODE_QUERY_DIMENSION_MISMATCH\x10\n\x12\x1e\n\x1a\x45RROR_CODE_NOT_IMPLEMENTED\x10\x0b\x12\x1e\n\x1a\x45RROR_CODE_UNHANDLED_ERROR\x10\x0c\x12 \n\x1c\x45RROR_CODE_LINKS_PARSE_ERROR\x10\r\x12-\n)ERROR_CODE_EMBEDDED_PROGRAM_EXECUTE_ERROR\x10\x0e\x12%\n!ERROR_CODE_SCHEMA_EMBEDDING_ERROR\x10\x0f\x12\x1c\n\x18\x45RROR_CODE_COZO_DB_ERROR\x10\x10\x12#\n\x1f\x45RROR_CODE_CANNOT_UPDATE_SCHEMA\x10\x11\x12\x1c\n\x18\x45RROR_CODE_ROCKSDB_ERROR\x10\x12\x12\x1d\n\x19\x45RROR_CODE_FASTTEXT_ERROR\x10\x13\x12\'\n#ERROR_CODE_INSUFFICIENT_PERMISSIONS\x10\x14\x12\x1a\n\x16\x45RROR_CODE_NOT_ALLOWED\x10\x15\x12\x1f\n\x1b\x45RROR_CODE_CSV_INGEST_ERROR\x10\x16\x12\'\n#ERROR_CODE_INVALID_HSQL_INSTRUCTION\x10\x17\x12\x1f\n\x1b\x45RROR_CODE_INVALID_OPERATOR\x10\x18\x12\x1f\n\x1b\x45RROR_CODE_ENTITY_COLLISION\x10\x19\x12\x1a\n\x16\x45RROR_CODE_CLOCK_ERROR\x10\x1a\x12\x1c\n\x18\x45RROR_CODE_TOKEN_EXPIRED\x10\x1b\x12\x1e\n\x1a\x45RROR_CODE_JWT_PARSE_ERROR\x10\x1c\x12\x1c\n\x18\x45RROR_CODE_JWT_NO_KEY_ID\x10\x1d\x12\x1f\n\x1b\x45RROR_CODE_JWT_NO_KEY_MATCH\x10\x1e\x12\x1f\n\x1b\x45RROR_CODE_JWT_DECODE_ERROR\x10\x1f*\xba\x02\n\x10IdentityProvider\x12\x1a\n\x16IDENTITY_PROVIDER_NONE\x10\x00\x12\x1b\n\x17IDENTITY_PROVIDER_AUTH0\x10\x01\x12\x1c\n\x18IDENTITY_PROVIDER_GOOGLE\x10\x02\x12\x1f\n\x1bIDENTITY_PROVIDER_MICROSOFT\x10\x03\x12\x1a\n\x16IDENTITY_PROVIDER_OKTA\x10\x04\x12\x1e\n\x1aIDENTITY_PROVIDER_FACEBOOK\x10\x05\x12\x1c\n\x18IDENTITY_PROVIDER_GITHUB\x10\x06\x12\x17\n\x13IDENTITY_PROVIDER_X\x10\x07\x12\x1e\n\x1aIDENTITY_PROVIDER_LINKEDIN\x10\x08\x12\x1b\n\x17IDENTITY_PROVIDER_APPLE\x10\t2\xb1\x06\n\x0bHSTPService\x12J\n\nGetAuthUrl\x12\x1a.hstp.v1.GetAuthUrlRequest\x1a\x1b.hstp.v1.GetAuthUrlResponse\"\x03\x88\x02\x01\x12\x44\n\tBatchRead\x12\x19.hstp.v1.BatchReadRequest\x1a\x1a.hstp.v1.BatchReadResponse\"\x00\x12J\n\x0b\x42\x61tchUpsert\x12\x1b.hstp.v1.BatchUpsertRequest\x1a\x1c.hstp.v1.BatchUpsertResponse\"\x00\x12M\n\x0c\x42\x61tchArchive\x12\x1c.hstp.v1.BatchArchiveRequest\x1a\x1d.hstp.v1.BatchArchiveResponse\"\x00\x12M\n\x0c\x42\x61tchRestore\x12\x1c.hstp.v1.BatchRestoreRequest\x1a\x1d.hstp.v1.BatchRestoreResponse\"\x00\x12M\n\x0c\x42\x61tchNearest\x12\x1c.hstp.v1.BatchNearestRequest\x1a\x1d.hstp.v1.BatchNearestResponse\"\x00\x12N\n\x0b\x42\x61tchListen\x12\x1b.hstp.v1.BatchListenRequest\x1a\x1c.hstp.v1.BatchListenResponse\"\x00(\x01\x30\x01\x12G\n\nBatchLinks\x12\x1a.hstp.v1.BatchLinksRequest\x1a\x1b.hstp.v1.BatchLinksResponse\"\x00\x12;\n\x06Ingest\x12\x16.hstp.v1.IngestRequest\x1a\x17.hstp.v1.IngestResponse\"\x00\x12\x38\n\x05Query\x12\x15.hstp.v1.QueryRequest\x1a\x16.hstp.v1.QueryResponse\"\x00\x12G\n\nParseQuery\x12\x1a.hstp.v1.ParseQueryRequest\x1a\x1b.hstp.v1.ParseQueryResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12hstp/v1/hstp.proto\x12\x07hstp.v1\"@\n\x11GetAuthUrlRequest\x12+\n\x08provider\x18\x01 \x01(\x0e\x32\x19.hstp.v1.IdentityProvider\"R\n\x08\x41uthInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x16\n\x0e\x63over_verifier\x18\x02 \x01(\t\x12\x12\n\ncsrf_token\x18\x03 \x01(\t\x12\r\n\x05nonce\x18\x04 \x01(\t\"m\n\x12GetAuthUrlResponse\x12&\n\tauth_info\x18\x01 \x01(\x0b\x32\x11.hstp.v1.AuthInfoH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"\x1e\n\x0e\x41rchiveRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"T\n\x0f\x41rchiveResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"@\n\x13\x42\x61tchArchiveRequest\x12)\n\x08requests\x18\x01 \x03(\x0b\x32\x17.hstp.v1.ArchiveRequest\"C\n\x14\x42\x61tchArchiveResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.hstp.v1.ArchiveResponse\"\x1b\n\x0bReadRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"Q\n\x0cReadResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\":\n\x10\x42\x61tchReadRequest\x12&\n\x08requests\x18\x01 \x03(\x0b\x32\x14.hstp.v1.ReadRequest\"=\n\x11\x42\x61tchReadResponse\x12(\n\tresponses\x18\x01 \x03(\x0b\x32\x15.hstp.v1.ReadResponse\"W\n\rUpsertRequest\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\x36\n\x12\x63ollision_strategy\x18\x02 \x01(\x0e\x32\x1a.hstp.v1.CollisionStrategy\"S\n\x0eUpsertResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\">\n\x12\x42\x61tchUpsertRequest\x12(\n\x08requests\x18\x01 \x03(\x0b\x32\x16.hstp.v1.UpsertRequest\"A\n\x13\x42\x61tchUpsertResponse\x12*\n\tresponses\x18\x01 \x03(\x0b\x32\x17.hstp.v1.UpsertResponse\"\x1e\n\x0eRestoreRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"T\n\x0fRestoreResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"@\n\x13\x42\x61tchRestoreRequest\x12)\n\x08requests\x18\x01 \x03(\x0b\x32\x17.hstp.v1.RestoreRequest\"C\n\x14\x42\x61tchRestoreResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.hstp.v1.RestoreResponse\"\x1c\n\x05Point\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\"m\n\x0eNearestRequest\x12\x0e\n\x04swid\x18\x01 \x01(\tH\x00\x12\x1f\n\x05point\x18\x02 \x01(\x0b\x32\x0e.hstp.v1.PointH\x00\x12\x12\n\nspace_swid\x18\x03 \x01(\t\x12\x0c\n\x04topk\x18\x04 \x01(\x04\x42\x08\n\x06target\"2\n\x0e\x45ntityDistance\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\x10\n\x08\x64istance\x18\x02 \x01(\x01\"?\n\x12\x45ntityDistanceList\x12)\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x17.hstp.v1.EntityDistance\"\x1e\n\nEntityList\x12\x10\n\x08\x65ntities\x18\x01 \x03(\t\"\xa8\x01\n\x0fNearestResponse\x12+\n\x08\x65ntities\x18\x01 \x01(\x0b\x32\x13.hstp.v1.EntityListB\x02\x18\x01H\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x12\x37\n\x10\x65ntity_distances\x18\x03 \x01(\x0b\x32\x1b.hstp.v1.EntityDistanceListH\x00\x42\n\n\x08response\"@\n\x13\x42\x61tchNearestRequest\x12)\n\x08requests\x18\x01 \x03(\x0b\x32\x17.hstp.v1.NearestRequest\"C\n\x14\x42\x61tchNearestResponse\x12+\n\tresponses\x18\x01 \x03(\x0b\x32\x18.hstp.v1.NearestResponse\"@\n\rListenRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\x12!\n\x04type\x18\x02 \x01(\x0e\x32\x13.hstp.v1.ListenType\"\xae\x01\n\x0eListenResponse\x12\x10\n\x06\x65ntity\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x12%\n\x04type\x18\x03 \x01(\x0e\x32\x13.hstp.v1.ListenTypeB\x02\x18\x01\x12\x32\n\rresponse_type\x18\x04 \x01(\x0e\x32\x1b.hstp.v1.ListenResponseTypeB\n\n\x08response\">\n\x12\x42\x61tchListenRequest\x12(\n\x08requests\x18\x01 \x03(\x0b\x32\x16.hstp.v1.ListenRequest\"A\n\x13\x42\x61tchListenResponse\x12*\n\tresponses\x18\x01 \x03(\x0b\x32\x17.hstp.v1.ListenResponse\"\x1c\n\x0cLinksRequest\x12\x0c\n\x04swid\x18\x01 \x01(\t\"a\n\rLinksResponse\x12\x1f\n\x05links\x18\x01 \x01(\x0b\x32\x0e.hstp.v1.LinksH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"<\n\x11\x42\x61tchLinksRequest\x12\'\n\x08requests\x18\x01 \x03(\x0b\x32\x15.hstp.v1.LinksRequest\"?\n\x12\x42\x61tchLinksResponse\x12)\n\tresponses\x18\x01 \x03(\x0b\x32\x16.hstp.v1.LinksResponse\"X\n\rIngestRequest\x12$\n\x07\x64octype\x18\x01 \x01(\x0e\x32\x13.hstp.v1.IngestType\x12\x10\n\x08\x64ocument\x18\x02 \x01(\t\x12\x0f\n\x07\x64ry_run\x18\x03 \x01(\x08\"A\n\rIngestSuccess\x12\x16\n\x0eingested_swids\x18\x01 \x03(\t\x12\x18\n\x10ingested_schemas\x18\x02 \x03(\t\"H\n\x13IngestDryRunSuccess\x12\x16\n\x0eprocessed_data\x18\x01 \x03(\t\x12\x19\n\x11generated_schemas\x18\x02 \x03(\t\"\xa5\x01\n\x0eIngestResponse\x12)\n\x07success\x18\x01 \x01(\x0b\x32\x16.hstp.v1.IngestSuccessH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x12\x37\n\x0f\x64ry_run_success\x18\x03 \x01(\x0b\x32\x1c.hstp.v1.IngestDryRunSuccessH\x00\x42\n\n\x08response\"\x1d\n\x0cQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"R\n\rQueryResponse\x12\x10\n\x06result\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"\"\n\x11ParseQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"^\n\x12ParseQueryResponse\x12\x17\n\rresponse_type\x18\x01 \x01(\tH\x00\x12#\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.hstp.v1.HSTPErrorH\x00\x42\n\n\x08response\"\x8d\x01\n\x05Links\x12\x0c\n\x04swid\x18\x01 \x01(\t\x12:\n\x1blinks_with_this_swid_as_dst\x18\x02 \x03(\x0b\x32\x15.hstp.v1.ReadResponse\x12:\n\x1blinks_with_this_swid_as_src\x18\x03 \x03(\x0b\x32\x15.hstp.v1.ReadResponse\"\x1c\n\x08\x45ntities\x12\x10\n\x08\x65ntities\x18\x01 \x03(\t\"L\n\tHSTPError\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.hstp.v1.ErrorCode\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0c\n\x04swid\x18\x03 \x01(\t*\x88\x01\n\nListenType\x12\x14\n\x10LISTEN_TYPE_NONE\x10\x00\x12\x13\n\x0fLISTEN_TYPE_ADD\x10\x01\x12\x16\n\x12LISTEN_TYPE_REMOVE\x10\x02\x12\x19\n\x15LISTEN_TYPE_LINKS_ADD\x10\x03\x12\x1c\n\x18LISTEN_TYPE_LINKS_REMOVE\x10\x04*\x8d\x02\n\x12ListenResponseType\x12\x1d\n\x19LISTEN_RESPONSE_TYPE_NONE\x10\x00\x12\x1e\n\x1aLISTEN_RESPONSE_TYPE_ADDED\x10\x01\x12 \n\x1cLISTEN_RESPONSE_TYPE_REMOVED\x10\x02\x12 \n\x1cLISTEN_RESPONSE_TYPE_UPDATED\x10\x03\x12$\n LISTEN_RESPONSE_TYPE_LINKS_ADDED\x10\x04\x12&\n\"LISTEN_RESPONSE_TYPE_LINKS_REMOVED\x10\x05\x12&\n\"LISTEN_RESPONSE_TYPE_LINKS_UPDATED\x10\x06*\xb5\x01\n\x11\x43ollisionStrategy\x12\x1b\n\x17\x43OLLISION_STRATEGY_NONE\x10\x00\x12\x1b\n\x17\x43OLLISION_STRATEGY_FAIL\x10\x01\x12\x1c\n\x18\x43OLLISION_STRATEGY_MERGE\x10\x02\x12 \n\x1c\x43OLLISION_STRATEGY_OVERWRITE\x10\x03\x12&\n\"COLLISION_STRATEGY_FORCE_OVERWRITE\x10\x04*M\n\nIngestType\x12\x14\n\x10INGEST_TYPE_NONE\x10\x00\x12\x14\n\x10INGEST_TYPE_JSON\x10\x01\x12\x13\n\x0fINGEST_TYPE_CSV\x10\x02*\xda\x08\n\tErrorCode\x12\x13\n\x0f\x45RROR_CODE_NONE\x10\x00\x12\x1f\n\x1b\x45RROR_CODE_MISSING_PROPERTY\x10\x01\x12 \n\x1c\x45RROR_CODE_SCHEMA_VALIDATION\x10\x02\x12\x1f\n\x1b\x45RROR_CODE_ENTITY_NOT_FOUND\x10\x03\x12\x1d\n\x19\x45RROR_CODE_INVALID_ENTITY\x10\x04\x12\x1b\n\x17\x45RROR_CODE_IMMUDB_ERROR\x10\x05\x12!\n\x1d\x45RROR_CODE_ENTITY_PARSE_ERROR\x10\x06\x12%\n!ERROR_CODE_ENTITY_SERIALIZE_ERROR\x10\x07\x12\x1f\n\x1b\x45RROR_CODE_UPSERT_COLLISION\x10\x08\x12 \n\x1c\x45RROR_CODE_PARSE_QUERY_ERROR\x10\t\x12\'\n#ERROR_CODE_QUERY_DIMENSION_MISMATCH\x10\n\x12\x1e\n\x1a\x45RROR_CODE_NOT_IMPLEMENTED\x10\x0b\x12\x1e\n\x1a\x45RROR_CODE_UNHANDLED_ERROR\x10\x0c\x12 \n\x1c\x45RROR_CODE_LINKS_PARSE_ERROR\x10\r\x12-\n)ERROR_CODE_EMBEDDED_PROGRAM_EXECUTE_ERROR\x10\x0e\x12%\n!ERROR_CODE_SCHEMA_EMBEDDING_ERROR\x10\x0f\x12\x1c\n\x18\x45RROR_CODE_COZO_DB_ERROR\x10\x10\x12#\n\x1f\x45RROR_CODE_CANNOT_UPDATE_SCHEMA\x10\x11\x12\x1c\n\x18\x45RROR_CODE_ROCKSDB_ERROR\x10\x12\x12\x1d\n\x19\x45RROR_CODE_FASTTEXT_ERROR\x10\x13\x12\'\n#ERROR_CODE_INSUFFICIENT_PERMISSIONS\x10\x14\x12\x1a\n\x16\x45RROR_CODE_NOT_ALLOWED\x10\x15\x12\x1f\n\x1b\x45RROR_CODE_CSV_INGEST_ERROR\x10\x16\x12\'\n#ERROR_CODE_INVALID_HSQL_INSTRUCTION\x10\x17\x12\x1f\n\x1b\x45RROR_CODE_INVALID_OPERATOR\x10\x18\x12\x1f\n\x1b\x45RROR_CODE_ENTITY_COLLISION\x10\x19\x12\x1a\n\x16\x45RROR_CODE_CLOCK_ERROR\x10\x1a\x12\x1c\n\x18\x45RROR_CODE_TOKEN_EXPIRED\x10\x1b\x12\x1e\n\x1a\x45RROR_CODE_JWT_PARSE_ERROR\x10\x1c\x12\x1c\n\x18\x45RROR_CODE_JWT_NO_KEY_ID\x10\x1d\x12\x1f\n\x1b\x45RROR_CODE_JWT_NO_KEY_MATCH\x10\x1e\x12\x1f\n\x1b\x45RROR_CODE_JWT_DECODE_ERROR\x10\x1f\x12\x1f\n\x1b\x45RROR_CODE_DUPLICATE_FACTOR\x10 *\xba\x02\n\x10IdentityProvider\x12\x1a\n\x16IDENTITY_PROVIDER_NONE\x10\x00\x12\x1b\n\x17IDENTITY_PROVIDER_AUTH0\x10\x01\x12\x1c\n\x18IDENTITY_PROVIDER_GOOGLE\x10\x02\x12\x1f\n\x1bIDENTITY_PROVIDER_MICROSOFT\x10\x03\x12\x1a\n\x16IDENTITY_PROVIDER_OKTA\x10\x04\x12\x1e\n\x1aIDENTITY_PROVIDER_FACEBOOK\x10\x05\x12\x1c\n\x18IDENTITY_PROVIDER_GITHUB\x10\x06\x12\x17\n\x13IDENTITY_PROVIDER_X\x10\x07\x12\x1e\n\x1aIDENTITY_PROVIDER_LINKEDIN\x10\x08\x12\x1b\n\x17IDENTITY_PROVIDER_APPLE\x10\t2\xb1\x06\n\x0bHSTPService\x12J\n\nGetAuthUrl\x12\x1a.hstp.v1.GetAuthUrlRequest\x1a\x1b.hstp.v1.GetAuthUrlResponse\"\x03\x88\x02\x01\x12\x44\n\tBatchRead\x12\x19.hstp.v1.BatchReadRequest\x1a\x1a.hstp.v1.BatchReadResponse\"\x00\x12J\n\x0b\x42\x61tchUpsert\x12\x1b.hstp.v1.BatchUpsertRequest\x1a\x1c.hstp.v1.BatchUpsertResponse\"\x00\x12M\n\x0c\x42\x61tchArchive\x12\x1c.hstp.v1.BatchArchiveRequest\x1a\x1d.hstp.v1.BatchArchiveResponse\"\x00\x12M\n\x0c\x42\x61tchRestore\x12\x1c.hstp.v1.BatchRestoreRequest\x1a\x1d.hstp.v1.BatchRestoreResponse\"\x00\x12M\n\x0c\x42\x61tchNearest\x12\x1c.hstp.v1.BatchNearestRequest\x1a\x1d.hstp.v1.BatchNearestResponse\"\x00\x12N\n\x0b\x42\x61tchListen\x12\x1b.hstp.v1.BatchListenRequest\x1a\x1c.hstp.v1.BatchListenResponse\"\x00(\x01\x30\x01\x12G\n\nBatchLinks\x12\x1a.hstp.v1.BatchLinksRequest\x1a\x1b.hstp.v1.BatchLinksResponse\"\x00\x12;\n\x06Ingest\x12\x16.hstp.v1.IngestRequest\x1a\x17.hstp.v1.IngestResponse\"\x00\x12\x38\n\x05Query\x12\x15.hstp.v1.QueryRequest\x1a\x16.hstp.v1.QueryResponse\"\x00\x12G\n\nParseQuery\x12\x1a.hstp.v1.ParseQueryRequest\x1a\x1b.hstp.v1.ParseQueryResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'hstp.v1.hstp_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _NEARESTRESPONSE.fields_by_name['entities']._options = None
@@ -31,17 +31,17 @@
   _LISTENRESPONSETYPE._serialized_start=3602
   _LISTENRESPONSETYPE._serialized_end=3871
   _COLLISIONSTRATEGY._serialized_start=3874
   _COLLISIONSTRATEGY._serialized_end=4055
   _INGESTTYPE._serialized_start=4057
   _INGESTTYPE._serialized_end=4134
   _ERRORCODE._serialized_start=4137
-  _ERRORCODE._serialized_end=5218
-  _IDENTITYPROVIDER._serialized_start=5221
-  _IDENTITYPROVIDER._serialized_end=5535
+  _ERRORCODE._serialized_end=5251
+  _IDENTITYPROVIDER._serialized_start=5254
+  _IDENTITYPROVIDER._serialized_end=5568
   _GETAUTHURLREQUEST._serialized_start=31
   _GETAUTHURLREQUEST._serialized_end=95
   _AUTHINFO._serialized_start=97
   _AUTHINFO._serialized_end=179
   _GETAUTHURLRESPONSE._serialized_start=181
   _GETAUTHURLRESPONSE._serialized_end=290
   _ARCHIVEREQUEST._serialized_start=292
@@ -126,10 +126,10 @@
   _PARSEQUERYRESPONSE._serialized_end=3208
   _LINKS._serialized_start=3211
   _LINKS._serialized_end=3352
   _ENTITIES._serialized_start=3354
   _ENTITIES._serialized_end=3382
   _HSTPERROR._serialized_start=3384
   _HSTPERROR._serialized_end=3460
-  _HSTPSERVICE._serialized_start=5538
-  _HSTPSERVICE._serialized_end=6355
+  _HSTPSERVICE._serialized_start=5571
+  _HSTPSERVICE._serialized_end=6388
 # @@protoc_insertion_point(module_scope)
```

### Comparing `proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.pyi` & `proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/hstp_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 COLLISION_STRATEGY_NONE: CollisionStrategy
 COLLISION_STRATEGY_OVERWRITE: CollisionStrategy
 DESCRIPTOR: _descriptor.FileDescriptor
 ERROR_CODE_CANNOT_UPDATE_SCHEMA: ErrorCode
 ERROR_CODE_CLOCK_ERROR: ErrorCode
 ERROR_CODE_COZO_DB_ERROR: ErrorCode
 ERROR_CODE_CSV_INGEST_ERROR: ErrorCode
+ERROR_CODE_DUPLICATE_FACTOR: ErrorCode
 ERROR_CODE_EMBEDDED_PROGRAM_EXECUTE_ERROR: ErrorCode
 ERROR_CODE_ENTITY_COLLISION: ErrorCode
 ERROR_CODE_ENTITY_NOT_FOUND: ErrorCode
 ERROR_CODE_ENTITY_PARSE_ERROR: ErrorCode
 ERROR_CODE_ENTITY_SERIALIZE_ERROR: ErrorCode
 ERROR_CODE_FASTTEXT_ERROR: ErrorCode
 ERROR_CODE_IMMUDB_ERROR: ErrorCode
```

### Comparing `proto_kortex-2.5.0/gen/python/proto_kortex/hstp/v1/hstp_pb2_grpc.py` & `proto_kortex-2.6.0/gen/python/proto_kortex/hstp/v1/hstp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `proto_kortex-2.5.0/PKG-INFO` & `proto_kortex-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proto-kortex
-Version: 2.5.0
+Version: 2.6.0
 Summary: 
 Author: VERSES AI
 Author-email: engineering@verses.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

