# Comparing `tmp/sentence-transformers-2.6.1.tar.gz` & `tmp/sentence_transformers-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentence-transformers-2.6.1.tar", last modified: Tue Mar 26 08:46:52 2024, max compression
+gzip compressed data, was "sentence_transformers-2.7.0.tar", last modified: Wed Apr 17 13:02:04 2024, max compression
```

## Comparing `sentence-transformers-2.6.1.tar` & `sentence_transformers-2.7.0.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:52.024392 sentence-transformers-2.6.1/
--rw-rw-rw-   0        0        0    11539 2023-12-18 14:58:04.000000 sentence-transformers-2.6.1/LICENSE
--rw-rw-rw-   0        0        0      254 2023-11-02 08:48:25.000000 sentence-transformers-2.6.1/NOTICE.txt
--rw-rw-rw-   0        0        0    11398 2024-03-26 08:46:52.024392 sentence-transformers-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    10374 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:51.952615 sentence-transformers-2.6.1/sentence_transformers/
--rw-rw-rw-   0        0        0     1824 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/LoggingHandler.py
--rw-rw-rw-   0        0        0    62317 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/SentenceTransformer.py
--rw-rw-rw-   0        0        0      574 2024-03-26 08:39:52.000000 sentence-transformers-2.6.1/sentence_transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:51.967127 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/
--rw-rw-rw-   0        0        0    22408 2024-03-25 08:00:20.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/CrossEncoder.py
--rw-rw-rw-   0        0        0       70 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:51.971638 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/
--rw-rw-rw-   0        0        0     2751 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CEBinaryAccuracyEvaluator.py
--rw-rw-rw-   0        0        0     3911 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CEBinaryClassificationEvaluator.py
--rw-rw-rw-   0        0        0     2586 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CECorrelationEvaluator.py
--rw-rw-rw-   0        0        0     4576 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CEF1Evaluator.py
--rw-rw-rw-   0        0        0     4564 2024-02-22 09:04:01.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CERerankingEvaluator.py
--rw-rw-rw-   0        0        0     2470 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CESoftmaxAccuracyEvaluator.py
--rw-rw-rw-   0        0        0      579 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:51.975637 sentence-transformers-2.6.1/sentence_transformers/datasets/
--rw-rw-rw-   0        0        0     1746 2024-02-22 09:04:01.000000 sentence-transformers-2.6.1/sentence_transformers/datasets/DenoisingAutoEncoderDataset.py
--rw-rw-rw-   0        0        0     1561 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/datasets/NoDuplicatesDataLoader.py
--rw-rw-rw-   0        0        0     7331 2024-02-07 11:32:26.000000 sentence-transformers-2.6.1/sentence_transformers/datasets/ParallelSentencesDataset.py
--rw-rw-rw-   0        0        0     4169 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/datasets/SentenceLabelDataset.py
--rw-rw-rw-   0        0        0      687 2024-02-07 11:32:26.000000 sentence-transformers-2.6.1/sentence_transformers/datasets/SentencesDataset.py
--rw-rw-rw-   0        0        0      470 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:51.985149 sentence-transformers-2.6.1/sentence_transformers/evaluation/
--rw-rw-rw-   0        0        0    10566 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/BinaryClassificationEvaluator.py
--rw-rw-rw-   0        0        0     8341 2024-03-26 08:39:10.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/EmbeddingSimilarityEvaluator.py
--rw-rw-rw-   0        0        0    13958 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/InformationRetrievalEvaluator.py
--rw-rw-rw-   0        0        0     2927 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/LabelAccuracyEvaluator.py
--rw-rw-rw-   0        0        0     3232 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/MSEEvaluator.py
--rw-rw-rw-   0        0        0     4046 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/MSEEvaluatorFromDataFrame.py
--rw-rw-rw-   0        0        0     8833 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/ParaphraseMiningEvaluator.py
--rw-rw-rw-   0        0        0     9284 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/RerankingEvaluator.py
--rw-rw-rw-   0        0        0     1111 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/SentenceEvaluator.py
--rw-rw-rw-   0        0        0      877 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/SequentialEvaluator.py
--rw-rw-rw-   0        0        0      135 2024-02-28 16:17:24.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/SimilarityFunction.py
--rw-rw-rw-   0        0        0     4869 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/TranslationEvaluator.py
--rw-rw-rw-   0        0        0     6584 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/TripletEvaluator.py
--rw-rw-rw-   0        0        0     1177 2024-02-28 16:17:24.000000 sentence-transformers-2.6.1/sentence_transformers/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:51.999774 sentence-transformers-2.6.1/sentence_transformers/losses/
--rw-rw-rw-   0        0        0    11065 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/losses/AdaptiveLayerLoss.py
--rw-rw-rw-   0        0        0     3059 2024-02-22 09:04:02.000000 sentence-transformers-2.6.1/sentence_transformers/losses/AnglELoss.py
--rw-rw-rw-   0        0        0     6110 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/losses/BatchAllTripletLoss.py
--rw-rw-rw-   0        0        0     6664 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/BatchHardSoftMarginTripletLoss.py
--rw-rw-rw-   0        0        0    11614 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/BatchHardTripletLoss.py
--rw-rw-rw-   0        0        0     7836 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/BatchSemiHardTripletLoss.py
--rw-rw-rw-   0        0        0    12020 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/losses/CachedMultipleNegativesRankingLoss.py
--rw-rw-rw-   0        0        0     4250 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/losses/CoSENTLoss.py
--rw-rw-rw-   0        0        0     4463 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/ContrastiveLoss.py
--rw-rw-rw-   0        0        0    10205 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/ContrastiveTensionLoss.py
--rw-rw-rw-   0        0        0     3558 2024-03-26 08:39:10.000000 sentence-transformers-2.6.1/sentence_transformers/losses/CosineSimilarityLoss.py
--rw-rw-rw-   0        0        0     8827 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/DenoisingAutoEncoderLoss.py
--rw-rw-rw-   0        0        0     7099 2024-03-25 08:00:20.000000 sentence-transformers-2.6.1/sentence_transformers/losses/GISTEmbedLoss.py
--rw-rw-rw-   0        0        0     3166 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/MSELoss.py
--rw-rw-rw-   0        0        0     4685 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/MarginMSELoss.py
--rw-rw-rw-   0        0        0     6014 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/losses/Matryoshka2dLoss.py
--rw-rw-rw-   0        0        0     5983 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/losses/MatryoshkaLoss.py
--rw-rw-rw-   0        0        0     6931 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/MegaBatchMarginLoss.py
--rw-rw-rw-   0        0        0     5463 2024-03-25 13:33:24.000000 sentence-transformers-2.6.1/sentence_transformers/losses/MultipleNegativesRankingLoss.py
--rw-rw-rw-   0        0        0     3853 2024-03-01 17:43:45.000000 sentence-transformers-2.6.1/sentence_transformers/losses/MultipleNegativesSymmetricRankingLoss.py
--rw-rw-rw-   0        0        0     3899 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/OnlineContrastiveLoss.py
--rw-rw-rw-   0        0        0     5417 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/SoftmaxLoss.py
--rw-rw-rw-   0        0        0     4027 2024-02-16 15:44:44.000000 sentence-transformers-2.6.1/sentence_transformers/losses/TripletLoss.py
--rw-rw-rw-   0        0        0     2279 2024-03-25 13:33:24.000000 sentence-transformers-2.6.1/sentence_transformers/losses/__init__.py
--rw-rw-rw-   0        0        0     5839 2024-03-14 09:11:07.000000 sentence-transformers-2.6.1/sentence_transformers/model_card_templates.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:52.009282 sentence-transformers-2.6.1/sentence_transformers/models/
--rw-rw-rw-   0        0        0     5672 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/Asym.py
--rw-rw-rw-   0        0        0     3376 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/models/BoW.py
--rw-rw-rw-   0        0        0     2826 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/models/CLIPModel.py
--rw-rw-rw-   0        0        0     2622 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/CNN.py
--rw-rw-rw-   0        0        0     2812 2024-02-20 09:08:59.000000 sentence-transformers-2.6.1/sentence_transformers/models/Dense.py
--rw-rw-rw-   0        0        0      958 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/Dropout.py
--rw-rw-rw-   0        0        0     2565 2024-02-06 21:29:21.000000 sentence-transformers-2.6.1/sentence_transformers/models/LSTM.py
--rw-rw-rw-   0        0        0     1187 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/LayerNorm.py
--rw-rw-rw-   0        0        0      592 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/Normalize.py
--rw-rw-rw-   0        0        0    10679 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/sentence_transformers/models/Pooling.py
--rw-rw-rw-   0        0        0     7902 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/models/Transformer.py
--rw-rw-rw-   0        0        0     2364 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/WeightedLayerPooling.py
--rw-rw-rw-   0        0        0     6349 2024-02-06 20:48:06.000000 sentence-transformers-2.6.1/sentence_transformers/models/WordEmbeddings.py
--rw-rw-rw-   0        0        0     3159 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/WordWeights.py
--rw-rw-rw-   0        0        0      716 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:52.011281 sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/
--rw-rw-rw-   0        0        0     4676 2024-02-22 09:04:02.000000 sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/PhraseTokenizer.py
--rw-rw-rw-   0        0        0     2435 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/WhitespaceTokenizer.py
--rw-rw-rw-   0        0        0     5779 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/WordTokenizer.py
--rw-rw-rw-   0        0        0      257 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/__init__.py
--rw-rw-rw-   0        0        0    19575 2024-03-26 08:39:10.000000 sentence-transformers-2.6.1/sentence_transformers/quantization.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:52.017282 sentence-transformers-2.6.1/sentence_transformers/readers/
--rw-rw-rw-   0        0        0      734 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/InputExample.py
--rw-rw-rw-   0        0        0     1286 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/LabelSentenceReader.py
--rw-rw-rw-   0        0        0     1676 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/NLIDataReader.py
--rw-rw-rw-   0        0        0     1127 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/PairedFilesReader.py
--rw-rw-rw-   0        0        0     3015 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/STSDataReader.py
--rw-rw-rw-   0        0        0     1443 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/TripletReader.py
--rw-rw-rw-   0        0        0      408 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/sentence_transformers/readers/__init__.py
--rw-rw-rw-   0        0        0    23569 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/sentence_transformers/util.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:52.023391 sentence-transformers-2.6.1/sentence_transformers.egg-info/
--rw-rw-rw-   0        0        0    11398 2024-03-26 08:46:51.000000 sentence-transformers-2.6.1/sentence_transformers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4923 2024-03-26 08:46:51.000000 sentence-transformers-2.6.1/sentence_transformers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 08:46:51.000000 sentence-transformers-2.6.1/sentence_transformers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-03-26 08:46:51.000000 sentence-transformers-2.6.1/sentence_transformers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-26 08:46:51.000000 sentence-transformers-2.6.1/sentence_transformers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-26 08:46:52.028757 sentence-transformers-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1265 2024-03-26 08:39:57.000000 sentence-transformers-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:52.023391 sentence-transformers-2.6.1/tests/
--rw-rw-rw-   0        0        0     4890 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/tests/test_cmnrl.py
--rw-rw-rw-   0        0        0     2739 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/tests/test_compute_embeddings.py
--rw-rw-rw-   0        0        0     7173 2024-03-25 08:00:20.000000 sentence-transformers-2.6.1/tests/test_cross_encoder.py
--rw-rw-rw-   0        0        0     3559 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/tests/test_evaluator.py
--rw-rw-rw-   0        0        0      869 2024-02-06 19:44:26.000000 sentence-transformers-2.6.1/tests/test_image_embeddings.py
--rw-rw-rw-   0        0        0     1496 2024-03-05 11:03:58.000000 sentence-transformers-2.6.1/tests/test_multi_process.py
--rw-rw-rw-   0        0        0     6459 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/tests/test_pretrained_stsb.py
--rw-rw-rw-   0        0        0    18351 2024-03-25 08:00:20.000000 sentence-transformers-2.6.1/tests/test_sentence_transformer.py
--rw-rw-rw-   0        0        0     6183 2024-03-25 13:33:27.000000 sentence-transformers-2.6.1/tests/test_train_stsb.py
--rw-rw-rw-   0        0        0     2884 2024-02-28 16:17:24.000000 sentence-transformers-2.6.1/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.265893 sentence_transformers-2.7.0/
+-rw-rw-rw-   0        0        0    11539 2023-12-18 14:58:04.000000 sentence_transformers-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0      254 2023-11-02 08:48:25.000000 sentence_transformers-2.7.0/NOTICE.txt
+-rw-rw-rw-   0        0        0    11774 2024-04-17 13:02:04.264893 sentence_transformers-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10603 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.190832 sentence_transformers-2.7.0/sentence_transformers/
+-rw-rw-rw-   0        0        0     1824 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/LoggingHandler.py
+-rw-rw-rw-   0        0        0    65209 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/SentenceTransformer.py
+-rw-rw-rw-   0        0        0      574 2024-04-17 11:45:09.000000 sentence_transformers-2.7.0/sentence_transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.211358 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/
+-rw-rw-rw-   0        0        0    23894 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/CrossEncoder.py
+-rw-rw-rw-   0        0        0       70 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.216865 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/
+-rw-rw-rw-   0        0        0     2751 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CEBinaryAccuracyEvaluator.py
+-rw-rw-rw-   0        0        0     3911 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CEBinaryClassificationEvaluator.py
+-rw-rw-rw-   0        0        0     2586 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CECorrelationEvaluator.py
+-rw-rw-rw-   0        0        0     4576 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CEF1Evaluator.py
+-rw-rw-rw-   0        0        0     4564 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CERerankingEvaluator.py
+-rw-rw-rw-   0        0        0     2470 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CESoftmaxAccuracyEvaluator.py
+-rw-rw-rw-   0        0        0      579 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.220867 sentence_transformers-2.7.0/sentence_transformers/datasets/
+-rw-rw-rw-   0        0        0     1746 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/datasets/DenoisingAutoEncoderDataset.py
+-rw-rw-rw-   0        0        0     1561 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/datasets/NoDuplicatesDataLoader.py
+-rw-rw-rw-   0        0        0     7331 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/datasets/ParallelSentencesDataset.py
+-rw-rw-rw-   0        0        0     4169 2024-04-12 10:00:45.000000 sentence_transformers-2.7.0/sentence_transformers/datasets/SentenceLabelDataset.py
+-rw-rw-rw-   0        0        0      687 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/datasets/SentencesDataset.py
+-rw-rw-rw-   0        0        0      470 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.228372 sentence_transformers-2.7.0/sentence_transformers/evaluation/
+-rw-rw-rw-   0        0        0    11329 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/BinaryClassificationEvaluator.py
+-rw-rw-rw-   0        0        0     8972 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/EmbeddingSimilarityEvaluator.py
+-rw-rw-rw-   0        0        0    14685 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/InformationRetrievalEvaluator.py
+-rw-rw-rw-   0        0        0     3003 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/LabelAccuracyEvaluator.py
+-rw-rw-rw-   0        0        0     3984 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/MSEEvaluator.py
+-rw-rw-rw-   0        0        0     4811 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/MSEEvaluatorFromDataFrame.py
+-rw-rw-rw-   0        0        0     9540 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/ParaphraseMiningEvaluator.py
+-rw-rw-rw-   0        0        0    10735 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/RerankingEvaluator.py
+-rw-rw-rw-   0        0        0     1191 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/SentenceEvaluator.py
+-rw-rw-rw-   0        0        0      953 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/SequentialEvaluator.py
+-rw-rw-rw-   0        0        0      135 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/SimilarityFunction.py
+-rw-rw-rw-   0        0        0     5766 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/TranslationEvaluator.py
+-rw-rw-rw-   0        0        0     7351 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/TripletEvaluator.py
+-rw-rw-rw-   0        0        0     1177 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.243879 sentence_transformers-2.7.0/sentence_transformers/losses/
+-rw-rw-rw-   0        0        0    11065 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/AdaptiveLayerLoss.py
+-rw-rw-rw-   0        0        0     3059 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/AnglELoss.py
+-rw-rw-rw-   0        0        0     6110 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/BatchAllTripletLoss.py
+-rw-rw-rw-   0        0        0     6664 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/BatchHardSoftMarginTripletLoss.py
+-rw-rw-rw-   0        0        0    11614 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/BatchHardTripletLoss.py
+-rw-rw-rw-   0        0        0     7836 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/BatchSemiHardTripletLoss.py
+-rw-rw-rw-   0        0        0    15064 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/CachedGISTEmbedLoss.py
+-rw-rw-rw-   0        0        0    12020 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/CachedMultipleNegativesRankingLoss.py
+-rw-rw-rw-   0        0        0     4250 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/CoSENTLoss.py
+-rw-rw-rw-   0        0        0     4463 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/ContrastiveLoss.py
+-rw-rw-rw-   0        0        0    10205 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/ContrastiveTensionLoss.py
+-rw-rw-rw-   0        0        0     3558 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/CosineSimilarityLoss.py
+-rw-rw-rw-   0        0        0     8827 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/DenoisingAutoEncoderLoss.py
+-rw-rw-rw-   0        0        0     7099 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/GISTEmbedLoss.py
+-rw-rw-rw-   0        0        0     3166 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/MSELoss.py
+-rw-rw-rw-   0        0        0     4685 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/MarginMSELoss.py
+-rw-rw-rw-   0        0        0     6014 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/Matryoshka2dLoss.py
+-rw-rw-rw-   0        0        0     6310 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/MatryoshkaLoss.py
+-rw-rw-rw-   0        0        0     6931 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/MegaBatchMarginLoss.py
+-rw-rw-rw-   0        0        0     5463 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/MultipleNegativesRankingLoss.py
+-rw-rw-rw-   0        0        0     3853 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/losses/MultipleNegativesSymmetricRankingLoss.py
+-rw-rw-rw-   0        0        0     3899 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/losses/OnlineContrastiveLoss.py
+-rw-rw-rw-   0        0        0     5417 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/SoftmaxLoss.py
+-rw-rw-rw-   0        0        0     4027 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/TripletLoss.py
+-rw-rw-rw-   0        0        0     2361 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/losses/__init__.py
+-rw-rw-rw-   0        0        0     5839 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/model_card_templates.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.252386 sentence_transformers-2.7.0/sentence_transformers/models/
+-rw-rw-rw-   0        0        0     5692 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/Asym.py
+-rw-rw-rw-   0        0        0     3396 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/models/BoW.py
+-rw-rw-rw-   0        0        0     3002 2024-04-17 11:44:02.000000 sentence_transformers-2.7.0/sentence_transformers/models/CLIPModel.py
+-rw-rw-rw-   0        0        0     2632 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/CNN.py
+-rw-rw-rw-   0        0        0     2812 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/Dense.py
+-rw-rw-rw-   0        0        0      958 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/Dropout.py
+-rw-rw-rw-   0        0        0     2575 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/LSTM.py
+-rw-rw-rw-   0        0        0     1187 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/LayerNorm.py
+-rw-rw-rw-   0        0        0      592 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/Normalize.py
+-rw-rw-rw-   0        0        0    10679 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/Pooling.py
+-rw-rw-rw-   0        0        0     7939 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/models/Transformer.py
+-rw-rw-rw-   0        0        0     2364 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/WeightedLayerPooling.py
+-rw-rw-rw-   0        0        0     6369 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/WordEmbeddings.py
+-rw-rw-rw-   0        0        0     3159 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/WordWeights.py
+-rw-rw-rw-   0        0        0      716 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.254386 sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/
+-rw-rw-rw-   0        0        0     4686 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/PhraseTokenizer.py
+-rw-rw-rw-   0        0        0     2445 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/WhitespaceTokenizer.py
+-rw-rw-rw-   0        0        0     5789 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/WordTokenizer.py
+-rw-rw-rw-   0        0        0      257 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/__init__.py
+-rw-rw-rw-   0        0        0    19710 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/quantization.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.257892 sentence_transformers-2.7.0/sentence_transformers/readers/
+-rw-rw-rw-   0        0        0      734 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/InputExample.py
+-rw-rw-rw-   0        0        0     1286 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/LabelSentenceReader.py
+-rw-rw-rw-   0        0        0     1676 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/NLIDataReader.py
+-rw-rw-rw-   0        0        0     1127 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/PairedFilesReader.py
+-rw-rw-rw-   0        0        0     3015 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/STSDataReader.py
+-rw-rw-rw-   0        0        0     1443 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/TripletReader.py
+-rw-rw-rw-   0        0        0      408 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/sentence_transformers/readers/__init__.py
+-rw-rw-rw-   0        0        0    24378 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/sentence_transformers/util.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.263893 sentence_transformers-2.7.0/sentence_transformers.egg-info/
+-rw-rw-rw-   0        0        0    11774 2024-04-17 13:02:04.000000 sentence_transformers-2.7.0/sentence_transformers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4975 2024-04-17 13:02:04.000000 sentence_transformers-2.7.0/sentence_transformers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:02:04.000000 sentence_transformers-2.7.0/sentence_transformers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-17 13:02:04.000000 sentence_transformers-2.7.0/sentence_transformers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-17 13:02:04.000000 sentence_transformers-2.7.0/sentence_transformers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-17 13:02:04.269973 sentence_transformers-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2024-04-17 11:45:09.000000 sentence_transformers-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:02:04.263893 sentence_transformers-2.7.0/tests/
+-rw-rw-rw-   0        0        0     4890 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_cmnrl.py
+-rw-rw-rw-   0        0        0     3001 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_compute_embeddings.py
+-rw-rw-rw-   0        0        0     7173 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_cross_encoder.py
+-rw-rw-rw-   0        0        0     3559 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      869 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_image_embeddings.py
+-rw-rw-rw-   0        0        0     1496 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_multi_process.py
+-rw-rw-rw-   0        0        0     6459 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/tests/test_pretrained_stsb.py
+-rw-rw-rw-   0        0        0    22906 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_sentence_transformer.py
+-rw-rw-rw-   0        0        0     6183 2024-04-17 11:20:12.000000 sentence_transformers-2.7.0/tests/test_train_stsb.py
+-rw-rw-rw-   0        0        0     2884 2024-04-11 13:54:17.000000 sentence_transformers-2.7.0/tests/test_util.py
```

### Comparing `sentence-transformers-2.6.1/LICENSE` & `sentence_transformers-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/PKG-INFO` & `sentence_transformers-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentence-transformers
-Version: 2.6.1
+Version: 2.7.0
 Summary: Multilingual text embeddings
 Home-page: https://www.SBERT.net
 Download-URL: https://github.com/UKPLab/sentence-transformers/
 Author: Nils Reimers
 Author-email: info@nils-reimers.de
 License: Apache License 2.0
 Keywords: Transformer Networks BERT XLNet sentence embedding PyTorch NLP deep learning
