# Comparing `tmp/dataquality-2.0.1.tar.gz` & `tmp/dataquality-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-2.0.1.tar", max compression
+gzip compressed data, was "dataquality-2.0.2.tar", max compression
```

## Comparing `dataquality-2.0.1.tar` & `dataquality-2.0.2.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0    10946 2024-03-05 21:23:43.274654 dataquality-2.0.1/LICENSE
--rw-r--r--   0        0        0     4427 2024-03-05 21:23:43.274654 dataquality-2.0.1/README.md
--rw-r--r--   0        0        0     4960 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/__init__.py
--rw-r--r--   0        0        0     7410 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/analytics.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/clients/__init__.py
--rw-r--r--   0        0        0    36493 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/clients/api.py
--rw-r--r--   0        0        0     8372 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/clients/objectstore.py
--rw-r--r--   0        0        0     1838 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/__init__.py
--rw-r--r--   0        0        0     9314 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/_config.py
--rw-r--r--   0        0        0     2740 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/auth.py
--rw-r--r--   0        0        0     7615 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/finish.py
--rw-r--r--   0        0        0     9663 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/init.py
--rw-r--r--   0        0        0    23749 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/log.py
--rw-r--r--   0        0        0     7039 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/core/report.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/__init__.py
--rw-r--r--   0        0        0    10238 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/auto.py
--rw-r--r--   0        0        0     6191 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0        0        0     7652 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/ner.py
--rw-r--r--   0        0        0     4374 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0        0        0     1594 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/notebook.py
--rw-r--r--   0        0        0     3865 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/schema.py
--rw-r--r--   0        0        0     3782 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0        0        0    10846 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_auto/text_classification.py
--rw-r--r--   0        0        0    11313 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dq_start/__init__.py
--rw-r--r--   0        0        0     4537 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/dqyolo.py
--rw-r--r--   0        0        0      293 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/__init__.py
--rw-r--r--   0        0        0    15040 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/fastai.py
--rw-r--r--   0        0        0    10008 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/hf.py
--rw-r--r--   0        0        0     6083 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/jsl.py
--rw-r--r--   0        0        0    15763 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/keras.py
--rw-r--r--   0        0        0     4375 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/legacy/keras.py
--rw-r--r--   0        0        0     4417 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/lightning.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/__init__.py
--rw-r--r--   0        0        0    12601 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/auto.py
--rw-r--r--   0        0        0     7996 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/core.py
--rw-r--r--   0        0        0      553 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/alpaca.py
--rw-r--r--   0        0        0     1815 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/base.py
--rw-r--r--   0        0        0     8472 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/chat.py
--rw-r--r--   0        0        0     9274 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/s2s_trainer.py
--rw-r--r--   0        0        0     3687 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/seq2seq/schema.py
--rw-r--r--   0        0        0    13713 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/setfit.py
--rw-r--r--   0        0        0    13024 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/torch.py
--rw-r--r--   0        0        0    29298 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0        0        0    13973 2024-03-05 21:23:43.274654 dataquality-2.0.1/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0        0        0    17587 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/integrations/ultralytics.py
--rw-r--r--   0        0        0     6626 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/internal.py
--rw-r--r--   0        0        0       95 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/__init__.py
--rw-r--r--   0        0        0    13566 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/base_logger.py
--rw-r--r--   0        0        0      698 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0        0        0    27785 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0        0        0    17227 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0        0        0    10591 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0        0        0     6093 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/__init__.py
--rw-r--r--   0        0        0      366 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/chat.py
--rw-r--r--   0        0        0      408 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/completion.py
--rw-r--r--   0        0        0    23082 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/formatters.py
--rw-r--r--   0        0        0    18337 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py
--rw-r--r--   0        0        0     9841 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0        0        0    21606 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0        0        0    15223 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0        0        0    31960 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/data_logger/text_ner.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0        0        0     2346 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0        0        0      510 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0        0        0      537 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0        0        0      226 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/seq2seq/__init__.py
--rw-r--r--   0        0        0      207 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/seq2seq/chat.py
--rw-r--r--   0        0        0      225 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/seq2seq/completion.py
--rw-r--r--   0        0        0     1275 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py
--rw-r--r--   0        0        0      398 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0        0        0      958 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0        0        0     1528 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0        0        0     1599 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/logger_config/text_ner.py
--rw-r--r--   0        0        0      554 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0        0        0     8185 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0        0        0     3309 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0        0        0     9435 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0        0        0    12319 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/__init__.py
--rw-r--r--   0        0        0      370 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/chat.py
--rw-r--r--   0        0        0      412 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/completion.py
--rw-r--r--   0        0        0     7449 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/formatters.py
--rw-r--r--   0        0        0    11888 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py
--rw-r--r--   0        0        0      519 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0        0        0     7064 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0        0        0     9120 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0        0        0    32052 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0        0        0    28938 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/metrics.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/py.typed
--rw-r--r--   0        0        0      165 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/__init__.py
--rw-r--r--   0        0        0     8665 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/condition.py
--rw-r--r--   0        0        0     1206 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/cv.py
--rw-r--r--   0        0        0      583 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/dataframe.py
--rw-r--r--   0        0        0     4873 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/edit.py
--rw-r--r--   0        0        0      662 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/hf.py
--rw-r--r--   0        0        0      118 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/job.py
--rw-r--r--   0        0        0     5259 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/metrics.py
--rw-r--r--   0        0        0      245 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/model.py
--rw-r--r--   0        0        0      992 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/ner.py
--rw-r--r--   0        0        0      631 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/report.py
--rw-r--r--   0        0        0      287 2024-03-05 21:23:43.278654 dataquality-2.0.1/dataquality/schemas/request_type.py
--rw-r--r--   0        0        0     1513 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/schemas/route.py
--rw-r--r--   0        0        0     4584 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0        0        0     5674 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/schemas/seq2seq.py
--rw-r--r--   0        0        0      992 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/schemas/split.py
--rw-r--r--   0        0        0     1968 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/schemas/task_type.py
--rw-r--r--   0        0        0      740 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/schemas/torch.py
--rw-r--r--   0        0        0      222 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/__init__.py
--rw-r--r--   0        0        0      496 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/arrow.py
--rw-r--r--   0        0        0      458 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/auth.py
--rw-r--r--   0        0        0     9929 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/auto.py
--rw-r--r--   0        0        0      925 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/auto_trainer.py
--rw-r--r--   0        0        0     1229 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/cuda.py
--rw-r--r--   0        0        0     2082 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/cv.py
--rw-r--r--   0        0        0    19896 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/cv_smart_features.py
--rw-r--r--   0        0        0     3585 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/dq_logger.py
--rw-r--r--   0        0        0     3514 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/dqyolo.py
--rw-r--r--   0        0        0     6790 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/emb.py
--rw-r--r--   0        0        0     4181 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/file.py
--rw-r--r--   0        0        0     5685 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/hdf5_store.py
--rw-r--r--   0        0        0     4255 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/helpers.py
--rw-r--r--   0        0        0     1468 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/hf_images.py
--rw-r--r--   0        0        0    10182 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0        0        0      429 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/imports.py
--rw-r--r--   0        0        0    14766 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/jsl.py
--rw-r--r--   0        0        0     9146 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/keras.py
--rw-r--r--   0        0        0     2408 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/ml.py
--rw-r--r--   0        0        0    24732 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/name.py
--rw-r--r--   0        0        0     1661 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/od.py
--rw-r--r--   0        0        0     3288 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/patcher.py
--rw-r--r--   0        0        0     5833 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/profiler.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0        0        0       43 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0        0        0    10055 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0        0        0    11898 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0        0        0    10658 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0        0        0     5340 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0        0        0     1914 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0        0        0     1317 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/seq2seq/__init__.py
--rw-r--r--   0        0        0     3768 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/seq2seq/data_error_potential.py
--rw-r--r--   0        0        0     3085 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/seq2seq/decoder_only.py
--rw-r--r--   0        0        0     7735 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/seq2seq/generation.py
--rw-r--r--   0        0        0     5396 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/seq2seq/logprobs.py
--rw-r--r--   0        0        0    12448 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/seq2seq/offsets.py
--rw-r--r--   0        0        0    15551 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/setfit.py
--rw-r--r--   0        0        0      475 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/task_helpers.py
--rw-r--r--   0        0        0      260 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/tf.py
--rw-r--r--   0        0        0     1987 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/thread_pool.py
--rw-r--r--   0        0        0    26656 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/torch.py
--rw-r--r--   0        0        0     5141 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/transformers.py
--rw-r--r--   0        0        0    12830 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/ultralytics.py
--rw-r--r--   0        0        0     5597 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/upload.py
--rw-r--r--   0        0        0     2004 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/upload_model.py
--rw-r--r--   0        0        0    12179 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/vaex.py
--rw-r--r--   0        0        0     1072 2024-03-05 21:23:43.282654 dataquality-2.0.1/dataquality/utils/version.py
--rw-r--r--   0        0        0     4277 2024-03-05 21:23:43.290654 dataquality-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6699 1970-01-01 00:00:00.000000 dataquality-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-17 00:55:59.936803 dataquality-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4427 2024-04-17 00:55:59.936803 dataquality-2.0.2/README.md
+-rw-r--r--   0        0        0     4960 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/__init__.py
+-rw-r--r--   0        0        0     7410 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/analytics.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/clients/__init__.py
+-rw-r--r--   0        0        0    36493 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/clients/api.py
+-rw-r--r--   0        0        0     8372 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/clients/objectstore.py
+-rw-r--r--   0        0        0     1838 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/__init__.py
+-rw-r--r--   0        0        0     9314 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/_config.py
+-rw-r--r--   0        0        0     2740 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/auth.py
+-rw-r--r--   0        0        0     7615 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/finish.py
+-rw-r--r--   0        0        0     9591 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/init.py
+-rw-r--r--   0        0        0    23749 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/log.py
+-rw-r--r--   0        0        0     7039 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/core/report.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/__init__.py
+-rw-r--r--   0        0        0    10238 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/auto.py
+-rw-r--r--   0        0        0     6191 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0        0        0     7652 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/ner.py
+-rw-r--r--   0        0        0     4374 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0        0        0     1594 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/notebook.py
+-rw-r--r--   0        0        0     3865 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/schema.py
+-rw-r--r--   0        0        0     3782 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0        0        0    10846 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_auto/text_classification.py
+-rw-r--r--   0        0        0    11313 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dq_start/__init__.py
+-rw-r--r--   0        0        0     4537 2024-04-17 00:55:59.936803 dataquality-2.0.2/dataquality/dqyolo.py
+-rw-r--r--   0        0        0      293 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/__init__.py
+-rw-r--r--   0        0        0    15040 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/fastai.py
+-rw-r--r--   0        0        0    10008 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/hf.py
+-rw-r--r--   0        0        0     6083 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/jsl.py
+-rw-r--r--   0        0        0    15763 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/keras.py
+-rw-r--r--   0        0        0     4375 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/legacy/keras.py
+-rw-r--r--   0        0        0     4417 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/lightning.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/__init__.py
+-rw-r--r--   0        0        0    12601 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/auto.py
+-rw-r--r--   0        0        0     7996 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/core.py
+-rw-r--r--   0        0        0      553 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/__init__.py
+-rw-r--r--   0        0        0     1459 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/alpaca.py
+-rw-r--r--   0        0        0     1815 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/base.py
+-rw-r--r--   0        0        0     8472 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/chat.py
+-rw-r--r--   0        0        0     9274 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/s2s_trainer.py
+-rw-r--r--   0        0        0     3687 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/seq2seq/schema.py
+-rw-r--r--   0        0        0    13713 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/setfit.py
+-rw-r--r--   0        0        0    13024 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/torch.py
+-rw-r--r--   0        0        0    29298 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0        0        0    13973 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0        0        0    17587 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/integrations/ultralytics.py
+-rw-r--r--   0        0        0     6626 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/internal.py
+-rw-r--r--   0        0        0       95 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/__init__.py
+-rw-r--r--   0        0        0    13566 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/base_logger.py
+-rw-r--r--   0        0        0      698 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0        0        0    27939 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0        0        0    17227 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0        0        0    10591 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0        0        0     6093 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/chat.py
+-rw-r--r--   0        0        0      408 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/completion.py
+-rw-r--r--   0        0        0    23082 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/formatters.py
+-rw-r--r--   0        0        0    18337 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py
+-rw-r--r--   0        0        0     9841 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0        0        0    21606 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0        0        0    15223 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0        0        0    31960 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/data_logger/text_ner.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0        0        0     2346 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0        0        0      510 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0        0        0      537 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0        0        0      226 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/chat.py
+-rw-r--r--   0        0        0      225 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/completion.py
+-rw-r--r--   0        0        0     1275 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py
+-rw-r--r--   0        0        0      398 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0        0        0      958 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0        0        0     1528 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0        0        0     1599 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/logger_config/text_ner.py
+-rw-r--r--   0        0        0      554 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0        0        0     8185 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0        0        0     3309 2024-04-17 00:55:59.940803 dataquality-2.0.2/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0        0        0     9435 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0        0        0    12319 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/__init__.py
+-rw-r--r--   0        0        0      370 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/chat.py
+-rw-r--r--   0        0        0      412 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/completion.py
+-rw-r--r--   0        0        0     7449 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/formatters.py
+-rw-r--r--   0        0        0    11888 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py
+-rw-r--r--   0        0        0      519 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0        0        0     7064 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0        0        0     9120 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0        0        0    32052 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0        0        0    28938 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/metrics.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/py.typed
+-rw-r--r--   0        0        0      165 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/__init__.py
+-rw-r--r--   0        0        0     8665 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/condition.py
+-rw-r--r--   0        0        0     1206 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/cv.py
+-rw-r--r--   0        0        0      583 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/dataframe.py
+-rw-r--r--   0        0        0     4873 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/edit.py
+-rw-r--r--   0        0        0      662 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/hf.py
+-rw-r--r--   0        0        0      118 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/job.py
+-rw-r--r--   0        0        0     5259 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/metrics.py
+-rw-r--r--   0        0        0      245 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/model.py
+-rw-r--r--   0        0        0      992 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/ner.py
+-rw-r--r--   0        0        0      631 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/report.py
+-rw-r--r--   0        0        0      287 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/request_type.py
+-rw-r--r--   0        0        0     1513 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/route.py
+-rw-r--r--   0        0        0     4584 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0        0        0     5674 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/seq2seq.py
+-rw-r--r--   0        0        0      992 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/split.py
+-rw-r--r--   0        0        0     1968 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/task_type.py
+-rw-r--r--   0        0        0      740 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/schemas/torch.py
+-rw-r--r--   0        0        0      222 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/arrow.py
+-rw-r--r--   0        0        0      458 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/auth.py
+-rw-r--r--   0        0        0     9929 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/auto.py
+-rw-r--r--   0        0        0      925 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/auto_trainer.py
+-rw-r--r--   0        0        0     1229 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/cuda.py
+-rw-r--r--   0        0        0     2129 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/cv.py
+-rw-r--r--   0        0        0    19933 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/cv_smart_features.py
+-rw-r--r--   0        0        0     3585 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/dq_logger.py
+-rw-r--r--   0        0        0     3514 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/dqyolo.py
+-rw-r--r--   0        0        0     6790 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/emb.py
+-rw-r--r--   0        0        0     4181 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/file.py
+-rw-r--r--   0        0        0     5685 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/hdf5_store.py
+-rw-r--r--   0        0        0     4255 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/helpers.py
+-rw-r--r--   0        0        0     1468 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/hf_images.py
+-rw-r--r--   0        0        0    10182 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0        0        0      429 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/imports.py
+-rw-r--r--   0        0        0    14766 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/jsl.py
+-rw-r--r--   0        0        0     9146 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/keras.py
+-rw-r--r--   0        0        0     2408 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/ml.py
+-rw-r--r--   0        0        0    24732 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/name.py
+-rw-r--r--   0        0        0     1661 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/od.py
+-rw-r--r--   0        0        0     3288 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/patcher.py
+-rw-r--r--   0        0        0     5833 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/profiler.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0        0        0    10055 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0        0        0    11898 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0        0        0    10666 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0        0        0     5340 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0        0        0     1914 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0        0        0     1317 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/seq2seq/__init__.py
+-rw-r--r--   0        0        0     3768 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/seq2seq/data_error_potential.py
+-rw-r--r--   0        0        0     3085 2024-04-17 00:55:59.944803 dataquality-2.0.2/dataquality/utils/seq2seq/decoder_only.py
+-rw-r--r--   0        0        0     7735 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/seq2seq/generation.py
+-rw-r--r--   0        0        0     5396 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/seq2seq/logprobs.py
+-rw-r--r--   0        0        0    12448 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/seq2seq/offsets.py
+-rw-r--r--   0        0        0    15551 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/setfit.py
+-rw-r--r--   0        0        0      475 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/task_helpers.py
+-rw-r--r--   0        0        0      260 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/tf.py
+-rw-r--r--   0        0        0     1987 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/thread_pool.py
+-rw-r--r--   0        0        0    26656 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/torch.py
+-rw-r--r--   0        0        0     5141 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/transformers.py
+-rw-r--r--   0        0        0    12830 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/ultralytics.py
+-rw-r--r--   0        0        0     5597 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/upload.py
+-rw-r--r--   0        0        0     2004 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/upload_model.py
+-rw-r--r--   0        0        0    12179 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/vaex.py
+-rw-r--r--   0        0        0     1072 2024-04-17 00:55:59.948803 dataquality-2.0.2/dataquality/utils/version.py
+-rw-r--r--   0        0        0     4649 2024-04-17 00:55:59.952803 dataquality-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6936 1970-01-01 00:00:00.000000 dataquality-2.0.2/PKG-INFO
```

### Comparing `dataquality-2.0.1/LICENSE` & `dataquality-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/README.md` & `dataquality-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/__init__.py` & `dataquality-2.0.2/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .. code-block:: python
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.integrations
 from dataquality.core import configure, set_console_url
 from dataquality.core._config import config
