# Comparing `tmp/pypolyclip-1.0.1.tar.gz` & `tmp/pypolyclip-1.1.0-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypolyclip-1.0.1.tar", last modified: Thu Nov 16 20:51:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

