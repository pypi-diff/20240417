# Comparing `tmp/libfwevt-python-20240101.tar.gz` & `tmp/libfwevt_python-20240416-cp38-cp38-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwevt-python-20240101.tar", last modified: Mon Jan  1 05:22:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

