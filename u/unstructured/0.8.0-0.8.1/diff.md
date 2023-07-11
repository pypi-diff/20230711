# Comparing `tmp/unstructured-0.8.0.tar.gz` & `tmp/unstructured-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.0.tar", last modified: Fri Jul  7 15:46:52 2023, max compression
+gzip compressed data, was "unstructured-0.8.1.tar", last modified: Tue Jul 11 14:37:58 2023, max compression
```

## Comparing `unstructured-0.8.0.tar` & `unstructured-0.8.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.844953 unstructured-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-07 15:46:44.000000 unstructured-0.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 15:46:44.000000 unstructured-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19205 2023-07-07 15:46:52.844953 unstructured-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-07 15:46:44.000000 unstructured-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.828952 unstructured-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-07 15:46:52.844953 unstructured-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 15:46:44.000000 unstructured-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.828952 unstructured-0.8.0/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.828952 unstructured-0.8.0/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.832953 unstructured-0.8.0/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.832953 unstructured-0.8.0/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28317 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.840953 unstructured-0.8.0/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.844953 unstructured-0.8.0/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.844953 unstructured-0.8.0/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.832953 unstructured-0.8.0/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19205 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.559194 unstructured-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-11 14:37:48.000000 unstructured-0.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 14:37:48.000000 unstructured-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-07-11 14:37:58.559194 unstructured-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-11 14:37:48.000000 unstructured-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.543195 unstructured-0.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 14:37:48.000000 unstructured-0.8.1/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-11 14:37:58.559194 unstructured-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-11 14:37:48.000000 unstructured-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.543195 unstructured-0.8.1/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.543195 unstructured-0.8.1/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-11 14:37:48.000000 unstructured-0.8.1/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 14:37:48.000000 unstructured-0.8.1/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-11 14:37:48.000000 unstructured-0.8.1/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-11 14:37:48.000000 unstructured-0.8.1/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.547195 unstructured-0.8.1/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.547195 unstructured-0.8.1/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.551195 unstructured-0.8.1/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.551195 unstructured-0.8.1/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.551195 unstructured-0.8.1/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.551195 unstructured-0.8.1/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.551195 unstructured-0.8.1/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28349 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.551195 unstructured-0.8.1/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.555194 unstructured-0.8.1/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.559194 unstructured-0.8.1/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14978 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.559194 unstructured-0.8.1/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-11 14:37:48.000000 unstructured-0.8.1/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:37:58.547195 unstructured-0.8.1/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-07-11 14:37:58.000000 unstructured-0.8.1/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-11 14:37:58.000000 unstructured-0.8.1/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:37:58.000000 unstructured-0.8.1/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 14:37:58.000000 unstructured-0.8.1/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 14:37:58.000000 unstructured-0.8.1/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 14:37:58.000000 unstructured-0.8.1/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.0/LICENSE.md` & `unstructured-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/MANIFEST.in` & `unstructured-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/PKG-INFO` & `unstructured-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.0
+Version: 0.8.1
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -296,14 +296,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.0 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.1 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -201,14 +201,15 @@
 Unstructured | Keywords: NLP PDF HTML CV XML parsing preprocessing Platform:
 UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
-Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
-discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
-Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
-Provides-Extra: gcs Provides-Extra: elasticsearch Provides-Extra: dropbox
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
+text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
+Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
+Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
+slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-Extra:
+gcs Provides-Extra: elasticsearch Provides-Extra: dropbox
```

### Comparing `unstructured-0.8.0/README.md` & `unstructured-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/setup.py` & `unstructured-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     author="Unstructured Technologies",
     author_email="devops@unstructuredai.io",
     license="Apache-2.0",
     packages=find_packages(),
     version=__version__,
