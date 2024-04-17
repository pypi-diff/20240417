# Comparing `tmp/dataquality-2.0.2.tar.gz` & `tmp/dataquality-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-2.0.2.tar", max compression
+gzip compressed data, was "dataquality-2.1.1.tar", max compression
```

## Comparing `dataquality-2.0.2.tar` & `dataquality-2.1.1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0    10946 2024-04-17 00:55:59.936803 dataquality-2.0.2/LICENSE
--rw-r--r--   0        0        0     4427 2024-04-17 00:55:59.936803 dataquality-2.0.2/README.md
--rw-r--r--   0        0        0     4960 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/__init__.py
--rw-r--r--   0        0        0     7410 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/analytics.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/clients/__init__.py
--rw-r--r--   0        0        0    36493 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/clients/api.py
--rw-r--r--   0        0        0     8372 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/clients/objectstore.py
--rw-r--r--   0        0        0     1838 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/__init__.py
--rw-r--r--   0        0        0     9314 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/_config.py
--rw-r--r--   0        0        0     2740 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/auth.py
--rw-r--r--   0        0        0     7615 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/finish.py
--rw-r--r--   0        0        0     9591 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/init.py
--rw-r--r--   0        0        0    23749 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/log.py
--rw-r--r--   0        0        0     7039 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/report.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/__init__.py
--rw-r--r--   0        0        0    10238 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/auto.py
--rw-r--r--   0        0        0     6191 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0        0        0     7652 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/ner.py
--rw-r--r--   0        0        0     4374 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0        0        0     1594 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/notebook.py
--rw-r--r--   0        0        0     3865 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/schema.py
--rw-r--r--   0        0        0     3782 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0        0        0    10846 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/text_classification.py
--rw-r--r--   0        0        0    11313 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_start/__init__.py
--rw-r--r--   0        0        0     4537 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dqyolo.py
--rw-r--r--   0        0        0      293 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/__init__.py
--rw-r--r--   0        0        0    15040 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/fastai.py
--rw-r--r--   0        0        0    10008 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/hf.py
--rw-r--r--   0        0        0     6083 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/jsl.py
--rw-r--r--   0        0        0    15763 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/keras.py
--rw-r--r--   0        0        0     4375 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/legacy/keras.py
--rw-r--r--   0        0        0     4417 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/lightning.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/__init__.py
--rw-r--r--   0        0        0    12601 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/auto.py
--rw-r--r--   0        0        0     7996 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/core.py
--rw-r--r--   0        0        0      553 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/__init__.py
--rw-r--r--   0        0        0     1459 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/alpaca.py
--rw-r--r--   0        0        0     1815 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/base.py
--rw-r--r--   0        0        0     8472 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/chat.py
--rw-r--r--   0        0        0     9274 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/s2s_trainer.py
--rw-r--r--   0        0        0     3687 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/schema.py
--rw-r--r--   0        0        0    13713 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/setfit.py
--rw-r--r--   0        0        0    13024 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/torch.py
--rw-r--r--   0        0        0    29298 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0        0        0    13973 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0        0        0    17587 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/ultralytics.py
--rw-r--r--   0        0        0     6626 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/internal.py
--rw-r--r--   0        0        0       95 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/__init__.py
--rw-r--r--   0        0        0    13566 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/base_logger.py
--rw-r--r--   0        0        0      698 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0        0        0    27939 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0        0        0    17227 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0        0        0    10591 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0        0        0     6093 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/__init__.py
--rw-r--r--   0        0        0      366 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/chat.py
--rw-r--r--   0        0        0      408 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/completion.py
--rw-r--r--   0        0        0    23082 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/formatters.py
--rw-r--r--   0        0        0    18337 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py
--rw-r--r--   0        0        0     9841 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0        0        0    21606 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0        0        0    15223 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0        0        0    31960 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/text_ner.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0        0        0     2346 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0        0        0      510 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0        0        0      537 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0        0        0      226 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/__init__.py
--rw-r--r--   0        0        0      207 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/chat.py
--rw-r--r--   0        0        0      225 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/completion.py
--rw-r--r--   0        0        0     1275 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py
--rw-r--r--   0        0        0      398 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0        0        0      958 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0        0        0     1528 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0        0        0     1599 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/text_ner.py
--rw-r--r--   0        0        0      554 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0        0        0     8185 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0        0        0     3309 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0        0        0     9435 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0        0        0    12319 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/__init__.py
--rw-r--r--   0        0        0      370 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/chat.py
--rw-r--r--   0        0        0      412 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/completion.py
--rw-r--r--   0        0        0     7449 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/formatters.py
--rw-r--r--   0        0        0    11888 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py
--rw-r--r--   0        0        0      519 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0        0        0     7064 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0        0        0     9120 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0        0        0    32052 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0        0        0    28938 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/metrics.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/py.typed
--rw-r--r--   0        0        0      165 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/__init__.py
--rw-r--r--   0        0        0     8665 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/condition.py
--rw-r--r--   0        0        0     1206 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/cv.py
--rw-r--r--   0        0        0      583 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/dataframe.py
--rw-r--r--   0        0        0     4873 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/edit.py
--rw-r--r--   0        0        0      662 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/hf.py
--rw-r--r--   0        0        0      118 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/job.py
--rw-r--r--   0        0        0     5259 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/metrics.py
--rw-r--r--   0        0        0      245 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/model.py
--rw-r--r--   0        0        0      992 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/ner.py
--rw-r--r--   0        0        0      631 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/report.py
--rw-r--r--   0        0        0      287 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/request_type.py
--rw-r--r--   0        0        0     1513 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/route.py
--rw-r--r--   0        0        0     4584 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0        0        0     5674 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/seq2seq.py
--rw-r--r--   0        0        0      992 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/split.py
--rw-r--r--   0        0        0     1968 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/task_type.py
--rw-r--r--   0        0        0      740 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/torch.py
--rw-r--r--   0        0        0      222 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/__init__.py
--rw-r--r--   0        0        0      496 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/arrow.py
--rw-r--r--   0        0        0      458 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/auth.py
--rw-r--r--   0        0        0     9929 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/auto.py
--rw-r--r--   0        0        0      925 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/auto_trainer.py
--rw-r--r--   0        0        0     1229 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/cuda.py
--rw-r--r--   0        0        0     2129 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/cv.py
--rw-r--r--   0        0        0    19933 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/cv_smart_features.py
--rw-r--r--   0        0        0     3585 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/dq_logger.py
--rw-r--r--   0        0        0     3514 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/dqyolo.py
--rw-r--r--   0        0        0     6790 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/emb.py
--rw-r--r--   0        0        0     4181 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/file.py
--rw-r--r--   0        0        0     5685 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/hdf5_store.py
--rw-r--r--   0        0        0     4255 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/helpers.py
--rw-r--r--   0        0        0     1468 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/hf_images.py
--rw-r--r--   0        0        0    10182 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0        0        0      429 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/imports.py
--rw-r--r--   0        0        0    14766 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/jsl.py
--rw-r--r--   0        0        0     9146 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/keras.py
--rw-r--r--   0        0        0     2408 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/ml.py
--rw-r--r--   0        0        0    24732 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/name.py
--rw-r--r--   0        0        0     1661 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/od.py
--rw-r--r--   0        0        0     3288 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/patcher.py
--rw-r--r--   0        0        0     5833 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/profiler.py
--rw-r--r--   0        0        0        0 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0        0        0       43 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0        0        0    10055 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0        0        0    11898 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0        0        0    10666 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0        0        0     5340 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0        0        0     1914 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0        0        0     1317 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/seq2seq/__init__.py
--rw-r--r--   0        0        0     3768 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/seq2seq/data_error_potential.py
--rw-r--r--   0        0        0     3085 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/seq2seq/decoder_only.py
--rw-r--r--   0        0        0     7735 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/seq2seq/generation.py
--rw-r--r--   0        0        0     5396 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/seq2seq/logprobs.py
--rw-r--r--   0        0        0    12448 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/seq2seq/offsets.py
--rw-r--r--   0        0        0    15551 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/setfit.py
--rw-r--r--   0        0        0      475 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/task_helpers.py
--rw-r--r--   0        0        0      260 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/tf.py
--rw-r--r--   0        0        0     1987 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/thread_pool.py
--rw-r--r--   0        0        0    26656 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/torch.py
--rw-r--r--   0        0        0     5141 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/transformers.py
--rw-r--r--   0        0        0    12830 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/ultralytics.py
--rw-r--r--   0        0        0     5597 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/upload.py
--rw-r--r--   0        0        0     2004 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/upload_model.py
--rw-r--r--   0        0        0    12179 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/vaex.py
--rw-r--r--   0        0        0     1072 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/version.py
--rw-r--r--   0        0        0     4649 2024-04-17 00:55:59.952803 dataquality-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6936 1970-01-01 00:00:00.000000 dataquality-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-17 15:45:15.840797 dataquality-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4427 2024-04-17 15:45:15.840797 dataquality-2.1.1/README.md
+-rw-r--r--   0        0        0     4960 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/__init__.py
+-rw-r--r--   0        0        0     7410 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/analytics.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/clients/__init__.py
+-rw-r--r--   0        0        0    36493 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/clients/api.py
+-rw-r--r--   0        0        0     8372 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/clients/objectstore.py
+-rw-r--r--   0        0        0     1838 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/__init__.py
+-rw-r--r--   0        0        0     9314 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/_config.py
+-rw-r--r--   0        0        0     2740 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/auth.py
+-rw-r--r--   0        0        0     7615 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/finish.py
+-rw-r--r--   0        0        0     9591 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/init.py
+-rw-r--r--   0        0        0    23749 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/log.py
+-rw-r--r--   0        0        0     7039 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/core/report.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/__init__.py
+-rw-r--r--   0        0        0    10238 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/auto.py
+-rw-r--r--   0        0        0     6191 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0        0        0     7652 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/ner.py
+-rw-r--r--   0        0        0     4374 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0        0        0     1594 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/notebook.py
+-rw-r--r--   0        0        0     3865 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/schema.py
+-rw-r--r--   0        0        0     3782 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0        0        0    10846 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_auto/text_classification.py
+-rw-r--r--   0        0        0    11313 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dq_start/__init__.py
+-rw-r--r--   0        0        0     4537 2024-04-17 15:45:15.840797 dataquality-2.1.1/dataquality/dqyolo.py
+-rw-r--r--   0        0        0      293 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/__init__.py
+-rw-r--r--   0        0        0    15040 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/fastai.py
+-rw-r--r--   0        0        0    10008 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/hf.py
+-rw-r--r--   0        0        0     6083 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/jsl.py
+-rw-r--r--   0        0        0    15763 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/keras.py
+-rw-r--r--   0        0        0     4375 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/legacy/keras.py
+-rw-r--r--   0        0        0     4417 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/lightning.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/__init__.py
+-rw-r--r--   0        0        0    12601 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/auto.py
+-rw-r--r--   0        0        0     7996 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/core.py
+-rw-r--r--   0        0        0      553 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/__init__.py
+-rw-r--r--   0        0        0     1459 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/alpaca.py
+-rw-r--r--   0        0        0     1815 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/base.py
+-rw-r--r--   0        0        0     8472 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/chat.py
+-rw-r--r--   0        0        0     9274 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/s2s_trainer.py
+-rw-r--r--   0        0        0     3687 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/seq2seq/schema.py
+-rw-r--r--   0        0        0    13713 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/setfit.py
+-rw-r--r--   0        0        0    13024 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/torch.py
+-rw-r--r--   0        0        0    29298 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0        0        0    13973 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0        0        0    17587 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/integrations/ultralytics.py
+-rw-r--r--   0        0        0     6626 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/internal.py
+-rw-r--r--   0        0        0       95 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/__init__.py
+-rw-r--r--   0        0        0    13566 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/base_logger.py
+-rw-r--r--   0        0        0      698 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0        0        0    27939 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0        0        0    17227 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0        0        0    10591 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0        0        0     6093 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/chat.py
+-rw-r--r--   0        0        0      408 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/completion.py
+-rw-r--r--   0        0        0    23082 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/formatters.py
+-rw-r--r--   0        0        0    18337 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py
+-rw-r--r--   0        0        0     9841 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0        0        0    21606 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0        0        0    15223 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0        0        0    31960 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/data_logger/text_ner.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0        0        0     2346 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0        0        0      510 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0        0        0      537 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0        0        0      226 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/seq2seq/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/seq2seq/chat.py
+-rw-r--r--   0        0        0      225 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/seq2seq/completion.py
+-rw-r--r--   0        0        0     1275 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py
+-rw-r--r--   0        0        0      398 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0        0        0      958 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0        0        0     1528 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0        0        0     1599 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/logger_config/text_ner.py
+-rw-r--r--   0        0        0      554 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0        0        0     8185 2024-04-17 15:45:15.844797 dataquality-2.1.1/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0        0        0     3309 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0        0        0     9435 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0        0        0    12319 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/__init__.py
+-rw-r--r--   0        0        0      370 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/chat.py
+-rw-r--r--   0        0        0      412 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/completion.py
+-rw-r--r--   0        0        0     7449 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/formatters.py
+-rw-r--r--   0        0        0    11888 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py
+-rw-r--r--   0        0        0      519 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0        0        0     7064 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0        0        0     9120 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0        0        0    32052 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0        0        0    28938 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/metrics.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/py.typed
+-rw-r--r--   0        0        0      165 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/__init__.py
+-rw-r--r--   0        0        0     8665 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/condition.py
+-rw-r--r--   0        0        0     1206 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/cv.py
+-rw-r--r--   0        0        0      583 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/dataframe.py
+-rw-r--r--   0        0        0     4873 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/edit.py
+-rw-r--r--   0        0        0      662 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/hf.py
+-rw-r--r--   0        0        0      118 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/job.py
+-rw-r--r--   0        0        0     5259 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/metrics.py
+-rw-r--r--   0        0        0      245 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/model.py
+-rw-r--r--   0        0        0      992 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/ner.py
+-rw-r--r--   0        0        0      631 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/report.py
+-rw-r--r--   0        0        0      287 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/request_type.py
+-rw-r--r--   0        0        0     1513 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/route.py
+-rw-r--r--   0        0        0     4584 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0        0        0     5674 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/seq2seq.py
+-rw-r--r--   0        0        0      992 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/split.py
+-rw-r--r--   0        0        0     1968 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/task_type.py
+-rw-r--r--   0        0        0      740 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/schemas/torch.py
+-rw-r--r--   0        0        0      222 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/arrow.py
+-rw-r--r--   0        0        0      458 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/auth.py
+-rw-r--r--   0        0        0     9929 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/auto.py
+-rw-r--r--   0        0        0      925 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/auto_trainer.py
+-rw-r--r--   0        0        0     1229 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/cuda.py
+-rw-r--r--   0        0        0     2129 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/cv.py
+-rw-r--r--   0        0        0    19933 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/cv_smart_features.py
+-rw-r--r--   0        0        0     3585 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/dq_logger.py
+-rw-r--r--   0        0        0     3514 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/dqyolo.py
+-rw-r--r--   0        0        0     6790 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/emb.py
+-rw-r--r--   0        0        0     4181 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/file.py
+-rw-r--r--   0        0        0     5685 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/hdf5_store.py
+-rw-r--r--   0        0        0     4255 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/helpers.py
+-rw-r--r--   0        0        0     1468 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/hf_images.py
+-rw-r--r--   0        0        0    10182 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0        0        0      429 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/imports.py
+-rw-r--r--   0        0        0    14766 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/jsl.py
+-rw-r--r--   0        0        0     9146 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/keras.py
+-rw-r--r--   0        0        0     2408 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/ml.py
+-rw-r--r--   0        0        0    24732 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/name.py
+-rw-r--r--   0        0        0     1661 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/od.py
+-rw-r--r--   0        0        0     3332 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/patcher.py
+-rw-r--r--   0        0        0     5833 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/profiler.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0        0        0    10055 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0        0        0    11898 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0        0        0    10666 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0        0        0     5340 2024-04-17 15:45:15.848797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0        0        0     1914 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0        0        0     1317 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/seq2seq/__init__.py
+-rw-r--r--   0        0        0     3768 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/seq2seq/data_error_potential.py
+-rw-r--r--   0        0        0     3085 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/seq2seq/decoder_only.py
+-rw-r--r--   0        0        0     7735 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/seq2seq/generation.py
+-rw-r--r--   0        0        0     5396 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/seq2seq/logprobs.py
+-rw-r--r--   0        0        0    12448 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/seq2seq/offsets.py
+-rw-r--r--   0        0        0    15551 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/setfit.py
+-rw-r--r--   0        0        0      475 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/task_helpers.py
+-rw-r--r--   0        0        0      260 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/tf.py
+-rw-r--r--   0        0        0     1987 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/thread_pool.py
+-rw-r--r--   0        0        0    26656 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/torch.py
+-rw-r--r--   0        0        0     5141 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/transformers.py
+-rw-r--r--   0        0        0    12830 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/ultralytics.py
+-rw-r--r--   0        0        0     5597 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/upload.py
+-rw-r--r--   0        0        0     2004 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/upload_model.py
+-rw-r--r--   0        0        0    12179 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/vaex.py
+-rw-r--r--   0        0        0     1072 2024-04-17 15:45:15.852797 dataquality-2.1.1/dataquality/utils/version.py
+-rw-r--r--   0        0        0     4649 2024-04-17 15:45:15.856797 dataquality-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6936 1970-01-01 00:00:00.000000 dataquality-2.1.1/PKG-INFO
```

### Comparing `dataquality-2.0.2/LICENSE` & `dataquality-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/README.md` & `dataquality-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/__init__.py` & `dataquality-2.1.1/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .. code-block:: python
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.integrations
 from dataquality.core import configure, set_console_url
 from dataquality.core._config import config
