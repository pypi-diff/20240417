# Comparing `tmp/paraphase-3.0.0.tar.gz` & `tmp/paraphase-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paraphase-3.0.0.tar", last modified: Tue Oct 31 23:23:21 2023, max compression
+gzip compressed data, was "paraphase-3.1.0.tar", last modified: Wed Apr 17 03:53:44 2024, max compression
```

## Comparing `paraphase-3.0.0.tar` & `paraphase-3.1.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.374946 paraphase-3.0.0/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-3.0.0/LICENSE
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7972 2023-10-31 23:23:21.373942 paraphase-3.0.0/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7642 2023-10-31 22:01:12.000000 paraphase-3.0.0/README.md
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:20.930886 paraphase-3.0.0/paraphase/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/__main__.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:20.982867 paraphase-3.0.0/paraphase/data/
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.015191 paraphase-3.0.0/paraphase/data/19/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5359 2023-10-31 18:32:12.000000 paraphase-3.0.0/paraphase/data/19/config.yaml
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2352 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/data/19/genome_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.043833 paraphase-3.0.0/paraphase/data/19/rccx/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/data/19/rccx/cyp21_diff_sites.txt
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1053 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/data/19/sex_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.074904 paraphase-3.0.0/paraphase/data/19/smn1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/data/19/smn1/known_haplotypes.json
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.131701 paraphase-3.0.0/paraphase/data/38/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    38991 2023-10-31 18:33:00.000000 paraphase-3.0.0/paraphase/data/38/config.yaml
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2023-10-31 04:01:35.000000 paraphase-3.0.0/paraphase/data/38/genome_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.136703 paraphase-3.0.0/paraphase/data/38/rccx/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/data/38/rccx/cyp21_diff_sites.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1104 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/data/38/sex_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.145911 paraphase-3.0.0/paraphase/data/38/smn1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/data/38/smn1/known_haplotypes.json
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      223 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/data/genes.yaml
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.265960 paraphase-3.0.0/paraphase/genes/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      394 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2847 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/cfc1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7938 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/f8_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5788 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/hba_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7553 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/ikbkg_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4926 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/ncf1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5647 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/neb_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    17325 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/opn1lw_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     4486 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/pms2_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    19943 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25155 2023-10-31 04:01:36.000000 paraphase-3.0.0/paraphase/genes/smn1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5707 2023-10-31 04:01:37.000000 paraphase-3.0.0/paraphase/genes/strc_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2791 2023-10-31 04:01:37.000000 paraphase-3.0.0/paraphase/genome_depth.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    48834 2023-10-31 04:01:37.000000 paraphase-3.0.0/paraphase/haplotype_assembler.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    28829 2023-10-31 04:01:37.000000 paraphase-3.0.0/paraphase/paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    78430 2023-10-31 18:36:00.000000 paraphase-3.0.0/paraphase/phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    42432 2023-10-31 18:45:34.000000 paraphase-3.0.0/paraphase/prepare_bam_and_vcf.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:20.985933 paraphase-3.0.0/paraphase.egg-info/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7972 2023-10-31 23:23:17.000000 paraphase-3.0.0/paraphase.egg-info/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1392 2023-10-31 23:23:17.000000 paraphase-3.0.0/paraphase.egg-info/SOURCES.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2023-10-31 23:23:17.000000 paraphase-3.0.0/paraphase.egg-info/dependency_links.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2023-10-31 23:23:17.000000 paraphase-3.0.0/paraphase.egg-info/entry_points.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2023-10-31 23:23:17.000000 paraphase-3.0.0/paraphase.egg-info/requires.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2023-10-31 23:23:17.000000 paraphase-3.0.0/paraphase.egg-info/top_level.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-10-31 23:23:21.375936 paraphase-3.0.0/setup.cfg
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2023-10-31 04:01:37.000000 paraphase-3.0.0/setup.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-10-31 23:23:21.360874 paraphase-3.0.0/tests/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1098 2023-10-31 04:01:38.000000 paraphase-3.0.0/tests/test_f8_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2023-10-31 04:01:38.000000 paraphase-3.0.0/tests/test_haplotype_assembler.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4712 2023-10-31 04:01:38.000000 paraphase-3.0.0/tests/test_opn1lw_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2023-10-31 04:01:38.000000 paraphase-3.0.0/tests/test_paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8616 2023-10-31 04:01:39.000000 paraphase-3.0.0/tests/test_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1835 2023-10-31 04:01:39.000000 paraphase-3.0.0/tests/test_prepare_bam_and_vcf.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2023-10-31 04:01:39.000000 paraphase-3.0.0/tests/test_rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     7844 2023-10-31 04:01:39.000000 paraphase-3.0.0/tests/test_smn1_phaser.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.762002 paraphase-3.1.0/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-3.1.0/LICENSE
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7393 2024-04-17 03:53:44.761011 paraphase-3.1.0/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7063 2024-04-16 20:57:56.000000 paraphase-3.1.0/README.md
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:43.958038 paraphase-3.1.0/paraphase/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2024-04-15 22:17:28.000000 paraphase-3.1.0/paraphase/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2024-01-11 16:37:31.000000 paraphase-3.1.0/paraphase/__main__.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.051052 paraphase-3.1.0/paraphase/data/
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.114039 paraphase-3.1.0/paraphase/data/19/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5390 2024-04-15 21:55:28.000000 paraphase-3.1.0/paraphase/data/19/config.yaml
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2352 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/genome_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.145036 paraphase-3.1.0/paraphase/data/19/rccx/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/rccx/cyp21_diff_sites.txt
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1053 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/sex_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.176028 paraphase-3.1.0/paraphase/data/19/smn1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/smn1/known_haplotypes.json
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.272028 paraphase-3.1.0/paraphase/data/38/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    40934 2024-04-12 16:48:47.000000 paraphase-3.1.0/paraphase/data/38/config.yaml
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    43629 2024-02-02 18:15:30.000000 paraphase-3.1.0/paraphase/data/38/fusion_genes.json
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/genome_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.296027 paraphase-3.1.0/paraphase/data/38/rccx/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/rccx/cyp21_diff_sites.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1104 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/sex_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.343024 paraphase-3.1.0/paraphase/data/38/smn1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/smn1/known_haplotypes.json
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      194 2024-02-21 18:17:36.000000 paraphase-3.1.0/paraphase/data/genes.yaml
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.616006 paraphase-3.1.0/paraphase/genes/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      425 2024-02-14 20:04:22.000000 paraphase-3.1.0/paraphase/genes/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2937 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/cfc1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1531 2024-02-15 03:52:32.000000 paraphase-3.1.0/paraphase/genes/cfhclust.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     8240 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/f8_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5788 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/genes/hba_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7553 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/genes/ikbkg_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4936 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/ncf1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5659 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/neb_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    17211 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/opn1lw_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     4353 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/pms2_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    19955 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25155 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/genes/smn1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5707 2024-01-11 16:37:51.000000 paraphase-3.1.0/paraphase/genes/strc_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2791 2024-01-11 16:37:51.000000 paraphase-3.1.0/paraphase/genome_depth.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    48834 2024-01-11 16:37:32.000000 paraphase-3.1.0/paraphase/haplotype_assembler.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30906 2024-04-15 22:34:32.000000 paraphase-3.1.0/paraphase/paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    86230 2024-04-16 03:39:23.000000 paraphase-3.1.0/paraphase/phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    45486 2024-04-09 23:05:47.000000 paraphase-3.1.0/paraphase/prepare_bam_and_vcf.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.034037 paraphase-3.1.0/paraphase.egg-info/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7393 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1456 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/entry_points.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/requires.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/top_level.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2024-04-17 03:53:44.762015 paraphase-3.1.0/setup.cfg
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2024-01-11 16:37:32.000000 paraphase-3.1.0/setup.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.749003 paraphase-3.1.0/tests/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1110 2024-03-26 20:30:19.000000 paraphase-3.1.0/tests/test_f8_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2024-01-11 16:37:32.000000 paraphase-3.1.0/tests/test_haplotype_assembler.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4712 2024-01-11 16:37:51.000000 paraphase-3.1.0/tests/test_opn1lw_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2024-01-11 16:37:32.000000 paraphase-3.1.0/tests/test_paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    12210 2024-04-16 01:39:44.000000 paraphase-3.1.0/tests/test_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4372 2024-04-15 16:41:24.000000 paraphase-3.1.0/tests/test_prepare_bam_and_vcf.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2024-01-11 16:37:33.000000 paraphase-3.1.0/tests/test_rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     7844 2024-01-11 16:37:51.000000 paraphase-3.1.0/tests/test_smn1_phaser.py
```

### Comparing `paraphase-3.0.0/LICENSE` & `paraphase-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/PKG-INFO` & `paraphase-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 3.0.0
+Version: 3.1.0
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Paraphase: HiFi-based caller for highly homologous genes
+<h1 align="center"><img width="300px" src="docs/logo_Paraphase.svg"/></h1>
+
+<h1 align="center">Paraphase</h1>
+
+<h3 align="center">HiFi-based caller for highly similar paralogous genes</h3>
 
 Many medically relevant genes fall into 'dark' regions where variant calling is limited due to high sequence homology with paralogs or pseudogenes. Paraphase is a Python tool that takes HiFi aligned BAMs as input (whole-genome or enrichment), phases haplotypes for genes of the same family, determines copy numbers and makes phased variant calls. 
 
 ![Paraphase diagram](docs/figures/paraphase_diagram.png)
 Paraphase takes all reads from a gene family, realigns to just the gene of interest and then phases them into haplotypes. This solves the problem of alignment difficulty due to sequence homology and allows us to examine all copies of genes in a gene family and call copy number changes and other variants.
 
-Paraphase supports 161 segmental duplication regions in GRCh38, listed in the [config](paraphase/data/38/config.yaml) file. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
+Paraphase supports 160 segmental duplication [regions](docs/regions.md) in GRCh38. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
 - SMN1/SMN2 (spinal muscular atrophy)
 - RCCX module
   - CYP21A2 (21-Hydroxylase-Deficient Congenital Adrenal Hyperplasia)
   - TNXB (Ehlers-Danlos syndrome)
   - C4A/C4B (relevant in autoimmune diseases)
 - PMS2 (Lynch Syndrome)
 - STRC (hereditary hearing loss and deafness)
 - IKBKG (Incontinentia Pigmenti)
 - NCF1 (chronic granulomatous disease; Williams syndrome)
 - NEB (Nemaline myopathy)
 - F8 (intron 22 inversion, Hemophilia A)
 - CFC1 (heterotaxy syndrome)
 - OPN1LW/OPN1MW (color vision deficiencies)
 - HBA1/HBA2 (Alpha-Thalassemia)
+- GBA (Gaucher disease and Parkison's disease)
+- CYP11B1/CYP11B2 (Glucocorticoid-remediable aldosteronism)
+- CFH/CFHR1/CFHR2/CFHR3/CFHR4 (large deletions/duplications, atypical hemolytic uremic syndrome and age-related macular degeneration)
 
 Please check out our [paper](https://www.cell.com/ajhg/fulltext/S0002-9297(23)00001-0) on its application to the gene SMN1 for more details about Paraphase.   
 Chen X, Harting J, Farrow E, et al. Comprehensive SMN1 and SMN2 profiling for spinal muscular atrophy analysis using long-read PacBio HiFi sequencing. The American Journal of Human Genetics. 2023;0(0). doi:10.1016/j.ajhg.2023.01.001
 
 For whole-genome sequencing (WGS) data, we recommend >20X, ideally 30X, genome coverage. Low coverage or short read length could result in less accurate phasing, especially when gene copies are highly similar to each other. For hybrid capture-based enrichment data, a higher read depth (>50X) is recommended as the read length is generally shorter than WGS.
 
 ## Contact
@@ -76,50 +83,49 @@
 ```
 
 Required parameters:
 - `-b`: Input BAM file or `-l`: text file listing BAM files one per line (a BAI file needs to exist in the same directory)
 - `-o`: Output directory
 - `-r`: Path to the reference genome fasta file
 
-Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. 
+Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. Recommendations on reference genomes to use are documented [here](https://github.com/PacificBiosciences/reference_genomes).
 
 Optional parameters:
-- `-g`: Gene(s) to analyze, separated by comma. All supported genes will be analyzed if not specified.
+- `-g`: Region(s) to analyze, separated by comma. All supported [regions](docs/regions.md) will be analyzed if not specified. Please use region name, i.e. first column in the doc.
 - `-t`: Number of threads.
-- `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](paraphase/data/19/config.yaml) are supported now for GRCh37/hg19).
-- `gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see [below](#interpreting-the-output).
+- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the name of the input BAM. 
+- `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](docs/regions.md) are supported now for GRCh37/hg19).
+- `--gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see more information [here](docs/vcf.md).
 - `--novcf`: If specified, no VCF files will be produced.
 - `--samtools`: path to samtools. If the paths to samtools or minimap2 are not already in the PATH environment variable, they can be provided through the `--samtools` and `--minimap2` parameters.
 - `--minimap2`: path to minimap2
 
 ## Interpreting the output
 
-Paraphase produces a few output files in the directory specified by `-o`, with the sample ID as the prefix.
-
-1. `.vcf` in `sampleID_vcfs` folder. A VCF file is written for each haplotype per gene family. There is also a `_variants.vcf` file containing merged variants from all haplotypes for each gene family. Note that this is not a diploid vcf as there are usually more than two copies of genes in a gene family in a sample.
+Paraphase produces a few output files in the directory specified by `-o`, with the specified or default prefix.
 
-As genes of the same family can be highly similar to each other in sequence and not easy to differentiate (at the sequence level or even at the functional level), variant calls are made against one selected "main" gene from the gene family (e.g. the functional gene is selected when the family has a gene and a pseudogene). In this way, all copies of the gene family can be evaluated for pathogenic variants and one can calculate the copy number of the functional genes in the family and hence infer the disease/carrier status.
+1. `.vcf` in `${prefix}_paraphase_vcfs` folder. A VCF file is written for each region (gene family). More descriptions on the VCF can be found [here](docs/vcf.md).
 
-Exceptions are SMN1 (paralog SMN2), PMS2 (pseudogene PMS2CL), STRC (pseudogene STRCP1), NCF1 (pseudogenes NCF1B and NCF1C) and IKBKG (pseudogene IKBKGP1), where gene differentiation is possible. In these families, haplotypes are assigned to each gene in the family, i.e. gene or paralog/pseudogene, and variants are called against the gene (or paralog/pseudogene) for the gene (or paralog/pseudogene) haplotypes, respectively. Variants calls can be made against the main gene only for these five families if `--gene1only` is specified. 
+2. `.paraphase.bam`: This BAM file can be loaded into IGV for visualization of haplotypes (group reads by `HP` tag and color alignments by `YC` tag). All haplotypes are aligned against the main gene of interest. Tutorials/Examples are provided for medically relevant genes (See below).  
 
-2. `_realigned_tagged.bam`: This BAM file can be loaded into IGV for visualization of haplotypes (group reads by `HP` tag and color alignments by `YC` tag). All haplotypes are aligned against the main gene of interest. Tutorials/Examples are provided for medically relevant genes (See below).  
-
-3. `.json`: Output file summarizing haplotypes and variant calls for each gene family in each sample. In brief, a few generally used fields are explained below.
+3. `.paraphase.json`: Output file summarizing haplotypes and variant calls for each gene family in each sample. In brief, a few generally used fields are explained below.
 - `final_haplotypes`: phased haplotypes for all gene copies in a gene family
 - `total_cn`: total copy number of the family (sum of gene and paralog/pseudogene)
 - `two_copy_haplotypes`: haplotypes that are present in two copies based on depth. This happens when (in a small number of cases) two haplotypes are identical and we infer that there exist two of them instead of one by checking the read depth.
 - `haplotype_details`: lists information about each haplotype 
   - `boundary`: the boundary of the region that is resolved on the haplotype. This is useful when a haplotype is only partially phased.
 - `alleles_final`: haplotypes phased into alleles. This is possible when the segmental duplication is in tandem.
-- `region_depth`: median depth of the gene family (include all copies of gene and paralog/pseudogene) 
 
 Tutorials/Examples are provided for interpreting the `json` output and visualizing haplotypes for medically relevant genes listed below: 
 - [SMN1/SMN2](docs/SMN1_SMN2.md)
 - [RCCX module (CYP21A2)](docs/RCCX.md)
 - [PMS2](docs/PMS2.md)
 - [STRC](docs/STRC.md)
 - [OPN1LW/OPN1MW](docs/OPN1LW_OPN1MW.md)
 - [HBA1/HBA2](docs/HBA1_HBA2.md)
 - [IKBKG](docs/IKBKG.md)
 - [F8](docs/F8.md)
 - [NEB](docs/NEB.md)
 - [NCF1](docs/NCF1.md)
+- [GBA](docs/GBA.md)
+- [CFH gene cluster](docs/CFH.md)
+
```

### Comparing `paraphase-3.0.0/README.md` & `paraphase-3.1.0/paraphase.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,47 @@
-# Paraphase: HiFi-based caller for highly homologous genes
+Metadata-Version: 2.1
+Name: paraphase
+Version: 3.1.0
+Summary: paraphase: HiFi-based caller for highly homologous genes
+Home-page: https://github.com/PacificBiosciences/paraphase
+Author: Xiao Chen
+Author-email: xchen@pacificbiosciences.com
+License: BSD-3-Clause-Clear
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center"><img width="300px" src="docs/logo_Paraphase.svg"/></h1>
+
+<h1 align="center">Paraphase</h1>
+
+<h3 align="center">HiFi-based caller for highly similar paralogous genes</h3>
 
 Many medically relevant genes fall into 'dark' regions where variant calling is limited due to high sequence homology with paralogs or pseudogenes. Paraphase is a Python tool that takes HiFi aligned BAMs as input (whole-genome or enrichment), phases haplotypes for genes of the same family, determines copy numbers and makes phased variant calls. 
 
 ![Paraphase diagram](docs/figures/paraphase_diagram.png)
 Paraphase takes all reads from a gene family, realigns to just the gene of interest and then phases them into haplotypes. This solves the problem of alignment difficulty due to sequence homology and allows us to examine all copies of genes in a gene family and call copy number changes and other variants.
 