@@ -13,22 +13,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
-Requires-Dist: transformers<5.0.0,>=4.32.0
+Requires-Dist: transformers<5.0.0,>=4.34.0
 Requires-Dist: tqdm
 Requires-Dist: torch>=1.11.0
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: huggingface-hub>=0.15.1
 Requires-Dist: Pillow
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ruff>=0.3.0; extra == "dev"
 
 <!--- BADGES: START --->
 [![GitHub - License](https://img.shields.io/github/license/UKPLab/sentence-transformers?logo=github&style=flat&color=green)][#github-license]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sentence-transformers?logo=pypi&style=flat&color=blue)][#pypi-package]
 [![PyPI - Package Version](https://img.shields.io/pypi/v/sentence-transformers?logo=pypi&style=flat&color=orange)][#pypi-package]
 [![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/sentence-transformers?logo=anaconda&style=flat)][#conda-forge-package]
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/sentence-transformers?logo=anaconda&style=flat&color=orange)][#conda-forge-package]
@@ -169,14 +173,30 @@
  - [Text Summarization](https://www.sbert.net/examples/applications/text-summarization/README.html) 
 - [Multilingual Image Search, Clustering & Duplicate Detection](https://www.sbert.net/examples/applications/image-search/README.html)
 
 and many more use-cases.
 
 For all examples, see [examples/applications](https://github.com/UKPLab/sentence-transformers/tree/master/examples/applications).
 
+## Development setup
+
+After cloning the repo (or a fork) to your machine, in a virtual environment, run:
+
+```
+python -m pip install -e ".[dev]"
+
+pre-commit install
+```
+
+To test your changes, run:
+
+```
+pytest
+```
+
 ## Citing & Authors
 
 If you find this repository helpful, feel free to cite our publication [Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks](https://arxiv.org/abs/1908.10084):
 
 ```bibtex 
 @inproceedings{reimers-2019-sentence-bert,
     title = "Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks",
```

### Comparing `sentence-transformers-2.6.1/README.md` & `sentence_transformers-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,30 @@
  - [Text Summarization](https://www.sbert.net/examples/applications/text-summarization/README.html) 
 - [Multilingual Image Search, Clustering & Duplicate Detection](https://www.sbert.net/examples/applications/image-search/README.html)
 
 and many more use-cases.
 
 For all examples, see [examples/applications](https://github.com/UKPLab/sentence-transformers/tree/master/examples/applications).
 
+## Development setup
+
+After cloning the repo (or a fork) to your machine, in a virtual environment, run:
+
+```
+python -m pip install -e ".[dev]"
+
+pre-commit install
+```
+
+To test your changes, run:
+
+```
+pytest
+```
+
 ## Citing & Authors
 
 If you find this repository helpful, feel free to cite our publication [Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks](https://arxiv.org/abs/1908.10084):
 
 ```bibtex 
 @inproceedings{reimers-2019-sentence-bert,
     title = "Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks",
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/LoggingHandler.py` & `sentence_transformers-2.7.0/sentence_transformers/LoggingHandler.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/SentenceTransformer.py` & `sentence_transformers-2.7.0/sentence_transformers/SentenceTransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import contextmanager
 import json
 import logging
 import os
 import shutil
 from collections import OrderedDict
 import warnings
 from typing import List, Dict, Literal, Tuple, Iterable, Type, Union, Callable, Optional, TYPE_CHECKING
@@ -27,14 +28,15 @@
     batch_to_device,
     fullname,
     is_sentence_transformer_model,
     load_dir_path,
     load_file_path,
     save_to_hub_args_decorator,
     get_device_name,
+    truncate_embeddings,
 )
 from .quantization import quantize_embeddings
 from .models import Transformer, Pooling, Normalize
 from .model_card_templates import ModelCardTemplate
 from . import __version__
 
 logger = logging.getLogger(__name__)
@@ -58,38 +60,42 @@
     :param prompts: A dictionary with prompts for the model. The key is the prompt name, the value is the prompt text.
         The prompt text will be prepended before any text to encode. For example:
         `{"query": "query: ", "passage": "passage: "}` or `{"clustering": "Identify the main category based on the
         titles in "}`.
     :param default_prompt_name: The name of the prompt that should be used by default. If not set,
         no prompt will be applied.
     :param cache_folder: Path to store models. Can also be set by the SENTENCE_TRANSFORMERS_HOME environment variable.
-    :param revision: The specific model version to use. It can be a branch name, a tag name, or a commit id,
-        for a stored model on Hugging Face.
     :param trust_remote_code: Whether or not to allow for custom models defined on the Hub in their own modeling files.
         This option should only be set to True for repositories you trust and in which you have read the code, as it
         will execute code present on the Hub on your local machine.
+    :param revision: The specific model version to use. It can be a branch name, a tag name, or a commit id,
+        for a stored model on Hugging Face.
     :param token: Hugging Face authentication token to download private models.
+    :param truncate_dim: The dimension to truncate sentence embeddings to. `None` does no truncation. Truncation is
+        only applicable during inference when `.encode` is called.
     """
 
     def __init__(
         self,
         model_name_or_path: Optional[str] = None,
         modules: Optional[Iterable[nn.Module]] = None,
         device: Optional[str] = None,
         prompts: Optional[Dict[str, str]] = None,
         default_prompt_name: Optional[str] = None,
         cache_folder: Optional[str] = None,
         trust_remote_code: bool = False,
         revision: Optional[str] = None,
         token: Optional[Union[bool, str]] = None,
         use_auth_token: Optional[Union[bool, str]] = None,
+        truncate_dim: Optional[int] = None,
     ):
         # Note: self._load_sbert_model can also update `self.prompts` and `self.default_prompt_name`
         self.prompts = prompts or {}
         self.default_prompt_name = default_prompt_name
+        self.truncate_dim = truncate_dim
         self._model_card_vars = {}
         self._model_card_text = None
         self._model_config = {}
         if use_auth_token is not None:
             warnings.warn(
                 "The `use_auth_token` argument is deprecated and will be removed in v3 of SentenceTransformers.",
                 FutureWarning,
@@ -209,14 +215,15 @@
 
         super().__init__(modules)
         if device is None:
             device = get_device_name()
             logger.info("Use pytorch device_name: {}".format(device))
 
         self.to(device)
+        self.is_hpu_graph_enabled = False
 
         if self.default_prompt_name is not None and self.default_prompt_name not in self.prompts:
             raise ValueError(
                 f"Default prompt name '{self.default_prompt_name}' not found in the configured prompts "
                 f"dictionary with keys {list(self.prompts.keys())!r}."
             )
 
@@ -249,15 +256,15 @@
     def encode(
         self,
         sentences: Union[str, List[str]],
         prompt_name: Optional[str] = None,
         prompt: Optional[str] = None,
         batch_size: int = 32,
         show_progress_bar: bool = None,
-        output_value: str = "sentence_embedding",
+        output_value: Optional[Literal["sentence_embedding", "token_embeddings"]] = "sentence_embedding",
         precision: Literal["float32", "int8", "uint8", "binary", "ubinary"] = "float32",
         convert_to_numpy: bool = True,
         convert_to_tensor: bool = False,
         device: str = None,
         normalize_embeddings: bool = False,
     ) -> Union[List[Tensor], ndarray, Tensor]:
         """
@@ -285,16 +292,23 @@
         :param convert_to_tensor: Whether the output should be one large tensor. Overwrites `convert_to_numpy`.
         :param device: Which `torch.device` to use for the computation.
         :param normalize_embeddings: Whether to normalize returned vectors to have length 1. In that case,
             the faster dot-product (util.dot_score) instead of cosine similarity can be used.
 
         :return: By default, a 2d numpy array with shape [num_inputs, output_dimension] is returned. If only one string
             input is provided, then the output is a 1d array with shape [output_dimension]. If `convert_to_tensor`, a
-            torch Tensor is returned instead.
+            torch Tensor is returned instead. If `self.truncate_dim <= output_dimension` then output_dimension is
+            `self.truncate_dim`.
         """
+        if self.device.type == "hpu" and not self.is_hpu_graph_enabled:
+            import habana_frameworks.torch as ht
+
+            ht.hpu.wrap_in_hpu_graph(self, disable_tensor_cache=True)
+            self.is_hpu_graph_enabled = True
+
         self.eval()
         if show_progress_bar is None:
             show_progress_bar = (
                 logger.getEffectiveLevel() == logging.INFO or logger.getEffectiveLevel() == logging.DEBUG
             )
 
         if convert_to_tensor:
@@ -351,14 +365,17 @@
             sentences_batch = sentences_sorted[start_index : start_index + batch_size]
             features = self.tokenize(sentences_batch)
             features = batch_to_device(features, device)
             features.update(extra_features)
 
             with torch.no_grad():
                 out_features = self.forward(features)
+                out_features["sentence_embedding"] = truncate_embeddings(
+                    out_features["sentence_embedding"], self.truncate_dim
+                )
 
                 if output_value == "token_embeddings":
                     embeddings = []
                     for token_emb, attention in zip(out_features[output_value], out_features["attention_mask"]):
                         last_mask_id = len(attention) - 1
                         while last_mask_id > 0 and attention[last_mask_id].item() == 0:
                             last_mask_id -= 1
@@ -562,25 +579,71 @@
 
         return None
 
     def tokenize(self, texts: Union[List[str], List[Dict], List[Tuple[str, str]]]):
         """
         Tokenizes the texts
         """
-        return self._first_module().tokenize(texts)
+        kwargs = {}
+        # HPU models reach optimal performance if the padding is not dynamic
+        if self.device.type == "hpu":
+            kwargs["padding"] = "max_length"
+
+        try:
+            return self._first_module().tokenize(texts, **kwargs)
+        except TypeError:
+            # In case some Module does not allow for kwargs in tokenize, we also try without any
+            return self._first_module().tokenize(texts)
 
     def get_sentence_features(self, *features):
         return self._first_module().get_sentence_features(*features)
 
-    def get_sentence_embedding_dimension(self):
+    def get_sentence_embedding_dimension(self) -> Optional[int]:
+        """
+        :return: The number of dimensions in the output of `encode`. If it's not known, it's `None`.
+        """
+        output_dim = None
         for mod in reversed(self._modules.values()):
             sent_embedding_dim_method = getattr(mod, "get_sentence_embedding_dimension", None)
             if callable(sent_embedding_dim_method):
-                return sent_embedding_dim_method()
-        return None
+                output_dim = sent_embedding_dim_method()
+                break
+        if self.truncate_dim is not None:
+            # The user requested truncation. If they set it to a dim greater than output_dim,
+            # no truncation will actually happen. So return output_dim insead of self.truncate_dim
+            return min(output_dim or np.inf, self.truncate_dim)
+        return output_dim
+
+    @contextmanager
+    def truncate_sentence_embeddings(self, truncate_dim: Optional[int]):
+        """
+        In this context, `model.encode` outputs sentence embeddings truncated at dimension `truncate_dim`.
+
+        This may be useful when you are using the same model for different applications where different dimensions
+        are needed.
+
+        :param truncate_dim: The dimension to truncate sentence embeddings to. `None` does no truncation.
+
+        Example::
+
+            from sentence_transformers import SentenceTransformer
+
+            model = SentenceTransformer("model-name")
+
+            with model.truncate_sentence_embeddings(truncate_dim=16):
+                embeddings_truncated = model.encode(["hello there", "hiya"])
+            assert embeddings_truncated.shape[-1] == 16
+
+        """
+        original_output_dim = self.truncate_dim
+        try:
+            self.truncate_dim = truncate_dim
+            yield
+        finally:
+            self.truncate_dim = original_output_dim
 
     def _first_module(self):
         """Returns the first module of this sequential embedder"""
         return self._modules[next(iter(self._modules))]
 
     def _last_module(self):
         """Returns the last module of this sequential embedder"""
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/__init__.py` & `sentence_transformers-2.7.0/sentence_transformers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.6.1"
+__version__ = "2.7.0"
 __MODEL_HUB_ORGANIZATION__ = "sentence-transformers"
 from .datasets import SentencesDataset, ParallelSentencesDataset
 from .LoggingHandler import LoggingHandler
 from .SentenceTransformer import SentenceTransformer
 from .readers import InputExample
 from .cross_encoder.CrossEncoder import CrossEncoder
 from .quantization import quantize_embeddings
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/CrossEncoder.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/CrossEncoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+from functools import wraps
+
 from transformers import AutoModelForSequenceClassification, AutoTokenizer, AutoConfig
 import numpy as np
 import logging
 import os
 from typing import Dict, Type, Callable, List, Optional
 import torch
 from torch import nn
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 from tqdm.autonotebook import tqdm, trange
 from transformers import is_torch_npu_available
+from transformers.utils import PushToHubMixin
+
 from .. import SentenceTransformer, util
 from ..evaluation import SentenceEvaluator
 from ..util import get_device_name
 
 
 logger = logging.getLogger(__name__)
 
 
-class CrossEncoder:
+class CrossEncoder(PushToHubMixin):
     """
     A CrossEncoder takes exactly two sentences / texts as input and either predicts
     a score or label for this sentence pair. It can for example predict the similarity of the sentence pair
     on a scale of 0 ... 1.
 
     It does not yield a sentence embedding and does not work for individual sentences.
 
@@ -31,14 +35,17 @@
         outputs a continuous score 0...1. If > 1, it output several scores that can be soft-maxed to get
         probability scores for the different classes.
     :param max_length: Max length for input sequences. Longer sequences will be truncated. If None, max
         length of the model will be used
     :param device: Device that should be used for the model. If None, it will use CUDA if available.
     :param tokenizer_args: Arguments passed to AutoTokenizer
     :param automodel_args: Arguments passed to AutoModelForSequenceClassification
+    :param trust_remote_code: Whether or not to allow for custom models defined on the Hub in their own modeling files.
+        This option should only be set to True for repositories you trust and in which you have read the code, as it
+        will execute code present on the Hub on your local machine.
     :param revision: The specific model version to use. It can be a branch name, a tag name, or a commit id,
         for a stored model on Hugging Face.
     :param default_activation_function: Callable (like nn.Sigmoid) about the default activation function that
         should be used on-top of model.predict(). If None. nn.Sigmoid() will be used if num_labels=1,
         else nn.Identity()
     :param classifier_dropout: The dropout ratio for the classification head.
     """
@@ -47,36 +54,36 @@
         self,
         model_name: str,
         num_labels: int = None,
         max_length: int = None,
         device: str = None,
         tokenizer_args: Dict = {},
         automodel_args: Dict = {},
+        trust_remote_code: bool = False,
         revision: Optional[str] = None,
         default_activation_function=None,
         classifier_dropout: float = None,
     ):
-        self.config = AutoConfig.from_pretrained(model_name, revision=revision)
+        self.config = AutoConfig.from_pretrained(model_name, trust_remote_code=trust_remote_code, revision=revision)
         classifier_trained = True
         if self.config.architectures is not None:
             classifier_trained = any(
                 [arch.endswith("ForSequenceClassification") for arch in self.config.architectures]
             )
 
         if classifier_dropout is not None:
             self.config.classifier_dropout = classifier_dropout
 
         if num_labels is None and not classifier_trained:
             num_labels = 1
 
         if num_labels is not None:
             self.config.num_labels = num_labels
-
         self.model = AutoModelForSequenceClassification.from_pretrained(
-            model_name, config=self.config, revision=revision, **automodel_args
+            model_name, config=self.config, revision=revision, trust_remote_code=trust_remote_code, **automodel_args
         )
         self.tokenizer = AutoTokenizer.from_pretrained(model_name, revision=revision, **tokenizer_args)
         self.max_length = max_length
 
         if device is None:
             device = get_device_name()
             logger.info("Use pytorch device: {}".format(device))
@@ -444,23 +451,49 @@
             if callback is not None:
                 callback(score, epoch, steps)
             if score > self.best_score:
                 self.best_score = score
                 if save_best_model:
                     self.save(output_path)
 
-    def save(self, path: str, safe_serialization: bool = True) -> None:
+    def save(self, path: str, *, safe_serialization: bool = True, **kwargs) -> None:
         """
-        Saves all model and tokenizer to path
+        Saves the model and tokenizer to path; identical to `save_pretrained`
         """
         if path is None:
             return
 
         logger.info("Save model to {}".format(path))
-        self.model.save_pretrained(path, safe_serialization=safe_serialization)
-        self.tokenizer.save_pretrained(path)
+        self.model.save_pretrained(path, safe_serialization=safe_serialization, **kwargs)
+        self.tokenizer.save_pretrained(path, **kwargs)
 
-    def save_pretrained(self, path: str) -> None:
+    def save_pretrained(self, path: str, *, safe_serialization: bool = True, **kwargs) -> None:
         """
-        Same function as save
+        Saves the model and tokenizer to path; identical to `save`
         """
-        return self.save(path)
+        return self.save(path, safe_serialization=safe_serialization, **kwargs)
+
+    @wraps(PushToHubMixin.push_to_hub)
+    def push_to_hub(
+        self,
+        repo_id: str,
+        *,
+        commit_message: Optional[str] = None,
+        private: Optional[bool] = None,
+        safe_serialization: bool = True,
+        tags: Optional[List[str]] = None,
+        **kwargs,
+    ) -> str:
+        if isinstance(tags, str):
+            tags = [tags]
+        elif tags is None:
+            tags = []
+        if "cross-encoder" not in tags:
+            tags.insert(0, "cross-encoder")
+        return super().push_to_hub(
+            repo_id=repo_id,
+            safe_serialization=safe_serialization,
+            commit_message=commit_message,
+            private=private,
+            tags=tags,
+            **kwargs,
+        )
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CEBinaryAccuracyEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CEBinaryAccuracyEvaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CEBinaryClassificationEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CEBinaryClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CECorrelationEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CECorrelationEvaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CEF1Evaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CEF1Evaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CERerankingEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CERerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/CESoftmaxAccuracyEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/CESoftmaxAccuracyEvaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/cross_encoder/evaluation/__init__.py` & `sentence_transformers-2.7.0/sentence_transformers/cross_encoder/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/datasets/DenoisingAutoEncoderDataset.py` & `sentence_transformers-2.7.0/sentence_transformers/datasets/DenoisingAutoEncoderDataset.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/datasets/NoDuplicatesDataLoader.py` & `sentence_transformers-2.7.0/sentence_transformers/datasets/NoDuplicatesDataLoader.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/datasets/ParallelSentencesDataset.py` & `sentence_transformers-2.7.0/sentence_transformers/datasets/ParallelSentencesDataset.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/datasets/SentenceLabelDataset.py` & `sentence_transformers-2.7.0/sentence_transformers/datasets/SentenceLabelDataset.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/datasets/SentencesDataset.py` & `sentence_transformers-2.7.0/sentence_transformers/datasets/SentencesDataset.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/BinaryClassificationEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/BinaryClassificationEvaluator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from . import SentenceEvaluator
 import logging
 import os
 import csv
 from sklearn.metrics.pairwise import paired_cosine_distances, paired_euclidean_distances, paired_manhattan_distances
 from sklearn.metrics import average_precision_score
 import numpy as np
-from typing import List
+from typing import List, Optional
 from ..readers import InputExample
 
 
 logger = logging.getLogger(__name__)
 
 
 class BinaryClassificationEvaluator(SentenceEvaluator):
@@ -26,29 +28,33 @@
     :param sentences1: The first column of sentences
     :param sentences2: The second column of sentences
     :param labels: labels[i] is the label for the pair (sentences1[i], sentences2[i]). Must be 0 or 1
     :param name: Name for the output
     :param batch_size: Batch size used to compute embeddings
     :param show_progress_bar: If true, prints a progress bar
     :param write_csv: Write results to a CSV file
+    :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current truncation
+        dimension. Defaults to None.
     """
 
     def __init__(
         self,
         sentences1: List[str],
         sentences2: List[str],
         labels: List[int],
         name: str = "",
         batch_size: int = 32,
         show_progress_bar: bool = False,
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
     ):
         self.sentences1 = sentences1
         self.sentences2 = sentences2
         self.labels = labels
+        self.truncate_dim = truncate_dim
 
         assert len(self.sentences1) == len(self.sentences2)
         assert len(self.sentences1) == len(self.labels)
         for label in labels:
             assert label == 0 or label == 1
 
         self.write_csv = write_csv
@@ -102,24 +108,26 @@
 
         for example in examples:
             sentences1.append(example.texts[0])
             sentences2.append(example.texts[1])
             scores.append(example.label)
         return cls(sentences1, sentences2, scores, **kwargs)
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         if epoch != -1:
             if steps == -1:
-                out_txt = f" after epoch {epoch}:"
+                out_txt = f" after epoch {epoch}"
             else:
-                out_txt = f" in epoch {epoch} after {steps} steps:"
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
 
-        logger.info("Binary Accuracy Evaluation of the model on " + self.name + " dataset" + out_txt)
+        logger.info(f"Binary Accuracy Evaluation of the model on the {self.name} dataset{out_txt}:")
 
         scores = self.compute_metrices(model)
 
         # Main score is the max of Average Precision (AP)
         main_score = max(scores[short_name]["ap"] for short_name in scores)
 
         file_output_data = [epoch, steps]
@@ -140,33 +148,39 @@
                 with open(csv_path, newline="", mode="a", encoding="utf-8") as f:
                     writer = csv.writer(f)
                     writer.writerow(file_output_data)
 
         return main_score
 
     def compute_metrices(self, model):
-        try:
-            # If the sentences are hashable, then we can use a set to avoid embedding the same sentences multiple times
-            sentences = list(set(self.sentences1 + self.sentences2))
-            embeddings = model.encode(
-                sentences, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar, convert_to_numpy=True
-            )
-            emb_dict = {sent: emb for sent, emb in zip(sentences, embeddings)}
-            embeddings1 = [emb_dict[sent] for sent in self.sentences1]
-            embeddings2 = [emb_dict[sent] for sent in self.sentences2]
-        except TypeError:
-            # Otherwise we just embed everything, e.g. if the sentences are images for evaluating a CLIP model
-            embeddings = model.encode(
-                self.sentences1 + self.sentences2,
-                batch_size=self.batch_size,
-                show_progress_bar=self.show_progress_bar,
-                convert_to_numpy=True,
-            )
-            embeddings1 = embeddings[: len(self.sentences1)]
-            embeddings2 = embeddings[len(self.sentences1) :]
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            try:
+                # If the sentences are hashable, then we can use a set to avoid embedding the same sentences multiple
+                # times
+                sentences = list(set(self.sentences1 + self.sentences2))
+            except TypeError:
+                # Otherwise we just embed everything, e.g. if the sentences are images for evaluating a CLIP model
+                embeddings = model.encode(
+                    self.sentences1 + self.sentences2,
+                    batch_size=self.batch_size,
+                    show_progress_bar=self.show_progress_bar,
+                    convert_to_numpy=True,
+                )
+                embeddings1 = embeddings[: len(self.sentences1)]
+                embeddings2 = embeddings[len(self.sentences1) :]
+            else:
+                embeddings = model.encode(
+                    sentences,
+                    batch_size=self.batch_size,
+                    show_progress_bar=self.show_progress_bar,
+                    convert_to_numpy=True,
+                )
+                emb_dict = {sent: emb for sent, emb in zip(sentences, embeddings)}
+                embeddings1 = [emb_dict[sent] for sent in self.sentences1]
+                embeddings2 = [emb_dict[sent] for sent in self.sentences2]
 
         cosine_scores = 1 - paired_cosine_distances(embeddings1, embeddings2)
         manhattan_distances = paired_manhattan_distances(embeddings1, embeddings2)
         euclidean_distances = paired_euclidean_distances(embeddings1, embeddings2)
 
         embeddings1_np = np.asarray(embeddings1)
         embeddings2_np = np.asarray(embeddings2)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/EmbeddingSimilarityEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/EmbeddingSimilarityEvaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from contextlib import nullcontext
+
+from sentence_transformers import SentenceTransformer
 from . import SentenceEvaluator, SimilarityFunction
 import logging
 import os
 import csv
 from sklearn.metrics.pairwise import paired_cosine_distances, paired_euclidean_distances, paired_manhattan_distances
 from scipy.stats import pearsonr, spearmanr
 import numpy as np
@@ -29,32 +32,36 @@
         scores: List[float],
         batch_size: int = 16,
         main_similarity: SimilarityFunction = None,
         name: str = "",
         show_progress_bar: bool = False,
         write_csv: bool = True,
         precision: Optional[Literal["float32", "int8", "uint8", "binary", "ubinary"]] = None,
+        truncate_dim: Optional[int] = None,
     ):
         """
         Constructs an evaluator based for the dataset
 
         The labels need to indicate the similarity between the sentences.
 
         :param sentences1:  List with the first sentence in a pair
         :param sentences2: List with the second sentence in a pair
         :param scores: Similarity score between sentences1[i] and sentences2[i]
         :param write_csv: Write results to a CSV file
         :param precision: The precision to use for the embeddings. Can be "float32", "int8", "uint8", "binary", or
             "ubinary". Defaults to None.
+        :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current
+            truncation dimension. Defaults to None.
         """
         self.sentences1 = sentences1
         self.sentences2 = sentences2
         self.scores = scores
         self.write_csv = write_csv
         self.precision = precision
+        self.truncate_dim = truncate_dim
 
         assert len(self.sentences1) == len(self.sentences2)
         assert len(self.sentences1) == len(self.scores)
 
         self.main_similarity = main_similarity
         self.name = name
 
@@ -92,41 +99,44 @@
 
         for example in examples:
             sentences1.append(example.texts[0])
             sentences2.append(example.texts[1])
             scores.append(example.label)
         return cls(sentences1, sentences2, scores, **kwargs)
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         if epoch != -1:
             if steps == -1:
-                out_txt = " after epoch {}:".format(epoch)
+                out_txt = f" after epoch {epoch}"
             else:
-                out_txt = " in epoch {} after {} steps:".format(epoch, steps)
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
-
-        logger.info("EmbeddingSimilarityEvaluator: Evaluating the model on " + self.name + " dataset" + out_txt)
-
-        embeddings1 = model.encode(
-            self.sentences1,
-            batch_size=self.batch_size,
-            show_progress_bar=self.show_progress_bar,
-            convert_to_numpy=True,
-            precision=self.precision,
-            normalize_embeddings=bool(self.precision),
-        )
-        embeddings2 = model.encode(
-            self.sentences2,
-            batch_size=self.batch_size,
-            show_progress_bar=self.show_progress_bar,
-            convert_to_numpy=True,
-            precision=self.precision,
-            normalize_embeddings=bool(self.precision),
-        )
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
+
+        logger.info(f"EmbeddingSimilarityEvaluator: Evaluating the model on the {self.name} dataset{out_txt}:")
+
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            embeddings1 = model.encode(
+                self.sentences1,
+                batch_size=self.batch_size,
+                show_progress_bar=self.show_progress_bar,
+                convert_to_numpy=True,
+                precision=self.precision,
+                normalize_embeddings=bool(self.precision),
+            )
+            embeddings2 = model.encode(
+                self.sentences2,
+                batch_size=self.batch_size,
+                show_progress_bar=self.show_progress_bar,
+                convert_to_numpy=True,
+                precision=self.precision,
+                normalize_embeddings=bool(self.precision),
+            )
         # Binary and ubinary embeddings are packed, so we need to unpack them for the distance metrics
         if self.precision == "binary":
             embeddings1 = (embeddings1 + 128).astype(np.uint8)
             embeddings2 = (embeddings2 + 128).astype(np.uint8)
         if self.precision in ("ubinary", "binary"):
             embeddings1 = np.unpackbits(embeddings1, axis=1)
             embeddings2 = np.unpackbits(embeddings2, axis=1)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/InformationRetrievalEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/InformationRetrievalEvaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from . import SentenceEvaluator
 import torch
 from torch import Tensor
 import logging
 from tqdm import trange
 from ..util import cos_sim, dot_score
 import os
 import numpy as np
-from typing import List, Dict, Set, Callable
+from typing import List, Dict, Optional, Set, Callable
 import heapq
 
 
 logger = logging.getLogger(__name__)
 
 
 class InformationRetrievalEvaluator(SentenceEvaluator):
@@ -32,14 +34,15 @@
         accuracy_at_k: List[int] = [1, 3, 5, 10],
         precision_recall_at_k: List[int] = [1, 3, 5, 10],
         map_at_k: List[int] = [100],
         show_progress_bar: bool = False,
         batch_size: int = 32,
         name: str = "",
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
         score_functions: Dict[str, Callable[[Tensor, Tensor], Tensor]] = {
             "cos_sim": cos_sim,
             "dot_score": dot_score,
         },  # Score function, higher=more similar
         main_score_function: str = None,
     ):
         self.queries_ids = []
@@ -63,14 +66,15 @@
         self.show_progress_bar = show_progress_bar
         self.batch_size = batch_size
         self.name = name
         self.write_csv = write_csv
         self.score_functions = score_functions
         self.score_function_names = sorted(list(self.score_functions.keys()))
         self.main_score_function = main_score_function
+        self.truncate_dim = truncate_dim
 
         if name:
             name = "_" + name
 
         self.csv_file: str = "Information-Retrieval_evaluation" + name + "_results.csv"
         self.csv_headers = ["epoch", "steps"]
 
@@ -87,25 +91,28 @@
 
             for k in ndcg_at_k:
                 self.csv_headers.append("{}-NDCG@{}".format(score_name, k))
 
             for k in map_at_k:
                 self.csv_headers.append("{}-MAP@{}".format(score_name, k))
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1, *args, **kwargs) -> float:
+    def __call__(
+        self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1, *args, **kwargs
+    ) -> float:
         if epoch != -1:
-            out_txt = (
-                " after epoch {}:".format(epoch)
-                if steps == -1
-                else " in epoch {} after {} steps:".format(epoch, steps)
-            )
+            if steps == -1:
+                out_txt = f" after epoch {epoch}"
+            else:
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
 
-        logger.info("Information Retrieval Evaluation on " + self.name + " dataset" + out_txt)
+        logger.info(f"Information Retrieval Evaluation of the model on the {self.name} dataset{out_txt}:")
 
         scores = self.compute_metrices(model, *args, **kwargs)
 
         # Write results to disc
         if output_path is not None and self.write_csv:
             csv_path = os.path.join(output_path, self.csv_file)
             if not os.path.isfile(csv_path):
@@ -139,49 +146,58 @@
             fOut.close()
 
         if self.main_score_function is None:
             return max([scores[name]["map@k"][max(self.map_at_k)] for name in self.score_function_names])
         else:
             return scores[self.main_score_function]["map@k"][max(self.map_at_k)]
 
-    def compute_metrices(self, model, corpus_model=None, corpus_embeddings: Tensor = None) -> Dict[str, float]:
+    def compute_metrices(
+        self, model: SentenceTransformer, corpus_model=None, corpus_embeddings: Tensor = None
+    ) -> Dict[str, float]:
         if corpus_model is None:
             corpus_model = model
 
         max_k = max(
             max(self.mrr_at_k),
             max(self.ndcg_at_k),
             max(self.accuracy_at_k),
             max(self.precision_recall_at_k),
             max(self.map_at_k),
         )
 
         # Compute embedding for the queries
-        query_embeddings = model.encode(
-            self.queries, show_progress_bar=self.show_progress_bar, batch_size=self.batch_size, convert_to_tensor=True
-        )
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            query_embeddings = model.encode(
+                self.queries,
+                show_progress_bar=self.show_progress_bar,
+                batch_size=self.batch_size,
+                convert_to_tensor=True,
+            )
 
         queries_result_list = {}
         for name in self.score_functions:
             queries_result_list[name] = [[] for _ in range(len(query_embeddings))]
 
         # Iterate over chunks of the corpus
         for corpus_start_idx in trange(
             0, len(self.corpus), self.corpus_chunk_size, desc="Corpus Chunks", disable=not self.show_progress_bar
         ):
             corpus_end_idx = min(corpus_start_idx + self.corpus_chunk_size, len(self.corpus))
 
             # Encode chunk of corpus
             if corpus_embeddings is None:
-                sub_corpus_embeddings = corpus_model.encode(
-                    self.corpus[corpus_start_idx:corpus_end_idx],
-                    show_progress_bar=False,
-                    batch_size=self.batch_size,
-                    convert_to_tensor=True,
-                )
+                with nullcontext() if self.truncate_dim is None else corpus_model.truncate_sentence_embeddings(
+                    self.truncate_dim
+                ):
+                    sub_corpus_embeddings = corpus_model.encode(
+                        self.corpus[corpus_start_idx:corpus_end_idx],
+                        show_progress_bar=False,
+                        batch_size=self.batch_size,
+                        convert_to_tensor=True,
+                    )
             else:
                 sub_corpus_embeddings = corpus_embeddings[corpus_start_idx:corpus_end_idx]
 
             # Compute cosine similarites
             for name, score_function in self.score_functions.items():
                 pair_scores = score_function(query_embeddings, sub_corpus_embeddings)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/LabelAccuracyEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/LabelAccuracyEvaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from sentence_transformers import SentenceTransformer
 from . import SentenceEvaluator
 import torch
 from torch.utils.data import DataLoader
 import logging
 from ..util import batch_to_device
 import os
 import csv
@@ -33,15 +34,15 @@
         if name:
             name = "_" + name
 
         self.write_csv = write_csv
         self.csv_file = "accuracy_evaluation" + name + "_results.csv"
         self.csv_headers = ["epoch", "steps", "accuracy"]
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         model.eval()
         total = 0
         correct = 0
 
         if epoch != -1:
             if steps == -1:
                 out_txt = " after epoch {}:".format(epoch)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/MSEEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/MSEEvaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from sentence_transformers.evaluation import SentenceEvaluator
 import logging
 import os
 import csv
-from typing import List
+from typing import List, Optional
 
 
 logger = logging.getLogger(__name__)
 
 
 class MSEEvaluator(SentenceEvaluator):
     """
@@ -20,59 +22,69 @@
 
     :param source_sentences: Source sentences are embedded with the teacher model
     :param target_sentences: Target sentences are ambedding with the student model.
     :param show_progress_bar: Show progress bar when computing embeddings
     :param batch_size: Batch size to compute sentence embeddings
     :param name: Name of the evaluator
     :param write_csv: Write results to CSV file
+    :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current truncation
+        dimension. Defaults to None.
     """
 
     def __init__(
         self,
         source_sentences: List[str],
         target_sentences: List[str],
         teacher_model=None,
         show_progress_bar: bool = False,
         batch_size: int = 32,
         name: str = "",
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
     ):
-        self.source_embeddings = teacher_model.encode(
-            source_sentences, show_progress_bar=show_progress_bar, batch_size=batch_size, convert_to_numpy=True
-        )
+        self.truncate_dim = truncate_dim
+        with nullcontext() if self.truncate_dim is None else teacher_model.truncate_sentence_embeddings(
+            self.truncate_dim
+        ):
+            self.source_embeddings = teacher_model.encode(
+                source_sentences, show_progress_bar=show_progress_bar, batch_size=batch_size, convert_to_numpy=True
+            )
 
         self.target_sentences = target_sentences
         self.show_progress_bar = show_progress_bar
         self.batch_size = batch_size
         self.name = name
 
         self.csv_file = "mse_evaluation_" + name + "_results.csv"
         self.csv_headers = ["epoch", "steps", "MSE"]
         self.write_csv = write_csv
 
-    def __call__(self, model, output_path, epoch=-1, steps=-1):
+    def __call__(self, model: SentenceTransformer, output_path, epoch=-1, steps=-1):
         if epoch != -1:
             if steps == -1:
-                out_txt = " after epoch {}:".format(epoch)
+                out_txt = f" after epoch {epoch}"
             else:
-                out_txt = " in epoch {} after {} steps:".format(epoch, steps)
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
-
-        target_embeddings = model.encode(
-            self.target_sentences,
-            show_progress_bar=self.show_progress_bar,
-            batch_size=self.batch_size,
-            convert_to_numpy=True,
-        )
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
+
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            target_embeddings = model.encode(
+                self.target_sentences,
+                show_progress_bar=self.show_progress_bar,
+                batch_size=self.batch_size,
+                convert_to_numpy=True,
+            )
 
         mse = ((self.source_embeddings - target_embeddings) ** 2).mean()
         mse *= 100
 
-        logger.info("MSE evaluation (lower = better) on " + self.name + " dataset" + out_txt)
+        logger.info(f"MSE evaluation (lower = better) on the {self.name} dataset{out_txt}:")
         logger.info("MSE (*100):\t{:4f}".format(mse))
 
         if output_path is not None and self.write_csv:
             csv_path = os.path.join(output_path, self.csv_file)
             output_file_exists = os.path.isfile(csv_path)
             with open(csv_path, newline="", mode="a" if output_file_exists else "w", encoding="utf-8") as f:
                 writer = csv.writer(f)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/MSEEvaluatorFromDataFrame.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/MSEEvaluatorFromDataFrame.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from contextlib import nullcontext
 from sentence_transformers.evaluation import SentenceEvaluator
 from sentence_transformers import SentenceTransformer
-from typing import List, Tuple, Dict
+from typing import List, Optional, Tuple, Dict
 import numpy as np
 import logging
 import os
 import csv
 
 
 logger = logging.getLogger(__name__)
@@ -13,41 +14,49 @@
 class MSEEvaluatorFromDataFrame(SentenceEvaluator):
     """
     Computes the mean squared error (x100) between the computed sentence embedding and some target sentence embedding.
 
     :param dataframe: It must have the following format. Rows contains different, parallel sentences.
         Columns are the respective language codes::
 
-            [{'en': 'My sentence', 'es': 'Sentence in Spanisch', 'fr': 'Sentence in French'...},
+            [{'en': 'My sentence in English', 'es': 'Oración en español', 'fr': 'Phrase en français'...},
              {'en': 'My second sentence', ...}]
+
     :param combinations: Must be of the format ``[('en', 'es'), ('en', 'fr'), ...]``.
         First entry in a tuple is the source language. The sentence in the respective language will be fetched from
         the dataframe and passed to the teacher model. Second entry in a tuple the the target language. Sentence
         will be fetched from the dataframe and passed to the student model
+    :param batch_size: Batch size to compute sentence embeddings
+    :param name: Name of the evaluator
+    :param write_csv: Write results to CSV file
+    :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current truncation
+        dimension. Defaults to None.
     """
 
     def __init__(
         self,
         dataframe: List[Dict[str, str]],
         teacher_model: SentenceTransformer,
         combinations: List[Tuple[str, str]],
         batch_size: int = 8,
-        name="",
+        name: str = "",
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
     ):
         self.combinations = combinations
         self.name = name
         self.batch_size = batch_size
 
         if name:
             name = "_" + name
 
         self.csv_file = "mse_evaluation" + name + "_results.csv"
         self.csv_headers = ["epoch", "steps"]
         self.write_csv = write_csv
+        self.truncate_dim = truncate_dim
         self.data = {}
 
         logger.info("Compute teacher embeddings")
         all_source_sentences = set()
         for src_lang, trg_lang in self.combinations:
             src_sentences = []
             trg_sentences = []
@@ -58,26 +67,30 @@
                     src_sentences.append(row[src_lang])
                     trg_sentences.append(row[trg_lang])
 
             self.data[(src_lang, trg_lang)] = (src_sentences, trg_sentences)
             self.csv_headers.append("{}-{}".format(src_lang, trg_lang))
 
         all_source_sentences = list(all_source_sentences)
-        all_src_embeddings = teacher_model.encode(all_source_sentences, batch_size=self.batch_size)
+        with nullcontext() if self.truncate_dim is None else teacher_model.truncate_sentence_embeddings(
+            self.truncate_dim
+        ):
+            all_src_embeddings = teacher_model.encode(all_source_sentences, batch_size=self.batch_size)
         self.teacher_embeddings = {sent: emb for sent, emb in zip(all_source_sentences, all_src_embeddings)}
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1):
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1):
         model.eval()
 
         mse_scores = []
         for src_lang, trg_lang in self.combinations:
             src_sentences, trg_sentences = self.data[(src_lang, trg_lang)]
 
             src_embeddings = np.asarray([self.teacher_embeddings[sent] for sent in src_sentences])
-            trg_embeddings = np.asarray(model.encode(trg_sentences, batch_size=self.batch_size))
+            with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+                trg_embeddings = np.asarray(model.encode(trg_sentences, batch_size=self.batch_size))
 
             mse = ((src_embeddings - trg_embeddings) ** 2).mean()
             mse *= 100
             mse_scores.append(mse)
 
             logger.info("MSE evaluation on {} dataset - {}-{}:".format(self.name, src_lang, trg_lang))
             logger.info("MSE (*100):\t{:4f}".format(mse))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/ParaphraseMiningEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/ParaphraseMiningEvaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from . import SentenceEvaluator
 import logging
 from sentence_transformers.util import paraphrase_mining
 import os
 import csv
 
-from typing import List, Tuple, Dict
+from typing import List, Optional, Tuple, Dict
 from collections import defaultdict
 
 
 logger = logging.getLogger(__name__)
 
 
 class ParaphraseMiningEvaluator(SentenceEvaluator):
@@ -28,14 +30,15 @@
         corpus_chunk_size: int = 100000,
         max_pairs: int = 500000,
         top_k: int = 100,
         show_progress_bar: bool = False,
         batch_size: int = 16,
         name: str = "",
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
     ):
         """
 
         :param sentences_map: A dictionary that maps sentence-ids to sentences, i.e. sentences_map[id] => sentence.
         :param duplicates_list: Duplicates_list is a list with id pairs [(id1, id2), (id1, id5)] that identifies the duplicates / paraphrases in the sentences_map
         :param duplicates_dict: A default dictionary mapping [id1][id2] to true if id1 and id2 are duplicates. Must be symmetric, i.e., if [id1][id2] => True, then [id2][id1] => True.
         :param add_transitive_closure: If true, it adds a transitive closure, i.e. if dup[a][b] and dup[b][c], then dup[a][c]
@@ -43,14 +46,17 @@
         :param corpus_chunk_size: The corpus will be batched, to reduce the memory requirement
         :param max_pairs: We will only extract up to #max_pairs potential paraphrase candidates.
         :param top_k: For each query, we extract the top_k most similar pairs and add it to a sorted list. I.e., for one sentence we cannot find more than top_k paraphrases
         :param show_progress_bar: Output a progress bar
         :param batch_size: Batch size for computing sentence embeddings
         :param name: Name of the experiment
         :param write_csv: Write results to CSV file
+        :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current truncation
+            dimension. Defaults to None.
+
         """
         self.sentences = []
         self.ids = []
 
         for id, sentence in sentences_map.items():
             self.sentences.append(sentence)
             self.ids.append(id)
@@ -58,14 +64,15 @@
         self.name = name
         self.show_progress_bar = show_progress_bar
         self.batch_size = batch_size
         self.query_chunk_size = query_chunk_size
         self.corpus_chunk_size = corpus_chunk_size
         self.max_pairs = max_pairs
         self.top_k = top_k
+        self.truncate_dim = truncate_dim
 
         self.duplicates = duplicates_dict if duplicates_dict is not None else defaultdict(lambda: defaultdict(bool))
         if duplicates_list is not None:
             for id1, id2 in duplicates_list:
                 if id1 in sentences_map and id2 in sentences_map:
                     self.duplicates[id1][id2] = True
                     self.duplicates[id2][id1] = True
@@ -89,33 +96,39 @@
         if name:
             name = "_" + name
 
         self.csv_file: str = "paraphrase_mining_evaluation" + name + "_results.csv"
         self.csv_headers = ["epoch", "steps", "precision", "recall", "f1", "threshold", "average_precision"]
         self.write_csv = write_csv
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         if epoch != -1:
-            out_txt = f" after epoch {epoch}:" if steps == -1 else f" in epoch {epoch} after {steps} steps:"
+            if steps == -1:
+                out_txt = f" after epoch {epoch}"
+            else:
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
 
-        logger.info("Paraphrase Mining Evaluation on " + self.name + " dataset" + out_txt)
+        logger.info(f"Paraphrase Mining Evaluation of the model on the {self.name} dataset{out_txt}:")
 
         # Compute embedding for the sentences
-        pairs_list = paraphrase_mining(
-            model,
-            self.sentences,
-            self.show_progress_bar,
-            self.batch_size,
-            self.query_chunk_size,
-            self.corpus_chunk_size,
-            self.max_pairs,
-            self.top_k,
-        )
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            pairs_list = paraphrase_mining(
+                model,
+                self.sentences,
+                self.show_progress_bar,
+                self.batch_size,
+                self.query_chunk_size,
+                self.corpus_chunk_size,
+                self.max_pairs,
+                self.top_k,
+            )
 
         logger.info("Number of candidate pairs: " + str(len(pairs_list)))
 
         # Compute F1 score and Average Precision
         n_extract = n_correct = 0
         threshold = 0
         best_f1 = best_recall = best_precision = 0
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/RerankingEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/RerankingEvaluator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,73 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from . import SentenceEvaluator
 import logging
 import numpy as np
 import os
 import csv
 from ..util import cos_sim
 import torch
 from sklearn.metrics import average_precision_score, ndcg_score
 import tqdm
-from typing import Optional
+from typing import Callable, Optional
 
 logger = logging.getLogger(__name__)
 
 
 class RerankingEvaluator(SentenceEvaluator):
     """
     This class evaluates a SentenceTransformer model for the task of re-ranking.
 
     Given a query and a list of documents, it computes the score [query, doc_i] for all possible
     documents and sorts them in decreasing order. Then, MRR@10, NDCG@10 and MAP is compute to measure the quality of the ranking.
 
-    :param samples: Must be a list and each element is of the form: {'query': '', 'positive': [], 'negative': []}. Query is the search query,
-     positive is a list of positive (relevant) documents, negative is a list of negative (irrelevant) documents.
+    :param samples: Must be a list and each element is of the form: {'query': '', 'positive': [], 'negative': []}.
+        Query is the search query, positive is a list of positive (relevant) documents, negative is a list of negative
+        (irrelevant) documents.
+
+    :param at_k: Only consider the top k most similar documents to each query for the evaluation
+    :param name: Name of the evaluator
+    :param write_csv: Write results to CSV file
+    :param similarity_fct: similarity function between sentence embeddings. By default, cosine similarity.
+    :param batch_size: Batch size to compute sentence embeddings
+    :param show_progress_bar: Show progress bar when computing embeddings
+    :param use_batched_encoding: Whether or not to encode queries and documents in batches for greater speed, or 1-by-1
+        to save memory
+    :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current truncation
+        dimension. Defaults to None.
     """
 
     def __init__(
         self,
         samples,
         at_k: int = 10,
         name: str = "",
         write_csv: bool = True,
-        similarity_fct=cos_sim,
+        similarity_fct: Callable[[torch.Tensor, torch.Tensor], torch.Tensor] = cos_sim,
         batch_size: int = 64,
         show_progress_bar: bool = False,
         use_batched_encoding: bool = True,
+        truncate_dim: Optional[int] = None,
         mrr_at_k: Optional[int] = None,
     ):
         self.samples = samples
         self.name = name
+
         if mrr_at_k is not None:
             logger.warning(f"The `mrr_at_k` parameter has been deprecated; please use `at_k={mrr_at_k}` instead.")
             self.at_k = mrr_at_k
         else:
             self.at_k = at_k
+
         self.similarity_fct = similarity_fct
         self.batch_size = batch_size
         self.show_progress_bar = show_progress_bar
         self.use_batched_encoding = use_batched_encoding
+        self.truncate_dim = truncate_dim
 
         if isinstance(self.samples, dict):
             self.samples = list(self.samples.values())
 
         ### Remove sample with empty positive / negative set
         self.samples = [
             sample for sample in self.samples if len(sample["positive"]) > 0 and len(sample["negative"]) > 0
@@ -61,24 +79,26 @@
             "steps",
             "MAP",
             "MRR@{}".format(self.at_k),
             "NDCG@{}".format(self.at_k),
         ]
         self.write_csv = write_csv
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         if epoch != -1:
             if steps == -1:
-                out_txt = " after epoch {}:".format(epoch)
+                out_txt = f" after epoch {epoch}"
             else:
-                out_txt = " in epoch {} after {} steps:".format(epoch, steps)
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
 
-        logger.info("RerankingEvaluator: Evaluating the model on " + self.name + " dataset" + out_txt)
+        logger.info(f"RerankingEvaluator: Evaluating the model on the {self.name} dataset{out_txt}:")
 
         scores = self.compute_metrices(model)
         mean_ap = scores["map"]
         mean_mrr = scores["mrr"]
         mean_ndcg = scores["ndcg"]
 
         #### Some stats about the dataset
@@ -125,30 +145,31 @@
         Computes the metrices in a batched way, by batching all queries and
         all documents together
         """
         all_mrr_scores = []
         all_ndcg_scores = []
         all_ap_scores = []
 
-        all_query_embs = model.encode(
-            [sample["query"] for sample in self.samples],
-            convert_to_tensor=True,
-            batch_size=self.batch_size,
-            show_progress_bar=self.show_progress_bar,
-        )
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            all_query_embs = model.encode(
+                [sample["query"] for sample in self.samples],
+                convert_to_tensor=True,
+                batch_size=self.batch_size,
+                show_progress_bar=self.show_progress_bar,
+            )
 
-        all_docs = []
+            all_docs = []
 
-        for sample in self.samples:
-            all_docs.extend(sample["positive"])
-            all_docs.extend(sample["negative"])
+            for sample in self.samples:
+                all_docs.extend(sample["positive"])
+                all_docs.extend(sample["negative"])
 
-        all_docs_embs = model.encode(
-            all_docs, convert_to_tensor=True, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar
-        )
+            all_docs_embs = model.encode(
+                all_docs, convert_to_tensor=True, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar
+            )
 
         # Compute scores
         query_idx, docs_idx = 0, 0
         for instance in self.samples:
             query_emb = all_query_embs[query_idx]
             query_idx += 1
 
@@ -206,18 +227,21 @@
 
             if len(positive) == 0 or len(negative) == 0:
                 continue
 
             docs = positive + negative
             is_relevant = [1] * len(positive) + [0] * len(negative)
 
-            query_emb = model.encode(
-                [query], convert_to_tensor=True, batch_size=self.batch_size, show_progress_bar=False
-            )
-            docs_emb = model.encode(docs, convert_to_tensor=True, batch_size=self.batch_size, show_progress_bar=False)
+            with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+                query_emb = model.encode(
+                    [query], convert_to_tensor=True, batch_size=self.batch_size, show_progress_bar=False
+                )
+                docs_emb = model.encode(
+                    docs, convert_to_tensor=True, batch_size=self.batch_size, show_progress_bar=False
+                )
 
             pred_scores = self.similarity_fct(query_emb, docs_emb)
             if len(pred_scores.shape) > 1:
                 pred_scores = pred_scores[0]
 
             pred_scores_argsort = torch.argsort(-pred_scores)  # Sort in decreasing order
             pred_scores = pred_scores.cpu().tolist()
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/SentenceEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/SentenceEvaluator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from sentence_transformers import SentenceTransformer
+
+
 class SentenceEvaluator:
     """
     Base class for all evaluators
 
     Extend this class and implement __call__ for custom evaluators.
     """
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         """
         This is called during training to evaluate the model.
         It returns a score for the evaluation with a higher score indicating a better result.
 
         :param model:
             the model to evaluate
         :param output_path:
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/SequentialEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/SequentialEvaluator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from sentence_transformers import SentenceTransformer
 from . import SentenceEvaluator
 from typing import Iterable
 
 
 class SequentialEvaluator(SentenceEvaluator):
     """
     This evaluator allows that multiple sub-evaluators are passed. When the model is evaluated,
@@ -10,13 +11,13 @@
     All scores are passed to 'main_score_function', which derives one final score value
     """
 
     def __init__(self, evaluators: Iterable[SentenceEvaluator], main_score_function=lambda scores: scores[-1]):
         self.evaluators = evaluators
         self.main_score_function = main_score_function
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         scores = []
         for evaluator in self.evaluators:
             scores.append(evaluator(model, output_path, epoch, steps))
 
         return self.main_score_function(scores)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/TranslationEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/TranslationEvaluator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from . import SentenceEvaluator
 import logging
 from ..util import pytorch_cos_sim
 import os
 import csv
 import numpy as np
-from typing import List
+from typing import List, Optional
 import torch
 
 
 logger = logging.getLogger(__name__)
 
 
 class TranslationEvaluator(SentenceEvaluator):
@@ -23,72 +25,86 @@
         source_sentences: List[str],
         target_sentences: List[str],
         show_progress_bar: bool = False,
         batch_size: int = 16,
         name: str = "",
         print_wrong_matches: bool = False,
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
     ):
         """
         Constructs an evaluator based for the dataset
 
         The labels need to indicate the similarity between the sentences.
 
         :param source_sentences:
             List of sentences in source language
         :param target_sentences:
             List of sentences in target language
+        :param show_progress_bar:
+            Show progress bar when computing embeddings
+        :param batch_size:
+            Batch size to compute sentence embeddings
+        :param name:
+            Name of the evaluator
         :param print_wrong_matches:
             Prints incorrect matches
         :param write_csv:
             Write results to CSV file
+        :param truncate_dim:
+            The dimension to truncate sentence embeddings to. `None` uses the model's current truncation dimension.
+            Defaults to None.
         """
         self.source_sentences = source_sentences
         self.target_sentences = target_sentences
         self.name = name
         self.batch_size = batch_size
         self.show_progress_bar = show_progress_bar
         self.print_wrong_matches = print_wrong_matches
+        self.truncate_dim = truncate_dim
 
         assert len(self.source_sentences) == len(self.target_sentences)
 
         if name:
             name = "_" + name
 
         self.csv_file = "translation_evaluation" + name + "_results.csv"
         self.csv_headers = ["epoch", "steps", "src2trg", "trg2src"]
         self.write_csv = write_csv
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         if epoch != -1:
             if steps == -1:
-                out_txt = " after epoch {}:".format(epoch)
+                out_txt = f" after epoch {epoch}"
             else:
-                out_txt = " in epoch {} after {} steps:".format(epoch, steps)
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
-
-        logger.info("Evaluating translation matching Accuracy on " + self.name + " dataset" + out_txt)
-
-        embeddings1 = torch.stack(
-            model.encode(
-                self.source_sentences,
-                show_progress_bar=self.show_progress_bar,
-                batch_size=self.batch_size,
-                convert_to_numpy=False,
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
+
+        logger.info(f"Evaluating translation matching Accuracy of the model on the {self.name} dataset{out_txt}:")
+
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            embeddings1 = torch.stack(
+                model.encode(
+                    self.source_sentences,
+                    show_progress_bar=self.show_progress_bar,
+                    batch_size=self.batch_size,
+                    convert_to_numpy=False,
+                )
             )
-        )
-        embeddings2 = torch.stack(
-            model.encode(
-                self.target_sentences,
-                show_progress_bar=self.show_progress_bar,
-                batch_size=self.batch_size,
-                convert_to_numpy=False,
+            embeddings2 = torch.stack(
+                model.encode(
+                    self.target_sentences,
+                    show_progress_bar=self.show_progress_bar,
+                    batch_size=self.batch_size,
+                    convert_to_numpy=False,
+                )
             )
-        )
 
         cos_sims = pytorch_cos_sim(embeddings1, embeddings2).detach().cpu().numpy()
 
         correct_src2trg = 0
         correct_trg2src = 0
 
         for i in range(len(cos_sims)):
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/TripletEvaluator.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/TripletEvaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from sentence_transformers import SentenceTransformer
+from contextlib import nullcontext
 from . import SentenceEvaluator, SimilarityFunction
 import logging
 import os
 import csv
 from sklearn.metrics.pairwise import paired_cosine_distances, paired_euclidean_distances, paired_manhattan_distances
-from typing import List
+from typing import List, Optional
 from ..readers import InputExample
 
 
 logger = logging.getLogger(__name__)
 
 
 class TripletEvaluator(SentenceEvaluator):
@@ -22,29 +24,33 @@
         positives: List[str],
         negatives: List[str],
         main_distance_function: SimilarityFunction = None,
         name: str = "",
         batch_size: int = 16,
         show_progress_bar: bool = False,
         write_csv: bool = True,
+        truncate_dim: Optional[int] = None,
     ):
         """
         :param anchors: Sentences to check similarity to. (e.g. a query)
         :param positives: List of positive sentences
         :param negatives: List of negative sentences
         :param main_distance_function: One of 0 (Cosine), 1 (Euclidean) or 2 (Manhattan). Defaults to None, returning all 3.
         :param name: Name for the output
         :param batch_size: Batch size used to compute embeddings
         :param show_progress_bar: If true, prints a progress bar
         :param write_csv: Write results to a CSV file
+        :param truncate_dim: The dimension to truncate sentence embeddings to. `None` uses the model's current
+            truncation dimension. Defaults to None.
         """
         self.anchors = anchors
         self.positives = positives
         self.negatives = negatives
         self.name = name
+        self.truncate_dim = truncate_dim
 
         assert len(self.anchors) == len(self.positives)
         assert len(self.anchors) == len(self.negatives)
 
         self.main_distance_function = main_distance_function
 
         self.batch_size = batch_size
@@ -66,37 +72,49 @@
 
         for example in examples:
             anchors.append(example.texts[0])
             positives.append(example.texts[1])
             negatives.append(example.texts[2])
         return cls(anchors, positives, negatives, **kwargs)
 
-    def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
+    def __call__(self, model: SentenceTransformer, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         if epoch != -1:
             if steps == -1:
-                out_txt = " after epoch {}:".format(epoch)
+                out_txt = f" after epoch {epoch}"
             else:
-                out_txt = " in epoch {} after {} steps:".format(epoch, steps)
+                out_txt = f" in epoch {epoch} after {steps} steps"
         else:
-            out_txt = ":"
+            out_txt = ""
+        if self.truncate_dim is not None:
+            out_txt += f" (truncated to {self.truncate_dim})"
 
-        logger.info("TripletEvaluator: Evaluating the model on " + self.name + " dataset" + out_txt)
+        logger.info(f"TripletEvaluator: Evaluating the model on the {self.name} dataset{out_txt}:")
 
         num_triplets = 0
         num_correct_cos_triplets, num_correct_manhattan_triplets, num_correct_euclidean_triplets = 0, 0, 0
 
-        embeddings_anchors = model.encode(
-            self.anchors, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar, convert_to_numpy=True
-        )
-        embeddings_positives = model.encode(
-            self.positives, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar, convert_to_numpy=True
-        )
-        embeddings_negatives = model.encode(
-            self.negatives, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar, convert_to_numpy=True
-        )
+        with nullcontext() if self.truncate_dim is None else model.truncate_sentence_embeddings(self.truncate_dim):
+            embeddings_anchors = model.encode(
+                self.anchors,
+                batch_size=self.batch_size,
+                show_progress_bar=self.show_progress_bar,
+                convert_to_numpy=True,
+            )
+            embeddings_positives = model.encode(
+                self.positives,
+                batch_size=self.batch_size,
+                show_progress_bar=self.show_progress_bar,
+                convert_to_numpy=True,
+            )
+            embeddings_negatives = model.encode(
+                self.negatives,
+                batch_size=self.batch_size,
+                show_progress_bar=self.show_progress_bar,
+                convert_to_numpy=True,
+            )
 
         # Cosine distance
         pos_cos_distance = paired_cosine_distances(embeddings_anchors, embeddings_positives)
         neg_cos_distances = paired_cosine_distances(embeddings_anchors, embeddings_negatives)
 
         # Manhattan
         pos_manhattan_distance = paired_manhattan_distances(embeddings_anchors, embeddings_positives)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/evaluation/__init__.py` & `sentence_transformers-2.7.0/sentence_transformers/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/AdaptiveLayerLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/AdaptiveLayerLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/AnglELoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/AnglELoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/BatchAllTripletLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/BatchAllTripletLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/BatchHardSoftMarginTripletLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/BatchHardSoftMarginTripletLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/BatchHardTripletLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/BatchHardTripletLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/BatchSemiHardTripletLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/BatchSemiHardTripletLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/CachedMultipleNegativesRankingLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/CachedMultipleNegativesRankingLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/CoSENTLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/CoSENTLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/ContrastiveLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/ContrastiveLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/ContrastiveTensionLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/ContrastiveTensionLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/CosineSimilarityLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/CosineSimilarityLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/DenoisingAutoEncoderLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/DenoisingAutoEncoderLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/GISTEmbedLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/GISTEmbedLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/MSELoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/MSELoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/MarginMSELoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/MarginMSELoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/Matryoshka2dLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/Matryoshka2dLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/MatryoshkaLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/MatryoshkaLoss.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,19 @@
         self.idx = 0
 
     def set_dim(self, dim):
         self.dim = dim
         self.idx = 0
 
     def shrink(self, tensor: Tensor) -> Tensor:
+        tensor_dim = tensor.shape[-1]
+        if self.dim > tensor_dim:
+            raise ValueError(
+                f"Dimension {self.dim} in matryoshka_dims cannot be greater than the model's embedding dimension: {tensor_dim}"
+            )
         tensor = tensor[..., : self.dim]
         tensor = F.normalize(tensor, p=2, dim=-1)
         return tensor
 
     def __call__(self, features):
         # Growing cache:
         if self.cache_dim is None or self.cache_dim == self.dim:
@@ -108,29 +113,30 @@
         if matryoshka_weights is None:
             matryoshka_weights = [1] * len(matryoshka_dims)
         self.matryoshka_weights = matryoshka_weights
         self.n_dims_per_step = n_dims_per_step
 
     def forward(self, sentence_features: Iterable[Dict[str, Tensor]], labels: Tensor) -> Tensor:
         original_forward = self.model.forward
-        decorated_forward = ForwardDecorator(original_forward)
-        self.model.forward = decorated_forward
-
-        dim_indices = range(len(self.matryoshka_dims))
-        if self.n_dims_per_step > 0 and self.n_dims_per_step < len(dim_indices):
-            dim_indices = random.sample(dim_indices, self.n_dims_per_step)
-
-        loss = 0.0
-        for idx in dim_indices:
-            dim = self.matryoshka_dims[idx]
-            weight = self.matryoshka_weights[idx]
-            decorated_forward.set_dim(dim)
-            loss += weight * self.loss(sentence_features, labels)
-
-        self.model.forward = original_forward
+        try:
+            decorated_forward = ForwardDecorator(original_forward)
+            self.model.forward = decorated_forward
+
+            dim_indices = range(len(self.matryoshka_dims))
+            if self.n_dims_per_step > 0 and self.n_dims_per_step < len(dim_indices):
+                dim_indices = random.sample(dim_indices, self.n_dims_per_step)
+
+            loss = 0.0
+            for idx in dim_indices:
+                dim = self.matryoshka_dims[idx]
+                weight = self.matryoshka_weights[idx]
+                decorated_forward.set_dim(dim)
+                loss += weight * self.loss(sentence_features, labels)
+        finally:
+            self.model.forward = original_forward
         return loss
 
     def get_config_dict(self) -> Dict[str, Any]:
         return {
             "loss": self.loss.__class__.__name__,
             "matryoshka_dims": self.matryoshka_dims,
             "matryoshka_weights": self.matryoshka_weights,
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/MegaBatchMarginLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/MegaBatchMarginLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/MultipleNegativesRankingLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/MultipleNegativesRankingLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/MultipleNegativesSymmetricRankingLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/MultipleNegativesSymmetricRankingLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/OnlineContrastiveLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/OnlineContrastiveLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/SoftmaxLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/SoftmaxLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/TripletLoss.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/TripletLoss.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/losses/__init__.py` & `sentence_transformers-2.7.0/sentence_transformers/losses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 from .CoSENTLoss import CoSENTLoss
 from .AnglELoss import AnglELoss
 from .OnlineContrastiveLoss import OnlineContrastiveLoss
 from .MegaBatchMarginLoss import MegaBatchMarginLoss
 from .DenoisingAutoEncoderLoss import DenoisingAutoEncoderLoss
 from .GISTEmbedLoss import GISTEmbedLoss
+from .CachedGISTEmbedLoss import CachedGISTEmbedLoss
 
 # Triplet losses
 from .BatchHardTripletLoss import BatchHardTripletLoss, BatchHardTripletLossDistanceFunction
 from .BatchHardSoftMarginTripletLoss import BatchHardSoftMarginTripletLoss
 from .BatchSemiHardTripletLoss import BatchSemiHardTripletLoss
 from .BatchAllTripletLoss import BatchAllTripletLoss
 
@@ -38,14 +39,15 @@
     "TripletDistanceMetric",
     "MarginMSELoss",
     "MatryoshkaLoss",
     "Matryoshka2dLoss",
     "MSELoss",
     "ContrastiveLoss",
     "SiameseDistanceMetric",
+    "CachedGISTEmbedLoss",
     "CachedMultipleNegativesRankingLoss",
     "ContrastiveTensionLoss",
     "ContrastiveTensionLossInBatchNegatives",
     "ContrastiveTensionDataLoader",
     "CoSENTLoss",
     "AnglELoss",
     "OnlineContrastiveLoss",
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/model_card_templates.py` & `sentence_transformers-2.7.0/sentence_transformers/model_card_templates.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/Asym.py` & `sentence_transformers-2.7.0/sentence_transformers/models/Asym.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,30 +86,30 @@
                     "structure": model_structure,
                     "parameters": {"allow_empty_key": self.allow_empty_key},
                 },
                 fOut,
                 indent=2,
             )
 
-    def tokenize(self, texts: Union[List[str], List[Tuple[str, str]]]):
+    def tokenize(self, texts: Union[List[str], List[Tuple[str, str]]], **kwargs):
         """
         Tokenizes a text and maps tokens to token-ids
         """
         if not isinstance(texts[0], dict):
             raise AttributeError("Asym. model requires that texts are passed as dicts: {'key': 'text'}")
 
         module_key = None
 
         for lookup in texts:
             text_key, text = next(iter(lookup.items()))
             if module_key is None:
                 module_key = text_key
 
             assert text_key == module_key  # Mixed batches are not allowed
-        return self.sub_modules[module_key][0].tokenize(texts)
+        return self.sub_modules[module_key][0].tokenize(texts, **kwargs)
 
     @staticmethod
     def load(input_path):
         with open(os.path.join(input_path, "config.json")) as fIn:
             config = json.load(fIn)
 
         modules = {}
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/BoW.py` & `sentence_transformers-2.7.0/sentence_transformers/models/BoW.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         self.tokenizer = WhitespaceTokenizer(vocab, stop_words=set(), do_lower_case=False)
         self.sentence_embedding_dimension = len(vocab)
 
     def forward(self, features: Dict[str, Tensor]):
         # Nothing to do, everything is done in get_sentence_features
         return features
 
-    def tokenize(self, texts: List[str]) -> List[int]:
-        tokenized = [self.tokenizer.tokenize(text) for text in texts]
+    def tokenize(self, texts: List[str], **kwargs) -> List[int]:
+        tokenized = [self.tokenizer.tokenize(text, **kwargs) for text in texts]
         return self.get_sentence_features(tokenized)
 
     def get_sentence_embedding_dimension(self):
         return self.sentence_embedding_dimension
 
     def get_sentence_features(self, tokenized_texts: List[List[int]], pad_seq_length: int = 0):
         vectors = []
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/CLIPModel.py` & `sentence_transformers-2.7.0/sentence_transformers/models/CLIPModel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from torch import nn
 import transformers
 import torch
 from PIL import Image
 
 
 class CLIPModel(nn.Module):
@@ -45,35 +46,37 @@
             else:
                 sentence_embedding.append(next(text_features))
 
         features["sentence_embedding"] = torch.stack(sentence_embedding).float()
 
         return features
 
-    def tokenize(self, texts):
+    def tokenize(self, texts, padding: Union[str, bool] = True):
         images = []
         texts_values = []
         image_text_info = []
 
         for idx, data in enumerate(texts):
             if isinstance(data, Image.Image):  # An Image
                 images.append(data)
                 image_text_info.append(0)
             else:  # A text
                 texts_values.append(data)
                 image_text_info.append(1)
 
-        if len(texts_values) == 0:
-            texts_values = None
-        if len(images) == 0:
-            images = None
-
-        inputs = self.processor(text=texts_values, images=images, return_tensors="pt", padding=True)
-        inputs["image_text_info"] = image_text_info
-        return inputs
+        encoding = {}
+        if len(texts_values):
+            encoding = self.processor.tokenizer(texts_values, return_tensors="pt", padding=padding)
+
+        if len(images):
+            image_features = self.processor.image_processor(images, return_tensors="pt")
+            encoding["pixel_values"] = image_features.pixel_values
+
+        encoding["image_text_info"] = image_text_info
+        return encoding
 
     def save(self, output_path: str):
         self.model.save_pretrained(output_path)
         self.processor.save_pretrained(output_path)
 
     @staticmethod
     def load(input_path: str):
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/CNN.py` & `sentence_transformers-2.7.0/sentence_transformers/models/CNN.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         features.update({"token_embeddings": out})
         return features
 
     def get_word_embedding_dimension(self) -> int:
         return self.embeddings_dimension
 
-    def tokenize(self, text: str) -> List[int]:
+    def tokenize(self, text: str, **kwargs) -> List[int]:
         raise NotImplementedError()
 
     def save(self, output_path: str):
         with open(os.path.join(output_path, "cnn_config.json"), "w") as fOut:
             json.dump(self.get_config_dict(), fOut, indent=2)
 
         torch.save(self.state_dict(), os.path.join(output_path, "pytorch_model.bin"))
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/Dense.py` & `sentence_transformers-2.7.0/sentence_transformers/models/Dense.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/Dropout.py` & `sentence_transformers-2.7.0/sentence_transformers/models/Dropout.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/LSTM.py` & `sentence_transformers-2.7.0/sentence_transformers/models/LSTM.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         unpack = nn.utils.rnn.pad_packed_sequence(packed[0], batch_first=True)[0]
         features.update({"token_embeddings": unpack})
         return features
 
     def get_word_embedding_dimension(self) -> int:
         return self.embeddings_dimension
 
-    def tokenize(self, text: str) -> List[int]:
+    def tokenize(self, text: str, **kwargs) -> List[int]:
         raise NotImplementedError()
 
     def save(self, output_path: str):
         with open(os.path.join(output_path, "lstm_config.json"), "w") as fOut:
             json.dump(self.get_config_dict(), fOut, indent=2)
 
         torch.save(self.state_dict(), os.path.join(output_path, "pytorch_model.bin"))
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/LayerNorm.py` & `sentence_transformers-2.7.0/sentence_transformers/models/LayerNorm.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/Normalize.py` & `sentence_transformers-2.7.0/sentence_transformers/models/Normalize.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/Pooling.py` & `sentence_transformers-2.7.0/sentence_transformers/models/Pooling.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/Transformer.py` & `sentence_transformers-2.7.0/sentence_transformers/models/Transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             features.update({"all_layer_embeddings": hidden_states})
 
         return features
 
     def get_word_embedding_dimension(self) -> int:
         return self.auto_model.config.hidden_size
 
-    def tokenize(self, texts: Union[List[str], List[Dict], List[Tuple[str, str]]]):
+    def tokenize(self, texts: Union[List[str], List[Dict], List[Tuple[str, str]]], padding: Union[str, bool] = True):
         """
         Tokenizes a text and maps tokens to token-ids
         """
         output = {}
         if isinstance(texts[0], str):
             to_tokenize = [texts]
         elif isinstance(texts[0], dict):
@@ -141,15 +141,15 @@
         # Lowercase
         if self.do_lower_case:
             to_tokenize = [[s.lower() for s in col] for col in to_tokenize]
 
         output.update(
             self.tokenizer(
                 *to_tokenize,
-                padding=True,
+                padding=padding,
                 truncation="longest_first",
                 return_tensors="pt",
                 max_length=self.max_seq_length,
             )
         )
         return output
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/WeightedLayerPooling.py` & `sentence_transformers-2.7.0/sentence_transformers/models/WeightedLayerPooling.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/WordEmbeddings.py` & `sentence_transformers-2.7.0/sentence_transformers/models/WordEmbeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
                 "token_embeddings": token_embeddings,
                 "cls_token_embeddings": cls_tokens,
                 "attention_mask": features["attention_mask"],
             }
         )
         return features
 
-    def tokenize(self, texts: List[str]):
-        tokenized_texts = [self.tokenizer.tokenize(text) for text in texts]
+    def tokenize(self, texts: List[str], **kwargs):
+        tokenized_texts = [self.tokenizer.tokenize(text, **kwargs) for text in texts]
         sentence_lengths = [len(tokens) for tokens in tokenized_texts]
         max_len = max(sentence_lengths)
 
         input_ids = []
         attention_masks = []
         for tokens in tokenized_texts:
             padding = [0] * (max_len - len(tokens))
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/WordWeights.py` & `sentence_transformers-2.7.0/sentence_transformers/models/WordWeights.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/__init__.py` & `sentence_transformers-2.7.0/sentence_transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/PhraseTokenizer.py` & `sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/PhraseTokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     self.ngram_lookup.add(word)
                     self.ngram_lengths.add(ngram_count)
 
         if len(vocab) > 0:
             logger.info("PhraseTokenizer - Phrase ngram lengths: {}".format(self.ngram_lengths))
             logger.info("PhraseTokenizer - Num phrases: {}".format(len(self.ngram_lookup)))
 
-    def tokenize(self, text: str) -> List[int]:
+    def tokenize(self, text: str, **kwargs) -> List[int]:
         from nltk import word_tokenize
 
         tokens = word_tokenize(text, preserve_line=True)
 
         # phrase detection
         for ngram_len in sorted(self.ngram_lengths, reverse=True):
             idx = 0
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/WhitespaceTokenizer.py` & `sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/WhitespaceTokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def get_vocab(self):
         return self.vocab
 
     def set_vocab(self, vocab: Iterable[str]):
         self.vocab = vocab
         self.word2idx = collections.OrderedDict([(word, idx) for idx, word in enumerate(vocab)])
 
-    def tokenize(self, text: str) -> List[int]:
+    def tokenize(self, text: str, **kwargs) -> List[int]:
         if self.do_lower_case:
             text = text.lower()
 
         tokens = text.split()
 
         tokens_filtered = []
         for token in tokens:
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/models/tokenizer/WordTokenizer.py` & `sentence_transformers-2.7.0/sentence_transformers/models/tokenizer/WordTokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         pass
 
     @abstractmethod
     def get_vocab(self, vocab: Iterable[str]):
         pass
 
     @abstractmethod
-    def tokenize(self, text: str) -> List[int]:
+    def tokenize(self, text: str, **kwargs) -> List[int]:
         pass
 
     @abstractmethod
     def save(self, output_path: str):
         pass
 
     @staticmethod
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/quantization.py` & `sentence_transformers-2.7.0/sentence_transformers/quantization.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,19 @@
 
     # Perform the search using the usearch index
     start_t = time.time()
     matches = corpus_index.search(query_embeddings, count=k, exact=exact)
     scores = matches.distances
     indices = matches.keys
 
+    if scores.ndim < 2:
+        scores = np.atleast_2d(scores)
+    if indices.ndim < 2:
+        indices = np.atleast_2d(indices)
+
     # If rescoring is enabled, we need to rescore the results using the rescore_embeddings
     if rescore_embeddings is not None:
         top_k_embeddings = np.array([corpus_index.get(query_indices) for query_indices in indices])
         # If the corpus precision is binary, we need to unpack the bits
         if corpus_precision == "binary":
             top_k_embeddings = np.unpackbits(top_k_embeddings.astype(np.uint8), axis=-1)
         top_k_embeddings = top_k_embeddings.astype(int)
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers/readers/InputExample.py` & `sentence_transformers-2.7.0/sentence_transformers/readers/InputExample.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/readers/LabelSentenceReader.py` & `sentence_transformers-2.7.0/sentence_transformers/readers/LabelSentenceReader.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/readers/NLIDataReader.py` & `sentence_transformers-2.7.0/sentence_transformers/readers/NLIDataReader.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/readers/PairedFilesReader.py` & `sentence_transformers-2.7.0/sentence_transformers/readers/PairedFilesReader.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/readers/STSDataReader.py` & `sentence_transformers-2.7.0/sentence_transformers/readers/STSDataReader.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/readers/TripletReader.py` & `sentence_transformers-2.7.0/sentence_transformers/readers/TripletReader.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/sentence_transformers/util.py` & `sentence_transformers-2.7.0/sentence_transformers/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import importlib
 import os
 import torch
 import numpy as np
 import queue
 import logging
-from typing import Dict, Optional, Union
+from typing import Dict, Optional, Union, overload
 
 from transformers import is_torch_npu_available
 from huggingface_hub import snapshot_download, hf_hub_download
 import heapq
 
 logger = logging.getLogger(__name__)
 
@@ -138,14 +138,33 @@
 def normalize_embeddings(embeddings: Tensor) -> Tensor:
     """
     Normalizes the embeddings matrix, so that each sentence embedding has unit length
     """
     return torch.nn.functional.normalize(embeddings, p=2, dim=1)
 
 
+@overload
+def truncate_embeddings(embeddings: np.ndarray, truncate_dim: Optional[int]) -> np.ndarray: ...
+
+
+@overload
+def truncate_embeddings(embeddings: torch.Tensor, truncate_dim: Optional[int]) -> torch.Tensor: ...
+
+
+def truncate_embeddings(
+    embeddings: Union[np.ndarray, torch.Tensor], truncate_dim: Optional[int]
+) -> Union[np.ndarray, torch.Tensor]:
+    """
+    :param embeddings: Embeddings to truncate.
+    :param truncate_dim: The dimension to truncate sentence embeddings to. `None` does no truncation.
+    :return: Truncated embeddings.
+    """
+    return embeddings[..., :truncate_dim]
+
+
 def paraphrase_mining(
     model, sentences: List[str], show_progress_bar: bool = False, batch_size: int = 32, *args, **kwargs
 ) -> List[List[Union[float, int]]]:
     """
     Given a list of sentences / texts, this function performs paraphrase mining. It compares all sentences against all
     other sentences and returns a list with the pairs that have the highest cosine similarity score.
 
@@ -588,24 +607,28 @@
             args = (*args[:2], None, *args[2:])
 
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
-def get_device_name() -> Literal["mps", "cuda", "npu", "cpu"]:
+def get_device_name() -> Literal["mps", "cuda", "npu", "hpu", "cpu"]:
     """
     Returns the name of the device where this module is running on.
     It's simple implementation that doesn't cover cases when more powerful GPUs are available and
     not a primary device ('cuda:0') or MPS device is available, but not configured properly:
     https://pytorch.org/docs/master/notes/mps.html
 
     :return: Device name, like 'cuda' or 'cpu'
     """
     if torch.cuda.is_available():
         return "cuda"
     elif torch.backends.mps.is_available():
         return "mps"
     elif is_torch_npu_available():
         return "npu"
-    else:
-        return "cpu"
+    elif importlib.util.find_spec("habana_frameworks") is not None:
+        import habana_frameworks.torch.hpu as hthpu
+
+        if hthpu.is_available():
+            return "hpu"
+    return "cpu"
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers.egg-info/PKG-INFO` & `sentence_transformers-2.7.0/sentence_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentence-transformers
-Version: 2.6.1
+Version: 2.7.0
 Summary: Multilingual text embeddings
 Home-page: https://www.SBERT.net
 Download-URL: https://github.com/UKPLab/sentence-transformers/
 Author: Nils Reimers
 Author-email: info@nils-reimers.de
 License: Apache License 2.0
 Keywords: Transformer Networks BERT XLNet sentence embedding PyTorch NLP deep learning
@@ -13,22 +13,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
-Requires-Dist: transformers<5.0.0,>=4.32.0
+Requires-Dist: transformers<5.0.0,>=4.34.0
 Requires-Dist: tqdm
 Requires-Dist: torch>=1.11.0
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: huggingface-hub>=0.15.1
 Requires-Dist: Pillow
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ruff>=0.3.0; extra == "dev"
 
 <!--- BADGES: START --->
 [![GitHub - License](https://img.shields.io/github/license/UKPLab/sentence-transformers?logo=github&style=flat&color=green)][#github-license]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sentence-transformers?logo=pypi&style=flat&color=blue)][#pypi-package]
 [![PyPI - Package Version](https://img.shields.io/pypi/v/sentence-transformers?logo=pypi&style=flat&color=orange)][#pypi-package]
 [![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/sentence-transformers?logo=anaconda&style=flat)][#conda-forge-package]
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/sentence-transformers?logo=anaconda&style=flat&color=orange)][#conda-forge-package]
@@ -169,14 +173,30 @@
  - [Text Summarization](https://www.sbert.net/examples/applications/text-summarization/README.html) 
 - [Multilingual Image Search, Clustering & Duplicate Detection](https://www.sbert.net/examples/applications/image-search/README.html)
 
 and many more use-cases.
 
 For all examples, see [examples/applications](https://github.com/UKPLab/sentence-transformers/tree/master/examples/applications).
 
+## Development setup
+
+After cloning the repo (or a fork) to your machine, in a virtual environment, run:
+
+```
+python -m pip install -e ".[dev]"
+
+pre-commit install
+```
+
+To test your changes, run:
+
+```
+pytest
+```
+
 ## Citing & Authors
 
 If you find this repository helpful, feel free to cite our publication [Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks](https://arxiv.org/abs/1908.10084):
 
 ```bibtex 
 @inproceedings{reimers-2019-sentence-bert,
     title = "Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks",
```

### Comparing `sentence-transformers-2.6.1/sentence_transformers.egg-info/SOURCES.txt` & `sentence_transformers-2.7.0/sentence_transformers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 sentence_transformers/evaluation/__init__.py
 sentence_transformers/losses/AdaptiveLayerLoss.py
 sentence_transformers/losses/AnglELoss.py
 sentence_transformers/losses/BatchAllTripletLoss.py
 sentence_transformers/losses/BatchHardSoftMarginTripletLoss.py
 sentence_transformers/losses/BatchHardTripletLoss.py
 sentence_transformers/losses/BatchSemiHardTripletLoss.py
+sentence_transformers/losses/CachedGISTEmbedLoss.py
 sentence_transformers/losses/CachedMultipleNegativesRankingLoss.py
 sentence_transformers/losses/CoSENTLoss.py
 sentence_transformers/losses/ContrastiveLoss.py
 sentence_transformers/losses/ContrastiveTensionLoss.py
 sentence_transformers/losses/CosineSimilarityLoss.py
 sentence_transformers/losses/DenoisingAutoEncoderLoss.py
 sentence_transformers/losses/GISTEmbedLoss.py
```

### Comparing `sentence-transformers-2.6.1/setup.py` & `sentence_transformers-2.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,42 @@
 
 with open("README.md", mode="r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 
 setup(
     name="sentence-transformers",
-    version="2.6.1",
+    version="2.7.0",
     author="Nils Reimers",
     author_email="info@nils-reimers.de",
     description="Multilingual text embeddings",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://www.SBERT.net",
     download_url="https://github.com/UKPLab/sentence-transformers/",
     packages=find_packages(),
     python_requires=">=3.8.0",
     install_requires=[
-        "transformers>=4.32.0,<5.0.0",
+        "transformers>=4.34.0,<5.0.0",
         "tqdm",
         "torch>=1.11.0",
         "numpy",
         "scikit-learn",
         "scipy",
         "huggingface-hub>=0.15.1",
         "Pillow",
     ],
+    extras_require={
+        "dev": [
+            "pre-commit",
+            "pytest",
+            "ruff>=0.3.0",
+        ],
+    },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
```

### Comparing `sentence-transformers-2.6.1/tests/test_cmnrl.py` & `sentence_transformers-2.7.0/tests/test_cmnrl.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_compute_embeddings.py` & `sentence_transformers-2.7.0/tests/test_compute_embeddings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Computes embeddings
 """
 
 import numpy as np
 
 from sentence_transformers import SentenceTransformer
+from sentence_transformers.util import get_device_name
 
 
 def test_encode_token_embeddings(paraphrase_distilroberta_base_v1_model: SentenceTransformer) -> None:
     """
     Test that encode(output_value='token_embeddings') works
     :return:
     """
@@ -18,40 +19,46 @@
         "Here comes another sentence",
         "My final sentence",
         "Sentences",
         "Sentence five five five five five five five",
     ]
     emb = model.encode(sent, output_value="token_embeddings", batch_size=2)
     assert len(emb) == len(sent)
-    for s, e in zip(sent, emb):
-        assert len(model.tokenize([s])["input_ids"][0]) == e.shape[0]
+
+    device = get_device_name()
+    if device == "hpu":
+        for s, e in zip(sent, emb):
+            assert len(model.tokenize([s])["input_ids"][0]) == model.get_max_seq_length()
+    else:
+        for s, e in zip(sent, emb):
+            assert len(model.tokenize([s])["input_ids"][0]) == e.shape[0]
 
 
 def test_encode_single_sentences(paraphrase_distilroberta_base_v1_model: SentenceTransformer) -> None:
     model = paraphrase_distilroberta_base_v1_model
     # Single sentence
     emb = model.encode("Hello Word, a test sentence")
     assert emb.shape == (768,)
-    assert abs(np.sum(emb) - 7.9811716) < 0.001
+    assert abs(np.sum(emb) - 7.9811716) < 0.002
 
     # Single sentence as list
     emb = model.encode(["Hello Word, a test sentence"])
     assert emb.shape == (1, 768)
-    assert abs(np.sum(emb) - 7.9811716) < 0.001
+    assert abs(np.sum(emb) - 7.9811716) < 0.002
 
     # Sentence list
     emb = model.encode(
         [
             "Hello Word, a test sentence",
             "Here comes another sentence",
             "My final sentence",
         ]
     )
     assert emb.shape == (3, 768)
-    assert abs(np.sum(emb) - 22.968266) < 0.001
+    assert abs(np.sum(emb) - 22.968266) < 0.007
 
 
 def test_encode_normalize(paraphrase_distilroberta_base_v1_model: SentenceTransformer) -> None:
     model = paraphrase_distilroberta_base_v1_model
     emb = model.encode(
         [
             "Hello Word, a test sentence",
@@ -66,19 +73,19 @@
 
 
 def test_encode_tuple_sentences(paraphrase_distilroberta_base_v1_model: SentenceTransformer) -> None:
     model = paraphrase_distilroberta_base_v1_model
     # Input a sentence tuple
     emb = model.encode([("Hello Word, a test sentence", "Second input for model")])
     assert emb.shape == (1, 768)
-    assert abs(np.sum(emb) - 9.503508) < 0.001
+    assert abs(np.sum(emb) - 9.503508) < 0.002
 
     # List of sentence tuples
     emb = model.encode(
         [
             ("Hello Word, a test sentence", "Second input for model"),
             ("My second tuple", "With two inputs"),
             ("Final tuple", "final test"),
         ]
     )
     assert emb.shape == (3, 768)
-    assert abs(np.sum(emb) - 32.14627) < 0.001
+    assert abs(np.sum(emb) - 32.14627) < 0.002
```

### Comparing `sentence-transformers-2.6.1/tests/test_cross_encoder.py` & `sentence_transformers-2.7.0/tests/test_cross_encoder.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_evaluator.py` & `sentence_transformers-2.7.0/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_image_embeddings.py` & `sentence_transformers-2.7.0/tests/test_image_embeddings.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_multi_process.py` & `sentence_transformers-2.7.0/tests/test_multi_process.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_pretrained_stsb.py` & `sentence_transformers-2.7.0/tests/test_pretrained_stsb.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_sentence_transformer.py` & `sentence_transformers-2.7.0/tests/test_sentence_transformer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 Tests general behaviour of the SentenceTransformer class
 """
 
+from functools import partial
 import json
 import logging
 import os
 from pathlib import Path
 import re
 import tempfile
+from typing import Dict, List, Literal, Optional, Union, cast
+
 import numpy as np
 import pytest
 
 from huggingface_hub import HfApi, RepoUrl, GitRefs, GitRefInfo
 import torch
 from sentence_transformers import SentenceTransformer
 from sentence_transformers.models import Normalize, Transformer, Pooling
+from sentence_transformers import util
 
 
 def test_load_with_safetensors() -> None:
     with tempfile.TemporaryDirectory() as cache_folder:
         safetensors_model = SentenceTransformer(
             "sentence-transformers-testing/stsb-bert-tiny-safetensors",
             cache_folder=cache_folder,
@@ -376,7 +380,100 @@
         assert isinstance(embeddings, torch.Tensor)
     elif convert_to_numpy:
         assert embeddings[0].dtype == expected_numpy_dtype
         assert isinstance(embeddings, np.ndarray)
     else:
         assert embeddings[0].dtype == expected_torch_dtype
         assert isinstance(embeddings, list)
+
+
+@pytest.mark.parametrize("sentences", ("Single sentence", ["One sentence", "Another sentence"]))
+@pytest.mark.parametrize("convert_to_tensor", [True, False])
+@pytest.mark.parametrize("convert_to_numpy", [True, False])
+@pytest.mark.parametrize("normalize_embeddings", [True, False])
+@pytest.mark.parametrize("output_value", ["sentence_embedding", None])
+def test_encode_truncate(
+    sentences: Union[str, List[str]],
+    convert_to_tensor: bool,
+    convert_to_numpy: bool,
+    normalize_embeddings: bool,
+    output_value: Optional[Literal["sentence_embedding"]],
+) -> None:
+    model = SentenceTransformer("sentence-transformers-testing/stsb-bert-tiny-safetensors")
+    embeddings_full_unnormalized: torch.Tensor = model.encode(
+        sentences, convert_to_numpy=False, convert_to_tensor=True
+    )  # These are raw embeddings which serve as the reference to test against
+
+    def test(model: SentenceTransformer, expected_dim: int):
+        outputs = model.encode(
+            sentences,
+            output_value=output_value,
+            convert_to_tensor=convert_to_tensor,
+            convert_to_numpy=convert_to_numpy,
+            normalize_embeddings=normalize_embeddings,
+        )
+
+        # Extract the sentence embeddings out of outputs
+        if output_value is None:
+            # We get the whole plate
+            if not isinstance(outputs, List):
+                embeddings = outputs["sentence_embedding"]
+            else:
+                outputs = cast(List[Dict[str, torch.Tensor]], outputs)
+                # TODO: can overload model.encode if ppl want type checker compatibility
+                embeddings = [out_features["sentence_embedding"] for out_features in outputs]
+        else:
+            embeddings = outputs
+
+        # Test shape
+        if isinstance(embeddings, list):  # list of tensors
+            embeddings_shape = (len(embeddings), embeddings[0].shape[-1])
+        else:
+            embeddings_shape = embeddings.shape
+        expected_shape = (expected_dim,) if isinstance(sentences, str) else (len(sentences), expected_dim)
+        assert embeddings_shape == expected_shape
+        assert model.get_sentence_embedding_dimension() == expected_dim
+
+        # Convert embeddings to a torch Tensor for ease of testing
+        if isinstance(embeddings, list):
+            embeddings = torch.stack(embeddings)
+        elif isinstance(embeddings, np.ndarray):
+            embeddings = torch.from_numpy(embeddings).to(embeddings_full_unnormalized.device)
+            # On a non-cpu device, the device of torch.from_numpy(embeddings) is always CPU
+
+        # Test content
+        if normalize_embeddings:
+            if output_value is None:
+                # Currently, normalization is not performed; it's the raw output of the forward pass
+                pass
+            else:
+                normalize = partial(torch.nn.functional.normalize, p=2, dim=-1)
+                assert torch.allclose(
+                    embeddings,
+                    normalize(util.truncate_embeddings(embeddings_full_unnormalized, expected_dim)),
+                )
+        else:
+            assert torch.allclose(embeddings, util.truncate_embeddings(embeddings_full_unnormalized, expected_dim))
+
+    # Test init w/o setting truncate_dim (it's None)
+    original_output_dim: int = model.get_sentence_embedding_dimension()
+    test(model, expected_dim=original_output_dim)
+
+    # Test init w/ a set truncate_dim
+    truncate_dim = int(original_output_dim / 4)
+    model = SentenceTransformer("sentence-transformers-testing/stsb-bert-tiny-safetensors", truncate_dim=truncate_dim)
+    test(model, expected_dim=truncate_dim)
+
+    # Test setting the attribute after init to a greater dimension
+    new_truncate_dim = 2 * truncate_dim
+    model.truncate_dim = new_truncate_dim
+    test(model, expected_dim=new_truncate_dim)
+
+    # Test context manager
+    final_truncate_dim = int(original_output_dim / 8)
+    with model.truncate_sentence_embeddings(final_truncate_dim):
+        test(model, expected_dim=final_truncate_dim)
+    test(model, expected_dim=new_truncate_dim)  # b/c we've exited the context
+
+    # Test w/ an ouptut_dim that's larger than the original_output_dim. No truncation ends up happening
+    model.truncate_dim = 2 * original_output_dim
+    test(model, expected_dim=original_output_dim)
```

### Comparing `sentence-transformers-2.6.1/tests/test_train_stsb.py` & `sentence_transformers-2.7.0/tests/test_train_stsb.py`

 * *Files identical despite different names*

### Comparing `sentence-transformers-2.6.1/tests/test_util.py` & `sentence_transformers-2.7.0/tests/test_util.py`

 * *Files identical despite different names*