```

### Comparing `dataquality-2.0.2/dataquality/analytics.py` & `dataquality-2.1.1/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/clients/api.py` & `dataquality-2.1.1/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/clients/objectstore.py` & `dataquality-2.1.1/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/__init__.py` & `dataquality-2.1.1/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/_config.py` & `dataquality-2.1.1/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/auth.py` & `dataquality-2.1.1/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/finish.py` & `dataquality-2.1.1/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/init.py` & `dataquality-2.1.1/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/log.py` & `dataquality-2.1.1/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/core/report.py` & `dataquality-2.1.1/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/auto.py` & `dataquality-2.1.1/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/base_data_manager.py` & `dataquality-2.1.1/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/ner.py` & `dataquality-2.1.1/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/ner_trainer.py` & `dataquality-2.1.1/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/notebook.py` & `dataquality-2.1.1/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/schema.py` & `dataquality-2.1.1/dataquality/dq_auto/schema.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/tc_trainer.py` & `dataquality-2.1.1/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_auto/text_classification.py` & `dataquality-2.1.1/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dq_start/__init__.py` & `dataquality-2.1.1/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/dqyolo.py` & `dataquality-2.1.1/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/fastai.py` & `dataquality-2.1.1/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/hf.py` & `dataquality-2.1.1/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/jsl.py` & `dataquality-2.1.1/dataquality/integrations/jsl.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/keras.py` & `dataquality-2.1.1/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/legacy/keras.py` & `dataquality-2.1.1/dataquality/integrations/legacy/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/lightning.py` & `dataquality-2.1.1/dataquality/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/auto.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/core.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/core.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/__init__.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/alpaca.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/alpaca.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/base.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/chat.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/formatters/chat.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/s2s_trainer.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/s2s_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/seq2seq/schema.py` & `dataquality-2.1.1/dataquality/integrations/seq2seq/schema.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/setfit.py` & `dataquality-2.1.1/dataquality/integrations/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/torch.py` & `dataquality-2.1.1/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-2.1.1/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/transformers_trainer.py` & `dataquality-2.1.1/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/integrations/ultralytics.py` & `dataquality-2.1.1/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/internal.py` & `dataquality-2.1.1/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/base_logger.py` & `dataquality-2.1.1/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/__init__.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/image_classification.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/object_detection.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/formatters.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/formatters.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/text_classification.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/data_logger/text_ner.py` & `dataquality-2.1.1/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-2.1.1/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/logger_config/object_detection.py` & `dataquality-2.1.1/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py` & `dataquality-2.1.1/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/logger_config/text_classification.py` & `dataquality-2.1.1/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-2.1.1/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/logger_config/text_ner.py` & `dataquality-2.1.1/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/__init__.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/image_classification.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/object_detection.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/formatters.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/formatters.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/text_classification.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/loggers/model_logger/text_ner.py` & `dataquality-2.1.1/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/metrics.py` & `dataquality-2.1.1/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/condition.py` & `dataquality-2.1.1/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/cv.py` & `dataquality-2.1.1/dataquality/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/dataframe.py` & `dataquality-2.1.1/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/edit.py` & `dataquality-2.1.1/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/hf.py` & `dataquality-2.1.1/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/metrics.py` & `dataquality-2.1.1/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/ner.py` & `dataquality-2.1.1/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/report.py` & `dataquality-2.1.1/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/route.py` & `dataquality-2.1.1/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/semantic_segmentation.py` & `dataquality-2.1.1/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/seq2seq.py` & `dataquality-2.1.1/dataquality/schemas/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/split.py` & `dataquality-2.1.1/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/task_type.py` & `dataquality-2.1.1/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/schemas/torch.py` & `dataquality-2.1.1/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/auto.py` & `dataquality-2.1.1/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/auto_trainer.py` & `dataquality-2.1.1/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/cuda.py` & `dataquality-2.1.1/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/cv.py` & `dataquality-2.1.1/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/cv_smart_features.py` & `dataquality-2.1.1/dataquality/utils/cv_smart_features.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/dq_logger.py` & `dataquality-2.1.1/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/dqyolo.py` & `dataquality-2.1.1/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/emb.py` & `dataquality-2.1.1/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/file.py` & `dataquality-2.1.1/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/hdf5_store.py` & `dataquality-2.1.1/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/helpers.py` & `dataquality-2.1.1/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/hf_images.py` & `dataquality-2.1.1/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/hf_tokenizer.py` & `dataquality-2.1.1/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/jsl.py` & `dataquality-2.1.1/dataquality/utils/jsl.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/keras.py` & `dataquality-2.1.1/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/ml.py` & `dataquality-2.1.1/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/name.py` & `dataquality-2.1.1/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/od.py` & `dataquality-2.1.1/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/patcher.py` & `dataquality-2.1.1/dataquality/utils/patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         weak_instance = weakref.ref(instance, self._cleanup_callback)
         self._instances.add(weak_instance)
 
     def _cleanup_callback(self, weak_instance: Any) -> None:
         """Call the cleanup function when the object is garbage collected.
         :param weak_instance: The weak reference to the object that was
         garbage collected."""