-Paraphase supports 161 segmental duplication regions in GRCh38, listed in the [config](paraphase/data/38/config.yaml) file. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
+Paraphase supports 160 segmental duplication [regions](docs/regions.md) in GRCh38. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
 - SMN1/SMN2 (spinal muscular atrophy)
 - RCCX module
   - CYP21A2 (21-Hydroxylase-Deficient Congenital Adrenal Hyperplasia)
   - TNXB (Ehlers-Danlos syndrome)
   - C4A/C4B (relevant in autoimmune diseases)
 - PMS2 (Lynch Syndrome)
 - STRC (hereditary hearing loss and deafness)
 - IKBKG (Incontinentia Pigmenti)
 - NCF1 (chronic granulomatous disease; Williams syndrome)
 - NEB (Nemaline myopathy)
 - F8 (intron 22 inversion, Hemophilia A)
 - CFC1 (heterotaxy syndrome)
 - OPN1LW/OPN1MW (color vision deficiencies)
 - HBA1/HBA2 (Alpha-Thalassemia)
+- GBA (Gaucher disease and Parkison's disease)
+- CYP11B1/CYP11B2 (Glucocorticoid-remediable aldosteronism)
+- CFH/CFHR1/CFHR2/CFHR3/CFHR4 (large deletions/duplications, atypical hemolytic uremic syndrome and age-related macular degeneration)
 
 Please check out our [paper](https://www.cell.com/ajhg/fulltext/S0002-9297(23)00001-0) on its application to the gene SMN1 for more details about Paraphase.   
 Chen X, Harting J, Farrow E, et al. Comprehensive SMN1 and SMN2 profiling for spinal muscular atrophy analysis using long-read PacBio HiFi sequencing. The American Journal of Human Genetics. 2023;0(0). doi:10.1016/j.ajhg.2023.01.001
 
 For whole-genome sequencing (WGS) data, we recommend >20X, ideally 30X, genome coverage. Low coverage or short read length could result in less accurate phasing, especially when gene copies are highly similar to each other. For hybrid capture-based enrichment data, a higher read depth (>50X) is recommended as the read length is generally shorter than WGS.
 
 ## Contact
@@ -65,50 +83,49 @@
 ```
 
 Required parameters:
 - `-b`: Input BAM file or `-l`: text file listing BAM files one per line (a BAI file needs to exist in the same directory)
 - `-o`: Output directory
 - `-r`: Path to the reference genome fasta file
 
-Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. 
+Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. Recommendations on reference genomes to use are documented [here](https://github.com/PacificBiosciences/reference_genomes).
 
 Optional parameters:
-- `-g`: Gene(s) to analyze, separated by comma. All supported genes will be analyzed if not specified.
+- `-g`: Region(s) to analyze, separated by comma. All supported [regions](docs/regions.md) will be analyzed if not specified. Please use region name, i.e. first column in the doc.
 - `-t`: Number of threads.
-- `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](paraphase/data/19/config.yaml) are supported now for GRCh37/hg19).
-- `gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see [below](#interpreting-the-output).
+- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the name of the input BAM. 
+- `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](docs/regions.md) are supported now for GRCh37/hg19).
+- `--gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see more information [here](docs/vcf.md).
 - `--novcf`: If specified, no VCF files will be produced.
 - `--samtools`: path to samtools. If the paths to samtools or minimap2 are not already in the PATH environment variable, they can be provided through the `--samtools` and `--minimap2` parameters.
 - `--minimap2`: path to minimap2
 
 ## Interpreting the output
 
-Paraphase produces a few output files in the directory specified by `-o`, with the sample ID as the prefix.
+Paraphase produces a few output files in the directory specified by `-o`, with the specified or default prefix.
 
-1. `.vcf` in `sampleID_vcfs` folder. A VCF file is written for each haplotype per gene family. There is also a `_variants.vcf` file containing merged variants from all haplotypes for each gene family. Note that this is not a diploid vcf as there are usually more than two copies of genes in a gene family in a sample.
+1. `.vcf` in `${prefix}_paraphase_vcfs` folder. A VCF file is written for each region (gene family). More descriptions on the VCF can be found [here](docs/vcf.md).
 
-As genes of the same family can be highly similar to each other in sequence and not easy to differentiate (at the sequence level or even at the functional level), variant calls are made against one selected "main" gene from the gene family (e.g. the functional gene is selected when the family has a gene and a pseudogene). In this way, all copies of the gene family can be evaluated for pathogenic variants and one can calculate the copy number of the functional genes in the family and hence infer the disease/carrier status.
+2. `.paraphase.bam`: This BAM file can be loaded into IGV for visualization of haplotypes (group reads by `HP` tag and color alignments by `YC` tag). All haplotypes are aligned against the main gene of interest. Tutorials/Examples are provided for medically relevant genes (See below).  
 
-Exceptions are SMN1 (paralog SMN2), PMS2 (pseudogene PMS2CL), STRC (pseudogene STRCP1), NCF1 (pseudogenes NCF1B and NCF1C) and IKBKG (pseudogene IKBKGP1), where gene differentiation is possible. In these families, haplotypes are assigned to each gene in the family, i.e. gene or paralog/pseudogene, and variants are called against the gene (or paralog/pseudogene) for the gene (or paralog/pseudogene) haplotypes, respectively. Variants calls can be made against the main gene only for these five families if `--gene1only` is specified. 
-
-2. `_realigned_tagged.bam`: This BAM file can be loaded into IGV for visualization of haplotypes (group reads by `HP` tag and color alignments by `YC` tag). All haplotypes are aligned against the main gene of interest. Tutorials/Examples are provided for medically relevant genes (See below).  
-
-3. `.json`: Output file summarizing haplotypes and variant calls for each gene family in each sample. In brief, a few generally used fields are explained below.
+3. `.paraphase.json`: Output file summarizing haplotypes and variant calls for each gene family in each sample. In brief, a few generally used fields are explained below.
 - `final_haplotypes`: phased haplotypes for all gene copies in a gene family
 - `total_cn`: total copy number of the family (sum of gene and paralog/pseudogene)
 - `two_copy_haplotypes`: haplotypes that are present in two copies based on depth. This happens when (in a small number of cases) two haplotypes are identical and we infer that there exist two of them instead of one by checking the read depth.
 - `haplotype_details`: lists information about each haplotype 
   - `boundary`: the boundary of the region that is resolved on the haplotype. This is useful when a haplotype is only partially phased.
 - `alleles_final`: haplotypes phased into alleles. This is possible when the segmental duplication is in tandem.
-- `region_depth`: median depth of the gene family (include all copies of gene and paralog/pseudogene) 
 
 Tutorials/Examples are provided for interpreting the `json` output and visualizing haplotypes for medically relevant genes listed below: 
 - [SMN1/SMN2](docs/SMN1_SMN2.md)
 - [RCCX module (CYP21A2)](docs/RCCX.md)
 - [PMS2](docs/PMS2.md)
 - [STRC](docs/STRC.md)
 - [OPN1LW/OPN1MW](docs/OPN1LW_OPN1MW.md)
 - [HBA1/HBA2](docs/HBA1_HBA2.md)
 - [IKBKG](docs/IKBKG.md)
 - [F8](docs/F8.md)
 - [NEB](docs/NEB.md)
 - [NCF1](docs/NCF1.md)
+- [GBA](docs/GBA.md)
+- [CFH gene cluster](docs/CFH.md)
+
```

### Comparing `paraphase-3.0.0/paraphase/data/19/config.yaml` & `paraphase-3.1.0/paraphase/data/19/config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,22 @@
   del1_3p_pos2: 70213622
   del1_5p_pos1: 70216894
   del1_5p_pos2: 70217087
 pms2: 
   genes: PMS2
   check_nm: 0.1
   realign_region: chr7:6004631-6049631
-  extract_regions: chr7:6004631-6028693 chr7:6775260-6799427
-  gene2_region: chr7:6775260-6799427
-  right_boundary: 6027131
+  extract_regions: chr7:6004631-6033041 chr7:6773174-6799427
+  gene2_region: chr7:6773174-6799427
+  right_boundary: 6033081
   pivot_site: 6026200
-  noisy_region: [[6020511, 6020611], [6019294, 6019300], [6015581, 6015711]]
+  noisy_region: [[6020511, 6020611], [6019294, 6019300], [6015581, 6015711], [6028131, 6031981], [6032411, 6033031]]
   is_reverse: True
   add_sites: ["6026200_G_A"]
+  clip_3p_positions: [6033041]
 rccx: 
   genes: CYP21A2,C4A,C4B,TNXB
   is_tandem: True
   data:
     snp_file: cyp21_diff_sites.txt
   realign_region: chr6:31981017-32016777
   extract_regions: chr6:31947777-32014577
@@ -50,15 +51,15 @@
   clip_3p_positions: [32013904]
   clip_5p_positions: [31981047]
   deletion1_size: 6367
   deletion2_size: 120
   deletion1_name: "31985208_del_6367"
   deletion2_name: "32011495_del_120"
   left_boundary: 31981077
-  right_boundary: 32013777
+  right_boundary: 32013977
   # 120bp sv
   del2_3p_pos1: 32011477
   del2_3p_pos2: 32011500
   del2_5p_pos1: 32011605
   del2_5p_pos2: 32011642
   # 6.3kb sv in C4B
   del1_3p_pos1: 31985177
@@ -82,16 +83,16 @@
   deletion1_name: "43894828_del_314"
   del1_3p_pos1: 43894826
   del1_3p_pos2: 43894829
   del1_5p_pos1: 43895142
   del1_5p_pos2: 43895146
 cfc1:
   genes: CFC1,CFC1B
-  realign_region: chr2:131349573-131367573
-  extract_regions: chr2:131268326-131291314 chr2:131344573-131367573
+  realign_region: chr2:131349573-131362573
+  extract_regions: chr2:131268326-131291314 chr2:131344573-131362573
   pivot_site: 131350634
   is_reverse: True
   add_sites: ["131350634_A_G"]
 ikbkg: 
   genes: IKBKG
   use_supplementary: True
   realign_region: chrX:153783815-153803263
@@ -158,12 +159,10 @@
   exon3_variants: [[["153418460_C_A"], "M", "L"], [["153418514_G_A", "153418516_G_T"], "I", "V"], [["153418524_C_T"], "V", "A"], [["153418535_A_G"], "V", "I"], [["153418541_T_G"], "A", "S"]]
 hba:
   genes: HBA1,HBA2
   realign_region: chr16:221799-223899
   extract_regions: chr16:218655-227540
   clip_5p_positions: [221988]
   clip_3p_positions: [223728]
-  gene_start: 221988
-  gene_end: 223728
   is_tandem: True
   depth_region: [[209999, 239999]]
   noisy_region: [[222416, 222417]]
