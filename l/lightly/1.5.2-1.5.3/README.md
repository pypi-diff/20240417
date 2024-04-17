# Comparing `tmp/lightly-1.5.2.tar.gz` & `tmp/lightly-1.5.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.5.2.tar", last modified: Tue Mar 26 13:01:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