```

### Comparing `dataquality-2.0.1/dataquality/analytics.py` & `dataquality-2.0.2/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/clients/api.py` & `dataquality-2.0.2/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/clients/objectstore.py` & `dataquality-2.0.2/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/core/__init__.py` & `dataquality-2.0.2/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/core/_config.py` & `dataquality-2.0.2/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/core/auth.py` & `dataquality-2.0.2/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/core/finish.py` & `dataquality-2.0.2/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/core/init.py` & `dataquality-2.0.2/dataquality/core/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from dataquality.core.auth import login
 from dataquality.exceptions import GalileoException, GalileoWarning
 from dataquality.loggers import BaseGalileoLogger
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.dq_logger import DQ_LOG_FILE_HOME
 from dataquality.utils.helpers import check_noop
 from dataquality.utils.name import validate_name
-from dataquality.utils.version import version_check
 
 api_client = ApiClient()
 
 
 class InitManager:
     @retry(
         retry=retry_if_exception_type(GalileoException),
@@ -179,15 +178,14 @@
     :param overwrite_local: If True, the current project/run log directory will be
     cleared during this function. If logging over many sessions with checkpoints, you
     may want to set this to False. Default True
     """
     if not api_client.valid_current_user():
         login()
     _check_dq_version()
-    version_check()
     _init = InitManager()
     task_type = BaseGalileoLogger.validate_task(task_type)
     config.task_type = task_type
     if not project_name and run_name:
         # The user provided a run name and no project name. No good
         warnings.warn(
             "⚠️ You must specify a project name to initialize or create a new Galileo "
```

### Comparing `dataquality-2.0.1/dataquality/core/log.py` & `dataquality-2.0.2/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/core/report.py` & `dataquality-2.0.2/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/auto.py` & `dataquality-2.0.2/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/base_data_manager.py` & `dataquality-2.0.2/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/ner.py` & `dataquality-2.0.2/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/ner_trainer.py` & `dataquality-2.0.2/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/notebook.py` & `dataquality-2.0.2/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/schema.py` & `dataquality-2.0.2/dataquality/dq_auto/schema.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/tc_trainer.py` & `dataquality-2.0.2/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_auto/text_classification.py` & `dataquality-2.0.2/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dq_start/__init__.py` & `dataquality-2.0.2/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/dqyolo.py` & `dataquality-2.0.2/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/fastai.py` & `dataquality-2.0.2/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/hf.py` & `dataquality-2.0.2/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/jsl.py` & `dataquality-2.0.2/dataquality/integrations/jsl.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/keras.py` & `dataquality-2.0.2/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/legacy/keras.py` & `dataquality-2.0.2/dataquality/integrations/legacy/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/lightning.py` & `dataquality-2.0.2/dataquality/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/auto.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/core.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/core.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/__init__.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/alpaca.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/alpaca.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/base.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/formatters/chat.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/formatters/chat.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/s2s_trainer.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/s2s_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/seq2seq/schema.py` & `dataquality-2.0.2/dataquality/integrations/seq2seq/schema.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/setfit.py` & `dataquality-2.0.2/dataquality/integrations/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/torch.py` & `dataquality-2.0.2/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-2.0.2/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/transformers_trainer.py` & `dataquality-2.0.2/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/integrations/ultralytics.py` & `dataquality-2.0.2/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/internal.py` & `dataquality-2.0.2/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/base_logger.py` & `dataquality-2.0.2/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/__init__.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,16 +281,18 @@
                 )
                 # We have already created them here, so don't try again later
                 create_data_embs = False
         else:
             print(
                 "CuML libraries not found, running standard process. "
                 "For faster Galileo processing, consider installing\n"
-                "`pip install 'dataquality[cuda]' --extra-index-url="
-                "https://pypi.nvidia.com/`"
+                "`pip install 'dataquality[cuda11]' --extra-index-url="
+                "https://pypi.nvidia.com/` or `pip install '"
+                "dataquality[cuda12]' --extra-index-url="
+                "https://pypi.nvidia.com/` depending on your CUDA version."
             )
 
         for split in Split.get_valid_attributes():
             self.upload_split(
                 location=location,
                 split=split,
                 object_store=object_store,
```

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/image_classification.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/object_detection.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/formatters.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/formatters.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/seq2seq/seq2seq_base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/text_classification.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/data_logger/text_ner.py` & `dataquality-2.0.2/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-2.0.2/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/logger_config/object_detection.py` & `dataquality-2.0.2/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py` & `dataquality-2.0.2/dataquality/loggers/logger_config/seq2seq/seq2seq_base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/logger_config/text_classification.py` & `dataquality-2.0.2/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-2.0.2/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/logger_config/text_ner.py` & `dataquality-2.0.2/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/__init__.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/image_classification.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/object_detection.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/formatters.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/formatters.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/seq2seq/seq2seq_base.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/text_classification.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/loggers/model_logger/text_ner.py` & `dataquality-2.0.2/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/metrics.py` & `dataquality-2.0.2/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/condition.py` & `dataquality-2.0.2/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/cv.py` & `dataquality-2.0.2/dataquality/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/dataframe.py` & `dataquality-2.0.2/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/edit.py` & `dataquality-2.0.2/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/hf.py` & `dataquality-2.0.2/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/metrics.py` & `dataquality-2.0.2/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/ner.py` & `dataquality-2.0.2/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/report.py` & `dataquality-2.0.2/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/route.py` & `dataquality-2.0.2/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/semantic_segmentation.py` & `dataquality-2.0.2/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/seq2seq.py` & `dataquality-2.0.2/dataquality/schemas/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/split.py` & `dataquality-2.0.2/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/task_type.py` & `dataquality-2.0.2/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/schemas/torch.py` & `dataquality-2.0.2/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/auto.py` & `dataquality-2.0.2/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/auto_trainer.py` & `dataquality-2.0.2/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/cuda.py` & `dataquality-2.0.2/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/cv.py` & `dataquality-2.0.2/dataquality/utils/cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import hashlib
 import os
 from io import BytesIO
 from typing import Any, Optional
 
-from PIL import Image
+from PIL.Image import Image
+from PIL.Image import open as Image_open
 from pydantic import UUID4
 
 from dataquality import config
 from dataquality.clients.api import ApiClient
 from dataquality.clients.objectstore import ObjectStore
 from dataquality.exceptions import GalileoException
 
 object_store = ObjectStore()
 B64_CONTENT_TYPE_DELIMITER = ";base64,"
 
 api_client = ApiClient()
 
 
 def _bytes_to_img(b: bytes) -> Image:
-    return Image.open(BytesIO(b))
+    return Image_open(BytesIO(b))
 
 
 def _write_img_bytes_to_file(
     img: Optional[Any] = None,
     img_path: Optional[str] = None,
     image_id: Optional[str] = None,
 ) -> str:
```

### Comparing `dataquality-2.0.1/dataquality/utils/cv_smart_features.py` & `dataquality-2.0.2/dataquality/utils/cv_smart_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 import vaex
 from imagededup.methods import PHash
 from multiprocess import Pool, cpu_count
-from PIL import Image, ImageFilter, ImageStat
+from PIL import ImageFilter, ImageStat
+from PIL.Image import Image
+from PIL.Image import open as Image_open
 from vaex.dataframe import DataFrame
 
 from dataquality.exceptions import GalileoWarning
 from dataquality.schemas.cv import GAL_LOCAL_IMAGES_PATHS
 from dataquality.schemas.cv import CVSmartFeatureColumn as CVSF
 
 """
 CONSTANTS: the constants for all these methods were chosen conservatively with the goal
 of minimizing the number of False Positives that they return.
 
 METHODS: the methods for detecting smart feature all follow the same architecture with
 a first method to quantify the anomaly (as a real number) followed by a method to
 threshold it and return a boolean (qualitive).
-For example to detect if a method is blurry we call 
+For example to detect if a method is blurry we call
     blurriness = _blurry_laplace(image_gray)
     is_blurry = _is_blurry_laplace(blurriness)
 These methods are kept separate to allow easy generalization to the use-case where we
 compute the quantitative value first (the real-valued number, say via _blurry_laplace),
 store it, and compute the qualitive value (boolean) by thresholding later at different
 values (for example if we compute it at different prec/rec in the console).
 """
@@ -252,15 +254,15 @@
 ) -> np.ndarray:
     """
     Thresholding method associated to low_contrast_ranges
     """
     return q_max_over <= under_exposed_max_thresh
 
 
-def _blurry_laplace(image_gray: Image.Image) -> float:
+def _blurry_laplace(image_gray: Image) -> float:
     """
     Bluriness detector method where we compute the Variance of the Laplacian.
     We use PIL to estimate the Laplacian via the 3x3 convolution filter
     -1, -1, -1
     -1,  8, -1
     -1, -1, -1.
     A LARGE variance indicates a lot of edges and thus a sharp image, whereas a SMALL
@@ -280,15 +282,15 @@
 ) -> np.ndarray:
     """
     Thresholding method associated to blurry_laplace
     """
     return blurriness < blurry_thresh
 
 