```

### Comparing `paraphase-3.0.0/paraphase/data/19/genome_region.bed` & `paraphase-3.1.0/paraphase/data/19/genome_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/data/19/sex_region.bed` & `paraphase-3.1.0/paraphase/data/19/sex_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/data/19/smn1/known_haplotypes.json` & `paraphase-3.1.0/paraphase/data/19/smn1/known_haplotypes.json`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/data/38/config.yaml` & `paraphase-3.1.0/paraphase/data/38/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,22 @@
   del1_3p_pos2: 70917795
   del1_5p_pos1: 70921067
   del1_5p_pos2: 70921260
 pms2: 
   genes: PMS2
   check_nm: 0.1
   realign_region: chr7:5965000-6010000
-  extract_regions: chr7:5965000-5989062 chr7:6735629-6759796
-  gene2_region: chr7:6735629-6759796
-  right_boundary: 5987500
+  extract_regions: chr7:5965000-5993410 chr7:6733543-6759796
+  gene2_region: chr7:6733543-6759796
+  right_boundary: 5993450
   pivot_site: 5986569
-  noisy_region: [[5980880, 5980980], [5979663, 5979669], [5975950, 5976080]]
+  noisy_region: [[5980880, 5980980], [5979663, 5979669], [5975950, 5976080], [5988500, 5992350], [5992780, 5993400]]
   is_reverse: True
   add_sites: ["5986569_G_A"]
+  clip_3p_positions: [5993410]
 rccx: 
   genes: CYP21A2,C4A,C4B,TNXB
   is_tandem: True
   data:
     snp_file: cyp21_diff_sites.txt
   realign_region: chr6:32013240-32049000
   extract_regions: chr6:31980000-32046800
@@ -50,15 +51,15 @@
   clip_3p_positions: [32046127]
   clip_5p_positions: [32013270]
   deletion1_size: 6367
   deletion2_size: 120
   deletion1_name: "32017431_del_6367"
   deletion2_name: "32043718_del_120"
   left_boundary: 32013300
-  right_boundary: 32046000
+  right_boundary: 32046200
   # 120bp sv
   del2_3p_pos1: 32043700
   del2_3p_pos2: 32043723
   del2_5p_pos1: 32043828
   del2_5p_pos2: 32043865
   # 6.3kb sv in C4B
   del1_3p_pos1: 32017400
@@ -82,16 +83,16 @@
   deletion1_name: "43602630_del_314"
   del1_3p_pos1: 43602628
   del1_3p_pos2: 43602631
   del1_5p_pos1: 43602944
   del1_5p_pos2: 43602948
 cfc1:
   genes: CFC1,CFC1B
-  realign_region: chr2:130592000-130610000
-  extract_regions: chr2:130510753-130533741 chr2:130587000-130610000
+  realign_region: chr2:130592000-130605000
+  extract_regions: chr2:130510753-130533741 chr2:130587000-130605000
   pivot_site: 130593061
   is_reverse: True
   add_sites: ["130593061_A_G"]
 ikbkg: 
   genes: IKBKG
   use_supplementary: True
   realign_region: chrX:154555600-154575000
@@ -158,120 +159,120 @@
   exon3_variants: [[["154152987_A_C"], "L", "M"], [["154153041_G_A", "154153043_G_T"], "I", "V"], [["154153051_C_T"], "V", "A"], [["154153062_A_G"], "V", "I"], [["154153068_G_T"], "S", "A"]]
 hba:
   genes: HBA1,HBA2
   realign_region: chr16:171800-173900
   extract_regions: chr16:168656-177541
   clip_5p_positions: [171989]
   clip_3p_positions: [173729]
-  gene_start: 171989
-  gene_end: 173729
   is_tandem: True
   depth_region: [[160000, 190000]]
   noisy_region: [[172417, 172418]]
 
 SSX2: 
   genes: SSX2,SSX2B
   is_tandem: True
   is_reverse: True
+  is_palindrome: True
   realign_region: chrX:52696000-52729000
   extract_regions: chrX:52696000-52762432
 SSX4: 
   genes: SSX4,SSX4B
   is_tandem: True
   is_reverse: True
+  is_palindrome: True
   realign_region: chrX:48380000-48396314
   extract_regions: chrX:48380000-48417000
   left_boundary: 48380500
-CR1:
-  genes: CR1
-  realign_region: chr1:207527100-207545700
-  extract_regions: chr1:207529087-207566209
-  is_tandem: True
-  check_nm: 0.02
+  noisy_region: [[48381096, 48381555]]
 CENPVL2:
   genes: CENPVL1,CENPVL2
   realign_region: chrX:51675000-51692963
   extract_regions: chrX:51675000-51692963 chrX:51700364-51718343  
   is_tandem: True
   is_reverse: True
+  is_palindrome: True
   noisy_region: [[51691779, 51691984]]
 DMRTC1:
   genes: DMRTC1,DMRTC1B,FAM236A,FAM236B,FAM236C,FAM236D
   realign_region: chrX:72861525-72944337
   extract_regions: chrX:72861526-72944337 chrX:72776489-72859301
   left_boundary: 72861527
   right_boundary: 72944336
   noisy_region: [[72943757, 72943880]]
   is_tandem: True
   is_reverse: True
+  is_palindrome: True
 XAGE1A:
   genes: XAGE1A,XAGE1B
   realign_region: chrX:52490000-52502000
   extract_regions: chrX:52490000-52502000 chrX:52510889-52522888  
   is_tandem: True
   is_reverse: True
 TRIM49D1:
   genes: TRIM49D1,TRIM49D2
   realign_region: chr11:89909105-89922500
   extract_regions: chr11:89909105-89922500 chr11:89923849-89935370
   left_boundary: 89909500
   right_boundary: 89922500
   clip_3p_positions: [89920623]
-  gene_end: 89920623
   is_tandem: True
   is_reverse: True
 CXorf51A:
   genes: CXorf51A,CXorf51B
   realign_region: chrX:146812425-146822425
   extract_regions: chrX:146812425-146822425 chrX:146802090-146812090
   is_tandem: True
   is_reverse: True
+  is_palindrome: True
+  noisy_region: [[146816220, 146816278]]
 DDT:
   genes: DDT,DDTL
   realign_region: chr22:23971000-23982905
   extract_regions: chr22:23971741-23982905 chr22:23958424-23969582
   left_boundary: 23972100
   is_tandem: True
   is_reverse: True
 H3C14:
   genes: H3C14,H3C15,H2AC18,H2AC19,H4C14,H4C15
-  realign_region: chr1:149828816-149845484
-  extract_regions: chr1:149828816-149843536 chr1:149850276-149865000
-  left_boundary: 149828816
-  right_boundary: 149843536
+  realign_region: chr1:149832000-149845484
+  extract_regions: chr1:149832000-149843536 chr1:149850276-149865000
+  clip_3p_positions: [149843518]
+  noisy_region: [[149837998, 149838086]]
   is_tandem: True
   is_reverse: True
 MBD3L2:
-  genes: MBD3L2,MBD3L2B
-  realign_region: chr19:7037528-7060528
-  extract_regions: chr19:7037528-7051624 chr19:7019148-7033227
+  genes: MBD3L2,MBD3L2B,MBD3L3,MBD3L4,MBD3L5
+  realign_region: chr19:7037528-7051735
+  extract_regions: chr19:7037528-7062000 chr19:7019148-7033227
   left_boundary: 7037528
   right_boundary: 7051623
   is_reverse: True
   is_tandem: True
+  clip_3p_positions: [7043226]
+  noisy_region: [[7042002, 7042106]]
 DEFA1:
   genes: DEFA1,DEFA1B,DEFA3
   realign_region: chr8:6974238-6991000
   extract_regions: chr8:6974238-7010103 chr8:7012454-7022661
   left_boundary: 6974300
   is_tandem: True
   check_nm: 0.1
-  noisy_region: [[6984000, 6985910]]
+  noisy_region: [[6975823, 6975828], [6984000, 6985910]]
   clip_3p_positions: [6985908]
-  keep_truncated: True
 CCZ1:
   genes: CCZ1
   realign_region: chr7:5898000-5930000
   extract_regions: chr7:5898000-5930000 chr7:6794958-6827006
   is_reverse: True
 CSAG2:
   genes: CSAG2,CSAG3,MAGEA2,MAGEA2B,MAGEA3,MAGEA6
   realign_region: chrX:152690000-152720620
   extract_regions: chrX:152690000-152720620 chrX:152747848-152778471
   is_reverse: True
+  is_palindrome: True
 OR4M2:
   genes: OR4M2,OR4N4,OR4M2B,OR4N4C
   realign_region: chr15:22071068-22105192
   extract_regions: chr15:22071068-22105192 chr15:21628482-21662721 chr15_KI270727v1_random:362857-396966
   noisy_region: [[22084673, 22084807]]
 RIMBP3B:
   genes: RIMBP3B,RIMBP3,RIMBP3C
@@ -332,40 +333,34 @@
   is_reverse: True
   expect_cn2: True
 PRY:
   genes: PRY,PRY2
   realign_region: chrY:22489897-22515137
   extract_regions: chrY:22489898-22515137 chrY:22071256-22096507 chrY:23680940-23702786 chrY:25967288-25989136
   left_boundary: 22493307
-  right_boundary: 
-  expect_cn2: True
 BPY2:
   genes: BPY2,BPY2B,BPY2C
   realign_region: chrY:22983763-23005965
   extract_regions: chrY:22983764-23005965 chrY:24617505-24639707 chrY:25030401-25052603
   left_boundary: 22983765
   right_boundary: 23005964
-  expect_cn2: True
 CHRNA7:
   genes: CHRNA7
-  realign_region: chr15:32030015-32173518
-  extract_regions: chr15:32030015-32173518 chr15:30360306-30375956
-  left_boundary: 32030015
-  right_boundary: 32173518
+  realign_region: chr15:32100015-32173518
+  extract_regions: chr15:32100015-32173518 chr15:30360306-30375956
   is_reverse: True
   clip_5p_positions: [32153206]
-CNTNAP3C:
+  noisy_region: [[32114013, 32114163]]
+CNTNAP3:
   genes: CNTNAP3,CNTNAP3C
-  realign_region: chr9:61330217-61453530
+  realign_region: chr9:39162500-39288814
   extract_regions: chr9:61330217-61453530 chr9:39165433-39288814
-  left_boundary: 61330217
-  right_boundary: 61453530
   is_reverse: True
   expect_cn2: True
-  noisy_region: [[61409346, 61409399], [61367691, 61367733]]
+  noisy_region: [[39209580, 39209791], [39251285, 39251389], [39253010, 39253051], [39257549, 39257559]]
 CTAGE6:
   genes: CTAGE6,CTAGE15
   realign_region: chr7:143746392-143762392
   extract_regions: chr7:143746393-143762392 chr7:143563074-143579072
   left_boundary: 143746394
   right_boundary: 143762392
   is_reverse: True
@@ -378,14 +373,15 @@
 CXorf49:
   genes: CXorf49,CXorf49B
   realign_region: chrX:71706328-71726328
   extract_regions: chrX:71706329-71726328 chrX:71755199-71775246
   left_boundary: 71706330
   right_boundary: 71726327
   is_reverse: True
+  is_palindrome: True
 
 DEFB109B:
   genes: DEFB109B,USP17L1,USP17L3,USP17L4,USP17L8
   realign_region: chr8:7306409-7339183
   extract_regions: chr8:7306410-7339183 chr8:7971187-8003955
   left_boundary: 7306411
   right_boundary: 7330000
@@ -394,14 +390,15 @@
 PRR23D1:
   genes: PRR23D1,PRR23D2
   realign_region: chr8:7531038-7546000
   extract_regions: chr8:7531039-7551038 chr8:7770002-7790002
   left_boundary: 7531040
   right_boundary: 7546000
   is_reverse: True
+  noisy_region: [[7538337, 7538352]]
 
 DEFB107A:
   genes: DEFB107A
   realign_region: chr8:7803718-7823718
   extract_regions: chr8:7803719-7823718 chr8:7487841-7517298
   left_boundary: 7803720
   right_boundary: 7823717
@@ -409,21 +406,23 @@
 DEFB105A:
   genes: DEFB105A,DEFB105B
   realign_region: chr8:7812442-7832442
   extract_regions: chr8:7813693-7832442 chr8:7479103-7497875
   left_boundary: 7813694
   right_boundary: 7832441
   is_reverse: True
+  noisy_region: [[7826969,7827750]]
 DEFB106A:
   genes: DEFB106A,DEFB106B
   realign_region: chr8:7817096-7837096
   extract_regions: chr8:7817097-7837096 chr8:7474458-7494461
   left_boundary: 7817098
   right_boundary: 7837095
   is_reverse: True
+  noisy_region: [[7826969,7827750]]
 DEFB104A:
   genes: DEFB104A,DEFB104B
   realign_region: chr8:7828839-7848839
   extract_regions: chr8:7828840-7848839 chr8:7462711-7482717
   left_boundary: 7828841
   right_boundary: 7848838
   is_reverse: True
@@ -459,16 +458,17 @@
   expect_cn2: True
 ZNF705D:
   genes: ZNF705D
   realign_region: chr8:12088838-12116016
   extract_regions: chr8:12088839-12116016 chr8:12335087-12362253 chr8:7930859-7955249
   left_boundary: 12088840
   right_boundary: 12116015
-  check_nm: 0.2
+  check_nm: 0.1
   noisy_region: [[12091626, 12101750]]
+  clip_5p_positions: [12091626]
 FAM86B1:
   genes: FAM86B1,FAM86B2
   realign_region: chr8:12180000-12200000
   extract_regions: chr8:12180000-12200000 chr8:12422319-12442278 chr8:8222630-8237853
   check_nm: 0.2
   clip_5p_positions: [12184797]
 
@@ -490,32 +490,32 @@
   genes: ETDA,ETDB
   realign_region: chrX:135242822-135262822
   extract_regions: chrX:135242823-135262822 chrX:135116125-135129713
   left_boundary: 135242824
   right_boundary: 135262822
   is_reverse: True
   clip_3p_positions: [135256413]
-  gene_end: 135256413
 FAM156A:
   genes: FAM156A,FAM156B
   realign_region: chrX:52942886-52962886
   extract_regions: chrX:52942887-52962886 chrX:52892928-52912927
   left_boundary: 52942888
   right_boundary: 52962885
   is_reverse: True
+  is_palindrome: True
 FAM246A:
   genes: FAM246A,FAM246B
   realign_region: chr22:21350950-21370950
   extract_regions: chr22:21350951-21370950 chr22:18624338-18644332
   left_boundary: 21350952
   right_boundary: 21370949
   is_reverse: True
 
 FCGR2C:
-  genes: FCGR2C
+  genes: FCGR2C,FCGR2B
   realign_region: chr1:161580571-161602000
   extract_regions: chr1:161580572-161594218 chr1:161662376-161676049
   left_boundary: 161580573
   right_boundary: 161601300
   clip_3p_positions: [161595612]
   noisy_region: [[161593000, 161595500]]
 FRG2:
@@ -554,47 +554,39 @@
   genes: GATD3
   realign_region: chr21:44129697-44149697
   extract_regions: chr21:44129698-44147864 chr21:5114188-5132354
   left_boundary: 44129699
   right_boundary: 44147500
   is_reverse: True
   expect_cn2: True
-
-GOLGA6L1:
-  genes: GOLGA6L1,GOLGA6L26
-  realign_region: chr15:23121944-23141944
-  extract_regions: chr15:23123715-23141944 chr15:23321180-23339370
-  left_boundary: 23123716
-  right_boundary: 23141943
 GOLGA6L24:
   genes: GOLGA6L24,GOLGA6L25
   realign_region: chr15:28342967-28362967
   extract_regions: chr15:28342968-28362967 chr15:28548676-28568662
   left_boundary: 28342969
   right_boundary: 28362966
   is_reverse: True
 GOLGA8A:
   genes: GOLGA8A,GOLGA8B
   realign_region: chr15:34378568-34438308
   extract_regions: chr15:34378799-34431301 chr15:34525011-34577508
   left_boundary: 34380000
   right_boundary: 34420000
+  noisy_region: [[34417325, 34417360]]
 GOLGA8F:
   genes: GOLGA8F,GOLGA8G
   realign_region: chr15:28375342-28395342
   extract_regions: chr15:28375343-28395342 chr15:28516294-28536276
   left_boundary: 28375344
   right_boundary: 28395341
   is_reverse: True
 GOLGA8K:
   genes: GOLGA8K,GOLGA8T
-  realign_region: chr15:32386445-32406445
+  realign_region: chr15:32389000-32406445
   extract_regions: chr15:32386446-32406445 chr15:30131900-30151905
-  left_boundary: 32386447
-  right_boundary: 32406444
   is_reverse: True
 GPAT2:
   genes: GPAT2
   realign_region: chr2:96018431-96038431
   extract_regions: chr2:96018431-96038431 chr2:95786150-95800198
   left_boundary: 96018431
   right_boundary: 96038430
@@ -619,14 +611,15 @@
 IQCK:
   genes: IQCK
   realign_region: chr16:19717771-19858967
   extract_regions: chr16:19760000-19830000 chr13:86252980-86269524
   left_boundary: 19760000
   right_boundary: 19830000
   expect_cn2: True
+  noisy_region: [[19786695, 19786930], [19792759, 19792771]]
 LGALS9B:
   genes: LGALS9B,LGALS9C
   realign_region: chr17:20448467-20468467
   extract_regions: chr17:20448468-20468467 chr17:18475856-18495871
   left_boundary: 20448469
   right_boundary: 20468466
   is_reverse: True
@@ -648,14 +641,15 @@
   genes: MAGEH1
   realign_region: chrX:55442846-55462846
   extract_regions: chrX:55453508-55462846 chrX:55510356-55519694
   left_boundary: 55451000
   right_boundary: 55462845
   clip_5p_positions: [55453508]
   is_reverse: True
+  is_palindrome: True
 MALL:
   genes: MALL
   realign_region: chr2:110083370-110118500
   extract_regions: chr2:110083371-110118500 chr2:110276211-110288005
   left_boundary: 110083372
   right_boundary: 110118500
   is_reverse: True
@@ -669,22 +663,16 @@
   expect_cn2: True
 NOTCH2:
   genes: NOTCH2,NOTCH2NLR
   realign_region: chr1:119980000-120070162
   extract_regions: chr1:120008822-120070162 chr1:120723414-120784768
   left_boundary: 120008823
   right_boundary: 120069700
-  noisy_region: [[120024344, 120024352]]
+  noisy_region: [[120024344, 120024352], [120019785, 120019790]]
   is_reverse: True
-NPIPA1:
-  genes: NPIPA1
-  realign_region: chr16:14934749-14954749
-  extract_regions: chr16:14934750-14952002 chr16:16333237-16350465
-  left_boundary: 14934751
-  right_boundary: 14952001
 NPIPA2:
   genes: NPIPA2,NPIPA3
   realign_region: chr16:14742033-14765962
   extract_regions: chr16:14742034-14765962 chr16:14702912-14726842
   left_boundary: 14742035
   right_boundary: 14765961
 NPY4R:
@@ -703,14 +691,15 @@
 NXF2:
   genes: NXF2,NXF2B
   realign_region: chrX:102246667-102327222
   extract_regions: chrX:102246668-102327222 chrX:102359893-102440441
   left_boundary: 102300000
   right_boundary: 102327221
   is_reverse: True
+  is_palindrome: True
 OCLN:
   genes: OCLN
   realign_region: chr5:69492290-69558604
   extract_regions: chr5:69492290-69558604 chr5:71069293-71093996
   left_boundary: 69492290
   right_boundary: 69558603
   is_reverse: True
@@ -747,23 +736,25 @@
   genes: PABPC1L2A,PABPC1L2B
   realign_region: chrX:73068394-73088394
   extract_regions: chrX:73068394-73086958 chrX:72996065-73005560
   left_boundary: 73068394
   right_boundary: 73086957
   clip_5p_positions: [73077480]
   is_reverse: True
-  gene_start: 73077480
+  is_palindrome: True
 PDPK1:
   genes: PDPK1
   realign_region: chr16:2537521-2603688
   extract_regions: chr16:2537521-2603688 chr16:2615333-2648513
   left_boundary: 2537521
   right_boundary: 2599224
   clip_3p_positions: [2584851]
   is_reverse: True
+  use_r2k: True
+  noisy_region: [[2551657, 2552272]]
 POTEE:
   genes: POTEE,POTEF
   realign_region: chr2:131209036-131265778
   extract_regions: chr2:131209037-131265778 chr2:130073149-130129844
   left_boundary: 131209038
   right_boundary: 131265777
   is_reverse: True
@@ -799,42 +790,40 @@
 PRAMEF7:
   genes: PRAMEF7,PRAMEF8
   realign_region: chr1:12908680-12928680
   extract_regions: chr1:12908681-12928680 chr1:13273109-13293100
   left_boundary: 12908682
   right_boundary: 12928679
   is_reverse: True
-PRAMEF5:
-  genes: PRAMEF5,PRAMEF6
-  realign_region: chr1:13248816-13268816
-  extract_regions: chr1:13248817-13268816 chr1:12932973-12952975
-  left_boundary: 13248818
-  right_boundary: 13268815
-  is_reverse: True
+  noisy_region: [[12915463, 12915676]]
 PRAMEF25:
   genes: PRAMEF25,PRAMEF26,HNRNPCL3,HNRNPCL4
   realign_region: chr1:13058000-13084329
   extract_regions: chr1:13058000-13084329 chr1:13142460-13171013
   left_boundary: 13058000
   right_boundary: 13084329
   is_reverse: True
+  check_nm: 0.02
+  clip_5p_positions: [13075113]
 PRAMEF13:
   genes: PRAMEF13
   realign_region: chr1:13191500-13208798
   extract_regions: chr1:13188799-13208798 chr1:13020162-13040136
   left_boundary: 13191500
   right_boundary: 13208797
   is_reverse: True
+  noisy_region: [[13203300, 13203576]]
 PRAMEF18:
   genes: PRAMEF18
-  realign_region: chr1:13220000-13234424
+  realign_region: chr1:13220900-13234424
   extract_regions: chr1:13220000-13234424 chr1:13004385-13014535
   left_boundary: 13220900
   right_boundary: 13234424
   is_reverse: True
+  clip_5p_positions: [13224057]
 
 POTED:
   genes: POTED
   realign_region: chr21:13609277-13646323
   extract_regions: chr21:13609278-13646288 chrUn_GL000213v1:103302-140211
   left_boundary: 13609279
   right_boundary: 13646287
@@ -896,14 +885,15 @@
 RGPD3:
   genes: RGPD3,RGPD4
   realign_region: chr2:106402906-106468913
   extract_regions: chr2:106402907-106466996 chr2:107828900-107893038
   left_boundary: 106402908
   right_boundary: 106466000
   is_reverse: True
+  noisy_region: [[106425157, 106425170]]
 RHOXF2:
   genes: RHOXF2,RHOXF2B
   realign_region: chrX:120152121-120172121
   extract_regions: chrX:120152122-120172121 chrX:120064181-120084181
   left_boundary: 120152123
   right_boundary: 120172120
   is_reverse: True
@@ -991,14 +981,15 @@
   genes: TMLHE
   realign_region: chrX:155488511-155613452
   extract_regions: chrX:155488512-155504550 chrX:155336693-155352737
   clip_3p_positions: [155504550]
   left_boundary: 155488513
   right_boundary: 155510000
   is_reverse: True
+  is_palindrome: True
 TRIM49:
   genes: TRIM49,TRIM49C
   realign_region: chr11:89793115-89813115
   extract_regions: chr11:89793116-89811854 chr11:90027825-90046559
   left_boundary: 89793117
   right_boundary: 89811853
   is_reverse: True
@@ -1022,18 +1013,17 @@
   extract_regions: chr21:43090264-43110263 chr21:6481931-6501941
   left_boundary: 43090265
   right_boundary: 43110262
   expect_cn2: True
 
 UPK3BL1: 
   genes: UPK3BL1,UPK3BL2
-  realign_region: chr7:102629908-102649908
+  realign_region: chr7:102629908-102646500
   extract_regions: chr7:102629909-102649908 chr7:102530825-102550815
-  left_boundary: 102629910
-  right_boundary: 102649907
+  noisy_region: [[102639951, 102640023]]
 POLR2J2:
   genes: POLR2J2,POLR2J3
   realign_region: chr7:102658854-102678854
   extract_regions: chr7:102658855-102678854 chr7:102559768-102579794
   left_boundary: 102658856
   right_boundary: 102678853
 
@@ -1043,28 +1033,28 @@
   extract_regions: chr4:52822-88708 chrUn_KI270744v1:125448-141446
   clip_3p_positions: [68825]
   left_boundary: 52823
   right_boundary: 88300
 
 FOXD4L4:
   genes: FOXD4L4,FOXD4L5
-  realign_region: chr9:65727771-65747771
-  extract_regions: chr9:65727772-65747771 chr9:65273748-65293756 chr9:68293705-68301609
+  realign_region: chr9:65727771-65740000
+  extract_regions: chr9:65727772-65740000 chr9:65281523-65293756 chr9:68293705-68301609
   left_boundary: 65727773
   right_boundary: 65738784
   is_reverse: True
-  check_nm: 0.2
   noisy_region: [[65735600, 65735970]]
 FOXD4L3:
   genes: FOXD4L3,FOXD4L6
   realign_region: chr9:68293975-68313975
   extract_regions: chr9:68293976-68313975 chr9:41117361-41137343
   left_boundary: 68293977
   right_boundary: 68313974
   is_reverse: True
+  check_nm: 0.012
 
 GTF2IRD2B:
   genes: GTF2IRD2B,GTF2IRD2
   realign_region: chr7:75092090-75150317
   extract_regions: chr7:75092091-75150317 chr7:74795644-74852041
   left_boundary: 75092092
   right_boundary: 75150316
@@ -1082,19 +1072,18 @@
   left_boundary: 44221969
   right_boundary: 44241966
   is_reverse: True
   noisy_region: [[44229611, 44229631], [44225597, 44225597]]
   expect_cn2: True
 MAGED4:
   genes: MAGED4,MAGED4B
-  realign_region: chrX:52178578-52198578
+  realign_region: chrX:52182000-52198578
   extract_regions: chrX:52178579-52198578 chrX:52055517-52075516
-  left_boundary: 52178580
-  right_boundary: 52198577
   is_reverse: True
+  is_palindrome: True
 CBS:
   genes: CBS
   realign_region: chr21:43052691-43076335
   extract_regions: chr21:43052692-43076335 chr21:6444370-6468013
   left_boundary: 43052693
   right_boundary: 43076334
   expect_cn2: True
@@ -1123,20 +1112,22 @@
 CASTOR2:
   genes: CASTOR2
   realign_region: chr7:74964205-75032028
   extract_regions: chr7:74964206-75032028 chr7:73156189-73174784 chr7:75217889-75238192
   left_boundary: 74965884
   right_boundary: 75032028
   clip_3p_positions: [74984489]
+  noisy_region: [[74976525, 74976574]]
 CLEC18C:
   genes: CLEC18A,CLEC18B,CLEC18C
-  realign_region: chr16:70170341-70190341
+  realign_region: chr16:70170341-70187341
   extract_regions: chr16:70170342-70190341 chr16:69947429-69967427 chr16:74405201-74425232
-  left_boundary: 70170343
-  right_boundary: 70190340
+  clip_5p_positions: [70180660]
+  noisy_region: [[70171285, 70171320], [70174152, 70174163]]
+  use_supplementary: True
 GTF2H2:
   genes: GTF2H2,GTF2H2C
   realign_region: chr5:71034847-71068176
   extract_regions: chr5:71034848-71068176 chr5:69559721-69593027 chr5:70414868-70448182
   left_boundary: 71034849
   right_boundary: 71068175
 GTF2I:
@@ -1156,14 +1147,15 @@
 NBPF4:
   genes: NBPF4,NBPF6
   realign_region: chr1:108221964-108244576
   extract_regions: chr1:108222602-108244576 chr1:108449787-108471742 chr1:108375304-108383706
   left_boundary: 108223000
   right_boundary: 108244575
   clip_5p_positions: [108236178]
+  noisy_region: [[108231294, 108231299]]
 PPIAL4D:
   genes: PPIAL4D,PPIAL4E,PPIAL4F
   realign_region: chr1:145231794-145251794
   extract_regions: chr1:145235770-145251794 chr1:144367229-144383246 chr1:144583278-144599298
   left_boundary: 145235771
   right_boundary: 145251793
 RGPD5:
@@ -1176,62 +1168,60 @@
   genes: FAM72A
   realign_region: chr1:206184509-206204509
   extract_regions: chr1:206184510-206204509 chr1:121165986-121185983 chr1:143953624-143973625 chr1:145094364-145114349
   left_boundary: 206184511
   right_boundary: 206204508
 GOLGA8N:
   genes: GOLGA8N,GOLGA8O,GOLGA8Q,GOLGA8R
-  realign_region: chr15:32590346-32610346
+  realign_region: chr15:32590346-32607237
   extract_regions: chr15:32590347-32607507 chr15:30400208-30417365 chr15:30548871-30566038 chr15:32441569-32458746
   left_boundary: 32590348
   right_boundary: 32606000
+  check_nm: 0.02
 POTEB:
-  genes: POTEB,POTEB2,POTE3
+  genes: POTEB,POTEB2,POTEB3
   realign_region: chr15:21845829-21878235
   extract_regions: chr15:21845830-21878235 chr15:20834873-20867269 chr15:21408465-21439843 chr15_KI270727v1_random:135661-167032
   left_boundary: 21845831
   right_boundary: 21877188
-SPATA31A1:
-  genes: SPATA31A1,SPATA31A3,SPATA31A5,SPATA31A7
-  realign_region: chr9:39348815-39368815
-  extract_regions: chr9:39348816-39368815 chr9:60907506-60927532 chr9:61184485-61203156 chr9:66979422-66998101
-  left_boundary: 39350176
-  right_boundary: 39368814
 NUTM2A:
   genes: NUTM2A,NUTM2B,NUTM2D,NUTM2E
   realign_region: chr10:87220213-87240213
   extract_regions: chr10:87220214-87240213 chr10:79697989-79718012 chr10:87354483-87369657 chr10:79838172-79853341
-  left_boundary: 87222272
-  right_boundary: 87237439
+  clip_5p_positions: [87222271]
+  clip_3p_positions: [87236514, 87237440]
 ANKRD20A1:
   genes: ANKRD20A1
   realign_region: chr9:67858431-67902894
   extract_regions: chr9:67858432-67902894 chr9:40223065-40266892 chr9:64368680-64413189 chr9:66109347-66153849
   left_boundary: 67859093
   right_boundary: 67902893
+  noisy_region: [[67859646, 67859662]]
 GRAPL:
   genes: GRAPL,GRAP
   realign_region: chr17:19127089-19159687
   extract_regions: chr17:19127089-19159687 chr17:19025179-19047456 chr17:19092398-19103046 chr17:19218567-19229213
   left_boundary: 19127089
   right_boundary: 19159687
   clip_5p_positions: [19149042]
   clip_3p_positions: [19149358]
 ARL17A:
   genes: ARL17A,ARL17B
   realign_region: chr17:46552256-46580191
   extract_regions: chr17:46552257-46580191 chr17:46334404-46362266
   left_boundary: 46552258
   right_boundary: 46580190
+  clip_3p_positions: [46565080]
 NSF:
   genes: NSF
   realign_region: chr17:46590169-46757964
   extract_regions: chr17:46590170-46707123 chr17:46372249-46489410
   left_boundary: 46590171
   right_boundary: 46707122
+  noisy_region: [[46609984, 46610171]]
 
 AMY1A:
   genes: AMY1A,AMY1B,AMY1C
   realign_region: chr1:103650157-103669000
   extract_regions: chr1:103650158-103668000 chr1:103684093-103701812 chr1:103744296-103762027
   left_boundary: 103650159
   right_boundary: 103667870
@@ -1243,17 +1233,75 @@
   genes: CTAG1A,CTAG1B
   realign_region: chrX:154575974-154592000
   extract_regions: chrX:154575975-154591500 chrX:154613097-154628455
   left_boundary: 154575976
   right_boundary: 154591300
   clip_3p_positions: [154591326]
   is_reverse: True
+  is_palindrome: True
   add_sites: ["154591380_A_G"]
 BOLA2:
   genes: BOLA2,BOLA2B,SLX1A,SLX1B,SULT1A3,SULT1A4
   realign_region: chr16:29448000-29470000
   extract_regions: chr16:29449191-29472438 chr16:30188529-30211782
   left_boundary: 29449200
   right_boundary: 29470000
   clip_5p_positions: [29449191]
   add_sites: ["29449010_T_G"]
-  
+
+CYP2D6:
+  genes: CYP2D6
+  realign_region: chr22:42122800-42132500
+  extract_regions: chr22:42123196-42145723
+  gene2_region: chr22:42135344-42145873
+  use_r2k: True
+  is_tandem: True
+  check_nm: 0.07
+  noisy_region: [[42125955, 42126005], [42132023, 42132051]]
+  clip_5p_positions: [42123192]
+  clip_3p_positions: [42132193]
+  call_fusion: 5p
+GBA:
+  genes: GBA1
+  realign_region: chr1:155230000-155242500
+  extract_regions: chr1:155210828-155219269 chr1:155230976-155241500
+  gene2_region: chr1:155210380-155219657
+  check_nm: 0.2
+  use_r2k: True
+  noisy_region: [[155236583, 155237172], [155238947, 155239582], [155240160, 155240489], [155241400, 155241900]]
+  use_supplementary: True
+  clip_5p_positions: [155230976]
+  clip_3p_positions: [155242229]
+  call_fusion: 3p
+CYP11B1:
+  genes: CYP11B1,CYP11B2
+  realign_region: chr8:142872000-142880500
+  extract_regions: chr8:142872000-142880500 chr8:142910559-142917843
+  gene2_region: chr8:142910760-142917977
+  check_nm: 0.2
+  use_r2k: True
+  noisy_region: [[142874825, 142874950]]
+  clip_5p_positions: [142873164]
+  clip_3p_positions: [142879950]
+  call_fusion: 5p
+CFH:
+  genes: CFH,CFHR1
+  realign_region: chr1:196740000-196772000
+  extract_regions: chr1:196740000-196772000 chr1:196827188-196855916
+  gene2_region: chr1:196827188-196855916
+  check_nm: 0.1
+  use_r2k: True
+  clip_5p_positions: [196742575]
+  clip_3p_positions: [196771224]
+  noisy_region: [[196748050, 196748125], [196768556, 196768896]]
+  call_fusion: 5p
+CFHR3:
+  genes: CFHR3,CFHR4,CFHR1,CFHR2
+  realign_region: chr1:196786000-196830000
+  extract_regions: chr1:196786000-196830000 chr1:196911478-196948804
+  gene2_region: chr1:196911478-196948804
+  check_nm: 0.1
+  use_r2k: True
+  clip_5p_positions: [196786955]
+  clip_3p_positions: [196827189]
+  noisy_region: [[196809513, 196812537], [196817000, 196817020], [196826466, 196826515]]
+  call_fusion: 5p
```

