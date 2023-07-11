# Comparing `tmp/dolma-0.6.2.tar.gz` & `tmp/dolma-0.6.3.tar.gz`

## Comparing `dolma-0.6.2.tar` & `dolma-0.6.3.tar`

### file list

```diff
@@ -1,82 +1,84 @@
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 dolma-0.6.2/Cargo.toml
--rw-r--r--   0     1001      123      475 2023-07-10 21:38:08.000000 dolma-0.6.2/.flake8
--rw-r--r--   0     1001      123     3220 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     2194 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0     1001      123      691 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0     1001      123     1077 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0     1001      123      414 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0     1001      123      549 2023-07-10 21:38:08.000000 dolma-0.6.2/.gitignore
--rw-r--r--   0     1001      123     1813 2023-07-10 21:38:08.000000 dolma-0.6.2/CITATION.cff
--rw-r--r--   0     1001      123    11357 2023-07-10 21:38:08.000000 dolma-0.6.2/LICENSE
--rw-r--r--   0     1001      123     2295 2023-07-10 21:38:08.000000 dolma-0.6.2/Makefile
--rw-r--r--   0     1001      123     3156 2023-07-10 21:38:08.000000 dolma-0.6.2/README.md
--rw-r--r--   0     1001      123     3217 2023-07-10 21:38:08.000000 dolma-0.6.2/pyproject.toml
--rw-r--r--   0     1001      123      736 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/__init__.py
--rw-r--r--   0     1001      123     4401 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/__init__.py
--rw-r--r--   0     1001      123     1494 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/__main__.py
--rw-r--r--   0     1001      123     4689 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/deduper.py
--rw-r--r--   0     1001      123     4589 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/mixer.py
--rw-r--r--   0     1001      123      473 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/shared.py
--rw-r--r--   0     1001      123     1957 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/tagger.py
--rw-r--r--   0     1001      123      219 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/__init__.py
--rw-r--r--   0     1001      123     6111 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/data_types.py
--rw-r--r--   0     1001      123      337 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/errors.py
--rw-r--r--   0     1001      123     6482 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/ft_dataset.py
--rw-r--r--   0     1001      123     5557 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/ft_tagger.py
--rw-r--r--   0     1001      123    15587 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/parallel.py
--rw-r--r--   0     1001      123     6326 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/paths.py
--rw-r--r--   0     1001      123     1254 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/registry.py
--rw-r--r--   0     1001      123    11812 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/runtime.py
--rw-r--r--   0     1001      123     1032 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/taggers.py
--rw-r--r--   0     1001      123       42 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/trainer.py
--rw-r--r--   0     1001      123     2031 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/utils.py
--rw-r--r--   0     1001      123     9484 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/vizualizer.py
--rw-r--r--   0     1001      123     3777 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/data/naughty_words_en.txt
--rw-r--r--   0     1001      123        0 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/py.typed
--rw-r--r--   0     1001      123       72 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/__init__.py
--rw-r--r--   0     1001      123     3277 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/c4.py
--rw-r--r--   0     1001      123     6433 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/code.py
--rw-r--r--   0     1001      123     6857 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/gopher.py
--rw-r--r--   0     1001      123     1898 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/jigsaw.py
--rw-r--r--   0     1001      123     6391 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/language.py
--rw-r--r--   0     1001      123     4876 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/length.py
--rw-r--r--   0     1001      123    10494 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/pii.py
--rw-r--r--   0     1001      123      744 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/sampling.py
--rw-r--r--   0     1001      123      232 2023-07-10 21:38:08.000000 dolma-0.6.2/res/logo.md
--rw-r--r--   0     1001      123  1813803 2023-07-10 21:38:08.000000 dolma-0.6.2/res/logo.png
--rw-r--r--   0     1001      123     9277 2023-07-10 21:38:08.000000 dolma-0.6.2/src/bloom_filter.rs
--rw-r--r--   0     1001      123    14421 2023-07-10 21:38:08.000000 dolma-0.6.2/src/deduper.rs
--rw-r--r--   0     1001      123     1124 2023-07-10 21:38:08.000000 dolma-0.6.2/src/lib.rs
--rw-r--r--   0     1001      123     7176 2023-07-10 21:38:08.000000 dolma-0.6.2/src/mixer.rs
--rw-r--r--   0     1001      123    11131 2023-07-10 21:38:08.000000 dolma-0.6.2/src/s3_util.rs
--rw-r--r--   0     1001      123    23416 2023-07-10 21:38:08.000000 dolma-0.6.2/src/shard.rs
--rw-r--r--   0     1001      123      863 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/c4-cleaned.json
--rw-r--r--   0     1001      123      564 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/dedupe-by-url.json
--rw-r--r--   0     1001      123      553 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/dedupe-paragraphs.json
--rw-r--r--   0     1001      123      815 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/email-spans.json
--rw-r--r--   0     1001      123      799 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/filter-by-spans.json
--rw-r--r--   0     1001      123      792 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/mixer.json
--rw-r--r--   0     1001      123      716 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/paragraph-spans.json
--rw-r--r--   0     1001      123    25985 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/documents.json.gz
--rw-r--r--   0     1001      123      702 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/duplicate-paragraphs.json.gz
--rw-r--r--   0     1001      123      489 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/dedupe-by-url.json.gz
--rw-r--r--   0     1001      123      746 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/dedupe-paragraphs.json.gz
--rw-r--r--   0     1001      123    26447 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/email-spans.json.gz
--rw-r--r--   0     1001      123    14879 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/filter-by-spans.json.gz
--rw-r--r--   0     1001      123    15748 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/mixer.json.gz
--rw-r--r--   0     1001      123    26524 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/remove-paragraphs.json.gz
--rw-r--r--   0     1001      123      614 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/pii-attributes.json.gz
--rw-r--r--   0     1001      123      570 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/sample-attributes.json.gz
--rw-r--r--   0     1001      123      543 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/toxicity-attributes.json.gz
--rw-r--r--   0     1001      123      352 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/__init__.py
--rw-r--r--   0     1001      123     3342 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_data_types.py
--rw-r--r--   0     1001      123      471 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_deduper.py
--rw-r--r--   0     1001      123      820 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_mixer.py
--rw-r--r--   0     1001      123     1395 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_omegaconf.py
--rw-r--r--   0     1001      123     2459 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_parallel.py
--rw-r--r--   0     1001      123     8972 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_paths.py
--rw-r--r--   0     1001      123     1846 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_runtime.py
--rw-r--r--   0     1001      123     9701 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_taggers.py
--rw-r--r--   0     1001      123     4043 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_utils.py
--rw-r--r--   0     1001      123    57199 2023-07-10 21:38:15.000000 dolma-0.6.2/Cargo.lock
--rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 dolma-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dolma-0.6.3/Cargo.toml
+-rw-r--r--   0     1001      123      299 2023-07-11 03:40:04.000000 dolma-0.6.3/.cargo/config.toml
+-rw-r--r--   0     1001      123      475 2023-07-11 03:40:04.000000 dolma-0.6.3/.flake8
+-rw-r--r--   0     1001      123     3220 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     2194 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      123      691 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0     1001      123     1077 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0     1001      123      414 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0     1001      123      549 2023-07-11 03:40:04.000000 dolma-0.6.3/.gitignore
+-rw-r--r--   0     1001      123     1813 2023-07-11 03:40:04.000000 dolma-0.6.3/CITATION.cff
+-rw-r--r--   0     1001      123    11357 2023-07-11 03:40:04.000000 dolma-0.6.3/LICENSE
+-rw-r--r--   0     1001      123     2209 2023-07-11 03:40:04.000000 dolma-0.6.3/Makefile
+-rw-r--r--   0     1001      123     3156 2023-07-11 03:40:04.000000 dolma-0.6.3/README.md
+-rw-r--r--   0     1001      123     3217 2023-07-11 03:40:04.000000 dolma-0.6.3/pyproject.toml
+-rw-r--r--   0     1001      123      736 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/__init__.py
+-rw-r--r--   0     1001      123     4401 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/__init__.py
+-rw-r--r--   0     1001      123     1494 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/__main__.py
+-rw-r--r--   0     1001      123     4689 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/deduper.py
+-rw-r--r--   0     1001      123     4589 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/mixer.py
+-rw-r--r--   0     1001      123      473 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/shared.py
+-rw-r--r--   0     1001      123     1957 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/tagger.py
+-rw-r--r--   0     1001      123      219 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/__init__.py
+-rw-r--r--   0     1001      123     6111 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/data_types.py
+-rw-r--r--   0     1001      123      337 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/errors.py
+-rw-r--r--   0     1001      123     6482 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/ft_dataset.py
+-rw-r--r--   0     1001      123     5557 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/ft_tagger.py
+-rw-r--r--   0     1001      123    15587 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/parallel.py
+-rw-r--r--   0     1001      123     6326 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/paths.py
+-rw-r--r--   0     1001      123     1254 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/registry.py
+-rw-r--r--   0     1001      123    11812 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/runtime.py
+-rw-r--r--   0     1001      123     1032 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/taggers.py
+-rw-r--r--   0     1001      123       42 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/trainer.py
+-rw-r--r--   0     1001      123     2031 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/utils.py
+-rw-r--r--   0     1001      123     9484 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/vizualizer.py
+-rw-r--r--   0     1001      123     3777 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/data/naughty_words_en.txt
+-rw-r--r--   0     1001      123        0 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/py.typed
+-rw-r--r--   0     1001      123       72 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/__init__.py
+-rw-r--r--   0     1001      123     3277 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/c4.py
+-rw-r--r--   0     1001      123     6433 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/code.py
+-rw-r--r--   0     1001      123     6857 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/gopher.py
+-rw-r--r--   0     1001      123     1898 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/jigsaw.py
+-rw-r--r--   0     1001      123     6391 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/language.py
+-rw-r--r--   0     1001      123     4876 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/length.py
+-rw-r--r--   0     1001      123    10494 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/pii.py
+-rw-r--r--   0     1001      123      744 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/sampling.py
+-rw-r--r--   0     1001      123      232 2023-07-11 03:40:04.000000 dolma-0.6.3/res/logo.md
+-rw-r--r--   0     1001      123  1813803 2023-07-11 03:40:04.000000 dolma-0.6.3/res/logo.png
+-rw-r--r--   0     1001      123     9277 2023-07-11 03:40:04.000000 dolma-0.6.3/src/bloom_filter.rs
+-rw-r--r--   0     1001      123    13521 2023-07-11 03:40:04.000000 dolma-0.6.3/src/deduper.rs
+-rw-r--r--   0     1001      123     1124 2023-07-11 03:40:04.000000 dolma-0.6.3/src/lib.rs
+-rw-r--r--   0     1001      123     7515 2023-07-11 03:40:04.000000 dolma-0.6.3/src/mixer.rs
+-rw-r--r--   0     1001      123    10738 2023-07-11 03:40:04.000000 dolma-0.6.3/src/s3_util.rs
+-rw-r--r--   0     1001      123    27475 2023-07-11 03:40:04.000000 dolma-0.6.3/src/shard.rs
+-rw-r--r--   0     1001      123      863 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/c4-cleaned.json
+-rw-r--r--   0     1001      123      564 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/dedupe-by-url.json
+-rw-r--r--   0     1001      123      553 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/dedupe-paragraphs.json
+-rw-r--r--   0     1001      123      815 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/email-spans.json
+-rw-r--r--   0     1001      123      799 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/filter-by-spans.json
+-rw-r--r--   0     1001      123      749 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/mixer-local.json
+-rw-r--r--   0     1001      123      792 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/mixer.json
+-rw-r--r--   0     1001      123      716 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/paragraph-spans.json
+-rw-r--r--   0     1001      123    25985 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/documents.json.gz
+-rw-r--r--   0     1001      123      702 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/duplicate-paragraphs.json.gz
+-rw-r--r--   0     1001      123      489 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/dedupe-by-url.json.gz
+-rw-r--r--   0     1001      123      746 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/dedupe-paragraphs.json.gz
+-rw-r--r--   0     1001      123    26447 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/email-spans.json.gz
+-rw-r--r--   0     1001      123    14879 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/filter-by-spans.json.gz
+-rw-r--r--   0     1001      123    15748 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/mixer.json.gz
+-rw-r--r--   0     1001      123    26524 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/remove-paragraphs.json.gz
+-rw-r--r--   0     1001      123      614 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/pii-attributes.json.gz
+-rw-r--r--   0     1001      123      570 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/sample-attributes.json.gz
+-rw-r--r--   0     1001      123      543 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/toxicity-attributes.json.gz
+-rw-r--r--   0     1001      123      352 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/__init__.py
+-rw-r--r--   0     1001      123     3342 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_data_types.py
+-rw-r--r--   0     1001      123      471 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_deduper.py
+-rw-r--r--   0     1001      123      820 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_mixer.py
+-rw-r--r--   0     1001      123     1395 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_omegaconf.py
+-rw-r--r--   0     1001      123     2459 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_parallel.py
+-rw-r--r--   0     1001      123     8972 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_paths.py
+-rw-r--r--   0     1001      123     1846 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_runtime.py
+-rw-r--r--   0     1001      123     9701 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_taggers.py
+-rw-r--r--   0     1001      123     4043 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_utils.py
+-rw-r--r--   0     1001      123    57396 2023-07-11 03:40:16.000000 dolma-0.6.3/Cargo.lock
+-rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 dolma-0.6.3/PKG-INFO
```

