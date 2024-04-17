# Comparing `tmp/gdstk-0.9.50.tar.gz` & `tmp/gdstk-0.9.51-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdstk-0.9.50.tar", last modified: Wed Feb  7 18:27:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