### Comparing `paraphase-3.0.0/paraphase/data/38/genome_region.bed` & `paraphase-3.1.0/paraphase/data/38/genome_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/data/38/sex_region.bed` & `paraphase-3.1.0/paraphase/data/38/sex_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/data/38/smn1/known_haplotypes.json` & `paraphase-3.1.0/paraphase/data/38/smn1/known_haplotypes.json`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/genes/cfc1_phaser.py` & `paraphase-3.1.0/paraphase/genes/cfc1_phaser.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             nonuniquely_supporting_reads,
             raw_read_haps,
             read_counts,
         ) = self.phase_haps(raw_read_haps)
 
         tmp = {}
         for i, hap in enumerate(ass_haps):
-            tmp.setdefault(hap, f"hap{i+1}")
+            tmp.setdefault(hap, f"{self.gene}_hap{i+1}")
         ass_haps = tmp
 
         haplotypes = None
         if self.het_sites != []:
             haplotypes = self.output_variants_in_haplotypes(
                 ass_haps,
                 uniquely_supporting_reads,
@@ -59,14 +59,18 @@
                 cp2_hap = haps[counts.index(max_count)]
                 others_max = sorted(counts, reverse=True)[1]
                 probs = self.depth_prob(max_count, others_max)
                 if probs[0] < 0.15 and others_max >= 10:
                     two_cp_haps.append(ass_haps[cp2_hap])
 
         total_cn = len(ass_haps) + len(two_cp_haps)
+
+        if self.het_sites == []:
+            total_cn = 4
+
         if total_cn < 4:
             total_cn = None
 
         self.close_handle()
 
         return self.GeneCall(
             total_cn,
@@ -83,8 +87,9 @@
             self.homo_sites,
             haplotypes,
             nonuniquely_supporting_reads,
             raw_read_haps,
             self.mdepth,
             self.region_avg_depth._asdict(),
             self.sample_sex,
+            None,
         )
```

### Comparing `paraphase-3.0.0/paraphase/genes/f8_phaser.py` & `paraphase-3.1.0/paraphase/genes/f8_phaser.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,27 +127,27 @@
         h1_count = 0
         h2_count = 0
         h3_count = 0
         unknown_count = 0
         for i, hap in enumerate(ass_haps):
             if len(hap) < 3:
                 unknown_count += 1
-                hap_name = f"unknown_hap{unknown_count}"
+                hap_name = f"{self.gene}_unknown_hap{unknown_count}"
             elif hap[-2:] == "00":
                 h1_count += 1
-                hap_name = f"int22h1_hap{h1_count}"
+                hap_name = f"{self.gene}_int22h1_hap{h1_count}"
             elif hap[-1] == "0" and hap[-2] != "x":
                 h3_count += 1
-                hap_name = f"int22h3_hap{h3_count}"
+                hap_name = f"{self.gene}_int22h3_hap{h3_count}"
             elif "x" not in hap[-2:] and "0" not in hap[-2:]:
                 h2_count += 1
-                hap_name = f"int22h2_hap{h2_count}"
+                hap_name = f"{self.gene}_int22h2_hap{h2_count}"
             else:
                 unknown_count += 1
-                hap_name = f"unknown_hap{unknown_count}"
+                hap_name = f"{self.gene}_unknown_hap{unknown_count}"
             tmp.setdefault(hap, hap_name)
         ass_haps = tmp
 
         haplotypes = None
         if self.het_sites != []:
             haplotypes = self.output_variants_in_haplotypes(
                 ass_haps,
@@ -188,14 +188,20 @@
                             sv_hap.setdefault(hap, "deletion")
                     if self.sample_sex == "male":
                         if e1_e22_depth < 1:
                             sv_hap.setdefault(hap, "deletion")
             elif links == "region1-region3" and "int22h3" in hap:
                 sv_hap.setdefault(hap, "inversion")
 
+        if sv_hap == {} and self.sample_sex is not None:
+            if self.sample_sex == "female" and total_cn < 6:
+                total_cn = None
+            if self.sample_sex == "male" and total_cn < 3:
+                total_cn = None
+
         self.close_handle()
 
         return self.GeneCall(
             total_cn,
             ass_haps,
             [],
             e1_e22_depth,
```

### Comparing `paraphase-3.0.0/paraphase/genes/hba_phaser.py` & `paraphase-3.1.0/paraphase/genes/hba_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/genes/ikbkg_phaser.py` & `paraphase-3.1.0/paraphase/genes/ikbkg_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/genes/ncf1_phaser.py` & `paraphase-3.1.0/paraphase/genes/ncf1_phaser.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,21 +79,21 @@
         for hap_seq, hap in ass_haps.items():
             var = haplotypes[hap]["variants"]
             if self.pivot_var not in var:
                 hap_reads = uniquely_supporting_reads[hap_seq]
                 hap_var = [var_reads.get(a) for a in hap_reads]
                 if hap_var.count("alt") > (len(hap_var) - hap_var.count(None)) * 0.7:
                     counter_pseudo += 1
-                    hap_rename.setdefault(hap, f"pseudo_hap{counter_pseudo}")
+                    hap_rename.setdefault(hap, f"ncf1_pseudo_hap{counter_pseudo}")
                 else:
                     counter_gene += 1
                     hap_rename.setdefault(hap, f"ncf1_hap{counter_gene}")
             else:
                 counter_pseudo += 1
-                hap_rename.setdefault(hap, f"pseudo_hap{counter_pseudo}")
+                hap_rename.setdefault(hap, f"ncf1_pseudo_hap{counter_pseudo}")
 
         tmp = {}
         for hap, hap_name in ass_haps.items():
             tmp.setdefault(hap, hap_rename[hap_name])
         ass_haps = tmp
 
         tmp = {}
```

### Comparing `paraphase-3.0.0/paraphase/genes/neb_phaser.py` & `paraphase-3.1.0/paraphase/genes/neb_phaser.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             nonuniquely_supporting_reads,
             raw_read_haps,
             read_counts,
         ) = self.phase_haps(raw_read_haps)
 
         tmp = {}
         for i, hap in enumerate(ass_haps):
-            tmp.setdefault(hap, f"hap{i+1}")
+            tmp.setdefault(hap, f"{self.gene}_hap{i+1}")
         ass_haps = tmp
 
         haplotypes = None
         if self.het_sites != []:
             haplotypes = self.output_variants_in_haplotypes(
                 ass_haps,
                 uniquely_supporting_reads,
```

### Comparing `paraphase-3.0.0/paraphase/genes/opn1lw_phaser.py` & `paraphase-3.1.0/paraphase/genes/opn1lw_phaser.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,24 @@
         "sample_sex",
     )
     GeneCall = namedtuple(
         "GeneCall",
         fields,
         defaults=(None,) * len(fields),
     )
-    pathogenic_haps = ["LIAVA", "LVAVA", "LIAVS", "MIAVA", "MVVVA", "MVAVA", "LIAIA"]
+    pathogenic_haps = [
+        "LIAVA",
+        "LVAVA",
+        "LIAVS",
+        "MIAVA",
+        "MVVVA",
+        "MVAVA",
+        "LIAIA",
+        "LIVVA",
+    ]
 
     def __init__(
         self, sample_id, outdir, genome_depth=None, genome_bam=None, sample_sex=None
     ):
         Phaser.__init__(self, sample_id, outdir, genome_depth, genome_bam, sample_sex)
 
     def set_parameter(self, config):
@@ -239,16 +248,15 @@
                 if var.intersection(last_copy_vars) != set():
                     last_copies.append(renamed_hap)
                 elif renamed_hap not in first_copies and "x" not in hap:
                     middle_copies.append(renamed_hap)
                 # annotate exon3
                 hap_annotated = self.call_exon3(var)
                 gene_annotated = renamed_hap.split("_")[0]
-                if hap_annotated in self.pathogenic_haps:
-                    gene_annotated += "_" + hap_annotated
+                gene_annotated += "_" + hap_annotated
                 annotated_haps.setdefault(renamed_hap, gene_annotated)
 
             tmp = {}
             for hap, hap_name in ass_haps.items():
                 tmp.setdefault(hap, hap_rename[hap_name])
             ass_haps = tmp
 
@@ -372,16 +380,15 @@
                 for each_allele in alleles_1st_2nd:
                     each_allele_annotated = []
                     for each_hap in each_allele:
                         if each_hap is not None:
                             hap_vars = haplotypes[each_hap]["variants"]
                             hap_annotated = self.call_exon3(hap_vars)
                             gene_annotated = each_hap.split("_")[0]
-                            if hap_annotated in self.pathogenic_haps:
-                                gene_annotated += "_" + hap_annotated
+                            gene_annotated += "_" + hap_annotated
                         else:
                             gene_annotated = None
                         each_allele_annotated.append(gene_annotated)
                     annotated_alleles.append(each_allele_annotated)
 
         # homozygous cases
         elif self.sample_sex is not None:
@@ -396,16 +403,15 @@
                 total_cn = baseline_cn
                 counter_mw = baseline_cn
                 gene_annotated = "opn1mw"
             else:
                 total_cn = baseline_cn
                 counter_lw = baseline_cn
                 gene_annotated = "opn1lw"
-            if hap_annotated in self.pathogenic_haps:
-                gene_annotated += "_" + hap_annotated
+            gene_annotated += "_" + hap_annotated
             annotated_alleles.append([gene_annotated])
             if self.sample_sex == "female":
                 annotated_alleles.append([gene_annotated])
 
         self.close_handle()
 
         return self.GeneCall(
```

### Comparing `paraphase-3.0.0/paraphase/genes/pms2_phaser.py` & `paraphase-3.1.0/paraphase/genes/pms2_phaser.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,17 @@
                 [self.del1_3p_pos1, self.del1_3p_pos2],
                 [self.del1_5p_pos1, self.del1_5p_pos2],
             ]
         self.get_candidate_pos()
         self.het_sites = sorted(list(self.candidate_pos))
         self.remove_noisy_sites()
         # for distinguishing pms2 from pms2cl
-        raw_read_haps = self.get_haplotypes_from_reads(add_sites=self.add_sites)
+        raw_read_haps = self.get_haplotypes_from_reads(
+            check_clip=True, add_sites=self.add_sites
+        )
 
         het_sites = self.het_sites
         known_del = {}
         if self.del1_reads_partial != set():
             raw_read_haps, het_sites = self.update_reads_for_deletions(
                 raw_read_haps,
                 het_sites,
@@ -62,28 +64,24 @@
             read_counts,
         ) = self.phase_haps(raw_read_haps)
 
         tmp = {}
         counter_gene = 0
         counter_pseudo = 0
         counter_unknown = 0
-        pivot_index, index_found = self.get_pivot_site_index()
-        if index_found is False:
-            return self.GeneCall()
         for hap in ass_haps:
-            start_seq = hap[pivot_index:]
-            if start_seq.count("2") >= 15:
+            if hap.endswith("x"):
+                counter_unknown += 1
+                hap_name = f"pms2_unknown_hap{counter_gene}"
+            elif hap.endswith("0"):
                 counter_pseudo += 1
                 hap_name = f"pms2clhap{counter_pseudo}"
-            elif start_seq.count("2") <= 5:
+            else:
                 counter_gene += 1
                 hap_name = f"pms2hap{counter_gene}"
-            else:
-                counter_unknown += 1
-                hap_name = f"pms2_unknown_hap{counter_gene}"
             tmp.setdefault(hap, hap_name)
         ass_haps = tmp
 
         haplotypes = None
         if self.het_sites != []:
             haplotypes = self.output_variants_in_haplotypes(
                 ass_haps,
@@ -129,8 +127,9 @@
             self.homo_sites,
             haplotypes,
             nonuniquely_supporting_reads,
             raw_read_haps,
             self.mdepth,
             self.region_avg_depth._asdict(),
             self.sample_sex,
+            None,
         )
```

### Comparing `paraphase-3.0.0/paraphase/genes/rccx_phaser.py` & `paraphase-3.1.0/paraphase/genes/rccx_phaser.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
             nonuniquely_supporting_reads,
             raw_read_haps,
             read_counts,
         ) = self.phase_haps(raw_read_haps)
 
         tmp = {}
         for i, hap in enumerate(ass_haps):
-            hap_name = f"hap{i+1}"
+            hap_name = f"{self.gene}_hap{i+1}"
             tmp.setdefault(hap, hap_name)
         final_haps = tmp
         # get haps that extend into tnxb
         ending_copies = [
             final_haps[a]
             for a in ass_haps
             if a[0] not in ["0", "x"] and a[-1] not in ["0", "x"]
```

### Comparing `paraphase-3.0.0/paraphase/genes/smn1_phaser.py` & `paraphase-3.1.0/paraphase/genes/smn1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/genes/strc_phaser.py` & `paraphase-3.1.0/paraphase/genes/strc_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/genome_depth.py` & `paraphase-3.1.0/paraphase/genome_depth.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/haplotype_assembler.py` & `paraphase-3.1.0/paraphase/haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/paraphase/paraphase.py` & `paraphase-3.1.0/paraphase/paraphase.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,23 +74,22 @@
         gene_list,
         configs,
         outdir,
         tmpdir,
         gdepth,
         bam,
         sample_sex,
-        novcf,
         prog_cmd,
-        gene1only=False,
+        sample_id,
+        args,
     ):
         """Workflow for each region"""
         phaser_calls = {}
         for gene in gene_list:
             try:
-                sample_id = bam.split("/")[-1].split(".")[0]
                 if gene == "smn1":
                     phaser = genes.Smn1Phaser(
                         sample_id, tmpdir, gdepth, bam, sample_sex
                     )
                 elif gene == "rccx":
                     phaser = genes.RccxPhaser(
                         sample_id, tmpdir, gdepth, bam, sample_sex
@@ -122,24 +121,24 @@
                 elif gene == "opn1lw":
                     phaser = genes.Opn1lwPhaser(
                         sample_id, tmpdir, gdepth, bam, sample_sex
                     )
                 elif gene == "hba":
                     phaser = genes.HbaPhaser(sample_id, tmpdir, gdepth, bam, sample_sex)
                 else:
-                    phaser = Phaser(sample_id, tmpdir, gdepth)
+                    phaser = Phaser(sample_id, tmpdir, gdepth, sample_sex=sample_sex)
 
                 config = configs[gene]
                 logging.info(
                     f"Running analysis for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
                 )
                 logging.info(
                     f"Realigning reads for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
                 )
-                bam_realigner = BamRealigner(bam, tmpdir, config, prog_cmd)
+                bam_realigner = BamRealigner(bam, tmpdir, config, prog_cmd, sample_id)
                 bam_realigner.write_realign_bam()
 
                 logging.info(
                     f"Phasing haplotypes for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
                 )
 
                 phaser.set_parameter(config)
@@ -156,19 +155,22 @@
                 if gene in self.two_reference_regions_genes:
                     logging.info(
                         f"Realigning to gene2 region for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
                     )
                     bam_realigner.write_realign_bam(gene2=True)
                     bam_tagger.write_bam(random_assign=True, gene2=True)
 
-                if novcf is False and gene not in self.no_vcf_genes:
+                if args.novcf is False and gene not in self.no_vcf_genes:
                     logging.info(
                         f"Generating VCFs for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
                     )
-                    if gene in self.two_reference_regions_genes and gene1only is False:
+                    if (
+                        gene in self.two_reference_regions_genes
+                        and args.gene1only is False
+                    ):
                         vcf_generater = TwoGeneVcfGenerater(
                             sample_id,
                             outdir,
                             phaser_call,
                         )
                         vcf_generater.set_parameter(
                             config, tmpdir=tmpdir, prog_cmd=prog_cmd
@@ -179,15 +181,16 @@
                             sample_id,
                             outdir,
                             phaser_call,
                         )
                         vcf_generater.set_parameter(
                             config, tmpdir=tmpdir, prog_cmd=prog_cmd
                         )
-                        vcf_generater.run_without_realign()
+                        vcf_generater.run()
+
             except Exception:
                 logging.error(
                     f"Error running {gene} for sample {sample_id}...See error message below"
                 )
                 traceback.print_exc()
                 phaser_calls.setdefault(gene, None)
         return phaser_calls
@@ -195,24 +198,31 @@
     def process_sample(
         self,
         bamlist,
         outdir,
         configs,
         tmpdir,
         prog_cmd,
+        args,
         num_threads=1,
         dcov={},
-        novcf=False,
         genome_build="38",
-        gene1only=False,
     ):
         """Main workflow"""
         for bam in bamlist:
             try:
-                sample_id = bam.split("/")[-1].split(".")[0]
+                if args.prefix is not None and args.bam is not None:
+                    sample_id = args.prefix
+                else:
+                    sample_id_from_header = self.get_sample_id_from_header(bam)
+                    if sample_id_from_header is not None:
+                        sample_id = sample_id_from_header
+                    else:
+                        sample_id = bam.split("/")[-1].split(".")[0]
+
                 logging.info(
                     f"Processing sample {sample_id} at {datetime.datetime.now()}..."
                 )
                 sample_out = {}
                 gdepth = None
                 sample_sex = None
                 query_genes = list(configs.keys())
@@ -237,15 +247,17 @@
                     )
                     gdepth, gmad = depth.call()
                     if gdepth < 10 or gmad > 0.25:
                         logging.warning(
                             f"For sample {sample_id}, due to low or highly variable genome coverage, genome coverage is not used for depth correction."
                         )
                         gdepth = None
-                if set(query_genes).intersection(set(self.check_sex_genes)) != set():
+
+                # call sample sex
+                if True in ["X" in configs[a]["nchr"] for a in configs]:
                     logging.info(f"Checking sample sex at {datetime.datetime.now()}...")
                     depth = GenomeDepth(
                         bam,
                         os.path.join(
                             os.path.dirname(__file__),
                             "data",
                             genome_build,
@@ -259,59 +271,89 @@
                         query_genes,
                         configs,
                         outdir,
                         tmpdir,
                         gdepth,
                         bam,
                         sample_sex,
-                        novcf,
                         prog_cmd,
-                        gene1only,
+                        sample_id,
+                        args,
                     )
                 else:
                     process_gene_partial = partial(
                         self.process_gene,
                         configs=configs,
                         outdir=outdir,
                         tmpdir=tmpdir,
                         gdepth=gdepth,
                         bam=bam,
                         sample_sex=sample_sex,
-                        novcf=novcf,
                         prog_cmd=prog_cmd,
-                        gene1only=gene1only,
+                        sample_id=sample_id,
+                        args=args,
                     )
                     gene_groups = [
                         query_genes[i::num_threads] for i in range(num_threads)
                     ]
                     pool = mp.Pool(num_threads)
                     phaser_calls = pool.map(process_gene_partial, gene_groups)
                     pool.close()
                     pool.join()
                     for phaser_call_set in phaser_calls:
                         sample_out.update(phaser_call_set)
+
+                # merge cfh cluster result
+                if "CFH" in sample_out and "CFHR3" in sample_out:
+                    cfh_cluster_caller = genes.CfhClust(
+                        sample_id,
+                        tmpdir,
+                        sample_out["CFH"],
+                        sample_out["CFHR3"],
+                    )
+                    sample_out.setdefault(
+                        "CFHclust", cfh_cluster_caller.call()._asdict()
+                    )
+
                 sample_out = dict(sorted(sample_out.items()))
 
                 logging.info(
                     f"Merging all bams for sample {sample_id} at {datetime.datetime.now()}..."
                 )
                 self.merge_bams(query_genes, outdir, tmpdir, sample_id)
 
                 logging.info(
                     f"Writing to json for sample {sample_id} at {datetime.datetime.now()}..."
                 )
-                out_json = os.path.join(outdir, sample_id + ".json")
+                out_json = os.path.join(outdir, sample_id + ".paraphase.json")
                 with open(out_json, "w") as json_output:
                     json.dump(sample_out, json_output, indent=4)
             except Exception:
                 logging.error(
                     f"Error running sample {sample_id}...See error message below"
                 )
                 traceback.print_exc()
 
+    @staticmethod
+    def get_sample_id_from_header(bam):
+        """Get sample ID from RG SM from the bam header"""
+        bam_handle = pysam.AlignmentFile(bam, "rb")
+        header = bam_handle.header
+        header = header.to_dict()
+        sample_ids = []
+        rg_lines = header.get("RG")
+        if rg_lines is not None:
+            sample_ids = [a.get("SM") for a in rg_lines if "SM" in a]
+        bam_handle.close()
+        sample_ids = [a for a in sample_ids if a is not None]
+        if len(set(sample_ids)) == 1:
+            return sample_ids[0]
+        else:
+            return None
+
     def merge_bams(self, query_genes, outdir, tmpdir, sample_id):
         """Merge realigned tagged bams for each gene into one bam"""
         bams = []
         for gene in query_genes:
             gene_bam = os.path.join(tmpdir, f"{sample_id}_{gene}_realigned_tagged.bam")
             if os.path.exists(gene_bam) is False:
                 gene_bam = os.path.join(tmpdir, f"{sample_id}_{gene}_realigned.bam")
@@ -327,15 +369,15 @@
                     )
                 if os.path.exists(gene2_bam):
                     bams.append(gene2_bam)
         bam_list_file = os.path.join(tmpdir, f"{sample_id}_bam_list.txt")
         with open(bam_list_file, "w") as fout:
             for bam in bams:
                 fout.write(bam + "\n")
-        merged_bam = os.path.join(outdir, f"{sample_id}_realigned_tagged.bam")
+        merged_bam = os.path.join(outdir, f"{sample_id}.paraphase.bam")
         tmp_bam = os.path.join(tmpdir, f"{sample_id}_merged.bam")
         pysam.merge("-f", "-o", tmp_bam, "-b", bam_list_file)
         pysam.sort("-o", merged_bam, tmp_bam)
         pysam.index(merged_bam)
 
     def get_samtools_minimap2_path(self, args):
         """Get and check path to third-party tools"""
@@ -378,14 +420,20 @@
                 genome_build_dir = "19"
             for data_entry in data_paths:
                 old_data_file = data_paths[data_entry]
                 new_data_file = os.path.join(
                     data_path, genome_build_dir, gene, old_data_file
                 )
                 data_paths[data_entry] = new_data_file
+            # add fusion gene definition file
+            if configs[gene].get("call_fusion") is not None:
+                data_paths.setdefault(
+                    "fusion_json",
+                    os.path.join(data_path, genome_build_dir, "fusion_genes.json"),
+                )
             # add reference fasta
             ref_file = os.path.join(ref_dir, f"{gene}_ref.fa")
             data_paths.setdefault("reference", ref_file)
             realign_region = configs[gene].get("realign_region")
             if genome_build == "37":
                 realign_region = realign_region.replace("chr", "")
                 configs[gene]["realign_region"] = realign_region
@@ -535,32 +583,41 @@
         outputp.add_argument(
             "-o",
             "--out",
             help="Output directory",
             required=True,
         )
         parser.add_argument(
+            "-p",
+            "--prefix",
+            help="Prefix of output files for a single sample. Used with -b.\n"
+            + "If not provided, prefix will be extracted from the name of the input BAM.\n",
+            required=False,
+        )
+        parser.add_argument(
             "-g",
             "--gene",
             help="Optionally specify which gene(s) to run (separated by comma).\n"
             + "Will run all genes if not specified.\n"
-            + "The full set of accepted genes are defined in the config file.\n",
+            + "The full set of accepted regions are defined in the config file.\n"
+            + "Alternatively, you can define genes to call by modifying paraphase/data/genes.yaml\n",
             required=False,
         )
         parser.add_argument(
             "-c",
             "--config",
             help="Optional path to a user-defined config file listing the full set of regions to analyze.\n"
             + "By default Paraphase uses the config file in paraphase/data/38/config.yaml",
             required=False,
         )
         parser.add_argument(
             "-d",
             "--depth",
-            help="Optional path to a file listing average depth for each sample",
+            help=argparse.SUPPRESS,
+            # help="Optional path to a file listing average depth for each sample",
             required=False,
         )
         parser.add_argument(
             "-t",
             "--threads",
             help="Optional number of threads",
             required=False,
@@ -648,19 +705,18 @@
                     bamlist = [args.bam]
                     self.process_sample(
                         bamlist,
                         outdir,
                         configs,
                         tmpdir,
                         prog_cmd,
+                        args,
                         num_threads,
                         dcov,
-                        args.novcf,
                         genome_build_dir,
-                        args.gene1only,
                     )
                 else:
                     logging.warning(f"{args.bam} bam or bai file doesn't exist")
             # multiple bams, multiprocess by sample
             elif args.list is not None:
                 with open(args.list) as f:
                     for line in f:
@@ -672,18 +728,17 @@
 
                 process_sample_partial = partial(
                     self.process_sample,
                     outdir=outdir,
                     configs=configs,
                     tmpdir=tmpdir,
                     prog_cmd=prog_cmd,
+                    args=args,
                     dcov=dcov,
-                    novcf=args.novcf,
                     genome_build=genome_build_dir,
-                    gene1only=args.gene1only,
                 )
                 bam_groups = [bamlist[i::num_threads] for i in range(num_threads)]
                 pool = mp.Pool(num_threads)
                 pool.map(process_sample_partial, bam_groups)
                 pool.close()
                 pool.join()
             else:
```

### Comparing `paraphase-3.0.0/paraphase/phaser.py` & `paraphase-3.1.0/paraphase/phaser.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import copy
 import numpy as np
 from collections import Counter
 from itertools import product
 import re
 import logging
+import json
 from scipy.stats import poisson
 from collections import namedtuple
 from .haplotype_assembler import VariantGraph
 
 
 class Phaser:
     clip_5p = r"^\d+S|^\d+H"
@@ -34,14 +35,15 @@
         "homozygous_sites",
         "haplotype_details",
         "nonunique_supporting_reads",
         "read_details",
         "genome_depth",
         "region_depth",
         "sample_sex",
+        "fusions_called",
     ]
     GeneCall = namedtuple(
         "GeneCall",
         fields,
         defaults=(None,) * len(fields),
     )
     CoverageSummary = namedtuple("CoverageSummary", "median percentile80")
@@ -93,23 +95,33 @@
         self.gene_start = config.get("gene_start")
         if self.gene_start is None:
             self.gene_start = self.left_boundary
         self.gene_end = config.get("gene_end")
         if self.gene_end is None:
             self.gene_end = self.right_boundary
 
+        self.call_fusion = None
+        if "call_fusion" in config:
+            self.call_fusion = config["call_fusion"]
+            fusion_json = config["data"].get("fusion_json")
+            self.fusion_gene_def_variants = []
+            with open(fusion_json) as f:
+                self.fusion_gene_def_variants = json.load(f).get(self.gene)
         self.use_supplementary = False
         if "use_supplementary" in config or "is_tandem" in config:
             self.use_supplementary = True
         self.to_phase = False
         if "to_phase" in config or "is_tandem" in config:
             self.to_phase = True
         self.is_reverse = False
         if "is_reverse" in config:
             self.is_reverse = config["is_reverse"]
+        self.is_palindrome = False
+        if "is_palindrome" in config:
+            self.is_palindrome = config["is_palindrome"]
         self.expect_cn2 = False
         if "expect_cn2" in config:
             self.expect_cn2 = True
         self.clip_3p_positions = []
         self.clip_5p_positions = []
         if "clip_3p_positions" in config:
             self.clip_3p_positions = config["clip_3p_positions"]
@@ -988,15 +1000,15 @@
                 else:
                     for hap_name in haps_with_variant:
                         haplotype_variants[hap_name].append(var)
         # het sites and homo sites
         for hap, hap_name in haps.items():
             # find boundary for confident variant calling
             hap_bound_start, hap_bound_end = self.get_hap_variant_ranges(hap)
-            is_truncated = False
+            is_truncated = None
             # het sites
             for i in range(len(hap)):
                 if hap[i] == "2":
                     haplotype_variants[hap_name].append(het_sites[i])
                 elif hap[i] in known_del:
                     del_name = known_del[hap[i]]
                     if del_name not in haplotype_variants[hap_name]:
@@ -1042,15 +1054,15 @@
                     a
                     for a in filtered_homo_sites
                     if int(a.split("_")[0]) > clip_position
                 ]
                 hap_bound_start = max(hap_bound_start, clip_position)
                 haplotype_variants[hap_name].append(f"{clip_position}_clip_5p")
                 if clip_position > self.gene_start:
