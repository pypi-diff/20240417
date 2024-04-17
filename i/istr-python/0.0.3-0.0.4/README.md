# Comparing `tmp/istr_python-0.0.3.tar.gz` & `tmp/istr_python-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.0.3.tar", last modified: Wed Apr 17 07:18:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

