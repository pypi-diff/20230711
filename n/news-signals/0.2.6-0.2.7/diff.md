# Comparing `tmp/news-signals-0.2.6.tar.gz` & `tmp/news-signals-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.2.6.tar", last modified: Tue Jul  4 07:51:31 2023, max compression
+gzip compressed data, was "news-signals-0.2.7.tar", last modified: Tue Jul 11 08:22:31 2023, max compression
```

## Comparing `news-signals-0.2.6.tar` & `news-signals-0.2.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.108557 news-signals-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 07:51:19.000000 news-signals-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 07:51:19.000000 news-signals-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 07:51:31.108557 news-signals-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-04 07:51:19.000000 news-signals-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 07:51:19.000000 news-signals-0.2.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.104557 news-signals-0.2.6/news_signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/wikidata_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/yfinance_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.104557 news-signals-0.2.6/news_signals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.100557 news-signals-0.2.6/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.104557 news-signals-0.2.6/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/elon_musk_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100.small.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.108557 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/politics_china_australia_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/sample_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/tesla_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:51:31.108557 news-signals-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-04 07:51:19.000000 news-signals-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.806055 news-signals-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 08:22:21.000000 news-signals-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 08:22:21.000000 news-signals-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-11 08:22:31.806055 news-signals-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-11 08:22:21.000000 news-signals-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 08:22:21.000000 news-signals-0.2.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.802055 news-signals-0.2.7/news_signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/wikidata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/yfinance_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.802055 news-signals-0.2.7/news_signals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.798055 news-signals-0.2.7/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.802055 news-signals-0.2.7/resources/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/elon_musk_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100.small.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.806055 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/politics_china_australia_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/sample_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/tesla_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:22:31.806055 news-signals-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-11 08:22:21.000000 news-signals-0.2.7/setup.py
```

### Comparing `news-signals-0.2.6/LICENSE` & `news-signals-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/PKG-INFO` & `news-signals-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
 ### Example Colab Notebooks
```

### Comparing `news-signals-0.2.6/README.md` & `news-signals-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/anomaly_detection.py` & `news-signals-0.2.7/news_signals/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/aql_builder.py` & `news-signals-0.2.7/news_signals/aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/dataset_transformations.py` & `news-signals-0.2.7/news_signals/dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/exogenous_signals.py` & `news-signals-0.2.7/news_signals/exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/newsapi.py` & `news-signals-0.2.7/news_signals/newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/plotting.py` & `news-signals-0.2.7/news_signals/plotting.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/representative_story.py` & `news-signals-0.2.7/news_signals/representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/signals.py` & `news-signals-0.2.7/news_signals/signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/signals_dataset.py` & `news-signals-0.2.7/news_signals/signals_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from copy import deepcopy
 
 import appdirs
 import arrow
 import gdown
 import pandas as pd
 import tqdm
-from google.cloud import storage
 
 import news_signals.signals as signals
 import news_signals.newsapi as newsapi
-from news_signals.data import aylien_ts_to_df, arrow_to_aylien_date
+from news_signals.data import (aylien_ts_to_df, arrow_to_aylien_date,
+                               load_from_gcs, save_to_gcs)
 from news_signals.aql_builder import params_to_aql
 from news_signals.log import create_logger
 
 
 logger = create_logger(__name__, level=logging.INFO)
 
 MAX_BODY_TOKENS = 500
@@ -30,15 +30,15 @@
     'name': 'News Signals Dataset'
 }
 
 
 class SignalsDataset:
     DEFAULT_CACHE_DIR = Path(appdirs.user_cache_dir('news-signals/datasets'))
 
-    def __init__(self, signals=None, metadata=None, cache_dir=None):
+    def __init__(self, signals=None, metadata=None):
         if metadata is None:
             metadata = {
                 # default dataset name
                 'name': 'News Signals Dataset'
             }
         else:
             assert 'name' in metadata, 'Dataset metadata must specify a name.'
@@ -59,14 +59,16 @@
     def load(cls, dataset_path, cache_dir=None):       
         # handle downloading from urls
         if type(dataset_path) is str \
             and (dataset_path.startswith('https://drive.google.com') or dataset_path.startswith('gs://')):
             basename = base64.b64encode(dataset_path.encode()).decode()
             if cache_dir is None:
                 cache_dir = cls.DEFAULT_CACHE_DIR
+            else:
+                cache_dir = Path(cache_dir)
 
             local_dataset_dir = cache_dir / basename
             if not local_dataset_dir.exists():
                 if dataset_path.startswith('https://drive.google.com'):
                     # folder vs file download from gdrive
                     if 'folders' in dataset_path:
                         local_dataset_dir = Path(cache_dir) / basename