```

### Comparing `unstructured-0.8.0/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.1/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.1/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/test_unstructured/test_utils.py` & `unstructured-0.8.1/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/cleaners/core.py` & `unstructured-0.8.1/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/cleaners/extract.py` & `unstructured-0.8.1/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/cleaners/translate.py` & `unstructured-0.8.1/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/documents/base.py` & `unstructured-0.8.1/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/documents/coordinates.py` & `unstructured-0.8.1/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/documents/elements.py` & `unstructured-0.8.1/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/documents/email_elements.py` & `unstructured-0.8.1/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/documents/html.py` & `unstructured-0.8.1/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/documents/xml.py` & `unstructured-0.8.1/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/file_utils/encoding.py` & `unstructured-0.8.1/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/file_utils/exploration.py` & `unstructured-0.8.1/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.1/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/file_utils/filetype.py` & `unstructured-0.8.1/unstructured/file_utils/filetype.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
 ) -> List[Element]:
     """Converts a DocumentLayout object to a list of unstructured elements."""
     elements: List[Element] = []
     num_pages = len(document.pages)
     for i, page in enumerate(document.pages):
         page_elements: List[Element] = []
         for layout_element in page.elements:
-            if hasattr(page, "image"):
+            if hasattr(page, "image") and hasattr(layout_element, "coordinates"):
                 image_format = page.image.format
                 coordinate_system = PixelSpace(width=page.image.width, height=page.image.height)
             else:
                 image_format = None
                 coordinate_system = None
             element = normalize_layout_element(layout_element, coordinate_system=coordinate_system)
             if isinstance(element, List):
```

### Comparing `unstructured-0.8.0/unstructured/file_utils/metadata.py` & `unstructured-0.8.1/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/azure.py` & `unstructured-0.8.1/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.1/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/discord.py` & `unstructured-0.8.1/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/dropbox.py` & `unstructured-0.8.1/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.8.1/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.1/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.1/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/git.py` & `unstructured-0.8.1/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/github.py` & `unstructured-0.8.1/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.1/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.1/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/local.py` & `unstructured-0.8.1/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/reddit.py` & `unstructured-0.8.1/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/s3.py` & `unstructured-0.8.1/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/slack.py` & `unstructured-0.8.1/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.8.1/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.1/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/interfaces.py` & `unstructured-0.8.1/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/ingest/main.py` & `unstructured-0.8.1/unstructured/ingest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             initargs=(logging.DEBUG if self.verbose else logging.INFO,),
         ) as pool:
             pool.map(self.doc_processor_fn, docs)
 
         self.cleanup()
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.pass_context
 @click.option(
     "--max-docs",
     default=None,
     type=int,
     help="If specified, process at most specified number of documents.",
 )
@@ -863,8 +863,8 @@
         reprocess=reprocess,
         verbose=verbose,
         max_docs=max_docs,
     ).run()
 
 
 if __name__ == "__main__":
-    main()
+    main()  # type: ignore
```

### Comparing `unstructured-0.8.0/unstructured/nlp/english-words.txt` & `unstructured-0.8.1/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/nlp/english_words.py` & `unstructured-0.8.1/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/nlp/patterns.py` & `unstructured-0.8.1/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/nlp/tokenize.py` & `unstructured-0.8.1/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/__init__.py` & `unstructured-0.8.1/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/api.py` & `unstructured-0.8.1/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/auto.py` & `unstructured-0.8.1/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/common.py` & `unstructured-0.8.1/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/csv.py` & `unstructured-0.8.1/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/doc.py` & `unstructured-0.8.1/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/docx.py` & `unstructured-0.8.1/unstructured/partition/docx.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,16 +144,16 @@
 
     headers_and_footers = _get_headers_and_footers(document, metadata_filename)
     if len(headers_and_footers) > 0:
         elements.extend(headers_and_footers[0][0])
 
     document_contains_pagebreaks = _element_contains_pagebreak(document._element)
     page_number = 1 if document_contains_pagebreaks else None
-
     section = 0
+    is_list = False
     for element_item in document.element.body:
         if element_item.tag.endswith("tbl"):
             table = document.tables[table_index]
             html_table = convert_ms_office_table_to_text(table, as_html=True)
             text_table = convert_ms_office_table_to_text(table, as_html=False)
             element = Table(text_table)
             if element is not None:
@@ -161,22 +161,25 @@
                     text_as_html=html_table,
                     filename=metadata_filename,
                     page_number=page_number,
                 )
                 elements.append(element)
             table_index += 1
         elif element_item.tag.endswith("p"):
