# Comparing `tmp/apt-wrapper-1.18.tar.gz` & `tmp/apt_wrapper-1.19-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apt-wrapper-1.18.tar", last modified: Mon Jul  6 22:14:03 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

