# Comparing `tmp/fluidimage-0.4.4.tar.gz` & `tmp/fluidimage-0.4.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidimage-0.4.4.tar", last modified: Tue Apr 16 10:07:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

