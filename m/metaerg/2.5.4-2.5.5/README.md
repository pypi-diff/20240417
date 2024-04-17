# Comparing `tmp/metaerg-2.5.4.tar.gz` & `tmp/metaerg-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaerg-2.5.4.tar", last modified: Thu Mar 14 17:59:11 2024, max compression
+gzip compressed data, was "metaerg-2.5.5.tar", last modified: Wed Apr 17 20:57:31 2024, max compression
```

## Comparing `metaerg-2.5.4.tar` & `metaerg-2.5.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.610743 metaerg-2.5.4/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27307 2024-03-14 17:59:11.610743 metaerg-2.5.4/PKG-INFO
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26159 2024-03-14 16:48:28.000000 metaerg-2.5.4/README.md
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2023-05-24 19:12:00.000000 metaerg-2.5.4/pyproject.toml
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)       78 2024-03-14 17:59:11.610743 metaerg-2.5.4/setup.cfg
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1630 2024-03-14 16:46:06.000000 metaerg-2.5.4/setup.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.597409 metaerg-2.5.4/src/
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.600743 metaerg-2.5.4/src/metaerg/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/__init__.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.600743 metaerg-2.5.4/src/metaerg/calculations/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/calculations/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3444 2023-08-30 16:15:59.000000 metaerg-2.5.4/src/metaerg/calculations/cluster_database.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14431 2024-02-16 15:24:10.000000 metaerg-2.5.4/src/metaerg/calculations/codon_usage_bias.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    22470 2024-03-14 16:48:28.000000 metaerg-2.5.4/src/metaerg/context.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.604076 metaerg-2.5.4/src/metaerg/datatypes/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/datatypes/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7085 2024-02-08 17:31:28.000000 metaerg-2.5.4/src/metaerg/datatypes/blast.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2837 2024-02-21 15:32:50.000000 metaerg-2.5.4/src/metaerg/datatypes/excel.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     8709 2023-08-18 21:22:31.000000 metaerg-2.5.4/src/metaerg/datatypes/fasta.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5914 2023-08-24 16:29:57.000000 metaerg-2.5.4/src/metaerg/datatypes/functional_genes.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4997 2024-02-21 20:53:57.000000 metaerg-2.5.4/src/metaerg/datatypes/gbk.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5628 2024-02-13 17:36:57.000000 metaerg-2.5.4/src/metaerg/datatypes/gff.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4951 2023-08-16 16:12:04.000000 metaerg-2.5.4/src/metaerg/datatypes/ncbi_ftp.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    16241 2024-03-08 20:29:43.000000 metaerg-2.5.4/src/metaerg/datatypes/sqlite.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.604076 metaerg-2.5.4/src/metaerg/html/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)       97 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/html/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3656 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/html/html_all_genomes.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6882 2024-02-16 22:08:40.000000 metaerg-2.5.4/src/metaerg/html/html_feature_details.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9850 2024-02-16 22:08:40.000000 metaerg-2.5.4/src/metaerg/html/html_feature_table.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3307 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/html/html_genome_properties_and_subsystems.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17193 2024-02-23 16:22:10.000000 metaerg-2.5.4/src/metaerg/installation.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14712 2024-02-13 17:47:35.000000 metaerg-2.5.4/src/metaerg/main.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      109 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/registry.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.607409 metaerg-2.5.4/src/metaerg/run_and_read/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      197 2023-12-07 19:43:19.000000 metaerg-2.5.4/src/metaerg/run_and_read/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7253 2024-03-04 22:15:12.000000 metaerg-2.5.4/src/metaerg/run_and_read/antismash.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5473 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/run_and_read/aragorn.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6289 2024-02-13 16:53:14.000000 metaerg-2.5.4/src/metaerg/run_and_read/cdd.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2387 2023-08-21 19:21:22.000000 metaerg-2.5.4/src/metaerg/run_and_read/checkm.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6325 2023-12-08 15:27:32.000000 metaerg-2.5.4/src/metaerg/run_and_read/cmscan.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    37789 2024-03-14 17:11:21.000000 metaerg-2.5.4/src/metaerg/run_and_read/comparative_genomics.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2146 2024-02-21 20:42:42.000000 metaerg-2.5.4/src/metaerg/run_and_read/crispr_detect.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.607409 metaerg-2.5.4/src/metaerg/run_and_read/data/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.4/src/metaerg/run_and_read/data/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    73396 2023-08-24 16:32:48.000000 metaerg-2.5.4/src/metaerg/run_and_read/data/functional_gene_data
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5541 2023-12-11 17:58:52.000000 metaerg-2.5.4/src/metaerg/run_and_read/deepsig.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    25842 2023-12-11 17:58:52.000000 metaerg-2.5.4/src/metaerg/run_and_read/diamond_and_blastn.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9987 2023-12-11 17:58:52.000000 metaerg-2.5.4/src/metaerg/run_and_read/functional_genes.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3629 2024-02-21 20:54:25.000000 metaerg-2.5.4/src/metaerg/run_and_read/gene_writer.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1653 2024-03-07 16:42:18.000000 metaerg-2.5.4/src/metaerg/run_and_read/ltr_harvest.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1410 2023-08-18 20:55:41.000000 metaerg-2.5.4/src/metaerg/run_and_read/minced.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5957 2024-03-04 22:15:12.000000 metaerg-2.5.4/src/metaerg/run_and_read/padloc.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4615 2023-12-06 16:22:37.000000 metaerg-2.5.4/src/metaerg/run_and_read/prodigal.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6196 2023-12-11 17:59:31.000000 metaerg-2.5.4/src/metaerg/run_and_read/pureseqtm.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5486 2023-08-18 20:18:09.000000 metaerg-2.5.4/src/metaerg/run_and_read/repeat_masker.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1825 2023-12-11 17:59:31.000000 metaerg-2.5.4/src/metaerg/run_and_read/signalp.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2644 2023-12-11 17:59:31.000000 metaerg-2.5.4/src/metaerg/run_and_read/tmhmm.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2175 2023-08-18 20:22:19.000000 metaerg-2.5.4/src/metaerg/run_and_read/trf.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-03-14 17:59:11.610743 metaerg-2.5.4/src/metaerg.egg-info/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27307 2024-03-14 17:59:11.000000 metaerg-2.5.4/src/metaerg.egg-info/PKG-INFO
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1892 2024-03-14 17:59:11.000000 metaerg-2.5.4/src/metaerg.egg-info/SOURCES.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        1 2024-03-14 17:59:11.000000 metaerg-2.5.4/src/metaerg.egg-info/dependency_links.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)       46 2024-03-14 17:59:11.000000 metaerg-2.5.4/src/metaerg.egg-info/entry_points.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      148 2024-03-14 17:59:11.000000 metaerg-2.5.4/src/metaerg.egg-info/requires.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        8 2024-03-14 17:59:11.000000 metaerg-2.5.4/src/metaerg.egg-info/top_level.txt
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.340289 metaerg-2.5.5/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27706 2024-04-17 20:57:31.340289 metaerg-2.5.5/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26558 2024-04-10 16:30:10.000000 metaerg-2.5.5/README.md
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2023-05-24 19:12:00.000000 metaerg-2.5.5/pyproject.toml
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       78 2024-04-17 20:57:31.340289 metaerg-2.5.5/setup.cfg
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1630 2024-04-10 16:30:10.000000 metaerg-2.5.5/setup.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.333623 metaerg-2.5.5/src/
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.333623 metaerg-2.5.5/src/metaerg/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/__init__.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.336956 metaerg-2.5.5/src/metaerg/calculations/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/calculations/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3444 2023-08-30 16:15:59.000000 metaerg-2.5.5/src/metaerg/calculations/cluster_database.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14431 2024-02-16 15:24:10.000000 metaerg-2.5.5/src/metaerg/calculations/codon_usage_bias.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    22700 2024-04-17 17:36:43.000000 metaerg-2.5.5/src/metaerg/context.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.336956 metaerg-2.5.5/src/metaerg/datatypes/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/datatypes/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7085 2024-02-08 17:31:28.000000 metaerg-2.5.5/src/metaerg/datatypes/blast.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2837 2024-02-21 15:32:50.000000 metaerg-2.5.5/src/metaerg/datatypes/excel.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     8709 2023-08-18 21:22:31.000000 metaerg-2.5.5/src/metaerg/datatypes/fasta.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7143 2024-04-11 15:56:34.000000 metaerg-2.5.5/src/metaerg/datatypes/functional_genes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4997 2024-02-21 20:53:57.000000 metaerg-2.5.5/src/metaerg/datatypes/gbk.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5628 2024-02-13 17:36:57.000000 metaerg-2.5.5/src/metaerg/datatypes/gff.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4951 2023-08-16 16:12:04.000000 metaerg-2.5.5/src/metaerg/datatypes/ncbi_ftp.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17721 2024-04-17 17:29:54.000000 metaerg-2.5.5/src/metaerg/datatypes/sqlite.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.336956 metaerg-2.5.5/src/metaerg/html/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       97 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/html/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3656 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/html/html_all_genomes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6882 2024-02-16 22:08:40.000000 metaerg-2.5.5/src/metaerg/html/html_feature_details.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9850 2024-02-16 22:08:40.000000 metaerg-2.5.5/src/metaerg/html/html_feature_table.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3307 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/html/html_genome_properties_and_subsystems.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17193 2024-02-23 16:22:10.000000 metaerg-2.5.5/src/metaerg/installation.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    15091 2024-04-17 20:06:08.000000 metaerg-2.5.5/src/metaerg/main.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      109 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/registry.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.336956 metaerg-2.5.5/src/metaerg/run_and_read/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      197 2023-12-07 19:43:19.000000 metaerg-2.5.5/src/metaerg/run_and_read/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7290 2024-04-17 17:36:43.000000 metaerg-2.5.5/src/metaerg/run_and_read/antismash.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5507 2024-04-17 17:36:40.000000 metaerg-2.5.5/src/metaerg/run_and_read/aragorn.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6460 2024-04-17 17:37:11.000000 metaerg-2.5.5/src/metaerg/run_and_read/cdd.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2387 2024-04-17 17:37:10.000000 metaerg-2.5.5/src/metaerg/run_and_read/checkm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6360 2024-04-17 17:37:31.000000 metaerg-2.5.5/src/metaerg/run_and_read/cmscan.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    37930 2024-04-17 18:06:00.000000 metaerg-2.5.5/src/metaerg/run_and_read/comparative_genomics.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2213 2024-04-17 17:37:53.000000 metaerg-2.5.5/src/metaerg/run_and_read/crispr_detect.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.340289 metaerg-2.5.5/src/metaerg/run_and_read/data/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.5/src/metaerg/run_and_read/data/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    75923 2024-04-11 15:35:57.000000 metaerg-2.5.5/src/metaerg/run_and_read/data/functional_gene_data
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5800 2024-04-17 17:38:44.000000 metaerg-2.5.5/src/metaerg/run_and_read/deepsig.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26068 2024-04-17 17:38:44.000000 metaerg-2.5.5/src/metaerg/run_and_read/diamond_and_blastn.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14194 2024-04-17 20:21:43.000000 metaerg-2.5.5/src/metaerg/run_and_read/functional_genes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3644 2024-04-17 17:38:42.000000 metaerg-2.5.5/src/metaerg/run_and_read/gene_writer.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1683 2024-04-17 17:38:59.000000 metaerg-2.5.5/src/metaerg/run_and_read/ltr_harvest.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1445 2024-04-17 17:39:10.000000 metaerg-2.5.5/src/metaerg/run_and_read/minced.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6214 2024-04-17 17:39:24.000000 metaerg-2.5.5/src/metaerg/run_and_read/padloc.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4676 2024-04-17 17:50:21.000000 metaerg-2.5.5/src/metaerg/run_and_read/prodigal.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6452 2024-04-17 17:41:08.000000 metaerg-2.5.5/src/metaerg/run_and_read/pureseqtm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5688 2024-04-17 18:01:07.000000 metaerg-2.5.5/src/metaerg/run_and_read/repeat_masker.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1825 2024-04-17 17:40:12.000000 metaerg-2.5.5/src/metaerg/run_and_read/signalp.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2644 2024-04-17 17:40:42.000000 metaerg-2.5.5/src/metaerg/run_and_read/tmhmm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2368 2024-04-17 18:01:07.000000 metaerg-2.5.5/src/metaerg/run_and_read/trf.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 20:57:31.340289 metaerg-2.5.5/src/metaerg.egg-info/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27706 2024-04-17 20:57:31.000000 metaerg-2.5.5/src/metaerg.egg-info/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1892 2024-04-17 20:57:31.000000 metaerg-2.5.5/src/metaerg.egg-info/SOURCES.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        1 2024-04-17 20:57:31.000000 metaerg-2.5.5/src/metaerg.egg-info/dependency_links.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       46 2024-04-17 20:57:31.000000 metaerg-2.5.5/src/metaerg.egg-info/entry_points.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      148 2024-04-17 20:57:31.000000 metaerg-2.5.5/src/metaerg.egg-info/requires.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        8 2024-04-17 20:57:31.000000 metaerg-2.5.5/src/metaerg.egg-info/top_level.txt
```

### Comparing `metaerg-2.5.4/PKG-INFO` & `metaerg-2.5.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaerg
-Version: 2.5.4
+Version: 2.5.5
 Summary: Annotation of genomes and contigs
 Home-page: https://github.com/kinestetika/MetaErg
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/MetaErg
 Keywords: repeat-regions genes functions taxonomy
