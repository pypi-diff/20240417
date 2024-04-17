# Comparing `tmp/legal_citation_parser-0.2.1.tar.gz` & `tmp/legal_citation_parser-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.2.1.tar", last modified: Thu Apr 11 01:10:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