@@ -84,22 +86,22 @@
                         status = gdown.download(url=dataset_path, output=str(local_dataset_path))
                         assert status is not None, 'Download as file failed.'
                         dataset_path = local_dataset_path
                 elif dataset_path.startswith('gs://'):
                     assert dataset_path.endswith('.tar.gz'), \
                         'Datasets stored in GCS currently must be in .tar.gz format'
                     local_dataset_path = Path(str(local_dataset_dir) + '.tar.gz')
-                    gcs_client = storage.Client()
                     bucket_name, blob_name = dataset_path.replace("gs://", "").split("/", 1)
-                    bucket = gcs_client.bucket(bucket_name)
-                    blob = bucket.blob(blob_name)
                     ds_cache_dir = Path(os.path.dirname(local_dataset_path))
                     ds_cache_dir.mkdir(parents=True, exist_ok=True)
-                    blob.download_to_filename(str(local_dataset_path))
-                    print(f'GCS blob {blob_name} downloaded to {local_dataset_path}.')
+                    load_from_gcs(
+                        bucket_name=bucket_name,
+                        blob_name=blob_name, 
+                        local_dataset_path=local_dataset_path
+                    )
                     dataset_path = local_dataset_path
             else:
                 logger.info(f'Using cached dataset at {local_dataset_dir}.') 
                 dataset_path = local_dataset_dir
 
         # handle decompressing tar.gz
         dataset_path = Path(dataset_path)
@@ -155,34 +157,26 @@
                 base_dir=dataset_path.name,
                 format='gztar'
             )
             if dataset_path.exists():
                 shutil.rmtree(dataset_path)
             logger.info(f'Saved compressed dataset to {dataset_path}.tar.gz')
             if gcs_bucket_name is not None:
-                self.upload_to_gcs(
+                save_to_gcs(
                     bucket_name=gcs_bucket_name,
                     source_file_name=f'{dataset_path}.tar.gz',
                     destination_blob_name=f'{dataset_path.name}.tar.gz'
                 )
             return f'{dataset_path}.tar.gz'
         else:
             logger.info(
                 f'Saved {len(self.signals)} signals in dataset to {dataset_path}.'
             )
             return dataset_path
     
-    @staticmethod
-    def upload_to_gcs(bucket_name, source_file_name, destination_blob_name):
-        gcs_client = storage.Client()
-        bucket = gcs_client.get_bucket(bucket_name)
-        blob = bucket.blob(destination_blob_name)
-        blob.upload_from_filename(source_file_name)
-        logger.info(f"File {source_file_name} uploaded to gs://{bucket_name}/{destination_blob_name}.")
-    
     def aggregate_signal(self, name=None):
         if name is None:
             name = self.metadata['name']
         return signals.AggregateSignal(
             name=name,
             components=list(self.signals.values())
         )
```

### Comparing `news-signals-0.2.6/news_signals/summarization.py` & `news-signals-0.2.7/news_signals/summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_anomaly_detection.py` & `news-signals-0.2.7/news_signals/test_anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_aql_builder.py` & `news-signals-0.2.7/news_signals/test_aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_data.py` & `news-signals-0.2.7/news_signals/test_data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_dataset_transformations.py` & `news-signals-0.2.7/news_signals/test_dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_exogenous_signals.py` & `news-signals-0.2.7/news_signals/test_exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_newsapi.py` & `news-signals-0.2.7/news_signals/test_newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_representative_story.py` & `news-signals-0.2.7/news_signals/test_representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_signals.py` & `news-signals-0.2.7/news_signals/test_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/test_signals_dataset.py` & `news-signals-0.2.7/news_signals/test_signals_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import datetime
 import base64
 from pathlib import Path
 
 import arrow
 import pandas as pd
 
+import news_signals.data as news_signals_data
 from news_signals.data import datetime_to_aylien_str
 from news_signals.log import create_logger
 from news_signals import signals, test_signals
 from news_signals import signals_dataset
 from news_signals.signals_dataset import SignalsDataset
 
 
@@ -96,14 +97,15 @@
         if self.output_dataset_dir.exists():
             shutil.rmtree(self.output_dataset_dir)
     
     def generate_sample_dataset(self):
         signals_dataset.generate_dataset(
             input=Path(self.input_csv),
             output_dataset_dir=Path(self.output_dataset_dir),
+            gcs_bucket=None,
             start=datetime.datetime(2023, 1, 1),
             end=datetime.datetime(2023, 1, 4),
             id_field="Wikidata ID",
             name_field="Wikidata Label",
             delete_tmp_files=True,
             stories_endpoint=self.stories_endpoint,
             ts_endpoint=self.ts_endpoint,
@@ -150,14 +152,15 @@
             name=name,
             params=params
         )
   
         signals_dataset.generate_dataset(
             input=[signal],
             output_dataset_dir=Path(self.output_dataset_dir),
+            gcs_bucket=None,
             start=start,
             end=end,
             stories_per_day=50,
             delete_tmp_files=True,
             stories_endpoint=self.stories_endpoint,
             ts_endpoint=self.ts_endpoint,
             compress=False
@@ -180,14 +183,19 @@
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
 
     @classmethod
     def tearDownClass(cls):
         pass
+
+    def tearDown(self):
+        tmp_dir = '/tmp/test_signals_dataset'
+        if Path(tmp_dir).exists():
+            shutil.rmtree(tmp_dir)
     
     def test_signals_dataset_dict_interface(self):
         """
         test that signals can be stored in a dataset
         and retrieved by index
         """
         aylien_signals = self.aylien_signals()
@@ -220,15 +228,14 @@
         d1 = SignalsDataset(self.aylien_signals())
         tmp_dir = Path('/tmp/test_signals_dataset')
         d1.save(tmp_dir, compress=False)
         d2 = SignalsDataset.load(tmp_dir)
         for k in d1:
             assert d1[k].name == d2[k].name
         assert json.dumps(d1.metadata) == json.dumps(d2.metadata)
-        shutil.rmtree(tmp_dir)
 
     def test_save_to_gcs(self):
         d1 = SignalsDataset(self.aylien_signals())
         tmp_dir = Path('/tmp/test_signals_dataset')
         fake_gcs_bucket = 'fake-path'
         
         class upload_from_filename:
@@ -247,16 +254,16 @@
                         self.path = path
                         self.upload_from_filename = upload_from_filename()
                         return self
                 self.get_bucket = get_bucket 
                 return self
         
         mock_storage = MockGCStorage()
-        signals_dataset.storage = mock_storage
-        save_path = d1.save(tmp_dir, compress=True, gcs_bucket_name=fake_gcs_bucket)
+        news_signals_data.storage = mock_storage
+        save_path = d1.save(tmp_dir, compress=True, overwrite=True, gcs_bucket_name=fake_gcs_bucket)
         assert upload_from_filename.args[0] == save_path
     
     def test_load_from_url(self):
         cache_dir = Path('/tmp/test_signals_dataset')
         cache_dir.mkdir(parents=True)
         fake_gdrive_path = 'https://drive.google.com/fake-path'
         basename = base64.b64encode(fake_gdrive_path.encode()).decode()
@@ -289,27 +296,27 @@
                     def blob(self, path):
                         self.path = path
                         self.download_to_filename = download_to_filename()
                         return self
                 self.bucket = bucket 
                 return self
         
-        signals_dataset.storage = MockGCStorage()
+        news_signals_data.storage = MockGCStorage()
         fake_gcs_path = 'gs://fake-path/dataset.tar.gz'
         basename = base64.b64encode(fake_gcs_path.encode()).decode()
         with self.assertRaises(FileNotFoundError):
             _ = SignalsDataset.load(fake_gcs_path, cache_dir=cache_dir)
             assert download_to_filename.args[0] == cache_dir / basename + '.tar.gz'
+        shutil.rmtree(cache_dir)
 
     def test_plot_dataset(self):
         dataset = SignalsDataset(self.aylien_signals())
         savedir = Path('/tmp/test_plot_dataset')
         dataset.plot(savedir=savedir)
         assert os.path.exists(savedir / f'{dataset.metadata["name"]}.png')
-        shutil.rmtree(savedir)
     
     def test_corr(self):
         dataset = SignalsDataset(self.aylien_signals())
         corr = dataset.corr()
         assert corr.shape == (len(dataset), len(dataset))
     
     def test_transform_dataset_signals(self):
```

### Comparing `news-signals-0.2.6/news_signals/test_summarization.py` & `news-signals-0.2.7/news_signals/test_summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/users.py` & `news-signals-0.2.7/news_signals/users.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/wikidata_utils.py` & `news-signals-0.2.7/news_signals/wikidata_utils.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals/yfinance_timeseries.py` & `news-signals-0.2.7/news_signals/yfinance_timeseries.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/news_signals.egg-info/PKG-INFO` & `news-signals-0.2.7/news_signals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
 ### Example Colab Notebooks
```

### Comparing `news-signals-0.2.6/news_signals.egg-info/SOURCES.txt` & `news-signals-0.2.7/news_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/elon_musk_timeseries.json` & `news-signals-0.2.7/resources/test/elon_musk_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/politics_china_australia_timeseries.json` & `news-signals-0.2.7/resources/test/politics_china_australia_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/sample_stories.json` & `news-signals-0.2.7/resources/test/sample_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/resources/test/tesla_stories.json` & `news-signals-0.2.7/resources/test/tesla_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.6/setup.py` & `news-signals-0.2.7/setup.py`

 * *Files identical despite different names*