+            if "<w:numPr>" in element_item.xml:
+                is_list = True
             paragraph = docx.text.paragraph.Paragraph(element_item, document)
-            para_element: Optional[Text] = _paragraph_to_element(paragraph)
+            para_element: Optional[Text] = _paragraph_to_element(paragraph, is_list)
             if para_element is not None:
                 para_element.metadata = ElementMetadata(
                     filename=metadata_filename,
                     page_number=page_number,
                 )
                 elements.append(para_element)
+            is_list = False
         elif element_item.tag.endswith("sectPr"):
             if len(headers_and_footers) > section:
                 footers = headers_and_footers[section][1]
                 elements.extend(footers)
 
             section += 1
             if len(headers_and_footers) > section:
@@ -187,29 +190,34 @@
             page_number += 1
             if include_page_breaks:
                 elements.append(PageBreak(text=""))
 
     return elements
 
 
-def _paragraph_to_element(paragraph: docx.text.paragraph.Paragraph) -> Optional[Text]:
+def _paragraph_to_element(
+    paragraph: docx.text.paragraph.Paragraph,
+    is_list=False,
+) -> Optional[Text]:
     """Converts a docx Paragraph object into the appropriate unstructured document element.
     If the paragraph style is "Normal" or unknown, we try to predict the element type from the
     raw text."""
     text = paragraph.text
     style_name = paragraph.style and paragraph.style.name  # .style can be None
 
     if len(text.strip()) == 0:
         return None
 
     element_class = STYLE_TO_ELEMENT_MAPPING.get(style_name)
 
     # NOTE(robinson) - The "Normal" style name will return None since it's in the mapping.
     # Unknown style names will also return None
