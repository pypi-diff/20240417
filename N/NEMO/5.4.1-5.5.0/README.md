# Comparing `tmp/NEMO-5.4.1.tar.gz` & `tmp/NEMO-5.5.0-py36-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-5.4.1.tar", last modified: Thu Apr  4 15:56:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

