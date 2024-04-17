# Comparing `tmp/openlane-2.0.0rc2.tar.gz` & `tmp/openlane-2.0.0rc3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.0rc2.tar", last modified: Sun Apr  7 19:01:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

