# Comparing `tmp/psqlpy-0.5.2.tar.gz` & `tmp/psqlpy-0.5.3-pp38-pypy38_pp73-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