-def _image_content_entropy(image: Image.Image) -> float:
+def _image_content_entropy(image: Image) -> float:
     """
     Returns the entropy of the pixels on the image. A high entropy means a more complex
     image with lots of variation in the pixel values (histogram closer to being uniform)
     whereas a low entropy means a simpler image with histogram more concentrated at a
     few specific intensities.
 
     There is no global threshold that will work for all images/datasets, experimentation
@@ -392,25 +394,25 @@
 def _is_near_duplicate(in_frame: DataFrame) -> np.ndarray:
     np_is_near_duplicate = in_frame.func.where(
         in_frame[CVSF.outlier_near_duplicate_id.value] == 0, False, True
     ).to_numpy()
     return np_is_near_duplicate
 
 
-def _open_and_resize(image_path: str) -> Tuple[Image.Image, Image.Image, np.ndarray]:
+def _open_and_resize(image_path: str) -> Tuple[Image, Image, np.ndarray]:
     """
     Open the image at the given path and return a triple with
     - the original image opened with PIL
     - the image converted to grey-scale with PIL
     - the numpy array of pixel intensities of the gray-scale image (as uint8)
 
     If any of the sides of the image is larger than 2**11, resize the image so that the
     largest side is now 2**11.
     """
-    image = Image.open(image_path)
+    image = Image_open(image_path)
     image_gray = image.convert(
         "L"
     )  # TODO: check if image already grey, faster to skip that ?
 
     # Resize for both blurriness detector and increasing speed for processing big images
     w, h = image_gray.size
     if min(w, h) > 2**11:
```

### Comparing `dataquality-2.0.1/dataquality/utils/dq_logger.py` & `dataquality-2.0.2/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/dqyolo.py` & `dataquality-2.0.2/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/emb.py` & `dataquality-2.0.2/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/file.py` & `dataquality-2.0.2/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/hdf5_store.py` & `dataquality-2.0.2/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/helpers.py` & `dataquality-2.0.2/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/hf_images.py` & `dataquality-2.0.2/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/hf_tokenizer.py` & `dataquality-2.0.2/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/jsl.py` & `dataquality-2.0.2/dataquality/utils/jsl.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/keras.py` & `dataquality-2.0.2/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/ml.py` & `dataquality-2.0.2/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/name.py` & `dataquality-2.0.2/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/od.py` & `dataquality-2.0.2/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/patcher.py` & `dataquality-2.0.2/dataquality/utils/patcher.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/profiler.py` & `dataquality-2.0.2/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-2.0.2/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-2.0.2/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-2.0.2/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from tempfile import NamedTemporaryFile
 from typing import List
 
 import numpy as np
 import torch
-from PIL import Image, ImageColor
+from PIL import ImageColor
+from PIL.Image import Image, fromarray
 
 from dataquality import config
 from dataquality.clients.objectstore import ObjectStore
 from dataquality.schemas.semantic_segmentation import (
     Polygon,
     SemSegMetricData,
     SemSegMetricType,
@@ -32,15 +33,15 @@
     Returns the dep_heatmaps
     """
     dep_heatmaps = calculate_dep_heatmaps(probs, gold_masks)
     write_dep_to_disk(dep_heatmaps, image_ids, local_folder_path)
     return dep_heatmaps
 
 