-                    is_truncated = True
+                    is_truncated = ["5p"]
             if hap.endswith("0") and self.clip_3p_positions != []:
                 for first_pos_before_clip in reversed(range(len(hap))):
                     if hap[first_pos_before_clip] != "0":
                         break
                 first_pos_before_clip_position = int(
                     het_sites[first_pos_before_clip].split("_")[0]
                 )
@@ -1061,15 +1073,18 @@
                     a
                     for a in filtered_homo_sites
                     if int(a.split("_")[0]) < clip_position
                 ]
                 hap_bound_end = min(hap_bound_end, clip_position)
                 haplotype_variants[hap_name].append(f"{clip_position}_clip_3p")
                 if clip_position < self.gene_end:
-                    is_truncated = True
+                    if is_truncated is None:
+                        is_truncated = ["3p"]
+                    else:
+                        is_truncated.append("3p")
 
             haplotype_variants[hap_name] += filtered_homo_sites
 
             hap_bound_start = max(hap_bound_start, self.left_boundary)
             hap_bound_end = min(hap_bound_end, self.right_boundary)
             boundary_gene2 = None
             if self.gene2_region is not None:
@@ -1675,14 +1690,160 @@
                 :: int(np.ceil(homo_sites_to_add_size / max_homo_var_to_add))
             ]
             self.het_sites += homo_sites_to_add
             self.het_sites = sorted(self.het_sites)
             self.remove_noisy_sites()
         return homo_sites_to_add
 