### Comparing `dolma-0.6.2/Cargo.toml` & `dolma-0.6.3/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [package]
 name = "dolma"
-version = "0.6.2"
+version = "0.6.3"
 edition = "2021"
 license = "Apache-2.0"
 
-
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dolma"
 crate-type = ["cdylib"]
 
 [dependencies]
 ahash = { version = "0.8.1", features = ["runtime-rng"] }
@@ -26,7 +25,8 @@
 rayon = "1.7.0"
 serde = {version = "1.0.160", features = ["derive"]}
 serde_json = "1.0"
 threadpool = "1.8.1"
 tokio = {version = "1.27.0", features = ["full"]}
 tokio-util = "0.7.7"
 unicode-segmentation = "1.7"
+glob = "0.3.1"
```

### Comparing `dolma-0.6.2/.github/workflows/CI.yml` & `dolma-0.6.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/bug_report.yml` & `dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/documentation.yml` & `dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/feature_request.yml` & `dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/.gitignore` & `dolma-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/CITATION.cff` & `dolma-0.6.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/LICENSE` & `dolma-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/Makefile` & `dolma-0.6.3/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -24,33 +24,32 @@
 	$(shell "${OPENSSL_SETUP}")
 	which cargo || curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
 	which maturin || pip install maturin
 
 publish:
 	maturin publish
 
-test: setup develop setup-test test-python test-rust clean-test
+test: setup develop setup-test test-python test-rust
 
 test-python:
 	pytest -vs tests/python
 
