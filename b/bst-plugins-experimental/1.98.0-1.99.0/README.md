# Comparing `tmp/bst-plugins-experimental-1.98.0.tar.gz` & `tmp/bst_plugins_experimental-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bst-plugins-experimental-1.98.0.tar", last modified: Sun Feb  4 17:33:43 2024, max compression
+gzip compressed data, was "bst_plugins_experimental-1.99.0.tar", last modified: Wed Apr 17 09:25:56 2024, max compression
```

## Comparing `bst-plugins-experimental-1.98.0.tar` & `bst_plugins_experimental-1.99.0.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.914830 bst-plugins-experimental-1.98.0/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/LICENSE
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/MANIFEST.in
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-02-04 17:33:43.913830 bst-plugins-experimental-1.98.0/PKG-INFO
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/README.rst
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      759 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/project.conf
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2731 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/pyproject.toml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.899830 bst-plugins-experimental-1.98.0/requirements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      205 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/requirements/plugin-requirements.txt
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/requirements/test-requirements.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       38 2024-02-04 17:33:43.914830 bst-plugins-experimental-1.98.0/setup.cfg
--rwxrwxrwx   0 testuser  (1000) testuser  (1000)       61 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/setup.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.896830 bst-plugins-experimental-1.98.0/src/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.899830 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.908830 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazel_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazel_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11344 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazelize.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazelize.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2149 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/check_forbidden.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/collect_integration.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11776 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/collect_manifest.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_deploy.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_bootimg.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_ext4.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4630 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/flatpak_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/flatpak_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/flatpak_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/flatpak_repo.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/makemaker.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/makemaker.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/modulebuild.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1084 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/modulebuild.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/oci.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/pyproject.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/pyproject.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/qmake.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/qmake.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2841 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/snap_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/snap_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/tar_element.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/tar_element.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/x86image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/x86image.yaml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.911830 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4728 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/_utils.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13074 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/bazel_source.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4025 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/cpan.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/deb.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/git_module.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    17442 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/git_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35320 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/git_tag.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/ostree.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2512 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/patch_queue.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5581 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/pypi.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/quilt.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/zip.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.911830 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.912830 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/gitrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/tarrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2024-02-04 17:33:28.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/ziprepo.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.913830 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-02-04 17:33:43.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3375 2024-02-04 17:33:43.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2024-02-04 17:33:43.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)     1806 2024-02-04 17:33:43.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2024-02-04 17:33:43.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/requires.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2024-02-04 17:33:43.000000 bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/top_level.txt
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.897830 bst-plugins-experimental-1.98.0/venv/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.897830 bst-plugins-experimental-1.98.0/venv/lib/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.897830 bst-plugins-experimental-1.98.0/venv/lib/python3.11/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.897830 bst-plugins-experimental-1.98.0/venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-02-04 17:33:43.912830 bst-plugins-experimental-1.98.0/venv/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2024-02-04 17:33:37.000000 bst-plugins-experimental-1.98.0/venv/lib/python3.11/site-packages/markdown_it/port.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.436927 bst_plugins_experimental-1.99.0/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/LICENSE
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/MANIFEST.in
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-17 09:25:56.436927 bst_plugins_experimental-1.99.0/PKG-INFO
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/README.rst
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      773 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/project.conf
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2731 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/pyproject.toml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.420927 bst_plugins_experimental-1.99.0/requirements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      213 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/requirements/plugin-requirements.txt
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/requirements/test-requirements.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       38 2024-04-17 09:25:56.436927 bst_plugins_experimental-1.99.0/setup.cfg
+-rwxrwxrwx   0 testuser  (1000) testuser  (1000)       61 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/setup.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.417927 bst_plugins_experimental-1.99.0/src/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.421927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.430927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11344 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazelize.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazelize.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2149 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/check_forbidden.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_integration.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10889 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_manifest.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7669 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1084 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/oci.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/pyproject.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/pyproject.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2895 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/snap_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/snap_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/tar_element.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/tar_element.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.433927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    15419 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_git_utils.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6386 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_utils.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13073 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/bazel_source.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4025 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/cpan.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/deb.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3672 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35633 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_tag.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5113 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/go_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/ostree.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2663 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/patch_queue.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5888 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/pypi.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/quilt.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/zip.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.433927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.434927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/gitrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/tarrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ziprepo.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.435927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3476 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     1806 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/requires.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/top_level.txt
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/lib/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/lib/python3.11/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.435927 bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2024-04-17 09:25:53.000000 bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/markdown_it/port.yaml
```

### Comparing `bst-plugins-experimental-1.98.0/LICENSE` & `bst_plugins_experimental-1.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/PKG-INFO` & `bst_plugins_experimental-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.98.0
+Version: 1.99.0
 Summary: A collection of experimental BuildStream plugins.
 License: LGPL-2.1-or-later
 Project-URL: documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Project-URL: repository, https://gitlab.com/BuildStream/bst-plugins-experimental
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `bst-plugins-experimental-1.98.0/README.rst` & `bst_plugins_experimental-1.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/project.conf` & `bst_plugins_experimental-1.99.0/project.conf`

 * *Files 2% similar despite different names*

```diff
@@ -34,12 +34,13 @@
   sources:
   - bazel_source
   - cpan
   - deb
   - git_module
   - git_repo
   - git_tag
+  - go_module
   - patch_queue
   - quilt
   - ostree
   - pypi
   - zip
```