@@ -30,15 +30,15 @@
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 
-## metaerg.py, version 2.5.4
+## metaerg.py, version 2.5.5
 
 Metaerg.py annotates genomes or sets of mags/bins from microbial ecosystems (bacteria, archaea, viruses). Input data 
 consists of nucleotide fasta files, one per genome or mag, each with one or more contigs. Output files with annotations 
 are in common formats such as .gff, .gbk, .fasta and .html with predicted genes, their functions and taxonomic 
 classifications.
 
 Metaerg 2.5 can annotate a group of related genomes and apply a suite of comparative genomics analyses. To do this, put
@@ -211,23 +211,27 @@
                         actually download and install the antismash database.
 
 ```
 
 ## Using the Docker Image
 Metaerg depends on many helper programs and may require some time and troubleshooting to install. To avoid these issues,
 use the [docker image](https://hub.docker.com/r/kinestetika/metaerg). Alternatively, use singularity or apptainer to run 
-the docker image on a HPC, as explained by [jkzorz](https://github.com/jkzorz/Metagenomes_Illumina/blob/main/annotation.md):
+the docker image on a HPC, as explained by [jkzorz](https://github.com/jkzorz/Metagenomes_Illumina/blob/main/annotation.md) and [lianchun yi]:
 
 ```commandline
 >singularity pull docker://kinestetika/metaerg
 >singularity build --sandbox /path/where/top/create/metaerg_latest.sif docker://kinestetika/metaerg:latest
->singularity run ~/metaerg_latest.sif
+>singularity exec --bind /path/to/metaerg_database:/databases --bind /path/to/fasta/files:/data --writable /path/to/the/sandbox/dir
+metaerg --database_dir /databases --contig_file /data --file_extension .fna
 ```
 
-Or:
+>[!NOTE]
+>The --bind instruction binds the dir "/path/to/metaerg_database" (which is on your real filesystem) to the dir "/databases" (which is inside your container). Same for the contig dir.
+
+Or, using apptainer:
 ```commandline
 >apptainer build metaerg.sif docker://kinestetika/metaerg:latest
 ```
 
 ## Installation
 
 To install metaerg, its 19 helper programs (diamond, prodigal, etc.) and databases run the following commands:
```

### Comparing `metaerg-2.5.4/README.md` & `metaerg-2.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## metaerg.py, version 2.5.4
+## metaerg.py, version 2.5.5
 
 Metaerg.py annotates genomes or sets of mags/bins from microbial ecosystems (bacteria, archaea, viruses). Input data 
 consists of nucleotide fasta files, one per genome or mag, each with one or more contigs. Output files with annotations 
 are in common formats such as .gff, .gbk, .fasta and .html with predicted genes, their functions and taxonomic 
 classifications.
 
 Metaerg 2.5 can annotate a group of related genomes and apply a suite of comparative genomics analyses. To do this, put
@@ -175,23 +175,27 @@
                         actually download and install the antismash database.
 
 ```
 
 ## Using the Docker Image
 Metaerg depends on many helper programs and may require some time and troubleshooting to install. To avoid these issues,
 use the [docker image](https://hub.docker.com/r/kinestetika/metaerg). Alternatively, use singularity or apptainer to run 
-the docker image on a HPC, as explained by [jkzorz](https://github.com/jkzorz/Metagenomes_Illumina/blob/main/annotation.md):
+the docker image on a HPC, as explained by [jkzorz](https://github.com/jkzorz/Metagenomes_Illumina/blob/main/annotation.md) and [lianchun yi]:
 
 ```commandline
 >singularity pull docker://kinestetika/metaerg
 >singularity build --sandbox /path/where/top/create/metaerg_latest.sif docker://kinestetika/metaerg:latest
->singularity run ~/metaerg_latest.sif
+>singularity exec --bind /path/to/metaerg_database:/databases --bind /path/to/fasta/files:/data --writable /path/to/the/sandbox/dir
+metaerg --database_dir /databases --contig_file /data --file_extension .fna
 ```
 
-Or:
+>[!NOTE]
+>The --bind instruction binds the dir "/path/to/metaerg_database" (which is on your real filesystem) to the dir "/databases" (which is inside your container). Same for the contig dir.
+
+Or, using apptainer:
 ```commandline
 >apptainer build metaerg.sif docker://kinestetika/metaerg:latest
 ```
 
 ## Installation
 
 To install metaerg, its 19 helper programs (diamond, prodigal, etc.) and databases run the following commands:
```

### Comparing `metaerg-2.5.4/setup.py` & `metaerg-2.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='metaerg',
-    version='2.5.4',
+    version='2.5.5',
     packages=setuptools.find_packages(where='src'),
     url='https://github.com/kinestetika/MetaErg',
     license='MIT',
     author='Marc Strous',
     author_email='mstrous@ucalgary.ca',
     description='Annotation of genomes and contigs',
     long_description=long_description,
```

### Comparing `metaerg-2.5.4/src/metaerg/calculations/cluster_database.py` & `metaerg-2.5.5/src/metaerg/calculations/cluster_database.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/calculations/codon_usage_bias.py` & `metaerg-2.5.5/src/metaerg/calculations/codon_usage_bias.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/context.py` & `metaerg-2.5.5/src/metaerg/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from multiprocessing import cpu_count
 from pathlib import Path
 from time import sleep
 
 import httpx
 
 from metaerg import registry
+from metaerg.datatypes import sqlite
 
-
-VERSION = "2.5.4"
+VERSION = "2.5.5"
 
 BASE_DIR = Path()
 TEMP_DIR = Path()
 HTML_DIR = Path()
 DATABASE_DIR = Path()
 CHECKM_DIR:None | Path = None
 GTDBTK_DIR:None | Path = None
@@ -358,14 +358,16 @@
         print(final_msg)
         try:
             with open(LOG_FILE, 'a') as log_handle:
                 log_handle.write(final_msg)
                 log_handle.write('\n')
         except FileNotFoundError:
             pass
+        except TypeError:
+            pass
 
 
 def format_runtime():
     runtime = time.monotonic() - START_TIME
     return f'[{int(runtime / 3600):02d}h:{int((runtime % 3600) / 60):02d}m:{int(runtime % 60):02d}s]'
 
 
@@ -410,25 +412,29 @@
 def write_metaerg_progress(genome_name, new_progress):
     progress_file = spawn_file('metaerg_progress', genome_name)
     with open(progress_file, 'w') as writer:
         for k,v in new_progress.items():
             writer.write(f'{k}={v}\n')
 
 
+def check_annotator_results_for_consistency_with_previous_run(db_connection):
+    pass
+
+
 def register_annotator(define_annotator):
     param = define_annotator()
 
     # If a database index needs to be loaded, that is done at the start6, to prevent it loading over and over by
     # each thread.
     try:
         registry.DB_PRELOADER_REGISTRY.append(param['preload_db'])
     except KeyError:
         pass
 
-    def annotator(genome, contig_dict, db_connection) -> int:
+    def annotator(genome, contig_dict, db_connection_current, db_connection_previous) -> int:
         """Runs programs and reads results."""
         # (1) Read metaerg progress file, update progress and log the start of the analysis
         if not ANNOTATOR_STATUS[param['annotator_key']]:
             return 0
         current_progress = parse_metaerg_progress(genome.name)
         if ANNOTATOR_STATUS[param['annotator_key']] == FORCE_ANNOTATOR or \
            ANNOTATOR_STATUS[param['annotator_key']] == UPDATE_ANNOTATOR or \
@@ -465,20 +471,15 @@
             p = 'X'
             for p in param.get('programs', []):
                 program_path = shutil.which(p, mode=os.X_OK)
                 if not program_path:
                     all_programs_in_path = False
             if all_programs_in_path:
                 try:
-                    param['run'](genome, contig_dict, db_connection, result_files)
-                except FatalException as e:
-                    log('({}) Error while running {}: {}', (genome.name, param['purpose'],
-                                                            "".join(traceback.format_exception(e))))
-                    raise(Exception('({}) Error while running {}: {}', (genome.name, param['purpose'],
-                                                            "".join(traceback.format_exception(e)))))
+                    param['run'](genome, contig_dict, db_connection_current, result_files)
                 except Exception as e:
                     log('({}) Error while running {}: {}', (genome.name, param['purpose'],
                                                             "".join(traceback.format_exception(e))))
                     return 0
             else:
                 log('({}) Unable to run {}, helper program "{}" not in path', (genome.name, param['purpose'], p))
                 return 0
@@ -493,15 +494,22 @@
                     'helper program failed to run.', (genome.name, f))
                 results_complete = False
         # (7) Report success, update progress
         current_progress[param['annotator_key']] = PROGRESS_COMPLETE
         write_metaerg_progress(genome.name, current_progress)
         positive_count = 0
         if results_complete:
-            positive_count = param['read'](genome, contig_dict, db_connection, result_files)
+            positive_count = param['read'](genome, contig_dict, db_connection_current, result_files)
+            # (8) Compare to previous results
+            if diff := sqlite.compare_annotation_results(db_connection_previous, db_connection_current, param["annotator_key"]):
+                if diff[2]:
+                    log(f'({genome.name}) {param["annotator_key"]} predicted {diff[1]} features, previously {diff[0]}, with {diff[2]} updates.')
+                else:
+                    log(f'({genome.name}) {param["annotator_key"]} prediction coordinates were identical to previous run.')
+
         log('({}) {} complete. Found {}.', (genome.name, param['purpose'].capitalize(), positive_count))
         return 0
 
     registry.ANNOTATOR_REGISTRY[param['pipeline_position']] = annotator
     return annotator
 
 
@@ -511,9 +519,8 @@
 
 
 def register_database_installer(database_installer):
     registry.DATABASE_INSTALLER_REGISTRY.append(database_installer)
     # print(len(registry.DATABASE_INSTALLER_REGISTRY))
     return database_installer
 
