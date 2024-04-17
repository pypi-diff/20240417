# Comparing `tmp/C_MTEB-1.1.0.tar.gz` & `tmp/C_MTEB-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C_MTEB-1.1.0.tar", last modified: Thu Nov 30 08:18:11 2023, max compression
+gzip compressed data, was "C_MTEB-1.1.1.tar", last modified: Wed Apr 17 05:43:05 2024, max compression
```

## Comparing `C_MTEB-1.1.0.tar` & `C_MTEB-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 08:18:11.000000 C_MTEB-1.1.0/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 08:18:11.000000 C_MTEB-1.1.0/C_MTEB/
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-09-15 10:08:07.000000 C_MTEB-1.1.0/C_MTEB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 08:18:11.000000 C_MTEB-1.1.0/C_MTEB/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-08-09 07:15:28.000000 C_MTEB-1.1.0/C_MTEB/tasks/Classification.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2023-08-09 07:15:28.000000 C_MTEB-1.1.0/C_MTEB/tasks/Clustering.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2023-08-09 07:15:28.000000 C_MTEB-1.1.0/C_MTEB/tasks/PairClassification.py
--rw-rw-rw-   0 root         (0) root         (0)     8773 2023-09-15 10:08:07.000000 C_MTEB-1.1.0/C_MTEB/tasks/Reranking.py
--rw-rw-rw-   0 root         (0) root         (0)     7649 2023-09-12 12:00:08.000000 C_MTEB-1.1.0/C_MTEB/tasks/Retrieval.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-08-09 07:15:28.000000 C_MTEB-1.1.0/C_MTEB/tasks/STS.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-09-12 12:00:08.000000 C_MTEB-1.1.0/C_MTEB/tasks/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 08:18:11.000000 C_MTEB-1.1.0/C_MTEB.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    23735 2023-11-30 08:18:10.000000 C_MTEB-1.1.0/C_MTEB.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-11-30 08:18:10.000000 C_MTEB-1.1.0/C_MTEB.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-11-30 08:18:10.000000 C_MTEB-1.1.0/C_MTEB.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-11-30 08:18:10.000000 C_MTEB-1.1.0/C_MTEB.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-11-30 08:18:10.000000 C_MTEB-1.1.0/C_MTEB.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    23735 2023-11-30 08:18:11.000000 C_MTEB-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    23490 2023-11-25 06:12:39.000000 C_MTEB-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-11-30 08:18:11.000000 C_MTEB-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-09-12 12:00:08.000000 C_MTEB-1.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB/
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-09-15 10:08:07.000000 C_MTEB-1.1.1/C_MTEB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-08-09 07:15:28.000000 C_MTEB-1.1.1/C_MTEB/tasks/Classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2023-08-09 07:15:28.000000 C_MTEB-1.1.1/C_MTEB/tasks/Clustering.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-02-19 03:56:00.000000 C_MTEB-1.1.1/C_MTEB/tasks/MultiLongDocRetrieval.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2023-08-09 07:15:28.000000 C_MTEB-1.1.1/C_MTEB/tasks/PairClassification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8773 2023-09-15 10:08:07.000000 C_MTEB-1.1.1/C_MTEB/tasks/Reranking.py
+-rw-rw-rw-   0 root         (0) root         (0)     7649 2023-09-12 12:00:08.000000 C_MTEB-1.1.1/C_MTEB/tasks/Retrieval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-08-09 07:15:28.000000 C_MTEB-1.1.1/C_MTEB/tasks/STS.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-09-12 12:00:08.000000 C_MTEB-1.1.1/C_MTEB/tasks/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    23735 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/C_MTEB.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    23735 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    23490 2024-01-23 08:48:12.000000 C_MTEB-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-17 05:43:05.000000 C_MTEB-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-04-17 05:43:02.000000 C_MTEB-1.1.1/setup.py
```

### Comparing `C_MTEB-1.1.0/C_MTEB/__init__.py` & `C_MTEB-1.1.1/C_MTEB/__init__.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB/tasks/Classification.py` & `C_MTEB-1.1.1/C_MTEB/tasks/Classification.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB/tasks/Clustering.py` & `C_MTEB-1.1.1/C_MTEB/tasks/Clustering.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB/tasks/PairClassification.py` & `C_MTEB-1.1.1/C_MTEB/tasks/PairClassification.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB/tasks/Reranking.py` & `C_MTEB-1.1.1/C_MTEB/tasks/Reranking.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB/tasks/Retrieval.py` & `C_MTEB-1.1.1/C_MTEB/tasks/Retrieval.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB/tasks/STS.py` & `C_MTEB-1.1.1/C_MTEB/tasks/STS.py`

 * *Files identical despite different names*

### Comparing `C_MTEB-1.1.0/C_MTEB.egg-info/PKG-INFO` & `C_MTEB-1.1.1/C_MTEB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: C-MTEB
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chinese Massive Text Embedding Benchmark
 Home-page: https://github.com/FlagOpen/FlagEmbedding/tree/master/C_MTEB
 Author-email: 2906698981@qq.com
 Description-Content-Type: text/markdown
 
 <h1 align="center">Chinese Massive Text Embedding Benchmark</h1>
 <p align="center">