### Comparing `bst-plugins-experimental-1.98.0/pyproject.toml` & `bst_plugins_experimental-1.99.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazel_build.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazel_build.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/bazelize.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazelize.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/check_forbidden.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/check_forbidden.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/collect_integration.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_integration.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/collect_manifest.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_manifest.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,87 +17,111 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Authors:
 #        Valentin David <valentin.david@gmail.com>
 #        Adam Jones <adam.jones@codethink.co.uk>
+"""
+Collect Manifest Element
+
+A buildstream plugin used to produce a manifest file
+containing a list of elements for a given dependency.
+
+The manifest contains useful information such as:
+    - CPE data, such as CVE patches
+    - Package name
+    - Version
+    - Sources
+    - Source locations
+    - SHAs
+    - Patch files
+
+The manifest file is exported as a json file to the path provided
+under the "path" variable defined in the .bst file.
+
+Dependency elements can manually declare CPE data in their public
+section. For example:
+
+.. code:: yaml
+
+   public:
+     cpe:
+       product: gnutls
+       vendor: gnu
+       version: '1.0'
+
+This data will be set in the ``x-cpe`` field of the entry.
+
+If not present, ``product`` will be automatically be inferred from the
+name of the element.
+
+For version resolution source plugin must opt-in to export_manifest protocol
+by setting BST_EXPORT_MANIFEST and implementing export_manifest method.
+
+Currently allowed outputs are:
+
+.. code-block:: JSON
+
+    {
+       "type": "git",
+       "url": "https://foo.bar/repo.git",
+       "commit": "hash/git-describe"
+    }
+
+.. code-block:: JSON
+
+    {
+       "type": "archive",
+       "url": "https://path/to/package.tgz",
+       "sha256": "checksum"
+    }
+
+.. code-block:: JSON
+
+    {
+       "type": "patch",
+       "path": "path/to/patches"
+    }
+
+Version will be calculated from commit for git and from basename of URL for
+archive.
+
+The default version regular expression is ``\\d+\\.\\d+(?:\\.\\d+)?`` (2 or 3
+numerical components separated by dots). It is possible to
+change the version regular expression with field ``version-match``.
+
+The version regular exression must follow Python regular expression
+syntax.  A version regular expression with no group will match exactly
+the version. A version regular expression with groups will match
+components of the version with each groups. The components will then
+be concatenated using ``.`` (dot) as a separator.
+
+``version-match`` in the ``cpe`` public data will never be exported in
+the ``x-cpe`` field of the manifest.
+
+Here is an example of ``version-match`` where the filename is
+``openssl1_1_1d.tar.gz``, the result version will be ``1.1.1d``.
+
+.. code:: yaml
+
+   public:
+     cpe:
+       version-match: '(\\d+)_(\\d+)_(\\d+[a-z]?)'
+"""
 
 import os
 import re
 import json
-from collections import OrderedDict
-from collections.abc import Mapping
+import posixpath
+
 from buildstream import Element, Node, ElementError
 
 
 class CollectManifestElement(Element):
-    """
-    Collect Manifest Element
-
-    A buildstream plugin used to produce a manifest file
-    containing a list of elements for a given dependency.
-
-    The manifest contains useful information such as:
-        - CPE data, such as CVE patches
-        - Package name
-        - Version
-        - Sources
-        - Source locations
-        - SHAs
-        - Patch files
-
-    The manifest file is exported as a json file to the path provided
-    under the "path" variable defined in the .bst file.
-
-    Dependency elements can manually declare CPE data in their public
-    section. For example:
-
-    .. code:: yaml
-
-       public:
-         cpe:
-           product: gnutls
-           vendor: gnu
-           version: '1.0'
-
-    This data will be set in the ``x-cpe`` field of the entry.
-
-    If not present, ``product`` will be automatically be inferred from the
-    name of the element.
-
-    If not present, ``version`` will be taken from first ``git``,
-    ``git_tag``, ``tar`` or ``zip`` source which filename (for ``tar`` and
-    ``zip``) or reference (for ``git`` and ``git_tag``) contains a
-    substring matching a version regular expression. That matched
-    substring will be the ``version``.
-
-    The default version regular expression is ``\\d+\\.\\d+(?:\\.\\d+)?`` (2 or 3
-    numerical components separated by dots). It is possible to
-    change the version regular expression with field ``version-match``.
-
-    The version regular exression must follow Python regular expression
-    syntax.  A version regular expression with no group will match exactly
-    the version. A version regular expression with groups will match
-    components of the version with each groups. The components will then
-    be concatenated using ``.`` (dot) as a separator.
-
-    ``version-match`` in the ``cpe`` public data will never be exported in
-    the ``x-cpe`` field of the manifest.
-
-    Here is an example of ``version-match`` where the filename is
-    ``openssl1_1_1d.tar.gz``, the result version will be ``1.1.1d``.
-
-    .. code:: yaml
-
-       public:
-         cpe:
-           version-match: '(\\d+)_(\\d+)_(\\d+[a-z]?)'
-    """
-
     BST_MIN_VERSION = "2.0"
     BST_ARTIFACT_VERSION = 1
 
     def configure(self, node):
         if "path" in node:
             self.path = self.node_subst_vars(node.get_scalar("path"))
         else:
@@ -169,19 +193,21 @@
             return
         visited.add(dep)
         for subdep in dep.dependencies(recurse=False):
             yield from self.get_dependencies(subdep, visited)
         yield dep
 
     def assemble(self, sandbox):
