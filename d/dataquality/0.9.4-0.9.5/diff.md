# Comparing `tmp/dataquality-0.9.4.tar.gz` & `tmp/dataquality-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.9.4.tar", last modified: Fri Jul  7 21:00:15 2023, max compression
+gzip compressed data, was "dataquality-0.9.5.tar", last modified: Mon Jul 10 15:11:28 2023, max compression
```

## Comparing `dataquality-0.9.4.tar` & `dataquality-0.9.5.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.110956 dataquality-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 20:58:05.000000 dataquality-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-07 21:00:15.110956 dataquality-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-07 20:58:05.000000 dataquality-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.038955 dataquality-0.9.4/dataquality/
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.042955 dataquality-0.9.4/dataquality/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/clients/objectstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.046955 dataquality-0.9.4/dataquality/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.050955 dataquality-0.9.4/dataquality/dq_auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.050955 dataquality-0.9.4/dataquality/dq_start/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.054955 dataquality-0.9.4/dataquality/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.054955 dataquality-0.9.4/dataquality/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/base_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.062955 dataquality-0.9.4/dataquality/loggers/data_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.070955 dataquality-0.9.4/dataquality/loggers/logger_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.074955 dataquality-0.9.4/dataquality/loggers/model_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.086955 dataquality-0.9.4/dataquality/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.102955 dataquality-0.9.4/dataquality/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/ampli.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/auto_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/dq_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/hdf5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/hf_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/od.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.102955 dataquality-0.9.4/dataquality/utils/semantic_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/vaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.038955 dataquality-0.9.4/dataquality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-07 20:58:05.000000 dataquality-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 21:00:15.110956 dataquality-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:58:05.000000 dataquality-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.106955 dataquality-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_dataquality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_telemetrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.110956 dataquality-0.9.4/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/ner_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/pt_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/tc_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.999847 dataquality-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 15:09:49.000000 dataquality-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-10 15:11:27.999847 dataquality-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-10 15:09:49.000000 dataquality-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.931845 dataquality-0.9.5/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.931845 dataquality-0.9.5/dataquality/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/clients/objectstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.935845 dataquality-0.9.5/dataquality/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/core/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.939845 dataquality-0.9.5/dataquality/dq_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_auto/text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.939845 dataquality-0.9.5/dataquality/dq_start/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dq_start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.943846 dataquality-0.9.5/dataquality/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/integrations/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.947846 dataquality-0.9.5/dataquality/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/base_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.951846 dataquality-0.9.5/dataquality/loggers/data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/data_logger/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.955846 dataquality-0.9.5/dataquality/loggers/logger_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/logger_config/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.959846 dataquality-0.9.5/dataquality/loggers/model_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.971846 dataquality-0.9.5/dataquality/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/schemas/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.987846 dataquality-0.9.5/dataquality/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/ampli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/auto_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/dq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/hdf5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/hf_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/od.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.991846 dataquality-0.9.5/dataquality/utils/semantic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/vaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 15:09:49.000000 dataquality-0.9.5/dataquality/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.931845 dataquality-0.9.5/dataquality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-10 15:11:27.000000 dataquality-0.9.5/dataquality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-10 15:11:27.000000 dataquality-0.9.5/dataquality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:11:27.000000 dataquality-0.9.5/dataquality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 15:11:27.000000 dataquality-0.9.5/dataquality.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-10 15:11:27.000000 dataquality-0.9.5/dataquality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 15:11:27.000000 dataquality-0.9.5/dataquality.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-10 15:09:49.000000 dataquality-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-10 15:11:27.999847 dataquality-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:09:49.000000 dataquality-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.991846 dataquality-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_dataquality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_telemetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:11:27.999847 dataquality-0.9.5/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/ner_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-10 15:09:49.000000 dataquality-0.9.5/tests/test_utils/tc_constants.py
```

### Comparing `dataquality-0.9.4/LICENSE` & `dataquality-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/PKG-INFO` & `dataquality-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.4
+Version: 0.9.5
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.4/README.md` & `dataquality-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/__init__.py` & `dataquality-0.9.5/dataquality/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
```

### Comparing `dataquality-0.9.4/dataquality/analytics.py` & `dataquality-0.9.5/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/clients/api.py` & `dataquality-0.9.5/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/clients/objectstore.py` & `dataquality-0.9.5/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/__init__.py` & `dataquality-0.9.5/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/_config.py` & `dataquality-0.9.5/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/auth.py` & `dataquality-0.9.5/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/finish.py` & `dataquality-0.9.5/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/init.py` & `dataquality-0.9.5/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/log.py` & `dataquality-0.9.5/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/core/report.py` & `dataquality-0.9.5/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/auto.py` & `dataquality-0.9.5/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.5/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/ner.py` & `dataquality-0.9.5/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.5/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/notebook.py` & `dataquality-0.9.5/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.5/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.5/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dq_start/__init__.py` & `dataquality-0.9.5/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/dqyolo.py` & `dataquality-0.9.5/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/fastai.py` & `dataquality-0.9.5/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/hf.py` & `dataquality-0.9.5/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/keras.py` & `dataquality-0.9.5/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/setfit.py` & `dataquality-0.9.5/dataquality/integrations/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/torch.py` & `dataquality-0.9.5/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-0.9.5/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/transformers_trainer.py` & `dataquality-0.9.5/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/integrations/ultralytics.py` & `dataquality-0.9.5/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/internal.py` & `dataquality-0.9.5/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/base_logger.py` & `dataquality-0.9.5/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/__init__.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/object_detection.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/seq2seq.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.5/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.5/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/logger_config/object_detection.py` & `dataquality-0.9.5/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/logger_config/seq2seq.py` & `dataquality-0.9.5/dataquality/loggers/logger_config/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.5/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.5/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.5/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/object_detection.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/seq2seq.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.5/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/metrics.py` & `dataquality-0.9.5/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/condition.py` & `dataquality-0.9.5/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/dataframe.py` & `dataquality-0.9.5/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/edit.py` & `dataquality-0.9.5/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/hf.py` & `dataquality-0.9.5/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/metrics.py` & `dataquality-0.9.5/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/ner.py` & `dataquality-0.9.5/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/report.py` & `dataquality-0.9.5/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/route.py` & `dataquality-0.9.5/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/semantic_segmentation.py` & `dataquality-0.9.5/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/seq2seq.py` & `dataquality-0.9.5/dataquality/schemas/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/split.py` & `dataquality-0.9.5/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/task_type.py` & `dataquality-0.9.5/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/schemas/torch.py` & `dataquality-0.9.5/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/ampli.py` & `dataquality-0.9.5/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/auto.py` & `dataquality-0.9.5/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/auto_trainer.py` & `dataquality-0.9.5/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/cuda.py` & `dataquality-0.9.5/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/cv.py` & `dataquality-0.9.5/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/dq_logger.py` & `dataquality-0.9.5/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/dqyolo.py` & `dataquality-0.9.5/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/emb.py` & `dataquality-0.9.5/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/file.py` & `dataquality-0.9.5/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/hdf5_store.py` & `dataquality-0.9.5/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/helpers.py` & `dataquality-0.9.5/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/hf_images.py` & `dataquality-0.9.5/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.5/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/keras.py` & `dataquality-0.9.5/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/ml.py` & `dataquality-0.9.5/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/name.py` & `dataquality-0.9.5/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/od.py` & `dataquality-0.9.5/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/patcher.py` & `dataquality-0.9.5/dataquality/utils/patcher.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/profiler.py` & `dataquality-0.9.5/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-0.9.5/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-0.9.5/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-0.9.5/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-0.9.5/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-0.9.5/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/seq2seq.py` & `dataquality-0.9.5/dataquality/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/setfit.py` & `dataquality-0.9.5/dataquality/utils/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/thread_pool.py` & `dataquality-0.9.5/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/torch.py` & `dataquality-0.9.5/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/transformers.py` & `dataquality-0.9.5/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/ultralytics.py` & `dataquality-0.9.5/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/upload.py` & `dataquality-0.9.5/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/vaex.py` & `dataquality-0.9.5/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality/utils/version.py` & `dataquality-0.9.5/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality.egg-info/PKG-INFO` & `dataquality-0.9.5/dataquality.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.4
+Version: 0.9.5
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.4/dataquality.egg-info/SOURCES.txt` & `dataquality-0.9.5/dataquality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/dataquality.egg-info/requires.txt` & `dataquality-0.9.5/dataquality.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pydantic>=1.8.2
+pydantic<2.0.0,>=1.8.2
 requests>=2.25.1
 types-requests>=2.25.2
 pandas>=0.20.0
 pyarrow>=5.0.0
 vaex-core==4.16.0
 vaex-hdf5<0.13,>=0.12
 diskcache>=5.2.1
