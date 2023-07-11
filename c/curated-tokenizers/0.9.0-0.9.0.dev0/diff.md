# Comparing `tmp/curated-tokenizers-0.9.0.tar.gz` & `tmp/curated-tokenizers-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-tokenizers-0.9.0.tar", last modified: Mon Jul 10 12:37:38 2023, max compression
+gzip compressed data, was "curated-tokenizers-0.9.0.dev0.tar", last modified: Thu Jul  6 13:19:20 2023, max compression
```

## Comparing `curated-tokenizers-0.9.0.tar` & `curated-tokenizers-0.9.0.dev0.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.814931 curated-tokenizers-0.9.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)     1880 2023-07-10 12:37:38.814931 curated-tokenizers-0.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      939 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.778930 curated-tokenizers-0.9.0/curated_tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/_bbpe.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     6335 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/_bbpe.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     2149 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/_spp.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     7754 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/_spp.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      654 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/_wordpiece.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     5041 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/_wordpiece.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/config.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/merges.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1190 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/merges.hh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.782930 curated-tokenizers-0.9.0/curated_tokenizers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/incorrect-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/robbert-merges-1000.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/robbert-vocab-1000.json
--rw-r--r--   0 vsts      (1001) docker     (122)     2252 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/test_bbpe_processor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4356 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/test_sp.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2220 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/test_word_piece_processor.py
--rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/toy-word-pieces.txt
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/tests/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/util.hh
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/wordpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/curated_tokenizers/wordpiece.hh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.778930 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1880 2023-07-10 12:37:38.000000 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    10431 2023-07-10 12:37:38.000000 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-10 12:37:38.000000 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-07-10 12:37:38.000000 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-10 12:37:38.000000 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-10 12:37:38.000000 curated-tokenizers-0.9.0/curated_tokenizers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.774930 curated-tokenizers-0.9.0/sentencepiece/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.798930 curated-tokenizers-0.9.0/sentencepiece/src/
--rw-r--r--   0 vsts      (1001) docker     (122)     6596 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/bpe_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    11226 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4521 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    18686 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builder.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5203 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builder.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.798930 curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/
--rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 vsts      (1001) docker     (122)   136631 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (122)   200094 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/char_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/char_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5168 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/common.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5936 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4103 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/error.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/filesystem.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/filesystem.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2605 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/freelist.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1280 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1770 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/init.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/init_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/model_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/model_factory.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/model_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8751 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/model_interface.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15351 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 vsts      (1001) docker     (122)    11583 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/normalizer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/normalizer.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2132 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2152 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2892 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    37639 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    27254 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 vsts      (1001) docker     (122)    54189 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6523 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10925 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/spec_parser.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4037 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6597 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2083 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4214 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13036 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/test_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/testharness.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/testharness.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    28978 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 vsts      (1001) docker     (122)    20727 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2817 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unicode_script.h
--rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    34126 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     7324 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unigram_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)    32283 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    22266 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4053 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6752 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     7393 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/util.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10907 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/util_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/word_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/word_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.778930 curated-tokenizers-0.9.0/sentencepiece/third_party/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.778930 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.798930 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/container/
--rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.798930 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 vsts      (1001) docker     (122)     5857 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1745 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.798930 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.798930 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/random/
--rw-r--r--   0 vsts      (1001) docker     (122)      959 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/random/distributions.h
--rw-r--r--   0 vsts      (1001) docker     (122)      926 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/random/random.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.802930 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2106 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.802930 curated-tokenizers-0.9.0/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.806930 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.778930 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.810930 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.810930 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-10 12:37:38.814931 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-07-10 12:37:25.000000 curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1196 2023-07-10 12:37:38.814931 curated-tokenizers-0.9.0/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     5941 2023-07-10 12:37:22.000000 curated-tokenizers-0.9.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     1885 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      939 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/curated_tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_bbpe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5992 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_bbpe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     2149 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      654 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4803 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/config.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1190 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.855949 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/incorrect-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-merges-1000.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-vocab-1000.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     2252 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_bbpe_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4233 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_sp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2220 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_word_piece_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/toy-word-pieces.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/util.hh
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1885 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    10431 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.847950 curated-tokenizers-0.9.0.dev0/sentencepiece/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6596 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11226 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4521 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    18686 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5203 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   136631 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)   200094 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5168 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5936 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4103 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/error.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2605 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1280 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1770 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/init.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/init_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8751 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15351 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11583 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2132 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2152 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2892 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    37639 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    27254 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    54189 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6523 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10925 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4037 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6597 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2083 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4214 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13036 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/test_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    28978 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20727 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2817 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    34126 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     7324 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32283 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    22266 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4053 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6752 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     7393 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10907 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/util_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5857 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1745 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/
+-rw-r--r--   0 vsts      (1001) docker     (122)      959 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/distributions.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      926 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/random.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2106 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.875949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.879949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.879949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1201 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5941 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/setup.py
```

### Comparing `curated-tokenizers-0.9.0/LICENSE` & `curated-tokenizers-0.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/PKG-INFO` & `curated-tokenizers-0.9.0.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.9.0
+Version: 0.9.0.dev0
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `curated-tokenizers-0.9.0/README.md` & `curated-tokenizers-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/_bbpe.pyx` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_bbpe.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,14 @@
         self._piece_to_id = vocab
         self._id_to_piece = {v: k for k, v in vocab.items()}
         cdef vector[pair[string, string]] c_merges
         for p1, p2 in merges:
             c_merges.push_back(pair[string, string](p1.encode('utf-8'), p2.encode('utf-8')))
         self._merges = make_shared[Merges](c_merges)
 