-        manifest = OrderedDict()
-        manifest[
-            "//NOTE"
-        ] = "This is a generated manifest from buildstream files and not usable by flatpak-builder"
-        manifest["modules"] = []
+        manifest = {
+            "//NOTE": (
+                "This is a generated manifest from buildstream files "
+                "and not usable by flatpak-builder"
+            ),
+            "modules": [],
+        }
 
         visited = set()
         for top_dep in self.dependencies(recurse=False):
             for dep in self.get_dependencies(top_dep, visited):
                 import_manifest = dep.get_public_data("cpe-manifest")
 
                 if import_manifest:
@@ -213,49 +239,20 @@
                     new_filename = list(filename)
                     new_filename[-1] = str(version)
                     filename = "".join(new_filename)
                 else:
                     filename = filename + "-1"
 
             with vdir.open_file(filename, mode="w") as o:
-                json.dump(cleanup_provenance(manifest), o, indent=2)
+                json.dump(manifest, o, indent=2)
 
         manifest_node = Node.from_dict(dict(manifest))
         self.set_public_data("cpe-manifest", manifest_node)
         return os.path.sep
 
-    def nodes_from_list(self, list_value):
-        ret_list = []
-
-        for item in list_value:
-            if isinstance(item, Mapping):
-                sub_node = Node.from_dict(item)
-                ret_list.append(sub_node)
-            elif isinstance(item, list):
-                sub_list = self.nodes_from_list(item)
-                ret_list.append(sub_list)
-            else:
-                ret_list.append(item)
-
-        return ret_list
-
-    def dicts_from_list(self, list_value):
-        ret_list = []
-
-        for item in list_value:
-            if isinstance(item, Mapping):
-                ret_list.append(item.strip_node_info())
-            elif isinstance(item, list):
-                sub_list = self.dicts_from_list(item)
-                ret_list.append(sub_list)
-            else:
-                ret_list.append(item)
-
-        return ret_list
-
 
 class VersionMatcher:
 
     DEFAULT_VERSION_RE = re.compile(r"\d+\.\d+(?:\.\d+)?")
 
     def __init__(self, match):
         if match is None:
@@ -277,14 +274,27 @@
         This method attempts to extract the source version
         from a dependency. This data can generally be found
         in the url for tar balls, or the ref for git repos.
 
         :sources A list of BuildStream Sources
         """
         for source in sources:
+            export_manifest = getattr(source, "BST_EXPORT_MANIFEST", False)
+            if export_manifest:
+                manifest = source.export_manifest()
+                version = None
+                if manifest["type"] == "git":
+                    version = self._parse_version(manifest["commit"])
+                elif manifest["type"] == "archive":
+                    version = self._parse_version(
+                        posixpath.basename(manifest["url"])
+                    )
+                if version is None:
+                    continue
+                return version
             if source.get_kind() in ["tar", "zip"]:
                 url = source.url
                 filename = url.rpartition("/")[2]
                 version = self._parse_version(filename)
                 if version is not None:
                     return version
             elif source.get_kind().startswith("git"):
@@ -300,63 +310,38 @@
     Returns a list of source URLs and refs, currently for
     git, tar and patch sources.
 
     :sources A list of BuildStream Sources
     """
     source_locations = []
     for source in sources:
+        export_manifest = getattr(source, "BST_EXPORT_MANIFEST", False)
+        if export_manifest:
+            manifest = source.export_manifest()
+            source_locations.append(manifest)
+            continue
         if source.get_kind() in ["git"]:
             url = source.translate_url(
                 source.mirror.url,
                 alias_override=None,
                 primary=source.mirror.primary,
             )
             source_locations.append(
                 {
                     "type": source.get_kind(),
                     "url": url,
                     "commit": source.mirror.ref,
                 }
             )
-        if source.get_kind() in ["git_repo", "git_tag"]:
-            url = source.translate_url(
-                source.mirror.url,
-                alias_override=None,
-                primary=source.mirror.primary,
-            )
-            source_locations.append(
-                {
-                    "type": "git",
-                    "x-bst-kind": source.get_kind(),
-                    "url": url,
-                    "commit": source.mirror.ref,
-                }
-            )
         if source.get_kind() in ["patch"]:
             patch = source.path.rpartition("/")[2]
             source_locations.append({"type": source.get_kind(), "path": patch})
         if source.get_kind() in ["tar", "zip"]:
             source_locations.append(
                 {"type": "archive", "url": source.url, "sha256": source.ref}
             )
 
     return source_locations
 
 
-def cleanup_provenance(data):
-    """
-    Remove buildstream provenance data from the output data
-    """
-    if isinstance(data, dict):
-        ret = OrderedDict()
-        for k, v in data.items():
-            if k != "__bst_provenance_info":
-                ret[k] = cleanup_provenance(v)
-        return ret
-    elif isinstance(data, list):
-        return [cleanup_provenance(v) for v in data]
-    else:
-        return data
-
-
 def setup():
     return CollectManifestElement
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_build.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_build.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_deploy.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/dpkg_deploy.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_bootimg.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_ext4.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/fastboot_ext4.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/flatpak_repo.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/flatpak_repo.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/makemaker.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/makemaker.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/modulebuild.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/modulebuild.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/oci.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/oci.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/pyproject.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/pyproject.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/qmake.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/qmake.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/snap_image.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/snap_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  License along with this library. If not, see <http://www.gnu.org/licenses/>.
 #
 #  Authors:
 #         Valentin David <valentin.david@codethink.co.uk>
 
 
 import os