-class FatalException(Exception):
-    pass
+
```

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/blast.py` & `metaerg-2.5.5/src/metaerg/datatypes/blast.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/excel.py` & `metaerg-2.5.5/src/metaerg/datatypes/excel.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/fasta.py` & `metaerg-2.5.5/src/metaerg/datatypes/fasta.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/gbk.py` & `metaerg-2.5.5/src/metaerg/datatypes/gbk.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/gff.py` & `metaerg-2.5.5/src/metaerg/datatypes/gff.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/ncbi_ftp.py` & `metaerg-2.5.5/src/metaerg/datatypes/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/datatypes/sqlite.py` & `metaerg-2.5.5/src/metaerg/datatypes/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,14 +149,18 @@
 
     def length_nt(self):
         return self.end - self.start
 
     def length_aa(self):
         return (self.end - self.start) // 3
 
+    def get_coord_key(self):
+        return f'{self.contig}-{self.start}-{self.end}'
+
+
 SQLITE_CREATE_GENOME_TABLE_SYNTAX = '''CREATE TABLE genomes(
     name TEXT,
     input_fasta_file TEXT,
     size INT,
     number_of_contigs INT,
     fraction_gc FLOAT,
     n50_contig_length INT,
@@ -320,16 +324,21 @@
 def genome_factory(cursor, row) -> Genome:
     fields = [column[0] for column in cursor.description]
     if len(fields) < 10:
         return fields[0]
     return Genome(**{key: value for key, value in zip(fields, row)})
 
 
-def connect_to_db(sql_db_file, target='Features'):
-    connection = sql.connect(sql_db_file)
+def connect_to_db(sql_db_file, target='Features', load_into_memory=True):
+    if load_into_memory:
+        source = sql.connect(sql_db_file)
+        connection = sql.connect(':memory:')
+        source.backup(connection)
+    else:
+        connection = sql.connect(sql_db_file)
     if 'Features' == target:
         connection.row_factory = feature_factory
     elif 'Genomes' == target:
         connection.row_factory = genome_factory
     return connection
 
 def create_db(target='Features'):
@@ -405,26 +414,29 @@
 
 def read_genome_by_id(sql_connection, genome_name) -> Genome:
     cursor = sql_connection.cursor()
     result = cursor.execute('SELECT rowid, * FROM genomes WHERE name = ?', (genome_name,))
     return result.fetchone()
 
 
-def read_all_features(sql_connection, contig='', type=None, start=-1, end=-1, additional_sql=None):
+def read_all_features(sql_connection, contig='', type=None, inference=None, start=-1, end=-1, additional_sql=None):
     cursor = sql_connection.cursor()
 
     where_str = []
     fields = []
     if type:
         if isinstance(type, list) or isinstance(type, tuple)  or isinstance(type, set):
             where_str.append('type IN ({})'.format(','.join('?' for t in type)))
             fields.extend(type)
         else:
             where_str.append('type = ?')
             fields.append(type)
+    if inference:
+        where_str.append('inference = ?')
+        fields.append(inference)
     if contig:
         where_str.append('contig = ?')
         fields.append(contig)
     if start >= 0 and end >= 0:
         where_str.append('start < ? AND end > ?')
         fields.append(end)
         fields.append(start)
@@ -443,10 +455,33 @@
         #print(fields)
         return cursor.execute('SELECT rowid, * FROM features WHERE ' + where_str + ' ORDER BY contig, start', tuple(fields))
     else:
         return cursor.execute('SELECT rowid, * FROM features ORDER BY contig, start')
     #for columns in result.fetchall():
     #    yield Feature(*columns)
 
+
+def compare_annotation_results(db_connection_prev, db_connection_current, inference):
+    previously_detected_feature_coordinates = set()
+    newly_detected_coordinates = set()
+    try:
+        features_detected_previously = 0
+        for prev_feature in read_all_features(db_connection_prev, inference=inference):
+            previously_detected_feature_coordinates.add(prev_feature.get_coord_key())
+            features_detected_previously += 1
+        features_detected_currently = 0
+        for current_feature in read_all_features(db_connection_current, inference=inference):
+            key = current_feature.get_coord_key()
+            if key in previously_detected_feature_coordinates:
+                previously_detected_feature_coordinates.remove(key)
+            else:
+                newly_detected_coordinates.add(key)
+            features_detected_currently += 1
+        update_count = len(previously_detected_feature_coordinates) + len(newly_detected_coordinates)
+        return features_detected_previously, features_detected_currently, update_count
+    except:
+        return None
+
+
 def read_all_genomes(sql_connection, sql_where=''):
     cursor = sql_connection.cursor()
     return cursor.execute('SELECT rowid, * FROM genomes ' + sql_where + ' ORDER BY name')
```

### Comparing `metaerg-2.5.4/src/metaerg/html/html_all_genomes.py` & `metaerg-2.5.5/src/metaerg/html/html_all_genomes.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/html/html_feature_details.py` & `metaerg-2.5.5/src/metaerg/html/html_feature_details.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/html/html_feature_table.py` & `metaerg-2.5.5/src/metaerg/html/html_feature_table.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/html/html_genome_properties_and_subsystems.py` & `metaerg-2.5.5/src/metaerg/html/html_genome_properties_and_subsystems.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/installation.py` & `metaerg-2.5.5/src/metaerg/installation.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/main.py` & `metaerg-2.5.5/src/metaerg/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,19 +77,25 @@
 def annotate_genome(genome_name, input_fasta_file: Path):
     context.log(f'Started annotation of {genome_name}...')
     current_progress = context.parse_metaerg_progress(genome_name)
     if context.ANNOTATOR_STATUS['visualization'] != context.FORCE_ANNOTATOR and \
             current_progress.get('visualization', 0) == context.PROGRESS_COMPLETE:
         context.log(f'({genome_name}) already completed! Use --update_annotations to re-annotate.')
         return
-    # (1) prepare feature sqlite3 database
-    #feature_db_file = context.spawn_file('annotations.sqlite', genome_name, context.BASE_DIR)
-    #sqlite.create_db(feature_db_file)
-    feature_db_connection = sqlite.create_db(target='Features')
-    # (2) load sequence data
+    # (1) prepare feature sqlite3 database, this database is created in memory and later saved to file
+    feature_db_connection_current = sqlite.create_db(target='Features')
+    # (2) If a database file exists, load existing annotations to memory
+    feature_db_file = context.spawn_file('annotations.sqlite', genome_name, context.BASE_DIR)
+    feature_db_connection_previous = None
+    if feature_db_file.exists():
+       try:
+           feature_db_connection_previous = sqlite.connect_to_db(feature_db_file)
+       except:
+           context.log('Detected sql db of existing annotations, but failed to read it.')
+    # (3) load sequence data
     contig_dict = fasta.load_contigs(genome_name, input_fasta_file, delimiter=context.DELIMITER,
                                      min_contig_length=context.MIN_CONTIG_LENGTH, rename_contigs=context.RENAME_CONTIGS)
     if not len(contig_dict):
         context.log(f'({genome_name}) WARNING: {input_fasta_file} appears to contain no fasta data... aborting!')
         return
     genome = sqlite.Genome(name=genome_name, input_fasta_file=input_fasta_file)
 
@@ -103,56 +109,55 @@
     cum_size = 0
     for c in contigs:
         cum_size += len(c['seq'])
         if cum_size > + genome.size / 2:
             genome.n50_contig_length = len(c['seq'])
             break
 
-    # (3) now annotate
+    # (4) now annotate
     for annotator in context.sorted_annotators():
-        annotator(genome, contig_dict, feature_db_connection)
+        annotator(genome, contig_dict, feature_db_connection_current, feature_db_connection_previous)
     # feather_file = context.spawn_file("all_genes.feather", genome_name, context.BASE_DIR)
     # feature_data = pd.read_feather(feather_file)
     # feature_data = feature_data.set_index('id', drop=False)
 
-    # (4) save results
+    # (5) save results
     context.log(f'({genome_name}) Now writing annotations to .fasta, .gbk...')
     faa_file = context.spawn_file("faa", genome_name, context.BASE_DIR, extension='faa')
     rna_file = context.spawn_file("rna.fna", genome_name, context.BASE_DIR, extension='fna')
     gbk_file = context.spawn_file("gbk", genome_name, context.BASE_DIR, extension='gbk')
     fna_file = context.spawn_file("fna", genome_name, context.BASE_DIR, extension='fna')
-    fasta.write_features_to_fasta(feature_db_connection, 'aa', faa_file, targets=('CDS',))
-    fasta.write_features_to_fasta(feature_db_connection, 'nt', rna_file, targets=('rRNA tRNA tmRNA ncRNA retrotransposon'.split()))
-    fasta.write_contigs_to_fasta(contig_dict, fna_file, feature_db_connection)
+    fasta.write_features_to_fasta(feature_db_connection_current, 'aa', faa_file, targets=('CDS',))
+    fasta.write_features_to_fasta(feature_db_connection_current, 'nt', rna_file, targets=('rRNA tRNA tmRNA ncRNA retrotransposon'.split()))
+    fasta.write_contigs_to_fasta(contig_dict, fna_file, feature_db_connection_current)
     with open(gbk_file, 'w') as gbk_writer:
-        gbk.gbk_write_genome(gbk_writer, contig_dict, feature_db_connection)
-    feature_count = sqlite.count_features(feature_db_connection)
+        gbk.gbk_write_genome(gbk_writer, contig_dict, feature_db_connection_current)
+    feature_count = sqlite.count_features(feature_db_connection_current)
     if feature_count < 1e6:
         context.log(f'({genome_name}) Writing {feature_count} annotations to .feather format...')
         feather_file = context.spawn_file("annotations.feather", genome_name, context.BASE_DIR, extension='pyarrow')
         rows = []
-        for feature in sqlite.read_all_features(feature_db_connection):
+        for feature in sqlite.read_all_features(feature_db_connection_current):
             rows.append({k: str(v) for k, v in feature})
         pd.DataFrame(rows).to_feather(feather_file)
     else:
         context.log(f'({genome_name}) Skipping feather format, too many ({feature_count}) annotations...')
     # (5) visualize
     context.log(f'({genome_name}) Now writing final result as .html for visualization...')
     for html_writer in registry.HTML_WRITER_REGISTRY:
-        html_writer(genome, feature_db_connection, context.HTML_DIR)
+        html_writer(genome, feature_db_connection_current, context.HTML_DIR)
     # (6) update progress
     current_progress = context.parse_metaerg_progress(genome_name)
     current_progress['visualization'] = context.PROGRESS_COMPLETE
     context.write_metaerg_progress(genome_name, current_progress)
     context.log(f'({genome_name}) Completed html visualization.')
     # (7) save feature sqlite database
-    feature_db_file = context.spawn_file('annotations.sqlite', genome_name, context.BASE_DIR)
     feature_db_file.unlink(missing_ok=True)
-    sqlite.write_db(feature_db_connection, feature_db_file)
-    feature_db_connection.close()
+    sqlite.write_db(feature_db_connection_current, feature_db_file)
+    feature_db_connection_current.close()
     return genome
 
 
 def main():
     context.init(**parse_arguments().__dict__)
     if context.METAERG_ACTION == context.METAERG_ACTION_CREATE_DATABASE:
         context.log(f'Creating/installing/downloading metaerg databases. Tasks: {context.DATABASE_TASKS}; ')
@@ -192,20 +197,20 @@
             preloader()
         genome_dict = {}
         if context.PARALLEL_ANNOTATIONS > 1:
             with futures.ProcessPoolExecutor(max_workers=context.PARALLEL_ANNOTATIONS) as executor:
                 for genome_name, contig_file in zip(context.GENOME_NAMES, context.CONTIG_FILES):
                     genome_dict[genome_name] = executor.submit(annotate_genome, genome_name, contig_file)
             for genome_name, future in genome_dict.items():