-    def __copy__(self):
-        return ByteBPEProcessor(vocab=self.vocab, merges=self.merges)
-
-    def __deepcopy__(self, memo):
-        # We don't need a deepcopy of the vocab and merges dicts as their
-        # contents will be copied into a backing store in the c'tor.
-        return ByteBPEProcessor(vocab=self.vocab, merges=self.merges)
-
     @staticmethod
     def load_from_files(*, vocab: Path, merges: Path) -> ByteBPEProcessor:
         """Construct a processor from the given vocabulary and merges files."""
         with open(vocab, encoding="utf-8") as f:
             vocab = json.load(f)
         with open(merges, encoding="utf-8") as f:
             version = f.readline()
```

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/_spp.pxd` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/_spp.pyx` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,14 @@
     def __init__(self):
         pass
 
     def __len__(self):
         _check_status(deref(self.spp).status())
         return deref(self.spp).GetPieceSize()
 
-    def __copy__(self):
-        return SentencePieceProcessor.from_protobuf(self.to_protobuf())
-
-    def __deepcopy__(self, memo):
-        result = SentencePieceProcessor.from_protobuf(self.to_protobuf())
-        memo[id(self)] = result
-        return result
-
     @staticmethod
     def from_file(str filename):
         """
         Constructs a SentencePieceProcessor by loading a serialized model from
         disk.
 
             filename (str): Path to model.
@@ -38,17 +30,14 @@
         Constructs a SentencePieceProcessor by loading a serialized model from
         a protocol buffer.
 
             protobuf (bytes): Byte array representing the model's serialized
                 protocol buffer.
         """
         cdef SentencePieceProcessor processor = SentencePieceProcessor.__new__(SentencePieceProcessor)
-        if len(protobuf) == 0:
-            # SentencePiece returns an empty protobuf for uninitialized models.
-            return processor
         cdef string_view protobuf_view = string_view(protobuf, len(protobuf))
         _check_status(deref(processor.spp).LoadFromSerializedProto(protobuf_view))
         return processor
 
     def to_protobuf(self) -> bytes:
         """
         Serializes the SentencePieceProcessor to a protocol buffer.
```

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/_wordpiece.pxd` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/_wordpiece.pyx` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,14 @@
         self._pieces = PieceStorage()
 
         for idx, piece in enumerate(pieces):
             is_initial = not piece.startswith("##")
             byte_array = piece[2:].encode('utf8') if not is_initial else piece.encode('utf8')
             self._pieces.add_piece(byte_array, is_initial)
 
