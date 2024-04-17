# Comparing `tmp/lightning-pose-1.2.3.tar.gz` & `tmp/lightning_pose-1.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-pose-1.2.3.tar", last modified: Thu Apr  4 18:45:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