-                try:
-                    if genome := future.result():
-                        sqlite.add_new_genome_to_db(genome_db_connection, genome)
-                    genome_dict[genome_name] = genome
-                except Exception as e:
-                    context.log(f'({genome_name}) {str(e)}')
+                #try:
+                if genome := future.result():
+                    sqlite.add_new_genome_to_db(genome_db_connection, genome)
+                genome_dict[genome_name] = genome
+                #except Exception as e:
+                #    context.log(f'({genome_name}) {e}')
         else:
             for genome_name, contig_file in zip(context.GENOME_NAMES, context.CONTIG_FILES):
                 try:
                     if genome := annotate_genome(genome_name, contig_file):
                         sqlite.add_new_genome_to_db(sql_connection=genome_db_connection,
                                                     genome=genome)
                         genome_dict[genome_name] = genome
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/antismash.py` & `metaerg-2.5.5/src/metaerg/run_and_read/antismash.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from metaerg import context
 from metaerg.datatypes import gbk
 from metaerg.datatypes import sqlite
 from metaerg.datatypes import functional_genes
 from metaerg.run_and_read import gene_writer
 
+ANNOTATOR_KEY = 'antismash'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     """Should execute the helper programs to complete the analysis"""
     gbk_file = context.spawn_file('gbk', genome.name, extension='gbk')
     with open(gbk_file, 'w') as handle:
         gbk.gbk_write_genome(handle, contig_dict, db_connection)
     if result_files[0].exists():
@@ -74,15 +75,15 @@
                     if existing_id[-1].isalpha():
                         return existing_id[:-1] + chr(ord(existing_id[-1]) + 1)
                     else:
                         return existing_id + 'a'
 
                 closest_gene = None
                 closest_distance = 100000
-                for f1 in sqlite.read_all_features(db_connection, contig=contig, start=max(g['start']-20000,0), end=g['end']+20000):
+                for f1 in sqlite.read_all_features(db_connection, contig=contig, start=max(g['start'] - 20000, 0), end=g['end'] + 20000):
                     new_distance = f1.start - g['start']
                     if new_distance < closest_distance:
                         closest_gene = f1
                         closest_distance = new_distance
                 if closest_gene:
                     new_id = create_new_id(closest_gene.id)
                 else:
@@ -92,29 +93,29 @@
                 new_feature = sqlite.Feature(id=new_id,
                                              genome=genome.name,
                                              contig=contig,
                                              start=g['start'],
                                              end=g['end'],
                                              strand=g['strand'],
                                              type=g['type'],
-                                             inference='antismash',
+                                             inference=ANNOTATOR_KEY,
                                              descr= ' '.join((region_feature.descr, antismash_gene_function,
                                                               antismash_gene_category)),
                                              aa_seq=g['translation'])
                 new_feature.parent = region_feature.id
                 new_feature.subsystems.append(functional_genes.SECONDARY_METABOLITE_GENE)
                 sqlite.add_new_feature_to_db(db_connection, new_feature)
             antismash_hit_count += 1
     return antismash_hit_count
 
 
 @context.register_annotator
 def run_and_read_antismash():
     return ({'pipeline_position': 91,
-             'annotator_key': 'antismash',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'prediction of secondary metabolite genes with antismash',
              'programs': ('antismash',),
              'result_files': ('antismash',),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/aragorn.py` & `metaerg-2.5.5/src/metaerg/run_and_read/aragorn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 
 from metaerg import context
 from metaerg.datatypes import fasta
 from metaerg.datatypes import sqlite
 
+ANNOTATOR_KEY = 'aragorn'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome.name)
     fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                       mask_targets=fasta.ALL_MASK_TARGETS)
     if not context.TRANSLATION_TABLE:
         set_translation_table(genome, 0, 0)
@@ -69,15 +70,15 @@
                                 seq = fasta.reverse_complement(seq)
                             feature = sqlite.Feature(genome = genome.name,
                                        contig = current_contig['id'],
                                        start = start,
                                        end = end,
                                        strand = strand,
                                        type = 'tRNA' if trna_type.startswith('tRNA') else 'tmRNA',
-                                       inference = 'aragorn',
+                                       inference = ANNOTATOR_KEY,
                                        nt_seq = seq,
                                        descr = f'{trna_type}-{codon}')
                             sqlite.add_new_feature_to_db(db_connection, feature)
                             count += 1
                         else:
                             context.log(f'Warning: Unexpected tRNA coordinates in "{line}" '
                                     f'at line {ln - 1} of {result_files[0]}')