-def colorize_dep_heatmap(image: Image.Image, dep_mean: int) -> Image.Image:
+def colorize_dep_heatmap(image: Image, dep_mean: int) -> Image:
     """Recolors a grayscale image to a color image based on our dep mapping"""
     color_1 = ImageColor.getrgb("#9bc33f")  # Red
     color_2 = ImageColor.getrgb("#ece113")  # Yellow
     color_3 = ImageColor.getrgb("#ba3612")  # Green
 
     # Convert the image to RGB mode if needed
     if image.mode != "RGB":
@@ -58,15 +59,15 @@
     colorized_image[threshold_mask, 2] = (1 - ratio) * color_1[2] + ratio * color_2[2]
 
     ratio = ((image_np - dep_mean) / (255 - dep_mean))[~threshold_mask][:, 0]
     colorized_image[~threshold_mask, 0] = (1 - ratio) * color_2[0] + ratio * color_3[0]
     colorized_image[~threshold_mask, 1] = (1 - ratio) * color_2[1] + ratio * color_3[1]
     colorized_image[~threshold_mask, 2] = (1 - ratio) * color_2[2] + ratio * color_3[2]
 
-    return Image.fromarray(colorized_image.astype(np.uint8))
+    return fromarray(colorized_image.astype(np.uint8))
 
 
 def calculate_dep_heatmaps(
     probs: torch.Tensor, gold_masks: torch.Tensor
 ) -> torch.Tensor:
     """
     Calculates the Data Error Potential (DEP) for each image in the batch
@@ -162,15 +163,15 @@
     :param dep_heatmap: DEP heatmap for each image in the batch
         shape = (height, width)
     :return: PIL Image object
     """
     # Scale the array values to the range [0, 255]
     dep_heatmap = (dep_heatmap * 255).astype(np.uint8)
     # Create a PIL Image object from the numpy array as grey-scale