-    def __copy__(self):
-        # This is essentially a deepcopy, but there's no better way to do it.
-        return WordPieceProcessor(self.to_list())
-
-    def __deepcopy__(self, memo):
-        return WordPieceProcessor(self.to_list())
-
     def encode(self, token: str) -> Tuple[List[int], List[str]]:
         """
         Encode a token using word pieces. The piece identifiers are
         returned. If no piece could be found for a suffix, the special
         piece identifier `-1` is used.
 
             token (str): The token to encode as pieces.
```

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/merges.cc` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/merges.hh` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/tests/robbert-merges-1000.txt` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-merges-1000.txt`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/tests/robbert-vocab-1000.json` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-vocab-1000.json`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/tests/test_bbpe_processor.py` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_bbpe_processor.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/tests/test_sp.py` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_sp.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,14 @@
     with open(str(test_dir / "toy.model"), "rb") as f:
         data = f.read()
     spp = SentencePieceProcessor.from_protobuf(data)
     _check_ids(spp)
     serialized_data = spp.to_protobuf()
     assert serialized_data == data
 
-    # Zero-length buffer.
-    spp = SentencePieceProcessor.from_protobuf(bytes())
-    assert spp.to_protobuf() == bytes()
-
 
 def test_load_unknown_file():
     with pytest.raises(OSError, match=r"No such file"):
         SentencePieceProcessor.from_file("bogus.model")
 
 
 def test_handles_nul_character(toy_model):
```

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/tests/test_word_piece_processor.py` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_word_piece_processor.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/tests/toy.model` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/toy.model`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/wordpiece.cc` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers/wordpiece.hh` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers.egg-info/PKG-INFO` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.9.0
+Version: 0.9.0.dev0
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `curated-tokenizers-0.9.0/curated_tokenizers.egg-info/SOURCES.txt` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/bpe_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/bpe_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/bpe_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builder.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builder.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builder_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/char_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/char_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/char_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/char_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/char_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/char_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/common.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/compile_charsmap_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/error.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/filesystem.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/filesystem.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/filesystem_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/freelist.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/freelist_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/init.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/init_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/model_factory.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/model_factory.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/model_factory_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/model_interface.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/model_interface.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/model_interface_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/normalization_rule.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/normalizer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/normalizer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/normalizer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/pretokenizer_for_training.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/pretokenizer_for_training.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/pretokenizer_for_training_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_processor.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_processor.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_processor_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/sentencepiece_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/spec_parser.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/spm_decode_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/spm_encode_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/spm_export_vocab_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/spm_normalize_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/spm_train_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/test_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/testharness.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/testharness.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/trainer_factory.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/trainer_factory.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/trainer_factory_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/trainer_interface.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/trainer_interface.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/trainer_interface_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unicode_script.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unicode_script.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unicode_script_map.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unicode_script_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unigram_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unigram_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/unigram_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/util.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/util_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/word_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/word_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/word_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/word_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/word_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/src/word_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/container/flat_hash_map.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/container/flat_hash_set.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/flag.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/flag.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/flags/parse.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/memory/memory.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/random/distributions.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/distributions.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/random/random.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/random.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/ascii.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/match.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/numbers.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_cat.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_format.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_join.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_replace.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/str_split.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/string_view.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/absl/strings/strip.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/darts_clone/darts.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/arena.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/common.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/int128.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/status.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/statusor.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/strutil.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/time.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.0/setup.cfg` & `curated-tokenizers-0.9.0.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 description = Lightweight piece tokenization library
-version = 0.9.0
+version = 0.9.0.dev0
 url = https://github.com/explosion/curated-tokenizers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `curated-tokenizers-0.9.0/setup.py` & `curated-tokenizers-0.9.0.dev0/setup.py`

 * *Files identical despite different names*

