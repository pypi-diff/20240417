# Comparing `tmp/cysgp4-0.3.5.tar.gz` & `tmp/cysgp4-0.3.6-cp38-cp38-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cysgp4-0.3.5.tar", last modified: Sat Nov 19 22:24:58 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

