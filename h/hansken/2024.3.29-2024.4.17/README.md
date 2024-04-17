# Comparing `tmp/hansken-2024.3.29.tar.gz` & `tmp/hansken-2024.4.17-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hansken-2024.3.29.tar", last modified: Fri Mar 29 10:18:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