```

### Comparing `dataquality-0.9.4/pyproject.toml` & `dataquality-0.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project]
 name = "dataquality"
 dynamic = ["version"]
 readme = "README.md"
 license = {text = 'See LICENSE'}
 requires-python = ">=3.7"
 dependencies = [
-    "pydantic>=1.8.2",
+    "pydantic>=1.8.2,<2.0.0",
     "requests>=2.25.1",
     "types-requests>=2.25.2",
     "pandas>=0.20.0",
     "pyarrow>=5.0.0",
     "vaex-core==4.16.0",
     "vaex-hdf5>=0.12,<0.13",
     "diskcache>=5.2.1",
```

### Comparing `dataquality-0.9.4/tests/test_dataquality.py` & `dataquality-0.9.5/tests/test_dataquality.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_telemetrics.py` & `dataquality-0.9.5/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/data_utils.py` & `dataquality-0.9.5/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.9.5/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.5/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.5/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/lightning_model.py` & `dataquality-0.9.5/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/mock_data.py` & `dataquality-0.9.5/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/mock_request.py` & `dataquality-0.9.5/tests/test_utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/ner_constants.py` & `dataquality-0.9.5/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/pt_datasets_mock.py` & `dataquality-0.9.5/tests/test_utils/pt_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.4/tests/test_utils/tc_constants.py` & `dataquality-0.9.5/tests/test_utils/tc_constants.py`

 * *Files identical despite different names*