-from ruamel import yaml
+from ruamel.yaml import YAML
 from buildstream import Element
 
 
 class SnapImageElement(Element):
 
     BST_MIN_VERSION = "2.0"
     BST_FORBID_RDEPENDS = True
@@ -72,14 +72,15 @@
             metadata_filename = "snap.yaml"
 
             basedir = sandbox.get_virtual_directory()
             metadir = basedir.open_directory(
                 metadir_path.lstrip(os.path.sep), create=True
             )
 
+            yaml = YAML(typ="unsafe", pure=True)
             with metadir.open_file(metadata_filename, mode="w") as file:
                 yaml.dump(self.metadata, file)
 
         return os.path.join(os.sep, reldirectory_path)
 
 
 def setup():
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/tar_element.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/tar_element.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/x86image.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/elements/x86image.yaml` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/bazel_source.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/bazel_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,14 @@
         self.ref = node.get_str("ref", None)
 
     def set_ref(self, ref, node):
         node["ref"] = self.ref = ref
 
     def track(self, previous_sources_dir):
         workspace = os.path.join(previous_sources_dir, self.workspace_dir)
-
         repo_file = os.path.join(workspace, self.repo_file)
         self._ensure_repo_file(repo_file, workspace)
 
         assert os.path.isfile(repo_file)
 
         with open(repo_file, encoding="utf-8") as repo:
             ref = hashlib.sha256()
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/cpan.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/cpan.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/deb.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/deb.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/git_module.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_module.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/git_repo.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_git_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,140 +1,61 @@
 """
-git_repo - plugin for git repo handling
+This module contains common helpers for git plugins
 ==============================================
 
-**Usage:**
-
-.. code:: yaml
-
-   # Specify the git_repo source kind
-   kind: git_repo
-
-   # Specify the repository url, using an alias defined
-   # in your project configuration is recommended.
-   url: upstream:repo.git
-
-   # Optionally specify a tracking branch or tag, this
-   # will be used to update the 'ref' when refreshing the pipeline.
-   # Tracking supports Unix shell-style globs, as implemented by Python's
-   # fnmatch module,  that can be used to filter wanted tag from repository.
-   track: release-*
-
-   # Specify the commit checksum, this must be specified in order
-   # to checkout sources and build, but can be automatically
-   # updated if the 'track' attribute was specified.
-   ref: release-3.0-0-gcad743283c43c776d03ae05578f353f728be62e3
-
-   # Specify tracks to exclude in case there's eg bad tags by upstream
-   exclude:
-   - release-3.0.1
-
-   # Declare the format of ref after tracking. When tracking branches,
-   # fetching will be required if sha1 is not used. If git-describe is
-   # given, ref follows output of `git describe`. Regardless of format,
-   # `git describe` and `git log -1` are expected to work in the sandbox.
-   ref-format: git-describe
 """
 
 import fnmatch
-import re
 import os
+import re
 import threading
-import netrc
+
 
 from enum import Enum
 from stat import S_ISDIR, S_ISLNK
-from dataclasses import dataclass
-from urllib.parse import urlparse
 
-from buildstream import Source, SourceFetcher, SourceError
+from buildstream import SourceFetcher, SourceError
 from buildstream.utils import url_directory_name
 
+import dulwich
 from dulwich.repo import Repo
 from dulwich.objects import Commit, Tag, S_ISGITLINK
 from dulwich.client import get_transport_and_path, HTTPUnauthorized
 from dulwich.errors import GitProtocolError, NotGitRepository
 from dulwich.refs import ANNOTATED_TAG_SUFFIX
 
+from ._utils import get_netrc_credentials
+
 
 REF_REGEX = re.compile(r"(?:(.*)(?:-(\d+)-g))?([0-9a-f]{40})")
 SPLITTER_REGEX = re.compile(rb"[a-zA-Z]+|[0-9]+")
 
 
-def pattern_to_regex(pattern):
-    """
-    Transforms a glob pattern into a regex to match refs.
-
-    If the pattern doesn't start with "refs/", it will be considered to only match refs in
-    refs/tags/ and refs/heads.
-    """
-    if pattern.startswith("refs/"):
-        return re.compile(fnmatch.translate(pattern).encode())
-
-    return re.compile(
-        ("refs/(heads|tags)/" + fnmatch.translate(pattern)).encode()
-    )
-
-
-def version_sort_key(elt):
-    """
-    A sort key that can be used to versions. It sorts letters before numbers (so 1.beta is earlier
-    than 1.0) and disregards separators (so 1.beta, 1~beta and 1beta are the same).
-    """
-    return [
-        # to sort letters before digits
-        (-1, part) if part.isalpha() else (int(part), "")
-        for part in SPLITTER_REGEX.findall(elt)
-    ]
-
-
-def get_matching_refs(refs, tracking, exclude):
-    real_refs = {ref for ref in refs if not ref.endswith(ANNOTATED_TAG_SUFFIX)}
-    matching_regex = pattern_to_regex(tracking)
-
-    matching_refs = [ref for ref in real_refs if matching_regex.match(ref)]
-
-    if exclude:
-        exclude_regexs = [pattern_to_regex(pattern) for pattern in exclude]
-        matching_refs = [
-            ref
-            for ref in matching_refs
-            if not any(regex.match(ref) for regex in exclude_regexs)
-        ]
-
-    return matching_refs
-
-
-def get_netrc_credentials(url):
-    p = urlparse(url)
-    if p.scheme != "https":
-        return {}
-    try:
-        n = netrc.netrc()
-        creds = n.authenticators(p.hostname)
-
-        if creds is not None:
-            # creds is a tuple (username, account, password)
-            return {"username": creds[0], "password": creds[2]}
-    except FileNotFoundError:
-        pass
-
-    return {}
-
-
 def init_repo(mirror_dir):
     """
     Open a repo at the given mirror_dir, creating an empty bare repo if it doesn't exist.
     """
     try:
         return Repo.init_bare(mirror_dir, mkdir=True)
     except FileExistsError:
         return Repo(mirror_dir, bare=True)
 
 
+def resolve_mirror_dir(source, url):
+    if url.endswith(".git"):
+        norm_url = url[:-4]
+    else:
+        norm_url = url
+
+    return os.path.join(
+        source.get_mirror_directory(),
+        url_directory_name(norm_url) + ".git",
+    )
+
+
 def collect_objects(mirror, commit, base, trees_only):
     if commit == base:
         commits = {commit}
     elif base is None:
         commits = {entry.commit for entry in mirror.get_walker(commit.id)}
     else:
         commits = {
@@ -231,36 +152,49 @@
 
     return revision
 
 
 LOCKS = {}
 
 
+class RefFormat(Enum):
+    SHA1 = "sha1"
+    GIT_DESCRIBE = "git-describe"
+
+
+def make_lock(mirror_dir):
+    return LOCKS.setdefault(mirror_dir, threading.Lock())
+
+
 class GitMirror(SourceFetcher):
     def __init__(self, source, url, ref):
         super().__init__()
         self.mark_download_url(url)
 
         self.source = source
         self.url = url
+        self.ref = ref
 
-        tag, depth, sha = REF_REGEX.match(ref).groups()
+        match = REF_REGEX.match(ref)
+        assert match is not None
+        tag, depth, sha = match.groups()
 
         self.sha = sha
         self.tagref = f"refs/tags/{tag}".encode() if tag else None
         self.depth = int(depth) + 1 if depth else None
+        self.mirror_dir = resolve_mirror_dir(source, url)
 
     def fetch(self, alias_override=None):
         url = self.source.translate_url(
             self.url, alias_override=alias_override
         )
-        lock = LOCKS.setdefault(self.source.mirror_dir, threading.Lock())
+        lock = make_lock(self.mirror_dir)
 
         with lock, init_repo(
-            self.source.mirror_dir
+            self.mirror_dir
         ) as repo, self.source.timed_activity(f"Fetching from {url}"):
             if self.sha.encode() in repo and (
                 not self.tagref or self.tagref in repo.refs
             ):
                 return
 
             self.source.status(f"Fetching {self.sha}")
@@ -278,15 +212,15 @@
                     wanted.add(refs[self.tagref])
                     return wanted
 
                 raise SourceError(
                     f"ref {self.tagref.decode()} not found in remote {url}"
                 )
 
-            # Another optimisation we can do is to request all the refs that match what we're
+            # Another optimization we can do is to request all the refs that match what we're
             # tracking. This is almost guaranteed to get us what we need without downloading
             # everything.
             def track_want(refs, depth=None):
                 wanted_refs = get_matching_refs(
                     refs, self.source.tracking, self.source.exclude
                 )
 
@@ -296,41 +230,35 @@
                 self.source.status(
                     "fetching tracked refs",
                     detail=b"\n".join(wanted_refs).decode(),
                 )
                 wanted = {refs[ref] for ref in wanted_refs}
                 return wanted
 
-            credentials = get_netrc_credentials(url)
-            client, path = get_transport_and_path(url, **credentials)
+            client, path = get_authenticated_transport_and_path(url)
 
             try:
                 try:
                     remote_refs = client.fetch(
                         path,
                         repo,
                         determine_wants=exact_want,
                         depth=self.depth,
                     )
                 except GitProtocolError as e:
                     if "not our ref" not in str(e):
                         raise
 
                     remote_refs = client.fetch(
-                        path,
-                        repo,
-                        determine_wants=track_want,
-                        depth=self.depth,
+                        path, repo, determine_wants=track_want
                     )
 
                     # Fall back to downloading everything
                     if self.sha.encode() not in repo:
-                        remote_refs = client.fetch(
-                            path, repo, depth=self.depth
-                        )
+                        remote_refs = client.fetch(path, repo)
             except (GitProtocolError, HTTPUnauthorized, NotGitRepository) as e:
                 raise SourceError(f"failed to fetch: {e}") from e
             except NotImplementedError as e:
                 self.source.warn(f"not implemented {e}")
                 if client.dumb:
                     raise SourceError(
                         "Fetching from a dumb repository is not currently supported, "
@@ -341,153 +269,17 @@
             # check that we actually pulled the required commit
             if self.sha.encode() not in repo:
                 raise SourceError(f"{self.sha} not found in remote {url}")
 
             if self.tagref:
                 repo.refs.add_if_new(self.tagref, remote_refs[self.tagref])
 
-
-class RefFormat(Enum):
-    SHA1 = "sha1"
-    GIT_DESCRIBE = "git-describe"
-
-
-@dataclass
-class RepoInfo:
-    primary: bool
-    ref: str
-    url: str
-
-
-class GitSource(Source):
-    BST_MIN_VERSION = "2.0"
-
-    def configure(self, node):
-        CONFIG_KEYS = ["ref", "url", "track", "exclude", "ref-format"]
-
-        node.validate_keys(Source.COMMON_CONFIG_KEYS + CONFIG_KEYS)
-        self.ref = None
-        self.load_ref(node)
-
-        self.url = node.get_str("url")
-        self.mark_download_url(self.url)
-
-        if self.url.endswith(".git"):
-            norm_url = self.url[:-4]
-        else:
-            norm_url = self.url
-
-        self.mirror_dir = os.path.join(
-            self.get_mirror_directory(),
-            url_directory_name(norm_url) + ".git",
-        )
-
-        self.tracking = node.get_str("track", None)
-        self.exclude = node.get_str_list("exclude", [])
-
-        self.ref_format = node.get_enum(
-            "ref-format", RefFormat, RefFormat.SHA1
-        )
-
-        # make the url-manifest script happy
-        self.mirror = RepoInfo(primary=True, ref=self.ref, url=self.url)
-
-    def preflight(self):
-        pass
-
-    def get_unique_key(self):
-        return {"ref": self.ref, "bugfix": 1}
-
-    # loading and saving refs
-    def load_ref(self, node):
-        if "ref" not in node:
-            return
-        ref = node.get_str("ref")
-        if REF_REGEX.match(ref) is None:
-            raise SourceError(f"ref {ref} is not in the expected format")
-        self.ref = ref
-
-    def get_ref(self):
-        return self.ref
-
-    def set_ref(self, ref, node):
-        self.ref = ref
-        node["ref"] = ref
-
-    def is_cached(self):
-        tag, _, sha = REF_REGEX.match(self.ref).groups()
-
-        with Repo(self.mirror_dir, bare=True) as repo:
-            cached = sha.encode() in repo
-            if tag:
-                ref = b"refs/tags/" + tag.encode()
-                cached_ref = ref in repo
-
-                cached = cached and cached_ref
-
-        return cached
-
-    def track(self):
-        if not self.tracking:
-            return None
-
-        url = self.translate_url(self.url)
-        self.status(f"Tracking {self.tracking} from {url}")
-
-        credentials = get_netrc_credentials(url)
-        client, path = get_transport_and_path(url, **credentials)
-
-        try:
-            refs = client.get_refs(path)
-        except (GitProtocolError, HTTPUnauthorized) as exc:
-            raise SourceError(f"Failed to track {url}") from exc
-
-        matching_refs = get_matching_refs(refs, self.tracking, self.exclude)
-        if not matching_refs:
-            raise SourceError("No matching refs")
-
-        self.debug(
-            "Refs to be tracked", detail=b"\n".join(matching_refs).decode()
-        )
-
-        ref = max(matching_refs, key=version_sort_key)
-
-        # peel the ref if possible
-        peeled_ref = ref + ANNOTATED_TAG_SUFFIX
-        if peeled_ref in refs:
-            resolved = refs[peeled_ref]
-        else:
-            resolved = refs[ref]
-
-        # Use str instead of bytes from here on
-        ref = ref.decode()
-        resolved = resolved.decode()
-
-        self.status(f"Tracked {ref}: {resolved}")
-
-        if self.ref_format == RefFormat.SHA1:
-            return resolved
-
-        if "tags" in ref:
-            tag = ref.split("/", 2)[-1]
-            return f"{tag}-0-g{resolved}"
-
-        # Need to fetch to generate the ref in git-describe format
-        fetcher = GitMirror(self, self.url, resolved)
-        fetcher.fetch()
-
-        with Repo(self.mirror_dir) as repo:
-            return git_describe(repo, resolved, refs)
-
-    def get_source_fetchers(self):
-        yield GitMirror(self, self.url, self.ref)
-
     def stage(self, directory):
         tag, _, sha = REF_REGEX.match(self.ref).groups()
-        self.status(f"Checking out {sha}")
+        self.source.status(f"Checking out {sha}")
 
         with Repo(self.mirror_dir, bare=True) as mirror:
             refs = {b"HEAD": sha.encode()}
             tag_objects = set()
 
             commit = mirror[sha.encode()]
             base = mirror[sha.encode()]
@@ -505,28 +297,28 @@
                 assert isinstance(
                     tag_target, Commit
                 ), f"Tag {tag} does not point to a commit (type {type(tag_target)}"
 
                 base = tag_target
 
             objects = collect_objects(mirror, commit, base, True)
-            self.status(f"Adding {len(objects)} objects")
+            self.source.status(f"Adding {len(objects)} objects")
 
             # `|` means union
             stage_repository(
                 mirror, directory, tag_objects | objects, refs, {}, pack=False
             )
 
     def init_workspace(self, directory):
         tag, _, sha = REF_REGEX.match(self.ref).groups()
-        self.status(f"Checking out {sha}")
+        self.source.status(f"Checking out {sha}")
 
         with Repo(self.mirror_dir, bare=True) as mirror:
             refs = {b"HEAD": sha.encode()}
-            remotes = {"origin": self.translate_url(self.url)}
+            remotes = {"origin": self.source.translate_url(self.url)}
 
             commit = mirror[sha.encode()]
             objects = collect_objects(mirror, commit, None, False)
 
             tag_objects = set()
 
             for tag, tag_sha in mirror.refs.as_dict(b"refs/tags").items():
@@ -548,22 +340,162 @@
                     tag_target, Commit
                 ), f"Tag {tag} does not point to a commit (type {type(tag_target)}"
 
                 if tag_target in objects:
                     tag_objects.add(tag_obj)
                     refs[tag_ref] = tag_obj.id
 
-            self.status(f"Adding {len(objects)} objects")
+            self.source.status(f"Adding {len(objects)} objects")
 
             # `|` means union
             stage_repository(
                 mirror,
                 directory,
                 tag_objects | objects,
                 refs,
                 remotes,
                 pack=True,
             )
 
+    def has_ref(self):
+        tag, _, sha = REF_REGEX.match(self.ref).groups()
+
+        with Repo(self.mirror_dir, bare=True) as repo:
+            cached = sha.encode() in repo
+            if tag:
+                ref = b"refs/tags/" + tag.encode()
+                cached_ref = ref in repo
+
+                cached = cached and cached_ref
+
+        return cached
+
+
+def version_sort_key(elt):
+    """
+    A sort key that can be used to versions. It sorts letters before numbers (so 1.beta is earlier
+    than 1.0) and disregards separators (so 1.beta, 1~beta and 1beta are the same).
+    """
+    return [
+        # to sort letters before digits
+        (-1, part) if part.isalpha() else (int(part), "")
+        for part in SPLITTER_REGEX.findall(elt)
+    ]
+
 
-def setup():
-    return GitSource
+def pattern_to_regex(pattern):
+    """
+    Transforms a glob pattern into a regex to match refs.
+
+    If the pattern doesn't start with "refs/", it will be considered to only match refs in
+    refs/tags/ and refs/heads.
+    """
+    if pattern.startswith("refs/"):
+        return re.compile(fnmatch.translate(pattern).encode())
+
+    return re.compile(
+        ("refs/(heads|tags)/" + fnmatch.translate(pattern)).encode()
+    )
+
+
+def get_matching_refs(refs, tracking, exclude):
+    real_refs = {ref for ref in refs if not ref.endswith(ANNOTATED_TAG_SUFFIX)}
+    matching_regex = pattern_to_regex(tracking)
+
+    matching_refs = [ref for ref in real_refs if matching_regex.match(ref)]
+
+    if exclude:
+        exclude_regexs = [pattern_to_regex(pattern) for pattern in exclude]
+        matching_refs = [
+            ref
+            for ref in matching_refs
+            if not any(regex.match(ref) for regex in exclude_regexs)
+        ]
+
+    return matching_refs
+
+
+def resolve_ref(source, url, tracking, ref_format, exclude):
+    mirror_dir = resolve_mirror_dir(source, url)
+    url = source.translate_url(url)
+    source.status(f"Tracking {tracking} from {url}")
+
+    client, path = get_authenticated_transport_and_path(url)
+
+    try:
+        refs = client.get_refs(path)
+    except (GitProtocolError, HTTPUnauthorized) as exc:
+        raise SourceError(f"Failed to track {url}") from exc
+
+    matching_refs = get_matching_refs(refs, tracking, exclude)
+    if not matching_refs:
+        raise SourceError("No matching refs")
+
+    source.debug(
+        "Refs to be tracked", detail=b"\n".join(matching_refs).decode()
+    )
+
+    ref = max(matching_refs, key=version_sort_key)
+
+    # peel the ref if possible
+    peeled_ref = ref + ANNOTATED_TAG_SUFFIX
+    if peeled_ref in refs:
+        resolved = refs[peeled_ref]
+    else:
+        resolved = refs[ref]
+
+    # Use str instead of bytes from here on
+    ref = ref.decode()
+    resolved = resolved.decode()
+
+    source.status(f"Tracked {ref}: {resolved}")
+
+    if ref_format == RefFormat.SHA1:
+        return resolved
+
+    if "tags" in ref:
+        tag = ref.split("/", 2)[-1]
+        return f"{tag}-0-g{resolved}"
+
+    # Need to fetch to generate the ref in git-describe format
+    fetcher = GitMirror(source, url, resolved)
+    fetcher.fetch()
+
+    with Repo(mirror_dir) as repo:
+        return git_describe(repo, resolved, refs)
+
+
+def get_authenticated_transport_and_path(url):
+    credentials = get_netrc_credentials(url)
+    return get_transport_and_path(url, **credentials)
+
+
+def get_full_sha(source, url, short_sha):
+    mirror_dir = resolve_mirror_dir(source, url)
+    url = source.translate_url(url)
+    source.status(f"Tracking {short_sha} from {url}")
+
+    lock = make_lock(mirror_dir)
+
+    with lock, init_repo(mirror_dir) as repo:
+        client, path = get_authenticated_transport_and_path(url)
+        client.fetch(path, repo)
+
+        for candidate in repo.object_store:
+            candidate = candidate.decode()
+            if candidate.startswith(short_sha):
+                source.status(f"Tracked {short_sha}: {candidate}")
+                return candidate
+
+    raise SourceError(f"Failed to find {short_sha} from {url}")
+
+
+def verify_version():
+    required = (0, 21, 7)
+    if dulwich.__version__ < required:
+        version_string = ".".join(map(str, dulwich.__version__))
+        required_string = ".".join(map(str, required))
+        raise SourceError(
+            "Dulwich version was {} but {} required".format(
+                version_string, required_string
+            )
+        )
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/git_tag.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -818,14 +818,15 @@
 
     def have_all_extra_refs(self):
         return True
 
 
 class GitTagSource(AbstractGitTagSource):
     # pylint: disable=attribute-defined-outside-init
+    BST_EXPORT_MANIFEST = True
 
     def get_extra_config_keys(self):
         return [
             "track",
             "track-extra",
             "track-tags",
             "match",
@@ -1028,11 +1029,23 @@
             ):
                 return False
             if not mirror.has_ref():
                 return False
 
         return True
 
+    def export_manifest(self):
+        url = self.translate_url(
+            self.mirror.url,
+            alias_override=None,
+            primary=False,
+        )
+        return {
+            "type": "git",
+            "url": url,
+            "commit": self.mirror.ref,
+        }
+
 
 # Plugin entry point
 def setup():
     return GitTagSource
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/ostree.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/ostree.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/patch_queue.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/patch_queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import os
 from buildstream import Source, utils
 
 
 class PatchQueueSource(Source):
     BST_MIN_VERSION = "2.0"
     BST_REQUIRES_PREVIOUS_SOURCES_STAGE = True
+    BST_EXPORT_MANIFEST = True
 
     def configure(self, node):
         node.validate_keys(Source.COMMON_CONFIG_KEYS + ["path", "strip"])
         self.path = self.node_get_project_path(
             node.get_scalar("path"), check_is_dir=True
         )
         self.fullpath = os.path.join(self.get_project_directory(), self.path)
@@ -74,10 +75,16 @@
                         directory,
                         "apply",
                         patch,
                     ],
                     fail="Failed to apply patches from {}".format(self.path),
                 )
 
+    def extract_manifest(self):
+        return {
+            "type": "patch",
+            "path": self.path,
+        }
+
 
 def setup():
     return PatchQueueSource
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/pypi.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/pypi.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import requests
 import packaging.utils
 
 from buildstream import Source, SourceError
 from buildstream.utils import url_directory_name
 
-from ._utils import HTTPFetcher, TarStager, ZipStager
+from ._utils import HTTPFetcher, TarStager, ZipStager, translate_url
 
 
 # We do not support parsing HTML
 ACCEPT = "application/vnd.pypi.simple.v1+json"
 
 
 def filter_files(files, matcher):
@@ -80,14 +80,15 @@
             if matcher.match(str(version)):
                 return True
         return False
 
 
 class PyPISource(Source):
     BST_MIN_VERSION = "2.0"
+    BST_EXPORT_MANIFEST = True
 
     REST_API = "https://pypi.org/simple/{name}"
     STORAGE_ROOT = "https://files.pythonhosted.org/packages/"
     KEYS = [
         "url",
         "name",
         "ref",
@@ -185,10 +186,22 @@
 
     def is_cached(self):
         return self.fetcher.is_cached()
 
     def get_source_fetchers(self):
         return [self.fetcher]
 
+    def export_manifest(self):
+        url = translate_url(
+            self,
+            self.base_url,
+            self.suffix,
+        )
+        return {
+            "type": "archive",
+            "url": url,
+            "sha256": self.sha256sum,
+        }
+
 
 def setup():
     return PyPISource
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/quilt.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/quilt.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/sources/zip.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/zip.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/gitrepo.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/gitrepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/ostreerepo.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ostreerepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/tarrepo.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/tarrepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental/testutils/repo/ziprepo.py` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ziprepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/PKG-INFO` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.98.0
+Version: 1.99.0
 Summary: A collection of experimental BuildStream plugins.
 License: LGPL-2.1-or-later
 Project-URL: documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Project-URL: repository, https://gitlab.com/BuildStream/bst-plugins-experimental
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/SOURCES.txt` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,21 +45,23 @@
 src/bst_plugins_experimental/elements/snap_image.py
 src/bst_plugins_experimental/elements/snap_image.yaml
 src/bst_plugins_experimental/elements/tar_element.py
 src/bst_plugins_experimental/elements/tar_element.yaml
 src/bst_plugins_experimental/elements/x86image.py
 src/bst_plugins_experimental/elements/x86image.yaml
 src/bst_plugins_experimental/sources/__init__.py
+src/bst_plugins_experimental/sources/_git_utils.py
 src/bst_plugins_experimental/sources/_utils.py
 src/bst_plugins_experimental/sources/bazel_source.py
 src/bst_plugins_experimental/sources/cpan.py
 src/bst_plugins_experimental/sources/deb.py
 src/bst_plugins_experimental/sources/git_module.py
 src/bst_plugins_experimental/sources/git_repo.py
 src/bst_plugins_experimental/sources/git_tag.py
+src/bst_plugins_experimental/sources/go_module.py
 src/bst_plugins_experimental/sources/ostree.py
 src/bst_plugins_experimental/sources/patch_queue.py
 src/bst_plugins_experimental/sources/pypi.py
 src/bst_plugins_experimental/sources/quilt.py
 src/bst_plugins_experimental/sources/zip.py
 src/bst_plugins_experimental/testutils/__init__.py
 src/bst_plugins_experimental/testutils/repo/__init__.py
```

### Comparing `bst-plugins-experimental-1.98.0/src/bst_plugins_experimental.egg-info/entry_points.txt` & `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.98.0/venv/lib/python3.11/site-packages/markdown_it/port.yaml` & `bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