@@ -265,15 +265,15 @@
 | [DuRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/DuRetrieval](https://huggingface.co/datasets/C-MTEB/DuRetrieval) | A Large-scale Chinese Benchmark for Passage Retrieval from Web Search Engine | Retrieval | s2p | 4,000 |
 | [CovidRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/CovidRetrieval](https://huggingface.co/datasets/C-MTEB/CovidRetrieval) | COVID-19 news articles | Retrieval | s2p | 949  |
 | [CmedqaRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/CmedqaRetrieval](https://huggingface.co/datasets/C-MTEB/CmedqaRetrieval) |  Online medical consultation text | Retrieval | s2p | 3,999 | 
 | [EcomRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/EcomRetrieval](https://huggingface.co/datasets/C-MTEB/EcomRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in e-commerce domain | Retrieval | s2p | 1,000 |  
 | [MedicalRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/MedicalRetrieval](https://huggingface.co/datasets/C-MTEB/MedicalRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in medical domain | Retrieval | s2p | 1,000  |
 | [VideoRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/VideoRetrieval](https://huggingface.co/datasets/C-MTEB/VideoRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in video domain | Retrieval | s2p | 1,000  |
 | [T2Reranking](https://arxiv.org/abs/2304.03679) | [C-MTEB/T2Reranking](https://huggingface.co/datasets/C-MTEB/T2Reranking) | T2Ranking: A large-scale Chinese Benchmark for Passage Ranking | Reranking | s2p | 24,382 | 
-| [MMarcoRetrieval](https://github.com/unicamp-dl/mMARCO) | [C-MTEB/MMarco-reranking](https://huggingface.co/datasets/C-MTEB/Mmarco-reranking) | mMARCO is a multilingual version of the MS MARCO passage ranking dataset | Reranking | s2p | 7,437 | 
+| [MMarcoReranking](https://github.com/unicamp-dl/mMARCO) | [C-MTEB/MMarco-reranking](https://huggingface.co/datasets/C-MTEB/Mmarco-reranking) | mMARCO is a multilingual version of the MS MARCO passage ranking dataset | Reranking | s2p | 7,437 | 
 | [CMedQAv1](https://github.com/zhangsheng93/cMedQA) | [C-MTEB/CMedQAv1-reranking](https://huggingface.co/datasets/C-MTEB/CMedQAv1-reranking) | Chinese community medical question answering | Reranking | s2p |  2,000  |
 | [CMedQAv2](https://github.com/zhangsheng93/cMedQA2) | [C-MTEB/CMedQAv2-reranking](https://huggingface.co/datasets/C-MTEB/C-MTEB/CMedQAv2-reranking) | Chinese community medical question answering | Reranking | s2p |  4,000  |
 | [Ocnli](https://arxiv.org/abs/2010.05444) | [C-MTEB/OCNLI](https://huggingface.co/datasets/C-MTEB/OCNLI) | Original Chinese Natural Language Inference dataset | PairClassification | s2s |  3,000  |
 | [Cmnli](https://huggingface.co/datasets/clue/viewer/cmnli) | [C-MTEB/CMNLI](https://huggingface.co/datasets/C-MTEB/CMNLI) | Chinese Multi-Genre NLI | PairClassification | s2s | 139,000  |
 | [CLSClusteringS2S](https://arxiv.org/abs/2209.05034) | [C-MTEB/CLSClusteringS2S](https://huggingface.co/datasets/C-MTEB/C-MTEB/CLSClusteringS2S) | Clustering of titles from CLS dataset. Clustering of 13 sets, based on the main category. | Clustering | s2s |  10,000  |
 | [CLSClusteringP2P](https://arxiv.org/abs/2209.05034) | [C-MTEB/CLSClusteringP2P](https://huggingface.co/datasets/C-MTEB/CLSClusteringP2P) | Clustering of titles + abstract from CLS dataset. Clustering of 13 sets, based on the main category. | Clustering | p2p | 10,000   |
 | [ThuNewsClusteringS2S](http://thuctc.thunlp.org/) | [C-MTEB/ThuNewsClusteringS2S](https://huggingface.co/datasets/C-MTEB/ThuNewsClusteringS2S) | Clustering of titles from the THUCNews dataset | Clustering | s2s |  10,000  |
```

### Comparing `C_MTEB-1.1.0/PKG-INFO` & `C_MTEB-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: C_MTEB
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chinese Massive Text Embedding Benchmark
 Home-page: https://github.com/FlagOpen/FlagEmbedding/tree/master/C_MTEB
 Author-email: 2906698981@qq.com
 Description-Content-Type: text/markdown
 
 <h1 align="center">Chinese Massive Text Embedding Benchmark</h1>
 <p align="center">
@@ -265,15 +265,15 @@
 | [DuRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/DuRetrieval](https://huggingface.co/datasets/C-MTEB/DuRetrieval) | A Large-scale Chinese Benchmark for Passage Retrieval from Web Search Engine | Retrieval | s2p | 4,000 |
 | [CovidRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/CovidRetrieval](https://huggingface.co/datasets/C-MTEB/CovidRetrieval) | COVID-19 news articles | Retrieval | s2p | 949  |
 | [CmedqaRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/CmedqaRetrieval](https://huggingface.co/datasets/C-MTEB/CmedqaRetrieval) |  Online medical consultation text | Retrieval | s2p | 3,999 | 
 | [EcomRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/EcomRetrieval](https://huggingface.co/datasets/C-MTEB/EcomRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in e-commerce domain | Retrieval | s2p | 1,000 |  
 | [MedicalRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/MedicalRetrieval](https://huggingface.co/datasets/C-MTEB/MedicalRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in medical domain | Retrieval | s2p | 1,000  |
 | [VideoRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/VideoRetrieval](https://huggingface.co/datasets/C-MTEB/VideoRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in video domain | Retrieval | s2p | 1,000  |
 | [T2Reranking](https://arxiv.org/abs/2304.03679) | [C-MTEB/T2Reranking](https://huggingface.co/datasets/C-MTEB/T2Reranking) | T2Ranking: A large-scale Chinese Benchmark for Passage Ranking | Reranking | s2p | 24,382 | 
-| [MMarcoRetrieval](https://github.com/unicamp-dl/mMARCO) | [C-MTEB/MMarco-reranking](https://huggingface.co/datasets/C-MTEB/Mmarco-reranking) | mMARCO is a multilingual version of the MS MARCO passage ranking dataset | Reranking | s2p | 7,437 | 
+| [MMarcoReranking](https://github.com/unicamp-dl/mMARCO) | [C-MTEB/MMarco-reranking](https://huggingface.co/datasets/C-MTEB/Mmarco-reranking) | mMARCO is a multilingual version of the MS MARCO passage ranking dataset | Reranking | s2p | 7,437 | 
 | [CMedQAv1](https://github.com/zhangsheng93/cMedQA) | [C-MTEB/CMedQAv1-reranking](https://huggingface.co/datasets/C-MTEB/CMedQAv1-reranking) | Chinese community medical question answering | Reranking | s2p |  2,000  |
 | [CMedQAv2](https://github.com/zhangsheng93/cMedQA2) | [C-MTEB/CMedQAv2-reranking](https://huggingface.co/datasets/C-MTEB/C-MTEB/CMedQAv2-reranking) | Chinese community medical question answering | Reranking | s2p |  4,000  |
 | [Ocnli](https://arxiv.org/abs/2010.05444) | [C-MTEB/OCNLI](https://huggingface.co/datasets/C-MTEB/OCNLI) | Original Chinese Natural Language Inference dataset | PairClassification | s2s |  3,000  |
 | [Cmnli](https://huggingface.co/datasets/clue/viewer/cmnli) | [C-MTEB/CMNLI](https://huggingface.co/datasets/C-MTEB/CMNLI) | Chinese Multi-Genre NLI | PairClassification | s2s | 139,000  |
 | [CLSClusteringS2S](https://arxiv.org/abs/2209.05034) | [C-MTEB/CLSClusteringS2S](https://huggingface.co/datasets/C-MTEB/C-MTEB/CLSClusteringS2S) | Clustering of titles from CLS dataset. Clustering of 13 sets, based on the main category. | Clustering | s2s |  10,000  |
 | [CLSClusteringP2P](https://arxiv.org/abs/2209.05034) | [C-MTEB/CLSClusteringP2P](https://huggingface.co/datasets/C-MTEB/CLSClusteringP2P) | Clustering of titles + abstract from CLS dataset. Clustering of 13 sets, based on the main category. | Clustering | p2p | 10,000   |
 | [ThuNewsClusteringS2S](http://thuctc.thunlp.org/) | [C-MTEB/ThuNewsClusteringS2S](https://huggingface.co/datasets/C-MTEB/ThuNewsClusteringS2S) | Clustering of titles from the THUCNews dataset | Clustering | s2s |  10,000  |
```

### Comparing `C_MTEB-1.1.0/README.md` & `C_MTEB-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 | [DuRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/DuRetrieval](https://huggingface.co/datasets/C-MTEB/DuRetrieval) | A Large-scale Chinese Benchmark for Passage Retrieval from Web Search Engine | Retrieval | s2p | 4,000 |
 | [CovidRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/CovidRetrieval](https://huggingface.co/datasets/C-MTEB/CovidRetrieval) | COVID-19 news articles | Retrieval | s2p | 949  |
 | [CmedqaRetrieval](https://aclanthology.org/2022.emnlp-main.357.pdf) | [C-MTEB/CmedqaRetrieval](https://huggingface.co/datasets/C-MTEB/CmedqaRetrieval) |  Online medical consultation text | Retrieval | s2p | 3,999 | 
 | [EcomRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/EcomRetrieval](https://huggingface.co/datasets/C-MTEB/EcomRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in e-commerce domain | Retrieval | s2p | 1,000 |  
 | [MedicalRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/MedicalRetrieval](https://huggingface.co/datasets/C-MTEB/MedicalRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in medical domain | Retrieval | s2p | 1,000  |
 | [VideoRetrieval](https://arxiv.org/abs/2203.03367) | [C-MTEB/VideoRetrieval](https://huggingface.co/datasets/C-MTEB/VideoRetrieval) | Passage retrieval dataset collected from Alibaba search engine systems in video domain | Retrieval | s2p | 1,000  |
 | [T2Reranking](https://arxiv.org/abs/2304.03679) | [C-MTEB/T2Reranking](https://huggingface.co/datasets/C-MTEB/T2Reranking) | T2Ranking: A large-scale Chinese Benchmark for Passage Ranking | Reranking | s2p | 24,382 | 
-| [MMarcoRetrieval](https://github.com/unicamp-dl/mMARCO) | [C-MTEB/MMarco-reranking](https://huggingface.co/datasets/C-MTEB/Mmarco-reranking) | mMARCO is a multilingual version of the MS MARCO passage ranking dataset | Reranking | s2p | 7,437 | 
+| [MMarcoReranking](https://github.com/unicamp-dl/mMARCO) | [C-MTEB/MMarco-reranking](https://huggingface.co/datasets/C-MTEB/Mmarco-reranking) | mMARCO is a multilingual version of the MS MARCO passage ranking dataset | Reranking | s2p | 7,437 | 
 | [CMedQAv1](https://github.com/zhangsheng93/cMedQA) | [C-MTEB/CMedQAv1-reranking](https://huggingface.co/datasets/C-MTEB/CMedQAv1-reranking) | Chinese community medical question answering | Reranking | s2p |  2,000  |
 | [CMedQAv2](https://github.com/zhangsheng93/cMedQA2) | [C-MTEB/CMedQAv2-reranking](https://huggingface.co/datasets/C-MTEB/C-MTEB/CMedQAv2-reranking) | Chinese community medical question answering | Reranking | s2p |  4,000  |
 | [Ocnli](https://arxiv.org/abs/2010.05444) | [C-MTEB/OCNLI](https://huggingface.co/datasets/C-MTEB/OCNLI) | Original Chinese Natural Language Inference dataset | PairClassification | s2s |  3,000  |
 | [Cmnli](https://huggingface.co/datasets/clue/viewer/cmnli) | [C-MTEB/CMNLI](https://huggingface.co/datasets/C-MTEB/CMNLI) | Chinese Multi-Genre NLI | PairClassification | s2s | 139,000  |
 | [CLSClusteringS2S](https://arxiv.org/abs/2209.05034) | [C-MTEB/CLSClusteringS2S](https://huggingface.co/datasets/C-MTEB/C-MTEB/CLSClusteringS2S) | Clustering of titles from CLS dataset. Clustering of 13 sets, based on the main category. | Clustering | s2s |  10,000  |
 | [CLSClusteringP2P](https://arxiv.org/abs/2209.05034) | [C-MTEB/CLSClusteringP2P](https://huggingface.co/datasets/C-MTEB/CLSClusteringP2P) | Clustering of titles + abstract from CLS dataset. Clustering of 13 sets, based on the main category. | Clustering | p2p | 10,000   |
 | [ThuNewsClusteringS2S](http://thuctc.thunlp.org/) | [C-MTEB/ThuNewsClusteringS2S](https://huggingface.co/datasets/C-MTEB/ThuNewsClusteringS2S) | Clustering of titles from the THUCNews dataset | Clustering | s2s |  10,000  |
```

### Comparing `C_MTEB-1.1.0/setup.py` & `C_MTEB-1.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", mode="r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name='C_MTEB',
-    version='1.1.0',
+    version='1.1.1',
     description='Chinese Massive Text Embedding Benchmark',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='2906698981@qq.com',
     url='https://github.com/FlagOpen/FlagEmbedding/tree/master/C_MTEB',
     packages=find_packages(),
     install_requires=[
-        'mteb[beir]',
+        'mteb[beir]==1.1.1',
     ],
 )
```