-        self.cleanup_func()
+        if callable(self.cleanup_func):
+            self.cleanup_func()
         self._instances.discard(weak_instance)
 
 
 class Cleanup:
     """Base class for objects that need to be cleaned up when they are
     garbage collected."""
```

### Comparing `dataquality-2.0.2/dataquality/utils/profiler.py` & `dataquality-2.1.1/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-2.1.1/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-2.1.1/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-2.1.1/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-2.1.1/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-2.1.1/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/seq2seq/__init__.py` & `dataquality-2.1.1/dataquality/utils/seq2seq/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/seq2seq/data_error_potential.py` & `dataquality-2.1.1/dataquality/utils/seq2seq/data_error_potential.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/seq2seq/decoder_only.py` & `dataquality-2.1.1/dataquality/utils/seq2seq/decoder_only.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/seq2seq/generation.py` & `dataquality-2.1.1/dataquality/utils/seq2seq/generation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/seq2seq/logprobs.py` & `dataquality-2.1.1/dataquality/utils/seq2seq/logprobs.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/seq2seq/offsets.py` & `dataquality-2.1.1/dataquality/utils/seq2seq/offsets.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/setfit.py` & `dataquality-2.1.1/dataquality/utils/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/thread_pool.py` & `dataquality-2.1.1/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/torch.py` & `dataquality-2.1.1/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/transformers.py` & `dataquality-2.1.1/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/ultralytics.py` & `dataquality-2.1.1/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/upload.py` & `dataquality-2.1.1/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/upload_model.py` & `dataquality-2.1.1/dataquality/utils/upload_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/vaex.py` & `dataquality-2.1.1/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/dataquality/utils/version.py` & `dataquality-2.1.1/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.2/pyproject.toml` & `dataquality-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dataquality"
-version = "2.0.2"
+version = "2.1.1"
 description = ""
 authors = ["Galileo Technologies, Inc. <team@rungalileo.io>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/rungalileo/dataquality"
 documentation = "https://rungalileo.gitbook.io/galileo"
 scripts = { dqyolo = "dataquality.dqyolo:main" }
```

### Comparing `dataquality-2.0.2/PKG-INFO` & `dataquality-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 2.0.2
+Version: 2.1.1
 Summary: 
 Home-page: https://github.com/rungalileo/dataquality
 License: Apache-2.0
 Author: Galileo Technologies, Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