-test-rust:
-	cargo test -- --nocapture
-
-clean-test:
+test-rust-clean:
 	rm -rf tests/work/*
 	aws s3 rm --recursive s3://ai2-llm/pretraining-data/tests/mixer/
 
-setup-test:
+test-rust-setup:
 	aws s3 cp tests/data/documents.json.gz s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/documents/head/0000.json.gz
 	aws s3 cp tests/data/pii-attributes.json.gz s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/pii/head/0000.json.gz
 	aws s3 cp tests/data/toxicity-attributes.json.gz s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/toxicity/head/0000.json.gz
 	aws s3 cp tests/data/sample-attributes.json.gz s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/sample/head/0000.json.gz
 	aws s3 cp tests/data/duplicate-paragraphs.json.gz s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/duplicate_paragraphs/head/0000.json.gz
-	aws s3 sync tests/data/expected s3://ai2-llm/pretraining-data/tests/mixer/expected  --exclude ".*" --exclude "*/.*"
+
+test-rust: test-rust-clean test-rust-setup
+	cargo test -- --nocapture
 
 develop:
 	maturin develop --extras=dev
 
 style:
 	rustfmt --edition 2021 src/*.rs
 	autopep8 --in-place --recursive python/
```

### Comparing `dolma-0.6.2/README.md` & `dolma-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/pyproject.toml` & `dolma-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dolma"
-version = "0.6.2"
+version = "0.6.3"
 description = "Data filters"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "requests",
     "tqdm",
```

### Comparing `dolma-0.6.2/python/dolma/__init__.py` & `dolma-0.6.3/python/dolma/__init__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/cli/__init__.py` & `dolma-0.6.3/python/dolma/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/cli/__main__.py` & `dolma-0.6.3/python/dolma/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/cli/deduper.py` & `dolma-0.6.3/python/dolma/cli/deduper.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/cli/mixer.py` & `dolma-0.6.3/python/dolma/cli/mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/cli/tagger.py` & `dolma-0.6.3/python/dolma/cli/tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/data_types.py` & `dolma-0.6.3/python/dolma/core/data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/ft_dataset.py` & `dolma-0.6.3/python/dolma/core/ft_dataset.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/ft_tagger.py` & `dolma-0.6.3/python/dolma/core/ft_tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/parallel.py` & `dolma-0.6.3/python/dolma/core/parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/paths.py` & `dolma-0.6.3/python/dolma/core/paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/registry.py` & `dolma-0.6.3/python/dolma/core/registry.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/runtime.py` & `dolma-0.6.3/python/dolma/core/runtime.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/taggers.py` & `dolma-0.6.3/python/dolma/core/taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/utils.py` & `dolma-0.6.3/python/dolma/core/utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/core/vizualizer.py` & `dolma-0.6.3/python/dolma/core/vizualizer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/data/naughty_words_en.txt` & `dolma-0.6.3/python/dolma/data/naughty_words_en.txt`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/c4.py` & `dolma-0.6.3/python/dolma/taggers/c4.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/code.py` & `dolma-0.6.3/python/dolma/taggers/code.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/gopher.py` & `dolma-0.6.3/python/dolma/taggers/gopher.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/jigsaw.py` & `dolma-0.6.3/python/dolma/taggers/jigsaw.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/language.py` & `dolma-0.6.3/python/dolma/taggers/language.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/length.py` & `dolma-0.6.3/python/dolma/taggers/length.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/pii.py` & `dolma-0.6.3/python/dolma/taggers/pii.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/python/dolma/taggers/sampling.py` & `dolma-0.6.3/python/dolma/taggers/sampling.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/res/logo.png` & `dolma-0.6.3/res/logo.png`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/src/bloom_filter.rs` & `dolma-0.6.3/src/bloom_filter.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/src/deduper.rs` & `dolma-0.6.3/src/deduper.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 use std::collections::VecDeque;
 use std::fs::OpenOptions;
 use std::io;
 use std::io::{BufRead, BufReader, BufWriter, Write};
-use std::path::{Path, PathBuf};
+use std::path::PathBuf;
 use std::process;
 use std::sync::atomic::{AtomicU32, Ordering};
 use std::sync::Arc;
 
 use flate2::read::MultiGzDecoder;
 use flate2::write::GzEncoder;
 use flate2::Compression;
 use serde_json::{json, Value};
 use threadpool::ThreadPool;
 
 use crate::bloom_filter::BloomFilter;
 use crate::s3_util;
-use crate::s3_util::{download_to_file, upload_file};
 use crate::shard::shard_config::WorkDirConfig;
+use crate::shard::FileCache;
 
 use deduper_config::*;
 
 pub fn run(config: DeduperConfig) {
     assert!(
         config.dedupe.paragraphs.is_some() ^ config.dedupe.documents.is_some(),
         "Must dedupe either paragraphs or documents"
@@ -70,73 +70,82 @@
     }
 }
 
 // Write attributes for the documents in the given file:
 // For doc-level deduping, check the Bloom filter for existence of the configured key and set the configured attribute to true.
 // For paragraph-level deduping, check the Bloom filter for existence of a paragraph in the text and add a span to the configured attribute.
 fn write_attributes(
-    doc_path: String,
+    docs_location: String,
     work_dirs: WorkDirConfig,
     dedupe_config: DedupeConfig,
     bloom_filter: Arc<BloomFilter>,
 ) -> Result<(), io::Error> {
-    let rt = tokio::runtime::Builder::new_current_thread()
-        .enable_all()
-        .build()
-        .unwrap();
-
-    let s3_client = s3_util::new_client(None)?;
-
-    let input_work_dir = Path::new(&work_dirs.input);
-    let output_work_dir = Path::new(&work_dirs.output);
+    let cache = FileCache {
+        s3_client: Box::new(s3_util::new_client(None)?),
+        work: work_dirs.clone(),
+    };
 
-    let output_path = {
+    let attrs_location = {
         let mut attr_prefix = "/attributes/".to_owned();
         attr_prefix.push_str(&dedupe_config.name);
         attr_prefix.push_str("/");
-        doc_path.to_owned().replace("/documents/", &attr_prefix)
+        docs_location
+            .to_owned()
+            .replace("/documents/", &attr_prefix)
     };
-    let local_output = output_work_dir.join(&output_path);
+    let local_output = cache.prepare_output(&attrs_location)?;
     if local_output.exists() {
-        log::info!("Skipping {:?} because it already exists", output_path);
+        log::info!("Skipping {:?} because it already exists", attrs_location);
         return Ok(());
     }
+    log::info!(
+        "Writing attributes for {} to {}",
+        docs_location,
+        local_output.display()
+    );
 
     std::fs::create_dir_all(local_output.parent().unwrap())?;
 
-    let tmp_output_path = output_work_dir.join(output_path.clone() + ".tmp");
+    log::info!(
+        "Writing attributes for {} to {}",
+        docs_location,
+        local_output.display()
+    );
     {
-        let local_input = input_work_dir.join(Path::new(&doc_path));
-        log::info!("Downloading {} to {}", doc_path, local_input.display());
-        rt.block_on(download_to_file(&s3_client, &doc_path, &local_input))?;
+        let local_input = cache.prepare_input(&docs_location)?;
         let input_file = OpenOptions::new()
             .read(true)
             .write(false)
             .create(false)
             .open(local_input.clone())?;
         let reader = BufReader::with_capacity(1024 * 1024, MultiGzDecoder::new(input_file));
 
         let tmp_output = OpenOptions::new()
             .read(false)
             .write(true)
             .create(true)
             .truncate(true)
-            .open(&tmp_output_path)?;
+            .open(&local_output)?;
 
         let mut writer = BufWriter::with_capacity(
             1024 * 1024,
             GzEncoder::new(tmp_output, Compression::default()),
         );
 
         let mut line_number = 0;
         for line in reader.lines() {
             match line {
                 Ok(_) => {}
                 Err(e) => {
-                    log::error!("Error reading line {} of {}: {}", line_number, &doc_path, e);
+                    log::error!(
+                        "Error reading line {} of {}: {}",
+                        line_number,
+                        &docs_location,
+                        e
+                    );
                     break;
                 }
             }
             line_number += 1;
             let line = line?;
             let data: Value = serde_json::from_str(&line)?;
             let mut attributes = json!({});
@@ -219,31 +228,15 @@
             output_object["id"] = data["id"].clone();
             output_object["attributes"] = attributes;
             serde_json::to_writer(&mut writer, &output_object)?;
             writer.write_all(b"\n")?;
         }
         std::fs::remove_file(local_input)?;
     }
-
-    log::info!(
-        "Uploading {} to {}",
-        &tmp_output_path.display(),
-        &output_path
-    );
-    rt.block_on(upload_file(&s3_client, &output_path, &tmp_output_path))?;
-
-    {
-        // Create empty file to indicate that the shard is done.
-        OpenOptions::new()
-            .create(true)
-            .write(true)
-            .open(&local_output)?;
-        std::fs::remove_file(&tmp_output_path)?;
-    }
-
+    cache.finalize_output(&attrs_location)?;
     Ok(())
 }
 
 pub mod deduper_config {
     use serde::{Deserialize, Serialize};
     use std::fs::File;
     use std::io;
@@ -299,24 +292,22 @@
             let config: DeduperConfig = serde_json::from_str(s)?;
             Ok(config)
         }
     }
 }
 
 #[cfg(test)]
-pub mod test {
+mod test {
     use std::fs::OpenOptions;
     use std::io;
     use std::io::{BufRead, BufReader};
-    use std::path::Path;
 
     use flate2::read::MultiGzDecoder;
 
     use crate::s3_util;
-    use crate::s3_util::download_to_file;
 
     use super::*;
 
     fn compare_contents(expected: &str, actual: &str) {
         let expected_lines = BufReader::new(MultiGzDecoder::new(
             OpenOptions::new()
                 .read(true)
@@ -348,58 +339,44 @@
             let actual = actual.unwrap();
             let expected = expected.unwrap();
             assert_eq!(actual, expected);
         }
     }
 
     #[test]
-    pub fn test_dedupe_by_url() -> Result<(), io::Error> {
+    fn test_dedupe_by_url() -> Result<(), io::Error> {
         let config = DeduperConfig::read_from_file("tests/config/dedupe-by-url.json").unwrap();
-        run(config);
+        run(config.clone());
 
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
-        let local_output_file = "tests/work/output/dedupe-by-url.json.gz";
-        let remote_output_file = "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/dedupe_by_url/head/0000.json.gz";
-        rt.block_on(download_to_file(
-            &s3_client,
-            remote_output_file,
-            Path::new(local_output_file),
-        ))?;
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: config.work_dir.clone(),
+        };
+
+        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/dedupe_by_url/head/0000.json.gz")?;
 
         compare_contents(
             "tests/data/expected/dedupe-by-url.json.gz",
-            local_output_file,
+            &local_output_file.display().to_string(),
         );
         Ok(())
     }
 
     #[test]
-    pub fn test_dedupe_paragraphs() -> Result<(), io::Error> {
+    fn test_dedupe_paragraphs() -> Result<(), io::Error> {
         let config = DeduperConfig::read_from_file("tests/config/dedupe-paragraphs.json").unwrap();
-        run(config);
+        run(config.clone());
+
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: config.work_dir.clone(),
+        };
 
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
-        let local_output_file = "tests/work/output/dedupe-paragraphs.json.gz";
-        let remote_output_file = "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/dedupe_paragraphs/head/0000.json.gz";
-        rt.block_on(download_to_file(
-            &s3_client,
-            remote_output_file,
-            Path::new(local_output_file),
-        ))?;
+        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/dedupe_paragraphs/head/0000.json.gz")?;
 
         compare_contents(
             "tests/data/expected/dedupe-paragraphs.json.gz",
-            local_output_file,
+            &local_output_file.display().to_string(),
         );
         Ok(())
     }
 }
```

### Comparing `dolma-0.6.2/src/lib.rs` & `dolma-0.6.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/src/mixer.rs` & `dolma-0.6.3/src/mixer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 pub mod mixer_config {
     use serde::{Deserialize, Serialize};
     use std::fs::File;
     use std::io;
 
     use crate::shard::shard_config::{StreamConfig, WorkDirConfig};
 
-    #[derive(Serialize, Deserialize)]
+    #[derive(Serialize, Deserialize, Clone)]
     pub struct MixerConfig {
         pub streams: Vec<StreamConfig>,
         pub processes: usize,
         pub work_dir: WorkDirConfig,
     }
 
     impl MixerConfig {
@@ -76,20 +76,20 @@
 }
 
 #[cfg(test)]
 mod test {
     use std::fs::OpenOptions;
     use std::io;
     use std::io::{BufRead, BufReader};
-    use std::path::Path;
 
     use flate2::read::MultiGzDecoder;
 
     use crate::s3_util;
-    use crate::s3_util::download_to_file;
+    use crate::shard::FileCache;
+    use mixer_config::MixerConfig;
 
     use super::*;
 
     fn compare_contents(expected: &str, actual: &str) {
         let expected_lines = BufReader::new(MultiGzDecoder::new(
             OpenOptions::new()
                 .read(true)
@@ -123,106 +123,107 @@
             assert_eq!(actual, expected);
         }
     }
 
     #[test]
     fn test_mixer() -> Result<(), io::Error> {
         let config = MixerConfig::read_from_file("tests/config/mixer.json")?;
-        run(config);
+        run(config.clone());
 
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
-        let local_output_file = "tests/work/output/mixer.json.gz";
-        let remote_output_file =
-            "s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/mixer-test-0000.json.gz";
-        rt.block_on(download_to_file(
-            &s3_client,
-            remote_output_file,
-            Path::new(local_output_file),
-        ))?;
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: config.work_dir.clone(),
+        };
 
-        compare_contents("tests/data/expected/mixer.json.gz", local_output_file);
+        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/mixer-test-0000.json.gz")?;
+
+        compare_contents(
+            "tests/data/expected/mixer.json.gz",
+            &local_output_file.display().to_string(),
+        );
+        Ok(())
+    }
+
+    #[test]
+    fn test_mixer_local() -> Result<(), io::Error> {
+        std::fs::create_dir_all("tests/work/mixer-local/input/documents/mixer-local")?;
+        std::fs::create_dir_all("tests/work/mixer-local/input/attributes/pii/mixer-local")?;
+        std::fs::create_dir_all("tests/work/mixer-local/input/attributes/toxicity/mixer-local")?;
+        std::fs::copy(
+            "tests/data/documents.json.gz",
+            "tests/work/mixer-local/input/documents/mixer-local/0000.json.gz",
+        )?;
+        std::fs::copy(
+            "tests/data/pii-attributes.json.gz",
+            "tests/work/mixer-local/input/attributes/pii/mixer-local/0000.json.gz",
+        )?;
+        std::fs::copy(
+            "tests/data/toxicity-attributes.json.gz",
+            "tests/work/mixer-local/input/attributes/toxicity/mixer-local/0000.json.gz",
+        )?;
+        let config = MixerConfig::read_from_file("tests/config/mixer-local.json")?;
+        run(config.clone());
+
+        compare_contents(
+            "tests/data/expected/mixer.json.gz",
+            "tests/work/mixer-local/output/mixer-local-test-0000.json.gz",
+        );
         Ok(())
     }
 
     #[test]
     fn test_email_span_replacement() -> Result<(), io::Error> {
         let config = MixerConfig::read_from_file("tests/config/email-spans.json")?;
-        run(config);
+        run(config.clone());
 
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
-        let local_output_file = "tests/work/output/email-spans.json.gz";
-        let remote_output_file =
-            "s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/email-spans-test-0000.json.gz";
-        rt.block_on(download_to_file(
-            &s3_client,
-            remote_output_file,
-            Path::new(local_output_file),
-        ))?;
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: config.work_dir.clone(),
+        };
 
-        compare_contents("tests/data/expected/email-spans.json.gz", local_output_file);
+        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/email-spans-test-0000.json.gz")?;
+
+        compare_contents(
+            "tests/data/expected/email-spans.json.gz",
+            &local_output_file.display().to_string(),
+        );
         Ok(())
     }
 
     #[test]
     fn test_paragraph_removal() -> Result<(), io::Error> {
         let config = MixerConfig::read_from_file("tests/config/paragraph-spans.json")?;
-        run(config);
+        run(config.clone());
+
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: config.work_dir.clone(),
+        };
 
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
-        let local_output_file = "tests/work/output/remove-paragraphs.json.gz";
-        let remote_output_file =
-            "s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/paragraph-spans-test-0000.json.gz";
-        rt.block_on(download_to_file(
-            &s3_client,
-            remote_output_file,
-            Path::new(local_output_file),
-        ))?;
+        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/paragraph-spans-test-0000.json.gz")?;
 
         compare_contents(
             "tests/data/expected/remove-paragraphs.json.gz",
-            local_output_file,
+            &local_output_file.display().to_string(),
         );
         Ok(())
     }
 
     #[test]
     fn test_filter_by_span() -> Result<(), io::Error> {
         let config = MixerConfig::read_from_file("tests/config/filter-by-spans.json")?;
-        run(config);
+        run(config.clone());
+
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: config.work_dir.clone(),
+        };
 
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
-        let local_output_file = "tests/work/output/filter-by-spans.json.gz";
-        let remote_output_file =
-            "s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/filter-by-spans-test-0000.json.gz";
-        rt.block_on(download_to_file(
-            &s3_client,
-            remote_output_file,
-            Path::new(local_output_file),
-        ))?;
+        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head/filter-by-spans-test-0000.json.gz")?;
 
         compare_contents(
             "tests/data/expected/filter-by-spans.json.gz",
-            local_output_file,
+            &local_output_file.display().to_string(),
         );
         Ok(())
     }
 }
```

### Comparing `dolma-0.6.2/src/s3_util.rs` & `dolma-0.6.3/src/s3_util.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 use std::io;
 use std::path::Path;
-use std::str::FromStr;
 
 use aws_sdk_s3::config::Region;
 use aws_sdk_s3::error::ProvideErrorMetadata;
 use aws_sdk_s3::primitives::ByteStream;
 use aws_sdk_s3::Client as S3Client;
-use regex::Regex;
 use tokio::fs::File as TokioFile;
 
-pub fn split_path(s3_prefix: &str) -> Result<(&str, &str), &'static str> {
+// Split an s3:// url into a bucket and key
+pub fn split_url(s3_url: &str) -> Result<(&str, &str), &'static str> {
     // use a regular expression to check if s3_prefix starts with s3://
-    let re = Regex::new(r"^s3://").unwrap();
-    if !re.is_match(s3_prefix) {
+    if !s3_url.starts_with("s3://") {
         return Err("s3_prefix must start with s3://");
     }
 
     // split the s3_prefix into parts
-    let parts: Vec<&str> = s3_prefix.splitn(4, '/').collect();
+    let parts: Vec<&str> = s3_url.splitn(4, '/').collect();
 
     // if there are less than 3 parts, then the s3_prefix is invalid
     if parts.len() < 3 {
         return Err("s3_prefix must be in the form s3://bucket/path/to/object");
     }
 
     let bucket = parts[2];
 
     // if there are not 4 parts, then the object path is empty, so we set it to "/"
-    let object_path = if parts.len() == 4 { parts[3] } else { "/" };
+    let key = if parts.len() == 4 { parts[3] } else { "/" };
 
-    Ok((bucket, object_path))
+    Ok((bucket, key))
 }
 
 pub async fn download_to_file(
     s3_client: &S3Client,
-    prefix: &str,
+    bucket: &str,
+    key: &str,
     path: &Path,
 ) -> Result<(), io::Error> {
-    let (bucket, key) = split_path(prefix).unwrap();
-
     let result = s3_client
         .get_object()
         .bucket(bucket)
-        .key(key)
+        .key(key.clone())
         .send()
         .await
         .map_err(|e| {
             io::Error::new(
                 io::ErrorKind::Other,
                 format!(
                     "Error downloading {}: {}",
@@ -60,21 +57,24 @@
     let mut file = TokioFile::create(path).await?;
     let mut body = result.body.into_async_read();
     tokio::io::copy(&mut body, &mut file).await?;
 
     Ok(())
 }
 
-pub async fn upload_file(s3_client: &S3Client, prefix: &str, path: &Path) -> Result<(), io::Error> {
-    let (bucket, key) = split_path(prefix).unwrap();
-
+pub async fn upload_file(
+    s3_client: &S3Client,
+    path: &Path,
+    bucket: &str,
+    key: &str,
+) -> Result<(), io::Error> {
     s3_client
         .put_object()
         .bucket(bucket)
-        .key(key)
+        .key(key.clone())
         .body(ByteStream::from_path(path).await?)
         .send()
         .await
         .map_err(|e| {
             io::Error::new(
                 io::ErrorKind::Other,
                 format!(
@@ -84,16 +84,19 @@
                 ),
             )
         })?;
 
     Ok(())
 }
 
-pub async fn object_size(s3_client: &S3Client, prefix: &str) -> Result<usize, io::Error> {
-    let (bucket, key) = split_path(prefix).unwrap();
+pub async fn object_size(
+    s3_client: &S3Client,
+    bucket: &str,
+    key: &str,
+) -> Result<usize, io::Error> {
     let resp = s3_client
         .head_object()
         .bucket(bucket)
         .key(key)
         .send()
         .await
         .map_err(|e| io::Error::new(io::ErrorKind::Other, e));
@@ -113,73 +116,66 @@
 ) -> Result<Vec<String>, io::Error> {
     let rt = tokio::runtime::Builder::new_current_thread()
         .enable_all()
         .build()
         .unwrap();
 
     let mut stream_inputs: Vec<String> = Vec::new();
-    for full_pattern in patterns.iter() {
+    for pattern in patterns.iter() {
         let start_size = stream_inputs.len();
-        let (bucket, pattern) = split_path(full_pattern).unwrap();
-
-        let mut output_prefix = String::from_str("s3://").unwrap();
-        output_prefix.push_str(bucket);
-        output_prefix.push_str("/");
-
-        let mut prefix = pattern.clone().to_string();
+        let mut prefix = pattern.clone();
         let mut suffix: Option<String> = Some("".to_owned());
         let maybe_index = pattern.chars().position(|c| c == '*');
         if let Some(index) = maybe_index {
             prefix = pattern[..index].to_string();
             suffix = None;
             if index < pattern.len() - 1 {
                 suffix = Some(pattern[index + 2..].to_string());
             }
         }
         let mut has_more = true;
         let mut token: Option<String> = None;
         while has_more {
+            let (bucket, key) = split_url(&prefix).unwrap();
             let resp = if token.is_some() {
+                log::info!("Listing objects in bucket={}, prefix={}", bucket, key);
                 rt.block_on(
                     s3_client
                         .list_objects_v2()
                         .bucket(bucket)
-                        .prefix(&prefix)
+                        .prefix(key)
                         .delimiter("/")
                         .continuation_token(token.unwrap())
                         .send(),
                 )
                 .unwrap()
             } else {
                 rt.block_on(
                     s3_client
                         .list_objects_v2()
                         .bucket(bucket)
-                        .prefix(&prefix)
+                        .prefix(key)
                         .delimiter("/")
                         .send(),
                 )
                 .unwrap()
             };
             resp.contents().unwrap_or_default().iter().for_each(|obj| {
-                let mut full_output_prefix = output_prefix.clone();
-                full_output_prefix.push_str(obj.key().unwrap());
-                stream_inputs.push(full_output_prefix);
+                let s3_url = format!("s3://{}/{}", bucket, obj.key().unwrap());
+                stream_inputs.push(s3_url);
             });
             suffix.iter().for_each(|s| {
                 resp.common_prefixes()
                     .unwrap_or_default()
                     .iter()
                     .for_each(|sub_folder| {
                         let mut full_path = sub_folder.prefix().unwrap().to_owned();
                         full_path.push_str(s);
-                        let mut full_output_prefix = output_prefix.clone();
-                        full_output_prefix.push_str(&full_path);
-
-                        stream_inputs.push(full_output_prefix);
+                        let s3_url = format!("s3://{}/{}", bucket, full_path);
+                        stream_inputs.push(s3_url);
                     });
             });
             token = resp.next_continuation_token().map(String::from);
             has_more = token.is_some();
         }
         log::info!(
             "Found {} objects for pattern \"{}\"",
@@ -250,40 +246,39 @@
             let actual = actual.unwrap();
             let expected = expected.unwrap();
             assert_eq!(actual, expected);
         }
     }
 
     #[test]
-    fn test_split_path() -> Result<(), ()> {
+    fn test_split_url() -> Result<(), ()> {
         // test case when path is correct
-        let prefix = "s3://my-bucket/my-key";
-        let (bucket, key) = split_path(prefix).unwrap();
+        let prefix = "s3://my-bucket/my-key-dir/my-key";
+        let (bucket, key) = split_url(prefix).unwrap();
         assert_eq!(bucket, "my-bucket");
-        assert_eq!(key, "my-key");
+        assert_eq!(key, "my-key-dir/my-key");
 
         // test case when path is incorrect
         let prefix = "s3:/my-bucket/my-key";
-        let result = split_path(prefix);
+        let result = split_url(prefix);
         assert!(result.is_err());
 
         Ok(())
     }
 
     #[test]
     fn test_object_size() -> Result<(), io::Error> {
         let rt = tokio::runtime::Builder::new_current_thread()
             .enable_all()
             .build()
             .unwrap();
         let s3_client = new_client(None)?;
 
-        let prefix =
-            "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/documents/head/0000.json.gz";
-        let resp = rt.block_on(object_size(&s3_client, prefix));
+        let key = "pretraining-data/tests/mixer/inputs/v0/documents/head/0000.json.gz";
+        let resp = rt.block_on(object_size(&s3_client, "ai2-llm", key));
 
         let size = resp.unwrap();
         assert_eq!(size, 25985);
         Ok(())
     }
 
     #[test]
@@ -292,19 +287,19 @@
             .enable_all()
             .build()
             .unwrap();
         let s3_client = new_client(None)?;
 
         let local_output_file =
             "tests/work/output/pretraining-data/tests/mixer/inputs/v0/documents/head/0000.json.gz";
-        let remote_output_file: &str =
-            "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/documents/head/0000.json.gz";
+        let s3_path: &str = "pretraining-data/tests/mixer/inputs/v0/documents/head/0000.json.gz";
         rt.block_on(download_to_file(
             &s3_client,
-            remote_output_file,
+            "ai2-llm",
+            s3_path,
             Path::new(local_output_file),
         ))?;
 
         compare_contents("tests/data/documents.json.gz", local_output_file);
 
         Ok(())
     }
```

### Comparing `dolma-0.6.2/src/shard.rs` & `dolma-0.6.3/src/shard.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 use std::fs::OpenOptions;
 use std::io;
 use std::io::{BufRead, BufReader, BufWriter, Write};
-use std::path::Path;
+use std::path::{Path, PathBuf};
 
+use aws_sdk_s3::Client as S3Client;
 use flate2::read::MultiGzDecoder;
 use flate2::write::GzEncoder;
 use flate2::Compression;
+use glob::glob;
 use rayon::prelude::*;
 use serde_json::Value;
 
 use crate::s3_util;
-use crate::s3_util::{download_to_file, object_size, upload_file};
 use crate::shard::shard_config::*;
 
 // A shard is a unit of work for the mixer.
 // It is a collection of input files that are combined into a single output file.
 #[derive(Clone)]
 pub struct Shard {
     pub inputs: Vec<DocumentPaths>,
@@ -33,55 +34,38 @@
 
 impl Shard {
     // Partition the input files of a stream into a set of shards.
     // Try to respect the max_size_in_bytes in the configuration, but this is approximate
     // since it doesn't account for the size of any attributes to merged,
     // or documents dropped by the filter.
     pub fn split_streams(streams: &Vec<StreamConfig>) -> Result<Vec<Shard>, io::Error> {
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-        let s3_client = s3_util::new_client(None)?;
-
         let mut shards: Vec<Shard> = Vec::new();
         for stream_config in streams {
             let mut stream_shard_count = 0;
             log::info!("Computing shards for stream {}...", stream_config.name);
-            let stream_inputs =
-                s3_util::find_objects_matching_patterns(&s3_client, &stream_config.documents)?;
-
-            let inputs_with_sizes = stream_inputs
-                .par_iter()
-                .map(|input| {
-                    let resp = rt.block_on(object_size(&s3_client, input));
+            let stream_inputs = find_objects_matching_patterns(&stream_config.documents)?;
+            let input_count = stream_inputs.len();
+            let input_sizes = get_object_sizes(&stream_inputs)?;
+            let inputs_with_sizes = std::iter::zip(stream_inputs, input_sizes)
+                .map(|(input, size)| {
                     let mut attr_paths = Vec::new();
                     for prefix in stream_config.attributes.iter() {
                         let mut attr_prefix = "/attributes/".to_owned();
                         attr_prefix.push_str(prefix);
                         attr_prefix.push_str("/");
-                        let attr_path = input.to_owned().replace("/documents/", &attr_prefix);
+                        let attr_path = input.replace("/documents/", &attr_prefix);
                         attr_paths.push(attr_path);
                     }
-                    match resp {
-                        Ok(size) => (
-                            DocumentPaths {
-                                doc_path: input.to_owned(),
-                                attribute_paths: attr_paths,
-                            },
-                            size,
-                        ),
-                        Err(_) => (
-                            DocumentPaths {
-                                doc_path: input.to_owned(),
-                                attribute_paths: attr_paths,
-                            },
-                            0,
-                        ),
-                    }
+                    (
+                        DocumentPaths {
+                            doc_path: input,
+                            attribute_paths: attr_paths,
+                        },
+                        size,
+                    )
                 })
                 .collect::<Vec<(DocumentPaths, usize)>>();
             let mut shard_size = inputs_with_sizes[0].1;
             let mut shard_inputs: Vec<DocumentPaths> = Vec::new();
             shard_inputs.push(inputs_with_sizes[0].0.clone());
             for (input, size) in inputs_with_sizes[1..].iter() {
                 if *size == 0 {
@@ -124,15 +108,15 @@
                     discard_fields: stream_config.output.discard_fields.clone(),
                 };
                 shards.push(shard);
                 stream_shard_count += 1;
             }
             log::info!(
                 "Splitting {} files for {} into {} shards",
-                stream_inputs.len(),
+                input_count,
                 stream_config.name,
                 stream_shard_count
             );
         }
 
         Ok(shards)
     }
@@ -140,74 +124,54 @@
     // Process a shard:
     // Read all input files sequentially,
     // Merge attributes
     // Apply filters
     // Apply span replacements
     // Upload the output file to S3.
     pub fn process(&self, work_dirs: WorkDirConfig) -> Result<(), io::Error> {
-        let rt = tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build()
-            .unwrap();
-
-        let s3_client = s3_util::new_client(None)?;
-
-        let inputs_dir = Path::new(&work_dirs.input);
-        let outputs_dir = Path::new(&work_dirs.output);
+        let cache = FileCache {
+            s3_client: Box::new(s3_util::new_client(None)?),
+            work: work_dirs.clone(),
+        };
 
-        let output_path = outputs_dir.join(self.output.clone());
-        std::fs::create_dir_all(output_path.parent().unwrap())?;
-
-        let tmp_output_path = outputs_dir.join(self.output.clone() + ".tmp");
+        let output_path = cache.prepare_output(&self.output)?;
         {
             let output_file = OpenOptions::new()
                 .read(false)
                 .write(true)
                 .create(true)
                 .truncate(true)
-                .open(tmp_output_path.clone())?;
+                .open(output_path.clone())?;
 
             let mut writer = BufWriter::with_capacity(
                 1024 * 1024,
                 GzEncoder::new(output_file, Compression::default()),
             );
 
             for input_path in self.inputs.iter() {
                 log::info!("Merging {} into {}", input_path.doc_path, self.output);
-                let local_docs_file = inputs_dir.join(Path::new(&input_path.doc_path));
-                log::info!(
-                    "Downloading {} to {}",
-                    input_path.doc_path,
-                    local_docs_file.display()
-                );
-                rt.block_on(download_to_file(
-                    &s3_client,
-                    &input_path.doc_path,
-                    &local_docs_file,
-                ))?;
+                let local_docs_file = cache.prepare_input(&input_path.doc_path)?;
                 let mut local_attr_readers = Vec::new();
                 let mut attr_reader_failure_counts = Vec::new();
                 for attr in &input_path.attribute_paths {
-                    let local_attr_file = inputs_dir.join(Path::new(&attr));
-                    log::info!("Downloading {} to {}", attr, local_attr_file.display());
-                    rt.block_on(download_to_file(&s3_client, &attr, &local_attr_file))?;
+                    let local_attr_file = cache.prepare_input(&attr)?;
                     let f = OpenOptions::new()
                         .read(true)
                         .write(false)
                         .create(false)
-                        .open(local_attr_file.clone())?;
+                        .open(&local_attr_file)?;
                     let attr_reader = BufReader::with_capacity(1024 * 1024, MultiGzDecoder::new(f));
-                    local_attr_readers.push(attr_reader.lines());
+                    local_attr_readers.push((local_attr_file, attr_reader.lines()));
                     attr_reader_failure_counts.push(0);
                 }
                 let input_file = OpenOptions::new()
                     .read(true)
                     .write(false)
                     .create(false)
-                    .open(local_docs_file.clone())?;
+                    .open(&local_docs_file)?;
                 let reader = BufReader::with_capacity(1024 * 1024, MultiGzDecoder::new(input_file));
 
                 let mut line_number = 0;
                 let mut lines_written = 0;
                 for line in reader.lines() {
                     match line {
                         Ok(_) => {}
@@ -222,15 +186,15 @@
                         }
                     }
                     line_number += 1;
                     let line = line?;
                     let mut data: Value = serde_json::from_str(&line)?;
                     let mut attrs = serde_json::Map::new();
                     let mut attr_reader_index = 0;
-                    for attr_reader in local_attr_readers.iter_mut() {
+                    for (_, attr_reader) in local_attr_readers.iter_mut() {
                         match attr_reader.next() {
                             Some(Ok(line)) => {
                                 let attr_data: Value = serde_json::from_str(&line)?;
                                 assert_eq!(
                                     attr_data["id"], data["id"],
                                     "Mismatched ids for line {} of {}: {} != {}",
                                     line_number, &input_path.doc_path, attr_data["id"], data["id"]
@@ -370,52 +334,34 @@
                             data.as_object_mut().unwrap().remove(f);
                         }
                         lines_written += 1;
                         serde_json::to_writer(&mut writer, &data)?;
                         writer.write_all(b"\n")?;
                     }
                 }
-                std::fs::remove_file(local_docs_file)?;
+                cache.finalize_input(&input_path.doc_path)?;
                 for i in 0..input_path.attribute_paths.len() {
                     if attr_reader_failure_counts[i] > 0 {
                         log::warn!(
                             "Failed to read {} attributes from {}",
                             input_path.attribute_paths[i],
                             attr_reader_failure_counts[i]
                         );
                     }
-                    std::fs::remove_file(
-                        inputs_dir.join(Path::new(&input_path.attribute_paths[i])),
-                    )?;
+                    cache.finalize_input(&input_path.attribute_paths[i])?;
                 }
                 log::info!(
                     "Dropped {} of {} documents from {}",
                     line_number - lines_written,
                     line_number,
                     &input_path.doc_path
                 );
             }
         }
-
-        log::info!(
-            "Uploading {} to {}",
-            &tmp_output_path.display(),
-            &self.output
-        );
-        rt.block_on(upload_file(&s3_client, &self.output, &tmp_output_path))?;
-
-        {
-            // Create empty file to indicate that the shard is done.
-            OpenOptions::new()
-                .create(true)
-                .write(true)
-                .open(&output_path)?;
-            std::fs::remove_file(&tmp_output_path)?;
-        }
-
+        cache.finalize_output(&self.output)?;
         Ok(())
     }
 }
 
 pub mod shard_config {
     use jsonpath_rust::JsonPathFinder;
     use serde::{Deserialize, Serialize};
@@ -527,7 +473,167 @@
                     }
                 }
             }
             Ok(keep)
         }
     }
 }
+
+// Handles input/output files, including S3 downloads/uploads
+pub struct FileCache {
+    pub s3_client: Box<S3Client>,
+    pub work: WorkDirConfig,
+}
+
+macro_rules! cached_s3_location {
+    ($url:expr, $dir:expr) => {{
+        let (bucket, key) = s3_util::split_url($url).unwrap();
+        (bucket, key.clone(), Path::new($dir).join(key.clone()))
+    }};
+}
+
+impl FileCache {
+    // If "location" is a path to a local file that exists, return it
+    // If it is an S3 URL, download the contents to the working input directory, and return the path
+    pub fn prepare_input(&self, location: &str) -> Result<PathBuf, io::Error> {
+        if location.starts_with("s3://") {
+            let (bucket, key, path) = cached_s3_location!(location, &self.work.input);
+            log::info!("Downloading {} to {}", location, path.display());
+            let rt = tokio::runtime::Builder::new_current_thread()
+                .enable_all()
+                .build()
+                .unwrap();
+            rt.block_on(s3_util::download_to_file(
+                &self.s3_client,
+                bucket,
+                &key,
+                &path,
+            ))?;
+            Ok(path.clone())
+        } else {
+            let path = Path::new(location);
+            if path.exists() {
+                Ok(path.to_path_buf())
+            } else {
+                Err(io::Error::new(
+                    io::ErrorKind::Other,
+                    format!("File not found: {}", location),
+                ))
+            }
+        }
+    }
+
+    // If input was downloaded from S3, delete the local cache
+    // Otherwise, do nothing
+    pub fn finalize_input(&self, location: &str) -> Result<(), io::Error> {
+        if location.starts_with("s3://") {
+            let (_, _, path) = cached_s3_location!(location, &self.work.input);
+            std::fs::remove_file(&path)?;
+            Ok(())
+        } else {
+            Ok(())
+        }
+    }
+
+    // If output is an S3 URL, return a path to a new temporary location in the working output directory
+    // If it is a local path, return a ".tmp" path in the same directory
+    pub fn prepare_output(&self, location: &str) -> Result<PathBuf, io::Error> {
+        if location.starts_with("s3://") {
+            let (_, _, path) = cached_s3_location!(location, &self.work.output);
+            std::fs::create_dir_all(path.parent().unwrap())?;
+            Ok(path.clone())
+        } else {
+            let tmp_location = location.to_owned() + ".tmp";
+            let path = Path::new(tmp_location.as_str());
+            std::fs::create_dir_all(path.parent().unwrap())?;
+            Ok(path.to_path_buf())
+        }
+    }
+
+    // If "output" is an S3 URL, upload contents from the temporary file,
+    //      then replace the temporary file with an empty one as a checkpoint
+    // If "output" is a local path, rename the ".tmp" file to the original name
+    pub fn finalize_output(&self, location: &str) -> Result<(), io::Error> {
+        if location.starts_with("s3://") {
+            let (bucket, key, path) = cached_s3_location!(location, &self.work.output);
+            let rt = tokio::runtime::Builder::new_current_thread()
+                .enable_all()
+                .build()
+                .unwrap();
+            rt.block_on(s3_util::upload_file(&self.s3_client, &path, &bucket, &key))?;
+            std::fs::remove_file(&path)?;
+            {
+                // Create empty file to indicate that the shard is done.
+                OpenOptions::new().create(true).write(true).open(&path)?;
+            }
+            Ok(())
+        } else {
+            let tmp_path = location.to_owned() + ".tmp";
+            let tmp_path = Path::new(tmp_path.as_str());
+            std::fs::rename(&tmp_path, &location)?;
+            Ok(())
+        }
+    }
+}
+
+pub fn find_objects_matching_patterns(patterns: &Vec<String>) -> Result<Vec<String>, io::Error> {
+    let s3_url_count = patterns.iter().filter(|p| p.starts_with("s3://")).count();
+    if s3_url_count == 0 {
+        let mut matches = Vec::new();
+        for pattern in patterns.iter() {
+            for entry in
+            glob(pattern).expect(format! {"Invalid file pattern: {}", pattern.clone()}.as_str())
+            {
+                matches.push(entry.unwrap().to_str().unwrap().to_owned());
+            }
+        }
+        Ok(matches)
+    } else if s3_url_count == patterns.len() {
+        let s3_client = s3_util::new_client(None)?;
+        s3_util::find_objects_matching_patterns(&s3_client, patterns)
+    } else {
+        Err(io::Error::new(
+            io::ErrorKind::Other,
+            "Cannot mix S3 and local paths",
+        ))
+    }
+}
+
+// Get the size in bytes of a list of objects, either S3 urls or local file paths
+pub fn get_object_sizes(locations: &Vec<String>) -> Result<Vec<usize>, io::Error> {
+    let s3_url_count = locations.iter().filter(|p| p.starts_with("s3://")).count();
+    if s3_url_count == 0 {
+        let sizes: Vec<usize> = locations
+            .par_iter()
+            .map(|location| {
+                let path = Path::new(location);
+                let metadata = path.metadata().unwrap();
+                metadata.len() as usize
+            })
+            .collect();
+        Ok(sizes)
+    } else if s3_url_count == locations.len() {
+        let s3_client = s3_util::new_client(None)?;
+        let rt = tokio::runtime::Builder::new_current_thread()
+            .enable_all()
+            .build()
+            .unwrap();
+
+        let sizes = locations
+            .par_iter()
+            .map(|location| {
+                let (bucket, key) = s3_util::split_url(location).unwrap();
+                let resp = rt.block_on(s3_util::object_size(&s3_client, &bucket, &key));
+                match resp {
+                    Ok(size) => size,
+                    Err(_) => 0,
+                }
+            })
+            .collect();
+        Ok(sizes)
+    } else {
+        Err(io::Error::new(
+            io::ErrorKind::Other,
+            "Cannot mix S3 and local paths",
+        ))
+    }
+}
```

### Comparing `dolma-0.6.2/tests/config/c4-cleaned.json` & `dolma-0.6.3/tests/config/c4-cleaned.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/config/dedupe-by-url.json` & `dolma-0.6.3/tests/config/dedupe-by-url.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/config/dedupe-paragraphs.json` & `dolma-0.6.3/tests/config/dedupe-paragraphs.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/config/email-spans.json` & `dolma-0.6.3/tests/config/email-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/config/filter-by-spans.json` & `dolma-0.6.3/tests/config/filter-by-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/config/mixer.json` & `dolma-0.6.3/tests/config/mixer.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/config/paragraph-spans.json` & `dolma-0.6.3/tests/config/paragraph-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/documents.json.gz` & `dolma-0.6.3/tests/data/documents.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/duplicate-paragraphs.json.gz` & `dolma-0.6.3/tests/data/duplicate-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/expected/dedupe-paragraphs.json.gz` & `dolma-0.6.3/tests/data/expected/dedupe-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/expected/email-spans.json.gz` & `dolma-0.6.3/tests/data/expected/email-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/expected/filter-by-spans.json.gz` & `dolma-0.6.3/tests/data/expected/filter-by-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/expected/mixer.json.gz` & `dolma-0.6.3/tests/data/expected/mixer.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/expected/remove-paragraphs.json.gz` & `dolma-0.6.3/tests/data/expected/remove-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/pii-attributes.json.gz` & `dolma-0.6.3/tests/data/pii-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/sample-attributes.json.gz` & `dolma-0.6.3/tests/data/sample-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/data/toxicity-attributes.json.gz` & `dolma-0.6.3/tests/data/toxicity-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_data_types.py` & `dolma-0.6.3/tests/python/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_mixer.py` & `dolma-0.6.3/tests/python/test_mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_omegaconf.py` & `dolma-0.6.3/tests/python/test_omegaconf.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_parallel.py` & `dolma-0.6.3/tests/python/test_parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_paths.py` & `dolma-0.6.3/tests/python/test_paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_runtime.py` & `dolma-0.6.3/tests/python/test_runtime.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_taggers.py` & `dolma-0.6.3/tests/python/test_taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/tests/python/test_utils.py` & `dolma-0.6.3/tests/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.2/Cargo.lock` & `dolma-0.6.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -678,23 +678,24 @@
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dolma"
-version = "0.6.2"
+version = "0.6.3"
 dependencies = [
  "ahash",
  "aws-config",
  "aws-sdk-s3",
  "byteorder",
  "clap",
  "env_logger",
  "flate2",
+ "glob",
  "jsonpath-rust",
  "log",
  "pyo3",
  "rand",
  "rayon",
  "regex",
  "serde",
@@ -837,14 +838,20 @@
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "h2"
 version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
```

### Comparing `dolma-0.6.2/PKG-INFO` & `dolma-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolma
-Version: 0.6.2
+Version: 0.6.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: requests
 Requires-Dist: tqdm
```