+    def find_fusion(self, ass_haps):
+        """Call fusion based on haplotypes"""
+        # update two-copy haplotypes
+        two_cp_haps = self.update_twp_cp_in_fusion_cases(ass_haps)
+        fusions_called = {}
+        for hap, hap_name in ass_haps.items():
+            if hap.endswith("x") is False and hap.startswith("x") is False:
+                if (hap.endswith("0") is False and hap.startswith("0") is True) or (
+                    hap.endswith("0") is True and hap.startswith("0") is False
+                ):
+                    new_hap, all_sites = self.new_hap_for_breakpoint(hap)
+                    fusion_breakpoint_index = self.get_fusion_breakpoint_index(
+                        hap, new_hap
+                    )
+                    if fusion_breakpoint_index is not None:
+                        bp1 = int(all_sites[fusion_breakpoint_index].split("_")[0])
+                        bp2 = self.get_range_in_other_gene(bp1, search_range=1000)
+                        bp3 = int(all_sites[fusion_breakpoint_index - 1].split("_")[0])
+                        bp4 = self.get_range_in_other_gene(bp3, search_range=1000)
+                        if bp1 < bp2:
+                            fusion_breakpoint = (
+                                (bp3, bp1),
+                                (bp4, bp2),
+                            )
+                        else:
+                            fusion_breakpoint = (
+                                (bp4, bp2),
+                                (bp3, bp1),
+                            )
+                        fusions_called.setdefault(hap_name, {})
+                        fusion_type = self.get_fusion_type(hap)
+                        fusions_called[hap_name].setdefault("type", fusion_type)
+                        fusions_called[hap_name].setdefault("sequence", new_hap)
+                        fusions_called[hap_name].setdefault(
+                            "breakpoint", fusion_breakpoint
+                        )
+        return two_cp_haps, fusions_called
+
+    def get_fusion_type(self, hap):
+        """Fusion type: deletion or duplication"""
+        fusion_type = None
+        if self.call_fusion == "5p":
+            if hap.endswith("0") is False and hap.startswith("0") is True:
+                fusion_type = "duplication"
+            elif hap.endswith("0") is True and hap.startswith("0") is False:
+                fusion_type = "deletion"
+        elif self.call_fusion == "3p":
+            if hap.endswith("0") is False and hap.startswith("0") is True:
+                fusion_type = "deletion"
+            elif hap.endswith("0") is True and hap.startswith("0") is False:
+                fusion_type = "duplication"
+        return fusion_type
+
+    @staticmethod
+    def update_twp_cp_in_fusion_cases(ass_haps):
+        """Update two-copy haplotypes based on the presence of gene/paralogs"""
+        two_cp_haps = []
+        if True not in [a.startswith("x") or a.endswith("x") for a in ass_haps]:
+            gene1s = [
+                a
+                for a in ass_haps
+                if a.endswith("0") is False and a.startswith("0") is False
+            ]
+            gene2s = [
+                a
+                for a in ass_haps
+                if a.endswith("0") is True and a.startswith("0") is True
+            ]
+            fusions = [
+                a
+                for a in ass_haps
+                if (a.endswith("0") is False and a.startswith("0") is True)
+                or (a.endswith("0") is True and a.startswith("0") is False)
+            ]
+            if fusions == [] and len(ass_haps) < 4:
+                if len(gene1s) == 1 and ass_haps[gene1s[0]] not in two_cp_haps:
+                    two_cp_haps.append(ass_haps[gene1s[0]])
+                if len(gene2s) == 1 and ass_haps[gene2s[0]] not in two_cp_haps:
+                    two_cp_haps.append(ass_haps[gene2s[0]])
+        return two_cp_haps
+
+    def new_hap_for_breakpoint(self, hap):
+        """
+        Get the haplotype sequence for breakpoint identification
+        This is ideally based on PSVs defined in self.fusion_gene_def_variants
+        """
+        new_hap = ""
+        if self.fusion_gene_def_variants != []:
+            all_sites = self.fusion_gene_def_variants
+            for var_site in all_sites:
+                base = "1"
+                if var_site in self.homo_sites:
+                    base = "2"
+                elif var_site in self.het_sites:
+                    base = hap[self.het_sites.index(var_site)]
+                new_hap += base
+        else:
+            all_sites = sorted(
+                self.homo_sites + self.het_sites, key=lambda x: int(x.split("_")[0])
+            )
+            if self.clip_5p_positions != []:
+                all_sites = [
+                    a
+                    for a in all_sites
+                    if int(a.split("_")[0]) > max(self.clip_5p_positions)
+                ]
+            if self.clip_3p_positions != []:
+                all_sites = [
+                    a
+                    for a in all_sites
+                    if int(a.split("_")[0]) < min(self.clip_3p_positions)
+                ]
+            for var_site in all_sites:
+                if var_site in self.homo_sites:
+                    new_hap += "2"
+                elif var_site in self.het_sites:
+                    new_hap += hap[self.het_sites.index(var_site)]
+        return new_hap, all_sites
+
+    @staticmethod
+    def get_fusion_breakpoint_index(hap, new_hap):
+        """Infer the switch from gene1 sequence to gene2 sequence"""
+        # 2s to 1s
+        if hap.startswith("0") is True and hap.endswith("0") is False:
+            counts = []
+            for i, _ in enumerate(new_hap):
+                counts.append(
+                    new_hap[:i].count("2") + new_hap[i:].count("1"),
+                )
+            bp_index = counts.index(max(counts))
+            if bp_index == 0 or bp_index == len(counts) - 1:
+                return None
+            return bp_index
+        # 1s to 2s
+        if hap.startswith("0") is False and hap.endswith("0") is True:
+            counts = []
+            for i, _ in enumerate(new_hap):
+                counts.append(
+                    new_hap[:i].count("1") + new_hap[i:].count("2"),
+                )
+            bp_index = counts.index(max(counts))
+            if bp_index == 0 or bp_index == len(counts) - 1:
+                return None
+            return bp_index
+        return None
+
     def call(self):
         """Main function to phase haplotypes and call copy numbers"""
         if self.check_coverage_before_analysis() is False:
             return self.GeneCall()
         self.get_homopolymer()
         # self.get_homopolymer_old()
         self.find_big_deletion()
@@ -1759,56 +1920,77 @@
             uniquely_supporting_reads,
             nonuniquely_supporting_reads,
             raw_read_haps,
             read_counts,
         ) = self.phase_haps(raw_read_haps)
 
         tmp = {}
-        mod_gene_name = ",".join(self.gene.split("-"))
         for i, hap in enumerate(ass_haps):
-            tmp.setdefault(hap, f"{mod_gene_name}_hap{i+1}")
+            tmp.setdefault(hap, f"{self.gene}_hap{i+1}")
         ass_haps = tmp
 
         haplotypes = None
         if ass_haps != {}:
             haplotypes = self.output_variants_in_haplotypes(
                 ass_haps,
                 uniquely_supporting_reads,
                 nonuniquely_supporting_reads,
                 known_del=known_del,
             )
 
         two_cp_haps = []
-        if len(ass_haps) == 3:
+        if (
+            len(ass_haps) == 3 and self.expect_cn2 is False and self.gene != "BPY2"
+        ) or (self.gene == "BPY2" and len(ass_haps) < 3):
             two_cp_haps = self.compare_depth(haplotypes, stringent=True)
             if two_cp_haps == [] and read_counts is not None:
                 # check if one haplotype has more reads than others
                 haps = list(read_counts.keys())
                 counts = list(read_counts.values())
                 max_count = max(counts)
                 cp2_hap = haps[counts.index(max_count)]
                 others_max = sorted(counts, reverse=True)[1]
                 probs = self.depth_prob(max_count, others_max)
                 # print(counts, probs)
                 if probs[0] < 0.05 and others_max >= 10:
                     two_cp_haps.append(ass_haps[cp2_hap])
 
+        # call fusion
+        fusions_called = None
+        if self.call_fusion is not None:
+            two_cp_haps, fusions_called = self.find_fusion(ass_haps)
+
         total_cn = len(ass_haps) + len(two_cp_haps)
 
         # fully homozygous
-        if self.het_sites == [] or total_cn == 1:
+        if self.het_sites == []:
             total_cn = 2
 
         # two pairs of identical copies
-        if two_cp_haps == [] and total_cn == 2 and self.expect_cn2 is False:
+        if (
+            two_cp_haps == []
+            and total_cn == 2
+            and self.expect_cn2 is False
+            and self.gene != "BPY2"
+        ):
             if self.mdepth is not None:
                 prob = self.depth_prob(int(self.region_avg_depth.median), self.mdepth)
                 if prob[0] < 0.75:
                     total_cn = 4
 
+        # correct CN for palindrome genes
+        # if self.sample_sex is not None:
+        #    if self.is_palindrome:
+        #        if self.sample_sex == "female" and total_cn < 4:
+        #            total_cn = None
+        #        elif self.sample_sex == "male" and total_cn < 2:
+        #            total_cn = None
+        if total_cn is not None and total_cn == 1:
+            total_cn = None
+
         # phase
         alleles = []
         hap_links = {}
         if self.to_phase is True:
             (
                 alleles,
                 hap_links,
@@ -1838,12 +2020,13 @@
             self.homo_sites,
             haplotypes,
             nonuniquely_supporting_reads,
             raw_read_haps,
             self.mdepth,
             self.region_avg_depth._asdict(),
             self.sample_sex,
+            fusions_called,
         )
 
     def close_handle(self):
         self._bamh.close()
         self._refh.close()
```

### Comparing `paraphase-3.0.0/paraphase/prepare_bam_and_vcf.py` & `paraphase-3.1.0/paraphase/prepare_bam_and_vcf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
     min_mapq = 50
     min_aln = 800
     max_mismatch = 0.05
     deletion = r"\d+D"
     insertion = r"\d+I"
 
-    def __init__(self, bam, outdir, config, prog_cmd):
+    def __init__(self, bam, outdir, config, prog_cmd, sample_id):
         self.bam = bam
         self.outdir = outdir
         self.prog_cmd = prog_cmd
+        self.sample_id = sample_id
         self.gene = config["gene"]
         self.ref = config["data"]["reference"]
         self.nchr_old = config["nchr_old"]
         self.nchr = config["nchr"]
         self.offset = int(self.nchr_old.split("_")[1]) - 1
         self.nchr_length = config["nchr_length"]
         self.extract_regions = config["extract_regions"]
@@ -40,15 +41,14 @@
         self.minimap2 = config["tools"]["minimap2"]
         if "check_nm" in config:
             self.max_mismatch = config["check_nm"]
         self.use_r2k = ""
         if "use_r2k" in config:
             self.use_r2k = "-r2k"
         self._bamh = pysam.AlignmentFile(bam, "rb")
-        self.sample_id = bam.split("/")[-1].split(".")[0]
         self.realign_bam = os.path.join(
             self.outdir, self.sample_id + f"_{self.gene}_realigned_old.bam"
         )
         self.realign_out_bam = os.path.join(
             self.outdir, self.sample_id + f"_{self.gene}_realigned.bam"
         )
         self.gene2_region = config.get("gene2_region")
@@ -338,14 +338,15 @@
 
 class VcfGenerater:
     """
     Call variants and generate individual/merged vcfs
     """
 
     search_range = 200
+    min_base_quality_for_variant_calling = 25
 
     def __init__(self, sample_id, outdir, call_sum):
         self.sample_id = sample_id
         self.outdir = outdir
         self.call_sum = call_sum
         self.match = {}
 
@@ -361,32 +362,26 @@
         self.deletion1_in_gene1 = config.get("deletion1_in_gene1")
         self.deletion1_in_gene2 = config.get("deletion1_in_gene2")
         self.extract_regions = config.get("extract_regions")
         if self.left_boundary is None:
             self.left_boundary = int(self.nchr_old.split("_")[1])
         if self.right_boundary is None:
             self.right_boundary = int(self.nchr_old.split("_")[2])
-        self.samtools = config["tools"]["samtools"]
-        self.minimap2 = config["tools"]["minimap2"]
         self.use_supplementary = False
         if "use_supplementary" in config or "is_tandem" in config:
             self.use_supplementary = True
-        self.keep_truncated = False
-        if "keep_truncated" in config:
-            self.keep_truncated = True
 
         self.prog_cmd = prog_cmd
         self.tmpdir = tmpdir
         if self.tmpdir is None:
             self.tmpdir = self.outdir
         self.bam = os.path.join(
             tmpdir, self.sample_id + f"_{self.gene}_realigned_tagged.bam"
         )
-        self.vcf_dir = os.path.join(self.outdir, f"{self.sample_id}_vcfs")
-        os.makedirs(self.vcf_dir, exist_ok=True)
+        self.vcf_dir = os.path.join(self.outdir, f"{self.sample_id}_paraphase_vcfs")
 
     def get_range_in_other_gene(self, pos):
         """
         Find the correponding coordinates in the other gene
         """
         if pos in self.match:
             return self.match[pos]
@@ -396,140 +391,234 @@
                 return self.match[new_pos]
         return None
 
     def write_header(self, fout):
         """Write VCF header"""
         fout.write("##fileformat=VCFv4.2\n")
         fout.write('##FILTER=<ID=PASS,Description="All filters passed">\n')
-        fout.write('##FILTER=<ID=LowDP,Description="Low depth at this site.">\n')
+        # fout.write('##FILTER=<ID=LowQual,Description="Nonpassing variant">\n')
         fout.write(
-            '##FILTER=<ID=LowQual,Description="Low confidence in this variant.">\n'
-        )
-        fout.write(
-            '##INFO=<ID=HapIDs,Number=R,Type=String,Description="Haplotype IDs">\n'
+            '##INFO=<ID=HPBOUND,Number=.,Type=String,Description="Boundary coordinates of the phased haplotype">\n'
         )
+        alleles = self.call_sum.get("alleles_final")
+        if alleles is not None and alleles != []:
+            fout.write(
+                '##INFO=<ID=ALLELE,Number=.,Type=String,Description="Haplotypes phased into alleles">\n'
+            )
         if self.gene in ["ikbkg", "f8"]:
             fout.write(
                 '##INFO=<ID=SVLEN,Number=1,Type=Integer,Description="Length of the SV">\n'
             )
             fout.write(
-                '##INFO=<ID=SVTYPE,Number=1,Type=String,Description="Type of the SV.">\n'
+                '##INFO=<ID=SVTYPE,Number=1,Type=String,Description="Type of the SV">\n'
             )
             fout.write(
                 '##INFO=<ID=END,Number=1,Type=Integer,Description="End position of the structural variant">\n'
             )
             fout.write('##ALT=<ID=DEL,Description="Deletion">\n')
             fout.write('##ALT=<ID=INV,Description="Inversion">\n')
