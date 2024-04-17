# Comparing `tmp/loristrck-1.6.1.tar.gz` & `tmp/loristrck-1.6.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loristrck-1.6.1.tar", last modified: Thu Feb 15 12:11:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