-    img = Image.fromarray(dep_heatmap, mode="L")
+    img = fromarray(dep_heatmap, mode="L")
     if img.size[0] > MAX_DEP_HEATMAP_SIZE or img.size[1] > MAX_DEP_HEATMAP_SIZE:
         img = img.resize((MAX_DEP_HEATMAP_SIZE, MAX_DEP_HEATMAP_SIZE))
     return img
 
 
 def compute_metric(
     pred_mask: np.ndarray,
```

### Comparing `dataquality-2.0.1/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-2.0.2/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-2.0.2/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/seq2seq/__init__.py` & `dataquality-2.0.2/dataquality/utils/seq2seq/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/seq2seq/data_error_potential.py` & `dataquality-2.0.2/dataquality/utils/seq2seq/data_error_potential.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/seq2seq/decoder_only.py` & `dataquality-2.0.2/dataquality/utils/seq2seq/decoder_only.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/seq2seq/generation.py` & `dataquality-2.0.2/dataquality/utils/seq2seq/generation.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/seq2seq/logprobs.py` & `dataquality-2.0.2/dataquality/utils/seq2seq/logprobs.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/seq2seq/offsets.py` & `dataquality-2.0.2/dataquality/utils/seq2seq/offsets.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/setfit.py` & `dataquality-2.0.2/dataquality/utils/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/thread_pool.py` & `dataquality-2.0.2/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/torch.py` & `dataquality-2.0.2/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/transformers.py` & `dataquality-2.0.2/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/ultralytics.py` & `dataquality-2.0.2/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/upload.py` & `dataquality-2.0.2/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/upload_model.py` & `dataquality-2.0.2/dataquality/utils/upload_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/vaex.py` & `dataquality-2.0.2/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/dataquality/utils/version.py` & `dataquality-2.0.2/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-2.0.1/pyproject.toml` & `dataquality-2.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dataquality"
-version = "2.0.1"
+version = "2.0.2"
 description = ""
 authors = ["Galileo Technologies, Inc. <team@rungalileo.io>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/rungalileo/dataquality"
 documentation = "https://rungalileo.gitbook.io/galileo"
 scripts = { dqyolo = "dataquality.dqyolo:main" }
@@ -45,33 +45,63 @@
 pyjwt = ">=2.8.0"
 peft = "*"
 # Pin opencv for linting incompatibility
 opencv-python = "<=4.8.1.78"
 pydantic-settings = ">=2.0.0"
 minio = {version = ">=7.1.0,<7.2.0", optional=true}
 setfit = {version ="==0.7.0", optional = true}
-
-# Cuda.
-ucx-py-cu11 = { version ="^0.36", source = "nvidia", optional = true }
-rmm-cu11 = {version = "^24.2.0", source = "nvidia", optional=true}
-raft-dask-cu11 = {version = "^24.2.0", source = "nvidia", optional=true}
-pylibraft-cu11 = {version = "^24.2.0", source = "nvidia", optional=true}
-dask-cudf-cu11 = {version = "^24.2.0", source = "nvidia", optional=true}
-cudf-cu11 = {version = "^24.2.0", source = "nvidia", optional=true}
-cuml-cu11 = {version = "^24.2.0", source = "nvidia", optional=true}
 sentencepiece = "^0.2.0"
 
+# cuda dependencies
+ucx-py-cu12 = { version ="^0.36", source = "nvidia", optional = true }
+rmm-cu12 = {version = "^24.2.0", source = "nvidia", optional=true}
+raft-dask-cu12 = {version = "^24.2.0", source = "nvidia", optional=true}
+pylibraft-cu12 = {version = "^24.2.0", source = "nvidia", optional=true}
+dask-cudf-cu12 = {version = "^24.2.0", source = "nvidia", optional=true}
+cudf-cu12 = {version = "^24.2.0", source = "nvidia", optional=true}
+cuml-cu12 = {version = "^24.2.0", source = "nvidia", optional=true}
+tensorflow = ">=2.9.1,<2.15.0"
+
+
+
+
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 invoke = ">=1.6.0"
 pre-commit = "^3.6.1"
 
 
 [tool.poetry.extras]
-cuda = ["ucx-py-cu11", "rmm-cu11", "raft-dask-cu11", "pylibraft-cu11", "dask-cudf-cu11", "cudf-cu11", "cuml-cu11"]
+cuda = [
+    "ucx-py-cu12",
+    "rmm-cu12",
+    "raft-dask-cu12",
+    "pylibraft-cu12",
+    "dask-cudf-cu12",
+    "cudf-cu12",
+    "cuml-cu12"
+]
+cuda11 = [
+    "ucx-py-cu11",
+    "rmm-cu11",
+    "raft-dask-cu11",
+    "pylibraft-cu11",
+    "dask-cudf-cu11",
+    "cudf-cu11", 
+    "cuml-cu11"
+]
+cuda12 = [
+    "ucx-py-cu12",
+    "rmm-cu12",
+    "raft-dask-cu12",
+    "pylibraft-cu12",
+    "dask-cudf-cu12",
+    "cudf-cu12",
+    "cuml-cu12"
+]
 minio = ["minio"]
 setfit = ["setfit"]
 
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2024.0.0"
 sphinx-autodoc-typehints = "^2.0.0"
@@ -84,15 +114,15 @@
 [tool.poetry.group.test.dependencies]
 ultralytics = ">=8.0.209"
 pytest = ">=7.2.1"
 freezegun = ">=1.2.2"
 coverage = { version = ">=7.0.5", extras = ["toml"] }
 pytest-cov = ">=4.0.0"
 scikit-learn = ">=1.0"
-tensorflow = ">=2.9.1"
+tensorflow = "<=2.15.0"
 pytest-env = ">=0.8.1"
 pytest-xdist = ">=2.4.0"
 types-setuptools = ">=67.3.0.1"
 types-cachetools = ">=4.2.4"
 torchvision = ">=0.13.1"
 torch = ">=1.12.1"
 torchtext = ">=0.13.1"
```

### Comparing `dataquality-2.0.1/PKG-INFO` & `dataquality-2.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 Home-page: https://github.com/rungalileo/dataquality
 License: Apache-2.0
 Author: Galileo Technologies, Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cuda
+Provides-Extra: cuda11
+Provides-Extra: cuda12
 Provides-Extra: minio
 Provides-Extra: setfit
 Requires-Dist: Pillow
 Requires-Dist: accelerate
 Requires-Dist: blake3 (>=0.2.1)
 Requires-Dist: cachetools (>=4.2.4)
-Requires-Dist: cudf-cu11 (>=24.2.0,<25.0.0) ; extra == "cuda"
-Requires-Dist: cuml-cu11 (>=24.2.0,<25.0.0) ; extra == "cuda"
-Requires-Dist: dask-cudf-cu11 (>=24.2.0,<25.0.0) ; extra == "cuda"
+Requires-Dist: cudf-cu12 (>=24.2.0,<25.0.0) ; extra == "cuda" or extra == "cuda12"
+Requires-Dist: cuml-cu12 (>=24.2.0,<25.0.0) ; extra == "cuda" or extra == "cuda12"
+Requires-Dist: dask-cudf-cu12 (>=24.2.0,<25.0.0) ; extra == "cuda" or extra == "cuda12"
 Requires-Dist: datasets (>=2.14.6)
 Requires-Dist: diskcache (>=5.2.1)
 Requires-Dist: evaluate
 Requires-Dist: h5py (>=3.1.0)
 Requires-Dist: imagededup (>=0.3.1,<0.3.2)
 Requires-Dist: importlib-metadata (<6.0.1)
 Requires-Dist: ipywidgets (>=8.1.0)
@@ -33,29 +35,30 @@
 Requires-Dist: opencv-python (<=4.8.1.78)
 Requires-Dist: pandas (>=0.20.0)
 Requires-Dist: peft
 Requires-Dist: pyarrow (>=5.0.0)
 Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: pydantic-settings (>=2.0.0)
 Requires-Dist: pyjwt (>=2.8.0)
-Requires-Dist: pylibraft-cu11 (>=24.2.0,<25.0.0) ; extra == "cuda"
-Requires-Dist: raft-dask-cu11 (>=24.2.0,<25.0.0) ; extra == "cuda"
+Requires-Dist: pylibraft-cu12 (>=24.2.0,<25.0.0) ; extra == "cuda" or extra == "cuda12"
+Requires-Dist: raft-dask-cu12 (>=24.2.0,<25.0.0) ; extra == "cuda" or extra == "cuda12"
 Requires-Dist: requests (>=2.25.1)
 Requires-Dist: resource (>=0.2.1)
-Requires-Dist: rmm-cu11 (>=24.2.0,<25.0.0) ; extra == "cuda"
+Requires-Dist: rmm-cu12 (>=24.2.0,<25.0.0) ; extra == "cuda" or extra == "cuda12"
 Requires-Dist: scipy (>=1.7.0)
 Requires-Dist: sentence-transformers (>=2.2)
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
 Requires-Dist: seqeval
 Requires-Dist: setfit (==0.7.0) ; extra == "setfit"
 Requires-Dist: tenacity (>=8.1.0)
+Requires-Dist: tensorflow (>=2.9.1,<2.15.0)
 Requires-Dist: tqdm (>=4.62.3)
 Requires-Dist: transformers (>=4.17.0)
 Requires-Dist: types-requests (>=2.25.2)
-Requires-Dist: ucx-py-cu11 (>=0.36,<0.37) ; extra == "cuda"
+Requires-Dist: ucx-py-cu12 (>=0.36,<0.37) ; extra == "cuda" or extra == "cuda12"
 Requires-Dist: vaex-core (==4.17.1)
 Requires-Dist: vaex-hdf5 (>=0.12,<0.13)
 Requires-Dist: wrapt (>=1.13.3)
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Description-Content-Type: text/markdown
 
 # dataquality
```