-        fout.write('##FORMAT=<ID=GT,Number=R,Type=String,Description="Genotype">\n')
-        fout.write('##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read depth">\n')
         fout.write(
-            '##FORMAT=<ID=AD,Number=R,Type=Integer,Description="Read depth for each allele">\n'
+            '##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype per haplotype">\n'
+        )
+        fout.write(
+            '##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Depth per haplotype">\n'
+        )
+        fout.write(
+            '##FORMAT=<ID=AD,Number=R,Type=Integer,Description="Read depth for REF and ALT per haplotype">\n'
         )
         fout.write(f"##contig=<ID={self.nchr},length={self.nchr_length}>\n")
         fout.write(f"##paraphase_version={paraphase.__version__}\n")
         fout.write(f"##paraphase_command=paraphase {self.prog_cmd}\n")
-        header = [
-            "#CHROM",
-            "POS",
-            "ID",
-            "REF",
-            "ALT",
-            "QUAL",
-            "FILTER",
-            "INFO",
-            "FORMAT",
-            "default",
-        ]
-        fout.write("\t".join(header) + "\n")
+
+    @staticmethod
+    def modify_hapbound(bound1, bound2, truncated):
+        """Get haplotype boundaries to appear in vcf"""
+        hap_bound = f"{bound1}-{bound2}"
+        if truncated is not None:
+            if truncated == ["5p"]:
+                hap_bound = f"{bound1}truncated-{bound2}"
+            elif truncated == ["3p"]:
+                hap_bound = f"{bound1}-{bound2}truncated"
+            elif truncated == ["5p", "3p"]:
+                hap_bound = f"{bound1}truncated-{bound2}truncated"
+        return hap_bound
+
+    @staticmethod
+    def convert_alt_record(ref, alt):
+        """Convert variant ALT allele to the pileup format"""
+        if len(alt) > 1:
+            ins_len = len(alt) - 1
+            return f"{ref}+{ins_len}{alt[1:]}"
+        if len(ref) > 1:
+            del_len = len(ref) - 1
+            del_seq_n = "N" * del_len
+            return f"{ref[0]}-{del_len}{del_seq_n}"
+        return alt
 
     def merge_vcf(self, vars_list):
         """
         Merge vcfs from multiple haplotypes.
         """
-        merged_vcf = os.path.join(
-            self.vcf_dir, self.sample_id + f"_{self.gene}_variants.vcf"
-        )
+        os.makedirs(self.vcf_dir, exist_ok=True)
+        merged_vcf = os.path.join(self.vcf_dir, self.sample_id + f"_{self.gene}.vcf")
         with open(merged_vcf, "w") as fout:
             self.write_header(fout)
-            for variants_info, haps_ids in vars_list:
+            assert len(vars_list) <= 2
+            haps_ids = []
+            haps_ids1 = []
+            haps_ids2 = []
+            haps_bounds = []
+            for list_counter, (variants_info, haps_info) in enumerate(vars_list):
+                for hap_name, bound1, bound2, truncated in haps_info:
+                    haps_ids.append(hap_name)
+                    hap_bound = self.modify_hapbound(bound1, bound2, truncated)
+                    haps_bounds.append(hap_bound)
+                    if list_counter == 0:
+                        haps_ids1.append(hap_name)
+                    else:
+                        haps_ids2.append(hap_name)
+            header = [
+                "#CHROM",
+                "POS",
+                "ID",
+                "REF",
+                "ALT",
+                "QUAL",
+                "FILTER",
+                "INFO",
+                "FORMAT",
+            ] + haps_ids
+            fout.write("\t".join(header) + "\n")
+
+            for list_counter, (variants_info, haps_info) in enumerate(vars_list):
                 variants_info = dict(sorted(variants_info.items()))
                 for pos in variants_info:
                     call_info = variants_info[pos]
                     # unique variants at this site
                     variant_observed = set([a[0] for a in call_info if a is not None])
-                    var_num = len(variant_observed)
                     for variant in variant_observed:
                         _, ref, alt = variant.split("_")
                         merge_gt = []
                         merge_ad = []
                         merge_dp = []
                         for each_call in call_info:
                             if each_call is None:
                                 merge_gt.append(".")
                                 merge_ad.append(".")
                                 merge_dp.append(".")
                             else:
-                                var_name, dp, ad, var_filter, gt = each_call
+                                var_name, dp, ad, var_filter, gt, counter = each_call
+                                if counter is None:
+                                    if ref != alt:
+                                        this_ad = ",".join([str(a) for a in ad])
+                                    else:
+                                        this_ad = ",".join([str(a) for a in [ad[0], 0]])
+                                else:
+                                    if ref != alt:
+                                        alt_converted = self.convert_alt_record(
+                                            ref, alt
+                                        )
+                                        this_ad = ",".join(
+                                            [
+                                                str(a)
+                                                for a in [
+                                                    ad[0],
+                                                    counter[alt_converted],
+                                                ]
+                                            ]
+                                        )
+                                    else:
+                                        this_ad = ",".join([str(a) for a in [ad[0], 0]])
                                 if var_filter != []:
                                     gt = "."
                                 merge_dp.append(str(dp))
                                 if gt == "0":
                                     merge_gt.append(gt)
-                                    merge_ad.append(str(dp - ad))
+                                    merge_ad.append(this_ad)
                                 elif var_name == variant:
                                     merge_gt.append(gt)
-                                    merge_ad.append(str(ad))
+                                    merge_ad.append(this_ad)
                                 else:
                                     merge_gt.append(".")
-                                    merge_ad.append(".")
+                                    merge_ad.append(this_ad)
+                        if list_counter == 0 and haps_ids != haps_ids1:
+                            for _ in range(len(haps_ids2)):
+                                merge_gt.append(".")
+                                merge_ad.append(".")
+                                merge_dp.append(".")
+                        elif list_counter > 0:
+                            for _ in range(len(haps_ids1)):
+                                merge_gt.insert(0, ".")
+                                merge_ad.insert(0, ".")
+                                merge_dp.insert(0, ".")
                         final_qual = "."
-                        if ref == alt:
-                            alt = "."
-                        if (var_num == 1 and ("1" in merge_gt or "." in merge_gt)) or (
-                            var_num > 1 and alt != "."
+                        if (
+                            alt != ref
+                            and alt not in [".", "*"]
+                            and "1" in merge_gt  # or "." in merge_gt
                         ):
+                            if "1" in merge_gt:
+                                variant_filter = "PASS"
+                            # else:
+                            #    variant_filter = "LowQual"
+                            info_field = "HPBOUND=" + ",".join(haps_bounds)
+                            alleles = self.call_sum.get("alleles_final")
+                            if alleles is not None and alleles != []:
+                                alleles_rename = []
+                                for allele in alleles:
+                                    allele_rename = []
+                                    for a in allele:
+                                        if a is not None:
+                                            allele_rename.append(a)
+                                        else:
+                                            allele_rename.append("unknown")
+                                    alleles_rename.append(allele_rename)
+                                info_field += (
+                                    ";"
+                                    + "ALLELE="
+                                    + ",".join(["+".join(a) for a in alleles_rename])
+                                )
                             if alt.isdigit() is False:
                                 merged_entry = [
                                     self.nchr,
                                     str(pos),
                                     ".",
                                     ref,
                                     alt,
                                     final_qual,
-                                    "PASS",
-                                    "HapIDs=" + ",".join(haps_ids),
+                                    variant_filter,
+                                    info_field,
                                     "GT:DP:AD",
-                                    "/".join(merge_gt)
-                                    + ":"
-                                    + ",".join(merge_dp)
-                                    + ":"
-                                    + ",".join(merge_ad),
+                                ] + [
+                                    ":".join([merge_gt[j], merge_dp[j], merge_ad[j]])
+                                    for j in range(len(haps_ids))
                                 ]
+
                             else:
                                 nstart, var_type, nend = variant.split("_")
                                 nstart = int(nstart)
                                 nend = int(nend)
                                 var_size = nend - nstart
+                                info_field = (
+                                    f"SVTYPE={var_type};END={nend};SVLEN={var_size};"
+                                    + info_field
+                                )
                                 merged_entry = [
                                     self.nchr,
                                     str(pos),
                                     ".",
                                     "N",
                                     f"<{var_type}>",
                                     final_qual,
-                                    "PASS",
-                                    f"SVTYPE={var_type};END={nend};SVLEN={var_size};"
-                                    + "HapIDs="
-                                    + ",".join(haps_ids),
+                                    variant_filter,
+                                    info_field,
                                     "GT:DP:AD",
-                                    "/".join(merge_gt)
-                                    + ":"
-                                    + ",".join(merge_dp)
-                                    + ":"
-                                    + ",".join(merge_ad),
+                                ] + [
+                                    ":".join([merge_gt[j], merge_dp[j], merge_ad[j]])
+                                    for j in range(len(haps_ids))
                                 ]
                             fout.write("\t".join(merged_entry) + "\n")
 
     @staticmethod
     def refine_indels(ref_seq, var_seq, pos, refh, ref_name):
         """process indels"""
         if "+" in var_seq:
@@ -570,29 +659,31 @@
     @staticmethod
     def get_var(all_bases, ref_seq):
         """Get most supported base as variant"""
         dp = len(all_bases)
         gt = "."
         qual = "."
         ad = len([a for a in all_bases if a != ref_seq])
+        ad_ref = len([a for a in all_bases if a == ref_seq])
         var_seq = ref_seq
+        counter = None
         if all_bases != []:
             counter = Counter(all_bases)
             most_common_base = counter.most_common(2)
             var_seq = most_common_base[0][0]
             ad = most_common_base[0][1]
             is_snp = False
             if len(var_seq) == 1 and len(ref_seq) == 1 and var_seq != "*":
                 is_snp = True
             if var_seq == ref_seq:
                 gt = "0"
             else:
                 gt = "1"
             # qual = VcfGenerater.get_var_call_qual(dp, ad, gt, is_snp)
-        return [var_seq, dp, ad, gt, qual]
+        return [var_seq, dp, (ad_ref, ad), gt, qual, counter]
 
     def get_hap_bound(self, hap_name):
         """Get haplotype boundaries"""
         hap_bound = list(self.call_sum["haplotype_details"][hap_name]["boundary"])
         # find the positions next to the existing boundaries
         confident_position = hap_bound[0]
         if confident_position == self.left_boundary:
@@ -618,137 +709,84 @@
         self,
         pileups_raw,
         read_names,
         uniq_reads,
         refh,
         offset,
         hap_bound,
-        vcf_out,
         min_depth=4,
         min_qual=25,
         variants_to_add={},
     ):
         """
         Filter pileups and make variant calls.
         """
         variants = []
-        # for now, report F8 SVs in the haplotype vcfs. Ideally they should be in a diploid vcf.
         if self.gene == "f8":
             for pos in variants_to_add:
                 var_name = variants_to_add[pos]
                 nstart, var_type, nend = var_name.split("_")
                 nstart = int(nstart)
                 nend = int(nend)
-                var_size = nend - nstart
-                variants.append([nstart, var_name, ".", ".", [], "1"])
-                vcf_out_line = [
-                    self.nchr,
-                    str(nstart),
-                    ".",
-                    "N",
-                    f"<{var_type}>",
-                    ".",
-                    "PASS",
-                    f"SVTYPE={var_type};END={nend};SVLEN={var_size}",
-                    "GT:DP:AD",
-                    f"1:.:.",
-                ]
-                vcf_out.write("\t".join(vcf_out_line) + "\n")
+                variants.append([nstart, var_name, ".", ".", [], "1", None])
 
         ref_name = refh.references[0]
         del_pos = []
         for pos in pileups_raw:
             if pos in variants_to_add:
                 var_name = variants_to_add[pos]
                 nstart, var_type, nend = var_name.split("_")
                 nstart = int(nstart)
                 nend = int(nend)
-                var_size = nend - nstart
-                variants.append([nstart, var_name, ".", ".", [], "1"])
-                vcf_out_line = [
-                    self.nchr,
-                    str(nstart),
-                    ".",
-                    "N",
-                    f"<{var_type}>",
-                    ".",
-                    "PASS",
-                    f"SVTYPE={var_type};END={nend};SVLEN={var_size}",
-                    "GT:DP:AD",
-                    f"1:.:.",
-                ]
-                vcf_out.write("\t".join(vcf_out_line) + "\n")
+                variants.append([nstart, var_name, ".", ".", [], "1", None])
                 del_pos = [nstart, nend]
 
             all_bases = pileups_raw[pos]
             if offset < 0:
                 true_pos = pos
                 refh_pos = pos + offset
             else:
                 true_pos = pos + offset
                 refh_pos = pos
             ref_seq = refh.fetch(ref_name, refh_pos - 1, refh_pos)
             alt_all_reads = self.get_var(all_bases, ref_seq)
+            var_seq, dp, ad, gt, qual, counter = alt_all_reads
             if (
                 hap_bound == []
                 or (None not in hap_bound and hap_bound[0] < true_pos < hap_bound[1])
             ) and (del_pos == [] or true_pos < del_pos[0] or true_pos > del_pos[1]):
                 # use only unique reads for positions at the edge
+                # or no-call when using all reads
                 if (
                     hap_bound == []
                     or true_pos < hap_bound[2]
                     or true_pos > hap_bound[3]
+                    or ad[1] < dp * 0.7
                 ):
                     bases_uniq_reads = []
                     for i, read_base in enumerate(all_bases):
                         if uniq_reads is None or read_names[pos][i] in uniq_reads:
                             bases_uniq_reads.append(read_base)
                     alt_uniq_reads = self.get_var(bases_uniq_reads, ref_seq)
-                    # if alt_uniq_reads[1] >= min_depth:
-                    var_seq, dp, ad, gt, qual = alt_uniq_reads
-                    # else:
-                    #    var_seq, dp, ad, gt, qual = alt_all_reads
-                    #    gt = "."
-                else:
-                    var_seq, dp, ad, gt, qual = alt_all_reads
+                    var_seq, dp, ad, gt, qual, counter = alt_uniq_reads
+                    if dp < min_depth or ad[1] < dp * 0.7:
+                        var_seq, dp, ad, gt, qual, counter = alt_all_reads
 
                 ref_seq, var_seq = self.refine_indels(
                     ref_seq, var_seq, refh_pos, refh, ref_name
                 )
                 var = f"{true_pos}_{ref_seq}_{var_seq}"
-                qual = "."
                 var_filter = []
                 if dp < min_depth:
                     var_filter.append("LowDP")
-                # if qual != "." and qual < min_qual:
-                if ad < dp * 0.7:
+                if ad[1] < dp * 0.7:
                     var_filter.append("LowQual")
-                if var_filter == []:
-                    call_filter = "PASS"
-                else:
-                    call_filter = ";".join(var_filter)
+                if var_filter != []:
                     gt = "."