-    if element_class is None:
+    if is_list:
+        return _text_to_element(text, is_list)
+    elif element_class is None:
         return _text_to_element(text)
     else:
         return element_class(text)
 
 
 def _element_contains_pagebreak(element) -> bool:
     """Detects if an element contains a page break. Checks for both "hard" page breaks
@@ -223,17 +231,17 @@
     if hasattr(element, "xml"):
         for indicators in page_break_indicators:
             if all(indicator in element.xml for indicator in indicators):
                 return True
     return False
 
 
-def _text_to_element(text: str) -> Optional[Text]:
+def _text_to_element(text: str, is_list=False) -> Optional[Text]:
     """Converts raw text into an unstructured Text element."""
-    if is_bulleted_text(text):
+    if is_bulleted_text(text) or is_list:
         clean_text = clean_bullets(text).strip()
         return ListItem(text=clean_bullets(text)) if clean_text else None
 
     elif is_us_city_state_zip(text):
         return Address(text=text)
 
     if len(text) < 2:
```

### Comparing `unstructured-0.8.0/unstructured/partition/email.py` & `unstructured-0.8.1/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/epub.py` & `unstructured-0.8.1/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/html.py` & `unstructured-0.8.1/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/image.py` & `unstructured-0.8.1/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/json.py` & `unstructured-0.8.1/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/md.py` & `unstructured-0.8.1/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/msg.py` & `unstructured-0.8.1/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/odt.py` & `unstructured-0.8.1/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/org.py` & `unstructured-0.8.1/unstructured/partition/org.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/pdf.py` & `unstructured-0.8.1/unstructured/partition/pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,26 @@
         infer_table_structure=infer_table_structure,
         ocr_languages=ocr_languages,
         max_partition=max_partition,
         **kwargs,
     )
 
 
+def extractable_elements(
+    filename: str = "",
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
+    include_page_breaks: bool = False,
+):
+    return _partition_pdf_with_pdfminer(
+        filename=filename,
+        file=file,
+        include_page_breaks=include_page_breaks,
+    )
+
+
 def partition_pdf_or_image(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     is_image: bool = False,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
@@ -107,20 +119,33 @@
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     # TODO(alan): Extract information about the filetype to be processed from the template
     # route. Decoding the routing should probably be handled by a single function designed for
     # that task so as routing design changes, those changes are implemented in a single
     # function.
 
+    if not is_image:
+        extracted_elements = extractable_elements(
+            filename=filename,
+            file=spooled_to_bytes_io_if_needed(file),
+            include_page_breaks=include_page_breaks,
+        )
+        pdf_text_extractable = any(
+            isinstance(el, Text) and el.text.strip() for el in extracted_elements
+        )
+    else:
+        pdf_text_extractable = False
+
     strategy = determine_pdf_or_image_strategy(
         strategy,
         filename=filename,
         file=file,
         is_image=is_image,
         infer_table_structure=infer_table_structure,
+        pdf_text_extractable=pdf_text_extractable,
     )
 
     if strategy == "hi_res":
         # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             layout_elements = _partition_pdf_or_image_local(
@@ -130,19 +155,15 @@
                 infer_table_structure=infer_table_structure,
                 include_page_breaks=include_page_breaks,
                 ocr_languages=ocr_languages,
                 **kwargs,
             )
 
     elif strategy == "fast":
-        return _partition_pdf_with_pdfminer(
-            filename=filename,
-            file=spooled_to_bytes_io_if_needed(file),
-            include_page_breaks=include_page_breaks,
-        )
+        return extracted_elements
 
     elif strategy == "ocr_only":
         # NOTE(robinson): Catches file conversion warnings when running with PDFs
         with warnings.catch_warnings():
             return _partition_pdf_or_image_with_ocr(
                 filename=filename,
                 file=file,
@@ -301,20 +322,24 @@
                 _text = _extract_text(obj)
                 _text_snippets = re.split(PARAGRAPH_PATTERN, _text)
 
             for _text in _text_snippets:
                 _text = clean_extra_whitespace(_text)
                 if _text.strip():
                     text_segments.append(_text)
-                    element = element_from_text(_text)
                     coordinate_system = PixelSpace(
                         width=width,
                         height=height,
                     )
                     points = ((x1, y1), (x1, y2), (x2, y2), (x2, y1))
+                    element = element_from_text(
+                        _text,
+                        coordinates=points,
+                        coordinate_system=coordinate_system,
+                    )
                     coordinates_metadata = CoordinatesMetadata(
                         points=points,
                         system=coordinate_system,
                     )
                     element.metadata = ElementMetadata(
                         filename=filename,
                         page_number=i + 1,
```

### Comparing `unstructured-0.8.0/unstructured/partition/ppt.py` & `unstructured-0.8.1/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/pptx.py` & `unstructured-0.8.1/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/rst.py` & `unstructured-0.8.1/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/rtf.py` & `unstructured-0.8.1/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/strategies.py` & `unstructured-0.8.1/unstructured/partition/strategies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from tempfile import SpooledTemporaryFile
-from typing import BinaryIO, Dict, List, Optional, Union, cast
-
-from pdfminer.pdfpage import PDFPage, PDFTextExtractionNotAllowed
-from pdfminer.utils import open_filename
+from typing import BinaryIO, Dict, List, Optional, Union
 
 from unstructured.logger import logger
-from unstructured.partition.common import exactly_one
 from unstructured.utils import dependency_exists
 
 VALID_STRATEGIES: Dict[str, List[str]] = {
     "auto": [
         "pdf",
         "image",
     ],
@@ -32,45 +28,21 @@
     valid_filetypes = VALID_STRATEGIES.get(strategy, None)
     if valid_filetypes is None:
         raise ValueError(f"{strategy} is not a valid strategy.")
     if filetype not in valid_filetypes:
         raise ValueError(f"{strategy} is not a valid strategy for filetype {filetype}.")
 
 
-def is_pdf_text_extractable(
-    filename: str = "",
-    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
-):
-    """Checks to see if the text from a PDF document is extractable. Sometimes the
-    text is not extractable due to PDF security settings."""
-    exactly_one(filename=filename, file=file)
-
-    def _fp_is_extractable(fp):
-        try:
-            next(PDFPage.get_pages(fp, check_extractable=True))
-            extractable = True
-        except PDFTextExtractionNotAllowed:
-            extractable = False
-        return extractable
-
-    if filename:
-        with open_filename(filename, "rb") as fp:
-            fp = cast(BinaryIO, fp)
-            return _fp_is_extractable(fp)
-    elif file:
-        fp = cast(BinaryIO, file)
-        return _fp_is_extractable(fp)
-
-
 def determine_pdf_or_image_strategy(
     strategy: str,
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     is_image: bool = False,
     infer_table_structure: bool = False,
+    pdf_text_extractable: bool = True,
 ):
     """Determines what strategy to use for processing PDFs or images, accounting for fallback
     logic if some dependencies are not available."""
     pytesseract_installed = dependency_exists("pytesseract")
     unstructured_inference_installed = dependency_exists("unstructured_inference")
 
     if is_image:
@@ -79,15 +51,14 @@
         # This can be removed once unstructured-api use auto as the default strategy.
         if strategy == "fast":
             strategy = "ocr_only"
         validate_strategy(strategy, "image")
         pdf_text_extractable = False
     else:
         validate_strategy(strategy, "pdf")
-        pdf_text_extractable = is_pdf_text_extractable(filename=filename, file=file)
 
     if strategy == "auto":
         if is_image:
             strategy = _determine_image_auto_strategy(infer_table_structure=infer_table_structure)
         else:
             strategy = _determine_pdf_auto_strategy(
                 pdf_text_extractable=pdf_text_extractable,
```

### Comparing `unstructured-0.8.0/unstructured/partition/text.py` & `unstructured-0.8.1/unstructured/partition/text.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
-from typing import IO, Callable, List, Optional
+from typing import IO, Callable, List, Optional, Tuple
 
 from unstructured.cleaners.core import clean_bullets, group_broken_paragraphs
+from unstructured.documents.coordinates import CoordinateSystem
 from unstructured.documents.elements import (
     Address,
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Text,
@@ -139,18 +140,30 @@
             element = element_from_text(ctext)
             element.metadata = metadata
             elements.append(element)
 
     return elements
 
 
-def element_from_text(text: str) -> Element:
+def element_from_text(
+    text: str,
+    coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
+    coordinate_system: Optional[CoordinateSystem] = None,
+) -> Element:
     if is_bulleted_text(text):
-        return ListItem(text=clean_bullets(text))
+        return ListItem(
+            text=clean_bullets(text),
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     elif is_us_city_state_zip(text):
-        return Address(text=text)
+        return Address(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
     elif is_possible_narrative_text(text):
-        return NarrativeText(text=text)
+        return NarrativeText(
+            text=text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     elif is_possible_title(text):
-        return Title(text=text)
+        return Title(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
     else:
-        return Text(text=text)
+        return Text(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
```

### Comparing `unstructured-0.8.0/unstructured/partition/text_type.py` & `unstructured-0.8.1/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/tsv.py` & `unstructured-0.8.1/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/xlsx.py` & `unstructured-0.8.1/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/partition/xml.py` & `unstructured-0.8.1/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/argilla.py` & `unstructured-0.8.1/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/base.py` & `unstructured-0.8.1/unstructured/staging/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,35 @@
     CheckBox,
     Element,
     ElementMetadata,
     NoID,
 )
 from unstructured.partition.common import exactly_one
 
+
+def _get_metadata_table_fieldnames():
+    metadata_fields = list(ElementMetadata.__annotations__.keys())
+    metadata_fields.remove("coordinates")
+    metadata_fields.extend(
+        [
+            "sender",
+            "coordinates_points",
+            "coordinates_system",
+            "coordinates_layout_width",
+            "coordinates_layout_height",
+        ],
+    )
+    return metadata_fields
+
+
 TABLE_FIELDNAMES: List[str] = [
     "type",
     "text",
     "element_id",
-    "coordinates_points",
-    "coordinates_system",
-    "coordinates_layout_width",
-    "coordinates_layout_height",
-    "filename",
-    "page_number",
-    "url",
-    "sent_from",
-    "sent_to",
-    "subject",
-    "sender",
-]
+] + _get_metadata_table_fieldnames()
 
 
 def convert_to_isd(elements: List[Element]) -> List[Dict[str, Any]]:
     """Represents the document elements as an Initial Structured Document (ISD)."""
     isd: List[Dict[str, str]] = []
     for element in elements:
         section = element.to_dict()
@@ -126,46 +131,60 @@
         if isinstance(value, dict):
             flattened_dict.update(flatten_dict(value, new_key, separator))
         else:
             flattened_dict[new_key] = value
     return flattened_dict
 
 
+def _get_table_fieldnames(rows):
+    table_fieldnames = list(TABLE_FIELDNAMES)
+    for row in rows:
+        metadata = row["metadata"]
+        for key in flatten_dict(metadata):
+            if key.startswith("regex_metadata") and key not in table_fieldnames:
+                table_fieldnames.append(key)
+    return table_fieldnames
+
+
 def convert_to_isd_csv(elements: List[Element]) -> str:
     """
     Returns the representation of document elements as an Initial Structured Document (ISD)
     in CSV Format.
     """
     rows: List[Dict[str, Any]] = convert_to_isd(elements)
+    table_fieldnames = _get_table_fieldnames(rows)
     # NOTE(robinson) - flatten metadata and add it to the table
     for row in rows:
         metadata = row.pop("metadata")
         for key, value in flatten_dict(metadata).items():
-            if key in TABLE_FIELDNAMES:
+            if key in table_fieldnames:
                 row[key] = value
 
         if row.get("sent_from"):
             row["sender"] = row.get("sent_from")
             if type(row["sender"]) == list:
                 row["sender"] = row["sender"][0]
 
     with io.StringIO() as buffer:
-        csv_writer = csv.DictWriter(buffer, fieldnames=TABLE_FIELDNAMES)
+        csv_writer = csv.DictWriter(buffer, fieldnames=table_fieldnames)
         csv_writer.writeheader()
         csv_writer.writerows(rows)
         return buffer.getvalue()
 
 
 def convert_to_csv(elements: List[Element]) -> str:
     """Converts a list of elements to a CSV."""
     return convert_to_isd_csv(elements)
 
 
-def convert_to_dataframe(elements: List[Element]) -> pd.DataFrame:
+def convert_to_dataframe(elements: List[Element], drop_empty_cols: bool = True) -> pd.DataFrame:
     """Converts document elements to a pandas DataFrame. The dataframe contains the
     following columns:
         text: the element text
         type: the text type (NarrativeText, Title, etc)
     """
     csv_string = convert_to_isd_csv(elements)
     csv_string_io = io.StringIO(csv_string)
-    return pd.read_csv(csv_string_io, sep=",")
+    df = pd.read_csv(csv_string_io, sep=",")
+    if drop_empty_cols:
+        df.dropna(axis=1, how="all", inplace=True)
+    return df
```

### Comparing `unstructured-0.8.0/unstructured/staging/baseplate.py` & `unstructured-0.8.1/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/datasaur.py` & `unstructured-0.8.1/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/huggingface.py` & `unstructured-0.8.1/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/label_box.py` & `unstructured-0.8.1/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/label_studio.py` & `unstructured-0.8.1/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/prodigy.py` & `unstructured-0.8.1/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/staging/weaviate.py` & `unstructured-0.8.1/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured/utils.py` & `unstructured-0.8.1/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.1/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.0
+Version: 0.8.1
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -296,14 +296,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.0 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.1 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -201,14 +201,15 @@
 Unstructured | Keywords: NLP PDF HTML CV XML parsing preprocessing Platform:
 UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
-Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
-discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
-Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
-Provides-Extra: gcs Provides-Extra: elasticsearch Provides-Extra: dropbox
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
+text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
+Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
+Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
+slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-Extra:
+gcs Provides-Extra: elasticsearch Provides-Extra: dropbox
```

### Comparing `unstructured-0.8.0/unstructured.egg-info/SOURCES.txt` & `unstructured-0.8.1/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.0/unstructured.egg-info/requires.txt` & `unstructured-0.8.1/unstructured.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-argilla
 chardet
 filetype
 lxml
 msg_parser
 nltk
 openpyxl
 pandas
```