@@ -94,14 +95,14 @@
         handle.write(str(table_id))
     genome.genetic_code = table_id
 
 
 @context.register_annotator
 def run_and_read_aragorn():
     return ({'pipeline_position': 11,
-             'annotator_key': 'aragorn',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'tRNA prediction with aragorn',
              'programs': ('aragorn',),
              'result_files': ("aragorn",),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/cdd.py` & `metaerg-2.5.5/src/metaerg/run_and_read/cdd.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from concurrent.futures import ProcessPoolExecutor
 
 from metaerg import context
 from metaerg.datatypes import functional_genes
 from metaerg.datatypes import fasta
 from metaerg.datatypes import sqlite
 from metaerg.datatypes.blast import DBentry, TabularBlastParser
-from metaerg.calculations.cluster_database import get_match_key
 
 CDD = {}
 CDD_CLUSTERS = {}
 CLUSTER_MAX_CDD_HITS = 5
 CLUSTER_MIN_MATCH_SCORE = 0.2
 
+ANNOTATOR_KEY = 'cdd'
+
 def _run_programs(genome, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome.name)
     cdd_database = Path(context.DATABASE_DIR, 'cdd', 'Cdd')
     if context.CPUS_PER_GENOME > 1:
         split_fasta_files = fasta.write_features_to_fasta(db_connection, 'aa', cds_aa_file, targets=('CDS',),
                                                                split=context.CPUS_PER_GENOME)
         split_cdd_files = [Path(result_files[0].parent, f'{result_files[0].name}.{i}')
@@ -40,29 +41,29 @@
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     cdd_result_count = 0
     subsystem_result_count = 0
     cdd_cluster_count = 0
     def get_cdd_db_entry(id: str) -> DBentry:
         return CDD[int(id[4:])]
-
     with TabularBlastParser(result_files[0], 'BLAST', get_cdd_db_entry) as handle:
         for cdd_result in handle:
             feature = sqlite.read_feature_by_id(db_connection, cdd_result.query())
             if not feature:
-                raise Exception(f'Found cdd result for unknown feature {cdd_result.query()}, '
+                context.log(f'({genome.name}) FATAL ERROR: Found {ANNOTATOR_KEY} result for unknown feature {cdd_result.query()}, '
+                                f'may need to rerun metaerg with --force')
+                raise Exception(f'({genome.name}) Found {ANNOTATOR_KEY} result for unknown feature {cdd_result.query()}, '
                                 f'may need to rerun metaerg with --force')
             # process the feature's cdd
             feature.cdd = cdd_result
             cdd_result_count += 1
-            if new_matches := functional_genes.match(cdd_result):
-                for new_match in new_matches:
-                    if not new_match in feature.subsystems:
-                        feature.subsystems.append(new_match)
-                        subsystem_result_count += 1
+            for new_match in functional_genes.match(cdd_result, number_of_hits_considered=5):
+                if not new_match in feature.subsystems:
+                    feature.subsystems.append(new_match)
+                    subsystem_result_count += 1
             top_entry: DBentry = cdd_result.hits[0].hit
             feature.descr = f'{top_entry.accession}|{top_entry.gene} {top_entry.descr}'
             if len(feature.descr) > 35:
                 feature.descr = feature.descr[:35] + '...'
             # write feature
             sqlite.update_feature_in_db(db_connection, feature)
 
@@ -87,15 +88,15 @@
     context.log(f'Parsed {len(CDD_CLUSTERS)} gene-context-associations for profiles.')
 
 
 
 @context.register_annotator
 def run_and_read_cdd():
     return ({'pipeline_position': 71,
-             'annotator_key': 'cdd',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'function prediction using RPSBlast and the conserved domain database',
              'programs': ('rpsblast',),
              'databases': (Path('cdd', 'cddid.tbl'), Path('cdd', 'Cdd.pal')),
              'result_files': ('cdd',),
              'run': _run_programs,
              'read': _read_results,
              'preload_db': preload_db})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/checkm.py` & `metaerg-2.5.5/src/metaerg/run_and_read/checkm.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/cmscan.py` & `metaerg-2.5.5/src/metaerg/run_and_read/cmscan.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from concurrent.futures import ProcessPoolExecutor
 from collections import namedtuple
 
 from metaerg import context
 from metaerg.datatypes import fasta
 from metaerg.datatypes import sqlite
 
+ANNOTATOR_KEY = 'cmscan'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome.name)
     rfam_database = Path(context.DATABASE_DIR, 'rfam', 'Rfam.cm')
     if context.CPUS_PER_GENOME > 1:
         split_fasta_files = fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                                          mask_targets=fasta.ALL_MASK_TARGETS,
@@ -87,26 +88,26 @@
             seq = fasta.reverse_complement(seq)
         feature = sqlite.Feature(genome = genome.name,
                    contig = hit.query_id,
                    start = hit.query_start - 1,
                    end = hit.query_end,
                    strand = hit.query_strand,
                    type = f_type,
-                   inference = 'cmscan',
+                   inference = ANNOTATOR_KEY,
                    nt_seq = seq,
                    descr = "{} {}".format(hit.hit_id, hit.descr))
         sqlite.add_new_feature_to_db(db_connection, feature)
         count += 1
     return count
 
 
 @context.register_annotator
 def run_and_read_cmscan():
     return ({'pipeline_position': 21,
-             'annotator_key': 'cmscan',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'noncoding (RNA) gene prediction with cmscan',
              'programs': ('cmscan',),
              'result_files': ("cmscan",),
              'databases': (Path('rfam', 'Rfam.cm'),),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/comparative_genomics.py` & `metaerg-2.5.5/src/metaerg/run_and_read/comparative_genomics.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,14 +423,15 @@
         for feature_id, taxon, is_paralogue, cluster in targets:
             feature = sqlite.read_feature_by_id(db_connection, feature_id)
             feature.homologous_group_feature_is_paralogue = is_paralogue
             feature.homologous_group_id = int(cluster.id)
             feature.homologous_group_taxon_representation = len(cluster.taxa) / len(all_taxa)
             feature.homologous_group_member_count = len(cluster.members)
             sqlite.update_feature_in_db(db_connection, feature)
+        sqlite.write_db(db_connection, db_file)
 
 
 def analyse_gene_context(cluster_list, all_taxa: list, window_size: int = 4, min_match_score: float = 0.5) -> dict:
     context.log("Now analysing gene context to identify homologous genes frequently found together...")
     context.log(f"Working with window size {window_size} and requiring {min_match_score:.1%} of pairs of homologous genes to be found close to each other.")
     profile_match_counts = Counter()
     for i, taxon in zip(range(len(all_taxa)), all_taxa):
@@ -531,14 +532,15 @@
                                             id=f'region_{region_id}')
             sqlite.add_new_feature_to_db(db_connection, region_feature)
             for f in sqlite.read_all_features(db_connection, contig=region_feature.contig,
                                               start=region_feature.start, end=region_feature.end):
                 if f.type != 'region':
                     f.parent = region_feature.id
                     sqlite.update_feature_in_db(db_connection, f)
+        sqlite.write_db(db_connection, db_file)
         context.log(f"Wrote {len(existing_regions)} homology-informed sequence regions to sql for '{taxon}'")
 
 
 def run(genome_dict: dict, cluster_window_size: int = 4, min_match_score: float = 0.5):
     context.log('Mode "comparative_genomics": Clustering and analysing homologous genes across genomes...')
     # prep/clear dirs
     cds_input_data_dir = context.BASE_DIR / 'faa'
@@ -601,16 +603,16 @@
     cluster_context_links = analyse_gene_context(cluster_list, taxa, cluster_window_size, min_match_score)
     write_overview_tsv_file(comparative_genomics_dir, cluster_list, taxa)
     write_remaining_results_to_sql(cluster_list, cluster_context_links, taxa, cluster_window_size)
     context.log('Updating html visualizations for all genomes...')
     for genome_name, genome in genome_dict.items():
         context.log(f'({genome_name}) Now writing final result as .html for visualization...')
         feature_db_connection = sqlite.connect_to_db(context.BASE_DIR / 'annotations.sqlite' / genome_name)
-        for html_writer in registry.HTML_WRITER_REGISTRY:
-            html_writer(genome, feature_db_connection, context.HTML_DIR)
+        html_feature_table.write_html(genome, feature_db_connection, context.HTML_DIR)
+        html_feature_details.write_html(genome, feature_db_connection, context.HTML_DIR)
 
 
 def make_match_key(id1: int, id2: int):
     if id1 > id2:
         return f'{id1} {id2}'
     else:
         return f'{id2} {id1}'
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/crispr_detect.py` & `metaerg-2.5.5/src/metaerg/run_and_read/crispr_detect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from metaerg import context
 from metaerg.datatypes import fasta, gff, sqlite
 
+ANNOTATOR_KEY = 'crispr_detect'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     """Executes the helper programs to complete the analysis"""
     result_file_without_extension = result_files[0].parent / result_files[0].stem
     fasta_file = context.spawn_file('masked', genome.name)
     fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
@@ -21,27 +22,27 @@
             file.chmod(0o666)  # crisprdetect for some reason makes results files executable - set permission to r/w
     if result_files[0].suffix != '.gff':
         (result_files[0].parent / (result_files[0].stem + '.gff')).rename(result_files[0].parent / result_files[0].stem)
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     """Should parse the result files and return the # of positives"""
-    with gff.GffParser(result_files[0], contig_dict) as gff_parser:
+    with gff.GffParser(result_files[0], contig_dict=contig_dict, inference=ANNOTATOR_KEY) as gff_parser:
         count = 0
         for feature in gff_parser:
             feature.genome = genome.name
             if 'direct_repeat' == feature.type:
                 feature.type = 'CRISPR'
                 count += 1
             sqlite.add_new_feature_to_db(db_connection, feature)
     return count
 
 
 @context.register_annotator
 def run_and_read_crispr_detect():
     return ({'pipeline_position': 2,
-             'annotator_key': 'crispr_detect',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'CRISPR prediction with CRISPRDetect',
              'programs': ('CRISPRDetect.pl',),
              'result_files': ("crispr_detect.gff",),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/data/functional_gene_data` & `metaerg-2.5.5/src/metaerg/run_and_read/data/functional_gene_data`

 * *Files 3% similar despite different names*

```diff
@@ -437,16 +437,49 @@
 2 COG2181 nitrate reductase gamma subunit (narI, narV, ec:1.7.5.1)
 1 PRK13532|TIGR01706 periplasmic nitrate reductase (NapA)
 2 COG3043|cl01153 periplasmic nitrate reductase (NapB)
 1 A0A0B5GVF0|A0A0U3NDF4|A0A0U5N0A2|A0A0X8K2K6|A0A168G368|D5MLH7|F8D6S2|Q2SXG4|Q9YCG9|A0A1W1I2B6|Q1QHW9 nxrA; nitrate reductase / nitrite oxidoreductase, alpha subunit Nitrobacter (ec:1.7.5.1)
 2 A0A0H3GNX1|A0A1Y0HZR5|A8M8C4|D2PSR0|J7LAS1|L0JX22|Q1QHX1|A0A1W1I5Y1 nxrB; nitrate reductase / nitrite oxidoreductase, beta subunit (ec:1.7.5.1)
 
 >Nitrogen Cycle, Denitrification
-1 A0A0F6Z3B6|A0A0K0XU36|A7NPI4|C7RR96|R4YN15 Nitrite reductase (NO-forming) / hydroxylamine reductase NirS
-1 A0A075TX59|A0A0D5C031|A0A0D5L9A8|A0A0G3G6R0|A0A0K2GJ77|A0A0K2HAK1|A0A0S2TH06|A0A0X8K2L5|A0A128A0R2|A0A1Q1FME2|A0A1Q2TQW5|A0A1S6FCE7|A0A291G5N2|A3P6P0|D3P4B7|D8JSS7|E1VIX6|E1W6F5|E6SGG5|F4GPW7|K0IEZ7|Q47L45|S5TI99 Nitrite reductase (NO-forming) NirK
+1 NirK_Clade1a!NirK_outgroup Nitrite reductase NirK Clade 1a
+1 NirK_Clade1b!NirK_outgroup Nitrite reductase NirK Clade 1b
+1 NirK_Clade1c!NirK_outgroup Nitrite reductase NirK Clade 1c
+1 NirK_Clade1d!NirK_outgroup Nitrite reductase NirK Clade 1d
+1 NirK_Clade1e!NirK_outgroup Nitrite reductase NirK Clade 1e
+1 NirK_Clade1f!NirK_outgroup Nitrite reductase NirK Clade 1f
+1 NirK_Clade1g!NirK_outgroup Nitrite reductase NirK Clade 1g
+1 NirK_Clade2!NirK_outgroup Nitrite reductase NirK Clade 2
+1 NirK_Clade3!NirK_outgroup Nitrite reductase NirK Clade 3
+1 NirK_Clade4!NirK_outgroup Nitrite reductase NirK Clade 4
+1 NirK_Clade5!NirK_outgroup Nitrite reductase NirK Clade 5
+1 NirK_Clade6!NirK_outgroup Nitrite reductase NirK Clade 6
+1 NirK_Clade7!NirK_outgroup Nitrite reductase NirK Clade 7
+1 NirK_Clade8!NirK_outgroup Nitrite reductase NirK Clade 8
+1 NirK_Clade9!NirK_outgroup Nitrite reductase NirK Clade 9
+1 NirK_Clade10!NirK_outgroup Nitrite reductase NirK Clade 10
+1 NirK_Clade11!NirK_outgroup Nitrite reductase NirK Clade 11
+1 NirS_Clade1a!NirF|NirN cd1 nitrite reductase NirS Clade 1a
+1 NirS_Clade1b!NirF|NirN cd1 nitrite reductase NirS Clade 1b
+1 NirS_Clade1c!NirF|NirN cd1 nitrite reductase NirS Clade 1c
+1 NirS_Clade1d!NirF|NirN cd1 nitrite reductase NirS Clade 1d
+1 NirS_Clade1e!NirF|NirN cd1 nitrite reductase NirS Clade 1e
+1 NirS_Clade1f!NirF|NirN cd1 nitrite reductase NirS Clade 1f
+1 NirS_Clade1g!NirF|NirN cd1 nitrite reductase NirS Clade 1g
+1 NirS_Clade1h!NirF|NirN cd1 nitrite reductase NirS Clade 1h
+1 NirS_Clade1i!NirF|NirN cd1 nitrite reductase NirS Clade 1i
+1 NirS_Clade1j!NirF|NirN cd1 nitrite reductase NirS Clade 1j
+1 NirS_Clade1k!NirF|NirN cd1 nitrite reductase NirS Clade 1k
+1 NirS_Clade2!NirF|NirN cd1 nitrite reductase NirS Clade 2
+1 NirS_Clade3!NirF|NirN cd1 nitrite reductase NirS Clade 3
+1 NirS_Clade4!NirF|NirN cd1 nitrite reductase NirS Clade 4
+1 NirS_Clade5!NirF|NirN cd1 nitrite reductase NirS Clade 5
+1 NirS_ArchaealHalophiles!NirF|NirN cd1 nitrite reductase NirS Archaeal-type
+1 NirF cd1 nitrite reductase NirS, accessory protein NirF
+1 NirN cd1 nitrite reductase NirS accessory protein NirN
 2 hco_BNOR Heme-copper oxidase B1-family, cyt c dependent nitric oxide reductases (bNOR)
 3 hco_B1subII Heme-copper oxidase B1-family, subunit II
 2 hco_CNOR Heme-copper oxidase C-family cyt c dependent nitric oxide reductases (cNOR)
 3 hco_CsubII Heme-copper oxidase C-family, subunit II
 2 hco_ENOR Heme-copper oxidase B9-family cyt c dependent nitric oxide reductases (eNOR)
 3 hco_ENORsubII Heme-copper oxidase B9-family eNOR, subunit II
 2 hco_GNOR Heme-copper oxidase B6/7-family cyt c dependent nitric oxide reductases (gNOR)
@@ -656,14 +689,29 @@
 7 TIGR01750|PRK00006|cd01288 Beta-hydroxyacyl-(acyl-carrier-protein) dehydratase FabZ
 8 TIGR02445|pfam09403|PRK08947 Acetyl-CoA C-acyltransferase FadA
 9 TIGR02437|PRK11730|COG1250 Fatty oxidation complex, alpha subunit FadB
 10 PRK05557|PRK05565|PRK05786|PRK06077|PRK06463|PRK06550|PRK07666|PRK07792|PRK08217|PRK08261|PRK08642|PRK12825 3-Oxoacyl-acyl-carrier protein reductase FabG
 11 PRK08063 Enoyl-acyl-carrier-protein reductase FabL
 12 PRK13656 Enoyl-acyl-carrier-protein reductase FabV
 
+>Metabolism, Phosphonate Biosynthesis
+1 TIGR02320 Phosphoenolpyruvate mutase, PepM
+2 TIGR03297 Phosphonopyruvate decarboxylase, Ppd/AepY
+3 cd08182 Hydroxyethylphosphoate dehydrogenase HepD/PhpC
+4 TIGR03405 Phosphonate-associated iron-containing alcohol dehydrogenase
+
+>Metabolism, Phosphonate Degradation, Generic Pathway
+1 cl01456|COG3626|pfam05861 Alpha-D-ribose 1-methylphosphonate 5-triphosphate synthase, PhnI
+2 COG3454|PRK15446|TIGR02318 Alpha-D-ribose 1-methylphosphonate 5-triphosphate diphosphatase, PhnM
+3 COG3627 Alpha-D-ribose 1-methylphosphonate 5-phosphate C-P lyase, PhnJ
+
+>Metabolism, Phosphonate Degradation, Specific Pathways
+1 TIGR00686|TIGR02335 alkylphosphonate utilization operon protein, PhnA
+1 TIGR02321 Phosphoenolpyruvate hydrolase, PalA
+
 >Metabolism, Inositol Phosphate Biosynthesis
 1 pfam16670|PLN02222|PLN02223|PLN02230|PLN02952 Phosphoinositide phospholipase C
 2 pfam16726 Inositol polyphosphate 5-phosphatase clathrin binding domain
 3 PRK10757 Inositol-1-monophosphatase SuhB
 4 COG1260 Myo-inositol-1-phosphate synthase
 5 PLN02438 Inositol-3-phosphate synthase
 6 TIGR04380|cl40708 Inositol 2-dehydrogenase IolG
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/deepsig.py` & `metaerg-2.5.5/src/metaerg/run_and_read/deepsig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from pathlib import Path
 
 from metaerg import context
 from metaerg.datatypes import sqlite
 
 
+ANNOTATOR_KEY = 'deepsig'
+
+
 def _run_programs(genome, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome.name)
     context.run_external(f'deepsig -f {cds_aa_file} -o {result_files[1]} -k gramn')
     context.run_external(f'deepsig -f {cds_aa_file} -o {result_files[0]} -k gramp')
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
@@ -18,15 +21,17 @@
                 words = line.strip().split('\t')
                 match words:
                     case [feature_id, _, 'Chain', start, end, score, _, _, _]:
                         pass
                     case [feature_id, _, 'Signal peptide', start, end, score, _, _, _]:
                         feature = sqlite.read_feature_by_id(db_connection, feature_id)
                         if not feature:
-                            raise Exception(f'({genome.name}) Found deepsig result for unknown feature {feature_id}, '
+                            context.log(f'({genome.name}) FATAL ERROR: Found {ANNOTATOR_KEY} result for unknown feature {feature_id}, '
+                                        f'may need to rerun metaerg with --force')
+                            raise Exception(f'({genome.name}) Found {ANNOTATOR_KEY} result for unknown feature {feature_id}, '
                                             f'may need to rerun metaerg with --force')
                         if feature.signal_peptide:
                             feature.signal_peptide += ','
                         else:
                             count += 1
                         feature.signal_peptide += f'{source}({end})'
                         sqlite.update_feature_in_db(db_connection, feature)
@@ -34,15 +39,15 @@
                         context.log(f'({genome.name}) Warning: Deepsig result file "{file}" contains unknown/new signal type "{x}"')
     return count
 
 
 @context.register_annotator
 def run_and_read_pureseqtm():
     return ({'pipeline_position': 122,
-             'annotator_key': 'deepsig',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'signal peptide prediction with DeepSig',
              'programs': ('deepsig',),
              'result_files': ('deepsig_gram-negative','deepsig_gram-positive'),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/diamond_and_blastn.py` & `metaerg-2.5.5/src/metaerg/run_and_read/diamond_and_blastn.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 IGNORED_FEATURE_TYPES = 'gene pseudogene exon direct_repeat region sequence_feature pseudogenic_tRNA pseudogenic_rRNA ' \
                         'repeat_region ribosome_entry_site minus_10_signal minus_35_signal protein_binding_site ' \
                         'regulatory transcript mRNA gap assembly_gap source misc_feature variation misc_structure ' \
                         'transcript 3\'UTR 5\'UTR intron signal_peptide_region_of_CDS sequence_alteration'.split()
 
 TAXONOMY = {'p': {}, 'e': {}, 'v': {}}
 DESCRIPTIONS = {'p': {}, 'e': {}, 'v': {}}
-
+ANNOTATOR_KEY = 'diamond_and_blastn'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     rna_nt_file = context.spawn_file('rna.fna', genome.name)
     blastn_result_file = context.spawn_file('blastn', genome.name)
     if rna_nt_file.exists() and rna_nt_file.stat().st_size:
         blastn_db = Path(context.DATABASE_DIR, DB_RNA_FILENAME)
         context.run_external(f'blastn -db {blastn_db} -query {rna_nt_file} -out {blastn_result_file} -max_target_seqs 10 '
@@ -52,14 +52,16 @@
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     taxon_counts = Counter()
     def process_blast_result(blast_result: BlastResult):
         feature = sqlite.read_feature_by_id(db_connection, blast_result.query())
         if not feature:
+            context.log(f'({genome.name}) FATAL ERROR: Found {ANNOTATOR_KEY} result for unknown feature {blast_result.query()}, '
+                        f'may need to rerun metaerg with --force')
             raise Exception(f'Found diamond_and_blastn result for unknown feature {blast_result.query()}, '
                             f'may need to rerun metaerg with --force')
         feature.blast = blast_result
         feature.descr = blast_result.hits[0].hit.descr
         feature.taxon =  blast_result.hits[0].hit.taxon
         sqlite.update_feature_in_db(db_connection, feature)
         taxon_counts.update((feature.taxon,))
@@ -114,15 +116,15 @@
     context.log(f'Parsed ({len(TAXONOMY["p"])}, {len(TAXONOMY["e"])}, {len(TAXONOMY["v"])}) '
                 f'taxa from db for (prokaryotes, eukaryotes and viruses) respectively.')
 
 
 @context.register_annotator
 def run_and_read_diamond_blastn():
     return ({'pipeline_position': 81,
-             'annotator_key': 'diamond_and_blastn',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'function prediction and taxonomic classification of genes with diamond and blastn',
              'programs': ('diamond', 'blastn'),
              'databases': (Path(DB_PROTEINS_FILENAME + '.dmnd'),
                            Path(DB_RNA_FILENAME + '.nhr'),
                            Path(DB_DESCRIPTIONS_FILENAME),
                            Path(DB_TAXONOMY_FILENAME)),
              'result_files': ('diamond',),
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/functional_genes.py` & `metaerg-2.5.5/src/metaerg/run_and_read/functional_genes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import gzip
 import shutil
-from math import log10
 from pathlib import Path
 from concurrent import futures
+from zipfile import ZipFile
 
 from metaerg.datatypes.blast import DBentry, TabularBlastParser
-from metaerg.datatypes import sqlite
+from metaerg.datatypes import sqlite, fasta
 from metaerg import context
 from metaerg.datatypes import functional_genes
 from metaerg.calculations.codon_usage_bias import compute_codon_bias_estimate_doubling_time
 
+ANNOTATOR_KEY = 'hmm'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome.name)
     hmm_db = context.DATABASE_DIR / 'hmm' / 'functional_genes.hmm'
     # the domtbl format includes alignment starts and ends, so we can use that information...
     context.run_external(f'hmmscan -o /dev/null -E 1e-6 --domtblout {result_files[0]} {hmm_db} {cds_aa_file}')
 
@@ -38,58 +39,53 @@
             elif line.startswith('DESC'):
                 db_entry.descr = line[4:].strip()
             elif line.startswith('LENG'):
                 db_entry.length = int(line[4:].strip())
     context.log(f'({genome.name}) {len(functional_gene_db)} functional gene profiles in database.')
 
     def get_db_entry(db_id) -> DBentry:
-        return functional_gene_db[db_id]
+        try:
+            return functional_gene_db[db_id]
+        except KeyError:
+            context.log(f'({genome.name}) Unkown hmm database id "{db_id}". Did the hmm database change after this prediction was done?')
+            raise Exception(f'({genome.name}) Unkown hmm database id "{db_id}". Did the hmm database change after this prediction was done?')
+
 
     with TabularBlastParser(result_files[0], 'HMMSCAN_DOM_TABLE', get_db_entry) as handle:
         hit_count = 0
         for blast_result in handle:
             feature = sqlite.read_feature_by_id(db_connection, blast_result.query())
             if not feature:
-                raise Exception(f'Found functional gene result for unknown feature {blast_result.query()}, '
+                context.log(
+                    f'({genome.name}) FATAL ERROR: Found {ANNOTATOR_KEY} result for unknown feature {blast_result.query()}, '
+                    f'may need to rerun metaerg with --force')
+                raise Exception(f'Found {ANNOTATOR_KEY} result for unknown feature {blast_result.query()}, '
                                 f'may need to rerun metaerg with --force')
-            blast_result.hits = blast_result.hits[:10]
+            if new_matches := functional_genes.match(blast_result, number_of_hits_considered=1):
+                hit_count += 1
+                for new_match in new_matches:
+                    if not new_match in feature.subsystems:
+                        feature.subsystems.append(new_match)
+            blast_result.hits = blast_result.hits[:5]
             feature.hmm = blast_result
-            for h in blast_result.hits:
-                db_entry = h.hit
-                confidence = 1.0
-                if h.aligned_length / db_entry.length < 0.7:
-                    continue
-                if db_entry.min_score:
-                    if h.score < db_entry.min_score:
-                        continue
-                    confidence = h.score / db_entry.min_t_score
-                else:
-                    if h.evalue > 0:
-                        confidence = min(1.0, - log10(h.evalue) / 100)
-                if new_matches := functional_genes.match_hit(h, confidence):
-                    hit_count += 1
-                    for new_match in new_matches:
-                        if not new_match in feature.subsystems:
-                            feature.subsystems.append(new_match)
-                break
             sqlite.update_feature_in_db(db_connection, feature)
     # with all subsystems annotated, we are ready to update the genome's subsystems:
     genome.codon_usage_bias, genome.doubling_time = compute_codon_bias_estimate_doubling_time(db_connection)
     genome.subsystems = functional_genes.aggregate(db_connection)
     for subsystem, subsystem_genes in genome.subsystems.items():
         subsystem_completeness = functional_genes.get_subsystem_completeness(subsystem, subsystem_genes)
         genome.subsystem_summary[subsystem] = subsystem_completeness
 
     return hit_count
 
 
 @context.register_annotator
 def run_and_read_canthyd():
     return ({'pipeline_position': 101,
-             'annotator_key': 'hmm',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'identification of functional genes with HMMs',
              'programs': ('hmmscan',),
              'databases': (Path('hmm', 'functional_genes.hmm'),),
              'result_files': ('hmm',),
              'run': _run_programs,
              'read': _read_results,
              'preload_db': functional_genes.init_functional_gene_config})
@@ -142,37 +138,39 @@
     if 'S' not in context.DATABASE_TASKS:
         return
 
     functional_genes.init_functional_gene_config()
     all_target_hmm_names = set()
     for gene_def in functional_genes.GENES:
         all_target_hmm_names.update(gene_def.cues)
+        all_target_hmm_names.update(gene_def.anti_cues)
 
     hmm_dir = context.DATABASE_DIR / 'hmm'
     hmm_dir.mkdir(exist_ok=True, parents=True)
     user_hmm_dir = hmm_dir / 'user_hmm'
     (hmm_dir / 'user_config').mkdir(exist_ok=True, parents=True)  # used by functional_genes.py
     user_hmm_dir.mkdir(exist_ok=True, parents=True)  # used below
     context.log(f'Installing functional gene hmm database at {hmm_dir}...')
-
     current_working_dir = os.getcwd()
+
     # fetch bd type oxygen reductases
     bdor_dir = hmm_dir / 'bdor'
     if bdor_dir.exists():
         shutil.rmtree(bdor_dir)
     bdor_dir.mkdir()
     os.chdir(bdor_dir)
     os.system('git init')
     os.system('git remote add bdor https://github.com/ranjani-m/cytbd-superfamily.git')
     os.system('git fetch bdor')
     os.system('git checkout bdor/main -- Cytbd_HMM_2020_paper_version')
     with open(hmm_dir / 'bdor.hmm', 'w') as writer:
         for hmm_file in sorted((bdor_dir / 'Cytbd_HMM_2020_paper_version').glob('*.hmm')):
             os.system(f'sed -i "s|^NAME.*|NAME  bdor_{hmm_file.stem}|" {hmm_file}')
             context.run_external(f'/bio/bin/hmmer3/bin/hmmconvert {hmm_file}', stdout=writer)
+
     # fetch heme copper oxidase hmms
     hco_dir = hmm_dir / 'hco'
     if hco_dir.exists():
         shutil.rmtree(hco_dir)
     hco_dir.mkdir()
     os.chdir(hco_dir)
     os.system('git init')
@@ -180,17 +178,44 @@
     os.system('git fetch hco')
     os.system('git checkout hco/main -- HMM')
     with open(hmm_dir / 'hco.hmm', 'w') as writer:
         for hmm_file in sorted((hco_dir / 'HMM').glob('*.hmm')):
             os.system(f'sed -i "s|^NAME.*|NAME  hco_{hmm_file.stem}|" {hmm_file}')
             context.run_external(f'hmmconvert {hmm_file}', stdout=writer)
 
-    # unzip hmms from data
+    # fetch nitrite reductase data from Pold et al. (2024) ISME Reports...
+    nir_hmm_file = hmm_dir / 'nir.hmm'
+    hmm_nir_install_dir = hmm_dir / 'nir'
+    hmm_nir_install_dir.mkdir(exist_ok=True, parents=True)
+    os.chdir(hmm_nir_install_dir)
+    os.system('wget -q https://figshare.com/ndownloader/articles/23913078/versions/1')
+    nir_archive_file = hmm_nir_install_dir / '1'
+    with ZipFile(nir_archive_file, 'r') as zipped_file:
+        zipped_file.extractall(path=hmm_nir_install_dir)
+    nir_hmm_archive_file = hmm_nir_install_dir / 'clade_specific_HMMs.zip'
+    with ZipFile(nir_hmm_archive_file, 'r') as zipped_file:
+        zipped_file.extractall(path=hmm_nir_install_dir)
+    with open(nir_hmm_file, 'w') as nir_hmm_writer:
+        for f in sorted((hmm_nir_install_dir / 'clade_specific_HMMs' / 'NirK').glob('*.hmm')):
+            with open(f, 'r') as reader:
+                for l in reader:
+                    if l.startswith('NAME'):
+                        l = 'NAME  NirK_' + l[6:]
+                    nir_hmm_writer.write(l)
+        for f in sorted((hmm_nir_install_dir / 'clade_specific_HMMs' / 'NirS').glob('*.hmm')):
+            with open(f, 'r') as reader:
+                for l in reader:
+                    if l.startswith('NAME  Clade') or l.startswith('NAME  Arch'):
+                        l = 'NAME  NirS_' + l[6:]
+                    nir_hmm_writer.write(l)
+    shutil.rmtree(hmm_nir_install_dir)
+
+    # unzip hmms from metaerg python module
     hmm_data_dir = Path(__file__).parent / 'data'
-    print (hmm_data_dir)
+    context.log(f'Now unpacking hmm data from {hmm_data_dir}')
     for hmm_file in hmm_data_dir.glob('*.hmm.gz'):
         with gzip.open(hmm_file, 'rb') as f_in:
             dest_hmm_file = hmm_dir / hmm_file.stem
             print ('unzipping to ', dest_hmm_file)
             with open(dest_hmm_file, 'wb') as f_out:
                 shutil.copyfileobj(f_in, f_out)
 
@@ -213,7 +238,62 @@
                 continue
             add_hmm_file_to_db(hmm_file, output, names_done, all_target_hmm_names)
         for f in user_hmm_dir.glob('*.hmm'):
             hmm_file = f.absolute()
             add_hmm_file_to_db(hmm_file, output, names_done, all_target_hmm_names)
     context.run_external(f'hmmpress -f {hmm_dir / "functional_genes.hmm"}')
     os.chdir(current_working_dir)
+
+
+def collect_nir_hmms():
+    context.log(f'Installing Nir HMMs from Pold et al. (2024) ISME Reports...')
+    hmm_nir_install_dir = context.DATABASE_DIR / 'hmm' / 'nir'
+    hmm_nir_install_dir.mkdir(exist_ok=True, parents=True)
+    os.chdir(hmm_nir_install_dir)
+    os.system('wget -q https://figshare.com/ndownloader/articles/23913078/versions/1')
+    nir_archive_file = hmm_nir_install_dir / '1'
+    with ZipFile(nir_archive_file, 'r') as zipped_file:
+        zipped_file.extractall(path=hmm_nir_install_dir)
+    nir_hmm_archive_file = hmm_nir_install_dir / 'clade_specific_HMMs.zip'
+    with ZipFile(nir_hmm_archive_file, 'r') as zipped_file:
+        zipped_file.extractall(path=hmm_nir_install_dir)
+    nir_hmm_archive_dir = hmm_nir_install_dir / 'clade_specific_HMMs'
+    nirk_hmm_archive_dir = nir_hmm_archive_dir / 'NirK'
+    nirk_fasta_dir = nirk_hmm_archive_dir / 'fasta'
+    nirk_hmm_dir = nirk_hmm_archive_dir / 'hmm'
+    nirk_fasta_dir.mkdir(exist_ok=True, parents=True)
+    nirk_hmm_dir.mkdir(exist_ok=True, parents=True)
+    for f in nirk_hmm_archive_dir.glob('*.hmm'):
+        with open(f, 'r') as reader, open(nirk_hmm_dir / f.name, 'w') as writer:
+            for l in reader:
+                if l.startswith('NAME'):
+                    l = 'NAME  NirK_' + l[6:]
+                writer.write(l)
+    for f in nirk_hmm_archive_dir.glob('*.fasta'):
+        with fasta.FastaParser(f, cleanup_seq=True) as reader, open(nirk_fasta_dir / f.name, 'w') as writer:
+            for fe in reader:
+                fe['seq'] = fe['seq'].replace('X', '')
+                fasta.write_fasta(writer, fe)
+    nirs_hmm_archive_dir = nir_hmm_archive_dir / 'NirS'
+    nirs_fasta_dir = nirs_hmm_archive_dir / 'fasta'
+    nirs_hmm_dir = nirs_hmm_archive_dir / 'hmm'
+    nirs_fasta_dir.mkdir(exist_ok=True, parents=True)
+    nirs_hmm_dir.mkdir(exist_ok=True, parents=True)
+    for f in nirs_hmm_archive_dir.glob('*.hmm'):
+        with open(f, 'r') as reader, open(nirs_hmm_dir / f.name, 'w') as writer:
+            for l in reader:
+                if l.startswith('NAME  Clade') or l.startswith('NAME  Arch'):
+                    l = 'NAME  NirS_' + l[6:]
+                writer.write(l)
+    for f in nirs_hmm_archive_dir.glob('*.fasta'):
+        with fasta.FastaParser(f, cleanup_seq=True) as reader, open(nirs_fasta_dir / f.name, 'w') as writer:
+            for fe in reader:
+                fe['seq'] = fe['seq'].replace('X', '')
+                fasta.write_fasta(writer, fe)
+
+def main():
+    context.DATABASE_DIR = Path('/bio/data/databases/metaerg')
+    collect_nir_hmms()
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/gene_writer.py` & `metaerg-2.5.5/src/metaerg/run_and_read/gene_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         #if feature.type == 'repeat_region':
         #    context.log(f"{feature.type}: {feature.id}")
         # some features already got an id assigned, to keep track of gene clusters
         if feature.parent:
             try:
                 feature.parent = preliminary_id_mapping[feature.parent]
             except KeyError:
-                context.log(f'WARNING: Unknown feature parent {feature.parent} reference for {feature.id}')
+                context.log(f'WARNING in gene_writer: Unknown feature parent {feature.parent} reference for {feature.id}')
         if feature.id:
             prelim_id = feature.id
         feature.id = create_new_id(genome.name, feature.contig, j)
         preliminary_id_mapping[prelim_id] = feature.id
         j += 1
         sqlite.update_feature_in_db(db_connection, feature)
         # update genome
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/ltr_harvest.py` & `metaerg-2.5.5/src/metaerg/run_and_read/ltr_harvest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from metaerg import context
 from metaerg.datatypes import fasta
 from metaerg.datatypes import gff
 from metaerg.datatypes import sqlite
 
+ANNOTATOR_KEY = 'ltr_harvest'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome.name)
     fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
     ltr_index_file = context.spawn_file('ltr_index', genome.name)
 
@@ -15,25 +16,25 @@
     # remove index files
     for file in ltr_index_file.parent.glob(f'{genome.name}.ltr_index*'):
         file.unlink()
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     count = 0
-    with gff.GffParser(result_files[0], contig_dict, inference='ltr_harvest',
+    with gff.GffParser(result_files[0], contig_dict, inference=ANNOTATOR_KEY,
                        target_feature_type_dict={'repeat_region': 'retrotransposon'}) as parser:
         for feature in parser:
             feature.descr = 'LTR retrotransposon'
             sqlite.add_new_feature_to_db(db_connection, feature)
             count += 1
     return count
 
 
 @context.register_annotator
 def run_and_read_ltr_harvest():
     return ({'pipeline_position': 31,
-             'annotator_key': 'ltr_harvest',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'retrotransposon prediction with ltrharvest',
              'programs': ('gt',),
              'result_files': ('ltr_harvest',),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/minced.py` & `metaerg-2.5.5/src/metaerg/run_and_read/minced.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from metaerg import context
 from metaerg.datatypes import fasta, gff, sqlite
 
+ANNOTATOR_KEY = 'minced'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     """Executes the helper programs to complete the analysis"""
     fasta_file = context.spawn_file('masked', genome.name)
     fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
     context.run_external(f'minced -gffFull {fasta_file} {result_files[0]}')
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     """Should parse the result files and return the # of positives"""
-    with gff.GffParser(result_files[0], contig_dict, inference='minced',
+    with gff.GffParser(result_files[0], contig_dict, inference=ANNOTATOR_KEY,
                        target_feature_type_dict={'repeat_unit': 'CRISPR'}) as gff_parser:
         count = 0
         for feature in gff_parser:
             feature.genome = genome.name
             sqlite.add_new_feature_to_db(db_connection, feature)
             count += 1
     return count
 
 
 #@context.register_annotator  # (to enable minced, uncomment and add to __init__
 def run_and_read_minced():
     return ({'pipeline_position': 1,
-             'annotator_key': 'minced',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'CRISPR prediction with minced',
              'programs': ('minced',),
              'result_files': ("minced",),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/padloc.py` & `metaerg-2.5.5/src/metaerg/run_and_read/padloc.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pathlib import Path
 
 from metaerg import context
 from metaerg.datatypes import gff
 from metaerg.datatypes import sqlite
 from metaerg.datatypes.functional_genes import FunctionalGene
 
+ANNOTATOR_KEY = 'padloc'
+
 def _run_programs(genome, contig_dict, db_connection, result_files):
     gff_file = context.spawn_file('gff', genome.name, extension='gff')
     with open(gff_file, 'w') as handle:
         gff.gff_write_genome(handle, contig_dict, db_connection)
     cds_aa_file = context.spawn_file('cds.faa', genome.name)
     padloc_database_path = context.DATABASE_DIR / 'padloc'
     # crispr_detect_gff_path = context.spawn_file('crispr_detect.gff', genome.name)
@@ -30,22 +32,25 @@
         return 0
     padloc_features = []
     padloc_feature_systems = {}
     with gff.GffParser(padloc_result_file) as gff_parser:
         for pf in gff_parser:
             # padloc does not report the origal gene id, so we find the genes by their start position
             found_feature = False
-            for f in sqlite.read_all_features(db_connection, additional_sql = f'start = {pf.start}'):
+            for f in sqlite.read_all_features(db_connection, additional_sql =f'start = {pf.start}'):
                 f.subsystems.append(FunctionalGene(f'Defense ({pf.type})', pf.id, 1))
                 padloc_features.append(f)
                 padloc_feature_systems[f] = pf.type  # we do not have easy access to the Functional Gene
                 found_feature = True
                 break
             if not found_feature:
-                raise Exception(f'Found padloc result for unknown feature at position {pf.start}, '
+                context.log(
+                    f'({genome.name}) FATAL ERROR: Found {ANNOTATOR_KEY} result for unknown feature at position {pf.start}, '
+                    f'may need to rerun metaerg with --force')
+                raise Exception(f'Found {ANNOTATOR_KEY} result for unknown feature at position {pf.start}, '
                                 f'may need to rerun metaerg with --force')
 
     # manage clusters
     region_features = []
     current_region_feature = None
     padloc_features.sort(key=lambda x: (x.contig, padloc_feature_systems[x], x.start))
     # first we simply create a region for cds that are close and have the same padloc "type"
@@ -92,15 +97,15 @@
             sqlite.update_feature_in_db(db_connection, r)
     return len(padloc_features)
 
 
 @context.register_annotator
 def run_and_read_antismash():
     return ({'pipeline_position': 92,
-             'annotator_key': 'padloc',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'prediction of antiviral defense mechanisms',
              'programs': ('padloc',),
              'result_files': ('padloc',),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/prodigal.py` & `metaerg-2.5.5/src/metaerg/run_and_read/prodigal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import re
 
 from metaerg import context
 from metaerg.datatypes import fasta
 from metaerg.datatypes import sqlite
 
+ANNOTATOR_KEY = 'prodigal'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome.name)
     # no masking here becasuse we want to arbitrate with repeatmasker results
     if not context.TRANSLATION_TABLE:
         context.run_external(f'prodigal -p meta -m -f gff -q -i {fasta_file} -a {result_files[0]} -d {result_files[1]}')
     else:
         # prodigal should have taken care of the genetic code...
         if not genome.genetic_code:
-            raise(context.FatalException('No available genetic code for prodigal to predict protein-coding genes, aborting!'))
+            raise(Exception('No available genetic code for prodigal to predict protein-coding genes, aborting!'))
         context.run_external(
             f'prodigal -g {genome.genetic_code} -m -f gff -q -i {fasta_file} -a {result_files[0]} -d {result_files[1]}')
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     ORF_ID_PATTERN = re.compile(r'_(\d+?)$')
     nucl_seq_hash = {}
@@ -42,21 +43,21 @@
                 context.log(f'({genome.name}) Warning: Failed to find contig with "{seq_rec["id"]}"')
                 continue
             start = int(words[1].strip()) - 1
             end = int(words[2].strip())
 
             # reconciliation with repeats
             overlapping_features = [f for f in sqlite.read_all_features(db_connection, contig=contig_id,
-                                    start=start, end=end, type='rRNA tRNA tmRNA ncRNA CRISPR repeat_unit binding_site retrotransposon'.split())]
+                                                                        start=start, end=end, type='rRNA tRNA tmRNA ncRNA CRISPR repeat_unit binding_site retrotransposon'.split())]
 
             if len(overlapping_features):
                 overlap = 0
                 for f in overlapping_features:
                     overlap += min(f.end, end) - max(start, f.start)
-                non_repeat_features = [f for f in overlapping_features if f.type in 'rRNA tRNA tmRNA ncRNA CRISPR binding_site retrotransposon'.split()]
+                non_repeat_features = [f for f in overlapping_features if f.inference in 'rRNA tRNA tmRNA ncRNA CRISPR binding_site retrotransposon'.split()]
                 if len(non_repeat_features):
                     rejected_cds_count += 1
                     continue
                 elif overlap < 0.33 * (end-start):
                     for overlapping_feature in overlapping_features:
                         sqlite.drop_feature(db_connection, overlapping_feature)
                         dropped_repeat_count += 1
@@ -69,15 +70,15 @@
                 seq_rec['seq'] = seq_rec['seq'][:-1]
             feature = sqlite.Feature(genome = genome.name,
                        contig = contig_id,
                        start = start,
                        end = end,
                        strand = strand,
                        type = 'CDS',
-                       inference = 'prodigal',
+                       inference = ANNOTATOR_KEY,
                        aa_seq = seq_rec['seq'],
                        nt_seq = nucl_seq_hash[seq_rec['id']])
             if 'partial=01' in seq_rec['descr'] or 'partial=01' in seq_rec['descr'] or 'partial=11' in seq_rec['descr']:
                 feature.notes = 'partial protein'
             sqlite.add_new_feature_to_db(db_connection, feature)
             count += 1
 
@@ -85,13 +86,13 @@
                     f' rejected {rejected_cds_count} CDS during arbitration of prodigal results.')
         return count
 
 
 @context.register_annotator
 def run_and_read_prodigal():
     return ({'pipeline_position': 61,
-             'annotator_key': 'prodigal',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'coding sequence prediction with prodigal',
              'programs': ('prodigal',),
              'result_files': ('prodigal','prodigal-nucl'),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/pureseqtm.py` & `metaerg-2.5.5/src/metaerg/run_and_read/pureseqtm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 
 from metaerg import context
 from metaerg.datatypes import sqlite
 from metaerg.datatypes.fasta import FastaParser
 
+ANNOTATOR_KEY = 'pureseqtm'
+
 def _run_programs(genome, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome.name)
     context.run_external(f'PureseqTM_proteome.sh -i {cds_aa_file} -o {result_files[0]} -c {context.CPUS_PER_GENOME}')
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     count = 0
@@ -28,27 +30,30 @@
                     current_tmh = None
             if current_tmh:
                 current_tmh['end'] = len(orf['seq']) - 1
                 tmh_list.append(current_tmh)
             if len(tmh_list):
                 feature = sqlite.read_feature_by_id(db_connection, orf['id'])
                 if not feature:
-                    raise Exception(f'({genome.name}) Found pureseqtm result for unknown feature {orf["id"]}, '
+                    context.log(
+                        f'({genome.name}) FATAL ERROR: Found {ANNOTATOR_KEY} result for unknown feature {orf["id"]}, '
+                        f'may need to rerun metaerg with --force')
+                    raise Exception(f'({genome.name}) Found {ANNOTATOR_KEY} result for unknown feature {orf["id"]}, '
                                     f'may need to rerun metaerg with --force')
                 feature.tmh = len(tmh_list)
                 feature.tmh_topology = ','.join(f'{tmh["start"]}-{tmh["end"]}' for tmh in tmh_list)
                 sqlite.update_feature_in_db(db_connection, feature)
                 count += 1
     return count
 
 
 @context.register_annotator
 def run_and_read_pureseqtm():
     return ({'pipeline_position': 112,
-             'annotator_key': 'pureseqtm',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'transmembrane helix prediction with PureseqTM',
              'programs': ('PureseqTM_proteome.sh',),
              'result_files': ('pureseqtm',),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/repeat_masker.py` & `metaerg-2.5.5/src/metaerg/run_and_read/repeat_masker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import shutil
 from pathlib import Path
 
 from metaerg import context
 from metaerg.datatypes import fasta
 from metaerg.datatypes import sqlite
 
+ANNOTATOR_KEY = 'repeat_masker'
+
 def _run_programs(genome, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome.name)
     fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
     lmer_table_file = context.spawn_file('lmer-table', genome.name)
     repeatscout_file_raw = context.spawn_file('repeatscout-raw', genome.name)
     repeatscout_file_filtered = context.spawn_file('repeatscout-filtered', genome.name)
@@ -63,15 +65,15 @@
         seq = fasta.reverse_complement(seq)
     return sqlite.Feature(genome = genome_name,
                           contig = contig['id'],
                           start = start,
                           end = end,
                           strand = strand,
                           type = 'repeat_unit',
-                          inference = 'repeatmasker',
+                          inference = ANNOTATOR_KEY,
                           nt_seq = seq)
 
 
 def _read_results(genome, contig_dict, db_connection, result_files) -> int:
     """(1) simple repeats, these are consecutive
        (2) unspecified repeats, these occur scattered and are identified by an id in words[9]. We only
            add those when they occur 10 or more times."""
@@ -97,19 +99,20 @@
                 repeat_list.append(words2feature(words, contig, genome.name))
     for repeat_list in repeat_hash.values():
         if len(repeat_list) >= 10:
             for feature in repeat_list:
                 feature.notes = f' (occurs {len(repeat_list)}x)'
                 sqlite.add_new_feature_to_db(db_connection, feature)
                 count += 1
+    context.log(f'({genome.name}) {ANNOTATOR_KEY} results may appear different from a previous run, but some repeats may later be rejected based on prodigal predictions.')
     return count
 
 
 @context.register_annotator
 def run_and_read_repeatmasker():
     return ({'pipeline_position': 51,
-             'annotator_key': 'repeat_masker',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'repeat prediction with repeatmasker',
              'programs': ('build_lmer_table', 'RepeatScout', 'filter-stage-1.prl', 'RepeatMasker'),
              'result_files': ('repeatmasker',),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/signalp.py` & `metaerg-2.5.5/src/metaerg/run_and_read/signalp.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/tmhmm.py` & `metaerg-2.5.5/src/metaerg/run_and_read/tmhmm.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.4/src/metaerg/run_and_read/trf.py` & `metaerg-2.5.5/src/metaerg/run_and_read/trf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from metaerg import context
 from metaerg.datatypes import fasta
 from metaerg.datatypes import sqlite
 
+ANNOTATOR_KEY = 'trf'
 
 def _run_programs(genome, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome.name)
     fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome.name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
     with open(result_files[0], 'w') as output:
         context.run_external(f'trf {fasta_file} 2 7 7 80 10 50 500 -d -h -ngs', stdout=output)
@@ -28,23 +29,24 @@
             seq = contig['seq'][start:end]
             feature = sqlite.Feature(genome = genome.name,
                                      contig = contig['id'],
                                      start = start,
                                      end = end,
                                      strand = 1,
                                      type = 'repeat_unit',
-                                     inference = 'tandem-repeat-finder',
+                                     inference = ANNOTATOR_KEY,
                                      nt_seq = seq,
                                      notes = f'period size {words[2]}; copies {words[3]}')
             sqlite.add_new_feature_to_db(db_connection, feature)
             count += 1
+    context.log(f'({genome.name}) {ANNOTATOR_KEY} results may appear different from a previous run, but some repeats may later be rejected based on prodigal predictions.')
     return count
 
 @context.register_annotator
 def run_and_read_trf():
     return ({'pipeline_position': 41,
-             'annotator_key': 'trf',
+             'annotator_key': ANNOTATOR_KEY,
              'purpose': 'tandem repeat prediction with trf',
              'programs': ('trf',),
              'result_files': ('tandem-repeat-finder',),
              'run': _run_programs,
              'read': _read_results})
```

### Comparing `metaerg-2.5.4/src/metaerg.egg-info/PKG-INFO` & `metaerg-2.5.5/src/metaerg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaerg
-Version: 2.5.4
+Version: 2.5.5
 Summary: Annotation of genomes and contigs
 Home-page: https://github.com/kinestetika/MetaErg
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/MetaErg
 Keywords: repeat-regions genes functions taxonomy
@@ -30,15 +30,15 @@
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 
-## metaerg.py, version 2.5.4
+## metaerg.py, version 2.5.5
 
 Metaerg.py annotates genomes or sets of mags/bins from microbial ecosystems (bacteria, archaea, viruses). Input data 
 consists of nucleotide fasta files, one per genome or mag, each with one or more contigs. Output files with annotations 
 are in common formats such as .gff, .gbk, .fasta and .html with predicted genes, their functions and taxonomic 
 classifications.
 
 Metaerg 2.5 can annotate a group of related genomes and apply a suite of comparative genomics analyses. To do this, put
@@ -211,23 +211,27 @@
                         actually download and install the antismash database.
 
 ```
 
 ## Using the Docker Image
 Metaerg depends on many helper programs and may require some time and troubleshooting to install. To avoid these issues,
 use the [docker image](https://hub.docker.com/r/kinestetika/metaerg). Alternatively, use singularity or apptainer to run 
-the docker image on a HPC, as explained by [jkzorz](https://github.com/jkzorz/Metagenomes_Illumina/blob/main/annotation.md):
+the docker image on a HPC, as explained by [jkzorz](https://github.com/jkzorz/Metagenomes_Illumina/blob/main/annotation.md) and [lianchun yi]:
 
 ```commandline
 >singularity pull docker://kinestetika/metaerg
 >singularity build --sandbox /path/where/top/create/metaerg_latest.sif docker://kinestetika/metaerg:latest
->singularity run ~/metaerg_latest.sif
+>singularity exec --bind /path/to/metaerg_database:/databases --bind /path/to/fasta/files:/data --writable /path/to/the/sandbox/dir
+metaerg --database_dir /databases --contig_file /data --file_extension .fna
 ```
 
-Or:
+>[!NOTE]
+>The --bind instruction binds the dir "/path/to/metaerg_database" (which is on your real filesystem) to the dir "/databases" (which is inside your container). Same for the contig dir.
+
+Or, using apptainer:
 ```commandline
 >apptainer build metaerg.sif docker://kinestetika/metaerg:latest
 ```
 
 ## Installation
 
 To install metaerg, its 19 helper programs (diamond, prodigal, etc.) and databases run the following commands:
```

### Comparing `metaerg-2.5.4/src/metaerg.egg-info/SOURCES.txt` & `metaerg-2.5.5/src/metaerg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