-                variants.append([true_pos, var, dp, ad, var_filter, gt])
-                if var_seq == ref_seq:
-                    var_seq = "."
-                # write all positions where gt is not confidently 0
-                if gt == "1" or gt == ".":
-                    vcf_out_line = [
-                        self.nchr,
-                        str(true_pos),
-                        ".",
-                        ref_seq,
-                        var_seq,
-                        str(qual),
-                        call_filter,
-                        ".",
-                        "GT:DP:AD",
-                        f"{gt}:{dp}:{ad}",
-                    ]
-                    vcf_out.write("\t".join(vcf_out_line) + "\n")
+                variants.append([true_pos, var, dp, ad, var_filter, gt, counter])
         return variants
 
     def run_without_realign(
         self,
         gene2=False,
         final_haps={},
         match_range=False,
@@ -799,88 +837,70 @@
                 # supplementary alignments
                 if self.use_supplementary and len(read_name_split) > 1:
                     uniq_reads.append(read_name_split[0])
                 else:
                     uniq_reads.append(read_name)
         variants_info = {}
         two_cp_haplotypes = self.call_sum.get("two_copy_haplotypes")
-        # exclude truncated copies
-        haps_not_truncated = [
-            a
-            for a in final_haps.values()
-            if self.call_sum["haplotype_details"][a]["is_truncated"] is False
-            or self.keep_truncated is True
-        ]
-        nhap = len(haps_not_truncated) + len(
-            [a for a in two_cp_haplotypes if a in haps_not_truncated]
-        )
-        hap_ids = []
+        nhap = len(final_haps)
+        if two_cp_haplotypes is not None:
+            nhap += len(two_cp_haplotypes)
+        hap_info = []
 
         # gene1only, or two-gene mode but gene1 side
         if gene2 is False or match_range is False:
             bamh = pysam.AlignmentFile(self.bam, "rb")
             refh = pysam.FastaFile(self.ref)
             offset = self.offset
             nchr = self.nchr
         else:
             bamh = pysam.AlignmentFile(self.bam_gene2, "rb")
             refh = pysam.FastaFile(self.ref_gene2)
             offset = self.offset_gene2
             nchr = self.nchr_gene2
 
         if (gene2 is False or match_range is False) and final_haps == {}:
-            hap_name = "homozygous_hap1"
-            hap_vcf_out = os.path.join(
-                self.vcf_dir, self.sample_id + f"_{self.gene}_{hap_name}.vcf"
-            )
-            vcf_out = open(hap_vcf_out, "w")
-            self.write_header(vcf_out)
+            hap_name = f"{self.gene}_homozygous_hap1"
             pileups_raw = {}
             read_names = {}
             for pileupcolumn in bamh.pileup(
                 nchr,
                 truncate=True,
-                min_base_quality=30,
+                min_base_quality=self.min_base_quality_for_variant_calling,
             ):
                 pos = pileupcolumn.pos + 1
                 this_pos_bases = [
                     a.upper() for a in pileupcolumn.get_query_sequences(add_indels=True)
                 ]
                 pileups_raw.setdefault(pos, this_pos_bases)
                 read_names.setdefault(pos, pileupcolumn.get_query_names())
             variants_called = self.pileup_to_variant(
                 pileups_raw,
                 read_names,
                 None,
                 refh,
                 0 - offset,
                 [],
-                vcf_out,
             )
-            vcf_out.close()
-            hap_ids.append(hap_name)
-            hap_ids.append(hap_name)
-            for pos, var_name, dp, ad, var_filter, gt in variants_called:
+            hap_info.append([hap_name, self.left_boundary, self.right_boundary, None])
+            hap_info.append(
+                [hap_name + "_cp2", self.left_boundary, self.right_boundary, None]
+            )
+
+            for pos, var_name, dp, ad, var_filter, gt, counter in variants_called:
                 variants_info.setdefault(
                     pos,
                     [
-                        [var_name, dp, ad, var_filter, gt],
-                        [var_name, dp, ad, var_filter, gt],
+                        [var_name, dp, ad, var_filter, gt, counter],
+                        [var_name, dp, ad, var_filter, gt, counter],
                     ],
                 )
 
         i = 0
         for hap_name in final_haps.values():
-            if (
-                self.call_sum["haplotype_details"][hap_name]["is_truncated"] is True
-                and self.keep_truncated is False
-            ):
-                continue
-            hap_ids.append(hap_name)
-
             variants_to_add = {}
             if hap_name in special_variants:
                 variant_to_add = special_variants[hap_name]
                 variants_to_add.setdefault(
                     int(variant_to_add.split("_")[0]), variant_to_add
                 )
 
@@ -899,27 +919,38 @@
                     else:
                         hap_bound = [
                             min(n1, n2),
                             max(n1, n2),
                             min(n3, n4),
                             max(n3, n4),
                         ]
-            hap_vcf_out = os.path.join(
-                self.vcf_dir, self.sample_id + f"_{self.gene}_{hap_name}.vcf"
-            )
-            vcf_out = open(hap_vcf_out, "w")
-            self.write_header(vcf_out)
+            if gene2 is False or match_range is False:
+                this_hap_info = [
+                    hap_name,
+                    hap_bound[0],
+                    hap_bound[1],
+                    self.call_sum["haplotype_details"][hap_name]["is_truncated"],
+                ]
+                hap_info.append(this_hap_info)
+            else:
+                this_hap_info = [
+                    hap_name,
+                    hap_bound[0],
+                    hap_bound[1],
+                    None,
+                ]
+                hap_info.append(this_hap_info)
 
             # by HP tag
             pileups_raw = {}
             read_names = {}
             for pileupcolumn in bamh.pileup(
                 nchr,
                 truncate=True,
-                min_base_quality=30,
+                min_base_quality=self.min_base_quality_for_variant_calling,
             ):
                 pos = pileupcolumn.pos + 1
                 this_pos_bases = [
                     a.upper() for a in pileupcolumn.get_query_sequences(add_indels=True)
                 ]
                 this_position_hps = []
                 this_pos_read_names = []
@@ -952,35 +983,44 @@
             variants_called = self.pileup_to_variant(
                 pileups_raw,
                 read_names,
                 uniq_reads,
                 refh,
                 0 - offset,
                 hap_bound,
-                vcf_out,
                 variants_to_add=variants_to_add,
             )
-            vcf_out.close()
 
-            for pos, var_name, dp, ad, var_filter, gt in variants_called:
+            for pos, var_name, dp, ad, var_filter, gt, counter in variants_called:
                 variants_info.setdefault(pos, [None] * nhap)
-                variants_info[pos][i] = [var_name, dp, ad, var_filter, gt]
+                variants_info[pos][i] = [var_name, dp, ad, var_filter, gt, counter]
                 if hap_name in two_cp_haplotypes:
-                    variants_info[pos][i + 1] = [var_name, dp, ad, var_filter, gt]
+                    variants_info[pos][i + 1] = [
+                        var_name,
+                        dp,
+                        ad,
+                        var_filter,
+                        gt,
+                        counter,
+                    ]
             if hap_name in two_cp_haplotypes:
                 i += 1
-                hap_ids.append(hap_name)
+                this_hap_info_cp2 = [this_hap_info[0] + "_cp2"] + this_hap_info[1:]
+                hap_info.append(this_hap_info_cp2)
             i += 1
 
         bamh.close()
         refh.close()
-        if gene2 is False:
-            self.merge_vcf([(variants_info, hap_ids)])
-        else:
-            return variants_info, hap_ids
+        return variants_info, hap_info
+
+    def run(self):
+        if self.call_sum.get("final_haplotypes") is None:
+            return
+        variants_info, hap_info = self.run_without_realign()
+        self.merge_vcf([(variants_info, hap_info)])
 
 
 class TwoGeneVcfGenerater(VcfGenerater):
     """
     Make vcf for two-gene scenario
     """
 
@@ -1029,40 +1069,49 @@
             for hap, hap_name in all_haps.items():
                 if "pseudo" not in hap_name:
                     gene1_haps.setdefault(hap, hap_name)
                 else:
                     gene2_haps.setdefault(hap, hap_name)
         elif self.gene == "ikbkg":
             for hap, hap_name in all_haps.items():
-                if "dup" not in hap_name:
-                    if "pseudo" not in hap_name:
-                        gene1_haps.setdefault(hap, hap_name)
-                    else:
-                        gene2_haps.setdefault(hap, hap_name)
+                if "pseudo" not in hap_name:
+                    gene1_haps.setdefault(hap, hap_name)
+                else:
+                    gene2_haps.setdefault(hap, hap_name)
         return gene1_haps, gene2_haps
 
     def run(self):
         """
         Process haplotypes one by one. Realign to different ref sequence
         in this two-gene scenario
         """
         call_sum = self.call_sum
         if call_sum.get("final_haplotypes") is None:
             return
         gene1_haps, gene2_haps = self.separate_two_genes()
-        vars_gene1, gene1_hap_ids = self.run_without_realign(
+        vars_gene1, gene1_hap_info = self.run_without_realign(
             gene2=True,
             final_haps=gene1_haps,
         )
-        vars_gene2, gene2_hap_ids = self.run_without_realign(
+        vars_gene2, gene2_hap_info = self.run_without_realign(
             gene2=True,
             final_haps=gene2_haps,
             match_range=True,
         )
         if (
             vars_gene1 != {}
             and vars_gene2 != {}
             and list(vars_gene1.keys())[0] < list(vars_gene2.keys())[0]
         ):
-            self.merge_vcf([(vars_gene1, gene1_hap_ids), (vars_gene2, gene2_hap_ids)])
+            self.merge_vcf(
+                [
+                    (vars_gene1, gene1_hap_info),
+                    (vars_gene2, gene2_hap_info),
+                ]
+            )
         else:
-            self.merge_vcf([(vars_gene2, gene2_hap_ids), (vars_gene1, gene1_hap_ids)])
+            self.merge_vcf(
+                [
+                    (vars_gene2, gene2_hap_info),
+                    (vars_gene1, gene1_hap_info),
+                ]
+            )
```

### Comparing `paraphase-3.0.0/paraphase.egg-info/PKG-INFO` & `paraphase-3.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-Metadata-Version: 2.1
-Name: paraphase
-Version: 3.0.0
-Summary: paraphase: HiFi-based caller for highly homologous genes
-Home-page: https://github.com/PacificBiosciences/paraphase
-Author: Xiao Chen
-Author-email: xchen@pacificbiosciences.com
-License: BSD-3-Clause-Clear
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<h1 align="center"><img width="300px" src="docs/logo_Paraphase.svg"/></h1>
 
-# Paraphase: HiFi-based caller for highly homologous genes
+<h1 align="center">Paraphase</h1>
+
+<h3 align="center">HiFi-based caller for highly similar paralogous genes</h3>
 
 Many medically relevant genes fall into 'dark' regions where variant calling is limited due to high sequence homology with paralogs or pseudogenes. Paraphase is a Python tool that takes HiFi aligned BAMs as input (whole-genome or enrichment), phases haplotypes for genes of the same family, determines copy numbers and makes phased variant calls. 
 
 ![Paraphase diagram](docs/figures/paraphase_diagram.png)
 Paraphase takes all reads from a gene family, realigns to just the gene of interest and then phases them into haplotypes. This solves the problem of alignment difficulty due to sequence homology and allows us to examine all copies of genes in a gene family and call copy number changes and other variants.
 
-Paraphase supports 161 segmental duplication regions in GRCh38, listed in the [config](paraphase/data/38/config.yaml) file. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
+Paraphase supports 160 segmental duplication [regions](docs/regions.md) in GRCh38. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
 - SMN1/SMN2 (spinal muscular atrophy)
 - RCCX module
   - CYP21A2 (21-Hydroxylase-Deficient Congenital Adrenal Hyperplasia)
   - TNXB (Ehlers-Danlos syndrome)
   - C4A/C4B (relevant in autoimmune diseases)
 - PMS2 (Lynch Syndrome)
 - STRC (hereditary hearing loss and deafness)
 - IKBKG (Incontinentia Pigmenti)
 - NCF1 (chronic granulomatous disease; Williams syndrome)
 - NEB (Nemaline myopathy)
 - F8 (intron 22 inversion, Hemophilia A)
 - CFC1 (heterotaxy syndrome)
 - OPN1LW/OPN1MW (color vision deficiencies)
 - HBA1/HBA2 (Alpha-Thalassemia)
+- GBA (Gaucher disease and Parkison's disease)
+- CYP11B1/CYP11B2 (Glucocorticoid-remediable aldosteronism)
+- CFH/CFHR1/CFHR2/CFHR3/CFHR4 (large deletions/duplications, atypical hemolytic uremic syndrome and age-related macular degeneration)
 
 Please check out our [paper](https://www.cell.com/ajhg/fulltext/S0002-9297(23)00001-0) on its application to the gene SMN1 for more details about Paraphase.   
 Chen X, Harting J, Farrow E, et al. Comprehensive SMN1 and SMN2 profiling for spinal muscular atrophy analysis using long-read PacBio HiFi sequencing. The American Journal of Human Genetics. 2023;0(0). doi:10.1016/j.ajhg.2023.01.001
 
 For whole-genome sequencing (WGS) data, we recommend >20X, ideally 30X, genome coverage. Low coverage or short read length could result in less accurate phasing, especially when gene copies are highly similar to each other. For hybrid capture-based enrichment data, a higher read depth (>50X) is recommended as the read length is generally shorter than WGS.
 
 ## Contact
@@ -76,50 +72,49 @@
 ```
 
 Required parameters:
 - `-b`: Input BAM file or `-l`: text file listing BAM files one per line (a BAI file needs to exist in the same directory)
 - `-o`: Output directory
 - `-r`: Path to the reference genome fasta file
 
-Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. 
+Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. Recommendations on reference genomes to use are documented [here](https://github.com/PacificBiosciences/reference_genomes).
 
 Optional parameters:
-- `-g`: Gene(s) to analyze, separated by comma. All supported genes will be analyzed if not specified.
+- `-g`: Region(s) to analyze, separated by comma. All supported [regions](docs/regions.md) will be analyzed if not specified. Please use region name, i.e. first column in the doc.
 - `-t`: Number of threads.
-- `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](paraphase/data/19/config.yaml) are supported now for GRCh37/hg19).
-- `gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see [below](#interpreting-the-output).
+- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the name of the input BAM. 
+- `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](docs/regions.md) are supported now for GRCh37/hg19).
+- `--gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see more information [here](docs/vcf.md).
 - `--novcf`: If specified, no VCF files will be produced.
 - `--samtools`: path to samtools. If the paths to samtools or minimap2 are not already in the PATH environment variable, they can be provided through the `--samtools` and `--minimap2` parameters.
 - `--minimap2`: path to minimap2
 
 ## Interpreting the output
 
-Paraphase produces a few output files in the directory specified by `-o`, with the sample ID as the prefix.
-
-1. `.vcf` in `sampleID_vcfs` folder. A VCF file is written for each haplotype per gene family. There is also a `_variants.vcf` file containing merged variants from all haplotypes for each gene family. Note that this is not a diploid vcf as there are usually more than two copies of genes in a gene family in a sample.
+Paraphase produces a few output files in the directory specified by `-o`, with the specified or default prefix.
 
-As genes of the same family can be highly similar to each other in sequence and not easy to differentiate (at the sequence level or even at the functional level), variant calls are made against one selected "main" gene from the gene family (e.g. the functional gene is selected when the family has a gene and a pseudogene). In this way, all copies of the gene family can be evaluated for pathogenic variants and one can calculate the copy number of the functional genes in the family and hence infer the disease/carrier status.
+1. `.vcf` in `${prefix}_paraphase_vcfs` folder. A VCF file is written for each region (gene family). More descriptions on the VCF can be found [here](docs/vcf.md).
 
-Exceptions are SMN1 (paralog SMN2), PMS2 (pseudogene PMS2CL), STRC (pseudogene STRCP1), NCF1 (pseudogenes NCF1B and NCF1C) and IKBKG (pseudogene IKBKGP1), where gene differentiation is possible. In these families, haplotypes are assigned to each gene in the family, i.e. gene or paralog/pseudogene, and variants are called against the gene (or paralog/pseudogene) for the gene (or paralog/pseudogene) haplotypes, respectively. Variants calls can be made against the main gene only for these five families if `--gene1only` is specified. 
+2. `.paraphase.bam`: This BAM file can be loaded into IGV for visualization of haplotypes (group reads by `HP` tag and color alignments by `YC` tag). All haplotypes are aligned against the main gene of interest. Tutorials/Examples are provided for medically relevant genes (See below).  
 
-2. `_realigned_tagged.bam`: This BAM file can be loaded into IGV for visualization of haplotypes (group reads by `HP` tag and color alignments by `YC` tag). All haplotypes are aligned against the main gene of interest. Tutorials/Examples are provided for medically relevant genes (See below).  
-
-3. `.json`: Output file summarizing haplotypes and variant calls for each gene family in each sample. In brief, a few generally used fields are explained below.
+3. `.paraphase.json`: Output file summarizing haplotypes and variant calls for each gene family in each sample. In brief, a few generally used fields are explained below.
 - `final_haplotypes`: phased haplotypes for all gene copies in a gene family
 - `total_cn`: total copy number of the family (sum of gene and paralog/pseudogene)
 - `two_copy_haplotypes`: haplotypes that are present in two copies based on depth. This happens when (in a small number of cases) two haplotypes are identical and we infer that there exist two of them instead of one by checking the read depth.
 - `haplotype_details`: lists information about each haplotype 
   - `boundary`: the boundary of the region that is resolved on the haplotype. This is useful when a haplotype is only partially phased.
 - `alleles_final`: haplotypes phased into alleles. This is possible when the segmental duplication is in tandem.
-- `region_depth`: median depth of the gene family (include all copies of gene and paralog/pseudogene) 
 
 Tutorials/Examples are provided for interpreting the `json` output and visualizing haplotypes for medically relevant genes listed below: 
 - [SMN1/SMN2](docs/SMN1_SMN2.md)
 - [RCCX module (CYP21A2)](docs/RCCX.md)
 - [PMS2](docs/PMS2.md)
 - [STRC](docs/STRC.md)
 - [OPN1LW/OPN1MW](docs/OPN1LW_OPN1MW.md)
 - [HBA1/HBA2](docs/HBA1_HBA2.md)
 - [IKBKG](docs/IKBKG.md)
 - [F8](docs/F8.md)
 - [NEB](docs/NEB.md)
 - [NCF1](docs/NCF1.md)
+- [GBA](docs/GBA.md)
+- [CFH gene cluster](docs/CFH.md)
+
```

### Comparing `paraphase-3.0.0/paraphase.egg-info/SOURCES.txt` & `paraphase-3.1.0/paraphase.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 paraphase/data/genes.yaml
 paraphase/data/19/config.yaml
 paraphase/data/19/genome_region.bed
 paraphase/data/19/sex_region.bed
 paraphase/data/19/rccx/cyp21_diff_sites.txt
 paraphase/data/19/smn1/known_haplotypes.json
 paraphase/data/38/config.yaml
+paraphase/data/38/fusion_genes.json
 paraphase/data/38/genome_region.bed
 paraphase/data/38/sex_region.bed
 paraphase/data/38/rccx/cyp21_diff_sites.txt
 paraphase/data/38/smn1/known_haplotypes.json
 paraphase/genes/__init__.py
 paraphase/genes/cfc1_phaser.py
+paraphase/genes/cfhclust.py
 paraphase/genes/f8_phaser.py
 paraphase/genes/hba_phaser.py
 paraphase/genes/ikbkg_phaser.py
 paraphase/genes/ncf1_phaser.py
 paraphase/genes/neb_phaser.py
 paraphase/genes/opn1lw_phaser.py
 paraphase/genes/pms2_phaser.py
```

### Comparing `paraphase-3.0.0/setup.py` & `paraphase-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/tests/test_f8_phaser.py` & `paraphase-3.1.0/tests/test_f8_phaser.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import os
 from paraphase.genes.f8_phaser import F8Phaser
 from .test_phaser import update_config
 
 
 class TestF8Phaser(object):
     cur_dir = os.path.dirname(__file__)
-    sample_dir = os.path.join(cur_dir, "test_data")
+    sample_dir = os.path.join(cur_dir, "test_data", "f8")
 
     def test_inversion(self):
         sample_id = "inv"
         genome_bam = os.path.join(self.sample_dir, f"f8_{sample_id}_genome.bam")
         phaser = F8Phaser(
             sample_id, self.sample_dir, genome_bam=genome_bam, sample_sex="male"
         )
         config = update_config("f8")
         phaser.set_parameter(config)
         f8_call = phaser.call()
-        assert f8_call.sv_called == {"int22h3_hap1": "inversion"}
+        assert f8_call.sv_called == {"f8_int22h3_hap1": "inversion"}
 
     def test_deletion(self):
         sample_id = "del"
         genome_bam = os.path.join(self.sample_dir, f"f8_{sample_id}_genome.bam")
         phaser = F8Phaser(
             sample_id, self.sample_dir, genome_bam=genome_bam, sample_sex="male"
         )
         config = update_config("f8")
         phaser.set_parameter(config)
         f8_call = phaser.call()
-        assert f8_call.sv_called == {"int22h2_hap1": "deletion"}
+        assert f8_call.sv_called == {"f8_int22h2_hap1": "deletion"}
```

### Comparing `paraphase-3.0.0/tests/test_haplotype_assembler.py` & `paraphase-3.1.0/tests/test_haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/tests/test_opn1lw_phaser.py` & `paraphase-3.1.0/tests/test_opn1lw_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/tests/test_paraphase.py` & `paraphase-3.1.0/tests/test_paraphase.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/tests/test_rccx_phaser.py` & `paraphase-3.1.0/tests/test_rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.0.0/tests/test_smn1_phaser.py` & `paraphase-3.1.0/tests/test_smn1_phaser.py`

 * *Files identical despite different names*

