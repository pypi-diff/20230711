# Comparing `tmp/easy_tpp-0.0.4.tar.gz` & `tmp/easy_tpp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_tpp-0.0.4.tar", last modified: Sun Jul  2 03:53:02 2023, max compression
+gzip compressed data, was "easy_tpp-0.0.5.tar", last modified: Tue Jul 11 14:05:42 2023, max compression
```

## Comparing `easy_tpp-0.0.4.tar` & `easy_tpp-0.0.5.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/
--rw-rw-r--   0 sissif     (501) staff       (20)    11415 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/LICENCE
--rw-rw-r--   0 sissif     (501) staff       (20)       43 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/MANIFEST.in
--rw-rw-r--   0 sissif     (501) staff       (20)      704 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/NOTICE
--rw-r--r--   0 sissif     (501) staff       (20)      296 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/PKG-INFO
--rw-rw-r--   0 sissif     (501) staff       (20)    12168 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/README.md
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/
--rw-rw-r--   0 sissif     (501) staff       (20)       21 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/__init__.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/config_factory/
--rw-rw-r--   0 sissif     (501) staff       (20)      495 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2801 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/base_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3067 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     5165 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/data_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     4347 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/hpo_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)    10944 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/model_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7723 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/runner_config.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/default_registers/
--rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/default_registers/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1432 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/default_registers/register_metrics.py
--rw-rw-r--   0 sissif     (501) staff       (20)      512 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/default_registers/register_optuna_trials.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/hpo/
--rw-rw-r--   0 sissif     (501) staff       (20)      208 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/hpo/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     4143 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/hpo/base_hpo.py
--rw-rw-r--   0 sissif     (501) staff       (20)    13912 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/hpo/optuna_hpo.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/model/
--rw-rw-r--   0 sissif     (501) staff       (20)     1950 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/__init__.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/
--rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)    15311 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_anhn.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14714 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_attnhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14993 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_baselayer.py
--rw-rw-r--   0 sissif     (501) staff       (20)    11994 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_basemodel.py
--rw-rw-r--   0 sissif     (501) staff       (20)     9485 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_fullynn.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7868 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_intensity_free.py
--rw-rw-r--   0 sissif     (501) staff       (20)    13935 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_nhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14001 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_ode_tpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8575 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_rmtpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    10020 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_sahp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     9178 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thinning.py
--rw-rw-r--   0 sissif     (501) staff       (20)     9361 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thp.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/
--rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)    12246 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_anhn.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14471 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_attnhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8860 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_baselayer.py
--rw-rw-r--   0 sissif     (501) staff       (20)    11617 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_basemodel.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8562 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_fullynn.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8085 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_intensity_free.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14572 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_nhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    11244 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_ode_tpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7765 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_rmtpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8815 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_sahp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    10684 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thinning.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7873 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thp.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/preprocess/
--rw-rw-r--   0 sissif     (501) staff       (20)      216 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1982 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/data_collator.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3217 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/data_loader.py
--rw-rw-r--   0 sissif     (501) staff       (20)     5048 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/dataset.py
--rw-rw-r--   0 sissif     (501) staff       (20)    25680 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/event_tokenizer.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/runner/
--rw-rw-r--   0 sissif     (501) staff       (20)      237 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/runner/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     6416 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/runner/base_runner.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8761 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/runner/tpp_runner.py
--rw-rw-r--   0 sissif     (501) staff       (20)     6201 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/tf_wrapper.py
--rw-rw-r--   0 sissif     (501) staff       (20)     5704 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/torch_wrapper.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/utils/
--rw-rw-r--   0 sissif     (501) staff       (20)     2462 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2166 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/const.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2419 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/generic.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7459 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/import_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1435 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/log_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3333 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/metrics.py
--rw-rw-r--   0 sissif     (501) staff       (20)     6890 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/misc.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2887 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/multiprocess_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2700 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/ode_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7118 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/registrable.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3150 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/tf_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1856 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/torch_utils.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/
--rw-r--r--   0 sissif     (501) staff       (20)      296 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/PKG-INFO
--rw-r--r--   0 sissif     (501) staff       (20)     2471 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/SOURCES.txt
--rw-r--r--   0 sissif     (501) staff       (20)        1 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/dependency_links.txt
--rw-r--r--   0 sissif     (501) staff       (20)       31 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/requires.txt
--rw-r--r--   0 sissif     (501) staff       (20)        9 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/top_level.txt
--rw-rw-r--   0 sissif     (501) staff       (20)       30 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/requirements.txt
--rw-rw-r--   0 sissif     (501) staff       (20)       79 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/setup.cfg
--rw-rw-r--   0 sissif     (501) staff       (20)     1838 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/setup.py
--rw-rw-r--   0 sissif     (501) staff       (20)       22 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/version.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.289689 easy_tpp-0.0.5/
+-rw-rw-rw-   0        0        0    11617 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0       44 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      726 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/NOTICE
+-rw-rw-rw-   0        0        0      355 2023-07-11 14:05:42.289689 easy_tpp-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13036 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.219874 easy_tpp-0.0.5/easy_tpp/
+-rw-rw-rw-   0        0        0       21 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.235174 easy_tpp-0.0.5/easy_tpp/config_factory/
+-rw-rw-rw-   0        0        0      508 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/config_factory/__init__.py
+-rw-rw-rw-   0        0        0     3186 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/config_factory/config.py
+-rw-rw-rw-   0        0        0     5310 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/config_factory/data_config.py
+-rw-rw-rw-   0        0        0     4479 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/config_factory/hpo_config.py
+-rw-rw-rw-   0        0        0    11219 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/config_factory/model_config.py
+-rw-rw-rw-   0        0        0     7907 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/config_factory/runner_config.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.238174 easy_tpp-0.0.5/easy_tpp/default_registers/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/default_registers/__init__.py
+-rw-rw-rw-   0        0        0     1475 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/default_registers/register_metrics.py
+-rw-rw-rw-   0        0        0      525 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/default_registers/register_optuna_trials.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.241175 easy_tpp-0.0.5/easy_tpp/hpo/
+-rw-rw-rw-   0        0        0      213 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/hpo/__init__.py
+-rw-rw-rw-   0        0        0     4274 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/hpo/base_hpo.py
+-rw-rw-rw-   0        0        0    14288 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/hpo/optuna_hpo.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.242175 easy_tpp-0.0.5/easy_tpp/model/
+-rw-rw-rw-   0        0        0     1993 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.255179 easy_tpp-0.0.5/easy_tpp/model/tf_model/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/__init__.py
+-rw-rw-rw-   0        0        0    15645 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_anhn.py
+-rw-rw-rw-   0        0        0    15055 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_attnhp.py
+-rw-rw-rw-   0        0        0    15397 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_baselayer.py
+-rw-rw-rw-   0        0        0    12265 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_basemodel.py
+-rw-rw-rw-   0        0        0     9714 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_fullynn.py
+-rw-rw-rw-   0        0        0     8075 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_intensity_free.py
+-rw-rw-rw-   0        0        0    14270 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_nhp.py
+-rw-rw-rw-   0        0        0    14342 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_ode_tpp.py
+-rw-rw-rw-   0        0        0     8766 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_rmtpp.py
+-rw-rw-rw-   0        0        0    10242 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_sahp.py
+-rw-rw-rw-   0        0        0     9394 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_thinning.py
+-rw-rw-rw-   0        0        0     9573 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_thp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.268684 easy_tpp-0.0.5/easy_tpp/model/torch_model/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/__init__.py
+-rw-rw-rw-   0        0        0    12519 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_anhn.py
+-rw-rw-rw-   0        0        0    14793 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_attnhp.py
+-rw-rw-rw-   0        0        0     9131 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_baselayer.py
+-rw-rw-rw-   0        0        0    11869 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_basemodel.py
+-rw-rw-rw-   0        0        0     8774 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_fullynn.py
+-rw-rw-rw-   0        0        0     8303 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_intensity_free.py
+-rw-rw-rw-   0        0        0    14927 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_nhp.py
+-rw-rw-rw-   0        0        0    11540 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_ode_tpp.py
+-rw-rw-rw-   0        0        0     7948 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_rmtpp.py
+-rw-rw-rw-   0        0        0     9027 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_sahp.py
+-rw-rw-rw-   0        0        0    10916 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_thinning.py
+-rw-rw-rw-   0        0        0     8044 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_thp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.273686 easy_tpp-0.0.5/easy_tpp/preprocess/
+-rw-rw-rw-   0        0        0      222 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2031 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/preprocess/data_collator.py
+-rw-rw-rw-   0        0        0     3305 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/preprocess/data_loader.py
+-rw-rw-rw-   0        0        0     5180 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/preprocess/dataset.py
+-rw-rw-rw-   0        0        0    26237 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/preprocess/event_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.276686 easy_tpp-0.0.5/easy_tpp/runner/
+-rw-rw-rw-   0        0        0      243 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/runner/__init__.py
+-rw-rw-rw-   0        0        0     6611 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/runner/base_runner.py
+-rw-rw-rw-   0        0        0     8986 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/runner/tpp_runner.py
+-rw-rw-rw-   0        0        0     6365 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/tf_wrapper.py
+-rw-rw-rw-   0        0        0     5847 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/torch_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.288689 easy_tpp-0.0.5/easy_tpp/utils/
+-rw-rw-rw-   0        0        0     2521 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/const.py
+-rw-rw-rw-   0        0        0     2525 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/generic.py
+-rw-rw-rw-   0        0        0     7677 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/import_utils.py
+-rw-rw-rw-   0        0        0     1489 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/log_utils.py
+-rw-rw-rw-   0        0        0     3445 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/metrics.py
+-rw-rw-rw-   0        0        0     7141 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/misc.py
+-rw-rw-rw-   0        0        0     3002 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/multiprocess_utils.py
+-rw-rw-rw-   0        0        0     2791 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/ode_utils.py
+-rw-rw-rw-   0        0        0     7274 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/registrable.py
+-rw-rw-rw-   0        0        0     3277 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/tf_utils.py
+-rw-rw-rw-   0        0        0     1930 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/easy_tpp/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:05:42.229173 easy_tpp-0.0.5/easy_tpp.egg-info/
+-rw-rw-rw-   0        0        0      355 2023-07-11 14:05:42.000000 easy_tpp-0.0.5/easy_tpp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-07-11 14:05:42.000000 easy_tpp-0.0.5/easy_tpp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:05:42.000000 easy_tpp-0.0.5/easy_tpp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-11 14:05:42.000000 easy_tpp-0.0.5/easy_tpp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 14:05:42.000000 easy_tpp-0.0.5/easy_tpp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-11 14:05:42.290690 easy_tpp-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1897 2023-07-11 14:03:07.000000 easy_tpp-0.0.5/setup.py
+-rw-rw-rw-   0        0        0       23 2023-07-11 14:05:30.000000 easy_tpp-0.0.5/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `easy_tpp-0.0.4/LICENCE` & `easy_tpp-0.0.5/LICENCE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-Copyright 2022 The EasyTPP Authors.  All rights reserved.
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+Copyright 2022 The EasyTPP Authors.  All rights reserved.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `easy_tpp-0.0.4/NOTICE` & `easy_tpp-0.0.5/NOTICE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-=============================================================
-EasyTPP is a open source tool developed by Machine Intelligence Team
-Copyright (c) 2020-2022, Ant Group Holding Limited.
-Licensed under the Apache License, Version 2.0
-
-=============================================================
-This toolkit contains various third-party components under
-different open source licenses
-
------------------------------
-Training evaluation pipeline
-Apache License, Version 2.0
-FuxiCTR authors
-
-----------------------------
-Training evaluation pipeline
-Apache License, Version 2.0
-EasyNLP, Alibaba Inc.
-
-----------------------------
-Tokenizer and DataLoader
-Apache License, Version 2.0
+=============================================================
+EasyTPP is a open source tool developed by Machine Intelligence Team
+Copyright (c) 2020-2022, Ant Group Holding Limited.
+Licensed under the Apache License, Version 2.0
+
+=============================================================
+This toolkit contains various third-party components under
+different open source licenses
+
+-----------------------------
+Training evaluation pipeline
+Apache License, Version 2.0
+FuxiCTR authors
+
+----------------------------
+Training evaluation pipeline
+Apache License, Version 2.0
+EasyNLP, Alibaba Inc.
+
+----------------------------
+Tokenizer and DataLoader
+Apache License, Version 2.0
 The HuggingFace Inc. team
```

### Comparing `easy_tpp-0.0.4/README.md` & `easy_tpp-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,207 +1,220 @@
-# EasyTPP
-
-![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)
-![](https://img.shields.io/badge/license-Apache-000000.svg)
-![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green) 
-![GitHub last commit](https://img.shields.io/github/last-commit/ant-research/EasyTemporalPointProcess)
-![Stars](https://img.shields.io/github/stars/ant-research/EasyTemporalPointProcess)
-[![PyPI version fury.io](https://badge.fury.io/py/easy-tpp.svg)](https://pypi.python.org/pypi/easy-tpp/)
-[![Downloads](https://pepy.tech/badge/easy-tpp)](https://pepy.tech/project/easy-tpp)
-
-** We are actively updating the repo now. We will try to finish the first version in a few days. **
-
-`EasyTPP` is an easy-to-use development and application toolkit for [Temporal Point Process](https://mathworld.wolfram.com/TemporalPointProcess.html) (TPP), with key features in configurability, compatibility and reproducibility. We hope this project could benefit both researchers and practitioners with the goal of easily customized development and open benchmarking in TPP.
-<span id='top'/>
-
-
-
-| <a href='#features'>Features</a>|<a href='#requirement'>Install</a>  | <a href='#model-list'>Model List</a> | <a href='#dataset'>Dataset</a>  | <a href='#quick-start'>Quick Start</a> | <a href='#doc'>Documentation</a> | <a href='#citation'>Citation</a> |<a href='#acknowledgment'>Acknowledgement</a> | <a href='#star-history'>Star History</a> | 
-
-## News
-<span id='news'/>
-
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [06-22-2023] Our paper [Language Model Can Improve Event Prediction by Few-Shot Abductive Reasoning](https://arxiv.org/abs/2305.16646) is accepted by the [Knowledge and Logical Reasoning Workshop, ICML'2023](https://klr-icml2023.github.io/cfp.html)!
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [05-29-2023] We release ``EasyTPP`` v0.0.1!
-- [12-27-2022] Our paper [Bellman Meets Hawkes: Model-Based Reinforcement Learning via Temporal Point Processes](https://arxiv.org/abs/2201.12569) was accepted by AAAI'2023!
-- [10-01-2022] Our paper [HYPRO: A Hybridly Normalized Probabilistic Model for Long-Horizon Prediction of Event Sequences](https://arxiv.org/abs/2210.01753) was accepted by NeurIPS'2022!
-- [05-01-2022] We started to develop `EasyTPP`.
-
-
-## Features <a href='#top'>[Back to Top]</a>
-<span id='features'/>
-
-- **Configurable and customizable**: models are modularized and configurable，with abstract classes to support developing customized
-  TPP models.
-- **Compatible with both Tensorflow and PyTorch framework**: `EasyTPP` implements two equivalent sets of models, which can
-  be run under Tensorflow (both Tensorflow 1.13.1 and Tensorflow 2.0) and PyTorch 1.7.0+ respectively. While the PyTorch models are more popular among researchers, the compatibility with Tensorflow is important for industrial practitioners.
-- **Reproducible**: all the benchmarks can be easily reproduced.
-- **Hyper-parameter optimization**: a pipeline of [optuna](https://github.com/optuna/optuna)-based HPO is provided.
-
-
-## Model List <a href='#top'>[Back to Top]</a>
-<span id='model-list'/>
-
-We provide reference implementations of various state-of-the-art TPP papers:
-
-| No  | Publication |     Model     | Paper                                                                                                                                    | Implementation                                                                                                             |
-|:---:|:-----------:|:-------------:|:-----------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
-|  1  |   KDD'16    |     RMTPP     | [Recurrent Marked Temporal Point Processes: Embedding Event History to Vector](https://www.kdd.org/kdd2016/papers/files/rpp1081-duA.pdf) | [Tensorflow](easy_tpp/model/tf_model/tf_rmtpp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_rmtpp.py)                   |
-|  2  | NeurIPS'17  |      NHP      | [The Neural Hawkes Process: A Neurally Self-Modulating Multivariate Point Process](https://arxiv.org/abs/1612.09328)                     | [Tensorflow](easy_tpp/model/tf_model/tf_nhp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_nhp.py)                       |
-|  3  | NeurIPS'19  |    FullyNN    | [Fully Neural Network based Model for General Temporal Point Processes](https://arxiv.org/abs/1905.09690)                                | [Tensorflow](easy_tpp/model/tf_model/tf_fullnn.py)<br/>[Torch](easy_tpp/model/torch_model/torch_fullynn.py)                |
-|  4  |   ICML'20   |     SAHP      | [Self-Attentive Hawkes process](https://arxiv.org/abs/1907.07561)                                                                        | [Tensorflow](easy_tpp/model/tf_model/tf_sahp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_sahp.py)                     |
-|  5  |   ICML'20   |      THP      | [Transformer Hawkes process](https://arxiv.org/abs/2002.09291)                                                                           | [Tensorflow](easy_tpp/model/tf_model/tf_thp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_thp.py)                       |
-|  6  |   ICLR'20   | IntensityFree | [Intensity-Free Learning of Temporal Point Processes](https://arxiv.org/abs/1909.12127)                                                  | [Tensorflow](easy_tpp/model/tf_model/tf_intensity_free.py)<br/>[Torch](easy_tpp/model/torch_model/torch_intensity_free.py) |
-|  7  |   ICLR'21   |    ODETPP     | [Neural Spatio-Temporal Point Processes (simplified)](https://arxiv.org/abs/2011.04583)                                                  | [Tensorflow](easy_tpp/model/tf_model/tf_ode_tpp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_ode_tpp.py)               |
-|  8  |   ICLR'22   |    AttNHP     | [Transformer Embeddings of Irregularly Spaced Events and Their Participants](https://arxiv.org/abs/2201.00044)                           | [Tensorflow](easy_tpp/model/tf_model/tf_attnhp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_attnhp.py)                 |
-
-
-
-## Dataset <a href='#top'>[Back to Top]</a>
-<span id='dataset'/>
-
-We preprocessed one synthetic and five real world datasets from widely-cited works that contain diverse characteristics in terms of their application domains and temporal statistics:
-- Synthetic: a univariate Hawkes process simulated by [Tick](https://github.com/X-DataInitiative/tick) library.
-- Retweet ([Zhou, 2013](http://proceedings.mlr.press/v28/zhou13.pdf)): timestamped user retweet events.
-- Taxi ([Whong, 2014](https://chriswhong.com/open-data/foil_nyc_taxi/)): timestamped taxi pick-up events.
-- StackOverflow ([Leskovec, 2014](https://snap.stanford.edu/data/)): timestamped user badge reward events in StackOverflow.
-- Taobao ([Xue et al, 2022](https://arxiv.org/abs/2210.01753)): timestamped user online shopping behavior events in Taobao platform.
-- Amazon ([Amazon Review, 2018](https://nijianmo.github.io/amazon/)): timestamped user online shopping behavior events in Amazon platform.
-
-  All datasets are preprocess to the `Gatech` format dataset widely used for TPP researchers, and saved at [Google Drive](https://drive.google.com/drive/u/0/folders/1f8k82-NL6KFKuNMsUwozmbzDSFycYvz7) with a public access.
-
-## Quick Start <a href='#top'>[Back to Top]</a>
-<span id='quick-start'/>
-
-We provide an end-to-end example for users to run a standard TPP model with `EasyTPP`.
-
-
-### Step 1. Installation
-
-First of all, we can install the package either by using pip or from the source code on Github.
-
-To install the latest stable version:
-```bash
-pip install easy-tpp
-```
-
-To install the latest on GitHub:
-```bash
-git clone https://github.com/ant-research/EasyTemporalPointProcess.git
-cd EasyTemporalPointProcess
-python setup.py install
-```
-
-
-### Step 2. Prepare datasets 
-
-We need to put the datasets in a local directory before running a model and the datasets should follow a certain format. See [OnlineDoc - Datasets](https://ant-research.github.io/EasyTemporalPointProcess/user_guide/dataset.html) for more details.
-
-Suppose we use the [taxi dataset](https://chriswhong.com/open-data/foil_nyc_taxi/) in the example.
-
-### Step 3. Train the model
-
-
-Before start training, we need to set up the config file for the pipeline. We provide a preset config file in [Example Config](https://github.com/ant-research/EasyTemporalPointProcess/blob/main/examples/configs/experiment_config.yaml). The details of the configuration can be found in [OnlineDoc - Training Pipeline](https://ant-research.github.io/EasyTemporalPointProcess/user_guide/run_train_pipeline.html).
-
-After the setup of data and config, the directory structure is as follows:
-
-```bash
-
-    data
-     |______taxi
-             |____ train.pkl
-             |____ dev.pkl
-             |____ test.pkl
-
-    configs
-     |______experiment_config.yaml
-
-```
-
-
-Then we start the training by simply running the script 
-
-```python
-
-import argparse
-from easy_tpp.config_factory import Config
-from easy_tpp.runner import Runner
-
-
-def main():
-    parser = argparse.ArgumentParser()
-
-    parser.add_argument('--config_dir', type=str, required=False, default='configs/experiment_config.yaml',
-                        help='Dir of configuration yaml to train and evaluate the model.')
-
-    parser.add_argument('--experiment_id', type=str, required=False, default='NHP_train',
-                        help='Experiment id in the config file.')
-
-    args = parser.parse_args()
-
-    config = Config.build_from_yaml_file(args.config_dir, experiment_id=args.experiment_id)
-
-    model_runner = Runner.build_from_config(config)
-
-    model_runner.run()
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-A more detailed example can be found at [OnlineDoc - QuickStart](https://ant-research.github.io/EasyTemporalPointProcess/get_started/quick_start.html).
-
-
-## Documentation <a href='#top'>[Back to Top]</a>
-<span id='doc'/>
-
-The classes and methods of `EasyTPP` have been well documented so that users can generate the documentation by:
-
-```shell
-cd doc
-pip install -r requirements.txt
-make html
-```
-NOTE:
-* The `doc/requirements.txt` is only for documentation by Sphinx, which can be automatically generated by Github actions `.github/workflows/docs.yml`. (Trigger by pull request.)
-
-The full documentation is available on the [website](https://ant-research.github.io/EasyTemporalPointProcess/).
- 
-
-## License <a href='#top'>[Back to Top]</a>
-
-This project is licensed under the [Apache License (Version 2.0)](https://github.com/alibaba/EasyNLP/blob/master/LICENSE). This toolkit also contains some code modified from other repos under other open-source licenses. See the [NOTICE](https://github.com/ant-research/EasyTPP/blob/master/NOTICE) file for more information.
-
-
-## Citation <a href='#top'>[Back to Top]</a>
-
-<span id='citation'/>
-
-If you find `EasyTPP` useful for your research or development, please cite the following <a href="https://arxiv.org/abs/2204.05011" target="_blank">paper</a>:
-```
-comming soon
-```
-
-## Acknowledgment <a href='#top'>[Back to Top]</a>
-<span id='acknowledgment'/>
-
-The project is jointly initiated by Machine Intelligence Group, Alipay and DAMO Academy, Alibaba. 
-
-The following repositories are used in `EasyTPP`, either in close to original form or as an inspiration:
-
-- [EasyRec](https://github.com/alibaba/EasyRec)
-- [EasyNLP](https://github.com/alibaba/EasyNLP)
-- [FuxiCTR](https://github.com/xue-pai/FuxiCTR)
-- [Neural Hawkes Process](https://github.com/hongyuanmei/neurawkes)
-- [Neural Hawkes Particle Smoothing](https://github.com/hongyuanmei/neural-hawkes-particle-smoothing)
-- [Attentive Neural Hawkes Process](https://github.com/yangalan123/anhp-andtt)
-- [Huggingface - transformers](https://github.com/huggingface/transformers)
-
-
-## Star History <a href='#top'>[Back to Top]</a>
-<span id='star-history'/>
-
-![Star History Chart](https://api.star-history.com/svg?repos=ant-research/EasyTemporalPointProcess&type=Date)
-
+# EasyTPP
+
+![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)
+![](https://img.shields.io/badge/license-Apache-000000.svg)
+![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green) 
+![GitHub last commit](https://img.shields.io/github/last-commit/ant-research/EasyTemporalPointProcess)
+![Stars](https://img.shields.io/github/stars/ant-research/EasyTemporalPointProcess)
+[![PyPI version fury.io](https://badge.fury.io/py/easy-tpp.svg)](https://pypi.python.org/pypi/easy-tpp/)
+[![Downloads](https://pepy.tech/badge/easy-tpp)](https://pepy.tech/project/easy-tpp)
+
+** We are actively updating the repo now. We will try to finish the first version in a few days. **
+
+`EasyTPP` is an easy-to-use development and application toolkit for [Temporal Point Process](https://mathworld.wolfram.com/TemporalPointProcess.html) (TPP), with key features in configurability, compatibility and reproducibility. We hope this project could benefit both researchers and practitioners with the goal of easily customized development and open benchmarking in TPP.
+<span id='top'/>
+
+
+
+| <a href='#features'>Features</a>  | <a href='#model-list'>Model List</a> | <a href='#dataset'>Dataset</a>  | <a href='#quick-start'>Quick Start</a> | <a href='#benchmark'>Benchmark</a> |<a href='#doc'>Documentation</a> | <a href='#citation'>Citation</a> |<a href='#acknowledgment'>Acknowledgement</a> | <a href='#star-history'>Star History</a> | 
+
+## News
+<span id='news'/>
+
+- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [06-22-2023] Our paper [Language Model Can Improve Event Prediction by Few-Shot Abductive Reasoning](https://arxiv.org/abs/2305.16646) is accepted by the [Knowledge and Logical Reasoning Workshop, ICML'2023](https://klr-icml2023.github.io/cfp.html)!
+- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [05-29-2023] We release ``EasyTPP`` v0.0.1!
+- [12-27-2022] Our paper [Bellman Meets Hawkes: Model-Based Reinforcement Learning via Temporal Point Processes](https://arxiv.org/abs/2201.12569) was accepted by AAAI'2023!
+- [10-01-2022] Our paper [HYPRO: A Hybridly Normalized Probabilistic Model for Long-Horizon Prediction of Event Sequences](https://arxiv.org/abs/2210.01753) was accepted by NeurIPS'2022!
+- [05-01-2022] We started to develop `EasyTPP`.
+
+
+## Features <a href='#top'>[Back to Top]</a>
+<span id='features'/>
+
+- **Configurable and customizable**: models are modularized and configurable，with abstract classes to support developing customized
+  TPP models.
+- **Compatible with both Tensorflow and PyTorch framework**: `EasyTPP` implements two equivalent sets of models, which can
+  be run under Tensorflow (both Tensorflow 1.13.1 and Tensorflow 2.0) and PyTorch 1.7.0+ respectively. While the PyTorch models are more popular among researchers, the compatibility with Tensorflow is important for industrial practitioners.
+- **Reproducible**: all the benchmarks can be easily reproduced.
+- **Hyper-parameter optimization**: a pipeline of [optuna](https://github.com/optuna/optuna)-based HPO is provided.
+
+
+## Model List <a href='#top'>[Back to Top]</a>
+<span id='model-list'/>
+
+We provide reference implementations of various state-of-the-art TPP papers:
+
+| No  | Publication |     Model     | Paper                                                                                                                                    | Implementation                                                                                                             |
+|:---:|:-----------:|:-------------:|:-----------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
+|  1  |   KDD'16    |     RMTPP     | [Recurrent Marked Temporal Point Processes: Embedding Event History to Vector](https://www.kdd.org/kdd2016/papers/files/rpp1081-duA.pdf) | [Tensorflow](easy_tpp/model/tf_model/tf_rmtpp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_rmtpp.py)                   |
+|  2  | NeurIPS'17  |      NHP      | [The Neural Hawkes Process: A Neurally Self-Modulating Multivariate Point Process](https://arxiv.org/abs/1612.09328)                     | [Tensorflow](easy_tpp/model/tf_model/tf_nhp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_nhp.py)                       |
+|  3  | NeurIPS'19  |    FullyNN    | [Fully Neural Network based Model for General Temporal Point Processes](https://arxiv.org/abs/1905.09690)                                | [Tensorflow](easy_tpp/model/tf_model/tf_fullnn.py)<br/>[Torch](easy_tpp/model/torch_model/torch_fullynn.py)                |
+|  4  |   ICML'20   |     SAHP      | [Self-Attentive Hawkes process](https://arxiv.org/abs/1907.07561)                                                                        | [Tensorflow](easy_tpp/model/tf_model/tf_sahp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_sahp.py)                     |
+|  5  |   ICML'20   |      THP      | [Transformer Hawkes process](https://arxiv.org/abs/2002.09291)                                                                           | [Tensorflow](easy_tpp/model/tf_model/tf_thp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_thp.py)                       |
+|  6  |   ICLR'20   | IntensityFree | [Intensity-Free Learning of Temporal Point Processes](https://arxiv.org/abs/1909.12127)                                                  | [Tensorflow](easy_tpp/model/tf_model/tf_intensity_free.py)<br/>[Torch](easy_tpp/model/torch_model/torch_intensity_free.py) |
+|  7  |   ICLR'21   |    ODETPP     | [Neural Spatio-Temporal Point Processes (simplified)](https://arxiv.org/abs/2011.04583)                                                  | [Tensorflow](easy_tpp/model/tf_model/tf_ode_tpp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_ode_tpp.py)               |
+|  8  |   ICLR'22   |    AttNHP     | [Transformer Embeddings of Irregularly Spaced Events and Their Participants](https://arxiv.org/abs/2201.00044)                           | [Tensorflow](easy_tpp/model/tf_model/tf_attnhp.py)<br/>[Torch](easy_tpp/model/torch_model/torch_attnhp.py)                 |
+
+
+
+## Dataset <a href='#top'>[Back to Top]</a>
+<span id='dataset'/>
+
+We preprocessed one synthetic and five real world datasets from widely-cited works that contain diverse characteristics in terms of their application domains and temporal statistics:
+- Synthetic: a univariate Hawkes process simulated by [Tick](https://github.com/X-DataInitiative/tick) library.
+- Retweet ([Zhou, 2013](http://proceedings.mlr.press/v28/zhou13.pdf)): timestamped user retweet events.
+- Taxi ([Whong, 2014](https://chriswhong.com/open-data/foil_nyc_taxi/)): timestamped taxi pick-up events.
+- StackOverflow ([Leskovec, 2014](https://snap.stanford.edu/data/)): timestamped user badge reward events in StackOverflow.
+- Taobao ([Xue et al, 2022](https://arxiv.org/abs/2210.01753)): timestamped user online shopping behavior events in Taobao platform.
+- Amazon ([Amazon Review, 2018](https://nijianmo.github.io/amazon/)): timestamped user online shopping behavior events in Amazon platform.
+
+  All datasets are preprocess to the `Gatech` format dataset widely used for TPP researchers, and saved at [Google Drive](https://drive.google.com/drive/u/0/folders/1f8k82-NL6KFKuNMsUwozmbzDSFycYvz7) with a public access.
+
+## Quick Start <a href='#top'>[Back to Top]</a>
+<span id='quick-start'/>
+
+We provide an end-to-end example for users to run a standard TPP model with `EasyTPP`.
+
+
+### Step 1. Installation
+
+First of all, we can install the package either by using pip or from the source code on Github.
+
+To install the latest stable version:
+```bash
+pip install easy-tpp
+```
+
+To install the latest on GitHub:
+```bash
+git clone https://github.com/ant-research/EasyTemporalPointProcess.git
+cd EasyTemporalPointProcess
+python setup.py install
+```
+
+
+### Step 2. Prepare datasets 
+
+We need to put the datasets in a local directory before running a model and the datasets should follow a certain format. See [OnlineDoc - Datasets](https://ant-research.github.io/EasyTemporalPointProcess/user_guide/dataset.html) for more details.
+
+Suppose we use the [taxi dataset](https://chriswhong.com/open-data/foil_nyc_taxi/) in the example.
+
+### Step 3. Train the model
+
+
+Before start training, we need to set up the config file for the pipeline. We provide a preset config file in [Example Config](https://github.com/ant-research/EasyTemporalPointProcess/blob/main/examples/configs/experiment_config.yaml). The details of the configuration can be found in [OnlineDoc - Training Pipeline](https://ant-research.github.io/EasyTemporalPointProcess/user_guide/run_train_pipeline.html).
+
+After the setup of data and config, the directory structure is as follows:
+
+```bash
+
+    data
+     |______taxi
+             |____ train.pkl
+             |____ dev.pkl
+             |____ test.pkl
+
+    configs
+     |______experiment_config.yaml
+
+```
+
+
+Then we start the training by simply running the script 
+
+```python
+
+import argparse
+from easy_tpp.config_factory import Config
+from easy_tpp.runner import Runner
+
+
+def main():
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument('--config_dir', type=str, required=False, default='configs/experiment_config.yaml',
+                        help='Dir of configuration yaml to train and evaluate the model.')
+
+    parser.add_argument('--experiment_id', type=str, required=False, default='NHP_train',
+                        help='Experiment id in the config file.')
+
+    args = parser.parse_args()
+
+    config = Config.build_from_yaml_file(args.config_dir, experiment_id=args.experiment_id)
+
+    model_runner = Runner.build_from_config(config)
+
+    model_runner.run()
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+A more detailed example can be found at [OnlineDoc - QuickStart](https://ant-research.github.io/EasyTemporalPointProcess/get_started/quick_start.html).
+
+
+## Documentation <a href='#top'>[Back to Top]</a>
+<span id='doc'/>
+
+The classes and methods of `EasyTPP` have been well documented so that users can generate the documentation by:
+
+```shell
+cd doc
+pip install -r requirements.txt
+make html
+```
+NOTE:
+* The `doc/requirements.txt` is only for documentation by Sphinx, which can be automatically generated by Github actions `.github/workflows/docs.yml`. (Trigger by pull request.)
+
+The full documentation is available on the [website](https://ant-research.github.io/EasyTemporalPointProcess/).
+ 
+## Benchmark <a href='#top'>[Back to Top]</a>
+<span id='benchmark'/>
+
+In the [examples](https://github.com/ant-research/EasyTemporalPointProcess/tree/main/examples) folder, we provide a [script](https://github.com/ant-research/EasyTemporalPointProcess/blob/main/examples/benchmark_script.py) to benchmark the TPPs, with Taxi dataset as the input. 
+
+To run the script, one should download the Taxi data following the above instructions. The [config](https://github.com/ant-research/EasyTemporalPointProcess/blob/main/examples/configs/experiment_config.yaml) file is readily setup up. Then run
+
+
+```shell
+cd examples
+python benchmark_script.py
+```
+
+
+## License <a href='#top'>[Back to Top]</a>
+
+This project is licensed under the [Apache License (Version 2.0)](https://github.com/alibaba/EasyNLP/blob/master/LICENSE). This toolkit also contains some code modified from other repos under other open-source licenses. See the [NOTICE](https://github.com/ant-research/EasyTPP/blob/master/NOTICE) file for more information.
+
+
+## Citation <a href='#top'>[Back to Top]</a>
+
+<span id='citation'/>
+
+If you find `EasyTPP` useful for your research or development, please cite the following <a href="https://arxiv.org/abs/2204.05011" target="_blank">paper</a>:
+```
+comming soon
+```
+
+## Acknowledgment <a href='#top'>[Back to Top]</a>
+<span id='acknowledgment'/>
+
+The project is jointly initiated by Machine Intelligence Group, Alipay and DAMO Academy, Alibaba. 
+
+The following repositories are used in `EasyTPP`, either in close to original form or as an inspiration:
+
+- [EasyRec](https://github.com/alibaba/EasyRec)
+- [EasyNLP](https://github.com/alibaba/EasyNLP)
+- [FuxiCTR](https://github.com/xue-pai/FuxiCTR)
+- [Neural Hawkes Process](https://github.com/hongyuanmei/neurawkes)
+- [Neural Hawkes Particle Smoothing](https://github.com/hongyuanmei/neural-hawkes-particle-smoothing)
+- [Attentive Neural Hawkes Process](https://github.com/yangalan123/anhp-andtt)
+- [Huggingface - transformers](https://github.com/huggingface/transformers)
+
+
+## Star History <a href='#top'>[Back to Top]</a>
+<span id='star-history'/>
+
+![Star History Chart](https://api.star-history.com/svg?repos=ant-research/EasyTemporalPointProcess&type=Date)
+
```

#### html2text {}

```diff
@@ -8,17 +8,17 @@
 pepy.tech/badge/easy-tpp)](https://pepy.tech/project/easy-tpp) ** We are
 actively updating the repo now. We will try to finish the first version in a
 few days. ** `EasyTPP` is an easy-to-use development and application toolkit
 for [Temporal Point Process](https://mathworld.wolfram.com/
 TemporalPointProcess.html) (TPP), with key features in configurability,
 compatibility and reproducibility. We hope this project could benefit both
 researchers and practitioners with the goal of easily customized development
-and open benchmarking in TPP.  | Features|Install | Model_List | Dataset |
-Quick_Start | Documentation | Citation |Acknowledgement | Star_History | ##
-News  - ![new](https://img.alicdn.com/imgextra/i4/
+and open benchmarking in TPP.  | Features | Model_List | Dataset | Quick_Start
+| Benchmark |Documentation | Citation |Acknowledgement | Star_History | ## News
+- ![new](https://img.alicdn.com/imgextra/i4/
 O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [06-22-2023] Our paper
 [Language Model Can Improve Event Prediction by Few-Shot Abductive Reasoning]
 (https://arxiv.org/abs/2305.16646) is accepted by the [Knowledge and Logical
 Reasoning Workshop, ICML'2023](https://klr-icml2023.github.io/cfp.html)! - !
 [new](https://img.alicdn.com/imgextra/i4/
 O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [05-29-2023] We
 release ``EasyTPP`` v0.0.1! - [12-27-2022] Our paper [Bellman Meets Hawkes:
@@ -119,26 +119,34 @@
 (https://ant-research.github.io/EasyTemporalPointProcess/get_started/
 quick_start.html). ## Documentation [Back_to_Top]  The classes and methods of
 `EasyTPP` have been well documented so that users can generate the
 documentation by: ```shell cd doc pip install -r requirements.txt make html ```
 NOTE: * The `doc/requirements.txt` is only for documentation by Sphinx, which
 can be automatically generated by Github actions `.github/workflows/docs.yml`.
 (Trigger by pull request.) The full documentation is available on the [website]
-(https://ant-research.github.io/EasyTemporalPointProcess/). ## License [Back_to
-Top] This project is licensed under the [Apache License (Version 2.0)](https://
-github.com/alibaba/EasyNLP/blob/master/LICENSE). This toolkit also contains
-some code modified from other repos under other open-source licenses. See the
-[NOTICE](https://github.com/ant-research/EasyTPP/blob/master/NOTICE) file for
-more information. ## Citation [Back_to_Top]  If you find `EasyTPP` useful for
-your research or development, please cite the following paper: ``` comming soon
-``` ## Acknowledgment [Back_to_Top]  The project is jointly initiated by
-Machine Intelligence Group, Alipay and DAMO Academy, Alibaba. The following
-repositories are used in `EasyTPP`, either in close to original form or as an
-inspiration: - [EasyRec](https://github.com/alibaba/EasyRec) - [EasyNLP](https:
-//github.com/alibaba/EasyNLP) - [FuxiCTR](https://github.com/xue-pai/FuxiCTR) -
-[Neural Hawkes Process](https://github.com/hongyuanmei/neurawkes) - [Neural
-Hawkes Particle Smoothing](https://github.com/hongyuanmei/neural-hawkes-
-particle-smoothing) - [Attentive Neural Hawkes Process](https://github.com/
-yangalan123/anhp-andtt) - [Huggingface - transformers](https://github.com/
-huggingface/transformers) ## Star History [Back_to_Top]  ![Star History Chart]
-(https://api.star-history.com/svg?repos=ant-research/
-EasyTemporalPointProcess&type=Date)
+(https://ant-research.github.io/EasyTemporalPointProcess/). ## Benchmark [Back
+to_Top]  In the [examples](https://github.com/ant-research/
+EasyTemporalPointProcess/tree/main/examples) folder, we provide a [script]
+(https://github.com/ant-research/EasyTemporalPointProcess/blob/main/examples/
+benchmark_script.py) to benchmark the TPPs, with Taxi dataset as the input. To
+run the script, one should download the Taxi data following the above
+instructions. The [config](https://github.com/ant-research/
+EasyTemporalPointProcess/blob/main/examples/configs/experiment_config.yaml)
+file is readily setup up. Then run ```shell cd examples python
+benchmark_script.py ``` ## License [Back_to_Top] This project is licensed under
+the [Apache License (Version 2.0)](https://github.com/alibaba/EasyNLP/blob/
+master/LICENSE). This toolkit also contains some code modified from other repos
+under other open-source licenses. See the [NOTICE](https://github.com/ant-
+research/EasyTPP/blob/master/NOTICE) file for more information. ## Citation
+[Back_to_Top]  If you find `EasyTPP` useful for your research or development,
+please cite the following paper: ``` comming soon ``` ## Acknowledgment [Back
+to_Top]  The project is jointly initiated by Machine Intelligence Group, Alipay
+and DAMO Academy, Alibaba. The following repositories are used in `EasyTPP`,
+either in close to original form or as an inspiration: - [EasyRec](https://
+github.com/alibaba/EasyRec) - [EasyNLP](https://github.com/alibaba/EasyNLP) -
+[FuxiCTR](https://github.com/xue-pai/FuxiCTR) - [Neural Hawkes Process](https:/
+/github.com/hongyuanmei/neurawkes) - [Neural Hawkes Particle Smoothing](https:/
+/github.com/hongyuanmei/neural-hawkes-particle-smoothing) - [Attentive Neural
+Hawkes Process](https://github.com/yangalan123/anhp-andtt) - [Huggingface -
+transformers](https://github.com/huggingface/transformers) ## Star History
+[Back_to_Top]  ![Star History Chart](https://api.star-history.com/
+svg?repos=ant-research/EasyTemporalPointProcess&type=Date)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/config_factory/base_config.py` & `easy_tpp-0.0.5/easy_tpp/config_factory/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,119 @@
-from abc import abstractmethod
-from typing import Any
-
-from easy_tpp.utils import save_yaml_config, load_yaml_config, Registrable, logger
-
-
-class Config(Registrable):
-
-    def save_to_yaml_file(self, fn):
-        """Save the config into the yaml file 'fn'.
-
-        Args:
-            fn (str): Target filename.
-
-        Returns:
-        """
-        yaml_config = self.get_yaml_config()
-        save_yaml_config(fn, yaml_config)
-
-    @staticmethod
-    def build_from_yaml_file(yaml_fn, **kwargs):
-        """Load yaml config file from disk.
-
-        Args:
-            yaml_fn (str): Path of the yaml config file.
-
-        Returns:
-            EasyTPP.Config: Config object corresponding to cls.
-        """
-        config = load_yaml_config(yaml_fn)
-        pipeline_config = config.get('pipeline_config_id')
-        runner_cls = Config.by_name(pipeline_config.lower())
-        logger.critical(f'Load pipeline config class {runner_cls.__name__}')
-        return runner_cls.parse_from_yaml_config(config, **kwargs)
-
-    @abstractmethod
-    def get_yaml_config(self):
-        """Get the yaml format config from self.
-
-        Returns:
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def parse_from_yaml_config(yaml_config, **kwargs):
-        """Parse from the yaml to generate the config object.
-
-        Args:
-            yaml_config (dict): configs from yaml file.
-
-        Returns:
-            EasyTPP.Config: Config class for data.
-        """
-        pass
-
-    @abstractmethod
-    def copy(self):
-        """Get a same and freely modifiable copy of self.
-
-        Returns:
-        """
-        pass
-
-    def __str__(self):
-        """Str representation of the config.
-
-        Returns:
-            str: str representation of the dict format of the config.
-        """
-        return str(self.get_yaml_config())
-
-    def update(self, config, **kwargs):
-        """Update the config.
-
-        Args:
-            config (dict): config dict.
-
-        Returns:
-            EasyTPP.Config: Config class for data.
-        """
-        logger.critical(f'Update config class {self.__class__.__name__}')
-        return self.parse_from_yaml_config(config, **kwargs)
-
-    def pop(self, key: str, default_var: Any):
-        """pop out the key-value item from the config.
-
-        Args:
-            key (str): key name.
-            default_var (Any): default value to pop.
-
-        Returns:
-            Any: value to pop.
-        """
-        return vars(self).pop(key) or default_var
-
-    def get(self, key: str, default_var: Any):
-        """Retrieve the key-value item from the config.
-
-        Args:
-            key (str): key name.
-            default_var (Any): default value to pop.
-
-        Returns:
-            Any: value to get.
-        """
-        return vars(self)[key] or default_var
+from abc import abstractmethod
+from typing import Any
+
+from easy_tpp.utils import save_yaml_config, load_yaml_config, Registrable, logger
+
+
+class Config(Registrable):
+
+    def save_to_yaml_file(self, fn):
+        """Save the config into the yaml file 'fn'.
+
+        Args:
+            fn (str): Target filename.
+
+        Returns:
+        """
+        yaml_config = self.get_yaml_config()
+        save_yaml_config(fn, yaml_config)
+
+    @staticmethod
+    def build_from_yaml_file(yaml_fn, **kwargs):
+        """Load yaml config file from disk.
+
+        Args:
+            yaml_fn (str): Path of the yaml config file.
+
+        Returns:
+            EasyTPP.Config: Config object corresponding to cls.
+        """
+        config = load_yaml_config(yaml_fn)
+        pipeline_config = config.get('pipeline_config_id')
+        config_cls = Config.by_name(pipeline_config.lower())
+        logger.critical(f'Load pipeline config class {config_cls.__name__}')
+        return config_cls.parse_from_yaml_config(config, **kwargs)
+
+    @abstractmethod
+    def get_yaml_config(self):
+        """Get the yaml format config from self.
+
+        Returns:
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def parse_from_yaml_config(yaml_config):
+        """Parse from the yaml to generate the config object.
+
+        Args:
+            yaml_config (dict): configs from yaml file.
+
+        Returns:
+            EasyTPP.Config: Config class for data.
+        """
+        pass
+
+    @abstractmethod
+    def copy(self):
+        """Get a same and freely modifiable copy of self.
+
+        Returns:
+        """
+        pass
+
+    def __str__(self):
+        """Str representation of the config.
+
+        Returns:
+            str: str representation of the dict format of the config.
+        """
+        return str(self.get_yaml_config())
+
+    def update(self, config):
+        """Update the config.
+
+        Args:
+            config (dict): config dict.
+
+        Returns:
+            EasyTPP.Config: Config class for data.
+        """
+        logger.critical(f'Update config class {self.__class__.__name__}')
+        return self.parse_from_yaml_config(config)
+
+    def pop(self, key: str, default_var: Any):
+        """pop out the key-value item from the config.
+
+        Args:
+            key (str): key name.
+            default_var (Any): default value to pop.
+
+        Returns:
+            Any: value to pop.
+        """
+        return vars(self).pop(key) or default_var
+
+    def get(self, key: str, default_var: Any):
+        """Retrieve the key-value item from the config.
+
+        Args:
+            key (str): key name.
+            default_var (Any): default value to pop.
+
+        Returns:
+            Any: value to get.
+        """
+        return vars(self)[key] or default_var
+
+    def set(self, key: str, var_to_set: Any):
+        """Set the key-value item from the config.
+
+        Args:
+            key (str): key name.
+            var_to_set (Any): default value to pop.
+
+        Returns:
+            Any: value to get.
+        """
+        vars(self)[key] = var_to_set
```

### Comparing `easy_tpp-0.0.4/easy_tpp/config_factory/runner_config.py` & `easy_tpp-0.0.5/easy_tpp/config_factory/runner_config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-import copy
-import os
-
-from easy_tpp.config_factory.config import Config
-from easy_tpp.config_factory.data_config import DataConfig
-from easy_tpp.config_factory.model_config import TrainerConfig, ModelConfig, BaseConfig
-from easy_tpp.utils import create_folder, logger, get_unique_id, get_stage, RunnerPhase, \
-    MetricsHelper, DefaultRunnerConfig, py_assert, is_torch_available, is_tf_available, is_tf_gpu_available, \
-    is_torch_gpu_available
-from easy_tpp.utils.const import Backend
-
-
-@Config.register('runner_config')
-class RunnerConfig(Config):
-    def __init__(self, base_config, model_config, data_config, trainer_config):
-        """Initialize the Config class.
-
-        Args:
-            base_config (EasyTPP.BaseConfig): BaseConfig object.
-            model_config (EasyTPP.ModelConfig): ModelConfig object.
-            data_config (EasyTPP.DataConfig): DataConfig object.
-            trainer_config (EasyTPP.TrainerConfig): TrainerConfig object
-        """
-        self.data_config = data_config
-        self.model_config = model_config
-        self.base_config = base_config
-        self.trainer_config = trainer_config
-
-        self.ensure_valid_config()
-        self.update_config()
-
-        # save the complete config
-        save_dir = self.base_config.specs['output_config_dir']
-        self.save_to_yaml_file(save_dir)
-
-        logger.info(f'Save the config to {save_dir}')
-
-    def get_yaml_config(self):
-        """Return the config in dict (yaml compatible) format.
-
-        Returns:
-            dict: config of the runner config in dict format.
-        """
-        return {'data_config': self.data_config.get_yaml_config(),
-                'base_config': self.base_config.get_yaml_config(),
-                'model_config': self.model_config.get_yaml_config(),
-                'trainer_config': self.trainer_config.get_yaml_config()}
-
-    @staticmethod
-    def parse_from_yaml_config(yaml_config, **kwargs):
-        """Parse from the yaml to generate the config object.
-
-        Args:
-            yaml_config (dict): configs from yaml file.
-
-        Returns:
-            RunnerConfig: Config class for trainer specs.
-        """
-        direct_parse = kwargs.get('direct_parse', False)
-        if not direct_parse:
-            exp_id = kwargs.get('experiment_id')
-            yaml_exp_config = yaml_config[exp_id]
-            dataset_id = yaml_exp_config.get('base_config').get('dataset_id')
-            if dataset_id is None:
-                dataset_id = DefaultRunnerConfig.DEFAULT_DATASET_ID
-            try:
-                yaml_data_config = yaml_config['data'][dataset_id]
-            except KeyError:
-                raise RuntimeError('dataset_id={} is not found in config.'.format(dataset_id))
-
-            data_config = DataConfig.parse_from_yaml_config(yaml_data_config)
-            # add exp id to base config
-            yaml_exp_config.get('base_config').update(exp_id=exp_id)
-
-        else:
-            yaml_exp_config = yaml_config
-            data_config = DataConfig.parse_from_yaml_config(yaml_exp_config.get('data_config'))
-
-        base_config = BaseConfig.parse_from_yaml_config(yaml_exp_config.get('base_config'))
-        model_config = ModelConfig.parse_from_yaml_config(yaml_exp_config.get('model_config'))
-        trainer_config = TrainerConfig.parse_from_yaml_config(yaml_exp_config.get('trainer_config'))
-
-        return RunnerConfig(
-            data_config=data_config,
-            base_config=base_config,
-            model_config=model_config,
-            trainer_config=trainer_config
-        )
-
-    def ensure_valid_config(self):
-        """Do some sanity check about the config, to avoid conflicts in settings.
-        """
-
-        # during testing we dont do shuffle by default
-        self.trainer_config.shuffle = False
-
-        # during testing we dont apply tfb by default
-        self.trainer_config.use_tfb = False
-
-        return
-
-    def update_config(self):
-        """Updated config dict.
-        """
-        model_folder_name = get_unique_id()
-
-        log_folder = create_folder(self.base_config.base_dir, model_folder_name)
-        model_folder = create_folder(log_folder, 'models')
-
-        self.base_config.specs['log_folder'] = log_folder
-        self.base_config.specs['saved_model_dir'] = os.path.join(model_folder, 'saved_model')
-        self.base_config.specs['saved_log_dir'] = os.path.join(log_folder, 'log')
-        self.base_config.specs['output_config_dir'] = os.path.join(log_folder,
-                                                                   f'{self.base_config.exp_id}_output.yaml')
-
-        if self.trainer_config.use_tfb:
-            self.base_config.specs['tfb_train_dir'] = create_folder(log_folder, 'tfb_train')
-            self.base_config.specs['tfb_valid_dir'] = create_folder(log_folder, 'tfb_valid')
-
-        current_stage = get_stage(self.base_config.stage)
-        is_training = current_stage == RunnerPhase.TRAIN
-        self.model_config.is_training = is_training
-
-        # update the dataset config => model config
-        self.model_config.num_event_types_pad = self.data_config.data_specs.num_event_types_pad
-        self.model_config.num_event_types = self.data_config.data_specs.num_event_types
-        self.model_config.pad_token_id = self.data_config.data_specs.pad_token_id
-        self.model_config.max_len = self.data_config.data_specs.max_len
-
-        # update base config => model config
-        model_id = self.base_config.model_id
-        self.model_config.model_id = model_id
-
-        if self.base_config.model_id == 'ODETPP' and self.base_config.backend == Backend.TF:
-            py_assert(self.data_config.data_specs.padding_strategy == 'max_length',
-                      ValueError,
-                      'For ODETPP in TensorFlow, we must pad all sequence to '
-                      'the same length (max len of the sequences)!')
-
-        run = current_stage
-        use_torch = self.base_config.backend == Backend.Torch
-        device = 'GPU' if self.trainer_config.gpu >= 0 else 'CPU'
-
-        py_assert(is_torch_available() if use_torch else is_tf_available(), ValueError,
-                  f'Backend {self.base_config.backend} is not supported in the current environment yet !')
-
-        if use_torch and device == 'GPU':
-            py_assert(is_torch_gpu_available(),
-                      ValueError,
-                      f'Torch cuda is not supported in the current environment yet!')
-
-        if not use_torch and device == 'GPU':
-            py_assert(is_tf_gpu_available(),
-                      ValueError,
-                      f'Tensorflow GPU is not supported in the current environment yet!')
-
-        critical_msg = '{run} model {model_name} using {device} ' \
-                       'with {tf_torch} backend'.format(run=run,
-                                                        model_name=model_id,
-                                                        device=device,
-                                                        tf_torch=self.base_config.backend)
-
-        logger.critical(critical_msg)
-
-        return
-
-    def get_metric_functions(self):
-        return MetricsHelper.get_metrics_callback_from_names(self.trainer_config.metrics)
-
-    def get_metric_direction(self, metric_name='rmse'):
-        return MetricsHelper.get_metric_direction(metric_name)
-
-    def copy(self):
-        """Copy the config.
-
-        Returns:
-            RunnerConfig: a copy of current config.
-        """
-        return RunnerConfig(
-            base_config=copy.deepcopy(self.base_config),
-            model_config=copy.deepcopy(self.model_config),
-            data_config=copy.deepcopy(self.data_config),
-            trainer_config=copy.deepcopy(self.trainer_config)
-        )
+import copy
+import os
+
+from easy_tpp.config_factory.config import Config
+from easy_tpp.config_factory.data_config import DataConfig
+from easy_tpp.config_factory.model_config import TrainerConfig, ModelConfig, BaseConfig
+from easy_tpp.utils import create_folder, logger, get_unique_id, get_stage, RunnerPhase, \
+    MetricsHelper, DefaultRunnerConfig, py_assert, is_torch_available, is_tf_available, is_tf_gpu_available, \
+    is_torch_gpu_available
+from easy_tpp.utils.const import Backend
+
+
+@Config.register('runner_config')
+class RunnerConfig(Config):
+    def __init__(self, base_config, model_config, data_config, trainer_config):
+        """Initialize the Config class.
+
+        Args:
+            base_config (EasyTPP.BaseConfig): BaseConfig object.
+            model_config (EasyTPP.ModelConfig): ModelConfig object.
+            data_config (EasyTPP.DataConfig): DataConfig object.
+            trainer_config (EasyTPP.TrainerConfig): TrainerConfig object
+        """
+        self.data_config = data_config
+        self.model_config = model_config
+        self.base_config = base_config
+        self.trainer_config = trainer_config
+
+        self.ensure_valid_config()
+        self.update_config()
+
+        # save the complete config
+        save_dir = self.base_config.specs['output_config_dir']
+        self.save_to_yaml_file(save_dir)
+
+        logger.info(f'Save the config to {save_dir}')
+
+    def get_yaml_config(self):
+        """Return the config in dict (yaml compatible) format.
+
+        Returns:
+            dict: config of the runner config in dict format.
+        """
+        return {'data_config': self.data_config.get_yaml_config(),
+                'base_config': self.base_config.get_yaml_config(),
+                'model_config': self.model_config.get_yaml_config(),
+                'trainer_config': self.trainer_config.get_yaml_config()}
+
+    @staticmethod
+    def parse_from_yaml_config(yaml_config, **kwargs):
+        """Parse from the yaml to generate the config object.
+
+        Args:
+            yaml_config (dict): configs from yaml file.
+
+        Returns:
+            RunnerConfig: Config class for trainer specs.
+        """
+        direct_parse = kwargs.get('direct_parse', False)
+        if not direct_parse:
+            exp_id = kwargs.get('experiment_id')
+            yaml_exp_config = yaml_config[exp_id]
+            dataset_id = yaml_exp_config.get('base_config').get('dataset_id')
+            if dataset_id is None:
+                dataset_id = DefaultRunnerConfig.DEFAULT_DATASET_ID
+            try:
+                yaml_data_config = yaml_config['data'][dataset_id]
+            except KeyError:
+                raise RuntimeError('dataset_id={} is not found in config.'.format(dataset_id))
+
+            data_config = DataConfig.parse_from_yaml_config(yaml_data_config)
+            # add exp id to base config
+            yaml_exp_config.get('base_config').update(exp_id=exp_id)
+
+        else:
+            yaml_exp_config = yaml_config
+            data_config = DataConfig.parse_from_yaml_config(yaml_exp_config.get('data_config'))
+
+        base_config = BaseConfig.parse_from_yaml_config(yaml_exp_config.get('base_config'))
+        model_config = ModelConfig.parse_from_yaml_config(yaml_exp_config.get('model_config'))
+        trainer_config = TrainerConfig.parse_from_yaml_config(yaml_exp_config.get('trainer_config'))
+
+        return RunnerConfig(
+            data_config=data_config,
+            base_config=base_config,
+            model_config=model_config,
+            trainer_config=trainer_config
+        )
+
+    def ensure_valid_config(self):
+        """Do some sanity check about the config, to avoid conflicts in settings.
+        """
+
+        # during testing we dont do shuffle by default
+        self.trainer_config.shuffle = False
+
+        # during testing we dont apply tfb by default
+        self.trainer_config.use_tfb = False
+
+        return
+
+    def update_config(self):
+        """Updated config dict.
+        """
+        model_folder_name = get_unique_id()
+
+        log_folder = create_folder(self.base_config.base_dir, model_folder_name)
+        model_folder = create_folder(log_folder, 'models')
+
+        self.base_config.specs['log_folder'] = log_folder
+        self.base_config.specs['saved_model_dir'] = os.path.join(model_folder, 'saved_model')
+        self.base_config.specs['saved_log_dir'] = os.path.join(log_folder, 'log')
+        self.base_config.specs['output_config_dir'] = os.path.join(log_folder,
+                                                                   f'{self.base_config.exp_id}_output.yaml')
+
+        if self.trainer_config.use_tfb:
+            self.base_config.specs['tfb_train_dir'] = create_folder(log_folder, 'tfb_train')
+            self.base_config.specs['tfb_valid_dir'] = create_folder(log_folder, 'tfb_valid')
+
+        current_stage = get_stage(self.base_config.stage)
+        is_training = current_stage == RunnerPhase.TRAIN
+        self.model_config.is_training = is_training
+
+        # update the dataset config => model config
+        self.model_config.num_event_types_pad = self.data_config.data_specs.num_event_types_pad
+        self.model_config.num_event_types = self.data_config.data_specs.num_event_types
+        self.model_config.pad_token_id = self.data_config.data_specs.pad_token_id
+        self.model_config.max_len = self.data_config.data_specs.max_len
+
+        # update base config => model config
+        model_id = self.base_config.model_id
+        self.model_config.model_id = model_id
+
+        if self.base_config.model_id == 'ODETPP' and self.base_config.backend == Backend.TF:
+            py_assert(self.data_config.data_specs.padding_strategy == 'max_length',
+                      ValueError,
+                      'For ODETPP in TensorFlow, we must pad all sequence to '
+                      'the same length (max len of the sequences)!')
+
+        run = current_stage
+        use_torch = self.base_config.backend == Backend.Torch
+        device = 'GPU' if self.trainer_config.gpu >= 0 else 'CPU'
+
+        py_assert(is_torch_available() if use_torch else is_tf_available(), ValueError,
+                  f'Backend {self.base_config.backend} is not supported in the current environment yet !')
+
+        if use_torch and device == 'GPU':
+            py_assert(is_torch_gpu_available(),
+                      ValueError,
+                      f'Torch cuda is not supported in the current environment yet!')
+
+        if not use_torch and device == 'GPU':
+            py_assert(is_tf_gpu_available(),
+                      ValueError,
+                      f'Tensorflow GPU is not supported in the current environment yet!')
+
+        critical_msg = '{run} model {model_name} using {device} ' \
+                       'with {tf_torch} backend'.format(run=run,
+                                                        model_name=model_id,
+                                                        device=device,
+                                                        tf_torch=self.base_config.backend)
+
+        logger.critical(critical_msg)
+
+        return
+
+    def get_metric_functions(self):
+        return MetricsHelper.get_metrics_callback_from_names(self.trainer_config.metrics)
+
+    def get_metric_direction(self, metric_name='rmse'):
+        return MetricsHelper.get_metric_direction(metric_name)
+
+    def copy(self):
+        """Copy the config.
+
+        Returns:
+            RunnerConfig: a copy of current config.
+        """
+        return RunnerConfig(
+            base_config=copy.deepcopy(self.base_config),
+            model_config=copy.deepcopy(self.model_config),
+            data_config=copy.deepcopy(self.data_config),
+            trainer_config=copy.deepcopy(self.trainer_config)
+        )
```

### Comparing `easy_tpp-0.0.4/easy_tpp/default_registers/register_metrics.py` & `easy_tpp-0.0.5/easy_tpp/default_registers/register_metrics.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import numpy as np
-
-from easy_tpp.utils.const import PredOutputIndex
-from easy_tpp.utils.metrics import MetricsHelper
-
-
-@MetricsHelper.register(name='rmse', direction=MetricsHelper.MINIMIZE, overwrite=False)
-def rmse_metric_function(predictions, labels, **kwargs):
-    """Compute rmse metrics of the time predictions.
-
-    Args:
-        predictions (np.array): model predictions.
-        labels (np.array): ground truth.
-
-    Returns:
-        float: average rmse of the time predictions.
-    """
-    seq_mask = kwargs.get('seq_mask')
-    pred = predictions[PredOutputIndex.TimePredIndex][seq_mask]
-    label = labels[PredOutputIndex.TimePredIndex][seq_mask]
-
-    pred = np.reshape(pred, [-1])
-    label = np.reshape(label, [-1])
-    return np.sqrt(np.mean((pred - label) ** 2))
-
-
-@MetricsHelper.register(name='acc', direction=MetricsHelper.MAXIMIZE, overwrite=False)
-def acc_metric_function(predictions, labels, **kwargs):
-    """Compute accuracy ratio metrics of the type predictions.
-
-    Args:
-        predictions (np.array): model predictions.
-        labels (np.array): ground truth.
-
-    Returns:
-        float: accuracy ratio of the type predictions.
-    """
-    seq_mask = kwargs.get('seq_mask')
-    pred = predictions[PredOutputIndex.TypePredIndex][seq_mask]
-    label = labels[PredOutputIndex.TypePredIndex][seq_mask]
-    pred = np.reshape(pred, [-1])
-    label = np.reshape(label, [-1])
-    return np.mean(pred == label)
+import numpy as np
+
+from easy_tpp.utils.const import PredOutputIndex
+from easy_tpp.utils.metrics import MetricsHelper
+
+
+@MetricsHelper.register(name='rmse', direction=MetricsHelper.MINIMIZE, overwrite=False)
+def rmse_metric_function(predictions, labels, **kwargs):
+    """Compute rmse metrics of the time predictions.
+
+    Args:
+        predictions (np.array): model predictions.
+        labels (np.array): ground truth.
+
+    Returns:
+        float: average rmse of the time predictions.
+    """
+    seq_mask = kwargs.get('seq_mask')
+    pred = predictions[PredOutputIndex.TimePredIndex][seq_mask]
+    label = labels[PredOutputIndex.TimePredIndex][seq_mask]
+
+    pred = np.reshape(pred, [-1])
+    label = np.reshape(label, [-1])
+    return np.sqrt(np.mean((pred - label) ** 2))
+
+
+@MetricsHelper.register(name='acc', direction=MetricsHelper.MAXIMIZE, overwrite=False)
+def acc_metric_function(predictions, labels, **kwargs):
+    """Compute accuracy ratio metrics of the type predictions.
+
+    Args:
+        predictions (np.array): model predictions.
+        labels (np.array): ground truth.
+
+    Returns:
+        float: accuracy ratio of the type predictions.
+    """
+    seq_mask = kwargs.get('seq_mask')
+    pred = predictions[PredOutputIndex.TypePredIndex][seq_mask]
+    label = labels[PredOutputIndex.TypePredIndex][seq_mask]
+    pred = np.reshape(pred, [-1])
+    label = np.reshape(label, [-1])
+    return np.mean(pred == label)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/hpo/base_hpo.py` & `easy_tpp-0.0.5/easy_tpp/hpo/base_hpo.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-from abc import abstractmethod
-from collections import defaultdict
-from typing import List
-
-from easy_tpp.utils import logger, Registrable
-
-
-class HyperTuner(Registrable):
-    _trial_register_center = defaultdict(dict)
-
-    def __init__(self, config, trial_end_callbacks: List[callable] = None):
-        """Initialize the tuner
-
-        Args:
-            config (EasyTPP.Config): config class
-            trial_end_callbacks (List[callable]): List of callback functions to be executed after each trial.
-        """
-        self.config = config
-        self.trial_end_callbacks = trial_end_callbacks or []
-        logger.info(f'Storage of hpo framework: {self.config.hpo_config.storage_uri}')
-
-    @abstractmethod
-    def get_all_best_runner_configs(self):
-        pass
-
-    @abstractmethod
-    def get_best_runner_config_by_name(self, runner_id):
-        """
-
-        Args:
-            runner_id (str):
-
-        Returns:
-
-        """
-        pass
-
-    @abstractmethod
-    def get_num_remain_trials_by_name(self, runner_id):
-        pass
-
-    @staticmethod
-    def build_from_config(config, trial_end_callbacks: List[callable] = None):
-        """Load yaml config file from disk.
-
-        Args:
-            config (EasyTPP.Config): config class
-            trial_end_callbacks (List[callable]): List of callback functions to be executed after each trial.
-
-        Returns:
-            EasyTPP.Config: Config object corresponding to cls.
-        """
-        runner_cls = HyperTuner.by_name(config.hpo_config.framework_id)
-        return runner_cls(config, trial_end_callbacks)
-
-    # ---------------------- Trail Register and Get Functions ---------------------
-
-    @classmethod
-    def register_trial_func(cls, model_id, overwrite=True):
-        """Register the trial functions in HPO
-
-        Args:
-            model_id (str): id of the models.
-            overwrite (bool, optional): whether to overwrite the trial function. Defaults to True.
-
-        Returns:
-            dict: the registered trial function
-        """
-        register_center = HyperTuner._trial_register_center
-
-        def _register_trial(func):
-            if model_id in register_center[cls]:
-                if overwrite:
-                    register_center[cls][model_id] = func
-                    logger.info(f'The trial for {model_id} is already registered, but overwrite it.')
-                else:
-                    logger.warn(f'The trial for {model_id} is already registered, and cannot be overwritten!')
-            else:
-                register_center[cls][model_id] = func
-                logger.info(f'Trial register: {cls.get_registered_name()} - {model_id}')
-            return func
-
-        return _register_trial
-
-    @classmethod
-    def retrieve_trial_func_by_model_name(cls, name):
-        """Retrieve the trail function by the model id
-
-        Args:
-            name (str): model id.
-
-        Raises:
-            RuntimeError: non registered error for the hpo framework.
-
-        Returns:
-            dict: registered trial center
-        """
-        cls_trial_rc = HyperTuner._trial_register_center[cls]
-        if name not in cls_trial_rc:
-            if 'default' in cls_trial_rc:
-                logger.warn(
-                    f'Trial for {name} in {cls.get_registered_name()} is not existed, and use default trial!'
-                )
-                name = 'default'
-            else:
-                raise RuntimeError(f'This HPO Framework is not registered!')
-        return cls_trial_rc[name]
-
-    @classmethod
-    def get_registered_name(cls):
-        """Get the name of the registered hpo class.
-
-        Returns:
-            str: the name of the registered hpo class.
-        """
-        hpo_rc = HyperTuner.registry_dict()
-        for registered_name, hpo_cls in hpo_rc.items():
-            if cls in hpo_cls:
-                return registered_name
-
-        logger.warn(f'The hpo framework is not registered: {cls}')
-        return None
-
-    @abstractmethod
-    def run(self):
-        """Run the process.
-
-        Raises:
-            NotImplementedError: error raised in base class.
-        """
-        raise NotImplementedError
+from abc import abstractmethod
+from collections import defaultdict
+from typing import List
+
+from easy_tpp.utils import logger, Registrable
+
+
+class HyperTuner(Registrable):
+    _trial_register_center = defaultdict(dict)
+
+    def __init__(self, config, trial_end_callbacks: List[callable] = None):
+        """Initialize the tuner
+
+        Args:
+            config (EasyTPP.Config): config class
+            trial_end_callbacks (List[callable]): List of callback functions to be executed after each trial.
+        """
+        self.config = config
+        self.trial_end_callbacks = trial_end_callbacks or []
+        logger.info(f'Storage of hpo framework: {self.config.hpo_config.storage_uri}')
+
+    @abstractmethod
+    def get_all_best_runner_configs(self):
+        pass
+
+    @abstractmethod
+    def get_best_runner_config_by_name(self, runner_id):
+        """
+
+        Args:
+            runner_id (str):
+
+        Returns:
+
+        """
+        pass
+
+    @abstractmethod
+    def get_num_remain_trials_by_name(self, runner_id):
+        pass
+
+    @staticmethod
+    def build_from_config(config, trial_end_callbacks: List[callable] = None):
+        """Load yaml config file from disk.
+
+        Args:
+            config (EasyTPP.Config): config class
+            trial_end_callbacks (List[callable]): List of callback functions to be executed after each trial.
+
+        Returns:
+            EasyTPP.Config: Config object corresponding to cls.
+        """
+        runner_cls = HyperTuner.by_name(config.hpo_config.framework_id)
+        return runner_cls(config, trial_end_callbacks)
+
+    # ---------------------- Trail Register and Get Functions ---------------------
+
+    @classmethod
+    def register_trial_func(cls, model_id, overwrite=True):
+        """Register the trial functions in HPO
+
+        Args:
+            model_id (str): id of the models.
+            overwrite (bool, optional): whether to overwrite the trial function. Defaults to True.
+
+        Returns:
+            dict: the registered trial function
+        """
+        register_center = HyperTuner._trial_register_center
+
+        def _register_trial(func):
+            if model_id in register_center[cls]:
+                if overwrite:
+                    register_center[cls][model_id] = func
+                    logger.info(f'The trial for {model_id} is already registered, but overwrite it.')
+                else:
+                    logger.warn(f'The trial for {model_id} is already registered, and cannot be overwritten!')
+            else:
+                register_center[cls][model_id] = func
+                logger.info(f'Trial register: {cls.get_registered_name()} - {model_id}')
+            return func
+
+        return _register_trial
+
+    @classmethod
+    def retrieve_trial_func_by_model_name(cls, name):
+        """Retrieve the trail function by the model id
+
+        Args:
+            name (str): model id.
+
+        Raises:
+            RuntimeError: non registered error for the hpo framework.
+
+        Returns:
+            dict: registered trial center
+        """
+        cls_trial_rc = HyperTuner._trial_register_center[cls]
+        if name not in cls_trial_rc:
+            if 'default' in cls_trial_rc:
+                logger.warn(
+                    f'Trial for {name} in {cls.get_registered_name()} is not existed, and use default trial!'
+                )
+                name = 'default'
+            else:
+                raise RuntimeError(f'This HPO Framework is not registered!')
+        return cls_trial_rc[name]
+
+    @classmethod
+    def get_registered_name(cls):
+        """Get the name of the registered hpo class.
+
+        Returns:
+            str: the name of the registered hpo class.
+        """
+        hpo_rc = HyperTuner.registry_dict()
+        for registered_name, hpo_cls in hpo_rc.items():
+            if cls in hpo_cls:
+                return registered_name
+
+        logger.warn(f'The hpo framework is not registered: {cls}')
+        return None
+
+    @abstractmethod
+    def run(self):
+        """Run the process.
+
+        Raises:
+            NotImplementedError: error raised in base class.
+        """
+        raise NotImplementedError
```

### Comparing `easy_tpp-0.0.4/easy_tpp/hpo/optuna_hpo.py` & `easy_tpp-0.0.5/easy_tpp/hpo/optuna_hpo.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-import logging
-import os
-import sys
-
-import optuna
-from optuna.samplers import TPESampler
-from optuna.trial import TrialState
-
-from easy_tpp.config_factory import RunnerConfig
-from easy_tpp.hpo.base_hpo import HyperTuner
-from easy_tpp.preprocess import TPPDataLoader
-from easy_tpp.runner import Runner
-from easy_tpp.utils import Timer, dict_deep_update
-from easy_tpp.utils.log_utils import get_logger
-
-optuna.logging.get_logger("optuna").addHandler(logging.StreamHandler(sys.stdout))
-logger = get_logger('optuna_hpo')
-
-
-@HyperTuner.register(name='optuna')
-class OptunaTuner(HyperTuner):
-    def __init__(self, config, trial_end_callbacks):
-        """Initialize the Optuna Tuner class.
-
-        Args:
-            config (EasyTPP.Config): config class.
-            trial_end_callbacks (list): list of trial callbacks.
-        """
-        super(OptunaTuner, self).__init__(config, trial_end_callbacks)
-
-        # fetch db storage from the given storage_uri
-        self.storage_fn = self._fetch_storage()
-
-        # optuna db storage uri
-        self.storage = 'sqlite:///{}'.format(self.storage_fn) if self.storage_fn else None
-
-        self.runner_config = self.config.runner_config
-        self.hpo_config = self.config.hpo_config
-
-        # build data reader
-        data_config = self.runner_config.data_config
-        backend = self.runner_config.base_config.backend
-        kwargs = self.runner_config.trainer_config.get_yaml_config()
-        self._data_loader = TPPDataLoader(
-            data_config=data_config,
-            backend=backend,
-            **kwargs
-        )
-
-    def get_all_best_runner_configs(self):
-        """Get all best runner configs. Obtain from storage.
-
-        Returns:
-            Dict[str, EasyTPP.RunnerConfig]: Dict of all best runner configs.
-        """
-        runner_configs = {}
-        for study_summary in optuna.get_all_study_summaries(self.storage):
-            runner_configs[study_summary.study_name] = self._build_runner_config_from_storage(
-                study=study_summary,
-                trial=study_summary.best_trial
-            )
-        return runner_configs
-
-    def get_best_runner_config_by_name(self, exp_id):
-        """Get the best runner config by runner_id. Obtain it from storage.
-
-        Args:
-            exp_id (str): experiment id.
-
-        Returns:
-            EasyTPP.RunnerConfig: best runner config.
-        """
-        for study_summary in optuna.get_all_study_summaries(self.storage):
-            if exp_id == study_summary.study_name:
-                return self._build_runner_config_from_storage(study_summary, study_summary.best_trial)
-        return None
-
-    def get_num_remain_trials_by_name(self, exp_id):
-        """Get the num of remaining trails by experiment id.
-
-        Args:
-            exp_id (str): experiment id.
-
-        Returns:
-            int: num of remaining trails.
-        """
-        for study_summary in optuna.get_all_study_summaries(self.storage):
-            if exp_id == study_summary.study_name:
-                study = optuna.load_study(study_name=exp_id, storage=self.storage)
-                num_completed_trials = len(study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)))
-                num_remain_trials = self.hpo_config.num_trials - num_completed_trials
-                return num_remain_trials
-        return self.hpo_config.num_trials
-
-    def optimize(
-            self,
-            base_runner_config,
-            train_loader,
-            valid_loader,
-            test_loader=None,
-            exp_id=None,
-            **kwargs
-    ):
-        """Run the optimization process.
-
-        Args:
-            base_runner_config (EasyTPP.RunnerConfig): runner config.
-            train_loader (EasyTPP.DataLoader): train data loader.
-            valid_loader (EasyTPP.DataLoader): valid data loader
-            test_loader (EasyTPP.DataLoader, optional): test data loader. Defaults to None.
-            exp_id (str, optional): experiment id. Defaults to None.
-
-        Raises:
-            RuntimeError: best trial is not found.
-
-        Returns:
-            tuple: best_metric and best_runner_config
-        """
-        # obtain parameters
-        storage = self.storage
-        load_if_exists = self.hpo_config.is_continuous
-        metric_direction = base_runner_config.get_metric_direction()
-
-        # delete the study if it already existed when 'is_continue' is false
-        if not load_if_exists and exp_id is not None:
-            if exp_id in [std_summary.study_name for std_summary in optuna.get_all_study_summaries(storage)]:
-                optuna.delete_study(
-                    study_name=exp_id,
-                    storage=storage
-                )
-        # create hpo study
-        study = optuna.create_study(
-            storage=storage,
-            direction=metric_direction,
-            load_if_exists=load_if_exists,
-            study_name=exp_id,
-            sampler=TPESampler(seed=9899),
-        )
-
-        # set user_attr to study
-        study.set_user_attr('data_config', base_runner_config.data_config.get_yaml_config())
-
-        # calculate the number of remaining trials
-        num_completed_trials = len(study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)))
-        num_remain_trials = self.hpo_config.num_trials - num_completed_trials
-        if num_remain_trials > 0:
-            logger.info(f'Number of hpo trials completed for runner {exp_id}: '
-                        f'{num_completed_trials}/{self.hpo_config.num_trials}')
-            objective_func = self._get_objective_func(
-                base_runner_config=base_runner_config,
-                train_loader=train_loader,
-                valid_loader=valid_loader,
-                test_loader=test_loader,
-                **kwargs
-            )
-            # hpo optimize
-            study.optimize(
-                objective_func,
-                n_trials=num_remain_trials,
-                callbacks=[self._optimize_trial_end],
-                gc_after_trial=True,
-                n_jobs=self.hpo_config.num_jobs,
-            )
-
-        # statistics of this hpo
-        pruned_trials = study.get_trials(deepcopy=False, states=(TrialState.PRUNED,))
-        complete_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
-        logger.info("HPO - Optuna statistics:")
-        logger.info(f"\tNumber of finished trials: {len(study.trials)}")
-        logger.info(f"\tNumber of pruned trials: {len(pruned_trials)}")
-        logger.info(f"\tNumber of complete trials: {len(complete_trials)}")
-
-        if len(study.best_trials) == 0:
-            raise RuntimeError('Best trial is not found, please check the model or metric.')
-        trial = study.best_trial
-        logger.info(f"HPO - Best metric value ({metric_direction}): {trial.value}")
-
-        logger.info(f"Best Parameters: ")
-        for key, value in trial.params.items():
-            logger.info(f"\t{key}: {value}")
-
-        best_metric = trial.value
-        best_runner_config = RunnerConfig.parse_from_yaml_config(
-            trial.user_attrs['runner_config'],
-            data_config=base_runner_config.data_config,
-        )
-        return best_metric, best_runner_config
-
-    def _get_objective_func(
-            self,
-            base_runner_config,
-            **kwargs,
-    ):
-        """Get the optimization objective function.
-
-        Args:
-            base_runner_config (EasyTPP.Config): runner config.
-
-        Raises:
-            e: RuntimeError
-            optuna.TrialPruned: message in trials.
-
-        Returns:
-            _type_: _description_
-        """
-        trial_func = self.retrieve_trial_func_by_model_name(base_runner_config.base_config.exp_id)
-
-        def objective(trial):
-            timer = Timer()
-            timer.start()
-            logger.info(f'Start the trial {trial.number} ...')
-            # get a copy of base runner config for isolation
-            # generate new runner  runners
-            runner_config = base_runner_config.copy()
-
-            trial_model_info = trial_func(
-                trial,
-                trainder_config=runner_config.trainer_config,
-                model_config=runner_config.model_config
-            )
-
-            # use predefined trial to update model_info
-            runner_config_dict = dict_deep_update(
-                target=runner_config.get_yaml_config(),
-                source=trial_model_info,
-                is_add_new_key=False)
-
-            # eval the "suggest" in runner_config (actually run trial suggestion)
-            runner_config_dict = self._eval_str_trial_to_dict(trial,
-                                                              runner_config_dict)
-
-            runner_config = RunnerConfig.parse_from_yaml_config(runner_config_dict, direct_parse=True)
-
-            runner = Runner.build_from_config(
-                runner_config=runner_config,
-                unique_model_dir=True,
-                skip_data_loader=True,
-            )
-            try:
-                # train model
-                runner.train(**kwargs)
-                # evaluate model
-                metric = runner.evaluate(trial=trial, **kwargs)
-                # save the final model
-                runner.save()
-            except RuntimeError as e:
-                # add the error message into trial
-                err_msg = str(e)
-                trial.set_user_attr("error", err_msg)
-
-                logger.error(f'Error in the trial {trial.number}: {err_msg}')
-
-                # just prune the errors like 'out of memory'
-                if 'out of memory' not in err_msg:
-                    raise e
-                raise optuna.TrialPruned()
-            finally:
-                # add model path into trial
-                trial.set_user_attr("model_dir", runner.runner_config.model_dir)
-                # trial.set_user_attr("model_config", runner.runner_config.model_config)
-                trial.set_user_attr("runner_config", runner.runner_config.get_yaml_config())
-
-                logger.info(f'End trial {trial.number} ! Cost time: {timer.end()}')
-
-            return metric
-
-        return objective
-
-    def _optimize_trial_end(self, study, trial):
-        """End the process of trials.
-
-        Args:
-            study (optuna.study.Study): an object of optuna :class:`~optuna.study` to be studied during optimization.
-            trial (optuna.trial.FrozenTrial): an object of optuna :class:`~optuna.trial` that stores trial information.
-        """
-        # push storage to the specified uri
-        self._push_storage(trial)
-
-        is_best_yet = (trial in study.best_trials)
-
-        runner_id = study.study_name
-        runner_config = self._build_runner_config_from_storage(study, trial)
-
-        # invoke callbacks
-        for callback in self.trial_end_callbacks:
-            callback(runner_id, runner_config, is_best_yet)
-
-        # clean disk
-        if not is_best_yet and os.path.exists(trial.user_attrs['model_dir']):
-            os.system(f"rm -fr {trial.user_attrs['model_dir']}")
-
-    def _eval_str_trial_to_dict(self, trial, a_dict):
-        for key, val in a_dict.items():
-            if type(val) == str and val.startswith('suggest_'):
-                idx = val.find('(')
-                prefix = val[:idx + 1]
-                suffix = val[idx + 1:]
-
-                # get trial variable name
-                trial_name = [k for k, v in locals().items() if v == trial][0]
-
-                code = '''{0}.{1}"{2}",{3}'''.format(trial_name, prefix, key, suffix)
-                a_dict[key] = eval(code)
-            elif type(val) == dict:
-                self._eval_str_trial_to_dict(trial, a_dict[key])
-
-        return a_dict
-
-    def _build_runner_config_from_storage(
-            self,
-            study,
-            trial
-    ):
-        """Initialize the RunnerConfig from the study and trial.
-
-        Args:
-            study (optuna.study.Study): an object of optuna :class:`~optuna.study` to be studied during optimization.
-            trial (optuna.trial.FrozenTrial): an object of optuna :class:`~optuna.trial` that stores trial information.
-
-        Returns:
-            EasyTPP.Config: RunnerConfig object.
-        """
-        runner_config_dict = trial.user_attrs['runner_config']
-        return RunnerConfig.parse_from_yaml_config(runner_config_dict, direct_parse=True)
-
-    def run(self):
-        """Run the HPO process.
-
-        Returns:
-            tuple: best_metric, best_runner_config
-        """
-        # to avoid to load unused data
-        train_loader, valid_loader, test_loader = None, None, None
-        exp_id = self.runner_config.base_config.exp_id
-
-        if self.get_num_remain_trials_by_name(exp_id) > 0:
-            train_loader = self._data_loader.get_loader(split='train')
-            valid_loader = self._data_loader.get_loader(split='dev')
-            if self.runner_config.data_config.test_dir is not None:
-                test_loader = self._data_loader.get_loader(split='test')
-
-        best_metric, best_runner_config = self.optimize(
-            base_runner_config=self.runner_config,
-            train_loader=train_loader,
-            valid_loader=valid_loader,
-            test_loader=test_loader,
-            exp_id=exp_id
-        )
-
-        return best_metric, best_runner_config
-
-    def _fetch_storage(self):
-        """Retrieve the stored model.
-
-        Returns:
-            str: dir of the stored model.
-        """
-        local_storage_fn = self.config.hpo_config.storage_path
-
-        # return the local storage location
-        return local_storage_fn
-
-    def _push_storage(self, trial):
-        """_summary_
-
-        Args:
-            trial (_type_): _description_
-
-        Raises:
-            NotImplementedError: _description_
-        """
-        # save hpo storage to remote if it's in remote
-        if self.config.hpo_config.storage_protocol == 'oss':
-            raise NotImplementedError
-
-        return
+import logging
+import os
+import sys
+
+import optuna
+from optuna.samplers import TPESampler
+from optuna.trial import TrialState
+
+from easy_tpp.config_factory import RunnerConfig
+from easy_tpp.hpo.base_hpo import HyperTuner
+from easy_tpp.preprocess import TPPDataLoader
+from easy_tpp.runner import Runner
+from easy_tpp.utils import Timer, dict_deep_update
+from easy_tpp.utils.log_utils import get_logger
+
+optuna.logging.get_logger("optuna").addHandler(logging.StreamHandler(sys.stdout))
+logger = get_logger('optuna_hpo')
+
+
+@HyperTuner.register(name='optuna')
+class OptunaTuner(HyperTuner):
+    def __init__(self, config, trial_end_callbacks):
+        """Initialize the Optuna Tuner class.
+
+        Args:
+            config (EasyTPP.Config): config class.
+            trial_end_callbacks (list): list of trial callbacks.
+        """
+        super(OptunaTuner, self).__init__(config, trial_end_callbacks)
+
+        # fetch db storage from the given storage_uri
+        self.storage_fn = self._fetch_storage()
+
+        # optuna db storage uri
+        self.storage = 'sqlite:///{}'.format(self.storage_fn) if self.storage_fn else None
+
+        self.runner_config = self.config.runner_config
+        self.hpo_config = self.config.hpo_config
+
+        # build data reader
+        data_config = self.runner_config.data_config
+        backend = self.runner_config.base_config.backend
+        kwargs = self.runner_config.trainer_config.get_yaml_config()
+        self._data_loader = TPPDataLoader(
+            data_config=data_config,
+            backend=backend,
+            **kwargs
+        )
+
+    def get_all_best_runner_configs(self):
+        """Get all best runner configs. Obtain from storage.
+
+        Returns:
+            Dict[str, EasyTPP.RunnerConfig]: Dict of all best runner configs.
+        """
+        runner_configs = {}
+        for study_summary in optuna.get_all_study_summaries(self.storage):
+            runner_configs[study_summary.study_name] = self._build_runner_config_from_storage(
+                study=study_summary,
+                trial=study_summary.best_trial
+            )
+        return runner_configs
+
+    def get_best_runner_config_by_name(self, exp_id):
+        """Get the best runner config by runner_id. Obtain it from storage.
+
+        Args:
+            exp_id (str): experiment id.
+
+        Returns:
+            EasyTPP.RunnerConfig: best runner config.
+        """
+        for study_summary in optuna.get_all_study_summaries(self.storage):
+            if exp_id == study_summary.study_name:
+                return self._build_runner_config_from_storage(study_summary, study_summary.best_trial)
+        return None
+
+    def get_num_remain_trials_by_name(self, exp_id):
+        """Get the num of remaining trails by experiment id.
+
+        Args:
+            exp_id (str): experiment id.
+
+        Returns:
+            int: num of remaining trails.
+        """
+        for study_summary in optuna.get_all_study_summaries(self.storage):
+            if exp_id == study_summary.study_name:
+                study = optuna.load_study(study_name=exp_id, storage=self.storage)
+                num_completed_trials = len(study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)))
+                num_remain_trials = self.hpo_config.num_trials - num_completed_trials
+                return num_remain_trials
+        return self.hpo_config.num_trials
+
+    def optimize(
+            self,
+            base_runner_config,
+            train_loader,
+            valid_loader,
+            test_loader=None,
+            exp_id=None,
+            **kwargs
+    ):
+        """Run the optimization process.
+
+        Args:
+            base_runner_config (EasyTPP.RunnerConfig): runner config.
+            train_loader (EasyTPP.DataLoader): train data loader.
+            valid_loader (EasyTPP.DataLoader): valid data loader
+            test_loader (EasyTPP.DataLoader, optional): test data loader. Defaults to None.
+            exp_id (str, optional): experiment id. Defaults to None.
+
+        Raises:
+            RuntimeError: best trial is not found.
+
+        Returns:
+            tuple: best_metric and best_runner_config
+        """
+        # obtain parameters
+        storage = self.storage
+        load_if_exists = self.hpo_config.is_continuous
+        metric_direction = base_runner_config.get_metric_direction()
+
+        # delete the study if it already existed when 'is_continue' is false
+        if not load_if_exists and exp_id is not None:
+            if exp_id in [std_summary.study_name for std_summary in optuna.get_all_study_summaries(storage)]:
+                optuna.delete_study(
+                    study_name=exp_id,
+                    storage=storage
+                )
+        # create hpo study
+        study = optuna.create_study(
+            storage=storage,
+            direction=metric_direction,
+            load_if_exists=load_if_exists,
+            study_name=exp_id,
+            sampler=TPESampler(seed=9899),
+        )
+
+        # set user_attr to study
+        study.set_user_attr('data_config', base_runner_config.data_config.get_yaml_config())
+
+        # calculate the number of remaining trials
+        num_completed_trials = len(study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)))
+        num_remain_trials = self.hpo_config.num_trials - num_completed_trials
+        if num_remain_trials > 0:
+            logger.info(f'Number of hpo trials completed for runner {exp_id}: '
+                        f'{num_completed_trials}/{self.hpo_config.num_trials}')
+            objective_func = self._get_objective_func(
+                base_runner_config=base_runner_config,
+                train_loader=train_loader,
+                valid_loader=valid_loader,
+                test_loader=test_loader,
+                **kwargs
+            )
+            # hpo optimize
+            study.optimize(
+                objective_func,
+                n_trials=num_remain_trials,
+                callbacks=[self._optimize_trial_end],
+                gc_after_trial=True,
+                n_jobs=self.hpo_config.num_jobs,
+            )
+
+        # statistics of this hpo
+        pruned_trials = study.get_trials(deepcopy=False, states=(TrialState.PRUNED,))
+        complete_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
+        logger.info("HPO - Optuna statistics:")
+        logger.info(f"\tNumber of finished trials: {len(study.trials)}")
+        logger.info(f"\tNumber of pruned trials: {len(pruned_trials)}")
+        logger.info(f"\tNumber of complete trials: {len(complete_trials)}")
+
+        if len(study.best_trials) == 0:
+            raise RuntimeError('Best trial is not found, please check the model or metric.')
+        trial = study.best_trial
+        logger.info(f"HPO - Best metric value ({metric_direction}): {trial.value}")
+
+        logger.info(f"Best Parameters: ")
+        for key, value in trial.params.items():
+            logger.info(f"\t{key}: {value}")
+
+        best_metric = trial.value
+        best_runner_config = RunnerConfig.parse_from_yaml_config(
+            trial.user_attrs['runner_config'],
+            data_config=base_runner_config.data_config,
+        )
+        return best_metric, best_runner_config
+
+    def _get_objective_func(
+            self,
+            base_runner_config,
+            **kwargs,
+    ):
+        """Get the optimization objective function.
+
+        Args:
+            base_runner_config (EasyTPP.Config): runner config.
+
+        Raises:
+            e: RuntimeError
+            optuna.TrialPruned: message in trials.
+
+        Returns:
+            _type_: _description_
+        """
+        trial_func = self.retrieve_trial_func_by_model_name(base_runner_config.base_config.exp_id)
+
+        def objective(trial):
+            timer = Timer()
+            timer.start()
+            logger.info(f'Start the trial {trial.number} ...')
+            # get a copy of base runner config for isolation
+            # generate new runner  runners
+            runner_config = base_runner_config.copy()
+
+            trial_model_info = trial_func(
+                trial,
+                trainder_config=runner_config.trainer_config,
+                model_config=runner_config.model_config
+            )
+
+            # use predefined trial to update model_info
+            runner_config_dict = dict_deep_update(
+                target=runner_config.get_yaml_config(),
+                source=trial_model_info,
+                is_add_new_key=False)
+
+            # eval the "suggest" in runner_config (actually run trial suggestion)
+            runner_config_dict = self._eval_str_trial_to_dict(trial,
+                                                              runner_config_dict)
+
+            runner_config = RunnerConfig.parse_from_yaml_config(runner_config_dict, direct_parse=True)
+
+            runner = Runner.build_from_config(
+                runner_config=runner_config,
+                unique_model_dir=True,
+                skip_data_loader=True,
+            )
+            try:
+                # train model
+                runner.train(**kwargs)
+                # evaluate model
+                metric = runner.evaluate(trial=trial, **kwargs)
+                # save the final model
+                runner.save()
+            except RuntimeError as e:
+                # add the error message into trial
+                err_msg = str(e)
+                trial.set_user_attr("error", err_msg)
+
+                logger.error(f'Error in the trial {trial.number}: {err_msg}')
+
+                # just prune the errors like 'out of memory'
+                if 'out of memory' not in err_msg:
+                    raise e
+                raise optuna.TrialPruned()
+            finally:
+                # add model path into trial
+                trial.set_user_attr("model_dir", runner.runner_config.model_dir)
+                # trial.set_user_attr("model_config", runner.runner_config.model_config)
+                trial.set_user_attr("runner_config", runner.runner_config.get_yaml_config())
+
+                logger.info(f'End trial {trial.number} ! Cost time: {timer.end()}')
+
+            return metric
+
+        return objective
+
+    def _optimize_trial_end(self, study, trial):
+        """End the process of trials.
+
+        Args:
+            study (optuna.study.Study): an object of optuna :class:`~optuna.study` to be studied during optimization.
+            trial (optuna.trial.FrozenTrial): an object of optuna :class:`~optuna.trial` that stores trial information.
+        """
+        # push storage to the specified uri
+        self._push_storage(trial)
+
+        is_best_yet = (trial in study.best_trials)
+
+        runner_id = study.study_name
+        runner_config = self._build_runner_config_from_storage(study, trial)
+
+        # invoke callbacks
+        for callback in self.trial_end_callbacks:
+            callback(runner_id, runner_config, is_best_yet)
+
+        # clean disk
+        if not is_best_yet and os.path.exists(trial.user_attrs['model_dir']):
+            os.system(f"rm -fr {trial.user_attrs['model_dir']}")
+
+    def _eval_str_trial_to_dict(self, trial, a_dict):
+        for key, val in a_dict.items():
+            if type(val) == str and val.startswith('suggest_'):
+                idx = val.find('(')
+                prefix = val[:idx + 1]
+                suffix = val[idx + 1:]
+
+                # get trial variable name
+                trial_name = [k for k, v in locals().items() if v == trial][0]
+
+                code = '''{0}.{1}"{2}",{3}'''.format(trial_name, prefix, key, suffix)
+                a_dict[key] = eval(code)
+            elif type(val) == dict:
+                self._eval_str_trial_to_dict(trial, a_dict[key])
+
+        return a_dict
+
+    def _build_runner_config_from_storage(
+            self,
+            study,
+            trial
+    ):
+        """Initialize the RunnerConfig from the study and trial.
+
+        Args:
+            study (optuna.study.Study): an object of optuna :class:`~optuna.study` to be studied during optimization.
+            trial (optuna.trial.FrozenTrial): an object of optuna :class:`~optuna.trial` that stores trial information.
+
+        Returns:
+            EasyTPP.Config: RunnerConfig object.
+        """
+        runner_config_dict = trial.user_attrs['runner_config']
+        return RunnerConfig.parse_from_yaml_config(runner_config_dict, direct_parse=True)
+
+    def run(self):
+        """Run the HPO process.
+
+        Returns:
+            tuple: best_metric, best_runner_config
+        """
+        # to avoid to load unused data
+        train_loader, valid_loader, test_loader = None, None, None
+        exp_id = self.runner_config.base_config.exp_id
+
+        if self.get_num_remain_trials_by_name(exp_id) > 0:
+            train_loader = self._data_loader.get_loader(split='train')
+            valid_loader = self._data_loader.get_loader(split='dev')
+            if self.runner_config.data_config.test_dir is not None:
+                test_loader = self._data_loader.get_loader(split='test')
+
+        best_metric, best_runner_config = self.optimize(
+            base_runner_config=self.runner_config,
+            train_loader=train_loader,
+            valid_loader=valid_loader,
+            test_loader=test_loader,
+            exp_id=exp_id
+        )
+
+        return best_metric, best_runner_config
+
+    def _fetch_storage(self):
+        """Retrieve the stored model.
+
+        Returns:
+            str: dir of the stored model.
+        """
+        local_storage_fn = self.config.hpo_config.storage_path
+
+        # return the local storage location
+        return local_storage_fn
+
+    def _push_storage(self, trial):
+        """_summary_
+
+        Args:
+            trial (_type_): _description_
+
+        Raises:
+            NotImplementedError: _description_
+        """
+        # save hpo storage to remote if it's in remote
+        if self.config.hpo_config.storage_protocol == 'oss':
+            raise NotImplementedError
+
+        return
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/__init__.py` & `easy_tpp-0.0.5/easy_tpp/model/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from easy_tpp.model.torch_model.torch_anhn import ANHN as TorchANHN
-from easy_tpp.model.torch_model.torch_attnhp import AttNHP as TorchAttNHP
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-from easy_tpp.model.torch_model.torch_fullynn import FullyNN as TorchFullyNN
-from easy_tpp.model.torch_model.torch_intensity_free import IntensityFree as TorchIntensityFree
-from easy_tpp.model.torch_model.torch_nhp import NHP as TorchNHP
-from easy_tpp.model.torch_model.torch_ode_tpp import ODETPP as TorchODETPP
-from easy_tpp.model.torch_model.torch_rmtpp import RMTPP as TorchRMTPP
-from easy_tpp.model.torch_model.torch_sahp import SAHP as TorchSAHP
-from easy_tpp.model.torch_model.torch_thp import THP as TorchTHP
-
-# by default, we use torch and do not install tf, therefore we ignore the import error
-try:
-    from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-    from easy_tpp.model.tf_model.tf_nhp import NHP as TfNHP
-    from easy_tpp.model.tf_model.tf_ode_tpp import ODETPP as TfODETPP
-    from easy_tpp.model.tf_model.tf_thp import THP as TfTHP
-    from easy_tpp.model.tf_model.tf_sahp import SAHP as TfSAHP
-    from easy_tpp.model.tf_model.tf_rmtpp import RMTPP as TfRMTPP
-    from easy_tpp.model.tf_model.tf_attnhp import AttNHP as TfAttNHP
-    from easy_tpp.model.tf_model.tf_anhn import ANHN as TfANHN
-    from easy_tpp.model.tf_model.tf_fullynn import FullyNN as TfFullyNN
-    from easy_tpp.model.tf_model.tf_intensity_free import IntensityFree as TfIntensityFree
-except ImportError:
-    pass
-
-__all__ = ['TorchBaseModel',
-           'TorchNHP',
-           'TorchAttNHP',
-           'TorchTHP',
-           'TorchSAHP',
-           'TorchFullyNN',
-           'TorchIntensityFree',
-           'TorchODETPP',
-           'TfBaseModel',
-           'TfNHP',
-           'TfAttNHP',
-           'TfTHP',
-           'TfSAHP',
-           'TfANHN',
-           'TfFullyNN',
-           'TfIntensityFree',
-           'TfODETPP']
+from easy_tpp.model.torch_model.torch_anhn import ANHN as TorchANHN
+from easy_tpp.model.torch_model.torch_attnhp import AttNHP as TorchAttNHP
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+from easy_tpp.model.torch_model.torch_fullynn import FullyNN as TorchFullyNN
+from easy_tpp.model.torch_model.torch_intensity_free import IntensityFree as TorchIntensityFree
+from easy_tpp.model.torch_model.torch_nhp import NHP as TorchNHP
+from easy_tpp.model.torch_model.torch_ode_tpp import ODETPP as TorchODETPP
+from easy_tpp.model.torch_model.torch_rmtpp import RMTPP as TorchRMTPP
+from easy_tpp.model.torch_model.torch_sahp import SAHP as TorchSAHP
+from easy_tpp.model.torch_model.torch_thp import THP as TorchTHP
+
+# by default, we use torch and do not install tf, therefore we ignore the import error
+try:
+    from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+    from easy_tpp.model.tf_model.tf_nhp import NHP as TfNHP
+    from easy_tpp.model.tf_model.tf_ode_tpp import ODETPP as TfODETPP
+    from easy_tpp.model.tf_model.tf_thp import THP as TfTHP
+    from easy_tpp.model.tf_model.tf_sahp import SAHP as TfSAHP
+    from easy_tpp.model.tf_model.tf_rmtpp import RMTPP as TfRMTPP
+    from easy_tpp.model.tf_model.tf_attnhp import AttNHP as TfAttNHP
+    from easy_tpp.model.tf_model.tf_anhn import ANHN as TfANHN
+    from easy_tpp.model.tf_model.tf_fullynn import FullyNN as TfFullyNN
+    from easy_tpp.model.tf_model.tf_intensity_free import IntensityFree as TfIntensityFree
+except ImportError:
+    pass
+
+__all__ = ['TorchBaseModel',
+           'TorchNHP',
+           'TorchAttNHP',
+           'TorchTHP',
+           'TorchSAHP',
+           'TorchFullyNN',
+           'TorchIntensityFree',
+           'TorchODETPP',
+           'TfBaseModel',
+           'TfNHP',
+           'TfAttNHP',
+           'TfTHP',
+           'TfSAHP',
+           'TfANHN',
+           'TfFullyNN',
+           'TfIntensityFree',
+           'TfODETPP']
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_anhn.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_basemodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,334 +1,271 @@
-import tensorflow as tf
-from tensorflow.python.keras import layers
-
-from easy_tpp.model.tf_model.tf_baselayer import MultiHeadAttention
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils.tf_utils import get_shape_list, tensordot, swap_axes, create_tensor
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class ANHN(TfBaseModel):
-    """Tensorflow implementation of Attentive Neural Hawkes Network, IJCNN 2021.
-        http://arxiv.org/abs/2211.11758
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (dict): config of model specs.
-        """
-        super(ANHN, self).__init__(model_config)
-        self.d_time = model_config['time_emb_size']
-        self.use_norm = model_config['use_ln']
-
-        self.n_layers = model_config['num_layers']
-        self.n_head = model_config['num_heads']
-        self.dropout = model_config['dropout']
-
-    def build_graph(self):
-        """ Build up the network """
-        with tf.variable_scope('ANHN'):
-            self.build_input_graph()
-
-            self.layer_rnn = layers.LSTM(self.hidden_size,
-                                         return_state=False,
-                                         return_sequences=True,
-                                         name='layer_rnn')
-
-            self.lambda_w = tf.get_variable('lambda_w',
-                                            shape=[self.hidden_size, self.num_event_types],
-                                            dtype=tf.float32,
-                                            initializer=tf.glorot_normal_initializer())
-            self.lambda_b = tf.get_variable('lambda_b',
-                                            shape=[self.num_event_types],
-                                            dtype=tf.float32,
-                                            initializer=tf.constant_initializer(0.1))
-
-            self.layer_time_delta = layers.Dense(self.hidden_size,
-                                                 activation=tf.nn.softplus,
-                                                 name='layer_time_delta')
-            self.layer_base_intensity = layers.Dense(self.hidden_size,
-                                                     activation=tf.nn.sigmoid,
-                                                     name='layer_mu')
-
-            self.layer_att = MultiHeadAttention(self.hidden_size,
-                                                self.n_head,
-                                                self.dropout)
-
-            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.gen_config and self.gen_config['num_step_gen'] == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.gen_config and self.gen_config['num_step_gen'] > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config['num_step_gen'])
-
-    def forward(self, dtime_seqs, type_seqs, attention_mask):
-        """Call the model.
-
-        Args:
-            dtime_seqs (tensor): [batch_size, seq_len].
-            type_seqs (tensor): [batch_size, seq_len].
-            attention_mask (tensor): [batch_size, seq_len, hidden_size].
-
-        Returns:
-            list: hidden states, [batch_size, seq_len, hidden_size], states right before the event happens;
-                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
-                  the event happens.
-        """
-
-        # [batch_size, seq_len, hidden_size]
-        event_emb = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size]
-        rnn_output = self.layer_rnn(event_emb)
-
-        # [batch_size, seq_len, hidden_size]
-        # mu in Equation (3)
-        intensity_base = self.layer_base_intensity(rnn_output)
-
-        # [batch_size, num_head, seq_len, seq_len]
-        _, att_weight = self.layer_att(rnn_output, attention_mask=attention_mask, output_weight=True)
-
-        # reformat the tensor
-        # [batch_size, seq_len, seq_len, 1]
-        att_weight = tf.reduce_mean(att_weight, axis=1)[..., None]
-
-        # At each step, alpha and delta reply on all previous event embeddings because there is a cumsum in Equation
-        # (3), therefore the alpha and beta have shape [batch_size, seq_len, seq_len, hidden_size] when performing
-        # matrix operations.
-        # [batch_size, seq_len, seq_len, hidden_size]
-        # alpha in Equation (3)
-        intensity_alpha = att_weight * rnn_output[:, None, :, :]
-
-        # compute delta
-        max_len = get_shape_list(event_emb)[1]
-
-        # [batch_size, seq_len, seq_len, hidden_dim]
-        left = tf.tile(rnn_output[:, None, :, :], [1, max_len, 1, 1])
-        right = tf.tile(rnn_output[:, :, None, :], [1, 1, max_len, 1])
-
-        # [batch_size, seq_len, seq_len, hidden_dim * 2]
-        cur_prev_concat = tf.concat([left, right], axis=-1)
-        # [batch_size, seq_len, seq_len, hidden_dim]
-        intensity_delta = self.layer_time_delta(cur_prev_concat)
-
-        # compute time elapse
-        # [batch_size, seq_len, seq_len, 1]
-        base_dtime, target_cumsum_dtime = self.compute_cumsum_dtime(dtime_seqs)
-
-        # [batch_size, max_len, hidden_size]
-        imply_lambdas = self.compute_states_at_event_times(intensity_base,
-                                                           intensity_alpha,
-                                                           intensity_delta,
-                                                           target_cumsum_dtime)
-
-        return imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime)
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            tuple: loglikelihood loss and num of events.
-        """
-
-        # 1. compute event-loglik
-        imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime) \
-            = self.forward(self.time_delta_seqs[:, 1:],
-                           self.type_seqs[:, :-1],
-                           self.attention_mask[:, 1:, :-1])
-        lambda_at_event = self.layer_intensity(imply_lambdas)
-
-        # 2. compute non-event-loglik (using MC sampling to compute integral)
-        # 2.1 sample times
-        # [batch_size, seq_len, num_sample]
-        sample_dtimes = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # [batch_size, num_times = max_len - 1, num_sample, event_num]
-        state_t_sample = self.compute_states_at_sample_times(intensity_base, intensity_alpha, intensity_delta,
-                                                             base_dtime, sample_dtimes)
-        lambda_t_sample = self.layer_intensity(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        # return enc_inten to compute accuracy
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_cumsum_dtime(self, dtime_seqs):
-        """Compute cumulative delta times.
-
-        Args:
-            dtime_seqs (tensor): [batch_size, seq_len].
-
-        Returns:
-            tensor: [batch_size, seq_len].
-        """
-        # [batch_size, seq_len, num_sample]
-        #  dtime_seqs here = dtime_seqs[:, 1:]
-        # [dt_1, dt_2, dt_3] => [dt_1 + dt_2, dt_2, 0]
-        cum_dtimes = tf.cumsum(dtime_seqs, axis=1, reverse=True, exclusive=True)
-
-        # [batch_size, seq_len, seq_len, 1] (lower triangular: positive, upper: negative, diagonal: zero)
-        base_elapses = tf.expand_dims(cum_dtimes[:, None, :] - cum_dtimes[:, :, None], axis=-1)
-
-        # [batch_size, seq_len, seq_len， 1]
-        target_cumsum = base_elapses + dtime_seqs[:, :, None, None]
-
-        return base_elapses, target_cumsum
-
-    def compute_states_at_event_times(self, intensity_base, intensity_alpha, intensity_delta, cumsum_dtimes):
-        """Compute implied lambda based on Equation (3).
-
-        Args:
-            intensity_base (tensor): [batch_size, seq_len, (num_sample), hidden_size]
-            intensity_alpha (tensor): [batch_size, seq_len, seq_len, (num_sample), hidden_size]
-            intensity_delta (tensor): [batch_size, seq_len, seq_len, (num_sample), hidden_size]
-            cumsum_dtimes: [batch_size, seq_len, (num_sample), 1]
-
-        Returns:
-            hidden states at all cumsum_dtimes: [batch_size, seq_len, num_samples, hidden_size]
-
-        """
-        # to avoid nan calculated by exp after (nan * 0 = nan)
-        elapse = tf.abs(cumsum_dtimes)
-
-        # [batch_size, seq_len, hidden_dim]
-        cumsum_term = tf.reduce_sum(intensity_alpha * tf.exp(-intensity_delta * elapse), axis=-2)
-        # [batch_size, seq_len, hidden_dim]
-        imply_lambdas = intensity_base + cumsum_term
-
-        return imply_lambdas
-
-    def compute_states_at_sample_times(self, intensity_base, intensity_alpha, intensity_delta, base_dtime,
-                                       sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            intensity_base (tensor): [batch_size, seq_len, hidden_size].
-            intensity_alpha (tensor): [batch_size, seq_len, seq_len, hidden_size].
-            intensity_delta (tensor): [batch_size, seq_len, seq_len, hidden_size].
-            base_dtime (tensor): [batch_size, seq_len, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: hidden state at each sampled time, [batch_size, seq_len, num_sample, hidden_size].
-        """
-        # [max_len, batch_size, n_sample, hidden_dim]
-        mus_trans = tf.transpose(intensity_base, perm=[1, 0, 2])[:, :, None]
-
-        # [max_len, batch_size, n_sample, max_len, hidden_dim]
-        alphas_trans = tf.transpose(intensity_alpha, perm=[1, 0, 2, 3])[:, :, None]
-        deltas_trans = tf.transpose(intensity_delta, perm=[1, 0, 2, 3])[:, :, None]
-
-        base_elapses_trans = tf.transpose(base_dtime, perm=[1, 0, 2, 3])[:, :, None]
-
-        batch_size, num_sample_per_step, _ = get_shape_list(sample_dtimes)
-
-        state_scan_initializer = create_tensor([batch_size,
-                                                num_sample_per_step,
-                                                self.hidden_size],
-                                               0.0)
-
-        # [seq_len, batch_size, num_sample, hidden_size]
-        states_samples = tf.scan(fn=self.get_compute_lambda_forward_fn(),
-                                 elems=[
-                                     mus_trans,
-                                     alphas_trans,
-                                     deltas_trans,
-                                     base_elapses_trans,
-                                     swap_axes(sample_dtimes[:, :, :, None, None], 0, 1)],
-                                 initializer=state_scan_initializer)
-
-        # [batch_size, seq_len, num_sample, hidden_size]
-        states_samples = swap_axes(states_samples, 1, 0)
-        return states_samples
-
-    def get_compute_lambda_forward_fn(self):
-        """Compute the lambda using scan function.
-
-        Returns:
-            function: a forward function used in tf.scan.
-        """
-        compute_states_fn = self.compute_states_at_event_times
-
-        def forward_fn(acc, item):
-            mu, alpha, delta, elapse, elapse_bias = item
-            return compute_states_fn(mu, alpha, delta, elapse + elapse_bias)
-
-        return forward_fn
-
-    def layer_intensity(self, hidden_states):
-        """Compute the intensity based on the hidden states.
-
-        Args:
-            hidden_states (tensor): [batch_size, seq_len, hidden_size].
-
-        Returns:
-            tensor: [batch_size, seq_len, num_event_type_no_pad].
-        """
-        return tf.nn.softplus(tensordot(hidden_states, self.lambda_w) + self.lambda_b)
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
-        """Compute the intensity at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
-            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
-            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
-            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
-
-        Returns:
-            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
-        """
-        attention_mask = kwargs.get('attention_mask', None)
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        if attention_mask is None:
-            batch_size, seq_len = get_shape_list(time_seqs)
-            attention_mask = tf.ones((seq_len, seq_len))
-            # only keep the strict upper triangular
-            lower_diag_masks = tf.linalg.LinearOperatorLowerTriangular(tf.ones_like(attention_mask)).to_dense()
-            attention_mask = tf.where(tf.equal(lower_diag_masks, 0),
-                                      attention_mask,
-                                      tf.zeros_like(attention_mask))
-            attention_mask = tf.tile(attention_mask[None, ...], (batch_size, 1, 1))
-            attention_mask = tf.cast(attention_mask, tf.int32)
-
-        # [batch_size, seq_len, num_samples]
-        imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime) \
-            = self.forward(time_delta_seqs, type_seqs, attention_mask)
-
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = self.compute_states_at_sample_times(intensity_base, intensity_alpha, intensity_delta,
-                                                             base_dtime, sample_dtimes)
-
-        if compute_last_step_only:
-            lambdas = self.layer_intensity(encoder_output[:, -1:, :, :])
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = self.layer_intensity(encoder_output)
-        return lambdas
+""" Base model with common functionality  """
+
+import tensorflow as tf
+
+from easy_tpp.model.tf_model.tf_thinning import EventSampler
+from easy_tpp.utils.tf_utils import get_shape_list
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class TfBaseModel(tf.keras.Model):
+    def __init__(self, model_config):
+        super(TfBaseModel, self).__init__()
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        self.model_config = model_config
+
+        self.loss_integral_num_sample_per_step = model_config.loss_integral_num_sample_per_step
+        self.hidden_size = model_config.hidden_size
+        self.num_event_types = model_config.num_event_types  # not include [PAD]
+        self.num_event_types_pad = model_config.num_event_types_pad  # include [PAD]
+        self.event_pad_index = model_config.pad_token_id
+        self.dropout_rate = model_config.dropout_rate
+
+        self.eps = 1e-7
+
+        self.layer_type_emb = tf.keras.layers.Embedding(self.num_event_types_pad,
+                                                        self.hidden_size)
+
+        self.gen_config = model_config.thinning
+        self.event_sampler = None
+        if self.gen_config:
+            self.event_sampler = EventSampler(num_sample=self.gen_config.num_sample,
+                                              num_exp=self.gen_config.num_exp,
+                                              over_sample_rate=self.gen_config.over_sample_rate,
+                                              patience_counter=self.gen_config.patience_counter,
+                                              num_samples_boundary=self.gen_config.num_samples_boundary,
+                                              dtime_max=self.gen_config.dtime_max)
+
+    def build_input_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('BaseModel'):
+            # Input placeholder
+            # shape - (batch_size, max_len)
+            # max_len - sequence length including time zero padding
+            self.time_delta_seqs = tf.placeholder(tf.float32, shape=[None, None])
+
+            # shape - (batch_size, max_len)
+            self.time_seqs = tf.placeholder(tf.float32, shape=[None, None])
+
+            # shape - (batch_size, max_len)
+            self.type_seqs = tf.placeholder(tf.int32, shape=[None, None])
+
+            # shape - (batch_size, max_len)
+            self.batch_non_pad_mask = tf.placeholder(tf.int32, shape=[None, None])
+
+            # shape - (batch_size, max_len, max_len)
+            self.attention_mask = tf.placeholder(tf.int32, shape=[None, None, None])
+
+            # Event type one-hot code
+            # shape - (batch_size, max_len, num_event_types)
+            self.type_mask = tf.placeholder(tf.float32, shape=[None, None, None])
+
+            # shape - (batch_size 1)
+            self.seq_len = tf.cast(tf.reduce_sum(tf.cast(self.batch_non_pad_mask, tf.float32), axis=1, keepdims=True),
+                                   tf.int32)
+
+            self.is_training = tf.placeholder(tf.bool)
+
+        return
+
+    @staticmethod
+    def generate_model_from_config(model_config):
+        """Generate the model in derived class based on model config.
+
+        Args:
+            model_config (EasyTPP.Config): config of model specs.
+        """
+        model_id = model_config.model_id
+
+        for subclass in TfBaseModel.__subclasses__():
+            if subclass.__name__ == model_id:
+                return subclass(model_config)
+
+        raise RuntimeError('No model named ' + model_id)
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, event_seqs, sampled_dtimes):
+        raise NotImplementedError
+
+    def make_dtime_loss_samples(self, time_delta_seq):
+        """Generate the time point samples for every interval.
+
+        Args:
+            time_delta_seq (tensor): [batch_size, seq_len].
+
+        Returns:
+            tensor: [batch_size, seq_len, n_samples]
+        """
+        # shape  (1, 1, n_samples)
+        dtimes_ratio_sampled = tf.linspace(start=0.0,
+                                           stop=1.0,
+                                           num=self.loss_integral_num_sample_per_step)[None, None, :]
+
+        # shape (batch_size, max_len, n_samples)
+        sampled_dtimes = time_delta_seq[:, :, None] * dtimes_ratio_sampled
+
+        return sampled_dtimes
+
+    def compute_loglikelihood(self, time_delta_seq, lambda_at_event, lambdas_loss_samples, seq_mask,
+                              lambda_type_mask):
+        """Compute the loglikelihood of the event sequence based on Equation (8) of NHP paper.
+
+        Args:
+            time_delta_seq (tensor): [batch_size, seq_len], time_delta_seq from model input.
+            lambda_at_event (tensor): [batch_size, seq_len, num_event_types], unmasked intensity at
+            (right after) the event.
+            lambdas_loss_samples (tensor): [batch_size, seq_len, num_sample, num_event_types],
+            intensity at sampling times.
+            seq_mask (tensor): [batch_size, seq_len], sequence mask vector to mask the padded events.
+            lambda_type_mask (tensor): [batch_size, seq_len, num_event_types], type mask matrix to mask
+            the padded event types.
+
+        Returns:
+            tuple: event loglike, non event loglike, intensity at event with padding events masked
+        """
+
+        # Sum of lambda over every type
+        # [batch_size, seq_len]
+        event_lambdas = tf.reduce_sum(lambda_at_event * lambda_type_mask, axis=-1)
+
+        # mask the pad event
+        event_lambdas = tf.boolean_mask(event_lambdas, seq_mask)
+
+        # Sum of lambda over every event point
+        # [num_unmasked_events]
+        event_ll = tf.reduce_sum(tf.log(event_lambdas))
+
+        # Compute the big lambda integral in Equation (8) of NHP paper
+        # 1 - take num_mc_sample rand points in each event interval
+        # 2 - compute its lambda value for every sample point
+        # 3 - take average of these sample points
+        # 4 - times the interval length
+
+        # [batch_size, max_len, n_loss_sample]
+        lambdas_total_samples = tf.reduce_sum(lambdas_loss_samples, axis=-1)
+
+        # interval_integral - [batch_size, num_times]
+        # interval_integral = length_interval * average of sampled lambda(t)
+        non_event_ll = tf.reduce_mean(lambdas_total_samples, axis=-1) * time_delta_seq * tf.cast(seq_mask, tf.float32)
+
+        non_event_ll = tf.reduce_sum(non_event_ll)
+
+        num_events = get_shape_list(event_lambdas)[0]
+
+        return event_ll, non_event_ll, num_events
+
+    def predict_one_step_at_every_event(self, time_seqs, time_delta_seqs, type_seqs):
+        """One-step prediction for every event in the sequence.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len].
+            time_delta_seqs (tensor): [batch_size, seq_len].
+            type_seqs (tensor): [batch_size, seq_len].
+
+        Returns:
+            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
+        """
+
+        # remove the last event, as the prediction based on the last event has no label
+        time_seqs, time_delta_seqs, type_seqs = time_seqs[:, :-1], time_delta_seqs[:, 1:], type_seqs[:, :-1]
+
+        # (batch_size, seq_len)
+        dtime_boundary = time_delta_seqs + self.event_sampler.dtime_max
+
+        # [batch_size, seq_len, num_sample]
+        accepted_dtimes, weights = self.event_sampler.draw_next_time_one_step(time_seqs,
+                                                                              time_delta_seqs,
+                                                                              type_seqs,
+                                                                              dtime_boundary,
+                                                                              self.compute_intensities_at_sample_times,
+                                                                              compute_last_step_only=False)
+
+        # [batch_size, seq_len]
+        dtimes_pred = tf.reduce_sum(accepted_dtimes * weights, axis=-1)
+
+        # [batch_size, seq_len, 1, event_num]
+        intensities_at_times = self.compute_intensities_at_sample_times(time_seqs,
+                                                                        time_delta_seqs,
+                                                                        type_seqs,
+                                                                        dtimes_pred[:, :, None])
+
+        # [batch_size, seq_len, event_num]
+        intensities_at_times = tf.squeeze(intensities_at_times, axis=-2)
+
+        # [batch_size, seq_len]
+        types_pred = tf.argmax(intensities_at_times, axis=-1)
+
+        return dtimes_pred, types_pred
+
+    def predict_multi_step_since_last_event(self, time_seqs, time_delta_seqs, type_seqs, num_step):
+        """Multi-step prediction for every event in the sequence.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len].
+            time_delta_seqs (tensor): [batch_size, seq_len].
+            type_seqs (tensor): [batch_size, seq_len].
+            num_step (int): num of steps for prediction.
+
+        Returns:
+            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
+        """
+        i = tf.constant(0)
+
+        time_seqs_ = time_seqs
+        time_delta_seqs_ = time_delta_seqs
+        type_seqs_ = type_seqs
+
+        def while_condition(i, time_seqs_, time_delta_seqs_, type_seqs_):
+            return tf.less(i, num_step)
+
+        def body(i, time_seqs_, time_delta_seqs_, type_seqs_):
+            # [batch_size, seq_len]
+            dtime_boundary = time_delta_seqs_ + self.event_sampler.dtime_max
+
+            # [batch_size, seq_len, num_sample]
+            accepted_dtimes, weights = \
+                self.event_sampler.draw_next_time_one_step(time_seqs_,
+                                                           time_delta_seqs_,
+                                                           type_seqs_,
+                                                           dtime_boundary,
+                                                           self.compute_intensities_at_sample_times,
+                                                           compute_last_step_only=True)
+
+            # [batch_size, seq_len]
+            dtimes_pred = tf.reduce_sum(accepted_dtimes * weights, axis=-1)
+
+            # [batch_size, seq_len, 1, event_num]
+            intensities_at_times = self.compute_intensities_at_sample_times(time_seqs_,
+                                                                            time_delta_seqs_,
+                                                                            type_seqs_,
+                                                                            dtimes_pred[:, :, None])
+
+            # [batch_size, seq_len, event_num]
+            intensities_at_times = tf.squeeze(intensities_at_times, axis=-2)
+
+            # [batch_size, seq_len]
+            types_pred = tf.argmax(intensities_at_times, axis=-1)
+
+            # [batch_size, 1]
+            types_pred_ = tf.cast(types_pred[:, -1:], tf.int32)
+            dtimes_pred_ = dtimes_pred[:, -1:]
+            time_pred_ = time_seqs_[:, -1:] + dtimes_pred_
+
+            # concat to the prefix sequence
+            time_seqs_ = tf.concat([time_seqs_, time_pred_], axis=-1)
+            time_delta_seqs_ = tf.concat([time_delta_seqs_, dtimes_pred_], axis=-1)
+            type_seqs_ = tf.concat([type_seqs_, types_pred_], axis=-1)
+
+            return [tf.add(i, 1), time_seqs_, time_delta_seqs_, type_seqs_]
+
+        _, _, time_delta_seqs_, type_seqs_ = tf.while_loop(while_condition,
+                                                           body,
+                                                           [i, time_seqs_, time_delta_seqs_, type_seqs_])
+        # to be consistent with the torch version
+        return time_delta_seqs_[:, -num_step - 1:], type_seqs_[:, -num_step - 1:]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_attnhp.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_attnhp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,341 +1,322 @@
-import math
-
-import numpy as np
-import tensorflow as tf
-from tensorflow.python.keras import layers
-
-from easy_tpp.model.tf_model.tf_baselayer import EncoderLayer
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class AttNHP(TfBaseModel):
-    def __init__(self, model_config):
-        super(AttNHP, self).__init__(model_config)
-        self.d_model = model_config.hidden_size
-        self.d_time = model_config.data_specs['time_emb_size']
-        self.use_norm = model_config.data_specs['use_ln']
-
-        self.n_layers = model_config.data_specs['num_layers']
-        self.n_head = model_config.data_specs['num_heads']
-        self.dropout = model_config.dropout_rate
-
-        # position vector, used for temporal encoding
-        self.div_term = self.make_div_term()
-
-    def make_div_term(self):
-        """Initialize the division term used in temporal embedding.
-
-        Returns:
-            np.array: diviser.
-        """
-        div_term_ = np.exp(np.arange(0, self.d_time, 2) * -(math.log(10000.0) / self.d_time))
-        div_term_ = np.reshape(div_term_, (1, 1, -1))
-
-        div_term = np.ones((1, 1, self.d_time))
-
-        for i in range(self.d_time):
-            div_term[..., i] = div_term_[..., i // 2]
-
-        return div_term
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('AttNHP'):
-            self.build_input_graph()
-
-            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
-
-            self.heads = []
-            for i in range(self.n_head):
-                self.heads.append([EncoderLayer(hidden_size=self.d_model,
-                                                num_heads=self.n_head,
-                                                dropout_rate=self.dropout) for _ in range(self.n_layers)])
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.event_sampler and self.gen_config.num_step_gen == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.event_sampler and self.gen_config.num_step_gen > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def compute_temporal_embedding(self, time_seqs):
-        """Compute the temporal embedding.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len].
-
-        Returns:
-            tensor: [batch_size, seq_len, emb_size].
-        """
-
-        batch_size, seq_len = get_shape_list(time_seqs)  # dynamic
-
-        # [self.d_time]
-        position_mask = np.array([1] * self.d_time)
-        position_mask[1::2] = 0  # dim 2i+1
-        position_mask = tf.convert_to_tensor(position_mask, tf.int32)
-
-        # [batch_size, max_len, d_time]
-        position_mask = tf.tile(position_mask[None, None, ...], [batch_size, seq_len, 1])
-
-        time_seqs_ = time_seqs[..., None]
-
-        position_enc = tf.where(tf.equal(position_mask, 0),  # dim 2i+1
-                                tf.cos(time_seqs_ * self.div_term),  # dim 2i+1
-                                tf.sin(time_seqs_ * self.div_term))  # dim 2i
-
-        # [batch_size, max_len, hidden_dim]
-        return position_enc
-
-    def seq_encoding(self, time_seqs, type_seqs):
-        """Encode the sequence.
-
-        Args:
-            time_seqs (tensor): time seqs input, [batch_size, seq_len].
-            event_seqs (_type_): event type seqs input, [batch_size, seq_len].
-
-        Returns:
-            tuple: event embedding, time embedding and type embedding.
-        """
-
-        # [batch_size, seq_len, hidden_size]
-        time_emb = self.compute_temporal_embedding(time_seqs)
-        # [batch_size, seq_len, hidden_size]
-        type_emb = tf.tanh(self.layer_type_emb(type_seqs))
-        # [batch_size, seq_len, hidden_size*2]
-        event_emb = tf.concat([type_emb, time_emb], axis=-1)
-
-        return event_emb, time_emb, type_emb
-
-    def make_layer_mask(self, attention_mask):
-        """Create a tensor to do masking on layers.
-
-        Args:
-            attention_mask (tensor): mask for attention operation, [batch_size, seq_len, seq_len]
-
-        Returns:
-            tensor: aim to keep the current layer, the same size of attention mask
-            a diagonal matrix, [batch_size, seq_len, seq_len]
-        """
-        # [batch_size, seq_len, seq_len]
-        layer_mask = tf.eye(get_shape_list(attention_mask)[1]) < 1
-        layer_mask = layer_mask[None, ...]
-        layer_mask = tf.tile(layer_mask, [get_shape_list(attention_mask)[0], 1, 1])
-        return tf.cast(layer_mask, tf.int32)
-
-    def make_combined_att_mask(self, attention_mask, layer_mask):
-        """Combined attention mask and layer mask.
-
-        Args:
-            attention_mask (tensor): mask for attention operation, [batch_size, seq_len, seq_len]
-            layer_mask (tensor): mask for other layers, [batch_size, seq_len, seq_len]
-
-        Returns:
-            tensor: [batch_size, seq_len * 2, seq_len * 2]
-        """
-
-        # [batch_size, seq_len, seq_len * 2]
-        combined_mask = tf.concat([attention_mask, layer_mask], axis=-1)
-        # [batch_size, seq_len, seq_len * 2]
-        contextual_mask = tf.concat([attention_mask, tf.ones_like(layer_mask)], axis=-1)
-        # [batch_size, seq_len * 2, seq_len * 2]
-        combined_mask = tf.concat([contextual_mask, combined_mask], axis=1)
-        return combined_mask
-
-    def forward_pass(self, init_cur_layer, time_emb, sample_time_emb, event_emb, combined_mask):
-        """update the structure sequentially.
-
-        Args:
-            init_cur_layer (tensor): [batch_size, seq_len, hidden_size]
-            time_emb (tensor): [batch_size, seq_len, hidden_size]
-            sample_time_emb (tensor): [batch_size, seq_len, hidden_size]
-            event_emb (tensor): [batch_size, seq_len, hidden_size]
-            combined_mask (tensor): [batch_size, seq_len, hidden_size]
-
-        Returns:
-            tensor: [batch_size, seq_len, hidden_size*2]
-        """
-        cur_layers = []
-        seq_len = get_shape_list(time_emb)[1]
-
-        for head_i in range(self.n_head):
-            # [batch_size, seq_len, hidden_size]
-            cur_layer_ = init_cur_layer
-            for layer_i in range(self.n_layers):
-                # each layer concats the temporal emb
-                # [batch_size, seq_len, hidden_size*2]
-                layer_ = tf.concat([cur_layer_, sample_time_emb], axis=-1)
-                # make combined input from event emb + layer emb
-                # [batch_size, seq_len*2, hidden_size*2]
-                _combined_input = tf.concat([event_emb, layer_], axis=1)
-
-                enc_layer = self.heads[head_i][layer_i]
-                # compute the output
-                enc_output = enc_layer((_combined_input, combined_mask),
-                                       training=self.is_training)
-
-                # the layer output
-                # [batch_size, seq_len, hidden_size]
-                _cur_layer_ = enc_output[:, seq_len:, :]
-                # add residual connection
-                cur_layer_ = tf.tanh(_cur_layer_) + cur_layer_
-
-                # event emb
-                event_emb = tf.concat([enc_output[:, :seq_len, :], time_emb], axis=-1)
-
-                if self.use_norm:
-                    cur_layer_ = self.norm(cur_layer_)
-            cur_layers.append(cur_layer_)
-        cur_layer_ = tf.concat(cur_layers, axis=-1)
-
-        return cur_layer_
-
-    def forward(self, time_seqs, type_seqs, attention_mask, sample_times=None):
-        """ Move forward through the network """
-
-        # [batch_size, seq_len, hidden_size]
-        event_emb, time_emb, type_emb = self.seq_encoding(time_seqs, type_seqs)
-        init_cur_layer = tf.zeros_like(type_emb)
-        layer_mask = self.make_layer_mask(attention_mask)
-
-        if sample_times is None:
-            sample_time_emb = time_emb
-        else:
-            sample_time_emb = self.compute_temporal_embedding(sample_times)
-        combined_mask = self.make_combined_att_mask(attention_mask, layer_mask)
-
-        encoder_output = self.forward_pass(init_cur_layer, time_emb, sample_time_emb, event_emb, combined_mask)
-
-        return encoder_output
-
-    def loglike_loss(self):
-        # 1. compute event-loglik
-        enc_out = self.forward(self.time_seqs[:, :-1],
-                               self.type_seqs[:, :-1],
-                               self.attention_mask[:, 1:, :-1],
-                               self.time_seqs[:, 1:])
-
-        # [batch_size, seq_len, num_event_types]
-        lambda_at_event = self.layer_intensity(enc_out)
-
-        # 2. compute non-event-loglik (using MC sampling to compute integral)
-        # 2.1 sample times
-        # [batch_size, seq_len, num_sample]
-        temp_time = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # [batch_size, seq_len, num_sample]
-        sample_times = temp_time + self.time_seqs[:, :-1][..., None]
-
-        # 2.2 compute intensities at sampled times
-        # [batch_size, num_times = max_len - 1, num_sample, event_num]
-        lambda_t_sample = self.compute_intensities_at_sample_times(self.time_seqs[:, :-1],
-                                                                   self.time_delta_seqs[:, :-1],  # not used
-                                                                   self.type_seqs[:, :-1],
-                                                                   sample_times,
-                                                                   attention_mask=self.attention_mask[:, 1:, :-1])
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        # return enc_inten to compute accuracy
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self,
-                                       time_seqs,
-                                       type_seqs,
-                                       attention_mask,
-                                       sample_times):
-        """
-
-        Args:
-            time_seqs: [batch_size, seq_len]
-            type_seqs: [batch_size, seq_len]
-            attention_mask: [batch_size, seq_len, seq_len]
-            sample_times: [batch_size, seq_len, num_samples]
-
-        Returns:
-            hidden states at all sampled times: [batch_size, seq_len, num_samples, hidden_size]
-
-        """
-        batch_size, seq_len = get_shape_list(type_seqs)
-        num_samples = get_shape_list(sample_times)[-1]
-
-        # [num_samples, batch_size, seq_len]
-        sample_times = tf.transpose(sample_times, perm=(2, 0, 1))
-        # [num_samples * batch_size, seq_len]
-        _sample_time = tf.reshape(sample_times, (num_samples * batch_size, -1))
-        # [num_samples * batch_size, seq_len]
-        _types = tf.reshape(tf.tile(type_seqs[None, ...], (num_samples, 1, 1)), (num_samples * batch_size, -1))
-        # [num_samples * batch_size, seq_len]
-        _times = tf.reshape(tf.tile(time_seqs[None, ...], (num_samples, 1, 1)), (num_samples * batch_size, -1))
-        # [num_samples * batch_size, seq_len]
-        _attn_mask = tf.tile(attention_mask[None, ...], (num_samples, 1, 1, 1))
-        _attn_mask = tf.reshape(_attn_mask, (num_samples * batch_size, seq_len, seq_len))
-
-        # [num_samples * batch_size, seq_len, hidden_size]
-        encoder_output = self.forward(_times,
-                                      _types,
-                                      _attn_mask,
-                                      _sample_time)
-
-        # [num_samples, batch_size, seq_len, hidden_size]
-        encoder_output = tf.reshape(encoder_output, (num_samples, batch_size, seq_len, -1))
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = tf.transpose(encoder_output, perm=(1, 2, 0, 3))
-        return encoder_output
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_times, **kwargs):
-        """
-        Args:
-            time_seqs: [batch_size, seq_len]
-            time_delta_seqs: [batch_size, seq_len]
-            type_seqs: [batch_size, seq_len]
-            sample_times: [batch_size, seq_len, num_samples]
-
-        Returns:
-            intensities at sample times: [batch_size, seq_len, num_samples, num_event_types]
-        """
-        attention_mask = kwargs.get('attention_mask', None)
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        if attention_mask is None:
-            batch_size, seq_len = get_shape_list(time_seqs)
-            attention_mask = tf.ones((seq_len, seq_len))
-            # only keep the strict upper triangular
-            lower_diag_masks = tf.linalg.LinearOperatorLowerTriangular(tf.ones_like(attention_mask)).to_dense()
-            attention_mask = tf.where(tf.equal(lower_diag_masks, 0),
-                                      attention_mask,
-                                      tf.zeros_like(attention_mask))
-            attention_mask = tf.tile(attention_mask[None, ...], (batch_size, 1, 1))
-            attention_mask = tf.cast(attention_mask, tf.int32)
-
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = self.compute_states_at_sample_times(time_seqs, type_seqs, attention_mask, sample_times)
-
-        if compute_last_step_only:
-            lambdas = self.layer_intensity(encoder_output[:, -1:, :, :])
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = self.layer_intensity(encoder_output)
-        return lambdas
+import math
+
+import torch
+from torch import nn
+
+from easy_tpp.model.torch_model.torch_baselayer import EncoderLayer, MultiHeadAttention
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class AttNHP(TorchBaseModel):
+    """Torch implementation of Attentive Neural Hawkes Process, ICLR 2022.
+    https://arxiv.org/abs/2201.00044.
+    Source code: https://github.com/yangalan123/anhp-andtt/blob/master/anhp/model/xfmr_nhp_fast.py
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(AttNHP, self).__init__(model_config)
+        self.d_model = model_config.hidden_size
+        self.use_norm = model_config.use_ln
+        self.d_time = model_config.time_emb_size
+
+        self.div_term = torch.exp(torch.arange(0, self.d_time, 2) * -(math.log(10000.0) / self.d_time)).reshape(1, 1,
+                                                                                                                -1)
+
+        self.n_layers = model_config.num_layers
+        self.n_head = model_config.num_heads
+        self.dropout = model_config.dropout_rate
+
+        self.heads = []
+        for i in range(self.n_head):
+            self.heads.append(
+                nn.ModuleList(
+                    [EncoderLayer(
+                        self.d_model + self.d_time,
+                        MultiHeadAttention(1, self.d_model + self.d_time, self.d_model, self.dropout,
+                                           output_linear=False),
+
+                        use_residual=False,
+                        dropout=self.dropout
+                    )
+                        for _ in range(self.n_layers)
+                    ]
+                )
+            )
+        self.heads = nn.ModuleList(self.heads)
+
+        if self.use_norm:
+            self.norm = nn.LayerNorm(self.d_model)
+        self.inten_linear = nn.Linear(self.d_model * self.n_head, self.num_event_types)
+        self.softplus = nn.Softplus()
+        self.layer_event_emb = nn.Linear(self.d_model + self.d_time, self.d_model)
+        self.layer_intensity = nn.Sequential(self.inten_linear, self.softplus)
+        self.eps = torch.finfo(torch.float32).eps
+
+    def compute_temporal_embedding(self, time):
+        """Compute the temporal embedding.
+
+        Args:
+            time (tensor): [batch_size, seq_len].
+
+        Returns:
+            tensor: [batch_size, seq_len, emb_size].
+        """
+        batch_size = time.size(0)
+        seq_len = time.size(1)
+        pe = torch.zeros(batch_size, seq_len, self.d_time).to(time)
+        _time = time.unsqueeze(-1)
+        div_term = self.div_term.to(time)
+        pe[..., 0::2] = torch.sin(_time * div_term)
+        pe[..., 1::2] = torch.cos(_time * div_term)
+
+        return pe
+
+    def forward_pass(self, init_cur_layer, time_emb, sample_time_emb, event_emb, combined_mask):
+        """update the structure sequentially.
+
+        Args:
+            init_cur_layer (tensor): [batch_size, seq_len, hidden_size]
+            time_emb (tensor): [batch_size, seq_len, hidden_size]
+            sample_time_emb (tensor): [batch_size, seq_len, hidden_size]
+            event_emb (tensor): [batch_size, seq_len, hidden_size]
+            combined_mask (tensor): [batch_size, seq_len, hidden_size]
+
+        Returns:
+            tensor: [batch_size, seq_len, hidden_size*2]
+        """
+        cur_layers = []
+        seq_len = event_emb.size(1)
+        for head_i in range(self.n_head):
+            # [batch_size, seq_len, hidden_size]
+            cur_layer_ = init_cur_layer
+            for layer_i in range(self.n_layers):
+                # each layer concats the temporal emb
+                # [batch_size, seq_len, hidden_size*2]
+                layer_ = torch.cat([cur_layer_, sample_time_emb], dim=-1)
+                # make combined input from event emb + layer emb
+                # [batch_size, seq_len*2, hidden_size*2]
+                _combined_input = torch.cat([event_emb, layer_], dim=1)
+                enc_layer = self.heads[head_i][layer_i]
+                # compute the output
+                enc_output = enc_layer(_combined_input, combined_mask)
+
+                # the layer output
+                # [batch_size, seq_len, hidden_size]
+                _cur_layer_ = enc_output[:, seq_len:, :]
+                # add residual connection
+                cur_layer_ = torch.tanh(_cur_layer_) + cur_layer_
+
+                # event emb
+                event_emb = torch.cat([enc_output[:, :seq_len, :], time_emb], dim=-1)
+
+                if self.use_norm:
+                    cur_layer_ = self.norm(cur_layer_)
+            cur_layers.append(cur_layer_)
+        cur_layer_ = torch.cat(cur_layers, dim=-1)
+
+        return cur_layer_
+
+    def seq_encoding(self, time_seqs, event_seqs):
+        """Encode the sequence.
+
+        Args:
+            time_seqs (tensor): time seqs input, [batch_size, seq_len].
+            event_seqs (_type_): event type seqs input, [batch_size, seq_len].
+
+        Returns:
+            tuple: event embedding, time embedding and type embedding.
+        """
+        # [batch_size, seq_len, hidden_size]
+        time_emb = self.compute_temporal_embedding(time_seqs)
+        # [batch_size, seq_len, hidden_size]
+        type_emb = torch.tanh(self.layer_type_emb(event_seqs.long()))
+        # [batch_size, seq_len, hidden_size*2]
+        event_emb = torch.cat([type_emb, time_emb], dim=-1)
+
+        return event_emb, time_emb, type_emb
+
+    def make_layer_mask(self, attention_mask):
+        """Create a tensor to do masking on layers.
+
+        Args:
+            attention_mask (tensor): mask for attention operation, [batch_size, seq_len, seq_len]
+
+        Returns:
+            tensor: aim to keep the current layer, the same size of attention mask
+            a diagonal matrix, [batch_size, seq_len, seq_len]
+        """
+        # [batch_size, seq_len, seq_len]
+        layer_mask = (torch.eye(attention_mask.size(1)) < 1).unsqueeze(0).expand_as(attention_mask)
+        return layer_mask
+
+    def make_combined_att_mask(self, attention_mask, layer_mask):
+        """Combined attention mask and layer mask.
+
+        Args:
+            attention_mask (tensor): mask for attention operation, [batch_size, seq_len, seq_len]
+            layer_mask (tensor): mask for other layers, [batch_size, seq_len, seq_len]
+
+        Returns:
+            tensor: [batch_size, seq_len * 2, seq_len * 2]
+        """
+        # [batch_size, seq_len, seq_len * 2]
+        combined_mask = torch.cat([attention_mask, layer_mask], dim=-1)
+        # [batch_size, seq_len, seq_len * 2]
+        contextual_mask = torch.cat([attention_mask, torch.ones_like(layer_mask)], dim=-1)
+        # [batch_size, seq_len * 2, seq_len * 2]
+        combined_mask = torch.cat([contextual_mask, combined_mask], dim=1)
+        return combined_mask
+
+    def forward(self, time_seqs, event_seqs, attention_mask, sample_times=None):
+        """Call the model.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            event_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            attention_mask (tensor): [batch_size, seq_len, seq_len], masks for event sequences.
+            sample_times (tensor, optional): [batch_size, seq_len, num_samples]. Defaults to None.
+
+        Returns:
+            tensor: states at sampling times, [batch_size, seq_len, num_samples].
+        """
+        event_emb, time_emb, type_emb = self.seq_encoding(time_seqs, event_seqs)
+        init_cur_layer = torch.zeros_like(type_emb)
+        layer_mask = self.make_layer_mask(attention_mask)
+        if sample_times is None:
+            sample_time_emb = time_emb
+        else:
+            sample_time_emb = self.compute_temporal_embedding(sample_times)
+        combined_mask = self.make_combined_att_mask(attention_mask, layer_mask)
+        cur_layer_ = self.forward_pass(init_cur_layer, time_emb, sample_time_emb, event_emb, combined_mask)
+
+        return cur_layer_
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch
+        # 1. compute event-loglik
+        # the prediction of last event has no label, so we proceed to the last but one
+        # att mask => diag is False, not mask.
+        enc_out = self.forward(time_seqs[:, :-1], type_seqs[:, :-1], attention_mask[:, 1:, :-1], time_seqs[:, 1:])
+        # [batch_size, seq_len, num_event_types]
+        lambda_at_event = self.layer_intensity(enc_out)
+
+        # 2. compute non-event-loglik (using MC sampling to compute integral)
+        # 2.1 sample times
+        # [batch_size, seq_len, num_sample]
+        temp_time = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        # [batch_size, seq_len, num_sample]
+        sample_times = temp_time + time_seqs[:, :-1].unsqueeze(-1)
+
+        # 2.2 compute intensities at sampled times
+        # [batch_size, seq_len = max_len - 1, num_sample, event_num]
+        lambda_t_sample = self.compute_intensities_at_sample_times(time_seqs[:, :-1],
+                                                                   time_delta_seqs[:, :-1],  # not used
+                                                                   type_seqs[:, :-1],
+                                                                   sample_times,
+                                                                   attention_mask=attention_mask[:, 1:, :-1])
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        # return enc_inten to compute accuracy
+        loss = - (event_ll - non_event_ll).sum()
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self,
+                                       time_seqs,
+                                       type_seqs,
+                                       attention_mask,
+                                       sample_times):
+        """Compute the states at sampling times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            attention_mask (tensor): [batch_size, seq_len, seq_len], masks for event sequences.
+            sample_dtimes (tensor): delta times in sampling.
+
+        Returns:
+            tensor: hiddens states at sampling times.
+        """
+        batch_size = type_seqs.size(0)
+        seq_len = type_seqs.size(1)
+        num_samples = sample_times.size(-1)
+
+        # [num_samples, batch_size, seq_len]
+        sample_times = sample_times.permute((2, 0, 1))
+        # [num_samples * batch_size, seq_len]
+        _sample_time = sample_times.reshape(num_samples * batch_size, -1)
+        # [num_samples * batch_size, seq_len]
+        _types = type_seqs.expand(num_samples, -1, -1).reshape(num_samples * batch_size, -1)
+        # [num_samples * batch_size, seq_len]
+        _times = time_seqs.expand(num_samples, -1, -1).reshape(num_samples * batch_size, -1)
+        # [num_samples * batch_size, seq_len]
+        _attn_mask = attention_mask.unsqueeze(0).expand(num_samples, -1, -1, -1).reshape(num_samples * batch_size,
+                                                                                         seq_len,
+                                                                                         seq_len)
+        # [num_samples * batch_size, seq_len, hidden_size]
+        encoder_output = self.forward(_times,
+                                      _types,
+                                      _attn_mask,
+                                      _sample_time)
+
+        # [num_samples, batch_size, seq_len, hidden_size]
+        encoder_output = encoder_output.reshape(num_samples, batch_size, seq_len, -1)
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = encoder_output.permute((1, 2, 0, 3))
+        return encoder_output
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_times, **kwargs):
+        """Compute the intensity at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
+
+        Returns:
+            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
+        """
+        attention_mask = kwargs.get('attention_mask', None)
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        if attention_mask is None:
+            batch_size, seq_len = time_seqs.size()
+            attention_mask = torch.triu(torch.ones(seq_len, seq_len), diagonal=1).unsqueeze(0)
+            attention_mask = attention_mask.expand(batch_size, -1, -1).to(torch.bool)
+
+        if sample_times.size()[1] < time_seqs.size()[1]:
+            # we pass sample_dtimes for last time step here
+            # we do a temp solution
+            # [batch_size, seq_len, num_samples]
+            sample_times = time_seqs[:, :, None] + torch.tile(sample_times, [1, time_seqs.size()[1], 1])
+
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = self.compute_states_at_sample_times(time_seqs, type_seqs, attention_mask, sample_times)
+
+        if compute_last_step_only:
+            lambdas = self.layer_intensity(encoder_output[:, -1:, :, :])
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = self.layer_intensity(encoder_output)
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_baselayer.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_baselayer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,404 +1,404 @@
-import numpy as np
-import tensorflow as tf
-from tensorflow.python.keras import layers
-
-from easy_tpp.utils import py_assert
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-def gelu(x):
-    """Gaussian Error Linear Unit.
-    This is a smoother version of the RELU.
-    Original paper: https://arxiv.org/abs/1606.08415
-    Args:
-        x: float Tensor to perform activation.
-    Returns:
-        `x` with the GELU activation applied.
-    """
-    cdf = 0.5 * (1.0 + tf.tanh((np.sqrt(2 / np.pi) * (x + 0.044715 * tf.pow(x, 3)))))
-    return x * cdf
-
-
-def swish(x):
-    return x * tf.sigmoid(x)
-
-
-def null_activation(x):
-    return x
-
-
-def activation_layer(activation):
-    if activation.lower() == 'null':
-        return null_activation
-    if activation.lower() == 'gelu':
-        act_layer = gelu
-    elif activation.lower() == 'swish':
-        act_layer = swish
-    elif isinstance(activation, str):
-        act_layer = tf.keras.layers.Activation(activation)
-    elif issubclass(activation, layers.Layer):
-        act_layer = activation()
-    else:
-        raise ValueError(
-            "Invalid activation,found %s.You should use a str or a Activation Layer Class." % (activation))
-    return act_layer
-
-
-def append_tensor_alias(tensor, alias):
-    """Append an alias to the list of aliases of the tensor.
-    Args:
-      tensor: A `Tensor`.
-      alias: String, to add to the list of aliases of the tensor.
-    Returns:
-      The tensor with a new alias appended to its list of aliases.
-    """
-    # Remove ending '/' if present.
-    if alias[-1] == '/':
-        alias = alias[:-1]
-    if hasattr(tensor, 'aliases'):
-        tensor.aliases.append(alias)
-    else:
-        tensor.aliases = [alias]
-    return tensor
-
-
-class LayerNormalization(layers.Layer):
-    """
-
-    ref: https://github.com/shenweichen/DeepCTR/blob/master/deepctr/layers/normalization.py
-
-    """
-
-    def __init__(self, axis=-1, eps=1e-9, center=True,
-                 scale=True, **kwargs):
-        self.axis = axis
-        self.eps = eps
-        self.center = center
-        self.scale = scale
-        super(LayerNormalization, self).__init__(**kwargs)
-
-    def build(self, input_shape):
-        self.gamma = self.add_weight(name='gamma', shape=input_shape[-1:],
-                                     initializer=tf.keras.initializers.Ones(), trainable=True)
-        self.beta = self.add_weight(name='beta', shape=input_shape[-1:],
-                                    initializer=tf.keras.initializers.Zeros(), trainable=True)
-        super(LayerNormalization, self).build(input_shape)
-
-    def call(self, inputs):
-        mean = tf.keras.backend.mean(inputs, axis=self.axis, keepdims=True)
-        variance = tf.keras.backend.mean(tf.keras.backend.square(inputs - mean), axis=-1, keepdims=True)
-        std = tf.keras.backend.sqrt(variance + self.eps)
-        outputs = (inputs - mean) / std
-        if self.scale:
-            outputs *= self.gamma
-        if self.center:
-            outputs += self.beta
-        return outputs
-
-
-class MultiHeadAttention(layers.Layer):
-    def __init__(self, hidden_size, num_heads, dropout_rate, **kwargs):
-        super(MultiHeadAttention, self).__init__(**kwargs)
-        self.hidden_size = hidden_size
-        self.num_heads = num_heads
-        py_assert(hidden_size % num_heads == 0, ValueError, 'In Attention, hidden size '
-                                                            'must be a multiplier of num_heads')
-        self.head_size = int(hidden_size / num_heads)
-        self.dropout = layers.Dropout(dropout_rate)
-
-    def build(self, input_shape):
-        """Build up weight tensors.
-
-        Args:
-            input_shape (tensor): shape of the input.
-        """
-        self.q_head_weight = self.add_weight(
-            shape=(self.hidden_size, self.head_size * self.num_heads),
-            initializer=tf.keras.initializers.TruncatedNormal(),
-            dtype=tf.float32,
-            name='query/kernel')
-
-        self.k_head_weight = self.add_weight(
-            shape=(self.hidden_size, self.head_size * self.num_heads),
-            initializer=tf.keras.initializers.TruncatedNormal(),
-            dtype=tf.float32,
-            name='key/kernel')
-
-        self.v_head_weight = self.add_weight(
-            shape=(self.hidden_size, self.head_size * self.num_heads),
-            initializer=tf.keras.initializers.TruncatedNormal(),
-            dtype=tf.float32,
-            name='value/kernel')
-
-        self.q_head_bias = self.add_weight(
-            shape=(self.head_size * self.num_heads,),
-            initializer=tf.keras.initializers.TruncatedNormal(),
-            dtype=tf.float32,
-            name='query/bias')
-
-        self.k_head_bias = self.add_weight(
-            shape=(self.head_size * self.num_heads,),
-            initializer=tf.keras.initializers.TruncatedNormal(),
-            dtype=tf.float32,
-            name='key/bias')
-
-        self.v_head_bias = self.add_weight(
-            shape=(self.head_size * self.num_heads,),
-            initializer=tf.keras.initializers.TruncatedNormal(),
-            dtype=tf.float32,
-            name='value/bias')
-
-        super(MultiHeadAttention, self).build(input_shape)
-
-    def _abs_attn_core(self, q_head, k_head, v_head, attn_mask, training,
-                       scale):
-        """Compute the attention weight score.
-
-        Args:
-            q_head (tensor): [batch_size, q_seq_len, num_head, head_size].
-            k_head (tensor): [batch_size, kv_seq_len, num_head, head_size].
-            v_head (tensor): [batch_size, kv_seq_len, num_head, head_size].
-            attn_mask (tensor): [batch_size, q_seq_len, kv_seq_len].
-            training (bool): whether in training mode.
-            scale (float): equals to 1 / (head_size ** 0.5), which scales down the attention score.
-
-        Returns:
-            tuple: attention context vector, [batch_size, q_seq_len, num_head, head_size];
-             and attention weight [batch_size, num_head, q_seq_len, kv_seq_len].
-        """
-        # [batch_size, num_head, q_seq_len, kv_seq_len]
-        attn_score = tf.einsum('bind,bjnd->bnij', q_head, k_head)
-
-        # [batch_size, num_head, q_seq_len, kv_seq_len]
-        attn_score = tf.multiply(attn_score, scale)
-
-        # [batch_size, 1, q_seq_len, kv_seq_len]
-        attn_mask = tf.expand_dims(attn_mask, axis=[1])
-
-        # elements 1 => need to mask, 0 => no mask
-        # adder = (1.0 - tf.cast(attn_mask, tf.float32)) * -10000.0
-        adder = tf.cast(attn_mask, tf.float32) * -10000.0
-        attn_score += adder
-
-        # [batch_size, num_head, q_seq_len, kv_seq_len]
-        attn_prob = tf.nn.softmax(attn_score)
-        attn_prob = self.dropout(attn_prob, training=training)
-
-        # [batch_size, q_seq_len, num_head, head_size]
-        attn_vec = tf.einsum('bnij,bjnd->bind', attn_prob, v_head)
-        return attn_vec, attn_prob
-
-    def call(self, attention_input, attention_mask, kv=None, training=False, output_weight=False, **kwargs):
-
-        q_input = attention_input
-        if kv is None:
-            k_input = attention_input
-            v_input = attention_input
-        else:
-            k_input = v_input = kv
-
-        batch_size, q_seq_length, kv_seq_length = get_shape_list(attention_mask)
-
-        q_head_h = tf.einsum('bih,hx->bix', q_input, self.q_head_weight)
-        q_head_h = tf.nn.bias_add(q_head_h, self.q_head_bias)
-
-        k_head_h = tf.einsum('bih,hx->bix', k_input, self.k_head_weight)
-        k_head_h = tf.nn.bias_add(k_head_h, self.k_head_bias)
-
-        v_head_h = tf.einsum('bih,hx->bix', v_input, self.v_head_weight)
-        v_head_h = tf.nn.bias_add(v_head_h, self.v_head_bias)
-
-        q_head_h = tf.reshape(q_head_h, [batch_size, q_seq_length, self.num_heads, self.head_size])
-        k_head_h = tf.reshape(k_head_h, [batch_size, kv_seq_length, self.num_heads, self.head_size])
-        v_head_h = tf.reshape(v_head_h, [batch_size, kv_seq_length, self.num_heads, self.head_size])
-
-        scale = 1 / (self.head_size ** 0.5)
-        attn_vec, attn_prob = self._abs_attn_core(q_head_h, k_head_h, v_head_h, attention_mask, training, scale)
-        attn_vec = tf.reshape(attn_vec, [batch_size, q_seq_length, self.head_size * self.num_heads])
-        if output_weight:
-            return attn_vec, attn_prob
-        else:
-            return attn_vec
-
-
-class DenseDropoutLayernorm(layers.Layer):
-    def __init__(self, hidden_size, dropout_rate, **kwargs):
-        super(DenseDropoutLayernorm, self).__init__(**kwargs)
-        self.dense = layers.Dense(hidden_size)
-        self.LayerNorm = LayerNormalization()
-        self.dropout = layers.Dropout(dropout_rate)
-
-    def call(self, inputs, training=False):
-        hidden_states, input_tensor = inputs
-        hidden_states = self.dense(hidden_states)
-        hidden_states = self.dropout(hidden_states, training=training)
-        hidden_states = self.LayerNorm(hidden_states + input_tensor)
-        return hidden_states
-
-
-class EncoderLayer(layers.Layer):
-    def __init__(self, hidden_size, num_heads, dropout_rate, **kwargs):
-        super(EncoderLayer, self).__init__(**kwargs)
-        self.input_layer = layers.Dense(hidden_size)
-        self.self_attention = MultiHeadAttention(hidden_size, num_heads, dropout_rate)
-        self.dense_output = DenseDropoutLayernorm(hidden_size, dropout_rate)
-
-    def call(self, inputs, training=False):
-        input_tensor, attention_mask = inputs
-        input_tensor = self.input_layer(input_tensor)
-        self_outputs = self.self_attention(input_tensor, attention_mask, training=training)
-        attention_output = self.dense_output([self_outputs, input_tensor], training=training)
-        return attention_output
-
-
-class TimePositionalEncoding(layers.Layer):
-    def __init__(self, hidden_size, max_len=5000):
-        """Standard positional encoder,
-        source code is from https://www.tensorflow.org/text/tutorials/transformer#the_encoder_layer
-        Args:
-            hidden_size (int):
-            max_len:
-        """
-        super(TimePositionalEncoding, self).__init__()
-
-        depth = hidden_size / 2
-        # [max_len, 1]
-        positions = np.arange(max_len)[:, None]
-        # [1, depth]
-        depths = np.arange(depth)[None, :] / depth
-        # [1, depth]
-        angle_rates = 1 / (10000 ** depths)
-        # [max_len, depth]
-        self.angle_rads = positions * angle_rates
-
-        pos_encoding = np.concatenate(
-            [np.sin(self.angle_rads), np.cos(self.angle_rads)],
-            axis=-1)
-
-        # [1, max_len, model_dim]
-        self.pe = tf.cast(pos_encoding, dtype=tf.float32)[None, ...]
-
-    def call(self, inputs, **kwargs):
-        """Compute time positional encoding defined in Equation (2) in THP model.
-
-        Args:
-            inputs: (tensor), [batch_size, seq_len]
-            **kwargs:
-
-        Returns:
-            positional encoding
-
-        """
-
-        _, seq_len = get_shape_list(inputs)
-
-        return self.pe[:, :seq_len]
-
-
-class TimeShiftedPositionalEncoding(TimePositionalEncoding):
-    def __init__(self, hidden_size, max_len=5000):
-        super(TimeShiftedPositionalEncoding, self).__init__(hidden_size, max_len)
-        self.hidden_size = hidden_size
-
-        self.layer_time_delta = layers.Dense(hidden_size // 2)
-
-        depth = self.hidden_size / 2
-
-        # [1, depth]
-        self.depths = tf.cast(tf.range(depth)[None, :] / depth, tf.float32)
-
-    def call(self, inputs, **kwargs):
-        """Compute time shifted positional encoding defined in Equation (8) in SAHP model
-
-        Args:
-            inputs: (time_seqs, time_delta_seqs), [batch_size, seq_len]
-            **kwargs:
-
-        Returns:
-            positional encoding
-
-        """
-        time_seqs, time_delta_seqs = inputs
-        _, seq_len = get_shape_list(time_seqs)
-
-        # [batch_size, seq_len, model_dim //2]
-        phi = self.layer_time_delta(time_delta_seqs[..., None])
-
-        # [seq_len, 1]
-        self.positions = tf.cast(tf.range(seq_len)[:, None], tf.float32)
-
-        # [1, model_dim // 2]
-        angle_rates = 1 / (10000 ** self.depths)
-        arc = (tf.multiply(self.positions, angle_rates))[None, ...]
-
-        pe_sin = tf.sin(arc + phi)
-        pe_cos = tf.cos(arc + phi)
-        pe = tf.concat([pe_sin, pe_cos], axis=-1)
-
-        return pe
-
-
-class DNN(layers.Layer):
-    """The Multi Layer Percetron
-      Input shape
-        - nD tensor with shape: ``(batch_size, ..., input_dim)``.
-        The most common situation would be a 2D input with shape ``(batch_size, input_dim)``.
-      Output shape
-        - nD tensor with shape: ``(batch_size, ..., hidden_size[-1])``.
-        For instance, for a 2D input with shape ``(batch_size, input_dim)``,
-        the output would have shape ``(batch_size, hidden_size[-1])``.
-      Arguments
-        - **hidden_units**:list of positive integer, the layer number and units in each layer.
-        - **activation**: Activation function to use.
-        - **l2_reg**: float between 0 and 1. L2 regularizer strength applied to the kernel weights matrix.
-        - **dropout_rate**: float in [0,1). Fraction of the units to dropout.
-        - **use_bn**: bool. Whether use BatchNormalization before activation or not.
-        - **output_activation**: Activation function to use in the last layer.If ``None``,
-        it will be same as ``activation``.
-        - **seed**: A Python integer to use as random seed.
-    """
-
-    def __init__(self, hidden_size, activation='relu', l2_reg=0, dropout_rate=0, use_bn=False,
-                 output_activation=None,
-                 **kwargs):
-        self.hidden_size = hidden_size if isinstance(hidden_size, list) else [hidden_size]
-        self.activation = activation
-        self.l2_reg = l2_reg
-        self.dropout_rate = dropout_rate
-        self.use_bn = use_bn
-        self.output_activation = output_activation
-
-        self.dense_layers = [layers.Dense(self.hidden_size[i]) for i in range(len(self.hidden_size))]
-        if self.use_bn:
-            self.bn_layers = [tf.keras.layers.BatchNormalization() for _ in range(len(self.hidden_size))]
-
-        self.dropout_layers = [tf.keras.layers.Dropout(self.dropout_rate) for _ in
-                               range(len(self.hidden_size))]
-
-        self.activation_layers = [activation_layer(self.activation) for _ in range(len(self.hidden_size))]
-
-        if self.output_activation:
-            self.activation_layers[-1] = activation_layer(self.output_activation)
-
-        super(DNN, self).__init__(**kwargs)
-
-    def call(self, inputs, training=None, **kwargs):
-
-        deep_input = inputs
-
-        for i in range(len(self.hidden_size)):
-            fc = self.dense_layers[i](deep_input)
-
-            if self.use_bn:
-                fc = self.bn_layers[i](fc, training=training)
-
-            fc = self.activation_layers[i](fc)
-
-            fc = self.dropout_layers[i](fc, training=training)
-            deep_input = fc
-
-        return deep_input
+import numpy as np
+import tensorflow as tf
+from tensorflow.python.keras import layers
+
+from easy_tpp.utils import py_assert
+from easy_tpp.utils.tf_utils import get_shape_list
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+def gelu(x):
+    """Gaussian Error Linear Unit.
+    This is a smoother version of the RELU.
+    Original paper: https://arxiv.org/abs/1606.08415
+    Args:
+        x: float Tensor to perform activation.
+    Returns:
+        `x` with the GELU activation applied.
+    """
+    cdf = 0.5 * (1.0 + tf.tanh((np.sqrt(2 / np.pi) * (x + 0.044715 * tf.pow(x, 3)))))
+    return x * cdf
+
+
+def swish(x):
+    return x * tf.sigmoid(x)
+
+
+def null_activation(x):
+    return x
+
+
+def activation_layer(activation):
+    if activation.lower() == 'null':
+        return null_activation
+    if activation.lower() == 'gelu':
+        act_layer = gelu
+    elif activation.lower() == 'swish':
+        act_layer = swish
+    elif isinstance(activation, str):
+        act_layer = tf.keras.layers.Activation(activation)
+    elif issubclass(activation, layers.Layer):
+        act_layer = activation()
+    else:
+        raise ValueError(
+            "Invalid activation,found %s.You should use a str or a Activation Layer Class." % (activation))
+    return act_layer
+
+
+def append_tensor_alias(tensor, alias):
+    """Append an alias to the list of aliases of the tensor.
+    Args:
+      tensor: A `Tensor`.
+      alias: String, to add to the list of aliases of the tensor.
+    Returns:
+      The tensor with a new alias appended to its list of aliases.
+    """
+    # Remove ending '/' if present.
+    if alias[-1] == '/':
+        alias = alias[:-1]
+    if hasattr(tensor, 'aliases'):
+        tensor.aliases.append(alias)
+    else:
+        tensor.aliases = [alias]
+    return tensor
+
+
+class LayerNormalization(layers.Layer):
+    """
+
+    ref: https://github.com/shenweichen/DeepCTR/blob/master/deepctr/layers/normalization.py
+
+    """
+
+    def __init__(self, axis=-1, eps=1e-9, center=True,
+                 scale=True, **kwargs):
+        self.axis = axis
+        self.eps = eps
+        self.center = center
+        self.scale = scale
+        super(LayerNormalization, self).__init__(**kwargs)
+
+    def build(self, input_shape):
+        self.gamma = self.add_weight(name='gamma', shape=input_shape[-1:],
+                                     initializer=tf.keras.initializers.Ones(), trainable=True)
+        self.beta = self.add_weight(name='beta', shape=input_shape[-1:],
+                                    initializer=tf.keras.initializers.Zeros(), trainable=True)
+        super(LayerNormalization, self).build(input_shape)
+
+    def call(self, inputs):
+        mean = tf.keras.backend.mean(inputs, axis=self.axis, keepdims=True)
+        variance = tf.keras.backend.mean(tf.keras.backend.square(inputs - mean), axis=-1, keepdims=True)
+        std = tf.keras.backend.sqrt(variance + self.eps)
+        outputs = (inputs - mean) / std
+        if self.scale:
+            outputs *= self.gamma
+        if self.center:
+            outputs += self.beta
+        return outputs
+
+
+class MultiHeadAttention(layers.Layer):
+    def __init__(self, hidden_size, num_heads, dropout_rate, **kwargs):
+        super(MultiHeadAttention, self).__init__(**kwargs)
+        self.hidden_size = hidden_size
+        self.num_heads = num_heads
+        py_assert(hidden_size % num_heads == 0, ValueError, 'In Attention, hidden size '
+                                                            'must be a multiplier of num_heads')
+        self.head_size = int(hidden_size / num_heads)
+        self.dropout = layers.Dropout(dropout_rate)
+
+    def build(self, input_shape):
+        """Build up weight tensors.
+
+        Args:
+            input_shape (tensor): shape of the input.
+        """
+        self.q_head_weight = self.add_weight(
+            shape=(self.hidden_size, self.head_size * self.num_heads),
+            initializer=tf.keras.initializers.TruncatedNormal(),
+            dtype=tf.float32,
+            name='query/kernel')
+
+        self.k_head_weight = self.add_weight(
+            shape=(self.hidden_size, self.head_size * self.num_heads),
+            initializer=tf.keras.initializers.TruncatedNormal(),
+            dtype=tf.float32,
+            name='key/kernel')
+
+        self.v_head_weight = self.add_weight(
+            shape=(self.hidden_size, self.head_size * self.num_heads),
+            initializer=tf.keras.initializers.TruncatedNormal(),
+            dtype=tf.float32,
+            name='value/kernel')
+
+        self.q_head_bias = self.add_weight(
+            shape=(self.head_size * self.num_heads,),
+            initializer=tf.keras.initializers.TruncatedNormal(),
+            dtype=tf.float32,
+            name='query/bias')
+
+        self.k_head_bias = self.add_weight(
+            shape=(self.head_size * self.num_heads,),
+            initializer=tf.keras.initializers.TruncatedNormal(),
+            dtype=tf.float32,
+            name='key/bias')
+
+        self.v_head_bias = self.add_weight(
+            shape=(self.head_size * self.num_heads,),
+            initializer=tf.keras.initializers.TruncatedNormal(),
+            dtype=tf.float32,
+            name='value/bias')
+
+        super(MultiHeadAttention, self).build(input_shape)
+
+    def _abs_attn_core(self, q_head, k_head, v_head, attn_mask, training,
+                       scale):
+        """Compute the attention weight score.
+
+        Args:
+            q_head (tensor): [batch_size, q_seq_len, num_head, head_size].
+            k_head (tensor): [batch_size, kv_seq_len, num_head, head_size].
+            v_head (tensor): [batch_size, kv_seq_len, num_head, head_size].
+            attn_mask (tensor): [batch_size, q_seq_len, kv_seq_len].
+            training (bool): whether in training mode.
+            scale (float): equals to 1 / (head_size ** 0.5), which scales down the attention score.
+
+        Returns:
+            tuple: attention context vector, [batch_size, q_seq_len, num_head, head_size];
+             and attention weight [batch_size, num_head, q_seq_len, kv_seq_len].
+        """
+        # [batch_size, num_head, q_seq_len, kv_seq_len]
+        attn_score = tf.einsum('bind,bjnd->bnij', q_head, k_head)
+
+        # [batch_size, num_head, q_seq_len, kv_seq_len]
+        attn_score = tf.multiply(attn_score, scale)
+
+        # [batch_size, 1, q_seq_len, kv_seq_len]
+        attn_mask = tf.expand_dims(attn_mask, axis=[1])
+
+        # elements 1 => need to mask, 0 => no mask
+        # adder = (1.0 - tf.cast(attn_mask, tf.float32)) * -10000.0
+        adder = tf.cast(attn_mask, tf.float32) * -10000.0
+        attn_score += adder
+
+        # [batch_size, num_head, q_seq_len, kv_seq_len]
+        attn_prob = tf.nn.softmax(attn_score)
+        attn_prob = self.dropout(attn_prob, training=training)
+
+        # [batch_size, q_seq_len, num_head, head_size]
+        attn_vec = tf.einsum('bnij,bjnd->bind', attn_prob, v_head)
+        return attn_vec, attn_prob
+
+    def call(self, attention_input, attention_mask, kv=None, training=False, output_weight=False, **kwargs):
+
+        q_input = attention_input
+        if kv is None:
+            k_input = attention_input
+            v_input = attention_input
+        else:
+            k_input = v_input = kv
+
+        batch_size, q_seq_length, kv_seq_length = get_shape_list(attention_mask)
+
+        q_head_h = tf.einsum('bih,hx->bix', q_input, self.q_head_weight)
+        q_head_h = tf.nn.bias_add(q_head_h, self.q_head_bias)
+
+        k_head_h = tf.einsum('bih,hx->bix', k_input, self.k_head_weight)
+        k_head_h = tf.nn.bias_add(k_head_h, self.k_head_bias)
+
+        v_head_h = tf.einsum('bih,hx->bix', v_input, self.v_head_weight)
+        v_head_h = tf.nn.bias_add(v_head_h, self.v_head_bias)
+
+        q_head_h = tf.reshape(q_head_h, [batch_size, q_seq_length, self.num_heads, self.head_size])
+        k_head_h = tf.reshape(k_head_h, [batch_size, kv_seq_length, self.num_heads, self.head_size])
+        v_head_h = tf.reshape(v_head_h, [batch_size, kv_seq_length, self.num_heads, self.head_size])
+
+        scale = 1 / (self.head_size ** 0.5)
+        attn_vec, attn_prob = self._abs_attn_core(q_head_h, k_head_h, v_head_h, attention_mask, training, scale)
+        attn_vec = tf.reshape(attn_vec, [batch_size, q_seq_length, self.head_size * self.num_heads])
+        if output_weight:
+            return attn_vec, attn_prob
+        else:
+            return attn_vec
+
+
+class DenseDropoutLayernorm(layers.Layer):
+    def __init__(self, hidden_size, dropout_rate, **kwargs):
+        super(DenseDropoutLayernorm, self).__init__(**kwargs)
+        self.dense = layers.Dense(hidden_size)
+        self.LayerNorm = LayerNormalization()
+        self.dropout = layers.Dropout(dropout_rate)
+
+    def call(self, inputs, training=False):
+        hidden_states, input_tensor = inputs
+        hidden_states = self.dense(hidden_states)
+        hidden_states = self.dropout(hidden_states, training=training)
+        hidden_states = self.LayerNorm(hidden_states + input_tensor)
+        return hidden_states
+
+
+class EncoderLayer(layers.Layer):
+    def __init__(self, hidden_size, num_heads, dropout_rate, **kwargs):
+        super(EncoderLayer, self).__init__(**kwargs)
+        self.input_layer = layers.Dense(hidden_size)
+        self.self_attention = MultiHeadAttention(hidden_size, num_heads, dropout_rate)
+        self.dense_output = DenseDropoutLayernorm(hidden_size, dropout_rate)
+
+    def call(self, inputs, training=False):
+        input_tensor, attention_mask = inputs
+        input_tensor = self.input_layer(input_tensor)
+        self_outputs = self.self_attention(input_tensor, attention_mask, training=training)
+        attention_output = self.dense_output([self_outputs, input_tensor], training=training)
+        return attention_output
+
+
+class TimePositionalEncoding(layers.Layer):
+    def __init__(self, hidden_size, max_len=5000):
+        """Standard positional encoder,
+        source code is from https://www.tensorflow.org/text/tutorials/transformer#the_encoder_layer
+        Args:
+            hidden_size (int):
+            max_len:
+        """
+        super(TimePositionalEncoding, self).__init__()
+
+        depth = hidden_size / 2
+        # [max_len, 1]
+        positions = np.arange(max_len)[:, None]
+        # [1, depth]
+        depths = np.arange(depth)[None, :] / depth
+        # [1, depth]
+        angle_rates = 1 / (10000 ** depths)
+        # [max_len, depth]
+        self.angle_rads = positions * angle_rates
+
+        pos_encoding = np.concatenate(
+            [np.sin(self.angle_rads), np.cos(self.angle_rads)],
+            axis=-1)
+
+        # [1, max_len, model_dim]
+        self.pe = tf.cast(pos_encoding, dtype=tf.float32)[None, ...]
+
+    def call(self, inputs, **kwargs):
+        """Compute time positional encoding defined in Equation (2) in THP model.
+
+        Args:
+            inputs: (tensor), [batch_size, seq_len]
+            **kwargs:
+
+        Returns:
+            positional encoding
+
+        """
+
+        _, seq_len = get_shape_list(inputs)
+
+        return self.pe[:, :seq_len]
+
+
+class TimeShiftedPositionalEncoding(TimePositionalEncoding):
+    def __init__(self, hidden_size, max_len=5000):
+        super(TimeShiftedPositionalEncoding, self).__init__(hidden_size, max_len)
+        self.hidden_size = hidden_size
+
+        self.layer_time_delta = layers.Dense(hidden_size // 2)
+
+        depth = self.hidden_size / 2
+
+        # [1, depth]
+        self.depths = tf.cast(tf.range(depth)[None, :] / depth, tf.float32)
+
+    def call(self, inputs, **kwargs):
+        """Compute time shifted positional encoding defined in Equation (8) in SAHP model
+
+        Args:
+            inputs: (time_seqs, time_delta_seqs), [batch_size, seq_len]
+            **kwargs:
+
+        Returns:
+            positional encoding
+
+        """
+        time_seqs, time_delta_seqs = inputs
+        _, seq_len = get_shape_list(time_seqs)
+
+        # [batch_size, seq_len, model_dim //2]
+        phi = self.layer_time_delta(time_delta_seqs[..., None])
+
+        # [seq_len, 1]
+        self.positions = tf.cast(tf.range(seq_len)[:, None], tf.float32)
+
+        # [1, model_dim // 2]
+        angle_rates = 1 / (10000 ** self.depths)
+        arc = (tf.multiply(self.positions, angle_rates))[None, ...]
+
+        pe_sin = tf.sin(arc + phi)
+        pe_cos = tf.cos(arc + phi)
+        pe = tf.concat([pe_sin, pe_cos], axis=-1)
+
+        return pe
+
+
+class DNN(layers.Layer):
+    """The Multi Layer Percetron
+      Input shape
+        - nD tensor with shape: ``(batch_size, ..., input_dim)``.
+        The most common situation would be a 2D input with shape ``(batch_size, input_dim)``.
+      Output shape
+        - nD tensor with shape: ``(batch_size, ..., hidden_size[-1])``.
+        For instance, for a 2D input with shape ``(batch_size, input_dim)``,
+        the output would have shape ``(batch_size, hidden_size[-1])``.
+      Arguments
+        - **hidden_units**:list of positive integer, the layer number and units in each layer.
+        - **activation**: Activation function to use.
+        - **l2_reg**: float between 0 and 1. L2 regularizer strength applied to the kernel weights matrix.
+        - **dropout_rate**: float in [0,1). Fraction of the units to dropout.
+        - **use_bn**: bool. Whether use BatchNormalization before activation or not.
+        - **output_activation**: Activation function to use in the last layer.If ``None``,
+        it will be same as ``activation``.
+        - **seed**: A Python integer to use as random seed.
+    """
+
+    def __init__(self, hidden_size, activation='relu', l2_reg=0, dropout_rate=0, use_bn=False,
+                 output_activation=None,
+                 **kwargs):
+        self.hidden_size = hidden_size if isinstance(hidden_size, list) else [hidden_size]
+        self.activation = activation
+        self.l2_reg = l2_reg
+        self.dropout_rate = dropout_rate
+        self.use_bn = use_bn
+        self.output_activation = output_activation
+
+        self.dense_layers = [layers.Dense(self.hidden_size[i]) for i in range(len(self.hidden_size))]
+        if self.use_bn:
+            self.bn_layers = [tf.keras.layers.BatchNormalization() for _ in range(len(self.hidden_size))]
+
+        self.dropout_layers = [tf.keras.layers.Dropout(self.dropout_rate) for _ in
+                               range(len(self.hidden_size))]
+
+        self.activation_layers = [activation_layer(self.activation) for _ in range(len(self.hidden_size))]
+
+        if self.output_activation:
+            self.activation_layers[-1] = activation_layer(self.output_activation)
+
+        super(DNN, self).__init__(**kwargs)
+
+    def call(self, inputs, training=None, **kwargs):
+
+        deep_input = inputs
+
+        for i in range(len(self.hidden_size)):
+            fc = self.dense_layers[i](deep_input)
+
+            if self.use_bn:
+                fc = self.bn_layers[i](fc, training=training)
+
+            fc = self.activation_layers[i](fc)
+
+            fc = self.dropout_layers[i](fc, training=training)
+            deep_input = fc
+
+        return deep_input
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_basemodel.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_sahp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,271 +1,222 @@
-""" Base model with common functionality  """
-
-import tensorflow as tf
-
-from easy_tpp.model.tf_model.tf_thinning import EventSampler
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class TfBaseModel(tf.keras.Model):
-    def __init__(self, model_config):
-        super(TfBaseModel, self).__init__()
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        self.model_config = model_config
-
-        self.loss_integral_num_sample_per_step = model_config.loss_integral_num_sample_per_step
-        self.hidden_size = model_config.hidden_size
-        self.num_event_types = model_config.num_event_types  # not include [PAD]
-        self.num_event_types_pad = model_config.num_event_types_pad  # include [PAD]
-        self.event_pad_index = model_config.pad_token_id
-        self.dropout_rate = model_config.dropout_rate
-
-        self.eps = 1e-7
-
-        self.layer_type_emb = tf.keras.layers.Embedding(self.num_event_types_pad,
-                                                        self.hidden_size)
-
-        self.gen_config = model_config.thinning
-        self.event_sampler = None
-        if self.gen_config:
-            self.event_sampler = EventSampler(num_sample=self.gen_config.num_sample,
-                                              num_exp=self.gen_config.num_exp,
-                                              over_sample_rate=self.gen_config.over_sample_rate,
-                                              patience_counter=self.gen_config.patience_counter,
-                                              num_samples_boundary=self.gen_config.num_samples_boundary,
-                                              dtime_max=self.gen_config.dtime_max)
-
-    def build_input_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('BaseModel'):
-            # Input placeholder
-            # shape - (batch_size, max_len)
-            # max_len - sequence length including time zero padding
-            self.time_delta_seqs = tf.placeholder(tf.float32, shape=[None, None])
-
-            # shape - (batch_size, max_len)
-            self.time_seqs = tf.placeholder(tf.float32, shape=[None, None])
-
-            # shape - (batch_size, max_len)
-            self.type_seqs = tf.placeholder(tf.int32, shape=[None, None])
-
-            # shape - (batch_size, max_len)
-            self.batch_non_pad_mask = tf.placeholder(tf.int32, shape=[None, None])
-
-            # shape - (batch_size, max_len, max_len)
-            self.attention_mask = tf.placeholder(tf.int32, shape=[None, None, None])
-
-            # Event type one-hot code
-            # shape - (batch_size, max_len, num_event_types)
-            self.type_mask = tf.placeholder(tf.float32, shape=[None, None, None])
-
-            # shape - (batch_size 1)
-            self.seq_len = tf.cast(tf.reduce_sum(tf.cast(self.batch_non_pad_mask, tf.float32), axis=1, keepdims=True),
-                                   tf.int32)
-
-            self.is_training = tf.placeholder(tf.bool)
-
-        return
-
-    @staticmethod
-    def generate_model_from_config(model_config):
-        """Generate the model in derived class based on model config.
-
-        Args:
-            model_config (EasyTPP.Config): config of model specs.
-        """
-        model_id = model_config.model_id
-
-        for subclass in TfBaseModel.__subclasses__():
-            if subclass.__name__ == model_id:
-                return subclass(model_config)
-
-        raise RuntimeError('No model named ' + model_id)
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, event_seqs, sampled_dtimes):
-        raise NotImplementedError
-
-    def make_dtime_loss_samples(self, time_delta_seq):
-        """Generate the time point samples for every interval.
-
-        Args:
-            time_delta_seq (tensor): [batch_size, seq_len].
-
-        Returns:
-            tensor: [batch_size, seq_len, n_samples]
-        """
-        # shape  (1, 1, n_samples)
-        dtimes_ratio_sampled = tf.linspace(start=0.0,
-                                           stop=1.0,
-                                           num=self.loss_integral_num_sample_per_step)[None, None, :]
-
-        # shape (batch_size, max_len, n_samples)
-        sampled_dtimes = time_delta_seq[:, :, None] * dtimes_ratio_sampled
-
-        return sampled_dtimes
-
-    def compute_loglikelihood(self, time_delta_seq, lambda_at_event, lambdas_loss_samples, seq_mask,
-                              lambda_type_mask):
-        """Compute the loglikelihood of the event sequence based on Equation (8) of NHP paper.
-
-        Args:
-            time_delta_seq (tensor): [batch_size, seq_len], time_delta_seq from model input.
-            lambda_at_event (tensor): [batch_size, seq_len, num_event_types], unmasked intensity at
-            (right after) the event.
-            lambdas_loss_samples (tensor): [batch_size, seq_len, num_sample, num_event_types],
-            intensity at sampling times.
-            seq_mask (tensor): [batch_size, seq_len], sequence mask vector to mask the padded events.
-            lambda_type_mask (tensor): [batch_size, seq_len, num_event_types], type mask matrix to mask
-            the padded event types.
-
-        Returns:
-            tuple: event loglike, non event loglike, intensity at event with padding events masked
-        """
-
-        # Sum of lambda over every type
-        # [batch_size, seq_len]
-        event_lambdas = tf.reduce_sum(lambda_at_event * lambda_type_mask, axis=-1)
-
-        # mask the pad event
-        event_lambdas = tf.boolean_mask(event_lambdas, seq_mask)
-
-        # Sum of lambda over every event point
-        # [num_unmasked_events]
-        event_ll = tf.reduce_sum(tf.log(event_lambdas))
-
-        # Compute the big lambda integral in Equation (8) of NHP paper
-        # 1 - take num_mc_sample rand points in each event interval
-        # 2 - compute its lambda value for every sample point
-        # 3 - take average of these sample points
-        # 4 - times the interval length
-
-        # [batch_size, max_len, n_loss_sample]
-        lambdas_total_samples = tf.reduce_sum(lambdas_loss_samples, axis=-1)
-
-        # interval_integral - [batch_size, num_times]
-        # interval_integral = length_interval * average of sampled lambda(t)
-        non_event_ll = tf.reduce_mean(lambdas_total_samples, axis=-1) * time_delta_seq * tf.cast(seq_mask, tf.float32)
-
-        non_event_ll = tf.reduce_sum(non_event_ll)
-
-        num_events = get_shape_list(event_lambdas)[0]
-
-        return event_ll, non_event_ll, num_events
-
-    def predict_one_step_at_every_event(self, time_seqs, time_delta_seqs, type_seqs):
-        """One-step prediction for every event in the sequence.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len].
-            time_delta_seqs (tensor): [batch_size, seq_len].
-            type_seqs (tensor): [batch_size, seq_len].
-
-        Returns:
-            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
-        """
-
-        # remove the last event, as the prediction based on the last event has no label
-        time_seqs, time_delta_seqs, type_seqs = time_seqs[:, :-1], time_delta_seqs[:, 1:], type_seqs[:, :-1]
-
-        # (batch_size, seq_len)
-        dtime_boundary = time_delta_seqs + self.event_sampler.dtime_max
-
-        # [batch_size, seq_len, num_sample]
-        accepted_dtimes, weights = self.event_sampler.draw_next_time_one_step(time_seqs,
-                                                                              time_delta_seqs,
-                                                                              type_seqs,
-                                                                              dtime_boundary,
-                                                                              self.compute_intensities_at_sample_times,
-                                                                              compute_last_step_only=False)
-
-        # [batch_size, seq_len]
-        dtimes_pred = tf.reduce_sum(accepted_dtimes * weights, axis=-1)
-
-        # [batch_size, seq_len, 1, event_num]
-        intensities_at_times = self.compute_intensities_at_sample_times(time_seqs,
-                                                                        time_delta_seqs,
-                                                                        type_seqs,
-                                                                        dtimes_pred[:, :, None])
-
-        # [batch_size, seq_len, event_num]
-        intensities_at_times = tf.squeeze(intensities_at_times, axis=-2)
-
-        # [batch_size, seq_len]
-        types_pred = tf.argmax(intensities_at_times, axis=-1)
-
-        return dtimes_pred, types_pred
-
-    def predict_multi_step_since_last_event(self, time_seqs, time_delta_seqs, type_seqs, num_step):
-        """Multi-step prediction for every event in the sequence.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len].
-            time_delta_seqs (tensor): [batch_size, seq_len].
-            type_seqs (tensor): [batch_size, seq_len].
-            num_step (int): num of steps for prediction.
-
-        Returns:
-            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
-        """
-        i = tf.constant(0)
-
-        time_seqs_ = time_seqs
-        time_delta_seqs_ = time_delta_seqs
-        type_seqs_ = type_seqs
-
-        def while_condition(i, time_seqs_, time_delta_seqs_, type_seqs_):
-            return tf.less(i, num_step)
-
-        def body(i, time_seqs_, time_delta_seqs_, type_seqs_):
-            # [batch_size, seq_len]
-            dtime_boundary = time_delta_seqs_ + self.event_sampler.dtime_max
-
-            # [batch_size, seq_len, num_sample]
-            accepted_dtimes, weights = \
-                self.event_sampler.draw_next_time_one_step(time_seqs_,
-                                                           time_delta_seqs_,
-                                                           type_seqs_,
-                                                           dtime_boundary,
-                                                           self.compute_intensities_at_sample_times,
-                                                           compute_last_step_only=True)
-
-            # [batch_size, seq_len]
-            dtimes_pred = tf.reduce_sum(accepted_dtimes * weights, axis=-1)
-
-            # [batch_size, seq_len, 1, event_num]
-            intensities_at_times = self.compute_intensities_at_sample_times(time_seqs_,
-                                                                            time_delta_seqs_,
-                                                                            type_seqs_,
-                                                                            dtimes_pred[:, :, None])
-
-            # [batch_size, seq_len, event_num]
-            intensities_at_times = tf.squeeze(intensities_at_times, axis=-2)
-
-            # [batch_size, seq_len]
-            types_pred = tf.argmax(intensities_at_times, axis=-1)
-
-            # [batch_size, 1]
-            types_pred_ = tf.cast(types_pred[:, -1:], tf.int32)
-            dtimes_pred_ = dtimes_pred[:, -1:]
-            time_pred_ = time_seqs_[:, -1:] + dtimes_pred_
-
-            # concat to the prefix sequence
-            time_seqs_ = tf.concat([time_seqs_, time_pred_], axis=-1)
-            time_delta_seqs_ = tf.concat([time_delta_seqs_, dtimes_pred_], axis=-1)
-            type_seqs_ = tf.concat([type_seqs_, types_pred_], axis=-1)
-
-            return [tf.add(i, 1), time_seqs_, time_delta_seqs_, type_seqs_]
-
-        _, _, time_delta_seqs_, type_seqs_ = tf.while_loop(while_condition,
-                                                           body,
-                                                           [i, time_seqs_, time_delta_seqs_, type_seqs_])
-        # to be consistent with the torch version
-        return time_delta_seqs_[:, -num_step - 1:], type_seqs_[:, -num_step - 1:]
+import tensorflow as tf
+
+from easy_tpp.model.tf_model.tf_baselayer import EncoderLayer, TimeShiftedPositionalEncoding
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+from easy_tpp.utils.tf_utils import get_shape_list
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class SAHP(TfBaseModel):
+    """Tensorflow implementation of Self-Attentive Hawkes Process, ICML 2020.
+    https://arxiv.org/abs/1907.07561
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(SAHP, self).__init__(model_config)
+        self.d_model = model_config.hidden_size
+        self.d_time = model_config.time_emb_size
+        self.use_norm = model_config.use_ln
+
+        self.n_layers = model_config.num_layers
+        self.n_head = model_config.num_heads
+        self.dropout = model_config.dropout_rate
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('THP'):
+            self.build_input_graph()
+
+            self.layer_position_emb = TimeShiftedPositionalEncoding(self.hidden_size)
+
+            # Equation (12) - (14)
+            # Equation (12): mu
+            self.mu = tf.get_variable(name='mu',
+                                      shape=[self.d_model, self.num_event_types],
+                                      initializer=tf.keras.initializers.glorot_uniform())
+            # Equation (13): eta
+            self.eta = tf.get_variable(name='eta',
+                                       shape=[self.d_model, self.num_event_types],
+                                       initializer=tf.keras.initializers.glorot_uniform())
+            # Equation (14): gamma
+            self.gamma = tf.get_variable(name='gamma',
+                                         shape=[self.d_model, self.num_event_types],
+                                         initializer=tf.keras.initializers.glorot_uniform())
+
+            self.stack_layers = [EncoderLayer(hidden_size=self.d_model,
+                                              num_heads=self.n_head,
+                                              dropout_rate=self.dropout) for _ in range(self.n_layers)]
+
+            self.loss, self.num_event = self.loglike_loss()
+
+            # Make predictions
+            if self.event_sampler and self.gen_config.num_step_gen == 1:
+                self.dtime_predict_one_step, self.type_predict_one_step = \
+                    self.predict_one_step_at_every_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs)
+
+            if self.event_sampler and self.gen_config.num_step_gen > 1:
+                # make generations
+                self.dtime_generation, self.type_generation = \
+                    self.predict_multi_step_since_last_event(self.time_seqs,
+                                                             self.time_delta_seqs,
+                                                             self.type_seqs,
+                                                             num_step=self.gen_config.num_step_gen)
+
+    def state_decay(self, encode_state, mu, eta, gamma, duration_t):
+        """Equation (15), which computes the pre-intensity states
+
+        Args:
+            encode_state (tensor): [batch_size, seq_len, hidden_size].
+            mu (tensor): [batch_size, seq_len, hidden_size].
+            eta (tensor): [batch_size, seq_len, hidden_size].
+            gamma (tensor): [batch_size, seq_len, hidden_size].
+            duration_t (tensor): [batch_size, seq_len, num_sample].
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+
+        # [batch_size, hidden_dim]
+        # i did not use the exp operation here because it can easily explode!
+        states = tf.matmul(encode_state, mu) + (tf.matmul(encode_state, eta) - tf.matmul(encode_state, mu)) * tf.matmul(
+            encode_state, gamma) * duration_t
+
+        return states
+
+    def forward(self, time_seqs, time_delta_seqs, event_seqs, attention_mask):
+        """Call the model
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            event_seqs (tensor): [batch_size, seq_len], event type seqs.
+            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+        type_embedding = self.layer_type_emb(event_seqs)
+        position_embedding = self.layer_position_emb((time_seqs, time_delta_seqs))
+
+        enc_output = type_embedding + position_embedding
+
+        for enc_layer in self.stack_layers:
+            enc_output = enc_layer(
+                (enc_output,
+                 attention_mask))
+
+        # [batch_size, seq_len, hidden_dim]
+        return enc_output
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Returns:
+            tuple: loglike loss and num of events.
+        """
+        # 1. compute event-loglik
+        enc_out = self.forward(self.time_seqs[:, 1:],
+                               self.time_delta_seqs[:, 1:],
+                               self.type_seqs[:, :-1],
+                               self.attention_mask[:, 1:, :-1])
+
+        cell_t = self.state_decay(encode_state=enc_out,
+                                  mu=self.mu[None, ...],
+                                  eta=self.eta[None, ...],
+                                  gamma=self.gamma[None, ...],
+                                  duration_t=self.time_delta_seqs[:, 1:, None])
+
+        # [batch_size, seq_len, num_event_types]
+        lambda_at_event = tf.nn.softplus(cell_t)
+
+        # 2. compute non-event-loglik (using MC sampling to compute integral)
+        # 2.1 sample times
+        # [batch_size, seq_len, num_sample]
+        sample_dtimes = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
+
+        # 2.2 compute intensities at sampled times
+        # [batch_size, num_times = max_len - 1, num_sample, event_num]
+        state_t_sample = self.compute_states_at_sample_times(encode_state=enc_out,
+                                                             sample_dtimes=sample_dtimes)
+        lambda_t_sample = tf.nn.softplus(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
+                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=self.type_mask[:, 1:])
+
+        # return enc_inten to compute accuracy
+        loss = - tf.reduce_sum(event_ll - non_event_ll)
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self,
+                                       encode_state,
+                                       sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            encode_state (tensor): three tensors with each shape [batch_size, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: [batch_size, seq_len, num_samples, hidden_size]， hidden state at each sampled time.
+        """
+
+        cell_states = self.state_decay(encode_state[:, :, None, :],
+                                       self.mu[None, None, ...],
+                                       self.eta[None, None, ...],
+                                       self.gamma[None, None, ...],
+                                       sample_dtimes[:, :, :, None])
+
+        return cell_states
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
+        """Compute the intensity at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
+
+        Returns:
+            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
+        """
+        attention_mask = kwargs.get('attention_mask', None)
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        if attention_mask is None:
+            batch_size, seq_len = get_shape_list(time_seqs)
+            attention_mask = tf.ones((seq_len, seq_len))
+            # only keep the strict upper triangular
+            lower_diag_masks = tf.linalg.LinearOperatorLowerTriangular(tf.ones_like(attention_mask)).to_dense()
+            attention_mask = tf.where(tf.equal(lower_diag_masks, 0),
+                                      attention_mask,
+                                      tf.zeros_like(attention_mask))
+            attention_mask = tf.tile(attention_mask[None, ...], (batch_size, 1, 1))
+            attention_mask = tf.cast(attention_mask, tf.int32)
+
+        # [batch_size, seq_len, num_samples]
+        enc_out = self.forward(time_seqs, time_delta_seqs, type_seqs, attention_mask)
+
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
+
+        if compute_last_step_only:
+            lambdas = tf.nn.softplus(encoder_output[:, -1:, :, :])
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = tf.nn.softplus(encoder_output)
+        return lambdas
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_fullynn.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_fullynn.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-import tensorflow as tf
-from tensorflow import keras
-from tensorflow.keras import layers
-
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class CumulHazardFunctionNetwork(keras.Model):
-    """Cumulative Hazard Function Network
-    ref: https://github.com/wassname/torch-neuralpointprocess
-    """
-
-    def __init__(self, model_config):
-        super(CumulHazardFunctionNetwork, self).__init__()
-        self.hidden_size = model_config.hidden_size
-        self.num_mlp_layers = model_config.data_specs['num_mlp_layers']
-        self.num_event_types = model_config.num_event_types
-
-        # transform inter-event time embedding
-        self.layer_dense_1 = layers.Dense(self.hidden_size,
-                                          kernel_constraint=keras.constraints.NonNeg(),
-                                          activation=tf.nn.softplus)
-
-        # concat rnn states and inter-event time embedding
-        self.layer_dense_2 = layers.Dense(self.hidden_size,
-                                          kernel_constraint=keras.constraints.NonNeg(),
-                                          activation=tf.nn.softplus)
-
-        # mlp layers
-        self.module_list = [layers.Dense(self.hidden_size, kernel_constraint=keras.constraints.NonNeg(),
-                                         activation=tf.nn.softplus) for _ in
-                            range(self.num_mlp_layers - 1)]
-
-        self.layer_dense_3 = layers.Dense(self.num_event_types, kernel_constraint=keras.constraints.NonNeg(),
-                                          activation=tf.nn.softplus)
-
-        self.params_eps = 1e-5  # ensure positiveness of parameters
-
-    def call(self, hidden_states, time_delta_seqs):
-        # [batch_size, seq_len, hidden_size]
-        t = self.layer_dense_1(time_delta_seqs[..., None])
-
-        # [batch_size, seq_len, hidden_size]
-        out = self.layer_dense_2(tf.concat([hidden_states, t], axis=-1))
-        for layer in self.module_list:
-            out = layer(out)
-
-        # [batch_size, seq_len, num_event_types]
-        integral_lambda = self.layer_dense_3(out)
-
-        # [batch_size, seq_len]
-        derivative_integral_lambda = tf.gradients(
-            tf.reduce_mean(tf.reduce_sum(integral_lambda, axis=-1)),
-            time_delta_seqs)[0]
-
-        return integral_lambda, derivative_integral_lambda
-
-
-class FullyNN(TfBaseModel):
-    """Tensorflow implementation of
-    Fully Neural Network based Model for General Temporal Point Processes, NeurIPS 2019.
-    https://arxiv.org/abs/1905.09690
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(FullyNN, self).__init__(model_config)
-        self.rnn_type = model_config.rnn_type
-        self.rnn_dict = {'lstm': layers.LSTM,
-                         'rnn': layers.SimpleRNN,
-                         'gru': layers.GRU}
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('FullyRNN'):
-            self.build_input_graph()
-
-            self.layer_intensity = CumulHazardFunctionNetwork(model_config=self.model_config)
-
-            # self.layer_intensity_
-            # we can add a method to do this
-            sub_rnn_class = self.rnn_dict[self.rnn_type.lower()]
-            self.layer_rnn = sub_rnn_class(self.hidden_size,
-                                           return_state=False,
-                                           return_sequences=True,
-                                           activation='tanh')
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.event_sampler and self.gen_config.num_step_gen == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.event_sampler and self.gen_config.num_step_gen > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def forward(self, time_seqs, time_delta_seqs, type_seqs):
-        """Call the model
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-        # [batch_size, seq_len, hidden_size]
-        type_embedding = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size + 1]
-        rnn_input = tf.concat([type_embedding, time_seqs[..., None]], axis=-1)
-
-        # [batch_size, seq_len, hidden_size]
-        # states right after the event
-        hidden_states = self.layer_rnn(rnn_input)
-
-        integral_lambda, derivative_integral_lambda = self.layer_intensity(hidden_states, time_delta_seqs)
-
-        # [batch_size, num_event_types, seq_len]
-        return integral_lambda, derivative_integral_lambda
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-
-        # [batch_size, seq_len, num_event_types]
-        integral_lambda, derivative_integral_lambda = self.forward(self.time_delta_seqs[:, 1:],
-                                                                   self.time_delta_seqs[:, 1:],
-                                                                   self.type_seqs[:, :-1])
-        seq_mask = self.batch_non_pad_mask[:, 1:]
-
-        # [batch_size, seq_len]
-        # A temp fix -> make it positive
-        event_lambdas = tf.maximum(tf.boolean_mask(derivative_integral_lambda, seq_mask), self.eps)
-
-        event_ll = tf.reduce_sum(tf.log(event_lambdas))
-
-        # [batch_size, seq_len]
-        # multiplied by sequence mask
-        non_event_ll = tf.reduce_sum(tf.reduce_sum(integral_lambda, axis=-1) * tf.cast(seq_mask, tf.float32))
-
-        num_events = get_shape_list(event_lambdas)[0]
-
-        loss = - (event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_intensities_at_sample_times(self,
-                                            time_seqs,
-                                            time_delta_seqs,
-                                            type_seqs,
-                                            sample_dtimes,
-                                            **kwargs):
-        """Compute hidden states at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-        _, seq_len, num_samples = get_shape_list(sample_dtimes)
-
-        self.test = sample_dtimes
-
-        # [batch_size, seq_len, hidden_size, num_samples]
-        type_emb = tf.tile(self.layer_type_emb(type_seqs)[..., None], (1, 1, 1, num_samples))
-
-        # [batch_size, seq_len, hidden_size + 1, num_samples]
-        rnn_input = tf.concat([type_emb, sample_dtimes[:, :, None, :]], axis=-2)
-
-        # [batch_size, num_samples， seq_len, hidden_size + 1]
-        rnn_input = tf.transpose(rnn_input, perm=[0, 3, 1, 2])
-
-        # [batch_size * num_samples， seq_len, hidden_size + 1]
-        rnn_input = tf.reshape(rnn_input, (-1, seq_len, self.hidden_size + 1))
-
-        # [batch_size * num_samples, seq_len, hidden_size]
-        # states right after the event
-        hidden_states = self.layer_rnn(rnn_input)
-
-        # [batch_size, num_samples， seq_len, hidden_size]
-        hidden_states = tf.reshape(hidden_states,
-                                   (-1, num_samples, seq_len, self.hidden_size))
-
-        # [batch_size, seq_len, num_sample, hidden_size]
-        hidden_states = tf.transpose(hidden_states, perm=(0, 2, 1, 3))
-
-        # [batch_size, seq_len, num_samples]
-        _, derivative_integral_lambda = self.layer_intensity(hidden_states, sample_dtimes)
-
-        # FIX: need to fix this later
-        # [batch_size, seq_len, num_samples, num_event_types]
-        derivative_integral_lambda = tf.tile(derivative_integral_lambda[..., None],
-                                             [1, 1, 1, self.num_event_types])
-
-        if compute_last_step_only:
-            lambdas = derivative_integral_lambda[:, -1:, :, :]
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = derivative_integral_lambda
-        return lambdas
+import tensorflow as tf
+from tensorflow import keras
+from tensorflow.keras import layers
+
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+from easy_tpp.utils.tf_utils import get_shape_list
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class CumulHazardFunctionNetwork(keras.Model):
+    """Cumulative Hazard Function Network
+    ref: https://github.com/wassname/torch-neuralpointprocess
+    """
+
+    def __init__(self, model_config):
+        super(CumulHazardFunctionNetwork, self).__init__()
+        self.hidden_size = model_config.hidden_size
+        self.num_mlp_layers = model_config.data_specs['num_mlp_layers']
+        self.num_event_types = model_config.num_event_types
+
+        # transform inter-event time embedding
+        self.layer_dense_1 = layers.Dense(self.hidden_size,
+                                          kernel_constraint=keras.constraints.NonNeg(),
+                                          activation=tf.nn.softplus)
+
+        # concat rnn states and inter-event time embedding
+        self.layer_dense_2 = layers.Dense(self.hidden_size,
+                                          kernel_constraint=keras.constraints.NonNeg(),
+                                          activation=tf.nn.softplus)
+
+        # mlp layers
+        self.module_list = [layers.Dense(self.hidden_size, kernel_constraint=keras.constraints.NonNeg(),
+                                         activation=tf.nn.softplus) for _ in
+                            range(self.num_mlp_layers - 1)]
+
+        self.layer_dense_3 = layers.Dense(self.num_event_types, kernel_constraint=keras.constraints.NonNeg(),
+                                          activation=tf.nn.softplus)
+
+        self.params_eps = 1e-5  # ensure positiveness of parameters
+
+    def call(self, hidden_states, time_delta_seqs):
+        # [batch_size, seq_len, hidden_size]
+        t = self.layer_dense_1(time_delta_seqs[..., None])
+
+        # [batch_size, seq_len, hidden_size]
+        out = self.layer_dense_2(tf.concat([hidden_states, t], axis=-1))
+        for layer in self.module_list:
+            out = layer(out)
+
+        # [batch_size, seq_len, num_event_types]
+        integral_lambda = self.layer_dense_3(out)
+
+        # [batch_size, seq_len]
+        derivative_integral_lambda = tf.gradients(
+            tf.reduce_mean(tf.reduce_sum(integral_lambda, axis=-1)),
+            time_delta_seqs)[0]
+
+        return integral_lambda, derivative_integral_lambda
+
+
+class FullyNN(TfBaseModel):
+    """Tensorflow implementation of
+    Fully Neural Network based Model for General Temporal Point Processes, NeurIPS 2019.
+    https://arxiv.org/abs/1905.09690
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(FullyNN, self).__init__(model_config)
+        self.rnn_type = model_config.rnn_type
+        self.rnn_dict = {'lstm': layers.LSTM,
+                         'rnn': layers.SimpleRNN,
+                         'gru': layers.GRU}
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('FullyRNN'):
+            self.build_input_graph()
+
+            self.layer_intensity = CumulHazardFunctionNetwork(model_config=self.model_config)
+
+            # self.layer_intensity_
+            # we can add a method to do this
+            sub_rnn_class = self.rnn_dict[self.rnn_type.lower()]
+            self.layer_rnn = sub_rnn_class(self.hidden_size,
+                                           return_state=False,
+                                           return_sequences=True,
+                                           activation='tanh')
+
+            self.loss, self.num_event = self.loglike_loss()
+
+            # Make predictions
+            if self.event_sampler and self.gen_config.num_step_gen == 1:
+                self.dtime_predict_one_step, self.type_predict_one_step = \
+                    self.predict_one_step_at_every_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs)
+
+            if self.event_sampler and self.gen_config.num_step_gen > 1:
+                # make generations
+                self.dtime_generation, self.type_generation = \
+                    self.predict_multi_step_since_last_event(self.time_seqs,
+                                                             self.time_delta_seqs,
+                                                             self.type_seqs,
+                                                             num_step=self.gen_config.num_step_gen)
+
+    def forward(self, time_seqs, time_delta_seqs, type_seqs):
+        """Call the model
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+        # [batch_size, seq_len, hidden_size]
+        type_embedding = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size + 1]
+        rnn_input = tf.concat([type_embedding, time_seqs[..., None]], axis=-1)
+
+        # [batch_size, seq_len, hidden_size]
+        # states right after the event
+        hidden_states = self.layer_rnn(rnn_input)
+
+        integral_lambda, derivative_integral_lambda = self.layer_intensity(hidden_states, time_delta_seqs)
+
+        # [batch_size, num_event_types, seq_len]
+        return integral_lambda, derivative_integral_lambda
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+
+        # [batch_size, seq_len, num_event_types]
+        integral_lambda, derivative_integral_lambda = self.forward(self.time_delta_seqs[:, 1:],
+                                                                   self.time_delta_seqs[:, 1:],
+                                                                   self.type_seqs[:, :-1])
+        seq_mask = self.batch_non_pad_mask[:, 1:]
+
+        # [batch_size, seq_len]
+        # A temp fix -> make it positive
+        event_lambdas = tf.maximum(tf.boolean_mask(derivative_integral_lambda, seq_mask), self.eps)
+
+        event_ll = tf.reduce_sum(tf.log(event_lambdas))
+
+        # [batch_size, seq_len]
+        # multiplied by sequence mask
+        non_event_ll = tf.reduce_sum(tf.reduce_sum(integral_lambda, axis=-1) * tf.cast(seq_mask, tf.float32))
+
+        num_events = get_shape_list(event_lambdas)[0]
+
+        loss = - (event_ll - non_event_ll)
+
+        return loss, num_events
+
+    def compute_intensities_at_sample_times(self,
+                                            time_seqs,
+                                            time_delta_seqs,
+                                            type_seqs,
+                                            sample_dtimes,
+                                            **kwargs):
+        """Compute hidden states at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+        _, seq_len, num_samples = get_shape_list(sample_dtimes)
+
+        self.test = sample_dtimes
+
+        # [batch_size, seq_len, hidden_size, num_samples]
+        type_emb = tf.tile(self.layer_type_emb(type_seqs)[..., None], (1, 1, 1, num_samples))
+
+        # [batch_size, seq_len, hidden_size + 1, num_samples]
+        rnn_input = tf.concat([type_emb, sample_dtimes[:, :, None, :]], axis=-2)
+
+        # [batch_size, num_samples， seq_len, hidden_size + 1]
+        rnn_input = tf.transpose(rnn_input, perm=[0, 3, 1, 2])
+
+        # [batch_size * num_samples， seq_len, hidden_size + 1]
+        rnn_input = tf.reshape(rnn_input, (-1, seq_len, self.hidden_size + 1))
+
+        # [batch_size * num_samples, seq_len, hidden_size]
+        # states right after the event
+        hidden_states = self.layer_rnn(rnn_input)
+
+        # [batch_size, num_samples， seq_len, hidden_size]
+        hidden_states = tf.reshape(hidden_states,
+                                   (-1, num_samples, seq_len, self.hidden_size))
+
+        # [batch_size, seq_len, num_sample, hidden_size]
+        hidden_states = tf.transpose(hidden_states, perm=(0, 2, 1, 3))
+
+        # [batch_size, seq_len, num_samples]
+        _, derivative_integral_lambda = self.layer_intensity(hidden_states, sample_dtimes)
+
+        # FIX: need to fix this later
+        # [batch_size, seq_len, num_samples, num_event_types]
+        derivative_integral_lambda = tf.tile(derivative_integral_lambda[..., None],
+                                             [1, 1, 1, self.num_event_types])
+
+        if compute_last_step_only:
+            lambdas = derivative_integral_lambda[:, -1:, :, :]
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = derivative_integral_lambda
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_intensity_free.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_intensity_free.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-import tensorflow as tf
-import tensorflow_probability as tfp
-from tensorflow.keras import layers
-
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils.tf_utils import get_shape_list
-
-tfd = tfp.distributions
-tfb = tfp.bijectors
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class MixtureSameFamily(tfd.MixtureSameFamily):
-    """Mixture (same-family) distribution, redefined `log_cdf` and `log_survival_function`.
-    """
-
-    def log_cdf(self, x):
-        x = x[..., None]
-        log_cdf_x = self.components_distribution.log_cdf(x)
-        mix_logits = self.mixture_distribution.logits
-        return tf.reduce_logsumexp(log_cdf_x + mix_logits, axis=-1)
-
-    def log_survival_function(self, x):
-        x = x[..., None]
-        log_sf_x = self.components_distribution.log_survival_function(x)
-        mix_logits = self.mixture_distribution.logits
-        return tf.reduce_logsumexp(log_sf_x + mix_logits, axis=-1)
-
-
-class LogNormalMixtureDistribution:
-    """
-    Mixture of log-normal distributions.
-
-    Args:
-        locs (tensor): [batch_size, seq_len, num_mix_components].
-        log_scales (tensor): [batch_size, seq_len, num_mix_components].
-        log_weights (tensor): [batch_size, seq_len, num_mix_components].
-        mean_log_inter_time (float): Average log-inter-event-time.
-        std_log_inter_time (float): Std of log-inter-event-times.
-    """
-
-    def __init__(self, locs, log_scales, log_weights, mean_log_inter_time, std_log_inter_time, validate_args=None):
-        mixture_dist = tfd.Categorical(logits=log_weights)
-        component_dist = tfd.Normal(loc=locs, scale=tf.exp(log_scales))
-        self.GMM = MixtureSameFamily(mixture_dist, component_dist)
-        self.mean_log_inter_time = mean_log_inter_time
-        self.std_log_inter_time = std_log_inter_time
-
-        self.transformed_distribution = tfd.TransformedDistribution(self.GMM,
-                                                                    bijector=tfb.Exp(),
-                                                                    validate_args=validate_args)
-
-    def log_prob(self, x):
-        return self.transformed_distribution.log_prob(x)
-
-    def log_survival_function(self, x):
-        return self.transformed_distribution.log_survival_function(x)
-
-
-class IntensityFree(TfBaseModel):
-    """Tensorflow implementation of Intensity-Free Learning of Temporal Point Processes, ICLR 2020.
-    https://openreview.net/pdf?id=HygOjhEYDH
-
-    reference: https://github.com/shchur/ifl-tpp
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(IntensityFree, self).__init__(model_config)
-
-        self.num_mix_components = model_config.data_specs['num_mix_components']
-        self.num_features = 1 + self.hidden_size
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('IntensityFree'):
-            self.build_input_graph()
-
-            self.layer_rnn = layers.GRU(self.hidden_size,
-                                        return_state=False,
-                                        return_sequences=True)
-            # activation='tanh')
-
-            self.context_init = tf.zeros(self.hidden_size)[None, None, :]
-            self.mark_linear = layers.Dense(self.num_event_types_pad)
-            self.linear = layers.Dense(3 * self.num_mix_components)
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.event_sampler and self.gen_config.num_step_gen == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.event_sampler and self.gen_config.num_step_gen > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def forward(self, time_delta_seqs, type_seqs):
-        """Call the model.
-
-        Args:
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-
-        Returns:
-            tensor: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens.
-        """
-        # [batch_size, seq_len, 1]
-        temporal_seqs = tf.log(time_delta_seqs + self.eps)[..., None]
-
-        # [batch_size, seq_len, hidden_size]
-        type_emb = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size + 1]
-        features = tf.concat([temporal_seqs, type_emb], axis=-1)
-
-        # [batch_size, seq_len, hidden_size]
-        context = self.layer_rnn(features)
-
-        batch_size, seq_len, hidden_size = get_shape_list(context)
-
-        # (batch_size, 1, hidden_size)
-        context_init = tf.tile(self.context_init, [batch_size, 1, 1])
-
-        # (batch_size, seq_len + 1, hidden_size)
-        context = tf.concat([context_init, context], axis=1)
-
-        return context
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Returns:
-            tuple: loglikelihood loss and num of events.
-
-        """
-
-        time_delta_seqs = self.time_delta_seqs
-        type_seqs = self.type_seqs
-        batch_non_pad_mask = self.batch_non_pad_mask
-
-        mean_log_inter_time = tf.reduce_mean(tf.log(time_delta_seqs))
-        std_log_inter_time = tf.math.reduce_std(tf.log(time_delta_seqs))
-
-        # [batch_size, seq_len, hidden_size]
-        # seq_len = time_delta_seqs[:, 1:].size()[1]
-        context = self.forward(time_delta_seqs[:, 1:], type_seqs[:, :-1])
-
-        # (batch_size, seq_len, 3 * num_mix_components)
-        raw_params = self.linear(context)
-        locs = raw_params[..., :self.num_mix_components]
-        log_scales = raw_params[..., self.num_mix_components: (2 * self.num_mix_components)]
-        log_weights = raw_params[..., (2 * self.num_mix_components):]
-
-        log_weights = tf.nn.log_softmax(log_weights, dim=-1)
-        inter_time_dist = LogNormalMixtureDistribution(
-            locs=locs,
-            log_scales=log_scales,
-            log_weights=log_weights,
-            mean_log_inter_time=mean_log_inter_time,
-            std_log_inter_time=std_log_inter_time
-        )
-
-        inter_times = tf.clip_by_value(time_delta_seqs, 1e-10, 1e10)
-        # (batch_size, seq_len)
-        log_p = inter_time_dist.log_prob(inter_times)
-
-        # (batch_size, 1)
-        # last_event_idx = tf.cast(tf.reduce_sum(batch_non_pad_mask, axis=-1, keepdims=True),
-        #                          tf.int32) - 1
-
-        log_surv_all = inter_time_dist.log_survival_function(inter_times)
-
-        self.inter_times = log_surv_all
-
-        #
-        # # (batch_size,)
-        # log_surv_last = tf.gather(log_surv_all, axis=-1, indices=last_event_idx)[..., None]
-
-        # (batch_size, seq_len, num_marks)
-        mark_logits = tf.nn.log_softmax(self.mark_linear(context), dim=-1)
-        mark_dist = tfd.Categorical(logits=mark_logits)
-        log_p += mark_dist.log_prob(type_seqs)
-
-        # (batch_size, seq_len)
-        log_p = tf.boolean_mask(log_p, batch_non_pad_mask) + self.eps
-        # (batch_size,)
-        loss = -tf.reduce_sum(log_p)
-
-        num_events = get_shape_list(log_p)[0]
-
-        return loss, num_events
+import tensorflow as tf
+import tensorflow_probability as tfp
+from tensorflow.keras import layers
+
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+from easy_tpp.utils.tf_utils import get_shape_list
+
+tfd = tfp.distributions
+tfb = tfp.bijectors
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class MixtureSameFamily(tfd.MixtureSameFamily):
+    """Mixture (same-family) distribution, redefined `log_cdf` and `log_survival_function`.
+    """
+
+    def log_cdf(self, x):
+        x = x[..., None]
+        log_cdf_x = self.components_distribution.log_cdf(x)
+        mix_logits = self.mixture_distribution.logits
+        return tf.reduce_logsumexp(log_cdf_x + mix_logits, axis=-1)
+
+    def log_survival_function(self, x):
+        x = x[..., None]
+        log_sf_x = self.components_distribution.log_survival_function(x)
+        mix_logits = self.mixture_distribution.logits
+        return tf.reduce_logsumexp(log_sf_x + mix_logits, axis=-1)
+
+
+class LogNormalMixtureDistribution:
+    """
+    Mixture of log-normal distributions.
+
+    Args:
+        locs (tensor): [batch_size, seq_len, num_mix_components].
+        log_scales (tensor): [batch_size, seq_len, num_mix_components].
+        log_weights (tensor): [batch_size, seq_len, num_mix_components].
+        mean_log_inter_time (float): Average log-inter-event-time.
+        std_log_inter_time (float): Std of log-inter-event-times.
+    """
+
+    def __init__(self, locs, log_scales, log_weights, mean_log_inter_time, std_log_inter_time, validate_args=None):
+        mixture_dist = tfd.Categorical(logits=log_weights)
+        component_dist = tfd.Normal(loc=locs, scale=tf.exp(log_scales))
+        self.GMM = MixtureSameFamily(mixture_dist, component_dist)
+        self.mean_log_inter_time = mean_log_inter_time
+        self.std_log_inter_time = std_log_inter_time
+
+        self.transformed_distribution = tfd.TransformedDistribution(self.GMM,
+                                                                    bijector=tfb.Exp(),
+                                                                    validate_args=validate_args)
+
+    def log_prob(self, x):
+        return self.transformed_distribution.log_prob(x)
+
+    def log_survival_function(self, x):
+        return self.transformed_distribution.log_survival_function(x)
+
+
+class IntensityFree(TfBaseModel):
+    """Tensorflow implementation of Intensity-Free Learning of Temporal Point Processes, ICLR 2020.
+    https://openreview.net/pdf?id=HygOjhEYDH
+
+    reference: https://github.com/shchur/ifl-tpp
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(IntensityFree, self).__init__(model_config)
+
+        self.num_mix_components = model_config.data_specs['num_mix_components']
+        self.num_features = 1 + self.hidden_size
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('IntensityFree'):
+            self.build_input_graph()
+
+            self.layer_rnn = layers.GRU(self.hidden_size,
+                                        return_state=False,
+                                        return_sequences=True)
+            # activation='tanh')
+
+            self.context_init = tf.zeros(self.hidden_size)[None, None, :]
+            self.mark_linear = layers.Dense(self.num_event_types_pad)
+            self.linear = layers.Dense(3 * self.num_mix_components)
+
+            self.loss, self.num_event = self.loglike_loss()
+
+            # Make predictions
+            if self.event_sampler and self.gen_config.num_step_gen == 1:
+                self.dtime_predict_one_step, self.type_predict_one_step = \
+                    self.predict_one_step_at_every_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs)
+
+            if self.event_sampler and self.gen_config.num_step_gen > 1:
+                # make generations
+                self.dtime_generation, self.type_generation = \
+                    self.predict_multi_step_since_last_event(self.time_seqs,
+                                                             self.time_delta_seqs,
+                                                             self.type_seqs,
+                                                             num_step=self.gen_config.num_step_gen)
+
+    def forward(self, time_delta_seqs, type_seqs):
+        """Call the model.
+
+        Args:
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+
+        Returns:
+            tensor: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens.
+        """
+        # [batch_size, seq_len, 1]
+        temporal_seqs = tf.log(time_delta_seqs + self.eps)[..., None]
+
+        # [batch_size, seq_len, hidden_size]
+        type_emb = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size + 1]
+        features = tf.concat([temporal_seqs, type_emb], axis=-1)
+
+        # [batch_size, seq_len, hidden_size]
+        context = self.layer_rnn(features)
+
+        batch_size, seq_len, hidden_size = get_shape_list(context)
+
+        # (batch_size, 1, hidden_size)
+        context_init = tf.tile(self.context_init, [batch_size, 1, 1])
+
+        # (batch_size, seq_len + 1, hidden_size)
+        context = tf.concat([context_init, context], axis=1)
+
+        return context
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Returns:
+            tuple: loglikelihood loss and num of events.
+
+        """
+
+        time_delta_seqs = self.time_delta_seqs
+        type_seqs = self.type_seqs
+        batch_non_pad_mask = self.batch_non_pad_mask
+
+        mean_log_inter_time = tf.reduce_mean(tf.log(time_delta_seqs))
+        std_log_inter_time = tf.math.reduce_std(tf.log(time_delta_seqs))
+
+        # [batch_size, seq_len, hidden_size]
+        # seq_len = time_delta_seqs[:, 1:].size()[1]
+        context = self.forward(time_delta_seqs[:, 1:], type_seqs[:, :-1])
+
+        # (batch_size, seq_len, 3 * num_mix_components)
+        raw_params = self.linear(context)
+        locs = raw_params[..., :self.num_mix_components]
+        log_scales = raw_params[..., self.num_mix_components: (2 * self.num_mix_components)]
+        log_weights = raw_params[..., (2 * self.num_mix_components):]
+
+        log_weights = tf.nn.log_softmax(log_weights, dim=-1)
+        inter_time_dist = LogNormalMixtureDistribution(
+            locs=locs,
+            log_scales=log_scales,
+            log_weights=log_weights,
+            mean_log_inter_time=mean_log_inter_time,
+            std_log_inter_time=std_log_inter_time
+        )
+
+        inter_times = tf.clip_by_value(time_delta_seqs, 1e-10, 1e10)
+        # (batch_size, seq_len)
+        log_p = inter_time_dist.log_prob(inter_times)
+
+        # (batch_size, 1)
+        # last_event_idx = tf.cast(tf.reduce_sum(batch_non_pad_mask, axis=-1, keepdims=True),
+        #                          tf.int32) - 1
+
+        log_surv_all = inter_time_dist.log_survival_function(inter_times)
+
+        self.inter_times = log_surv_all
+
+        #
+        # # (batch_size,)
+        # log_surv_last = tf.gather(log_surv_all, axis=-1, indices=last_event_idx)[..., None]
+
+        # (batch_size, seq_len, num_marks)
+        mark_logits = tf.nn.log_softmax(self.mark_linear(context), dim=-1)
+        mark_dist = tfd.Categorical(logits=mark_logits)
+        log_p += mark_dist.log_prob(type_seqs)
+
+        # (batch_size, seq_len)
+        log_p = tf.boolean_mask(log_p, batch_non_pad_mask) + self.eps
+        # (batch_size,)
+        loss = -tf.reduce_sum(log_p)
+
+        num_events = get_shape_list(log_p)[0]
+
+        return loss, num_events
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_nhp.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_nhp.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,335 +1,335 @@
-import tensorflow as tf
-from tensorflow import keras
-from tensorflow.keras import layers
-
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class ContTimeLSTMCell(keras.Model):
-    """LSTM Cell in Neural Hawkes Process.
-    """
-
-    def __init__(self, hidden_size):
-        """Initialize the continuous LSTM Cell
-
-        Args:
-            hidden_size (int): size of hidden states.
-        """
-        super(ContTimeLSTMCell, self).__init__()
-
-        with tf.variable_scope('ContTimeLSTMCell'):
-            self.hidden_size = hidden_size
-            self.init_dense_layer()
-
-    def init_dense_layer(self):
-        """Initialize related dense layers.
-        """
-        self.layer_input = layers.Dense(self.hidden_size,
-                                        activation=tf.nn.sigmoid,
-                                        name='layer_input')
-        self.layer_forget = layers.Dense(self.hidden_size,
-                                         activation=tf.nn.sigmoid,
-                                         name='layer_forget')
-        self.layer_output = layers.Dense(self.hidden_size,
-                                         activation=tf.nn.sigmoid,
-                                         name='layer_output')
-        self.layer_input_bar = layers.Dense(self.hidden_size,
-                                            activation=tf.nn.sigmoid,
-                                            name='layer_input_bar')
-        self.layer_forget_bar = layers.Dense(self.hidden_size,
-                                             activation=tf.nn.sigmoid,
-                                             name='layer_forget_bar')
-
-        self.layer_pre_c = layers.Dense(self.hidden_size,
-                                        activation=tf.nn.tanh,
-                                        name='layer_z')
-        self.layer_decay = layers.Dense(self.hidden_size,
-                                        activation=tf.nn.softplus,
-                                        name='layer_decay')
-
-    def init_state(self, batch_size):
-        """Initialize hidden and cell states with zeros.
-
-        Args:
-            batch_size (tensor): size of the batch.
-
-        Returns:
-            tuple: rnn state, a tuple of three tensors and decay states, a tuple of four tensors.
-        """
-        zero_dims = tf.stack([batch_size, self.hidden_size])
-        rnn_state = (tf.fill(zero_dims, 0.0),
-                     tf.fill(zero_dims, 0.0),
-                     tf.fill(zero_dims, 0.0))
-        decay_state = (tf.fill(zero_dims, 0.0),
-                       tf.fill(zero_dims, 0.0),
-                       tf.fill(zero_dims, 0.0),
-                       tf.fill(zero_dims, 0.0))
-        return rnn_state, decay_state
-
-    def call(self, x_t, dtime_t, initial_state):
-        """Update the continuous time LSTM cell.
-
-        Args:
-            x_t (tensor): [batch_size, hidden_size]
-            dtime_t (tensor): [batch_size, 1]
-            initial_state (tuple): states initialized in function init_state.
-
-        Returns:
-            tuple: updated hidden state and tuple of rnn and decay states.
-        """
-        # parameter process
-        h_t, c_func_t, c_bar_t = initial_state[0]
-        input_t = tf.concat([x_t, h_t], axis=-1)
-
-        # update input gate - Equation (5a)
-        gate_input = self.layer_input(input_t)
-
-        # update forget gate - Equation (5b)
-        gate_forget = self.layer_forget(input_t)
-
-        # update output gate - Equation (5d)
-        gate_output = self.layer_output(input_t)
-
-        # update input bar - similar to Equation (5a)
-        gate_input_bar = self.layer_input_bar(input_t)
-
-        # update forget bar - similar to Equation (5b)
-        gate_forget_bar = self.layer_forget_bar(input_t)
-
-        # update gate decay - Equation (6c)
-        gate_decay = self.layer_decay(input_t)
-
-        # update gate z - Equation (5c)
-        z_t = self.layer_pre_c(input_t)
-
-        # update cell state to t_i+ - Equation (6a)
-        c_t = gate_forget * c_func_t + gate_input * z_t
-
-        # update cell state bar - Equation (6b)
-        c_bar_t = gate_forget_bar * c_bar_t + gate_input_bar * z_t
-
-        c_func_t, h_t = ContTimeLSTMCell.decay(c_t, c_bar_t, gate_decay, gate_output, dtime_t)
-
-        rnn_state = (h_t, c_func_t, c_bar_t)
-        decay_state = (c_t, c_bar_t, gate_decay, gate_output)
-        return h_t, (rnn_state, decay_state)
-
-    @staticmethod
-    def decay(cell_i, cell_bar_i, gate_decay, gate_output, dtime):
-        """Cell and hidden state decay - Equation (7)
-
-        Args:
-            cell_i (tensor): cell state, [batch_size, hidden_size].
-            cell_bar_i (tensor): cell bar state, [batch_size, hidden_size].
-            gate_decay (tensor): decay state, [batch_size, hidden_size].
-            gate_output (tensor): output state, [batch_size, hidden_size].
-            dtime (tensor): delta time, , [batch_size, 1].
-
-        Returns:
-            tuple: cell state and hidden state.
-        """
-        c_t = cell_bar_i + (cell_i - cell_bar_i) * tf.math.exp(-gate_decay * dtime)
-        h_t = gate_output * tf.tanh(c_t)
-        return c_t, h_t
-
-    def dynamic_run(self, seq_type_embed, dtime):
-        """Update the continuous time LSTM for all time steps.
-
-        Args:
-            seq_type_embed (tensor): [batch_size, seq_len, hidden_size].
-            dtime (tensor): [batch_size, seq_len].
-
-        Returns:
-            tuple: hidden state, [batch_size, seq_len, hidden_size] and decay state,
-            [batch_size, 4, seq_len, hidden_size].
-        """
-
-        def move_forward_fn(accumulator, item):
-            init_state = accumulator[1]
-            x_t = item[0]
-            dtime_t = item[1]
-            h_t, init_state = self.call(x_t, dtime_t, initial_state=init_state)
-            return h_t, init_state
-
-        initial_state = self.init_state(tf.shape(seq_type_embed)[0])
-        initial_h_t = initial_state[0][0]
-
-        # Scan(move forward) along times axis
-        h_ts, cell_states = tf.scan(move_forward_fn,
-                                    (tf.transpose(seq_type_embed, perm=[1, 0, 2]),
-                                     tf.transpose(tf.expand_dims(dtime, -1), perm=[1, 0, 2])),
-                                    initializer=(initial_h_t, initial_state))
-
-        # Transpose the tensor so that batch_size is in the first dimension
-        h_ts = tf.transpose(h_ts, perm=[1, 0, 2])
-        decay_states = tf.stack(cell_states[1])
-        decay_states = tf.transpose(decay_states, perm=[2, 1, 0, 3])
-
-        return h_ts, decay_states
-
-
-class NHP(TfBaseModel):
-
-    def __init__(self,
-                 model_config):
-        """Initialize the model
-
-        Args:
-            model_config (dict): config of model specs.
-        """
-        super(NHP, self).__init__(model_config)
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('NHP'):
-            self.build_input_graph()
-
-            # Initialize the rnn cell
-            self.rnn_cell = ContTimeLSTMCell(self.hidden_size)
-
-            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
-
-        # Compute the loss
-        self.loss, self.num_event = self.loglike_loss()
-
-        # Make predictions
-        if self.event_sampler and self.gen_config.num_step_gen == 1:
-            self.dtime_predict_one_step, self.type_predict_one_step = \
-                self.predict_one_step_at_every_event(self.time_seqs,
-                                                     self.time_delta_seqs,
-                                                     self.type_seqs)
-
-        if self.event_sampler and self.gen_config.num_step_gen > 1:
-            # make generations
-            self.dtime_generation, self.type_generation = \
-                self.predict_multi_step_since_last_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs,
-                                                         num_step=self.gen_config.num_step_gen)
-
-    def forward(self, dtimes_seq, event_seq, len_seq=None):
-        """ Move forward through the network """
-
-        # shape - (batch_size, seq_len, hidden_size)
-        types_seq_emb = self.layer_type_emb(event_seq)
-
-        h_ts, decay_states = self.rnn_cell.dynamic_run(types_seq_emb,
-                                                       dtimes_seq)
-
-        if len_seq is not None:
-            # Get last decay state for every seq
-            # Find out the index position of last decay states for each sequence
-            ind_shape = tf.shape(len_seq)
-            ndind = tf.concat([tf.range(ind_shape[0])[:, None], len_seq], axis=-1)
-
-            # shape  (batch_size, 4, hidden_size)
-            last_decay_states = tf.gather_nd(decay_states, ndind)
-        else:
-            last_decay_states = decay_states[:, -1, :, :]
-
-        # h_ts   (batch_size, seq_len, event_num)
-        # decay_states (batch_size, seq_len, 4, hidden_size)
-        # last_decay_states (batch_size, 4, hidden_size)
-        return h_ts, decay_states, last_decay_states
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Returns:
-            tuple: loglike loss and num of events.
-        """
-        hiddens_ti, decay_states, _ = self.forward(self.time_delta_seqs[:, 1:], self.type_seqs[:, :-1])
-
-        # Lambda(t) right before each event time point
-        # lambda_at_event - [batch_size, seq_len = max_len-1, num_event_types]
-        # Here we drop the last event because it has no delta_time label (can not decay)
-        lambda_at_event = self.layer_intensity(hiddens_ti)
-
-        # interval_t_sample - [batch_size, seq_len = max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seq[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # [batch_size, seq_len = max_len - 1, num_mc_sample]
-        state_t_sample = self.compute_states_at_sampled_times(decay_states, interval_t_sample)
-
-        # [batch_size, seq_len = max_len - 1, num_mc_sample, event_num]
-        lambda_t_sample = self.layer_intensity(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        # (num_samples, num_times)
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_states_at_sampled_times(self, decay_states, sample_dtimes, compute_last_step_only=False):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            decay_states (tensor): [batch_size, 4, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-            compute_last_step_only (bool, optional): whether to compute the last step only. Defaults to False.
-
-        Returns:
-            tensor: hidden state at each sampled time.
-        """
-
-        # update the states given last event
-        # cells (batch_size, num_times, hidden_dim)
-        cells, cell_bars, decays, outputs = tf.unstack(decay_states, 4, axis=-2)
-
-        if compute_last_step_only:
-            _, h_ts = self.rnn_cell.decay(cells[:, -1:, None, :],
-                                          cell_bars[:, -1:, None, :],
-                                          decays[:, -1:, None, :],
-                                          outputs[:, -1:, None, :],
-                                          sample_dtimes[:, -1:, :, None])
-
-        else:
-            # Use broadcasting to compute the decays at all time steps
-            # at all sample points
-            # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
-            # cells[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
-            _, h_ts = self.rnn_cell.decay(cells[:, :, None, :],
-                                          cell_bars[:, :, None, :],
-                                          decays[:, :, None, :],
-                                          outputs[:, :, None, :],
-                                          sample_dtimes[..., None])
-
-        return h_ts
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sampled_dtimes,
-                                            **kwargs):
-        """Compute the intensity at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
-            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
-            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
-            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
-
-        Returns:
-            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        hiddens_ti, decay_states, _ = self.forward(time_delta_seqs, type_seqs)
-
-        # [batch_size, seq_len, num_mc_sample, hidden_dim]
-        state_t_sample = self.compute_states_at_sampled_times(decay_states, sampled_dtimes, compute_last_step_only)
-
-        # [batch_size, seq_len, num_samples, event_num]
-        lambdas = self.layer_intensity(state_t_sample)
-
-        return lambdas
+import tensorflow as tf
+from tensorflow import keras
+from tensorflow.keras import layers
+
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class ContTimeLSTMCell(keras.Model):
+    """LSTM Cell in Neural Hawkes Process.
+    """
+
+    def __init__(self, hidden_size):
+        """Initialize the continuous LSTM Cell
+
+        Args:
+            hidden_size (int): size of hidden states.
+        """
+        super(ContTimeLSTMCell, self).__init__()
+
+        with tf.variable_scope('ContTimeLSTMCell'):
+            self.hidden_size = hidden_size
+            self.init_dense_layer()
+
+    def init_dense_layer(self):
+        """Initialize related dense layers.
+        """
+        self.layer_input = layers.Dense(self.hidden_size,
+                                        activation=tf.nn.sigmoid,
+                                        name='layer_input')
+        self.layer_forget = layers.Dense(self.hidden_size,
+                                         activation=tf.nn.sigmoid,
+                                         name='layer_forget')
+        self.layer_output = layers.Dense(self.hidden_size,
+                                         activation=tf.nn.sigmoid,
+                                         name='layer_output')
+        self.layer_input_bar = layers.Dense(self.hidden_size,
+                                            activation=tf.nn.sigmoid,
+                                            name='layer_input_bar')
+        self.layer_forget_bar = layers.Dense(self.hidden_size,
+                                             activation=tf.nn.sigmoid,
+                                             name='layer_forget_bar')
+
+        self.layer_pre_c = layers.Dense(self.hidden_size,
+                                        activation=tf.nn.tanh,
+                                        name='layer_z')
+        self.layer_decay = layers.Dense(self.hidden_size,
+                                        activation=tf.nn.softplus,
+                                        name='layer_decay')
+
+    def init_state(self, batch_size):
+        """Initialize hidden and cell states with zeros.
+
+        Args:
+            batch_size (tensor): size of the batch.
+
+        Returns:
+            tuple: rnn state, a tuple of three tensors and decay states, a tuple of four tensors.
+        """
+        zero_dims = tf.stack([batch_size, self.hidden_size])
+        rnn_state = (tf.fill(zero_dims, 0.0),
+                     tf.fill(zero_dims, 0.0),
+                     tf.fill(zero_dims, 0.0))
+        decay_state = (tf.fill(zero_dims, 0.0),
+                       tf.fill(zero_dims, 0.0),
+                       tf.fill(zero_dims, 0.0),
+                       tf.fill(zero_dims, 0.0))
+        return rnn_state, decay_state
+
+    def call(self, x_t, dtime_t, initial_state):
+        """Update the continuous time LSTM cell.
+
+        Args:
+            x_t (tensor): [batch_size, hidden_size]
+            dtime_t (tensor): [batch_size, 1]
+            initial_state (tuple): states initialized in function init_state.
+
+        Returns:
+            tuple: updated hidden state and tuple of rnn and decay states.
+        """
+        # parameter process
+        h_t, c_func_t, c_bar_t = initial_state[0]
+        input_t = tf.concat([x_t, h_t], axis=-1)
+
+        # update input gate - Equation (5a)
+        gate_input = self.layer_input(input_t)
+
+        # update forget gate - Equation (5b)
+        gate_forget = self.layer_forget(input_t)
+
+        # update output gate - Equation (5d)
+        gate_output = self.layer_output(input_t)
+
+        # update input bar - similar to Equation (5a)
+        gate_input_bar = self.layer_input_bar(input_t)
+
+        # update forget bar - similar to Equation (5b)
+        gate_forget_bar = self.layer_forget_bar(input_t)
+
+        # update gate decay - Equation (6c)
+        gate_decay = self.layer_decay(input_t)
+
+        # update gate z - Equation (5c)
+        z_t = self.layer_pre_c(input_t)
+
+        # update cell state to t_i+ - Equation (6a)
+        c_t = gate_forget * c_func_t + gate_input * z_t
+
+        # update cell state bar - Equation (6b)
+        c_bar_t = gate_forget_bar * c_bar_t + gate_input_bar * z_t
+
+        c_func_t, h_t = ContTimeLSTMCell.decay(c_t, c_bar_t, gate_decay, gate_output, dtime_t)
+
+        rnn_state = (h_t, c_func_t, c_bar_t)
+        decay_state = (c_t, c_bar_t, gate_decay, gate_output)
+        return h_t, (rnn_state, decay_state)
+
+    @staticmethod
+    def decay(cell_i, cell_bar_i, gate_decay, gate_output, dtime):
+        """Cell and hidden state decay - Equation (7)
+
+        Args:
+            cell_i (tensor): cell state, [batch_size, hidden_size].
+            cell_bar_i (tensor): cell bar state, [batch_size, hidden_size].
+            gate_decay (tensor): decay state, [batch_size, hidden_size].
+            gate_output (tensor): output state, [batch_size, hidden_size].
+            dtime (tensor): delta time, , [batch_size, 1].
+
+        Returns:
+            tuple: cell state and hidden state.
+        """
+        c_t = cell_bar_i + (cell_i - cell_bar_i) * tf.math.exp(-gate_decay * dtime)
+        h_t = gate_output * tf.tanh(c_t)
+        return c_t, h_t
+
+    def dynamic_run(self, seq_type_embed, dtime):
+        """Update the continuous time LSTM for all time steps.
+
+        Args:
+            seq_type_embed (tensor): [batch_size, seq_len, hidden_size].
+            dtime (tensor): [batch_size, seq_len].
+
+        Returns:
+            tuple: hidden state, [batch_size, seq_len, hidden_size] and decay state,
+            [batch_size, 4, seq_len, hidden_size].
+        """
+
+        def move_forward_fn(accumulator, item):
+            init_state = accumulator[1]
+            x_t = item[0]
+            dtime_t = item[1]
+            h_t, init_state = self.call(x_t, dtime_t, initial_state=init_state)
+            return h_t, init_state
+
+        initial_state = self.init_state(tf.shape(seq_type_embed)[0])
+        initial_h_t = initial_state[0][0]
+
+        # Scan(move forward) along times axis
+        h_ts, cell_states = tf.scan(move_forward_fn,
+                                    (tf.transpose(seq_type_embed, perm=[1, 0, 2]),
+                                     tf.transpose(tf.expand_dims(dtime, -1), perm=[1, 0, 2])),
+                                    initializer=(initial_h_t, initial_state))
+
+        # Transpose the tensor so that batch_size is in the first dimension
+        h_ts = tf.transpose(h_ts, perm=[1, 0, 2])
+        decay_states = tf.stack(cell_states[1])
+        decay_states = tf.transpose(decay_states, perm=[2, 1, 0, 3])
+
+        return h_ts, decay_states
+
+
+class NHP(TfBaseModel):
+
+    def __init__(self,
+                 model_config):
+        """Initialize the model
+
+        Args:
+            model_config (dict): config of model specs.
+        """
+        super(NHP, self).__init__(model_config)
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('NHP'):
+            self.build_input_graph()
+
+            # Initialize the rnn cell
+            self.rnn_cell = ContTimeLSTMCell(self.hidden_size)
+
+            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
+
+        # Compute the loss
+        self.loss, self.num_event = self.loglike_loss()
+
+        # Make predictions
+        if self.event_sampler and self.gen_config.num_step_gen == 1:
+            self.dtime_predict_one_step, self.type_predict_one_step = \
+                self.predict_one_step_at_every_event(self.time_seqs,
+                                                     self.time_delta_seqs,
+                                                     self.type_seqs)
+
+        if self.event_sampler and self.gen_config.num_step_gen > 1:
+            # make generations
+            self.dtime_generation, self.type_generation = \
+                self.predict_multi_step_since_last_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs,
+                                                         num_step=self.gen_config.num_step_gen)
+
+    def forward(self, dtimes_seq, event_seq, len_seq=None):
+        """ Move forward through the network """
+
+        # shape - (batch_size, seq_len, hidden_size)
+        types_seq_emb = self.layer_type_emb(event_seq)
+
+        h_ts, decay_states = self.rnn_cell.dynamic_run(types_seq_emb,
+                                                       dtimes_seq)
+
+        if len_seq is not None:
+            # Get last decay state for every seq
+            # Find out the index position of last decay states for each sequence
+            ind_shape = tf.shape(len_seq)
+            ndind = tf.concat([tf.range(ind_shape[0])[:, None], len_seq], axis=-1)
+
+            # shape  (batch_size, 4, hidden_size)
+            last_decay_states = tf.gather_nd(decay_states, ndind)
+        else:
+            last_decay_states = decay_states[:, -1, :, :]
+
+        # h_ts   (batch_size, seq_len, event_num)
+        # decay_states (batch_size, seq_len, 4, hidden_size)
+        # last_decay_states (batch_size, 4, hidden_size)
+        return h_ts, decay_states, last_decay_states
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Returns:
+            tuple: loglike loss and num of events.
+        """
+        hiddens_ti, decay_states, _ = self.forward(self.time_delta_seqs[:, 1:], self.type_seqs[:, :-1])
+
+        # Lambda(t) right before each event time point
+        # lambda_at_event - [batch_size, seq_len = max_len-1, num_event_types]
+        # Here we drop the last event because it has no delta_time label (can not decay)
+        lambda_at_event = self.layer_intensity(hiddens_ti)
+
+        # interval_t_sample - [batch_size, seq_len = max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seq[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
+
+        # [batch_size, seq_len = max_len - 1, num_mc_sample]
+        state_t_sample = self.compute_states_at_sampled_times(decay_states, interval_t_sample)
+
+        # [batch_size, seq_len = max_len - 1, num_mc_sample, event_num]
+        lambda_t_sample = self.layer_intensity(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
+                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=self.type_mask[:, 1:])
+
+        # (num_samples, num_times)
+        loss = - tf.reduce_sum(event_ll - non_event_ll)
+
+        return loss, num_events
+
+    def compute_states_at_sampled_times(self, decay_states, sample_dtimes, compute_last_step_only=False):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            decay_states (tensor): [batch_size, 4, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+            compute_last_step_only (bool, optional): whether to compute the last step only. Defaults to False.
+
+        Returns:
+            tensor: hidden state at each sampled time.
+        """
+
+        # update the states given last event
+        # cells (batch_size, num_times, hidden_dim)
+        cells, cell_bars, decays, outputs = tf.unstack(decay_states, 4, axis=-2)
+
+        if compute_last_step_only:
+            _, h_ts = self.rnn_cell.decay(cells[:, -1:, None, :],
+                                          cell_bars[:, -1:, None, :],
+                                          decays[:, -1:, None, :],
+                                          outputs[:, -1:, None, :],
+                                          sample_dtimes[:, -1:, :, None])
+
+        else:
+            # Use broadcasting to compute the decays at all time steps
+            # at all sample points
+            # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
+            # cells[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
+            _, h_ts = self.rnn_cell.decay(cells[:, :, None, :],
+                                          cell_bars[:, :, None, :],
+                                          decays[:, :, None, :],
+                                          outputs[:, :, None, :],
+                                          sample_dtimes[..., None])
+
+        return h_ts
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sampled_dtimes,
+                                            **kwargs):
+        """Compute the intensity at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
+
+        Returns:
+            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        hiddens_ti, decay_states, _ = self.forward(time_delta_seqs, type_seqs)
+
+        # [batch_size, seq_len, num_mc_sample, hidden_dim]
+        state_t_sample = self.compute_states_at_sampled_times(decay_states, sampled_dtimes, compute_last_step_only)
+
+        # [batch_size, seq_len, num_samples, event_num]
+        lambdas = self.layer_intensity(state_t_sample)
+
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_ode_tpp.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_ode_tpp.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-import numpy as np
-import tensorflow as tf
-from tensorflow.keras import layers
-
-from easy_tpp.model.tf_model.tf_baselayer import DNN
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils import rk4_step_method
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-def get_neural_ode_layer(
-        ode_fn,
-        num_samples=10,
-        solver=rk4_step_method,
-        return_states=False
-):
-    """Get a black-box neural ode layer parameterized by parameters.
-
-    Args:
-        ode_fn: function
-            It likes f(solver_function, dt, z_list), and contains the learnable variables.
-        num_samples: int
-            Number of samples in time interval dt.
-        solver: function
-            Solver function like f(ode_func, dt, z_0)
-        return_states: bool, default False
-            Identify whether return whole states or just last state.
-
-    Returns:
-        A neural_ode_layer (function) with signature f(z0, dt).
-    """
-
-    @tf.custom_gradient
-    def neural_ode_layer(
-            z0,
-            dt,
-    ):
-        """Calculate z1 by z0 and time gap dt.
-
-        Args:
-            z0: Tensor with shape [..., dim]
-            dt: Tensor with shape [..., 1 or dim]
-
-        Returns:
-            A tensor presents z1, whose shape is the same as z0.
-        """
-        with tf.name_scope('neural_ode'):
-            # Forward activity
-            dt_ratio = 1.0 / num_samples
-            delta_t = dt * dt_ratio
-
-            z = z0
-            z_list = []
-            for i in range(num_samples):
-                z = solver(ode_fn, delta_t, z)
-                z_list.append(z)
-            z1 = z
-
-            def grad(a1, variables=None):
-                # a1 is grad_z1 == dL/dz1
-                if variables is None:
-                    variables = []
-
-                def aug_dynamics(tmp_states):
-                    """
-                    Ode function for states [z_1, a_1, \thetas (many)].
-
-                    Args:
-                        tmp_states: list
-                            Elements are [z_1, a_1, \thetas (many)].
-
-                    Returns:
-                        List contains differentiations of states.
-                    """
-
-                    tmp_z = tmp_states[0]
-                    tmp_neg_a = -tmp_states[1]
-                    # tmp_var_grad = tmp_states[2:]
-
-                    # calculate dz/dt
-
-                    # if tf.__version__ < '2.0':
-                    #     # using GradientType to calculate (faster when building graph)
-                    #     with tf.GradientTape() as g:
-                    #         g.watch([tmp_z, *variables])
-                    #         func_eval = ode_fn(tmp_z)
-                    #         tmp_ds = g.gradient(func_eval, [tmp_z, *variables], output_gradients=tmp_neg_a)
-                    # else:
-                    # using tf.gradients to calculate
-                    func_eval = ode_fn(tmp_z)
-                    tmp_ds = tf.gradients(func_eval, [tmp_z, *variables], grad_ys=tmp_neg_a)
-
-                    neg_adfdz = tmp_ds[0]
-                    neg_adfdtheta = [tf.reshape(var, [-1]) for var in tmp_ds[1:]]
-
-                    return [func_eval, neg_adfdz, *neg_adfdtheta]
-
-                # Backward activity
-                if tf.__version__ < '2.0':
-                    # Compile EAGER graph to static (this will be much faster)
-                    import tensorflow.contrib.eager as tfe
-                    aug_dynamics = tfe.defun(aug_dynamics)
-
-                # Construct back-state for ode solver
-                # reshape variable \theta for batch solving
-                init_var_grad = [tf.zeros([np.prod(get_shape_list(var))]) for var in variables]
-
-                if a1 is None:
-                    a1 = tf.zeros_like(z1)
-
-                # [z(t_1), a(t_1), \theta]
-                states = [z1, a1, *init_var_grad]
-                # print('states:', states)
-                for i in range(num_samples):
-                    states = solver(aug_dynamics, -delta_t, states)
-
-                grad_z0 = states[1]
-                grad_t = tf.ones_like(dt)
-
-                if variables is not None:
-                    # average the different dt effect on variable \theta
-                    grad_theta = [tf.reshape(tf.reduce_mean(var_grad, axis=0), var.shape) for var, var_grad in
-                                  zip(variables, states[2:])]
-                    return (grad_z0, grad_t), grad_theta
-                else:
-                    return grad_z0, grad_t
-
-        if return_states:
-            return z_list, grad
-        else:
-            return z1, grad
-
-    return neural_ode_layer
-
-
-class ODETPP(TfBaseModel):
-    """
-    TODO: this version runs ok under tf 1.13, but is very slow under tf 2.0
-    """
-    def __init__(self, model_config):
-        super(ODETPP, self).__init__(model_config)
-        self.ode_num_sample_per_step = model_config.model_specs['ode_num_sample_per_step']
-        self.time_factor = model_config.model_specs['time_factor']
-        self.seq_len = model_config.max_len
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('ODETPP'):
-            # have to specify the max len of the input to avoid a variable length of tensor.
-            # for looping over the variable length of tensor, custom gradient can not properly work
-            # in the scan (while_loop)
-            # tf.GradientTape.gradients() does not support graph control flow operations
-            # like tf.cond or tf.while at this time
-
-            # Input placeholder
-            # shape - (batch_size, max_len)
-            # max_len - sequence length including time zero padding
-            self.time_delta_seqs = tf.placeholder(tf.float32, shape=[None, self.seq_len])
-
-            # shape - (batch_size, max_len)
-            self.time_seqs = tf.placeholder(tf.float32, shape=[None, self.seq_len])
-
-            # shape - (batch_size, max_len)
-            self.type_seqs = tf.placeholder(tf.int32, shape=[None, self.seq_len])
-
-            # shape - (batch_size, max_len)
-            self.batch_non_pad_mask = tf.placeholder(tf.int32, shape=[None, self.seq_len])
-
-            # shape - (batch_size, max_len, max_len)
-            self.attention_mask = tf.placeholder(tf.int32, shape=[None, None, None])
-
-            # Event type one-hot code
-            # shape - (batch_size, max_len, num_event_types)
-            self.type_mask = tf.placeholder(tf.float32, shape=[None, None, None])
-
-            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
-
-            self.event_model = DNN(hidden_size=self.hidden_size)
-
-            self.solver = rk4_step_method
-
-            self.layer_neural_ode = get_neural_ode_layer(ode_fn=self.event_model,
-                                                         solver=self.solver,
-                                                         num_samples=self.ode_num_sample_per_step)
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            self.is_training = tf.placeholder(tf.bool)
-
-            # Make predictions
-            if self.event_sampler and self.gen_config.num_step_gen == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.event_sampler and self.gen_config.num_step_gen > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def forward(self, time_delta_seqs, type_seqs, **kwargs):
-        """Call the model.
-
-        Args:
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-
-        Returns:
-            tensor: hidden states at event times.
-
-        """
-        # [batch_size, seq_len=max_len, hidden_size]
-        type_seq_emb = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len=max_len, 1]
-        time_delta_seqs_ = time_delta_seqs[..., None]
-
-        total_state_at_event_minus = []
-        total_state_at_event_plus = []
-        last_state = tf.zeros_like(type_seq_emb[:, 0, :])
-        for type_emb, dt in zip(tf.unstack(type_seq_emb, axis=-2),
-                                tf.unstack(time_delta_seqs_, axis=-2)):
-            # the bp may break for tf 1.13 when dt is large
-            # after testing, we put a time factor here to avoid the failure of bp
-            # it is not needed for tf 2.0.
-            dt = dt / self.time_factor
-            last_state = self.layer_neural_ode(last_state + type_emb, dt)
-            total_state_at_event_minus.append(last_state)
-            total_state_at_event_plus.append(last_state + type_emb)
-
-        # [batch_size, seq_len, hidden_size]
-        state_ti = tf.stack(total_state_at_event_minus, axis=1)
-
-        # [batch_size, seq_len, hidden_size]
-        state_to_evolve = tf.stack(total_state_at_event_plus, axis=1)
-
-        return state_ti, state_to_evolve
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-
-        state_ti, state_ti_plus = self.forward(self.time_delta_seqs[:, 1:], self.type_seqs[:, :-1])
-
-        # Lambda(t) right before each event time point
-        # lambda_at_event - [batch_size, num_times=max_len-1, num_event_types]
-        # Here we drop the last event because it has no delta_time label (can not decay)
-        lambda_at_event = self.layer_intensity(state_ti)
-
-        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seq[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample, hidden_size]
-        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, interval_t_sample)
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample, event_num]
-        lambda_t_sample = self.layer_intensity(sample_state_ti)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self, state_ti_plus, sample_dtimes):
-        """Compute the states at sampling times.
-
-        Args:
-            state_ti_plus (tensor): [batch_size, seq_len, hidden_size], states right after the events.
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples], delta times in sampling.
-
-        Returns:
-            tensor: hiddens states at sampling times.
-        """
-
-        # Use broadcasting to compute the decays at all time steps
-        # at all sample points
-        # h_ts shape (batch_size, seq_len, num_samples, hidden_dim)
-        state = self.solver(diff_func=self.event_model,
-                            dt=sample_dtimes[..., None],  # [batch_size, seq_len, num_samples, 1]
-                            z0=state_ti_plus[..., None, :])  # [batch_size, seq_len, 1, hidden_size]
-
-        return state
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
-        """Compute the intensity at sampled times, not only event times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
-                    intensity at each timestamp for each event type.
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        state_ti, state_ti_plus = self.forward(time_delta_seqs, type_seqs, **kwargs)
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = get_shape_list(state_ti)
-
-        if compute_last_step_only:
-            interval_t_sample = sample_dtimes[:, -1:, :]
-        else:
-            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
-            interval_t_sample = sample_dtimes
-            # Use broadcasting to compute the decays at all time steps
-            # at all sample points
-
-        # [batch_size, num_sample_times / 1, num_mc_sample, hidden_size]
-        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, interval_t_sample)
-
-        # [batch_size, num_sample_times / 1, num_mc_sample, num_event_types]
-        sampled_intensities = self.layer_intensity(sample_state_ti)
-
-        return sampled_intensities
+import numpy as np
+import tensorflow as tf
+from tensorflow.keras import layers
+
+from easy_tpp.model.tf_model.tf_baselayer import DNN
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+from easy_tpp.utils import rk4_step_method
+from easy_tpp.utils.tf_utils import get_shape_list
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+def get_neural_ode_layer(
+        ode_fn,
+        num_samples=10,
+        solver=rk4_step_method,
+        return_states=False
+):
+    """Get a black-box neural ode layer parameterized by parameters.
+
+    Args:
+        ode_fn: function
+            It likes f(solver_function, dt, z_list), and contains the learnable variables.
+        num_samples: int
+            Number of samples in time interval dt.
+        solver: function
+            Solver function like f(ode_func, dt, z_0)
+        return_states: bool, default False
+            Identify whether return whole states or just last state.
+
+    Returns:
+        A neural_ode_layer (function) with signature f(z0, dt).
+    """
+
+    @tf.custom_gradient
+    def neural_ode_layer(
+            z0,
+            dt,
+    ):
+        """Calculate z1 by z0 and time gap dt.
+
+        Args:
+            z0: Tensor with shape [..., dim]
+            dt: Tensor with shape [..., 1 or dim]
+
+        Returns:
+            A tensor presents z1, whose shape is the same as z0.
+        """
+        with tf.name_scope('neural_ode'):
+            # Forward activity
+            dt_ratio = 1.0 / num_samples
+            delta_t = dt * dt_ratio
+
+            z = z0
+            z_list = []
+            for i in range(num_samples):
+                z = solver(ode_fn, delta_t, z)
+                z_list.append(z)
+            z1 = z
+
+            def grad(a1, variables=None):
+                # a1 is grad_z1 == dL/dz1
+                if variables is None:
+                    variables = []
+
+                def aug_dynamics(tmp_states):
+                    """
+                    Ode function for states [z_1, a_1, \thetas (many)].
+
+                    Args:
+                        tmp_states: list
+                            Elements are [z_1, a_1, \thetas (many)].
+
+                    Returns:
+                        List contains differentiations of states.
+                    """
+
+                    tmp_z = tmp_states[0]
+                    tmp_neg_a = -tmp_states[1]
+                    # tmp_var_grad = tmp_states[2:]
+
+                    # calculate dz/dt
+
+                    # if tf.__version__ < '2.0':
+                    #     # using GradientType to calculate (faster when building graph)
+                    #     with tf.GradientTape() as g:
+                    #         g.watch([tmp_z, *variables])
+                    #         func_eval = ode_fn(tmp_z)
+                    #         tmp_ds = g.gradient(func_eval, [tmp_z, *variables], output_gradients=tmp_neg_a)
+                    # else:
+                    # using tf.gradients to calculate
+                    func_eval = ode_fn(tmp_z)
+                    tmp_ds = tf.gradients(func_eval, [tmp_z, *variables], grad_ys=tmp_neg_a)
+
+                    neg_adfdz = tmp_ds[0]
+                    neg_adfdtheta = [tf.reshape(var, [-1]) for var in tmp_ds[1:]]
+
+                    return [func_eval, neg_adfdz, *neg_adfdtheta]
+
+                # Backward activity
+                if tf.__version__ < '2.0':
+                    # Compile EAGER graph to static (this will be much faster)
+                    import tensorflow.contrib.eager as tfe
+                    aug_dynamics = tfe.defun(aug_dynamics)
+
+                # Construct back-state for ode solver
+                # reshape variable \theta for batch solving
+                init_var_grad = [tf.zeros([np.prod(get_shape_list(var))]) for var in variables]
+
+                if a1 is None:
+                    a1 = tf.zeros_like(z1)
+
+                # [z(t_1), a(t_1), \theta]
+                states = [z1, a1, *init_var_grad]
+                # print('states:', states)
+                for i in range(num_samples):
+                    states = solver(aug_dynamics, -delta_t, states)
+
+                grad_z0 = states[1]
+                grad_t = tf.ones_like(dt)
+
+                if variables is not None:
+                    # average the different dt effect on variable \theta
+                    grad_theta = [tf.reshape(tf.reduce_mean(var_grad, axis=0), var.shape) for var, var_grad in
+                                  zip(variables, states[2:])]
+                    return (grad_z0, grad_t), grad_theta
+                else:
+                    return grad_z0, grad_t
+
+        if return_states:
+            return z_list, grad
+        else:
+            return z1, grad
+
+    return neural_ode_layer
+
+
+class ODETPP(TfBaseModel):
+    """
+    TODO: this version runs ok under tf 1.13, but is very slow under tf 2.0
+    """
+    def __init__(self, model_config):
+        super(ODETPP, self).__init__(model_config)
+        self.ode_num_sample_per_step = model_config.model_specs['ode_num_sample_per_step']
+        self.time_factor = model_config.model_specs['time_factor']
+        self.seq_len = model_config.max_len
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('ODETPP'):
+            # have to specify the max len of the input to avoid a variable length of tensor.
+            # for looping over the variable length of tensor, custom gradient can not properly work
+            # in the scan (while_loop)
+            # tf.GradientTape.gradients() does not support graph control flow operations
+            # like tf.cond or tf.while at this time
+
+            # Input placeholder
+            # shape - (batch_size, max_len)
+            # max_len - sequence length including time zero padding
+            self.time_delta_seqs = tf.placeholder(tf.float32, shape=[None, self.seq_len])
+
+            # shape - (batch_size, max_len)
+            self.time_seqs = tf.placeholder(tf.float32, shape=[None, self.seq_len])
+
+            # shape - (batch_size, max_len)
+            self.type_seqs = tf.placeholder(tf.int32, shape=[None, self.seq_len])
+
+            # shape - (batch_size, max_len)
+            self.batch_non_pad_mask = tf.placeholder(tf.int32, shape=[None, self.seq_len])
+
+            # shape - (batch_size, max_len, max_len)
+            self.attention_mask = tf.placeholder(tf.int32, shape=[None, None, None])
+
+            # Event type one-hot code
+            # shape - (batch_size, max_len, num_event_types)
+            self.type_mask = tf.placeholder(tf.float32, shape=[None, None, None])
+
+            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
+
+            self.event_model = DNN(hidden_size=self.hidden_size)
+
+            self.solver = rk4_step_method
+
+            self.layer_neural_ode = get_neural_ode_layer(ode_fn=self.event_model,
+                                                         solver=self.solver,
+                                                         num_samples=self.ode_num_sample_per_step)
+
+            self.loss, self.num_event = self.loglike_loss()
+
+            self.is_training = tf.placeholder(tf.bool)
+
+            # Make predictions
+            if self.event_sampler and self.gen_config.num_step_gen == 1:
+                self.dtime_predict_one_step, self.type_predict_one_step = \
+                    self.predict_one_step_at_every_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs)
+
+            if self.event_sampler and self.gen_config.num_step_gen > 1:
+                # make generations
+                self.dtime_generation, self.type_generation = \
+                    self.predict_multi_step_since_last_event(self.time_seqs,
+                                                             self.time_delta_seqs,
+                                                             self.type_seqs,
+                                                             num_step=self.gen_config.num_step_gen)
+
+    def forward(self, time_delta_seqs, type_seqs, **kwargs):
+        """Call the model.
+
+        Args:
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+
+        Returns:
+            tensor: hidden states at event times.
+
+        """
+        # [batch_size, seq_len=max_len, hidden_size]
+        type_seq_emb = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len=max_len, 1]
+        time_delta_seqs_ = time_delta_seqs[..., None]
+
+        total_state_at_event_minus = []
+        total_state_at_event_plus = []
+        last_state = tf.zeros_like(type_seq_emb[:, 0, :])
+        for type_emb, dt in zip(tf.unstack(type_seq_emb, axis=-2),
+                                tf.unstack(time_delta_seqs_, axis=-2)):
+            # the bp may break for tf 1.13 when dt is large
+            # after testing, we put a time factor here to avoid the failure of bp
+            # it is not needed for tf 2.0.
+            dt = dt / self.time_factor
+            last_state = self.layer_neural_ode(last_state + type_emb, dt)
+            total_state_at_event_minus.append(last_state)
+            total_state_at_event_plus.append(last_state + type_emb)
+
+        # [batch_size, seq_len, hidden_size]
+        state_ti = tf.stack(total_state_at_event_minus, axis=1)
+
+        # [batch_size, seq_len, hidden_size]
+        state_to_evolve = tf.stack(total_state_at_event_plus, axis=1)
+
+        return state_ti, state_to_evolve
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+
+        state_ti, state_ti_plus = self.forward(self.time_delta_seqs[:, 1:], self.type_seqs[:, :-1])
+
+        # Lambda(t) right before each event time point
+        # lambda_at_event - [batch_size, num_times=max_len-1, num_event_types]
+        # Here we drop the last event because it has no delta_time label (can not decay)
+        lambda_at_event = self.layer_intensity(state_ti)
+
+        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seq[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample, hidden_size]
+        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, interval_t_sample)
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample, event_num]
+        lambda_t_sample = self.layer_intensity(sample_state_ti)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
+                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=self.type_mask[:, 1:])
+
+        loss = - tf.reduce_sum(event_ll - non_event_ll)
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, state_ti_plus, sample_dtimes):
+        """Compute the states at sampling times.
+
+        Args:
+            state_ti_plus (tensor): [batch_size, seq_len, hidden_size], states right after the events.
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples], delta times in sampling.
+
+        Returns:
+            tensor: hiddens states at sampling times.
+        """
+
+        # Use broadcasting to compute the decays at all time steps
+        # at all sample points
+        # h_ts shape (batch_size, seq_len, num_samples, hidden_dim)
+        state = self.solver(diff_func=self.event_model,
+                            dt=sample_dtimes[..., None],  # [batch_size, seq_len, num_samples, 1]
+                            z0=state_ti_plus[..., None, :])  # [batch_size, seq_len, 1, hidden_size]
+
+        return state
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
+        """Compute the intensity at sampled times, not only event times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
+                    intensity at each timestamp for each event type.
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        state_ti, state_ti_plus = self.forward(time_delta_seqs, type_seqs, **kwargs)
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = get_shape_list(state_ti)
+
+        if compute_last_step_only:
+            interval_t_sample = sample_dtimes[:, -1:, :]
+        else:
+            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
+            interval_t_sample = sample_dtimes
+            # Use broadcasting to compute the decays at all time steps
+            # at all sample points
+
+        # [batch_size, num_sample_times / 1, num_mc_sample, hidden_size]
+        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, interval_t_sample)
+
+        # [batch_size, num_sample_times / 1, num_mc_sample, num_event_types]
+        sampled_intensities = self.layer_intensity(sample_state_ti)
+
+        return sampled_intensities
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_rmtpp.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_rmtpp.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import tensorflow as tf
-from tensorflow.keras import layers
-
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class RMTPP(TfBaseModel):
-    """Tensorflow implementation of Recurrent Marked Temporal Point Process, KDD 2016.
-    https://www.kdd.org/kdd2016/papers/files/rpp1081-duA.pdf
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (dict): config of model specs.
-        """
-        super(RMTPP, self).__init__(model_config)
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('RMTPP'):
-            self.build_input_graph()
-
-            # Initialize the rnn cell
-            self.layer_rnn = layers.SimpleRNN(self.hidden_size,
-                                              return_state=False,
-                                              return_sequences=True)
-
-            self.layer_temporal_emb = layers.Dense(self.hidden_size)
-
-            self.layer_hidden = layers.Dense(self.num_event_types)
-
-            self.factor_intensity_base = tf.get_variable(name='intensity_base',
-                                                         shape=[1, 1, self.num_event_types],
-                                                         initializer=tf.keras.initializers.glorot_uniform())
-            self.factor_intensity_current_influence = tf.get_variable(name='intensity_current_influence',
-                                                                      shape=[1, 1, self.num_event_types],
-                                                                      initializer=tf.keras.initializers.glorot_uniform()
-                                                                      )
-
-            # Compute the loss
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.event_sampler and self.gen_config.num_step_gen == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.event_sampler and self.gen_config.num_step_gen > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def state_decay(self, states_to_decay, duration_t):
-        """Equation (11), which computes the intensity
-        """
-
-        # [batch_size, seq_len, num_event_types]
-        states_to_decay_ = self.layer_hidden(states_to_decay)
-
-        # [batch_size, seq_len, num_event_types]
-        intensity = tf.exp(
-            states_to_decay_ + self.factor_intensity_current_influence * duration_t + self.factor_intensity_base)
-        return intensity
-
-    def forward(self, time_seqs, time_delta_seqs, type_seqs):
-        """Call the model.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-
-        Returns:
-            list: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens;
-                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
-                  the event happens.
-        """
-
-        # [batch_size, seq_len, hidden_size]
-        type_emb = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size]
-        temporal_emb = self.layer_temporal_emb(time_seqs[..., None])
-
-        # [batch_size, seq_len, hidden_size]
-        # states right after the event
-        decay_states = self.layer_rnn(type_emb + temporal_emb)
-
-        # States decay - Equation (7) in the paper
-        # states before the happening of the next event
-        h_t = self.state_decay(decay_states, time_delta_seqs[..., None])
-
-        return h_t, decay_states
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Returns:
-            tuple: loglike loss and num of events.
-        """
-
-        lambda_at_event, decay_states = self.forward(self.time_seqs[:, :-1], self.time_delta_seqs[:, 1:],
-                                                     self.type_seqs[:, :-1])
-
-        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seq[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample]
-        lambda_t_sample = self.compute_states_at_sample_times(decay_states, interval_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        # (num_samples, num_times)
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self, decay_states, sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            decay_states (tensor): [batch_size, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: hidden state at each sampled time.
-        """
-        # update the states given last event
-
-        # Use broadcasting to compute the decays at all time steps
-        # decay_states[..., None, :]: [batch_size, seq_len, 1, hidden_size]
-        # sample_dtimes[..., None]: [batch_size, seq_len, num_mc_sample, 1]
-        # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
-        h_ts = self.state_decay(decay_states[..., None, :],
-                                sample_dtimes[..., None])
-
-        return h_ts
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sampled_dtimes,
-                                            **kwargs):
-        """Compute the intensity at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
-            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
-            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
-            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
-
-        Returns:
-            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        _, decay_states = self.forward(time_seqs, time_delta_seqs, type_seqs)
-
-        if compute_last_step_only:
-            interval_t_sample = sampled_dtimes[:, -1:, :, None]
-            # [batch_size, 1, num_mc_sample, num_event_types]
-            sampled_intensities = self.state_decay(decay_states[:, -1:, None, :],
-                                                   interval_t_sample)
-
-        else:
-            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
-            interval_t_sample = sampled_dtimes[..., None]
-            # Use broadcasting to compute the decays at all time steps
-            # at all sample points
-            # sampled_intensities shape (batch_size, num_times, num_mc_sample, hidden_dim)
-            # decay_states[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
-            sampled_intensities = self.state_decay(decay_states[..., None, :],
-                                                   interval_t_sample)
-
-        return sampled_intensities
+import tensorflow as tf
+from tensorflow.keras import layers
+
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class RMTPP(TfBaseModel):
+    """Tensorflow implementation of Recurrent Marked Temporal Point Process, KDD 2016.
+    https://www.kdd.org/kdd2016/papers/files/rpp1081-duA.pdf
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (dict): config of model specs.
+        """
+        super(RMTPP, self).__init__(model_config)
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('RMTPP'):
+            self.build_input_graph()
+
+            # Initialize the rnn cell
+            self.layer_rnn = layers.SimpleRNN(self.hidden_size,
+                                              return_state=False,
+                                              return_sequences=True)
+
+            self.layer_temporal_emb = layers.Dense(self.hidden_size)
+
+            self.layer_hidden = layers.Dense(self.num_event_types)
+
+            self.factor_intensity_base = tf.get_variable(name='intensity_base',
+                                                         shape=[1, 1, self.num_event_types],
+                                                         initializer=tf.keras.initializers.glorot_uniform())
+            self.factor_intensity_current_influence = tf.get_variable(name='intensity_current_influence',
+                                                                      shape=[1, 1, self.num_event_types],
+                                                                      initializer=tf.keras.initializers.glorot_uniform()
+                                                                      )
+
+            # Compute the loss
+            self.loss, self.num_event = self.loglike_loss()
+
+            # Make predictions
+            if self.event_sampler and self.gen_config.num_step_gen == 1:
+                self.dtime_predict_one_step, self.type_predict_one_step = \
+                    self.predict_one_step_at_every_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs)
+
+            if self.event_sampler and self.gen_config.num_step_gen > 1:
+                # make generations
+                self.dtime_generation, self.type_generation = \
+                    self.predict_multi_step_since_last_event(self.time_seqs,
+                                                             self.time_delta_seqs,
+                                                             self.type_seqs,
+                                                             num_step=self.gen_config.num_step_gen)
+
+    def state_decay(self, states_to_decay, duration_t):
+        """Equation (11), which computes the intensity
+        """
+
+        # [batch_size, seq_len, num_event_types]
+        states_to_decay_ = self.layer_hidden(states_to_decay)
+
+        # [batch_size, seq_len, num_event_types]
+        intensity = tf.exp(
+            states_to_decay_ + self.factor_intensity_current_influence * duration_t + self.factor_intensity_base)
+        return intensity
+
+    def forward(self, time_seqs, time_delta_seqs, type_seqs):
+        """Call the model.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+
+        Returns:
+            list: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens;
+                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
+                  the event happens.
+        """
+
+        # [batch_size, seq_len, hidden_size]
+        type_emb = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size]
+        temporal_emb = self.layer_temporal_emb(time_seqs[..., None])
+
+        # [batch_size, seq_len, hidden_size]
+        # states right after the event
+        decay_states = self.layer_rnn(type_emb + temporal_emb)
+
+        # States decay - Equation (7) in the paper
+        # states before the happening of the next event
+        h_t = self.state_decay(decay_states, time_delta_seqs[..., None])
+
+        return h_t, decay_states
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Returns:
+            tuple: loglike loss and num of events.
+        """
+
+        lambda_at_event, decay_states = self.forward(self.time_seqs[:, :-1], self.time_delta_seqs[:, 1:],
+                                                     self.type_seqs[:, :-1])
+
+        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seq[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample]
+        lambda_t_sample = self.compute_states_at_sample_times(decay_states, interval_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
+                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=self.type_mask[:, 1:])
+
+        # (num_samples, num_times)
+        loss = - tf.reduce_sum(event_ll - non_event_ll)
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, decay_states, sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            decay_states (tensor): [batch_size, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: hidden state at each sampled time.
+        """
+        # update the states given last event
+
+        # Use broadcasting to compute the decays at all time steps
+        # decay_states[..., None, :]: [batch_size, seq_len, 1, hidden_size]
+        # sample_dtimes[..., None]: [batch_size, seq_len, num_mc_sample, 1]
+        # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
+        h_ts = self.state_decay(decay_states[..., None, :],
+                                sample_dtimes[..., None])
+
+        return h_ts
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sampled_dtimes,
+                                            **kwargs):
+        """Compute the intensity at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
+
+        Returns:
+            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        _, decay_states = self.forward(time_seqs, time_delta_seqs, type_seqs)
+
+        if compute_last_step_only:
+            interval_t_sample = sampled_dtimes[:, -1:, :, None]
+            # [batch_size, 1, num_mc_sample, num_event_types]
+            sampled_intensities = self.state_decay(decay_states[:, -1:, None, :],
+                                                   interval_t_sample)
+
+        else:
+            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
+            interval_t_sample = sampled_dtimes[..., None]
+            # Use broadcasting to compute the decays at all time steps
+            # at all sample points
+            # sampled_intensities shape (batch_size, num_times, num_mc_sample, hidden_dim)
+            # decay_states[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
+            sampled_intensities = self.state_decay(decay_states[..., None, :],
+                                                   interval_t_sample)
+
+        return sampled_intensities
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_sahp.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_sahp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,222 +1,212 @@
-import tensorflow as tf
-
-from easy_tpp.model.tf_model.tf_baselayer import EncoderLayer, TimeShiftedPositionalEncoding
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class SAHP(TfBaseModel):
-    """Tensorflow implementation of Self-Attentive Hawkes Process, ICML 2020.
-    https://arxiv.org/abs/1907.07561
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(SAHP, self).__init__(model_config)
-        self.d_model = model_config.hidden_size
-        self.d_time = model_config.time_emb_size
-        self.use_norm = model_config.use_ln
-
-        self.n_layers = model_config.num_layers
-        self.n_head = model_config.num_heads
-        self.dropout = model_config.dropout_rate
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('THP'):
-            self.build_input_graph()
-
-            self.layer_position_emb = TimeShiftedPositionalEncoding(self.hidden_size)
-
-            # Equation (12) - (14)
-            # Equation (12): mu
-            self.mu = tf.get_variable(name='mu',
-                                      shape=[self.d_model, self.num_event_types],
-                                      initializer=tf.keras.initializers.glorot_uniform())
-            # Equation (13): eta
-            self.eta = tf.get_variable(name='eta',
-                                       shape=[self.d_model, self.num_event_types],
-                                       initializer=tf.keras.initializers.glorot_uniform())
-            # Equation (14): gamma
-            self.gamma = tf.get_variable(name='gamma',
-                                         shape=[self.d_model, self.num_event_types],
-                                         initializer=tf.keras.initializers.glorot_uniform())
-
-            self.stack_layers = [EncoderLayer(hidden_size=self.d_model,
-                                              num_heads=self.n_head,
-                                              dropout_rate=self.dropout) for _ in range(self.n_layers)]
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.event_sampler and self.gen_config.num_step_gen == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.event_sampler and self.gen_config.num_step_gen > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def state_decay(self, encode_state, mu, eta, gamma, duration_t):
-        """Equation (15), which computes the pre-intensity states
-
-        Args:
-            encode_state (tensor): [batch_size, seq_len, hidden_size].
-            mu (tensor): [batch_size, seq_len, hidden_size].
-            eta (tensor): [batch_size, seq_len, hidden_size].
-            gamma (tensor): [batch_size, seq_len, hidden_size].
-            duration_t (tensor): [batch_size, seq_len, num_sample].
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-
-        # [batch_size, hidden_dim]
-        # i did not use the exp operation here because it can easily explode!
-        states = tf.matmul(encode_state, mu) + (tf.matmul(encode_state, eta) - tf.matmul(encode_state, mu)) * tf.matmul(
-            encode_state, gamma) * duration_t
-
-        return states
-
-    def forward(self, time_seqs, time_delta_seqs, event_seqs, attention_mask):
-        """Call the model
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            event_seqs (tensor): [batch_size, seq_len], event type seqs.
-            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-        type_embedding = self.layer_type_emb(event_seqs)
-        position_embedding = self.layer_position_emb((time_seqs, time_delta_seqs))
-
-        enc_output = type_embedding + position_embedding
-
-        for enc_layer in self.stack_layers:
-            enc_output = enc_layer(
-                (enc_output,
-                 attention_mask))
-
-        # [batch_size, seq_len, hidden_dim]
-        return enc_output
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Returns:
-            tuple: loglike loss and num of events.
-        """
-        # 1. compute event-loglik
-        enc_out = self.forward(self.time_seqs[:, 1:],
-                               self.time_delta_seqs[:, 1:],
-                               self.type_seqs[:, :-1],
-                               self.attention_mask[:, 1:, :-1])
-
-        cell_t = self.state_decay(encode_state=enc_out,
-                                  mu=self.mu[None, ...],
-                                  eta=self.eta[None, ...],
-                                  gamma=self.gamma[None, ...],
-                                  duration_t=self.time_delta_seqs[:, 1:, None])
-
-        # [batch_size, seq_len, num_event_types]
-        lambda_at_event = tf.nn.softplus(cell_t)
-
-        # 2. compute non-event-loglik (using MC sampling to compute integral)
-        # 2.1 sample times
-        # [batch_size, seq_len, num_sample]
-        sample_dtimes = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # 2.2 compute intensities at sampled times
-        # [batch_size, num_times = max_len - 1, num_sample, event_num]
-        state_t_sample = self.compute_states_at_sample_times(encode_state=enc_out,
-                                                             sample_dtimes=sample_dtimes)
-        lambda_t_sample = tf.nn.softplus(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        # return enc_inten to compute accuracy
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self,
-                                       encode_state,
-                                       sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            encode_state (tensor): three tensors with each shape [batch_size, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: [batch_size, seq_len, num_samples, hidden_size]， hidden state at each sampled time.
-        """
-
-        cell_states = self.state_decay(encode_state[:, :, None, :],
-                                       self.mu[None, None, ...],
-                                       self.eta[None, None, ...],
-                                       self.gamma[None, None, ...],
-                                       sample_dtimes[:, :, :, None])
-
-        return cell_states
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
-        """Compute the intensity at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
-            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
-            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
-            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
-
-        Returns:
-            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
-        """
-        attention_mask = kwargs.get('attention_mask', None)
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        if attention_mask is None:
-            batch_size, seq_len = get_shape_list(time_seqs)
-            attention_mask = tf.ones((seq_len, seq_len))
-            # only keep the strict upper triangular
-            lower_diag_masks = tf.linalg.LinearOperatorLowerTriangular(tf.ones_like(attention_mask)).to_dense()
-            attention_mask = tf.where(tf.equal(lower_diag_masks, 0),
-                                      attention_mask,
-                                      tf.zeros_like(attention_mask))
-            attention_mask = tf.tile(attention_mask[None, ...], (batch_size, 1, 1))
-            attention_mask = tf.cast(attention_mask, tf.int32)
-
-        # [batch_size, seq_len, num_samples]
-        enc_out = self.forward(time_seqs, time_delta_seqs, type_seqs, attention_mask)
-
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
-
-        if compute_last_step_only:
-            lambdas = tf.nn.softplus(encoder_output[:, -1:, :, :])
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = tf.nn.softplus(encoder_output)
-        return lambdas
+import torch
+import torch.nn as nn
+
+from easy_tpp.model.torch_model.torch_baselayer import EncoderLayer, MultiHeadAttention, \
+    TimeShiftedPositionalEncoding
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class SAHP(TorchBaseModel):
+    """Torch implementation of Self-Attentive Hawkes Process, ICML 2020.
+    Part of the code is collected from https://github.com/yangalan123/anhp-andtt/blob/master/sahp
+
+    I slightly modify the original code because it is not stable.
+
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(SAHP, self).__init__(model_config)
+        self.d_model = model_config.hidden_size
+        self.d_time = model_config.time_emb_size
+
+        self.use_norm = model_config.use_ln
+
+        # position vector, used for temporal encoding
+        self.layer_position_emb = TimeShiftedPositionalEncoding(d_model=self.d_model)
+
+        self.n_layers = model_config.num_layers
+        self.n_head = model_config.num_heads
+        self.dropout = model_config.dropout_rate
+
+        # convert hidden vectors into a scalar
+        self.layer_intensity_hidden = nn.Linear(self.d_model, self.num_event_types)
+        self.softplus = nn.Softplus()
+
+        self.stack_layers = nn.ModuleList(
+            [EncoderLayer(
+                self.d_model,
+                MultiHeadAttention(self.n_head, self.d_model, self.d_model, self.dropout,
+                                   output_linear=False),
+
+                use_residual=False,
+                dropout=self.dropout
+            ) for _ in range(self.n_layers)])
+
+        if self.use_norm:
+            self.norm = nn.LayerNorm(self.d_model)
+
+        # Equation (12): mu
+        self.mu = torch.empty([self.d_model, self.num_event_types])
+        # Equation (13): eta
+        self.eta = torch.empty([self.d_model, self.num_event_types])
+        # Equation (14): gamma
+        self.gamma = torch.empty([self.d_model, self.num_event_types])
+
+        nn.init.xavier_normal_(self.mu)
+        nn.init.xavier_normal_(self.eta)
+        nn.init.xavier_normal_(self.gamma)
+
+    def state_decay(self, encode_state, mu, eta, gamma, duration_t):
+        """Equation (15), which computes the pre-intensity states
+
+        Args:
+            encode_state (tensor): [batch_size, seq_len, hidden_size].
+            mu (tensor): [batch_size, seq_len, hidden_size].
+            eta (tensor): [batch_size, seq_len, hidden_size].
+            gamma (tensor): [batch_size, seq_len, hidden_size].
+            duration_t (tensor): [batch_size, seq_len, num_sample].
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+
+        # [batch_size, hidden_dim]
+        states = torch.matmul(encode_state, mu) + (
+                    torch.matmul(encode_state, eta) - torch.matmul(encode_state, mu)) * torch.exp(
+            -torch.matmul(encode_state, gamma) * duration_t)
+        return states
+
+    def forward(self, time_seqs, time_delta_seqs, event_seqs, attention_mask):
+        """Call the model
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            event_seqs (tensor): [batch_size, seq_len], event type seqs.
+            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+        type_embedding = self.layer_type_emb(event_seqs)
+        position_embedding = self.layer_position_emb(time_seqs, time_delta_seqs)
+
+        enc_output = type_embedding + position_embedding
+
+        for enc_layer in self.stack_layers:
+            enc_output = enc_layer(
+                enc_output,
+                mask=attention_mask)
+            if self.use_norm:
+                enc_output = self.norm(enc_output)
+        # [batch_size, seq_len, hidden_dim]
+        return enc_output
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (tuple, list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch
+
+        enc_out = self.forward(time_seqs[:, :-1], time_delta_seqs[:, 1:], type_seqs[:, :-1], attention_mask[:, 1:, :-1])
+
+        cell_t = self.state_decay(encode_state=enc_out,
+                                  mu=self.mu[None, ...],
+                                  eta=self.eta[None, ...],
+                                  gamma=self.gamma[None, ...],
+                                  duration_t=time_delta_seqs[:, 1:, None])
+
+        # [batch_size, seq_len, num_event_types]
+        lambda_at_event = self.softplus(cell_t)
+
+        # 2. compute non-event-loglik (using MC sampling to compute integral)
+        # 2.1 sample times
+        # [batch_size, seq_len, num_sample]
+        sample_dtimes = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        # 2.2 compute intensities at sampled times
+        # [batch_size, num_times = max_len - 1, num_sample, event_num]
+        state_t_sample = self.compute_states_at_sample_times(encode_state=enc_out,
+                                                             sample_dtimes=sample_dtimes)
+        lambda_t_sample = self.softplus(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        # return enc_inten to compute accuracy
+        loss = - (event_ll - non_event_ll).sum()
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self,
+                                       encode_state,
+                                       sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            encode_state (tensor): three tensors with each shape [batch_size, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: [batch_size, seq_len, num_samples, hidden_size]， hidden state at each sampled time.
+        """
+
+        cell_states = self.state_decay(encode_state[:, :, None, :],
+                                       self.mu[None, None, ...],
+                                       self.eta[None, None, ...],
+                                       self.gamma[None, None, ...],
+                                       sample_dtimes[:, :, :, None])
+
+        return cell_states
+
+    def compute_intensities_at_sample_times(self,
+                                            time_seqs,
+                                            time_delta_seqs,
+                                            type_seqs,
+                                            sample_dtimes,
+                                            **kwargs):
+        """Compute hidden states at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
+        """
+
+        attention_mask = kwargs.get('attention_mask', None)
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        if attention_mask is None:
+            batch_size, seq_len = time_seqs.size()
+            attention_mask = torch.triu(torch.ones(seq_len, seq_len), diagonal=1).unsqueeze(0)
+            attention_mask = attention_mask.expand(batch_size, -1, -1).to(torch.bool)
+
+        # [batch_size, seq_len, num_samples]
+        enc_out = self.forward(time_seqs, time_delta_seqs, type_seqs, attention_mask)
+
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
+
+        if compute_last_step_only:
+            lambdas = self.softplus(encoder_output[:, -1:, :, :])
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = self.softplus(encoder_output)
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thinning.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_thinning.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-import tensorflow as tf
-from tensorflow import keras
-
-from easy_tpp.utils.tf_utils import get_shape_list
-
-
-class EventSampler(keras.Model):
-    """
-    Event Sequence Sampler based on thinning algorithm
-
-    The algorithm can be found at Algorithm 2 of The Neural Hawkes Process: A Neurally Self-Modulating
-    Multivariate Point Process, https://arxiv.org/abs/1612.09328.
-
-    The implementation uses code from https://github.com/yangalan123/anhp-andtt/blob/master/anhp/esm/thinning.py
-
-    """
-
-    def __init__(self, num_sample, num_exp, over_sample_rate, num_samples_boundary, dtime_max, patience_counter):
-        super(EventSampler, self).__init__()
-        self.num_sample = num_sample  # number of sampled next event times via thinning algorithm,
-        # used to compute predictions
-        self.num_exp = num_exp  # number of i.i.d. Exp(intensity_bound) draws at one time in thinning algorithm
-        self.over_sample_rate = over_sample_rate
-        self.num_samples_boundary = num_samples_boundary
-        self.dtime_max = dtime_max
-        self.patience_counter = patience_counter
-
-    def compute_intensity_upper_bound(self,
-                                      time_seqs,
-                                      time_delta_seqs,
-                                      type_seqs,
-                                      intensity_fn,
-                                      compute_last_step_only):
-        """
-
-        Args:
-            time_seqs: [batch_size, seq_len]
-            time_delta_seqs: [batch_size, seq_len]
-            type_seqs: [batch_size, seq_len]
-
-        Returns:
-            The upper bound of intensity at each event timestamp
-            [batch_size, seq_len]
-
-        """
-
-        # [1, 1, num_samples_boundary]
-        time_for_bound_sampled = tf.linspace(start=0.0,
-                                             stop=1.0,
-                                             num=self.num_samples_boundary)[None, None, :]
-
-        # [batch_size, seq_len, num_sample]
-        dtime_for_bound_sampled = time_delta_seqs[:, :, None] * time_for_bound_sampled
-
-        # [batch_size, seq_len, num_sample, event_num]
-        intensities_for_bound = intensity_fn(time_seqs,
-                                             time_delta_seqs,
-                                             type_seqs,
-                                             dtime_for_bound_sampled,
-                                             compute_last_step_only=compute_last_step_only)
-
-        # [batch_size, seq_len]
-        bounds = tf.reduce_max(tf.reduce_sum(intensities_for_bound, axis=-1), axis=-1) * self.over_sample_rate
-
-        return bounds
-
-    def sample_exp_distribution(self, sample_rate):
-        """
-
-        Args:
-            sample_rate: [batch_size, seq_len]
-            time_delta_seq: [batch_size, seq_len]
-
-        Returns:
-            exp_numbers: [batch_size, seq_len, num_sample, num_exp]
-
-        """
-
-        # can not pass batch_size and seq_len to the random generator as they are dynamics
-        # so we reuse rnd for all samples
-        batch_size, seq_len = get_shape_list(sample_rate)
-        # [batch_size, seq_len, num_exp]
-        exp_numbers = tf.random.gamma(shape=[batch_size, seq_len, self.num_exp], alpha=1.0)
-
-        # [batch_size, seq_len, num_exp]
-        # exp_numbers = torch.tile(exp_numbers, [1, 1, self.num_sample, 1])
-
-        # [batch_size, seq_len, num_exp]
-        # div by sample_rate is equivalent to exp(sample_rate),
-        # see https://en.wikipedia.org/wiki/Exponential_distribution
-        exp_numbers = exp_numbers / sample_rate[:, :, None]
-
-        return exp_numbers
-
-    def sample_uniform_distribution(self, intensity_upper_bound):
-        """
-
-        Returns:
-            unif_numbers: [batch_size, seq_len, num_sample, num_exp]
-
-        """
-        batch_size, seq_len = get_shape_list(intensity_upper_bound)
-        unif_numbers = tf.random.uniform([batch_size, seq_len, self.num_sample, self.num_exp])
-
-        return unif_numbers
-
-    def sample_accept(self, unif_numbers, sample_rate, total_intensities):
-        """
-
-        Args:
-            unif_numbers: [batch_size, max_len, num_sample, num_exp]
-            sample_rate: [batch_size, max_len]
-            total_intensities: [batch_size, seq_len, num_sample, num_exp]
-
-        for each parallel draw, find its min criterion： if that < 1.0, the 1st (i.e. smallest) sampled time
-        with cri < 1.0 is accepted; if none is accepted, use boundary / maxsampletime for that draw
-
-        Returns:
-
-        """
-        # [batch_size, max_len, num_sample, num_exp]
-        criterion = unif_numbers * sample_rate[:, :, None, None] / total_intensities
-
-        # [batch_size, max_len, num_sample]
-        min_cri_each_draw = tf.reduce_min(criterion, axis=-1)
-
-        # find out unif_numbers * sample_rate < intensity
-        # [batch_size, max_len, num_sample]
-        who_has_accepted_times = min_cri_each_draw < 1.0
-
-        return criterion, who_has_accepted_times
-
-    def draw_next_time_one_step(self,
-                                time_seqs,
-                                time_delta_seqs,
-                                type_seqs,
-                                dtime_boundary,
-                                intensity_fn,
-                                compute_last_step_only):
-        # 1. compute the upper bound of the intensity at each timestamp
-        # [batch_size, seq_len]
-        intensity_upper_bound = self.compute_intensity_upper_bound(time_seqs,
-                                                                   time_delta_seqs,
-                                                                   type_seqs,
-                                                                   intensity_fn,
-                                                                   compute_last_step_only)
-
-        # 2. draw exp distribution with intensity = intensity_upper_bound
-        # we apply fast approximation, i.e., re-use exp sample times for computation
-        # [batch_size, seq_len, num_exp]
-        exp_numbers = self.sample_exp_distribution(intensity_upper_bound)
-
-        # 3. compute intensity at sampled times from exp distribution
-        # [batch_size, seq_len, num_exp, event_num]
-        intensities_at_sampled_times = intensity_fn(time_seqs,
-                                                    time_delta_seqs,
-                                                    type_seqs,
-                                                    exp_numbers,
-                                                    compute_last_step_only=compute_last_step_only)
-
-        # [batch_size, seq_len, num_exp]
-        total_intensities = tf.reduce_sum(intensities_at_sampled_times, axis=-1)
-
-        # add one dim of num_sample: re-use the intensity for samples for prediction
-        # [batch_size, seq_len, num_sample, num_exp]
-        total_intensities = tf.tile(total_intensities[:, :, None, :], [1, 1, self.num_sample, 1])
-        # [batch_size, seq_len, num_sample, num_exp]
-        exp_numbers = tf.tile(exp_numbers[:, :, None, :], [1, 1, self.num_sample, 1])
-
-        # 4. draw uniform distribution
-        # [batch_size, seq_len, num_sample, num_exp]
-        unif_numbers = self.sample_uniform_distribution(intensity_upper_bound)
-
-        # 5. find out accepted intensities
-        # [batch_size, max_len, num_sample]
-        criterion, who_has_accepted_times = self.sample_accept(unif_numbers, intensity_upper_bound,
-                                                               total_intensities)
-
-        # 6. find out accepted dtimes
-        sampled_dtimes_accepted = tf.identity(exp_numbers)
-        # for unaccepted, use boundary/maxsampletime for that draw
-
-        # [batch_size, seq_len, num_sample, num_exp]
-        sampled_dtimes_accepted = tf.where(criterion >= 1.0,
-                                           tf.ones_like(sampled_dtimes_accepted) * tf.reduce_max(exp_numbers,
-                                                                                                 axis=-1,
-                                                                                                 keepdims=True) + 1.0,
-                                           sampled_dtimes_accepted)
-
-        accepted_times_each_draw = tf.reduce_min(sampled_dtimes_accepted, axis=-1)
-
-        # 7. fill out result
-        # [batch_size, seq_len, num_sample]
-        dtime_boundary = tf.tile(dtime_boundary[..., None], [1, 1, self.num_sample])
-
-        # [batch_size, seq_len, num_sample]
-        res = tf.ones_like(dtime_boundary) * dtime_boundary
-
-        # [batch_size, seq_len, num_sample]
-        weights = tf.ones_like(dtime_boundary)
-        weights /= tf.reduce_sum(weights, axis=-1, keepdims=True)
-
-        # [batch_size, seq_len, num_sample]
-        res = tf.where(who_has_accepted_times,
-                       tf.ones_like(res) * accepted_times_each_draw,
-                       res)
-
-        who_not_accept = ~who_has_accepted_times
-
-        who_reach_further = exp_numbers[..., -1] > dtime_boundary
-
-        res = tf.where(who_not_accept & who_reach_further,
-                       exp_numbers[..., -1],
-                       res)
-
-        return res, weights
+import tensorflow as tf
+from tensorflow import keras
+
+from easy_tpp.utils.tf_utils import get_shape_list
+
+
+class EventSampler(keras.Model):
+    """
+    Event Sequence Sampler based on thinning algorithm
+
+    The algorithm can be found at Algorithm 2 of The Neural Hawkes Process: A Neurally Self-Modulating
+    Multivariate Point Process, https://arxiv.org/abs/1612.09328.
+
+    The implementation uses code from https://github.com/yangalan123/anhp-andtt/blob/master/anhp/esm/thinning.py
+
+    """
+
+    def __init__(self, num_sample, num_exp, over_sample_rate, num_samples_boundary, dtime_max, patience_counter):
+        super(EventSampler, self).__init__()
+        self.num_sample = num_sample  # number of sampled next event times via thinning algorithm,
+        # used to compute predictions
+        self.num_exp = num_exp  # number of i.i.d. Exp(intensity_bound) draws at one time in thinning algorithm
+        self.over_sample_rate = over_sample_rate
+        self.num_samples_boundary = num_samples_boundary
+        self.dtime_max = dtime_max
+        self.patience_counter = patience_counter
+
+    def compute_intensity_upper_bound(self,
+                                      time_seqs,
+                                      time_delta_seqs,
+                                      type_seqs,
+                                      intensity_fn,
+                                      compute_last_step_only):
+        """
+
+        Args:
+            time_seqs: [batch_size, seq_len]
+            time_delta_seqs: [batch_size, seq_len]
+            type_seqs: [batch_size, seq_len]
+
+        Returns:
+            The upper bound of intensity at each event timestamp
+            [batch_size, seq_len]
+
+        """
+
+        # [1, 1, num_samples_boundary]
+        time_for_bound_sampled = tf.linspace(start=0.0,
+                                             stop=1.0,
+                                             num=self.num_samples_boundary)[None, None, :]
+
+        # [batch_size, seq_len, num_sample]
+        dtime_for_bound_sampled = time_delta_seqs[:, :, None] * time_for_bound_sampled
+
+        # [batch_size, seq_len, num_sample, event_num]
+        intensities_for_bound = intensity_fn(time_seqs,
+                                             time_delta_seqs,
+                                             type_seqs,
+                                             dtime_for_bound_sampled,
+                                             compute_last_step_only=compute_last_step_only)
+
+        # [batch_size, seq_len]
+        bounds = tf.reduce_max(tf.reduce_sum(intensities_for_bound, axis=-1), axis=-1) * self.over_sample_rate
+
+        return bounds
+
+    def sample_exp_distribution(self, sample_rate):
+        """
+
+        Args:
+            sample_rate: [batch_size, seq_len]
+            time_delta_seq: [batch_size, seq_len]
+
+        Returns:
+            exp_numbers: [batch_size, seq_len, num_sample, num_exp]
+
+        """
+
+        # can not pass batch_size and seq_len to the random generator as they are dynamics
+        # so we reuse rnd for all samples
+        batch_size, seq_len = get_shape_list(sample_rate)
+        # [batch_size, seq_len, num_exp]
+        exp_numbers = tf.random.gamma(shape=[batch_size, seq_len, self.num_exp], alpha=1.0)
+
+        # [batch_size, seq_len, num_exp]
+        # exp_numbers = torch.tile(exp_numbers, [1, 1, self.num_sample, 1])
+
+        # [batch_size, seq_len, num_exp]
+        # div by sample_rate is equivalent to exp(sample_rate),
+        # see https://en.wikipedia.org/wiki/Exponential_distribution
+        exp_numbers = exp_numbers / sample_rate[:, :, None]
+
+        return exp_numbers
+
+    def sample_uniform_distribution(self, intensity_upper_bound):
+        """
+
+        Returns:
+            unif_numbers: [batch_size, seq_len, num_sample, num_exp]
+
+        """
+        batch_size, seq_len = get_shape_list(intensity_upper_bound)
+        unif_numbers = tf.random.uniform([batch_size, seq_len, self.num_sample, self.num_exp])
+
+        return unif_numbers
+
+    def sample_accept(self, unif_numbers, sample_rate, total_intensities):
+        """
+
+        Args:
+            unif_numbers: [batch_size, max_len, num_sample, num_exp]
+            sample_rate: [batch_size, max_len]
+            total_intensities: [batch_size, seq_len, num_sample, num_exp]
+
+        for each parallel draw, find its min criterion： if that < 1.0, the 1st (i.e. smallest) sampled time
+        with cri < 1.0 is accepted; if none is accepted, use boundary / maxsampletime for that draw
+
+        Returns:
+
+        """
+        # [batch_size, max_len, num_sample, num_exp]
+        criterion = unif_numbers * sample_rate[:, :, None, None] / total_intensities
+
+        # [batch_size, max_len, num_sample]
+        min_cri_each_draw = tf.reduce_min(criterion, axis=-1)
+
+        # find out unif_numbers * sample_rate < intensity
+        # [batch_size, max_len, num_sample]
+        who_has_accepted_times = min_cri_each_draw < 1.0
+
+        return criterion, who_has_accepted_times
+
+    def draw_next_time_one_step(self,
+                                time_seqs,
+                                time_delta_seqs,
+                                type_seqs,
+                                dtime_boundary,
+                                intensity_fn,
+                                compute_last_step_only):
+        # 1. compute the upper bound of the intensity at each timestamp
+        # [batch_size, seq_len]
+        intensity_upper_bound = self.compute_intensity_upper_bound(time_seqs,
+                                                                   time_delta_seqs,
+                                                                   type_seqs,
+                                                                   intensity_fn,
+                                                                   compute_last_step_only)
+
+        # 2. draw exp distribution with intensity = intensity_upper_bound
+        # we apply fast approximation, i.e., re-use exp sample times for computation
+        # [batch_size, seq_len, num_exp]
+        exp_numbers = self.sample_exp_distribution(intensity_upper_bound)
+
+        # 3. compute intensity at sampled times from exp distribution
+        # [batch_size, seq_len, num_exp, event_num]
+        intensities_at_sampled_times = intensity_fn(time_seqs,
+                                                    time_delta_seqs,
+                                                    type_seqs,
+                                                    exp_numbers,
+                                                    compute_last_step_only=compute_last_step_only)
+
+        # [batch_size, seq_len, num_exp]
+        total_intensities = tf.reduce_sum(intensities_at_sampled_times, axis=-1)
+
+        # add one dim of num_sample: re-use the intensity for samples for prediction
+        # [batch_size, seq_len, num_sample, num_exp]
+        total_intensities = tf.tile(total_intensities[:, :, None, :], [1, 1, self.num_sample, 1])
+        # [batch_size, seq_len, num_sample, num_exp]
+        exp_numbers = tf.tile(exp_numbers[:, :, None, :], [1, 1, self.num_sample, 1])
+
+        # 4. draw uniform distribution
+        # [batch_size, seq_len, num_sample, num_exp]
+        unif_numbers = self.sample_uniform_distribution(intensity_upper_bound)
+
+        # 5. find out accepted intensities
+        # [batch_size, max_len, num_sample]
+        criterion, who_has_accepted_times = self.sample_accept(unif_numbers, intensity_upper_bound,
+                                                               total_intensities)
+
+        # 6. find out accepted dtimes
+        sampled_dtimes_accepted = tf.identity(exp_numbers)
+        # for unaccepted, use boundary/maxsampletime for that draw
+
+        # [batch_size, seq_len, num_sample, num_exp]
+        sampled_dtimes_accepted = tf.where(criterion >= 1.0,
+                                           tf.ones_like(sampled_dtimes_accepted) * tf.reduce_max(exp_numbers,
+                                                                                                 axis=-1,
+                                                                                                 keepdims=True) + 1.0,
+                                           sampled_dtimes_accepted)
+
+        accepted_times_each_draw = tf.reduce_min(sampled_dtimes_accepted, axis=-1)
+
+        # 7. fill out result
+        # [batch_size, seq_len, num_sample]
+        dtime_boundary = tf.tile(dtime_boundary[..., None], [1, 1, self.num_sample])
+
+        # [batch_size, seq_len, num_sample]
+        res = tf.ones_like(dtime_boundary) * dtime_boundary
+
+        # [batch_size, seq_len, num_sample]
+        weights = tf.ones_like(dtime_boundary)
+        weights /= tf.reduce_sum(weights, axis=-1, keepdims=True)
+
+        # [batch_size, seq_len, num_sample]
+        res = tf.where(who_has_accepted_times,
+                       tf.ones_like(res) * accepted_times_each_draw,
+                       res)
+
+        who_not_accept = ~who_has_accepted_times
+
+        who_reach_further = exp_numbers[..., -1] > dtime_boundary
+
+        res = tf.where(who_not_accept & who_reach_further,
+                       exp_numbers[..., -1],
+                       res)
+
+        return res, weights
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thp.py` & `easy_tpp-0.0.5/easy_tpp/model/tf_model/tf_thp.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-import tensorflow as tf
-from tensorflow.python.keras import layers
-
-from easy_tpp.model.tf_model.tf_baselayer import EncoderLayer, TimePositionalEncoding
-from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-from easy_tpp.utils.tf_utils import get_shape_list
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class THP(TfBaseModel):
-    """Tensorflow implementation of Transformer Hawkes Process, ICML 2020, https://arxiv.org/abs/2002.09291.
-    """
-
-    def __init__(self, model_config):
-        """Intialiaze the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(THP, self).__init__(model_config)
-        self.d_model = model_config.hidden_size
-        self.d_time = model_config.time_emb_size
-        self.use_norm = model_config.use_ln
-
-        self.n_layers = model_config.num_layers
-        self.n_head = model_config.num_heads
-        self.dropout = model_config.dropout_rate
-
-    def build_graph(self):
-        """Build up the network
-        """
-        with tf.variable_scope('THP'):
-            self.build_input_graph()
-
-            self.layer_temporal_encoding = TimePositionalEncoding(self.d_model)
-
-            self.factor_intensity_base = tf.get_variable(name='intensity_base', shape=[1, self.num_event_types])
-            self.factor_intensity_decay = tf.get_variable(name='intensity_decay',
-                                                          shape=[1, self.num_event_types])
-
-            # convert hidden vectors into event-type-sized vector
-            self.layer_intensity_hidden = layers.Dense(self.num_event_types)
-            self.softplus = tf.nn.softplus
-
-            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
-
-            self.stack_layers = [EncoderLayer(hidden_size=self.d_model,
-                                              num_heads=self.n_head,
-                                              dropout_rate=self.dropout) for _ in range(self.n_layers)]
-
-            self.loss, self.num_event = self.loglike_loss()
-
-            # Make predictions
-            if self.gen_config and self.gen_config['num_step_gen'] == 1:
-                self.dtime_predict_one_step, self.type_predict_one_step = \
-                    self.predict_one_step_at_every_event(self.time_seqs,
-                                                         self.time_delta_seqs,
-                                                         self.type_seqs)
-
-            if self.gen_config and self.gen_config['num_step_gen'] > 1:
-                # make generations
-                self.dtime_generation, self.type_generation = \
-                    self.predict_multi_step_since_last_event(self.time_seqs,
-                                                             self.time_delta_seqs,
-                                                             self.type_seqs,
-                                                             num_step=self.gen_config.num_step_gen)
-
-    def forward(self, time_seqs, type_seqs, attention_mask):
-        """Call the model
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-        # [batch_size, seq_len, hidden_size]
-        tem_enc = self.layer_temporal_encoding(time_seqs)
-        enc_output = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size]
-        for enc_layer in self.stack_layers:
-            enc_output += tem_enc
-            enc_output = enc_layer((
-                enc_output,
-                attention_mask))
-        return enc_output
-
-    def loglike_loss(self):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-        # 1. compute event-loglik
-        enc_out = self.forward(self.time_seqs[:, :-1],
-                               self.type_seqs[:, :-1],
-                               self.attention_mask[:, 1:, :-1])
-
-        # [1, 1, num_event_types]
-        factor_intensity_decay = self.factor_intensity_decay[None, ...]
-        factor_intensity_base = self.factor_intensity_base[None, ...]
-
-        # update time decay based on Equation (6)
-        # [batch_size, seq_len, num_event_types]
-        intensity_states = factor_intensity_decay * self.time_delta_seqs[:, 1:, None] + self.layer_intensity_hidden(
-            enc_out) + factor_intensity_base
-
-        lambda_at_event = self.softplus(intensity_states)
-
-        # 2. compute non-event-loglik (using MC sampling to compute integral)
-        # 2.1 sample times
-        # [batch_size, seq_len, num_sample]
-        sample_dtimes = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
-
-        # 2.2 compute intensities at sampled times
-        # [batch_size, num_times = max_len - 1, num_sample, event_num]
-        state_t_sample = self.compute_states_at_sample_times(event_states=enc_out,
-                                                             sample_dtimes=sample_dtimes)
-        lambda_t_sample = self.softplus(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
-                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=self.type_mask[:, 1:])
-
-        # return enc_inten to compute accuracy
-        loss = - tf.reduce_sum(event_ll - non_event_ll)
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self, event_states, sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            event_states (tensor): [batch_size, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: hidden state at each sampled time.
-        """
-        # [batch_size, seq_len, 1, hidden_size]
-        event_states = event_states[:, :, None, :]
-
-        # [batch_size, seq_len, num_samples, 1]
-        sample_dtimes = sample_dtimes[..., None]
-
-        # [1, 1, 1, num_event_types]
-        factor_intensity_decay = self.factor_intensity_decay[None, None, ...]
-        factor_intensity_base = self.factor_intensity_base[None, None, ...]
-
-        # update time decay based on Equation (6)
-        # [batch_size, seq_len, num_samples, num_event_types]
-        intensity_states = factor_intensity_decay * sample_dtimes + self.layer_intensity_hidden(
-            event_states) + factor_intensity_base
-
-        return intensity_states
-
-    def compute_intensities_at_sample_times(self,
-                                            time_seqs,
-                                            time_delta_seqs,
-                                            type_seqs,
-                                            sample_dtimes,
-                                            **kwargs):
-        """Compute the intensity at sampled times.
-
-         Args:
-             time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
-             time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
-             type_seqs (tensor): [batch_size, seq_len], sequences of event types.
-             sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
-
-         Returns:
-             tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
-         """
-
-        attention_mask = kwargs.get('attention_mask', None)
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        if attention_mask is None:
-            batch_size, seq_len = get_shape_list(time_seqs)
-            attention_mask = tf.ones((seq_len, seq_len))
-            # only keep the strict upper triangular
-            lower_diag_masks = tf.linalg.LinearOperatorLowerTriangular(tf.ones_like(attention_mask)).to_dense()
-            attention_mask = tf.where(tf.equal(lower_diag_masks, 0),
-                                      attention_mask,
-                                      tf.zeros_like(attention_mask))
-            attention_mask = tf.tile(attention_mask[None, ...], (batch_size, 1, 1))
-            attention_mask = tf.cast(attention_mask, tf.int32)
-
-        # [batch_size, seq_len, num_samples]
-        enc_out = self.forward(time_seqs, type_seqs, attention_mask)
-
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
-
-        if compute_last_step_only:
-            lambdas = self.layer_intensity(encoder_output[:, -1:, :, :])
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = self.layer_intensity(encoder_output)
-        return lambdas
+import tensorflow as tf
+from tensorflow.python.keras import layers
+
+from easy_tpp.model.tf_model.tf_baselayer import EncoderLayer, TimePositionalEncoding
+from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+from easy_tpp.utils.tf_utils import get_shape_list
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class THP(TfBaseModel):
+    """Tensorflow implementation of Transformer Hawkes Process, ICML 2020, https://arxiv.org/abs/2002.09291.
+    """
+
+    def __init__(self, model_config):
+        """Intialiaze the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(THP, self).__init__(model_config)
+        self.d_model = model_config.hidden_size
+        self.d_time = model_config.time_emb_size
+        self.use_norm = model_config.use_ln
+
+        self.n_layers = model_config.num_layers
+        self.n_head = model_config.num_heads
+        self.dropout = model_config.dropout_rate
+
+    def build_graph(self):
+        """Build up the network
+        """
+        with tf.variable_scope('THP'):
+            self.build_input_graph()
+
+            self.layer_temporal_encoding = TimePositionalEncoding(self.d_model)
+
+            self.factor_intensity_base = tf.get_variable(name='intensity_base', shape=[1, self.num_event_types])
+            self.factor_intensity_decay = tf.get_variable(name='intensity_decay',
+                                                          shape=[1, self.num_event_types])
+
+            # convert hidden vectors into event-type-sized vector
+            self.layer_intensity_hidden = layers.Dense(self.num_event_types)
+            self.softplus = tf.nn.softplus
+
+            self.layer_intensity = layers.Dense(self.num_event_types, activation=tf.nn.softplus)
+
+            self.stack_layers = [EncoderLayer(hidden_size=self.d_model,
+                                              num_heads=self.n_head,
+                                              dropout_rate=self.dropout) for _ in range(self.n_layers)]
+
+            self.loss, self.num_event = self.loglike_loss()
+
+            # Make predictions
+            if self.gen_config and self.gen_config['num_step_gen'] == 1:
+                self.dtime_predict_one_step, self.type_predict_one_step = \
+                    self.predict_one_step_at_every_event(self.time_seqs,
+                                                         self.time_delta_seqs,
+                                                         self.type_seqs)
+
+            if self.gen_config and self.gen_config['num_step_gen'] > 1:
+                # make generations
+                self.dtime_generation, self.type_generation = \
+                    self.predict_multi_step_since_last_event(self.time_seqs,
+                                                             self.time_delta_seqs,
+                                                             self.type_seqs,
+                                                             num_step=self.gen_config.num_step_gen)
+
+    def forward(self, time_seqs, type_seqs, attention_mask):
+        """Call the model
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+        # [batch_size, seq_len, hidden_size]
+        tem_enc = self.layer_temporal_encoding(time_seqs)
+        enc_output = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size]
+        for enc_layer in self.stack_layers:
+            enc_output += tem_enc
+            enc_output = enc_layer((
+                enc_output,
+                attention_mask))
+        return enc_output
+
+    def loglike_loss(self):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+        # 1. compute event-loglik
+        enc_out = self.forward(self.time_seqs[:, :-1],
+                               self.type_seqs[:, :-1],
+                               self.attention_mask[:, 1:, :-1])
+
+        # [1, 1, num_event_types]
+        factor_intensity_decay = self.factor_intensity_decay[None, ...]
+        factor_intensity_base = self.factor_intensity_base[None, ...]
+
+        # update time decay based on Equation (6)
+        # [batch_size, seq_len, num_event_types]
+        intensity_states = factor_intensity_decay * self.time_delta_seqs[:, 1:, None] + self.layer_intensity_hidden(
+            enc_out) + factor_intensity_base
+
+        lambda_at_event = self.softplus(intensity_states)
+
+        # 2. compute non-event-loglik (using MC sampling to compute integral)
+        # 2.1 sample times
+        # [batch_size, seq_len, num_sample]
+        sample_dtimes = self.make_dtime_loss_samples(self.time_delta_seqs[:, 1:])
+
+        # 2.2 compute intensities at sampled times
+        # [batch_size, num_times = max_len - 1, num_sample, event_num]
+        state_t_sample = self.compute_states_at_sample_times(event_states=enc_out,
+                                                             sample_dtimes=sample_dtimes)
+        lambda_t_sample = self.softplus(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=self.time_delta_seqs[:, 1:],
+                                                                        seq_mask=self.batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=self.type_mask[:, 1:])
+
+        # return enc_inten to compute accuracy
+        loss = - tf.reduce_sum(event_ll - non_event_ll)
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, event_states, sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            event_states (tensor): [batch_size, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: hidden state at each sampled time.
+        """
+        # [batch_size, seq_len, 1, hidden_size]
+        event_states = event_states[:, :, None, :]
+
+        # [batch_size, seq_len, num_samples, 1]
+        sample_dtimes = sample_dtimes[..., None]
+
+        # [1, 1, 1, num_event_types]
+        factor_intensity_decay = self.factor_intensity_decay[None, None, ...]
+        factor_intensity_base = self.factor_intensity_base[None, None, ...]
+
+        # update time decay based on Equation (6)
+        # [batch_size, seq_len, num_samples, num_event_types]
+        intensity_states = factor_intensity_decay * sample_dtimes + self.layer_intensity_hidden(
+            event_states) + factor_intensity_base
+
+        return intensity_states
+
+    def compute_intensities_at_sample_times(self,
+                                            time_seqs,
+                                            time_delta_seqs,
+                                            type_seqs,
+                                            sample_dtimes,
+                                            **kwargs):
+        """Compute the intensity at sampled times.
+
+         Args:
+             time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+             time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+             type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+             sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
+
+         Returns:
+             tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
+         """
+
+        attention_mask = kwargs.get('attention_mask', None)
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        if attention_mask is None:
+            batch_size, seq_len = get_shape_list(time_seqs)
+            attention_mask = tf.ones((seq_len, seq_len))
+            # only keep the strict upper triangular
+            lower_diag_masks = tf.linalg.LinearOperatorLowerTriangular(tf.ones_like(attention_mask)).to_dense()
+            attention_mask = tf.where(tf.equal(lower_diag_masks, 0),
+                                      attention_mask,
+                                      tf.zeros_like(attention_mask))
+            attention_mask = tf.tile(attention_mask[None, ...], (batch_size, 1, 1))
+            attention_mask = tf.cast(attention_mask, tf.int32)
+
+        # [batch_size, seq_len, num_samples]
+        enc_out = self.forward(time_seqs, type_seqs, attention_mask)
+
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
+
+        if compute_last_step_only:
+            lambdas = self.layer_intensity(encoder_output[:, -1:, :, :])
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = self.layer_intensity(encoder_output)
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_anhn.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_anhn.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-import torch
-from torch import nn
-
-from easy_tpp.model.torch_model.torch_baselayer import MultiHeadAttention
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-
-
-class ANHN(TorchBaseModel):
-    """Torch implementation of Attentive Neural Hawkes Network, IJCNN 2021.
-       http://arxiv.org/abs/2211.11758
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(ANHN, self).__init__(model_config)
-
-        self.d_time = model_config['time_emb_size']
-        self.use_norm = model_config['use_ln']
-
-        self.n_layers = model_config['num_layers']
-        self.n_head = model_config['num_heads']
-        self.dropout = model_config['dropout']
-
-        self.layer_rnn = nn.LSTM(input_size=self.hidden_size, hidden_size=self.hidden_size, batch_first=True)
-
-        self.lambda_w = torch.empty([self.hidden_size, self.num_event_types])
-        self.lambda_b = torch.empty([self.num_event_types, 1])
-        nn.init.xavier_normal_(self.lambda_w)
-        nn.init.xavier_normal_(self.lambda_b)
-
-        self.layer_time_delta = nn.Sequential(nn.Linear(2 * self.hidden_size, self.hidden_size), nn.Softplus())
-
-        self.layer_base_intensity = nn.Sequential(nn.Linear(self.hidden_size, self.hidden_size), nn.Sigmoid())
-
-        self.layer_att = MultiHeadAttention(self.n_head,
-                                            self.hidden_size,
-                                            self.hidden_size,
-                                            self.dropout)
-
-        self.layer_intensity = nn.Sequential(nn.Linear(self.hidden_size, self.num_event_types), nn.Softplus())
-
-        self.layer_temporal_emb = nn.Linear(1, self.hidden_size)
-
-    def forward(self, dtime_seqs, type_seqs, attention_mask):
-        """Call the model.
-
-        Args:
-            dtime_seqs (tensor): [batch_size, seq_len].
-            type_seqs (tensor): [batch_size, seq_len].
-            attention_mask (tensor): [batch_size, seq_len, hidden_size].
-
-        Returns:
-            list: hidden states, [batch_size, seq_len, hidden_size], states right before the event happens;
-                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
-                  the event happens.
-        """
-
-        # [batch_size, seq_len, hidden_size]
-        event_emb = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size]
-        rnn_output, _ = self.layer_rnn(event_emb)
-
-        # [batch_size, seq_len, hidden_size]
-        # mu in Equation (3)
-        intensity_base = self.layer_base_intensity(rnn_output)
-
-        # [batch_size, num_head, seq_len, seq_len]
-        _, att_weight = self.layer_att(rnn_output,
-                                       rnn_output,
-                                       rnn_output,
-                                       mask=attention_mask,
-                                       output_weight=True)
-
-        # [batch_size, seq_len, seq_len, 1]
-        att_weight = torch.sum(att_weight, dim=1)[..., None]
-
-        # At each step, alpha and delta reply on all previous event embeddings because there is a cumsum in Equation
-        # (3), therefore the alpha and beta have shape [batch_size, seq_len, seq_len, hidden_size] when performing
-        # matrix operations.
-        # [batch_size, seq_len, seq_len, hidden_dim]
-        # alpha in Equation (3)
-        intensity_alpha = att_weight * rnn_output[:, None, :, :]
-
-        # compute delta
-        max_len = event_emb.size()[1]
-
-        # [batch_size, seq_len, seq_len, hidden_dim]
-        left = rnn_output[:, None, :, :].repeat(1, max_len, 1, 1)
-        right = rnn_output[:, :, None, :].repeat(1, 1, max_len, 1)
-        # [batch_size, seq_len, seq_len, hidden_dim * 2]
-        cur_prev_concat = torch.concat([left, right], dim=-1)
-        # [batch_size, seq_len, seq_len, hidden_dim]
-        intensity_delta = self.layer_time_delta(cur_prev_concat)
-
-        # compute time elapse
-        # [batch_size, seq_len, seq_len, 1]
-        base_dtime, target_cumsum_dtime = self.compute_cumsum_dtime(dtime_seqs)
-
-        # [batch_size, max_len, hidden_size]
-        imply_lambdas = self.compute_states_at_event_times(intensity_base,
-                                                           intensity_alpha,
-                                                           intensity_delta,
-                                                           target_cumsum_dtime)
-
-        return imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime)
-
-    def loglike_loss(self, batch):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            tuple: loglikelihood loss and num of events.
-        """
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch
-
-        imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime) \
-            = self.forward(time_delta_seqs[:, 1:],
-                           type_seqs[:, :-1],
-                           attention_mask[:, 1:, :-1])
-        lambda_at_event = self.layer_intensity(imply_lambdas)
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = lambda_at_event.size()
-
-        # Compute the big lambda integral in equation (8)
-        # 1 - take num_mc_sample rand points in each event interval
-        # 2 - compute its lambda value for every sample point
-        # 3 - take average of these sample points
-        # 4 - times the interval length
-
-        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seqs[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
-
-        state_t_sample = self.compute_states_at_sample_times(intensity_base, intensity_alpha, intensity_delta,
-                                                             base_dtime, interval_t_sample)
-        lambda_t_sample = self.layer_intensity(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=time_delta_seqs[:, 1:],
-                                                                        seq_mask=batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=type_mask[:, 1:])
-
-        # (num_samples, num_times)
-        loss = - (event_ll - non_event_ll).sum()
-        return loss, num_events
-
-    def compute_cumsum_dtime(self, dtime_seqs):
-        """Compute cumulative delta times.
-
-        Args:
-            dtime_seqs (tensor): [batch_size, seq_len].
-
-        Returns:
-            tensor: [batch_size, seq_len].
-        """
-        # try to replicate tf.cumsum()
-        # [batch_size, seq_len, num_sample]
-        # [0, dt_1, dt_2] => [dt_1 + dt_2, dt_2, 0]
-        cum_dtimes = torch.cumsum(torch.flip(dtime_seqs, dims=[-1]), dim=1)
-        cum_dtimes = torch.concat([torch.zeros_like(cum_dtimes[:, :1]), cum_dtimes[:, 1:]], dim=1)
-
-        # [batch_size, seq_len, seq_len, 1] (lower triangular: positive, upper: negative, diagonal: zero)
-        base_elapses = torch.unsqueeze(cum_dtimes[:, None, :] - cum_dtimes[:, :, None], dim=-1)
-
-        # [batch_size, seq_len, seq_len， 1]
-        target_cumsum = base_elapses + dtime_seqs[:, :, None, None]
-
-        return base_elapses, target_cumsum
-
-    def compute_states_at_event_times(self, intensity_base, intensity_alpha, intensity_delta, cumsum_dtimes):
-        """Compute implied lambda based on Equation (3).
-
-        Args:
-            intensity_base (tensor): [batch_size, seq_len, (num_sample), hidden_size]
-            intensity_alpha (tensor): [batch_size, seq_len, seq_len, (num_sample), hidden_size]
-            intensity_delta (tensor): [batch_size, seq_len, seq_len, (num_sample), hidden_size]
-            cumsum_dtimes: [batch_size, seq_len, (num_sample), 1]
-
-        Returns:
-            hidden states at all cumsum_dtimes: [batch_size, seq_len, num_samples, hidden_size]
-
-        """
-        # to avoid nan calculated by exp after (nan * 0 = nan)
-        elapse = torch.abs(cumsum_dtimes)
-
-        # [batch_size, seq_len, hidden_dim]
-        cumsum_term = torch.sum(intensity_alpha * torch.exp(-intensity_delta * elapse), dim=-2)
-        # [batch_size, seq_len, hidden_dim]
-        imply_lambdas = intensity_base + cumsum_term
-
-        return imply_lambdas
-
-    def compute_states_at_sample_times(self, intensity_base, intensity_alpha, intensity_delta, base_dtime,
-                                       sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            intensity_base (tensor): [batch_size, seq_len, hidden_size].
-            intensity_alpha (tensor): [batch_size, seq_len, seq_len, hidden_size].
-            intensity_delta (tensor): [batch_size, seq_len, seq_len, hidden_size].
-            base_dtime (tensor): [batch_size, seq_len, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: hidden state at each sampled time, [batch_size, seq_len, num_sample, hidden_size].
-        """
-
-        # [batch_size, seq_len, 1, hidden_size]
-        mu = intensity_base[:, :, None]
-
-        # [batch_size, seq_len, 1, seq_len, hidden_size]
-        alpha = intensity_alpha[:, :, None]
-        delta = intensity_delta[:, :, None]
-        base_elapses = base_dtime[:, :, None]
-
-        # [batch_size, seq_len, num_samples, 1, 1]
-        sample_dtimes_ = sample_dtimes[:, :, :, None, None]
-
-        states_samples = []
-        seq_len = intensity_base.size()[1]
-        for _ in range(seq_len):
-            states_samples_ = self.compute_states_at_event_times(mu, alpha, delta, base_elapses + sample_dtimes_)
-            states_samples.append(states_samples_)
-
-        # [batch_size, seq_len, num_sample, hidden_size]
-        states_samples = torch.stack(states_samples, dim=1)
-        return states_samples
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
-        """Compute the intensity at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
-            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
-            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
-            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
-
-        Returns:
-            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
-        """
-
-        attention_mask = kwargs.get('attention_mask', None)
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        if attention_mask is None:
-            batch_size, seq_len = time_seqs.size()
-            attention_mask = torch.triu(torch.ones(seq_len, seq_len), diagonal=1).unsqueeze(0)
-            attention_mask = attention_mask.expand(batch_size, -1, -1).to(torch.bool)
-
-        # [batch_size, seq_len, num_samples]
-        imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime) \
-            = self.forward(time_delta_seqs, type_seqs, attention_mask)
-
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = self.compute_states_at_sample_times(intensity_base, intensity_alpha, intensity_delta,
-                                                             base_dtime, sample_dtimes)
-
-        if compute_last_step_only:
-            lambdas = self.softplus(encoder_output[:, -1:, :, :])
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = self.softplus(encoder_output)
-        return lambdas
+import torch
+from torch import nn
+
+from easy_tpp.model.torch_model.torch_baselayer import MultiHeadAttention
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class ANHN(TorchBaseModel):
+    """Torch implementation of Attentive Neural Hawkes Network, IJCNN 2021.
+       http://arxiv.org/abs/2211.11758
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(ANHN, self).__init__(model_config)
+
+        self.d_time = model_config['time_emb_size']
+        self.use_norm = model_config['use_ln']
+
+        self.n_layers = model_config['num_layers']
+        self.n_head = model_config['num_heads']
+        self.dropout = model_config['dropout']
+
+        self.layer_rnn = nn.LSTM(input_size=self.hidden_size, hidden_size=self.hidden_size, batch_first=True)
+
+        self.lambda_w = torch.empty([self.hidden_size, self.num_event_types])
+        self.lambda_b = torch.empty([self.num_event_types, 1])
+        nn.init.xavier_normal_(self.lambda_w)
+        nn.init.xavier_normal_(self.lambda_b)
+
+        self.layer_time_delta = nn.Sequential(nn.Linear(2 * self.hidden_size, self.hidden_size), nn.Softplus())
+
+        self.layer_base_intensity = nn.Sequential(nn.Linear(self.hidden_size, self.hidden_size), nn.Sigmoid())
+
+        self.layer_att = MultiHeadAttention(self.n_head,
+                                            self.hidden_size,
+                                            self.hidden_size,
+                                            self.dropout)
+
+        self.layer_intensity = nn.Sequential(nn.Linear(self.hidden_size, self.num_event_types), nn.Softplus())
+
+        self.layer_temporal_emb = nn.Linear(1, self.hidden_size)
+
+    def forward(self, dtime_seqs, type_seqs, attention_mask):
+        """Call the model.
+
+        Args:
+            dtime_seqs (tensor): [batch_size, seq_len].
+            type_seqs (tensor): [batch_size, seq_len].
+            attention_mask (tensor): [batch_size, seq_len, hidden_size].
+
+        Returns:
+            list: hidden states, [batch_size, seq_len, hidden_size], states right before the event happens;
+                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
+                  the event happens.
+        """
+
+        # [batch_size, seq_len, hidden_size]
+        event_emb = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size]
+        rnn_output, _ = self.layer_rnn(event_emb)
+
+        # [batch_size, seq_len, hidden_size]
+        # mu in Equation (3)
+        intensity_base = self.layer_base_intensity(rnn_output)
+
+        # [batch_size, num_head, seq_len, seq_len]
+        _, att_weight = self.layer_att(rnn_output,
+                                       rnn_output,
+                                       rnn_output,
+                                       mask=attention_mask,
+                                       output_weight=True)
+
+        # [batch_size, seq_len, seq_len, 1]
+        att_weight = torch.sum(att_weight, dim=1)[..., None]
+
+        # At each step, alpha and delta reply on all previous event embeddings because there is a cumsum in Equation
+        # (3), therefore the alpha and beta have shape [batch_size, seq_len, seq_len, hidden_size] when performing
+        # matrix operations.
+        # [batch_size, seq_len, seq_len, hidden_dim]
+        # alpha in Equation (3)
+        intensity_alpha = att_weight * rnn_output[:, None, :, :]
+
+        # compute delta
+        max_len = event_emb.size()[1]
+
+        # [batch_size, seq_len, seq_len, hidden_dim]
+        left = rnn_output[:, None, :, :].repeat(1, max_len, 1, 1)
+        right = rnn_output[:, :, None, :].repeat(1, 1, max_len, 1)
+        # [batch_size, seq_len, seq_len, hidden_dim * 2]
+        cur_prev_concat = torch.concat([left, right], dim=-1)
+        # [batch_size, seq_len, seq_len, hidden_dim]
+        intensity_delta = self.layer_time_delta(cur_prev_concat)
+
+        # compute time elapse
+        # [batch_size, seq_len, seq_len, 1]
+        base_dtime, target_cumsum_dtime = self.compute_cumsum_dtime(dtime_seqs)
+
+        # [batch_size, max_len, hidden_size]
+        imply_lambdas = self.compute_states_at_event_times(intensity_base,
+                                                           intensity_alpha,
+                                                           intensity_delta,
+                                                           target_cumsum_dtime)
+
+        return imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime)
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            tuple: loglikelihood loss and num of events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch
+
+        imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime) \
+            = self.forward(time_delta_seqs[:, 1:],
+                           type_seqs[:, :-1],
+                           attention_mask[:, 1:, :-1])
+        lambda_at_event = self.layer_intensity(imply_lambdas)
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = lambda_at_event.size()
+
+        # Compute the big lambda integral in equation (8)
+        # 1 - take num_mc_sample rand points in each event interval
+        # 2 - compute its lambda value for every sample point
+        # 3 - take average of these sample points
+        # 4 - times the interval length
+
+        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seqs[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        state_t_sample = self.compute_states_at_sample_times(intensity_base, intensity_alpha, intensity_delta,
+                                                             base_dtime, interval_t_sample)
+        lambda_t_sample = self.layer_intensity(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        # (num_samples, num_times)
+        loss = - (event_ll - non_event_ll).sum()
+        return loss, num_events
+
+    def compute_cumsum_dtime(self, dtime_seqs):
+        """Compute cumulative delta times.
+
+        Args:
+            dtime_seqs (tensor): [batch_size, seq_len].
+
+        Returns:
+            tensor: [batch_size, seq_len].
+        """
+        # try to replicate tf.cumsum()
+        # [batch_size, seq_len, num_sample]
+        # [0, dt_1, dt_2] => [dt_1 + dt_2, dt_2, 0]
+        cum_dtimes = torch.cumsum(torch.flip(dtime_seqs, dims=[-1]), dim=1)
+        cum_dtimes = torch.concat([torch.zeros_like(cum_dtimes[:, :1]), cum_dtimes[:, 1:]], dim=1)
+
+        # [batch_size, seq_len, seq_len, 1] (lower triangular: positive, upper: negative, diagonal: zero)
+        base_elapses = torch.unsqueeze(cum_dtimes[:, None, :] - cum_dtimes[:, :, None], dim=-1)
+
+        # [batch_size, seq_len, seq_len， 1]
+        target_cumsum = base_elapses + dtime_seqs[:, :, None, None]
+
+        return base_elapses, target_cumsum
+
+    def compute_states_at_event_times(self, intensity_base, intensity_alpha, intensity_delta, cumsum_dtimes):
+        """Compute implied lambda based on Equation (3).
+
+        Args:
+            intensity_base (tensor): [batch_size, seq_len, (num_sample), hidden_size]
+            intensity_alpha (tensor): [batch_size, seq_len, seq_len, (num_sample), hidden_size]
+            intensity_delta (tensor): [batch_size, seq_len, seq_len, (num_sample), hidden_size]
+            cumsum_dtimes: [batch_size, seq_len, (num_sample), 1]
+
+        Returns:
+            hidden states at all cumsum_dtimes: [batch_size, seq_len, num_samples, hidden_size]
+
+        """
+        # to avoid nan calculated by exp after (nan * 0 = nan)
+        elapse = torch.abs(cumsum_dtimes)
+
+        # [batch_size, seq_len, hidden_dim]
+        cumsum_term = torch.sum(intensity_alpha * torch.exp(-intensity_delta * elapse), dim=-2)
+        # [batch_size, seq_len, hidden_dim]
+        imply_lambdas = intensity_base + cumsum_term
+
+        return imply_lambdas
+
+    def compute_states_at_sample_times(self, intensity_base, intensity_alpha, intensity_delta, base_dtime,
+                                       sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            intensity_base (tensor): [batch_size, seq_len, hidden_size].
+            intensity_alpha (tensor): [batch_size, seq_len, seq_len, hidden_size].
+            intensity_delta (tensor): [batch_size, seq_len, seq_len, hidden_size].
+            base_dtime (tensor): [batch_size, seq_len, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: hidden state at each sampled time, [batch_size, seq_len, num_sample, hidden_size].
+        """
+
+        # [batch_size, seq_len, 1, hidden_size]
+        mu = intensity_base[:, :, None]
+
+        # [batch_size, seq_len, 1, seq_len, hidden_size]
+        alpha = intensity_alpha[:, :, None]
+        delta = intensity_delta[:, :, None]
+        base_elapses = base_dtime[:, :, None]
+
+        # [batch_size, seq_len, num_samples, 1, 1]
+        sample_dtimes_ = sample_dtimes[:, :, :, None, None]
+
+        states_samples = []
+        seq_len = intensity_base.size()[1]
+        for _ in range(seq_len):
+            states_samples_ = self.compute_states_at_event_times(mu, alpha, delta, base_elapses + sample_dtimes_)
+            states_samples.append(states_samples_)
+
+        # [batch_size, seq_len, num_sample, hidden_size]
+        states_samples = torch.stack(states_samples, dim=1)
+        return states_samples
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
+        """Compute the intensity at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], sequences of timestamps.
+            time_delta_seqs (tensor): [batch_size, seq_len], sequences of delta times.
+            type_seqs (tensor): [batch_size, seq_len], sequences of event types.
+            sampled_dtimes (tensor): [batch_size, seq_len, num_sample], sampled time delta sequence.
+
+        Returns:
+            tensor: intensities as sampled_dtimes, [batch_size, seq_len, num_samples, event_num].
+        """
+
+        attention_mask = kwargs.get('attention_mask', None)
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        if attention_mask is None:
+            batch_size, seq_len = time_seqs.size()
+            attention_mask = torch.triu(torch.ones(seq_len, seq_len), diagonal=1).unsqueeze(0)
+            attention_mask = attention_mask.expand(batch_size, -1, -1).to(torch.bool)
+
+        # [batch_size, seq_len, num_samples]
+        imply_lambdas, (intensity_base, intensity_alpha, intensity_delta), (base_dtime, target_cumsum_dtime) \
+            = self.forward(time_delta_seqs, type_seqs, attention_mask)
+
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = self.compute_states_at_sample_times(intensity_base, intensity_alpha, intensity_delta,
+                                                             base_dtime, sample_dtimes)
+
+        if compute_last_step_only:
+            lambdas = self.softplus(encoder_output[:, -1:, :, :])
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = self.softplus(encoder_output)
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_basemodel.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_basemodel.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-""" Base model with common functionality  """
-
-import torch
-from torch import nn
-
-from easy_tpp.model.torch_model.torch_thinning import EventSampler
-
-
-class TorchBaseModel(nn.Module):
-    def __init__(self, model_config):
-        """Initialize the BaseModel
-
-        Args:
-            model_config (EasyTPP.ModelConfig): model spec of configs
-        """
-        super(TorchBaseModel, self).__init__()
-        self.loss_integral_num_sample_per_step = model_config.loss_integral_num_sample_per_step
-        self.hidden_size = model_config.hidden_size
-        self.num_event_types = model_config.num_event_types  # not include [PAD], [BOS], [EOS]
-        self.num_event_types_pad = model_config.num_event_types_pad  # include [PAD], [BOS], [EOS]
-        self.pad_token_id = model_config.pad_token_id
-        self.eps = torch.finfo(torch.float32).eps
-
-        self.layer_type_emb = nn.Embedding(self.num_event_types_pad,  # have padding
-                                           self.hidden_size,
-                                           padding_idx=self.pad_token_id)
-
-        self.gen_config = model_config.thinning
-        self.event_sampler = None
-        if self.gen_config:
-            self.event_sampler = EventSampler(num_sample=self.gen_config.num_sample,
-                                              num_exp=self.gen_config.num_exp,
-                                              over_sample_rate=self.gen_config.over_sample_rate,
-                                              patience_counter=self.gen_config.patience_counter,
-                                              num_samples_boundary=self.gen_config.num_samples_boundary,
-                                              dtime_max=self.gen_config.dtime_max)
-
-    @staticmethod
-    def generate_model_from_config(model_config):
-        """Generate the model in derived class based on model config.
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        model_id = model_config.model_id
-
-        for subclass in TorchBaseModel.__subclasses__():
-            if subclass.__name__ == model_id:
-                return subclass(model_config)
-
-        raise RuntimeError('No model named ' + model_id)
-
-    @staticmethod
-    def get_logits_at_last_step(logits, batch_non_pad_mask, sample_len=None):
-        """Retrieve the hidden states of last non-pad events.
-
-        Args:
-            logits (tensor): [batch_size, seq_len, hidden_dim], a sequence of logits
-            batch_non_pad_mask (tensor): [batch_size, seq_len], a sequence of masks
-            sample_len (tensor): default None, use batch_non_pad_mask to find out the last non-mask position
-
-        ref: https://medium.com/analytics-vidhya/understanding-indexing-with-pytorch-gather-33717a84ebc4
-
-        Returns:
-            tensor: retrieve the logits of EOS event
-        """
-
-        seq_len = batch_non_pad_mask.sum(dim=1)
-        select_index = seq_len - 1 if sample_len is None else seq_len - 1 - sample_len
-        # [batch_size, hidden_dim]
-        select_index = select_index.unsqueeze(1).repeat(1, logits.size(-1))
-        # [batch_size, 1, hidden_dim]
-        select_index = select_index.unsqueeze(1)
-        # [batch_size, hidden_dim]
-        last_logits = torch.gather(logits, dim=1, index=select_index).squeeze(1)
-        return last_logits
-
-    def compute_loglikelihood(self, time_delta_seq, lambda_at_event, lambdas_loss_samples, seq_mask,
-                              lambda_type_mask):
-        """Compute the loglikelihood of the event sequence based on Equation (8) of NHP paper.
-
-        Args:
-            time_delta_seq (tensor): [batch_size, seq_len], time_delta_seq from model input.
-            lambda_at_event (tensor): [batch_size, seq_len, num_event_types], unmasked intensity at
-            (right after) the event.
-            lambdas_loss_samples (tensor): [batch_size, seq_len, num_sample, num_event_types],
-            intensity at sampling times.
-            seq_mask (tensor): [batch_size, seq_len], sequence mask vector to mask the padded events.
-            lambda_type_mask (tensor): [batch_size, seq_len, num_event_types], type mask matrix to mask the
-            padded event types.
-
-        Returns:
-            tuple: event loglike, non-event loglike, intensity at event with padding events masked
-        """
-
-        # Sum of lambda over every type and every event point
-        # [batch_size, seq_len]
-        event_lambdas = torch.sum(lambda_at_event * lambda_type_mask, dim=-1) + self.eps
-
-        # mask the pad event
-        event_lambdas = event_lambdas.masked_fill_(~seq_mask, 1.0)
-
-        # [batch_size, seq_len)
-        event_ll = torch.log(event_lambdas)
-
-        # Compute the big lambda integral in equation (8) of NHP paper
-        # 1 - take num_mc_sample rand points in each event interval
-        # 2 - compute its lambda value for every sample point
-        # 3 - take average of these sample points
-        # 4 - times the interval length
-
-        # [batch_size, seq_len, n_loss_sample]
-        lambdas_total_samples = lambdas_loss_samples.sum(dim=-1)
-
-        # interval_integral - [batch_size, seq_len]
-        # interval_integral = length_interval * average of sampled lambda(t)
-        non_event_ll = lambdas_total_samples.mean(dim=-1) * time_delta_seq * seq_mask
-
-        num_events = torch.masked_select(event_ll, event_ll.ne(0.0)).size()[0]
-
-        return event_ll, non_event_ll, num_events
-
-    def make_dtime_loss_samples(self, time_delta_seq):
-        """Generate the time point samples for every interval.
-
-        Args:
-            time_delta_seq (tensor): [batch_size, seq_len].
-
-        Returns:
-            tensor: [batch_size, seq_len, n_samples]
-        """
-        # [1, 1, n_samples]
-        dtimes_ratio_sampled = torch.linspace(start=0.0,
-                                              end=1.0,
-                                              steps=self.loss_integral_num_sample_per_step)[None, None, :]
-
-        # [batch_size, max_len, n_samples]
-        sampled_dtimes = time_delta_seq[:, :, None] * dtimes_ratio_sampled
-
-        return sampled_dtimes
-
-    def compute_states_at_sample_times(self, **kwargs):
-        raise NotImplementedError('This need to implemented in inherited class ! ')
-
-    def predict_one_step_at_every_event(self, batch):
-        """One-step prediction for every event in the sequence.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len].
-            time_delta_seqs (tensor): [batch_size, seq_len].
-            type_seqs (tensor): [batch_size, seq_len].
-
-        Returns:
-            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
-        """
-        time_seq, time_delta_seq, event_seq, batch_non_pad_mask, _, type_mask = batch
-
-        # remove the last event, as the prediction based on the last event has no label
-        # time_delta_seq should start from 1, because the first one is zero
-        time_seq, time_delta_seq, event_seq = time_seq[:, :-1], time_delta_seq[:, 1:], event_seq[:, :-1]
-
-        # [batch_size, seq_len]
-        dtime_boundary = time_delta_seq + self.event_sampler.dtime_max
-
-        # [batch_size, seq_len, num_sample]
-        accepted_dtimes, weights = self.event_sampler.draw_next_time_one_step(time_seq,
-                                                                              time_delta_seq,
-                                                                              event_seq,
-                                                                              dtime_boundary,
-                                                                              self.compute_intensities_at_sample_times)
-
-        # [batch_size, seq_len]
-        dtimes_pred = torch.sum(accepted_dtimes * weights, dim=-1)
-
-        # [batch_size, seq_len, 1, event_num]
-        intensities_at_times = self.compute_intensities_at_sample_times(time_seq,
-                                                                        time_delta_seq,
-                                                                        event_seq,
-                                                                        dtimes_pred[:, :, None],
-                                                                        max_steps=event_seq.size()[1])
-
-        # [batch_size, seq_len, event_num]
-        intensities_at_times = intensities_at_times.squeeze(dim=-2)
-
-        types_pred = torch.argmax(intensities_at_times, dim=-1)
-
-        return dtimes_pred, types_pred
-
-    def predict_multi_step_since_last_event(self, batch, forward=False):
-        """Multi-step prediction since last event in the sequence.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len].
-            time_delta_seqs (tensor): [batch_size, seq_len].
-            type_seqs (tensor): [batch_size, seq_len].
-            num_step (int): num of steps for prediction.
-
-        Returns:
-            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
-        """
-        time_seq_label, time_delta_seq_label, event_seq_label, batch_non_pad_mask_label, _, type_mask_label = batch
-
-        num_step = self.gen_config.num_step_gen
-
-        if not forward:
-            time_seq = time_seq_label[:, :-num_step]
-            time_delta_seq = time_delta_seq_label[:, :-num_step]
-            event_seq = event_seq_label[:, :-num_step]
-        else:
-            time_seq, time_delta_seq, event_seq = time_seq_label, time_delta_seq_label, event_seq_label
-
-        for i in range(num_step):
-            # [batch_size, seq_len]
-            dtime_boundary = time_delta_seq + self.event_sampler.dtime_max
-
-            # [batch_size, 1, num_sample]
-            accepted_dtimes, weights = \
-                self.event_sampler.draw_next_time_one_step(time_seq,
-                                                           time_delta_seq,
-                                                           event_seq,
-                                                           dtime_boundary,
-                                                           self.compute_intensities_at_sample_times,
-                                                           compute_last_step_only=True)
-
-            # [batch_size, 1]
-            dtimes_pred = torch.sum(accepted_dtimes * weights, dim=-1)
-
-            # [batch_size, seq_len, 1, event_num]
-            intensities_at_times = self.compute_intensities_at_sample_times(time_seq,
-                                                                            time_delta_seq,
-                                                                            event_seq,
-                                                                            dtimes_pred[:, :, None],
-                                                                            max_steps=event_seq.size()[1])
-
-            # [batch_size, seq_len, event_num]
-            intensities_at_times = intensities_at_times.squeeze(dim=-2)
-
-            # [batch_size, seq_len]
-            types_pred = torch.argmax(intensities_at_times, dim=-1)
-
-            # [batch_size, 1]
-            types_pred_ = types_pred[:, -1:]
-            dtimes_pred_ = dtimes_pred[:, -1:]
-            time_pred_ = time_seq[:, -1:] + dtimes_pred_
-
-            # concat to the prefix sequence
-            time_seq = torch.cat([time_seq, time_pred_], dim=-1)
-            time_delta_seq = torch.cat([time_delta_seq, dtimes_pred_], dim=-1)
-            event_seq = torch.cat([event_seq, types_pred_], dim=-1)
-
-        return time_delta_seq[:, -num_step - 1:], event_seq[:, -num_step - 1:], \
-            time_delta_seq_label[:, -num_step - 1:], event_seq_label[:, -num_step - 1:]
+""" Base model with common functionality  """
+
+import torch
+from torch import nn
+
+from easy_tpp.model.torch_model.torch_thinning import EventSampler
+
+
+class TorchBaseModel(nn.Module):
+    def __init__(self, model_config):
+        """Initialize the BaseModel
+
+        Args:
+            model_config (EasyTPP.ModelConfig): model spec of configs
+        """
+        super(TorchBaseModel, self).__init__()
+        self.loss_integral_num_sample_per_step = model_config.loss_integral_num_sample_per_step
+        self.hidden_size = model_config.hidden_size
+        self.num_event_types = model_config.num_event_types  # not include [PAD], [BOS], [EOS]
+        self.num_event_types_pad = model_config.num_event_types_pad  # include [PAD], [BOS], [EOS]
+        self.pad_token_id = model_config.pad_token_id
+        self.eps = torch.finfo(torch.float32).eps
+
+        self.layer_type_emb = nn.Embedding(self.num_event_types_pad,  # have padding
+                                           self.hidden_size,
+                                           padding_idx=self.pad_token_id)
+
+        self.gen_config = model_config.thinning
+        self.event_sampler = None
+        if self.gen_config:
+            self.event_sampler = EventSampler(num_sample=self.gen_config.num_sample,
+                                              num_exp=self.gen_config.num_exp,
+                                              over_sample_rate=self.gen_config.over_sample_rate,
+                                              patience_counter=self.gen_config.patience_counter,
+                                              num_samples_boundary=self.gen_config.num_samples_boundary,
+                                              dtime_max=self.gen_config.dtime_max)
+
+    @staticmethod
+    def generate_model_from_config(model_config):
+        """Generate the model in derived class based on model config.
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        model_id = model_config.model_id
+
+        for subclass in TorchBaseModel.__subclasses__():
+            if subclass.__name__ == model_id:
+                return subclass(model_config)
+
+        raise RuntimeError('No model named ' + model_id)
+
+    @staticmethod
+    def get_logits_at_last_step(logits, batch_non_pad_mask, sample_len=None):
+        """Retrieve the hidden states of last non-pad events.
+
+        Args:
+            logits (tensor): [batch_size, seq_len, hidden_dim], a sequence of logits
+            batch_non_pad_mask (tensor): [batch_size, seq_len], a sequence of masks
+            sample_len (tensor): default None, use batch_non_pad_mask to find out the last non-mask position
+
+        ref: https://medium.com/analytics-vidhya/understanding-indexing-with-pytorch-gather-33717a84ebc4
+
+        Returns:
+            tensor: retrieve the logits of EOS event
+        """
+
+        seq_len = batch_non_pad_mask.sum(dim=1)
+        select_index = seq_len - 1 if sample_len is None else seq_len - 1 - sample_len
+        # [batch_size, hidden_dim]
+        select_index = select_index.unsqueeze(1).repeat(1, logits.size(-1))
+        # [batch_size, 1, hidden_dim]
+        select_index = select_index.unsqueeze(1)
+        # [batch_size, hidden_dim]
+        last_logits = torch.gather(logits, dim=1, index=select_index).squeeze(1)
+        return last_logits
+
+    def compute_loglikelihood(self, time_delta_seq, lambda_at_event, lambdas_loss_samples, seq_mask,
+                              lambda_type_mask):
+        """Compute the loglikelihood of the event sequence based on Equation (8) of NHP paper.
+
+        Args:
+            time_delta_seq (tensor): [batch_size, seq_len], time_delta_seq from model input.
+            lambda_at_event (tensor): [batch_size, seq_len, num_event_types], unmasked intensity at
+            (right after) the event.
+            lambdas_loss_samples (tensor): [batch_size, seq_len, num_sample, num_event_types],
+            intensity at sampling times.
+            seq_mask (tensor): [batch_size, seq_len], sequence mask vector to mask the padded events.
+            lambda_type_mask (tensor): [batch_size, seq_len, num_event_types], type mask matrix to mask the
+            padded event types.
+
+        Returns:
+            tuple: event loglike, non-event loglike, intensity at event with padding events masked
+        """
+
+        # Sum of lambda over every type and every event point
+        # [batch_size, seq_len]
+        event_lambdas = torch.sum(lambda_at_event * lambda_type_mask, dim=-1) + self.eps
+
+        # mask the pad event
+        event_lambdas = event_lambdas.masked_fill_(~seq_mask, 1.0)
+
+        # [batch_size, seq_len)
+        event_ll = torch.log(event_lambdas)
+
+        # Compute the big lambda integral in equation (8) of NHP paper
+        # 1 - take num_mc_sample rand points in each event interval
+        # 2 - compute its lambda value for every sample point
+        # 3 - take average of these sample points
+        # 4 - times the interval length
+
+        # [batch_size, seq_len, n_loss_sample]
+        lambdas_total_samples = lambdas_loss_samples.sum(dim=-1)
+
+        # interval_integral - [batch_size, seq_len]
+        # interval_integral = length_interval * average of sampled lambda(t)
+        non_event_ll = lambdas_total_samples.mean(dim=-1) * time_delta_seq * seq_mask
+
+        num_events = torch.masked_select(event_ll, event_ll.ne(0.0)).size()[0]
+
+        return event_ll, non_event_ll, num_events
+
+    def make_dtime_loss_samples(self, time_delta_seq):
+        """Generate the time point samples for every interval.
+
+        Args:
+            time_delta_seq (tensor): [batch_size, seq_len].
+
+        Returns:
+            tensor: [batch_size, seq_len, n_samples]
+        """
+        # [1, 1, n_samples]
+        dtimes_ratio_sampled = torch.linspace(start=0.0,
+                                              end=1.0,
+                                              steps=self.loss_integral_num_sample_per_step)[None, None, :]
+
+        # [batch_size, max_len, n_samples]
+        sampled_dtimes = time_delta_seq[:, :, None] * dtimes_ratio_sampled
+
+        return sampled_dtimes
+
+    def compute_states_at_sample_times(self, **kwargs):
+        raise NotImplementedError('This need to implemented in inherited class ! ')
+
+    def predict_one_step_at_every_event(self, batch):
+        """One-step prediction for every event in the sequence.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len].
+            time_delta_seqs (tensor): [batch_size, seq_len].
+            type_seqs (tensor): [batch_size, seq_len].
+
+        Returns:
+            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
+        """
+        time_seq, time_delta_seq, event_seq, batch_non_pad_mask, _, type_mask = batch
+
+        # remove the last event, as the prediction based on the last event has no label
+        # time_delta_seq should start from 1, because the first one is zero
+        time_seq, time_delta_seq, event_seq = time_seq[:, :-1], time_delta_seq[:, 1:], event_seq[:, :-1]
+
+        # [batch_size, seq_len]
+        dtime_boundary = time_delta_seq + self.event_sampler.dtime_max
+
+        # [batch_size, seq_len, num_sample]
+        accepted_dtimes, weights = self.event_sampler.draw_next_time_one_step(time_seq,
+                                                                              time_delta_seq,
+                                                                              event_seq,
+                                                                              dtime_boundary,
+                                                                              self.compute_intensities_at_sample_times)
+
+        # [batch_size, seq_len]
+        dtimes_pred = torch.sum(accepted_dtimes * weights, dim=-1)
+
+        # [batch_size, seq_len, 1, event_num]
+        intensities_at_times = self.compute_intensities_at_sample_times(time_seq,
+                                                                        time_delta_seq,
+                                                                        event_seq,
+                                                                        dtimes_pred[:, :, None],
+                                                                        max_steps=event_seq.size()[1])
+
+        # [batch_size, seq_len, event_num]
+        intensities_at_times = intensities_at_times.squeeze(dim=-2)
+
+        types_pred = torch.argmax(intensities_at_times, dim=-1)
+
+        return dtimes_pred, types_pred
+
+    def predict_multi_step_since_last_event(self, batch, forward=False):
+        """Multi-step prediction since last event in the sequence.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len].
+            time_delta_seqs (tensor): [batch_size, seq_len].
+            type_seqs (tensor): [batch_size, seq_len].
+            num_step (int): num of steps for prediction.
+
+        Returns:
+            tuple: tensors of dtime and type prediction, [batch_size, seq_len].
+        """
+        time_seq_label, time_delta_seq_label, event_seq_label, batch_non_pad_mask_label, _, type_mask_label = batch
+
+        num_step = self.gen_config.num_step_gen
+
+        if not forward:
+            time_seq = time_seq_label[:, :-num_step]
+            time_delta_seq = time_delta_seq_label[:, :-num_step]
+            event_seq = event_seq_label[:, :-num_step]
+        else:
+            time_seq, time_delta_seq, event_seq = time_seq_label, time_delta_seq_label, event_seq_label
+
+        for i in range(num_step):
+            # [batch_size, seq_len]
+            dtime_boundary = time_delta_seq + self.event_sampler.dtime_max
+
+            # [batch_size, 1, num_sample]
+            accepted_dtimes, weights = \
+                self.event_sampler.draw_next_time_one_step(time_seq,
+                                                           time_delta_seq,
+                                                           event_seq,
+                                                           dtime_boundary,
+                                                           self.compute_intensities_at_sample_times,
+                                                           compute_last_step_only=True)
+
+            # [batch_size, 1]
+            dtimes_pred = torch.sum(accepted_dtimes * weights, dim=-1)
+
+            # [batch_size, seq_len, 1, event_num]
+            intensities_at_times = self.compute_intensities_at_sample_times(time_seq,
+                                                                            time_delta_seq,
+                                                                            event_seq,
+                                                                            dtimes_pred[:, :, None],
+                                                                            max_steps=event_seq.size()[1])
+
+            # [batch_size, seq_len, event_num]
+            intensities_at_times = intensities_at_times.squeeze(dim=-2)
+
+            # [batch_size, seq_len]
+            types_pred = torch.argmax(intensities_at_times, dim=-1)
+
+            # [batch_size, 1]
+            types_pred_ = types_pred[:, -1:]
+            dtimes_pred_ = dtimes_pred[:, -1:]
+            time_pred_ = time_seq[:, -1:] + dtimes_pred_
+
+            # concat to the prefix sequence
+            time_seq = torch.cat([time_seq, time_pred_], dim=-1)
+            time_delta_seq = torch.cat([time_delta_seq, dtimes_pred_], dim=-1)
+            event_seq = torch.cat([event_seq, types_pred_], dim=-1)
+
+        return time_delta_seq[:, -num_step - 1:], event_seq[:, -num_step - 1:], \
+            time_delta_seq_label[:, -num_step - 1:], event_seq_label[:, -num_step - 1:]
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_fullynn.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_fullynn.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-import torch
-from torch import nn
-from torch.autograd import grad
-
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-
-
-class CumulHazardFunctionNetwork(nn.Module):
-    """Cumulative Hazard Function Network
-    ref: https://github.com/wassname/torch-neuralpointprocess
-    """
-
-    def __init__(self, model_config):
-        super(CumulHazardFunctionNetwork, self).__init__()
-        self.hidden_size = model_config.hidden_size
-        self.num_mlp_layers = model_config.model_specs['num_mlp_layers']
-        self.num_event_types = model_config.num_event_types
-
-        # transform inter-event time embedding
-        self.layer_dense_1 = nn.Linear(in_features=1, out_features=self.hidden_size)
-
-        # concat rnn states and inter-event time embedding
-        self.layer_dense_2 = nn.Linear(in_features=self.hidden_size * 2, out_features=self.hidden_size)
-
-        # mlp layers
-        self.module_list = nn.ModuleList(
-            [nn.Linear(in_features=self.hidden_size, out_features=self.hidden_size) for _ in
-             range(self.num_mlp_layers - 1)])
-
-        self.layer_dense_3 = nn.Sequential(nn.Linear(in_features=self.hidden_size,
-                                                     out_features=self.num_event_types),
-                                           nn.Softplus())
-
-        self.params_eps = torch.finfo(torch.float32).eps  # ensure positiveness of parameters
-
-        self.init_weights_positive()
-
-    def init_weights_positive(self):
-        for p in self.parameters():
-            p.data = torch.abs(p.data)
-            p.data = torch.clamp(p.data, min=self.params_eps)
-
-    def forward(self, hidden_states, time_delta_seqs):
-        for p in self.parameters():
-            p.data = torch.clamp(p.data, min=self.params_eps)
-
-        time_delta_seqs.requires_grad_(True)
-
-        # [batch_size, seq_len, hidden_size]
-        t = self.layer_dense_1(time_delta_seqs.unsqueeze(dim=-1))
-
-        # [batch_size, seq_len, hidden_size]
-        out = torch.tanh(self.layer_dense_2(torch.cat([hidden_states, t], dim=-1)))
-        for layer in self.module_list:
-            out = torch.tanh(layer(out))
-
-        # [batch_size, seq_len, num_event_types]
-        integral_lambda = self.layer_dense_3(out)
-
-        # [batch_size, seq_len]
-        derivative_integral_lambda = grad(
-            integral_lambda.sum(dim=-1).mean(),
-            time_delta_seqs,
-            create_graph=True, retain_graph=True)[0]
-
-        return integral_lambda, derivative_integral_lambda
-
-
-class FullyNN(TorchBaseModel):
-    """Torch implementation of
-        Fully Neural Network based Model for General Temporal Point Processes, NeurIPS 2019.
-        https://arxiv.org/abs/1905.09690
-
-        ref: https://github.com/KanghoonYoon/torch-neuralpointprocess/blob/master/module.py;
-            https://github.com/wassname/torch-neuralpointprocess
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(FullyNN, self).__init__(model_config)
-
-        self.rnn_type = model_config.rnn_type
-        self.rnn_list = [nn.LSTM, nn.RNN, nn.GRU]
-        for sub_rnn_class in self.rnn_list:
-            if sub_rnn_class.__name__ == self.rnn_type:
-                self.layer_rnn = sub_rnn_class(input_size=1 + self.hidden_size,
-                                               hidden_size=self.hidden_size,
-                                               num_layers=1,
-                                               batch_first=True,
-                                               dropout=0.1)
-
-        self.layer_intensity = CumulHazardFunctionNetwork(model_config)
-
-    def forward(self, time_seqs, time_delta_seqs, type_seqs):
-        """Call the model
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-        # [batch_size, seq_len, hidden_size]
-        type_embedding = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size + 1]
-        rnn_input = torch.cat((type_embedding, time_delta_seqs.unsqueeze(-1)), dim=-1)
-
-        # [batch_size, seq_len, hidden_size]
-        # states right after the event
-        hidden_states, _ = self.layer_rnn(rnn_input)
-
-        integral_lambda, derivative_integral_lambda = self.layer_intensity(hidden_states, time_delta_seqs)
-
-        # [batch_size, num_event_types, seq_len]
-        return integral_lambda, derivative_integral_lambda
-
-    def loglike_loss(self, batch):
-        """Compute the loglike loss.
-
-        Args:
-            batch (tuple, list): batch input.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-        # [batch_size, seq_len]
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
-
-        # [batch_size, seq_len, num_event_types]
-        integral_lambda, derivative_integral_lambda = self.forward(time_seqs[:, :-1],
-                                                                   time_delta_seqs[:, 1:],
-                                                                   type_seqs[:, :-1])
-
-        # [batch_size, seq_len]
-        event_ll = (derivative_integral_lambda + self.eps).log() * batch_non_pad_mask[:, 1:]
-
-        # [batch_size, seq_len]
-        # multiplied by sequence mask
-        non_event_ll = integral_lambda.sum(-1) * batch_non_pad_mask[:, 1:]
-
-        num_events = torch.masked_select(event_ll, event_ll.ne(0.0)).size()[0]
-
-        # return enc_inten to compute accuracy
-        loss = - (event_ll - non_event_ll).sum()
-
-        return loss, num_events
-
-    def compute_intensities_at_sample_times(self,
-                                            time_seqs,
-                                            time_delta_seqs,
-                                            type_seqs,
-                                            sample_dtimes,
-                                            **kwargs):
-        """Compute hidden states at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-        num_samples = sample_dtimes.size()[-1]
-
-        # [batch_size, seq_len, hidden_size, num_samples]
-        type_emb = torch.tile(self.layer_type_emb(type_seqs)[..., None], (1, 1, 1, num_samples))
-
-        # [batch_size, seq_len, hidden_size + 1, num_samples]
-        rnn_input = torch.cat([type_emb, sample_dtimes.unsqueeze(-2)], dim=-2)
-
-        # [batch_size, num_samples， seq_len, hidden_size + 1]
-        rnn_input = torch.permute(rnn_input, (0, 3, 1, 2))
-
-        # [batch_size * num_samples， seq_len, hidden_size + 1]
-        rnn_input = torch.reshape(rnn_input, (-1, rnn_input.size(-2), rnn_input.size(-1)))
-
-        # [batch_size * num_samples, seq_len, hidden_size]
-        # states right after the event
-        hidden_states, _ = self.layer_rnn(rnn_input)
-
-        # [batch_size, num_samples， seq_len, hidden_size]
-        hidden_states = torch.reshape(hidden_states,
-                                      (-1, num_samples, hidden_states.size(-2), hidden_states.size(-1)))
-
-        # [batch_size, seq_len, num_sample, hidden_size]
-        hidden_states = torch.transpose(hidden_states, -2, -3)
-
-        # [batch_size, seq_len, num_samples]
-        _, derivative_integral_lambda = self.layer_intensity(hidden_states, sample_dtimes)
-
-        # FIX: need to fix this later
-        # current version does not truly support multi-event types
-        # [batch_size, seq_len, num_samples, num_event_types]
-        derivative_integral_lambda = torch.tile(derivative_integral_lambda[..., None], (1, 1, 1, self.num_event_types))
-
-        if compute_last_step_only:
-            lambdas = derivative_integral_lambda[:, -1:, :, :]
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = derivative_integral_lambda
-        return lambdas
+import torch
+from torch import nn
+from torch.autograd import grad
+
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class CumulHazardFunctionNetwork(nn.Module):
+    """Cumulative Hazard Function Network
+    ref: https://github.com/wassname/torch-neuralpointprocess
+    """
+
+    def __init__(self, model_config):
+        super(CumulHazardFunctionNetwork, self).__init__()
+        self.hidden_size = model_config.hidden_size
+        self.num_mlp_layers = model_config.model_specs['num_mlp_layers']
+        self.num_event_types = model_config.num_event_types
+
+        # transform inter-event time embedding
+        self.layer_dense_1 = nn.Linear(in_features=1, out_features=self.hidden_size)
+
+        # concat rnn states and inter-event time embedding
+        self.layer_dense_2 = nn.Linear(in_features=self.hidden_size * 2, out_features=self.hidden_size)
+
+        # mlp layers
+        self.module_list = nn.ModuleList(
+            [nn.Linear(in_features=self.hidden_size, out_features=self.hidden_size) for _ in
+             range(self.num_mlp_layers - 1)])
+
+        self.layer_dense_3 = nn.Sequential(nn.Linear(in_features=self.hidden_size,
+                                                     out_features=self.num_event_types),
+                                           nn.Softplus())
+
+        self.params_eps = torch.finfo(torch.float32).eps  # ensure positiveness of parameters
+
+        self.init_weights_positive()
+
+    def init_weights_positive(self):
+        for p in self.parameters():
+            p.data = torch.abs(p.data)
+            p.data = torch.clamp(p.data, min=self.params_eps)
+
+    def forward(self, hidden_states, time_delta_seqs):
+        for p in self.parameters():
+            p.data = torch.clamp(p.data, min=self.params_eps)
+
+        time_delta_seqs.requires_grad_(True)
+
+        # [batch_size, seq_len, hidden_size]
+        t = self.layer_dense_1(time_delta_seqs.unsqueeze(dim=-1))
+
+        # [batch_size, seq_len, hidden_size]
+        out = torch.tanh(self.layer_dense_2(torch.cat([hidden_states, t], dim=-1)))
+        for layer in self.module_list:
+            out = torch.tanh(layer(out))
+
+        # [batch_size, seq_len, num_event_types]
+        integral_lambda = self.layer_dense_3(out)
+
+        # [batch_size, seq_len]
+        derivative_integral_lambda = grad(
+            integral_lambda.sum(dim=-1).mean(),
+            time_delta_seqs,
+            create_graph=True, retain_graph=True)[0]
+
+        return integral_lambda, derivative_integral_lambda
+
+
+class FullyNN(TorchBaseModel):
+    """Torch implementation of
+        Fully Neural Network based Model for General Temporal Point Processes, NeurIPS 2019.
+        https://arxiv.org/abs/1905.09690
+
+        ref: https://github.com/KanghoonYoon/torch-neuralpointprocess/blob/master/module.py;
+            https://github.com/wassname/torch-neuralpointprocess
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(FullyNN, self).__init__(model_config)
+
+        self.rnn_type = model_config.rnn_type
+        self.rnn_list = [nn.LSTM, nn.RNN, nn.GRU]
+        for sub_rnn_class in self.rnn_list:
+            if sub_rnn_class.__name__ == self.rnn_type:
+                self.layer_rnn = sub_rnn_class(input_size=1 + self.hidden_size,
+                                               hidden_size=self.hidden_size,
+                                               num_layers=1,
+                                               batch_first=True,
+                                               dropout=0.1)
+
+        self.layer_intensity = CumulHazardFunctionNetwork(model_config)
+
+    def forward(self, time_seqs, time_delta_seqs, type_seqs):
+        """Call the model
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+        # [batch_size, seq_len, hidden_size]
+        type_embedding = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size + 1]
+        rnn_input = torch.cat((type_embedding, time_delta_seqs.unsqueeze(-1)), dim=-1)
+
+        # [batch_size, seq_len, hidden_size]
+        # states right after the event
+        hidden_states, _ = self.layer_rnn(rnn_input)
+
+        integral_lambda, derivative_integral_lambda = self.layer_intensity(hidden_states, time_delta_seqs)
+
+        # [batch_size, num_event_types, seq_len]
+        return integral_lambda, derivative_integral_lambda
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (tuple, list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+        # [batch_size, seq_len]
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
+
+        # [batch_size, seq_len, num_event_types]
+        integral_lambda, derivative_integral_lambda = self.forward(time_seqs[:, :-1],
+                                                                   time_delta_seqs[:, 1:],
+                                                                   type_seqs[:, :-1])
+
+        # [batch_size, seq_len]
+        event_ll = (derivative_integral_lambda + self.eps).log() * batch_non_pad_mask[:, 1:]
+
+        # [batch_size, seq_len]
+        # multiplied by sequence mask
+        non_event_ll = integral_lambda.sum(-1) * batch_non_pad_mask[:, 1:]
+
+        num_events = torch.masked_select(event_ll, event_ll.ne(0.0)).size()[0]
+
+        # return enc_inten to compute accuracy
+        loss = - (event_ll - non_event_ll).sum()
+
+        return loss, num_events
+
+    def compute_intensities_at_sample_times(self,
+                                            time_seqs,
+                                            time_delta_seqs,
+                                            type_seqs,
+                                            sample_dtimes,
+                                            **kwargs):
+        """Compute hidden states at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+        num_samples = sample_dtimes.size()[-1]
+
+        # [batch_size, seq_len, hidden_size, num_samples]
+        type_emb = torch.tile(self.layer_type_emb(type_seqs)[..., None], (1, 1, 1, num_samples))
+
+        # [batch_size, seq_len, hidden_size + 1, num_samples]
+        rnn_input = torch.cat([type_emb, sample_dtimes.unsqueeze(-2)], dim=-2)
+
+        # [batch_size, num_samples， seq_len, hidden_size + 1]
+        rnn_input = torch.permute(rnn_input, (0, 3, 1, 2))
+
+        # [batch_size * num_samples， seq_len, hidden_size + 1]
+        rnn_input = torch.reshape(rnn_input, (-1, rnn_input.size(-2), rnn_input.size(-1)))
+
+        # [batch_size * num_samples, seq_len, hidden_size]
+        # states right after the event
+        hidden_states, _ = self.layer_rnn(rnn_input)
+
+        # [batch_size, num_samples， seq_len, hidden_size]
+        hidden_states = torch.reshape(hidden_states,
+                                      (-1, num_samples, hidden_states.size(-2), hidden_states.size(-1)))
+
+        # [batch_size, seq_len, num_sample, hidden_size]
+        hidden_states = torch.transpose(hidden_states, -2, -3)
+
+        # [batch_size, seq_len, num_samples]
+        _, derivative_integral_lambda = self.layer_intensity(hidden_states, sample_dtimes)
+
+        # FIX: need to fix this later
+        # current version does not truly support multi-event types
+        # [batch_size, seq_len, num_samples, num_event_types]
+        derivative_integral_lambda = torch.tile(derivative_integral_lambda[..., None], (1, 1, 1, self.num_event_types))
+
+        if compute_last_step_only:
+            lambdas = derivative_integral_lambda[:, -1:, :, :]
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = derivative_integral_lambda
+        return lambdas
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_nhp.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_nhp.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,355 +1,355 @@
-import torch
-from torch import nn
-
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-
-
-class ContTimeLSTMCell(nn.Module):
-    """LSTM Cell in Neural Hawkes Process, NeurIPS'17.
-    """
-
-    def __init__(self, hidden_dim, beta=1.0):
-        """Initialize the continuous LSTM cell.
-
-        Args:
-            hidden_dim (int): dim of hidden state.
-            beta (float, optional): beta in nn.Softplus. Defaults to 1.0.
-        """
-        super(ContTimeLSTMCell, self).__init__()
-        self.hidden_dim = hidden_dim
-        self.init_dense_layer(hidden_dim, bias=True, beta=beta)
-
-    def init_dense_layer(self, hidden_dim, bias, beta):
-        """Initialize linear layers given Equations (5a-6c) in the paper.
-
-        Args:
-            hidden_dim (int): dim of hidden state.
-            bias (bool): whether to use bias term in nn.Linear.
-            beta (float): beta in nn.Softplus.
-        """
-
-        self.layer_input = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
-        self.layer_forget = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
-        self.layer_output = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
-        self.layer_input_bar = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
-        self.layer_forget_bar = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
-        self.layer_pre_c = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
-        self.layer_decay = nn.Sequential(
-            nn.Linear(hidden_dim * 2, hidden_dim, bias=bias),
-            nn.Softplus(beta=beta))
-
-    def forward(self, x_i, hidden_i_minus, cell_i_minus, cell_bar_i_minus_1):
-        """Update the continuous-time LSTM cell.
-
-        Args:
-            x_i (tensor): event embedding vector at t_i.
-            hidden_i_minus (tensor): hidden state at t_i-
-            cell_i_minus (tensor): cell state at t_i-
-            cell_bar_i_minus_1 (tensor): cell bar state at t_{i-1}
-
-        Returns:
-            list: cell state, cell bar state, decay and output at t_i
-        """
-
-        x_i_ = torch.cat((x_i, hidden_i_minus), dim=1)
-
-        # update input gate - Equation (5a)
-        gate_input = torch.nn.Sigmoid()(self.layer_input(x_i_))
-
-        # update forget gate - Equation (5b)
-        gate_forget = torch.nn.Sigmoid()(self.layer_forget(x_i_))
-
-        # update output gate - Equation (5d)
-        gate_output = torch.nn.Sigmoid()(self.layer_output(x_i_))
-
-        # update input bar - similar to Equation (5a)
-        gate_input_bar = torch.nn.Sigmoid()(self.layer_input_bar(x_i_))
-
-        # update forget bar - similar to Equation (5b)
-        gate_forget_bar = torch.nn.Sigmoid()(self.layer_forget_bar(x_i_))
-
-        # update gate z - Equation (5c)
-        gate_pre_c = torch.tanh(self.layer_pre_c(x_i_))
-
-        # update gate decay - Equation (6c)
-        gate_decay = self.layer_decay(x_i_)
-
-        # update cell state to t_i+ - Equation (6a)
-        cell_i = gate_forget * cell_i_minus + gate_input * gate_pre_c
-
-        # update cell state bar - Equation (6b)
-        cell_bar_i = gate_forget_bar * cell_bar_i_minus_1 + gate_input_bar * gate_pre_c
-
-        return cell_i, cell_bar_i, gate_decay, gate_output
-
-    def decay(self, cell_i, cell_bar_i, gate_decay, gate_output, dtime):
-        """Cell and hidden state decay according to Equation (7).
-
-        Args:
-            cell_i (tensor): cell state at t_i.
-            cell_bar_i (tensor): cell bar state at t_i.
-            gate_decay (tensor): gate decay state at t_i.
-            gate_output (tensor): gate output state at t_i.
-            dtime (tensor): delta time to decay.
-
-        Returns:
-            list: list of cell and hidden state tensors after the decay.
-        """
-        c_t = cell_bar_i + (cell_i - cell_bar_i) * torch.exp(-gate_decay * dtime)
-
-        h_t = gate_output * torch.tanh(c_t)
-
-        return c_t, h_t
-
-
-class NHP(TorchBaseModel):
-    """Torch implementation of The Neural Hawkes Process: A Neurally Self-Modulating Multivariate Point Process,
-       NeurIPS 2017, https://arxiv.org/abs/1612.09328.
-    """
-
-    def __init__(self, model_config):
-        """Initialize the NHP model.
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(NHP, self).__init__(model_config)
-        self.beta = model_config.model_specs.get('beta', 1.0)
-        self.bias = model_config.model_specs.get('bias', False)
-        self.rnn_cell = ContTimeLSTMCell(self.hidden_size)
-
-        self.layer_intensity = nn.Sequential(
-            nn.Linear(self.hidden_size, self.num_event_types, self.bias),
-            nn.Softplus(self.beta))
-
-    def init_state(self, batch_size):
-        """Initialize hidden and cell states.
-
-        Args:
-            batch_size (int): size of batch data.
-
-        Returns:
-            list: list of hidden states, cell states and cell bar states.
-        """
-        h_t, c_t, c_bar = torch.zeros(batch_size,
-                                      3 * self.hidden_size).chunk(3, dim=1)
-        return h_t, c_t, c_bar
-
-    def forward(self, batch, **kwargs):
-        """Call the model.
-
-        Args:
-            batch (tuple, list): batch input.
-
-        Returns:
-            list: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens;
-                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
-                  the event happens.
-        """
-        time_seq, time_delta_seq, event_seq, batch_non_pad_mask, _, type_mask = batch
-
-        all_hiddens = []
-        all_outputs = []
-        all_cells = []
-        all_cell_bars = []
-        all_decays = []
-
-        max_steps = kwargs.get('max_steps', None)
-
-        max_decay_time = kwargs.get('max_decay_time', 5.0)
-
-        # last event has no time label
-        max_seq_length = max_steps if max_steps is not None else event_seq.size(1) - 1
-
-        batch_size = len(event_seq)
-        h_t, c_t, c_bar_i = self.init_state(batch_size)
-
-        # if only one event, then we dont decay
-        if max_seq_length == 1:
-            types_sub_batch = event_seq[:, 0]
-            x_t = self.layer_type_emb(types_sub_batch)
-            cell_i, c_bar_i, decay_i, output_i = \
-                self.rnn_cell(x_t, h_t, c_t, c_bar_i)
-
-            # Append all output
-            all_outputs.append(output_i)
-            all_decays.append(decay_i)
-            all_cells.append(cell_i)
-            all_cell_bars.append(c_bar_i)
-            all_hiddens.append(h_t)
-        else:
-            # Loop over all events
-            for i in range(max_seq_length):
-                if i == event_seq.size(1) - 1:
-                    dt = torch.ones_like(time_delta_seq[:, i]) * max_decay_time
-                else:
-                    dt = time_delta_seq[:, i + 1]  # need to carefully check here
-                types_sub_batch = event_seq[:, i]
-                x_t = self.layer_type_emb(types_sub_batch)
-
-                # cell_i  (batch_size, process_dim)
-                cell_i, c_bar_i, decay_i, output_i = \
-                    self.rnn_cell(x_t, h_t, c_t, c_bar_i)
-
-                # States decay - Equation (7) in the paper
-                c_t, h_t = self.rnn_cell.decay(cell_i,
-                                               c_bar_i,
-                                               decay_i,
-                                               output_i,
-                                               dt[:, None])
-
-                # Append all output
-                all_outputs.append(output_i)
-                all_decays.append(decay_i)
-                all_cells.append(cell_i)
-                all_cell_bars.append(c_bar_i)
-                all_hiddens.append(h_t)
-
-        # (batch_size, max_seq_length, hidden_dim)
-        cell_stack = torch.stack(all_cells, dim=1)
-        cell_bar_stack = torch.stack(all_cell_bars, dim=1)
-        decay_stack = torch.stack(all_decays, dim=1)
-        output_stack = torch.stack(all_outputs, dim=1)
-
-        # [batch_size, max_seq_length, hidden_dim]
-        hiddens_stack = torch.stack(all_hiddens, dim=1)
-
-        # [batch_size, max_seq_length, 4, hidden_dim]
-        decay_states_stack = torch.stack((cell_stack,
-                                          cell_bar_stack,
-                                          decay_stack,
-                                          output_stack),
-                                         dim=2)
-
-        return hiddens_stack, decay_states_stack
-
-    def loglike_loss(self, batch):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
-
-        hiddens_ti, decay_states = self.forward(batch)
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = hiddens_ti.size()
-
-        # Lambda(t) right before each event time point
-        # lambda_at_event - [batch_size, num_times=max_len-1, num_event_types]
-        # Here we drop the last event because it has no delta_time label (can not decay)
-        lambda_at_event = self.layer_intensity(hiddens_ti)
-
-        # Compute the big lambda integral in Equation (8)
-        # 1 - take num_mc_sample rand points in each event interval
-        # 2 - compute its lambda value for every sample point
-        # 3 - take average of these sample points
-        # 4 - times the interval length
-
-        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seq[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample, hidden_size]
-        state_t_sample = self.compute_states_at_sample_times(decay_states, interval_t_sample)
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample, event_num]
-        lambda_t_sample = self.layer_intensity(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=time_delta_seqs[:, 1:],
-                                                                        seq_mask=batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=type_mask[:, 1:])
-
-        # (num_samples, num_times)
-        loss = - (event_ll - non_event_ll).sum()
-        return loss, num_events
-
-    def compute_states_at_sample_times(self, decay_states, sample_dtimes):
-        """Compute the states at sampling times.
-
-        Args:
-            decay_states (tensor): states right after the events.
-            sample_dtimes (tensor): delta times in sampling.
-
-        Returns:
-            tensor: hiddens states at sampling times.
-        """
-        # update the states given last event
-        # cells (batch_size, num_times, hidden_dim)
-        cells, cell_bars, decays, outputs = decay_states.unbind(dim=-2)
-
-        # Use broadcasting to compute the decays at all time steps
-        # at all sample points
-        # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
-        # cells[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
-        _, h_ts = self.rnn_cell.decay(cells[:, :, None, :],
-                                      cell_bars[:, :, None, :],
-                                      decays[:, :, None, :],
-                                      outputs[:, :, None, :],
-                                      sample_dtimes[..., None])
-
-        return h_ts
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
-        """Compute the intensity at sampled times, not only event times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
-                    intensity at each timestamp for each event type.
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        input_ = time_seqs, time_delta_seqs, type_seqs, None, None, None
-
-        # forward to the last but one event
-        hiddens_ti, decay_states = self.forward(input_, **kwargs)
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = hiddens_ti.size()
-
-        # update the states given last event
-        # cells (batch_size, num_times, hidden_dim)
-        cells, cell_bars, decays, outputs = decay_states.unbind(dim=-2)
-
-        if compute_last_step_only:
-            interval_t_sample = sample_dtimes[:, -1:, :, None]
-            _, h_ts = self.rnn_cell.decay(cells[:, -1:, None, :],
-                                          cell_bars[:, -1:, None, :],
-                                          decays[:, -1:, None, :],
-                                          outputs[:, -1:, None, :],
-                                          interval_t_sample)
-
-            # [batch_size, 1, num_mc_sample, num_event_types]
-            sampled_intensities = self.layer_intensity(h_ts)
-
-        else:
-            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
-            interval_t_sample = sample_dtimes[..., None]
-            # Use broadcasting to compute the decays at all time steps
-            # at all sample points
-            # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
-            # cells[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
-            _, h_ts = self.rnn_cell.decay(cells[:, :, None, :],
-                                          cell_bars[:, :, None, :],
-                                          decays[:, :, None, :],
-                                          outputs[:, :, None, :],
-                                          interval_t_sample)
-
-            # [batch_size, num_times, num_mc_sample, num_event_types]
-            sampled_intensities = self.layer_intensity(h_ts)
-
-        return sampled_intensities
+import torch
+from torch import nn
+
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class ContTimeLSTMCell(nn.Module):
+    """LSTM Cell in Neural Hawkes Process, NeurIPS'17.
+    """
+
+    def __init__(self, hidden_dim, beta=1.0):
+        """Initialize the continuous LSTM cell.
+
+        Args:
+            hidden_dim (int): dim of hidden state.
+            beta (float, optional): beta in nn.Softplus. Defaults to 1.0.
+        """
+        super(ContTimeLSTMCell, self).__init__()
+        self.hidden_dim = hidden_dim
+        self.init_dense_layer(hidden_dim, bias=True, beta=beta)
+
+    def init_dense_layer(self, hidden_dim, bias, beta):
+        """Initialize linear layers given Equations (5a-6c) in the paper.
+
+        Args:
+            hidden_dim (int): dim of hidden state.
+            bias (bool): whether to use bias term in nn.Linear.
+            beta (float): beta in nn.Softplus.
+        """
+
+        self.layer_input = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
+        self.layer_forget = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
+        self.layer_output = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
+        self.layer_input_bar = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
+        self.layer_forget_bar = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
+        self.layer_pre_c = nn.Linear(hidden_dim * 2, hidden_dim, bias=bias)
+        self.layer_decay = nn.Sequential(
+            nn.Linear(hidden_dim * 2, hidden_dim, bias=bias),
+            nn.Softplus(beta=beta))
+
+    def forward(self, x_i, hidden_i_minus, cell_i_minus, cell_bar_i_minus_1):
+        """Update the continuous-time LSTM cell.
+
+        Args:
+            x_i (tensor): event embedding vector at t_i.
+            hidden_i_minus (tensor): hidden state at t_i-
+            cell_i_minus (tensor): cell state at t_i-
+            cell_bar_i_minus_1 (tensor): cell bar state at t_{i-1}
+
+        Returns:
+            list: cell state, cell bar state, decay and output at t_i
+        """
+
+        x_i_ = torch.cat((x_i, hidden_i_minus), dim=1)
+
+        # update input gate - Equation (5a)
+        gate_input = torch.nn.Sigmoid()(self.layer_input(x_i_))
+
+        # update forget gate - Equation (5b)
+        gate_forget = torch.nn.Sigmoid()(self.layer_forget(x_i_))
+
+        # update output gate - Equation (5d)
+        gate_output = torch.nn.Sigmoid()(self.layer_output(x_i_))
+
+        # update input bar - similar to Equation (5a)
+        gate_input_bar = torch.nn.Sigmoid()(self.layer_input_bar(x_i_))
+
+        # update forget bar - similar to Equation (5b)
+        gate_forget_bar = torch.nn.Sigmoid()(self.layer_forget_bar(x_i_))
+
+        # update gate z - Equation (5c)
+        gate_pre_c = torch.tanh(self.layer_pre_c(x_i_))
+
+        # update gate decay - Equation (6c)
+        gate_decay = self.layer_decay(x_i_)
+
+        # update cell state to t_i+ - Equation (6a)
+        cell_i = gate_forget * cell_i_minus + gate_input * gate_pre_c
+
+        # update cell state bar - Equation (6b)
+        cell_bar_i = gate_forget_bar * cell_bar_i_minus_1 + gate_input_bar * gate_pre_c
+
+        return cell_i, cell_bar_i, gate_decay, gate_output
+
+    def decay(self, cell_i, cell_bar_i, gate_decay, gate_output, dtime):
+        """Cell and hidden state decay according to Equation (7).
+
+        Args:
+            cell_i (tensor): cell state at t_i.
+            cell_bar_i (tensor): cell bar state at t_i.
+            gate_decay (tensor): gate decay state at t_i.
+            gate_output (tensor): gate output state at t_i.
+            dtime (tensor): delta time to decay.
+
+        Returns:
+            list: list of cell and hidden state tensors after the decay.
+        """
+        c_t = cell_bar_i + (cell_i - cell_bar_i) * torch.exp(-gate_decay * dtime)
+
+        h_t = gate_output * torch.tanh(c_t)
+
+        return c_t, h_t
+
+
+class NHP(TorchBaseModel):
+    """Torch implementation of The Neural Hawkes Process: A Neurally Self-Modulating Multivariate Point Process,
+       NeurIPS 2017, https://arxiv.org/abs/1612.09328.
+    """
+
+    def __init__(self, model_config):
+        """Initialize the NHP model.
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(NHP, self).__init__(model_config)
+        self.beta = model_config.model_specs.get('beta', 1.0)
+        self.bias = model_config.model_specs.get('bias', False)
+        self.rnn_cell = ContTimeLSTMCell(self.hidden_size)
+
+        self.layer_intensity = nn.Sequential(
+            nn.Linear(self.hidden_size, self.num_event_types, self.bias),
+            nn.Softplus(self.beta))
+
+    def init_state(self, batch_size):
+        """Initialize hidden and cell states.
+
+        Args:
+            batch_size (int): size of batch data.
+
+        Returns:
+            list: list of hidden states, cell states and cell bar states.
+        """
+        h_t, c_t, c_bar = torch.zeros(batch_size,
+                                      3 * self.hidden_size).chunk(3, dim=1)
+        return h_t, c_t, c_bar
+
+    def forward(self, batch, **kwargs):
+        """Call the model.
+
+        Args:
+            batch (tuple, list): batch input.
+
+        Returns:
+            list: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens;
+                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
+                  the event happens.
+        """
+        time_seq, time_delta_seq, event_seq, batch_non_pad_mask, _, type_mask = batch
+
+        all_hiddens = []
+        all_outputs = []
+        all_cells = []
+        all_cell_bars = []
+        all_decays = []
+
+        max_steps = kwargs.get('max_steps', None)
+
+        max_decay_time = kwargs.get('max_decay_time', 5.0)
+
+        # last event has no time label
+        max_seq_length = max_steps if max_steps is not None else event_seq.size(1) - 1
+
+        batch_size = len(event_seq)
+        h_t, c_t, c_bar_i = self.init_state(batch_size)
+
+        # if only one event, then we dont decay
+        if max_seq_length == 1:
+            types_sub_batch = event_seq[:, 0]
+            x_t = self.layer_type_emb(types_sub_batch)
+            cell_i, c_bar_i, decay_i, output_i = \
+                self.rnn_cell(x_t, h_t, c_t, c_bar_i)
+
+            # Append all output
+            all_outputs.append(output_i)
+            all_decays.append(decay_i)
+            all_cells.append(cell_i)
+            all_cell_bars.append(c_bar_i)
+            all_hiddens.append(h_t)
+        else:
+            # Loop over all events
+            for i in range(max_seq_length):
+                if i == event_seq.size(1) - 1:
+                    dt = torch.ones_like(time_delta_seq[:, i]) * max_decay_time
+                else:
+                    dt = time_delta_seq[:, i + 1]  # need to carefully check here
+                types_sub_batch = event_seq[:, i]
+                x_t = self.layer_type_emb(types_sub_batch)
+
+                # cell_i  (batch_size, process_dim)
+                cell_i, c_bar_i, decay_i, output_i = \
+                    self.rnn_cell(x_t, h_t, c_t, c_bar_i)
+
+                # States decay - Equation (7) in the paper
+                c_t, h_t = self.rnn_cell.decay(cell_i,
+                                               c_bar_i,
+                                               decay_i,
+                                               output_i,
+                                               dt[:, None])
+
+                # Append all output
+                all_outputs.append(output_i)
+                all_decays.append(decay_i)
+                all_cells.append(cell_i)
+                all_cell_bars.append(c_bar_i)
+                all_hiddens.append(h_t)
+
+        # (batch_size, max_seq_length, hidden_dim)
+        cell_stack = torch.stack(all_cells, dim=1)
+        cell_bar_stack = torch.stack(all_cell_bars, dim=1)
+        decay_stack = torch.stack(all_decays, dim=1)
+        output_stack = torch.stack(all_outputs, dim=1)
+
+        # [batch_size, max_seq_length, hidden_dim]
+        hiddens_stack = torch.stack(all_hiddens, dim=1)
+
+        # [batch_size, max_seq_length, 4, hidden_dim]
+        decay_states_stack = torch.stack((cell_stack,
+                                          cell_bar_stack,
+                                          decay_stack,
+                                          output_stack),
+                                         dim=2)
+
+        return hiddens_stack, decay_states_stack
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
+
+        hiddens_ti, decay_states = self.forward(batch)
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = hiddens_ti.size()
+
+        # Lambda(t) right before each event time point
+        # lambda_at_event - [batch_size, num_times=max_len-1, num_event_types]
+        # Here we drop the last event because it has no delta_time label (can not decay)
+        lambda_at_event = self.layer_intensity(hiddens_ti)
+
+        # Compute the big lambda integral in Equation (8)
+        # 1 - take num_mc_sample rand points in each event interval
+        # 2 - compute its lambda value for every sample point
+        # 3 - take average of these sample points
+        # 4 - times the interval length
+
+        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seq[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample, hidden_size]
+        state_t_sample = self.compute_states_at_sample_times(decay_states, interval_t_sample)
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample, event_num]
+        lambda_t_sample = self.layer_intensity(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        # (num_samples, num_times)
+        loss = - (event_ll - non_event_ll).sum()
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, decay_states, sample_dtimes):
+        """Compute the states at sampling times.
+
+        Args:
+            decay_states (tensor): states right after the events.
+            sample_dtimes (tensor): delta times in sampling.
+
+        Returns:
+            tensor: hiddens states at sampling times.
+        """
+        # update the states given last event
+        # cells (batch_size, num_times, hidden_dim)
+        cells, cell_bars, decays, outputs = decay_states.unbind(dim=-2)
+
+        # Use broadcasting to compute the decays at all time steps
+        # at all sample points
+        # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
+        # cells[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
+        _, h_ts = self.rnn_cell.decay(cells[:, :, None, :],
+                                      cell_bars[:, :, None, :],
+                                      decays[:, :, None, :],
+                                      outputs[:, :, None, :],
+                                      sample_dtimes[..., None])
+
+        return h_ts
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
+        """Compute the intensity at sampled times, not only event times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
+                    intensity at each timestamp for each event type.
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        input_ = time_seqs, time_delta_seqs, type_seqs, None, None, None
+
+        # forward to the last but one event
+        hiddens_ti, decay_states = self.forward(input_, **kwargs)
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = hiddens_ti.size()
+
+        # update the states given last event
+        # cells (batch_size, num_times, hidden_dim)
+        cells, cell_bars, decays, outputs = decay_states.unbind(dim=-2)
+
+        if compute_last_step_only:
+            interval_t_sample = sample_dtimes[:, -1:, :, None]
+            _, h_ts = self.rnn_cell.decay(cells[:, -1:, None, :],
+                                          cell_bars[:, -1:, None, :],
+                                          decays[:, -1:, None, :],
+                                          outputs[:, -1:, None, :],
+                                          interval_t_sample)
+
+            # [batch_size, 1, num_mc_sample, num_event_types]
+            sampled_intensities = self.layer_intensity(h_ts)
+
+        else:
+            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
+            interval_t_sample = sample_dtimes[..., None]
+            # Use broadcasting to compute the decays at all time steps
+            # at all sample points
+            # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
+            # cells[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
+            _, h_ts = self.rnn_cell.decay(cells[:, :, None, :],
+                                          cell_bars[:, :, None, :],
+                                          decays[:, :, None, :],
+                                          outputs[:, :, None, :],
+                                          interval_t_sample)
+
+            # [batch_size, num_times, num_mc_sample, num_event_types]
+            sampled_intensities = self.layer_intensity(h_ts)
+
+        return sampled_intensities
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_ode_tpp.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_ode_tpp.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,296 +1,296 @@
-import torch
-from torch import nn
-
-from easy_tpp.model.torch_model.torch_baselayer import DNN
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-from easy_tpp.utils import rk4_step_method
-
-
-def flatten_parameters(model):
-    p_shapes = []
-    flat_parameters = []
-    for p in model.parameters():
-        p_shapes.append(p.size())
-        flat_parameters.append(p.flatten())
-    return torch.cat(flat_parameters)
-
-
-class NeuralODEAdjoint(torch.autograd.Function):
-    @staticmethod
-    def forward(ctx, z_init, delta_t, ode_fn, solver, num_sample_times, *model_parameters):
-        """
-
-        Args:
-            ctx:
-            input: (tensor): [batch_size]
-            model:
-            solver:
-            delta_t (tensor): [batch_size, num_sample_times]
-
-        Returns:
-
-        """
-
-        ctx.ode_fn = ode_fn
-        ctx.solver = solver
-        ctx.delta_t = delta_t
-        ctx.model_parameters = model_parameters
-        ctx.num_sample_times = num_sample_times
-
-        total_state = []
-        dt_ratio = 1.0 / num_sample_times
-        delta_t = delta_t * dt_ratio
-        with torch.no_grad():
-            state = z_init
-            for i in range(num_sample_times):
-                # [batch_size, hidden_size]
-                state = solver(diff_func=ode_fn, dt=delta_t, z0=state)
-                total_state.append(state)
-
-        # [batch_size, num_samples, hidden_size]
-        ctx.save_for_backward(state)
-
-        return state
-
-    @staticmethod
-    def backward(ctx, grad_z):
-        output_state = ctx.saved_tensors[0]  # return a tuple
-        ode_fn = ctx.ode_fn
-        solver = ctx.solver
-        delta_t = ctx.delta_t
-        model_parameters = ctx.model_parameters
-        num_sample_times = ctx.num_sample_times
-
-        # Dynamics of augmented system to be calculated backwards in time
-        def aug_dynamics(aug_states):
-            tmp_z = aug_states[0]
-            tmp_neg_a = -aug_states[1]
-
-            with torch.set_grad_enabled(True):
-                tmp_z = tmp_z.detach().requires_grad_(True)
-                func_eval = ode_fn(tmp_z)
-                tmp_ds = torch.autograd.grad(
-                    (func_eval,), (tmp_z, *model_parameters),
-                    grad_outputs=tmp_neg_a,
-                    allow_unused=True,
-                    retain_graph=True)
-
-            neg_adfdz = tmp_ds[0]
-            neg_adfdtheta = [torch.flatten(var) for var in tmp_ds[1:]]
-
-            return [func_eval, neg_adfdz, *neg_adfdtheta]
-
-        dt_ratio = 1.0 / num_sample_times
-        delta_t = delta_t * dt_ratio
-
-        with torch.no_grad():
-            # Construct back-state for ode solver
-            # reshape variable \theta for batch solving
-            init_var_grad = [torch.zeros_like(torch.flatten(var)) for var in model_parameters]
-
-            # [z(t_1), a(t_1), \theta]
-            z1 = output_state
-            a1 = grad_z
-            states = [z1, a1, *init_var_grad]
-
-            for i in range(num_sample_times):
-                states = solver(aug_dynamics, -delta_t, states)
-
-            grad_z0 = states[1]
-
-            grad_theta = [torch.reshape(torch.mean(var_grad, dim=0), var.shape) for var, var_grad in
-                          zip(model_parameters, states[2:])]
-
-        return (grad_z0, None, None, None, None, *grad_theta)
-
-
-class NeuralODE(nn.Module):
-    def __init__(self, model, solver, num_sample_times):
-        super().__init__()
-        self.model = model
-        self.solver = solver
-        self.params = [w for w in model.parameters()]
-        self.num_sample_times = num_sample_times
-
-    def forward(self, input_state, delta_time):
-        """
-
-        Args:
-            input_state: [batch_size, hidden_size]
-            return_state:
-
-        Returns:
-
-        """
-        output_state = NeuralODEAdjoint.apply(input_state,
-                                              delta_time,
-                                              self.model,
-                                              self.solver,
-                                              self.num_sample_times,
-                                              *self.params)
-
-        # [batch_size, num_sample_times, hidden_size]
-        return output_state
-
-
-class ODETPP(TorchBaseModel):
-    """Torch implementation of a TPP with Neural ODE state evolution, which is a simplified version of TPP in
-    https://arxiv.org/abs/2011.04583, ICLR 2021
-
-    code reference: https://msurtsukov.github.io/Neural-ODE/;
-    https://github.com/liruilong940607/NeuralODE/blob/master/NeuralODE.py
-
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(ODETPP, self).__init__(model_config)
-
-        self.layer_intensity = nn.Sequential(
-            nn.Linear(self.hidden_size, self.num_event_types),
-            nn.Softplus())
-
-        self.event_model = DNN(inputs_dim=self.hidden_size,
-                               hidden_size=[self.hidden_size])
-
-        self.ode_num_sample_per_step = model_config.model_specs['ode_num_sample_per_step']
-        self.time_factor = model_config.model_specs['time_factor']
-
-        self.solver = rk4_step_method
-
-        self.layer_neural_ode = NeuralODE(model=self.event_model,
-                                          solver=self.solver,
-                                          num_sample_times=self.ode_num_sample_per_step)
-
-    def forward(self, time_delta_seqs, type_seqs, **kwargs):
-        """Call the model.
-
-        Args:
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-
-        Returns:
-            tensor: hidden states at event times.
-
-        """
-        # [batch_size, seq_len=max_len-1, hidden_size]
-        type_seq_emb = self.layer_type_emb(type_seqs)
-        time_delta_seqs_ = time_delta_seqs[..., None]
-
-        total_state_at_event_minus = []
-        total_state_at_event_plus = []
-        last_state = torch.zeros_like(type_seq_emb[:, 0, :])
-        for type_emb, dt in zip(torch.unbind(type_seq_emb, dim=-2),
-                                torch.unbind(time_delta_seqs_, dim=-2)):
-            dt = dt / self.time_factor
-            last_state = self.layer_neural_ode(last_state + type_emb, dt)
-            total_state_at_event_minus.append(last_state)
-            total_state_at_event_plus.append(last_state + type_emb)
-
-        # [batch_size, seq_len, hidden_size]
-        state_ti = torch.stack(total_state_at_event_minus, dim=1)
-
-        # [batch_size, seq_len, hidden_size]
-        state_to_evolve = torch.stack(total_state_at_event_plus, dim=1)
-
-        return state_ti, state_to_evolve
-
-    def loglike_loss(self, batch):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
-
-        state_ti, state_ti_plus = self.forward(time_delta_seqs[:, 1:], type_seqs[:, :-1])
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = state_ti.size()
-
-        # Lambda(t) right before each event time point
-        # lambda_at_event - [batch_size, num_times=max_len-1, num_event_types]
-        # Here we drop the last event because it has no delta_time label (can not decay)
-        lambda_at_event = self.layer_intensity(state_ti)
-
-        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seq[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample, hidden_size]
-        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, interval_t_sample)
-
-        # [batch_size, num_times = max_len - 1, num_mc_sample, event_num]
-        lambda_t_sample = self.layer_intensity(sample_state_ti)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=time_delta_seqs[:, 1:],
-                                                                        seq_mask=batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=type_mask[:, 1:])
-
-        loss = - (event_ll - non_event_ll).sum()
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self, state_ti_plus, sample_dtimes):
-        """Compute the states at sampling times.
-
-        Args:
-            state_ti_plus (tensor): [batch_size, seq_len, hidden_size], states right after the events.
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples], delta times in sampling.
-
-        Returns:
-            tensor: hiddens states at sampling times.
-        """
-
-        # Use broadcasting to compute the decays at all time steps
-        # at all sample points
-        # h_ts shape (batch_size, seq_len, num_samples, hidden_dim)
-        state = self.solver(diff_func=self.event_model,
-                            dt=sample_dtimes[..., None],  # [batch_size, seq_len, num_samples, 1]
-                            z0=state_ti_plus[..., None, :])  # [batch_size, seq_len, 1, hidden_size]
-
-        return state
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
-        """Compute the intensity at sampled times, not only event times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
-                    intensity at each timestamp for each event type.
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        # forward to the last but one event
-        state_ti, state_ti_plus = self.forward(time_delta_seqs, type_seqs, **kwargs)
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = state_ti.size()
-
-        # [batch_size, num_sample_times, num_mc_sample, hidden_size]
-        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, sample_dtimes)
-
-        if compute_last_step_only:
-            # [batch_size, 1, num_mc_sample, num_event_types]
-            sampled_intensities = self.layer_intensity(sample_state_ti[:, -1:, :, :])
-        else:
-            # [batch_size, num_sample_times, num_mc_sample, num_event_types]
-            sampled_intensities = self.layer_intensity(sample_state_ti)
-
-        return sampled_intensities
+import torch
+from torch import nn
+
+from easy_tpp.model.torch_model.torch_baselayer import DNN
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+from easy_tpp.utils import rk4_step_method
+
+
+def flatten_parameters(model):
+    p_shapes = []
+    flat_parameters = []
+    for p in model.parameters():
+        p_shapes.append(p.size())
+        flat_parameters.append(p.flatten())
+    return torch.cat(flat_parameters)
+
+
+class NeuralODEAdjoint(torch.autograd.Function):
+    @staticmethod
+    def forward(ctx, z_init, delta_t, ode_fn, solver, num_sample_times, *model_parameters):
+        """
+
+        Args:
+            ctx:
+            input: (tensor): [batch_size]
+            model:
+            solver:
+            delta_t (tensor): [batch_size, num_sample_times]
+
+        Returns:
+
+        """
+
+        ctx.ode_fn = ode_fn
+        ctx.solver = solver
+        ctx.delta_t = delta_t
+        ctx.model_parameters = model_parameters
+        ctx.num_sample_times = num_sample_times
+
+        total_state = []
+        dt_ratio = 1.0 / num_sample_times
+        delta_t = delta_t * dt_ratio
+        with torch.no_grad():
+            state = z_init
+            for i in range(num_sample_times):
+                # [batch_size, hidden_size]
+                state = solver(diff_func=ode_fn, dt=delta_t, z0=state)
+                total_state.append(state)
+
+        # [batch_size, num_samples, hidden_size]
+        ctx.save_for_backward(state)
+
+        return state
+
+    @staticmethod
+    def backward(ctx, grad_z):
+        output_state = ctx.saved_tensors[0]  # return a tuple
+        ode_fn = ctx.ode_fn
+        solver = ctx.solver
+        delta_t = ctx.delta_t
+        model_parameters = ctx.model_parameters
+        num_sample_times = ctx.num_sample_times
+
+        # Dynamics of augmented system to be calculated backwards in time
+        def aug_dynamics(aug_states):
+            tmp_z = aug_states[0]
+            tmp_neg_a = -aug_states[1]
+
+            with torch.set_grad_enabled(True):
+                tmp_z = tmp_z.detach().requires_grad_(True)
+                func_eval = ode_fn(tmp_z)
+                tmp_ds = torch.autograd.grad(
+                    (func_eval,), (tmp_z, *model_parameters),
+                    grad_outputs=tmp_neg_a,
+                    allow_unused=True,
+                    retain_graph=True)
+
+            neg_adfdz = tmp_ds[0]
+            neg_adfdtheta = [torch.flatten(var) for var in tmp_ds[1:]]
+
+            return [func_eval, neg_adfdz, *neg_adfdtheta]
+
+        dt_ratio = 1.0 / num_sample_times
+        delta_t = delta_t * dt_ratio
+
+        with torch.no_grad():
+            # Construct back-state for ode solver
+            # reshape variable \theta for batch solving
+            init_var_grad = [torch.zeros_like(torch.flatten(var)) for var in model_parameters]
+
+            # [z(t_1), a(t_1), \theta]
+            z1 = output_state
+            a1 = grad_z
+            states = [z1, a1, *init_var_grad]
+
+            for i in range(num_sample_times):
+                states = solver(aug_dynamics, -delta_t, states)
+
+            grad_z0 = states[1]
+
+            grad_theta = [torch.reshape(torch.mean(var_grad, dim=0), var.shape) for var, var_grad in
+                          zip(model_parameters, states[2:])]
+
+        return (grad_z0, None, None, None, None, *grad_theta)
+
+
+class NeuralODE(nn.Module):
+    def __init__(self, model, solver, num_sample_times):
+        super().__init__()
+        self.model = model
+        self.solver = solver
+        self.params = [w for w in model.parameters()]
+        self.num_sample_times = num_sample_times
+
+    def forward(self, input_state, delta_time):
+        """
+
+        Args:
+            input_state: [batch_size, hidden_size]
+            return_state:
+
+        Returns:
+
+        """
+        output_state = NeuralODEAdjoint.apply(input_state,
+                                              delta_time,
+                                              self.model,
+                                              self.solver,
+                                              self.num_sample_times,
+                                              *self.params)
+
+        # [batch_size, num_sample_times, hidden_size]
+        return output_state
+
+
+class ODETPP(TorchBaseModel):
+    """Torch implementation of a TPP with Neural ODE state evolution, which is a simplified version of TPP in
+    https://arxiv.org/abs/2011.04583, ICLR 2021
+
+    code reference: https://msurtsukov.github.io/Neural-ODE/;
+    https://github.com/liruilong940607/NeuralODE/blob/master/NeuralODE.py
+
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(ODETPP, self).__init__(model_config)
+
+        self.layer_intensity = nn.Sequential(
+            nn.Linear(self.hidden_size, self.num_event_types),
+            nn.Softplus())
+
+        self.event_model = DNN(inputs_dim=self.hidden_size,
+                               hidden_size=[self.hidden_size])
+
+        self.ode_num_sample_per_step = model_config.model_specs['ode_num_sample_per_step']
+        self.time_factor = model_config.model_specs['time_factor']
+
+        self.solver = rk4_step_method
+
+        self.layer_neural_ode = NeuralODE(model=self.event_model,
+                                          solver=self.solver,
+                                          num_sample_times=self.ode_num_sample_per_step)
+
+    def forward(self, time_delta_seqs, type_seqs, **kwargs):
+        """Call the model.
+
+        Args:
+            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+
+        Returns:
+            tensor: hidden states at event times.
+
+        """
+        # [batch_size, seq_len=max_len-1, hidden_size]
+        type_seq_emb = self.layer_type_emb(type_seqs)
+        time_delta_seqs_ = time_delta_seqs[..., None]
+
+        total_state_at_event_minus = []
+        total_state_at_event_plus = []
+        last_state = torch.zeros_like(type_seq_emb[:, 0, :])
+        for type_emb, dt in zip(torch.unbind(type_seq_emb, dim=-2),
+                                torch.unbind(time_delta_seqs_, dim=-2)):
+            dt = dt / self.time_factor
+            last_state = self.layer_neural_ode(last_state + type_emb, dt)
+            total_state_at_event_minus.append(last_state)
+            total_state_at_event_plus.append(last_state + type_emb)
+
+        # [batch_size, seq_len, hidden_size]
+        state_ti = torch.stack(total_state_at_event_minus, dim=1)
+
+        # [batch_size, seq_len, hidden_size]
+        state_to_evolve = torch.stack(total_state_at_event_plus, dim=1)
+
+        return state_ti, state_to_evolve
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            list: loglike loss, num events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
+
+        state_ti, state_ti_plus = self.forward(time_delta_seqs[:, 1:], type_seqs[:, :-1])
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = state_ti.size()
+
+        # Lambda(t) right before each event time point
+        # lambda_at_event - [batch_size, num_times=max_len-1, num_event_types]
+        # Here we drop the last event because it has no delta_time label (can not decay)
+        lambda_at_event = self.layer_intensity(state_ti)
+
+        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seq[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample, hidden_size]
+        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, interval_t_sample)
+
+        # [batch_size, num_times = max_len - 1, num_mc_sample, event_num]
+        lambda_t_sample = self.layer_intensity(sample_state_ti)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        loss = - (event_ll - non_event_ll).sum()
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, state_ti_plus, sample_dtimes):
+        """Compute the states at sampling times.
+
+        Args:
+            state_ti_plus (tensor): [batch_size, seq_len, hidden_size], states right after the events.
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples], delta times in sampling.
+
+        Returns:
+            tensor: hiddens states at sampling times.
+        """
+
+        # Use broadcasting to compute the decays at all time steps
+        # at all sample points
+        # h_ts shape (batch_size, seq_len, num_samples, hidden_dim)
+        state = self.solver(diff_func=self.event_model,
+                            dt=sample_dtimes[..., None],  # [batch_size, seq_len, num_samples, 1]
+                            z0=state_ti_plus[..., None, :])  # [batch_size, seq_len, 1, hidden_size]
+
+        return state
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_dtimes, **kwargs):
+        """Compute the intensity at sampled times, not only event times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
+                    intensity at each timestamp for each event type.
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        # forward to the last but one event
+        state_ti, state_ti_plus = self.forward(time_delta_seqs, type_seqs, **kwargs)
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = state_ti.size()
+
+        # [batch_size, num_sample_times, num_mc_sample, hidden_size]
+        sample_state_ti = self.compute_states_at_sample_times(state_ti_plus, sample_dtimes)
+
+        if compute_last_step_only:
+            # [batch_size, 1, num_mc_sample, num_event_types]
+            sampled_intensities = self.layer_intensity(sample_state_ti[:, -1:, :, :])
+        else:
+            # [batch_size, num_sample_times, num_mc_sample, num_event_types]
+            sampled_intensities = self.layer_intensity(sample_state_ti)
+
+        return sampled_intensities
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_rmtpp.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_rmtpp.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-import torch
-from torch import nn
-
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-
-
-class RMTPP(TorchBaseModel):
-    """Torch implementation of Recurrent Marked Temporal Point Processes, KDD 2016.
-    https://www.kdd.org/kdd2016/papers/files/rpp1081-duA.pdf
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(RMTPP, self).__init__(model_config)
-
-        self.layer_temporal_emb = nn.Linear(1, self.hidden_size)
-
-        self.layer_rnn = nn.RNN(input_size=self.hidden_size, hidden_size=self.hidden_size,
-                                num_layers=1, batch_first=True)
-
-        self.layer_hidden = nn.Linear(self.hidden_size, self.num_event_types)
-
-        self.factor_intensity_base = torch.empty([1, 1, self.num_event_types])
-        self.factor_intensity_current_influence = torch.empty([1, 1, self.num_event_types])
-
-        nn.init.xavier_normal_(self.factor_intensity_base)
-        nn.init.xavier_normal_(self.factor_intensity_current_influence)
-
-    def state_decay(self, states_to_decay, duration_t):
-        """Equation (11), which computes intensity
-        """
-
-        # [batch_size, seq_len, num_event_types]
-        states_to_decay_ = self.layer_hidden(states_to_decay)
-
-        # [batch_size, seq_len, num_event_types]
-        # put a max number to avoid explode during HPO
-        intensity = torch.exp(
-            states_to_decay_ + self.factor_intensity_current_influence * duration_t +
-            self.factor_intensity_base).clamp(max=1e5)
-        return intensity
-
-    def forward(self, time_seqs, time_delta_seqs, type_seqs, **kwargs):
-        """Call the model.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            list: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens;
-                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
-                  the event happens.
-        """
-
-        max_steps = kwargs.get('max_steps', None)
-
-        # last event has no time label
-        max_seq_length = max_steps if max_steps is not None else type_seqs.size(1) - 1
-
-        # [batch_size, seq_len, hidden_size]
-        type_emb = self.layer_type_emb(type_seqs)
-
-        # [batch_size, seq_len, hidden_size]
-        temporal_emb = self.layer_temporal_emb(time_seqs[..., None])
-
-        # [batch_size, seq_len, hidden_size]
-        # states right after the event
-        decay_states, _ = self.layer_rnn(type_emb + temporal_emb)
-
-        # if only one event, then we dont decay
-        if max_seq_length == 1:
-            h_t = decay_states
-        else:
-            # States decay - Equation (7) in the paper
-            # states before the happening of the next event
-            h_t = self.state_decay(decay_states, time_delta_seqs[..., None])
-
-        return h_t, decay_states
-
-    def loglike_loss(self, batch):
-        """Compute the loglike loss.
-
-        Args:
-            batch (list): batch input.
-
-        Returns:
-            tuple: loglikelihood loss and num of events.
-        """
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
-
-        lambda_at_event, decay_states = self.forward(time_seqs[:, :-1], time_delta_seqs[:, 1:], type_seqs[:, :-1])
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = lambda_at_event.size()
-
-        # Compute the big lambda integral in equation (8)
-        # 1 - take num_mc_sample rand points in each event interval
-        # 2 - compute its lambda value for every sample point
-        # 3 - take average of these sample points
-        # 4 - times the interval length
-
-        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
-        # for every batch and every event point => do a sampling (num_mc_sampling)
-        # the first dtime is zero, so we use time_delta_seqs[:, 1:]
-        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
-
-        # [batch_size, num_times = max_len - 1, num_sample, event_num]
-        lambda_t_sample = self.compute_states_at_sample_times(decay_states, interval_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=time_delta_seqs[:, 1:],
-                                                                        seq_mask=batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=type_mask[:, 1:])
-
-        # (num_samples, num_times)
-        loss = - (event_ll - non_event_ll).sum()
-        return loss, num_events
-
-    def compute_states_at_sample_times(self, decay_states, sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            decay_states (tensor): [batch_size, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: hidden state at each sampled time.
-        """
-        # update the states given last event
-
-        # Use broadcasting to compute the decays at all time steps
-        # decay_states[..., None, :]: [batch_size, seq_len, 1, hidden_size]
-        # sample_dtimes[..., None]: [batch_size, seq_len, num_mc_sample, 1]
-        # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
-        h_ts = self.state_decay(decay_states[..., None, :],
-                                sample_dtimes[..., None])
-
-        return h_ts
-
-    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_times, **kwargs):
-        """Compute the intensity at sampled times, not only event times.
-
-        Args:
-            time_seq (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seq (tensor): [batch_size, seq_len], time delta seqs.
-            event_seq (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
-                    intensity at each timestamp for each event type.
-        """
-
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        # forward to the last but one event
-        _, decay_states = self.forward(time_seqs, time_delta_seqs, type_seqs, **kwargs)
-
-        # Num of samples in each batch and num of event time point in the sequence
-        batch_size, seq_len, _ = decay_states.size()
-
-        if compute_last_step_only:
-            interval_t_sample = sample_times[:, -1:, :, None]
-            # [batch_size, 1, num_mc_sample, num_event_types]
-            sampled_intensities = self.state_decay(decay_states[:, -1:, None, :],
-                                                   interval_t_sample)
-
-        else:
-            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
-            interval_t_sample = sample_times[..., None]
-            # Use broadcasting to compute the decays at all time steps
-            # at all sample points
-            # sampled_intensities shape (batch_size, num_times, num_mc_sample, hidden_dim)
-            # decay_states[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
-            sampled_intensities = self.state_decay(decay_states[..., None, :],
-                                                   interval_t_sample)
-
-        return sampled_intensities
+import torch
+from torch import nn
+
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class RMTPP(TorchBaseModel):
+    """Torch implementation of Recurrent Marked Temporal Point Processes, KDD 2016.
+    https://www.kdd.org/kdd2016/papers/files/rpp1081-duA.pdf
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(RMTPP, self).__init__(model_config)
+
+        self.layer_temporal_emb = nn.Linear(1, self.hidden_size)
+
+        self.layer_rnn = nn.RNN(input_size=self.hidden_size, hidden_size=self.hidden_size,
+                                num_layers=1, batch_first=True)
+
+        self.layer_hidden = nn.Linear(self.hidden_size, self.num_event_types)
+
+        self.factor_intensity_base = torch.empty([1, 1, self.num_event_types])
+        self.factor_intensity_current_influence = torch.empty([1, 1, self.num_event_types])
+
+        nn.init.xavier_normal_(self.factor_intensity_base)
+        nn.init.xavier_normal_(self.factor_intensity_current_influence)
+
+    def state_decay(self, states_to_decay, duration_t):
+        """Equation (11), which computes intensity
+        """
+
+        # [batch_size, seq_len, num_event_types]
+        states_to_decay_ = self.layer_hidden(states_to_decay)
+
+        # [batch_size, seq_len, num_event_types]
+        # put a max number to avoid explode during HPO
+        intensity = torch.exp(
+            states_to_decay_ + self.factor_intensity_current_influence * duration_t +
+            self.factor_intensity_base).clamp(max=1e5)
+        return intensity
+
+    def forward(self, time_seqs, time_delta_seqs, type_seqs, **kwargs):
+        """Call the model.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            list: hidden states, [batch_size, seq_len, hidden_dim], states right before the event happens;
+                  stacked decay states,  [batch_size, max_seq_length, 4, hidden_dim], states right after
+                  the event happens.
+        """
+
+        max_steps = kwargs.get('max_steps', None)
+
+        # last event has no time label
+        max_seq_length = max_steps if max_steps is not None else type_seqs.size(1) - 1
+
+        # [batch_size, seq_len, hidden_size]
+        type_emb = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size]
+        temporal_emb = self.layer_temporal_emb(time_seqs[..., None])
+
+        # [batch_size, seq_len, hidden_size]
+        # states right after the event
+        decay_states, _ = self.layer_rnn(type_emb + temporal_emb)
+
+        # if only one event, then we dont decay
+        if max_seq_length == 1:
+            h_t = decay_states
+        else:
+            # States decay - Equation (7) in the paper
+            # states before the happening of the next event
+            h_t = self.state_decay(decay_states, time_delta_seqs[..., None])
+
+        return h_t, decay_states
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (list): batch input.
+
+        Returns:
+            tuple: loglikelihood loss and num of events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, _, type_mask = batch
+
+        lambda_at_event, decay_states = self.forward(time_seqs[:, :-1], time_delta_seqs[:, 1:], type_seqs[:, :-1])
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = lambda_at_event.size()
+
+        # Compute the big lambda integral in equation (8)
+        # 1 - take num_mc_sample rand points in each event interval
+        # 2 - compute its lambda value for every sample point
+        # 3 - take average of these sample points
+        # 4 - times the interval length
+
+        # interval_t_sample - [batch_size, num_times=max_len-1, num_mc_sample]
+        # for every batch and every event point => do a sampling (num_mc_sampling)
+        # the first dtime is zero, so we use time_delta_seqs[:, 1:]
+        interval_t_sample = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        # [batch_size, num_times = max_len - 1, num_sample, event_num]
+        lambda_t_sample = self.compute_states_at_sample_times(decay_states, interval_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        # (num_samples, num_times)
+        loss = - (event_ll - non_event_ll).sum()
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, decay_states, sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            decay_states (tensor): [batch_size, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: hidden state at each sampled time.
+        """
+        # update the states given last event
+
+        # Use broadcasting to compute the decays at all time steps
+        # decay_states[..., None, :]: [batch_size, seq_len, 1, hidden_size]
+        # sample_dtimes[..., None]: [batch_size, seq_len, num_mc_sample, 1]
+        # h_ts shape (batch_size, num_times, num_mc_sample, hidden_dim)
+        h_ts = self.state_decay(decay_states[..., None, :],
+                                sample_dtimes[..., None])
+
+        return h_ts
+
+    def compute_intensities_at_sample_times(self, time_seqs, time_delta_seqs, type_seqs, sample_times, **kwargs):
+        """Compute the intensity at sampled times, not only event times.
+
+        Args:
+            time_seq (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seq (tensor): [batch_size, seq_len], time delta seqs.
+            event_seq (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_sample], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, num_times, num_mc_sample, num_event_types],
+                    intensity at each timestamp for each event type.
+        """
+
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        # forward to the last but one event
+        _, decay_states = self.forward(time_seqs, time_delta_seqs, type_seqs, **kwargs)
+
+        # Num of samples in each batch and num of event time point in the sequence
+        batch_size, seq_len, _ = decay_states.size()
+
+        if compute_last_step_only:
+            interval_t_sample = sample_times[:, -1:, :, None]
+            # [batch_size, 1, num_mc_sample, num_event_types]
+            sampled_intensities = self.state_decay(decay_states[:, -1:, None, :],
+                                                   interval_t_sample)
+
+        else:
+            # interval_t_sample - [batch_size, num_times, num_mc_sample, 1]
+            interval_t_sample = sample_times[..., None]
+            # Use broadcasting to compute the decays at all time steps
+            # at all sample points
+            # sampled_intensities shape (batch_size, num_times, num_mc_sample, hidden_dim)
+            # decay_states[:, :, None, :]  (batch_size, num_times, 1, hidden_dim)
+            sampled_intensities = self.state_decay(decay_states[..., None, :],
+                                                   interval_t_sample)
+
+        return sampled_intensities
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_sahp.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_thp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,212 +1,187 @@
-import torch
-import torch.nn as nn
-
-from easy_tpp.model.torch_model.torch_baselayer import EncoderLayer, MultiHeadAttention, \
-    TimeShiftedPositionalEncoding
-from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-
-
-class SAHP(TorchBaseModel):
-    """Torch implementation of Self-Attentive Hawkes Process, ICML 2020.
-    Part of the code is collected from https://github.com/yangalan123/anhp-andtt/blob/master/sahp
-
-    I slightly modify the original code because it is not stable.
-
-    """
-
-    def __init__(self, model_config):
-        """Initialize the model
-
-        Args:
-            model_config (EasyTPP.ModelConfig): config of model specs.
-        """
-        super(SAHP, self).__init__(model_config)
-        self.d_model = model_config.hidden_size
-        self.d_time = model_config.time_emb_size
-
-        self.use_norm = model_config.use_ln
-
-        # position vector, used for temporal encoding
-        self.layer_position_emb = TimeShiftedPositionalEncoding(d_model=self.d_model)
-
-        self.n_layers = model_config.num_layers
-        self.n_head = model_config.num_heads
-        self.dropout = model_config.dropout_rate
-
-        # convert hidden vectors into a scalar
-        self.layer_intensity_hidden = nn.Linear(self.d_model, self.num_event_types)
-        self.softplus = nn.Softplus()
-
-        self.stack_layers = nn.ModuleList(
-            [EncoderLayer(
-                self.d_model,
-                MultiHeadAttention(self.n_head, self.d_model, self.d_model, self.dropout,
-                                   output_linear=False),
-
-                use_residual=False,
-                dropout=self.dropout
-            ) for _ in range(self.n_layers)])
-
-        if self.use_norm:
-            self.norm = nn.LayerNorm(self.d_model)
-
-        # Equation (12): mu
-        self.mu = torch.empty([self.d_model, self.num_event_types])
-        # Equation (13): eta
-        self.eta = torch.empty([self.d_model, self.num_event_types])
-        # Equation (14): gamma
-        self.gamma = torch.empty([self.d_model, self.num_event_types])
-
-        nn.init.xavier_normal_(self.mu)
-        nn.init.xavier_normal_(self.eta)
-        nn.init.xavier_normal_(self.gamma)
-
-    def state_decay(self, encode_state, mu, eta, gamma, duration_t):
-        """Equation (15), which computes the pre-intensity states
-
-        Args:
-            encode_state (tensor): [batch_size, seq_len, hidden_size].
-            mu (tensor): [batch_size, seq_len, hidden_size].
-            eta (tensor): [batch_size, seq_len, hidden_size].
-            gamma (tensor): [batch_size, seq_len, hidden_size].
-            duration_t (tensor): [batch_size, seq_len, num_sample].
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-
-        # [batch_size, hidden_dim]
-        states = torch.matmul(encode_state, mu) + (
-                    torch.matmul(encode_state, eta) - torch.matmul(encode_state, mu)) * torch.exp(
-            -torch.matmul(encode_state, gamma) * duration_t)
-        return states
-
-    def forward(self, time_seqs, time_delta_seqs, event_seqs, attention_mask):
-        """Call the model
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], inter-event time seqs.
-            event_seqs (tensor): [batch_size, seq_len], event type seqs.
-            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
-
-        Returns:
-            tensor: hidden states at event times.
-        """
-        type_embedding = self.layer_type_emb(event_seqs)
-        position_embedding = self.layer_position_emb(time_seqs, time_delta_seqs)
-
-        enc_output = type_embedding + position_embedding
-
-        for enc_layer in self.stack_layers:
-            enc_output = enc_layer(
-                enc_output,
-                mask=attention_mask)
-            if self.use_norm:
-                enc_output = self.norm(enc_output)
-        # [batch_size, seq_len, hidden_dim]
-        return enc_output
-
-    def loglike_loss(self, batch):
-        """Compute the loglike loss.
-
-        Args:
-            batch (tuple, list): batch input.
-
-        Returns:
-            list: loglike loss, num events.
-        """
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch
-
-        enc_out = self.forward(time_seqs[:, :-1], time_delta_seqs[:, 1:], type_seqs[:, :-1], attention_mask[:, 1:, :-1])
-
-        cell_t = self.state_decay(encode_state=enc_out,
-                                  mu=self.mu[None, ...],
-                                  eta=self.eta[None, ...],
-                                  gamma=self.gamma[None, ...],
-                                  duration_t=time_delta_seqs[:, 1:, None])
-
-        # [batch_size, seq_len, num_event_types]
-        lambda_at_event = self.softplus(cell_t)
-
-        # 2. compute non-event-loglik (using MC sampling to compute integral)
-        # 2.1 sample times
-        # [batch_size, seq_len, num_sample]
-        sample_dtimes = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
-
-        # 2.2 compute intensities at sampled times
-        # [batch_size, num_times = max_len - 1, num_sample, event_num]
-        state_t_sample = self.compute_states_at_sample_times(encode_state=enc_out,
-                                                             sample_dtimes=sample_dtimes)
-        lambda_t_sample = self.softplus(state_t_sample)
-
-        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
-                                                                        lambdas_loss_samples=lambda_t_sample,
-                                                                        time_delta_seq=time_delta_seqs[:, 1:],
-                                                                        seq_mask=batch_non_pad_mask[:, 1:],
-                                                                        lambda_type_mask=type_mask[:, 1:])
-
-        # return enc_inten to compute accuracy
-        loss = - (event_ll - non_event_ll).sum()
-
-        return loss, num_events
-
-    def compute_states_at_sample_times(self,
-                                       encode_state,
-                                       sample_dtimes):
-        """Compute the hidden states at sampled times.
-
-        Args:
-            encode_state (tensor): three tensors with each shape [batch_size, seq_len, hidden_size].
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
-
-        Returns:
-            tensor: [batch_size, seq_len, num_samples, hidden_size]， hidden state at each sampled time.
-        """
-
-        cell_states = self.state_decay(encode_state[:, :, None, :],
-                                       self.mu[None, None, ...],
-                                       self.eta[None, None, ...],
-                                       self.gamma[None, None, ...],
-                                       sample_dtimes[:, :, :, None])
-
-        return cell_states
-
-    def compute_intensities_at_sample_times(self,
-                                            time_seqs,
-                                            time_delta_seqs,
-                                            type_seqs,
-                                            sample_dtimes,
-                                            **kwargs):
-        """Compute hidden states at sampled times.
-
-        Args:
-            time_seqs (tensor): [batch_size, seq_len], times seqs.
-            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
-            type_seqs (tensor): [batch_size, seq_len], event type seqs.
-            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
-
-        Returns:
-            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
-        """
-
-        attention_mask = kwargs.get('attention_mask', None)
-        compute_last_step_only = kwargs.get('compute_last_step_only', False)
-
-        if attention_mask is None:
-            batch_size, seq_len = time_seqs.size()
-            attention_mask = torch.triu(torch.ones(seq_len, seq_len), diagonal=1).unsqueeze(0)
-            attention_mask = attention_mask.expand(batch_size, -1, -1).to(torch.bool)
-
-        # [batch_size, seq_len, num_samples]
-        enc_out = self.forward(time_seqs, time_delta_seqs, type_seqs, attention_mask)
-
-        # [batch_size, seq_len, num_samples, hidden_size]
-        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
-
-        if compute_last_step_only:
-            lambdas = self.softplus(encoder_output[:, -1:, :, :])
-        else:
-            # [batch_size, seq_len, num_samples, num_event_types]
-            lambdas = self.softplus(encoder_output)
-        return lambdas
+import torch
+import torch.nn as nn
+
+from easy_tpp.model.torch_model.torch_baselayer import EncoderLayer, MultiHeadAttention, TimePositionalEncoding
+from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+
+
+class THP(TorchBaseModel):
+    """Torch implementation of Transformer Hawkes Process, ICML 2020, https://arxiv.org/abs/2002.09291.
+    Note: Part of the code is collected from https://github.com/yangalan123/anhp-andtt/tree/master/thp.
+    """
+
+    def __init__(self, model_config):
+        """Initialize the model
+
+        Args:
+            model_config (EasyTPP.ModelConfig): config of model specs.
+        """
+        super(THP, self).__init__(model_config)
+        self.d_model = model_config.hidden_size
+        self.d_time = model_config.time_emb_size
+        self.use_norm = model_config.use_ln
+
+        self.n_layers = model_config.num_layers
+        self.n_head = model_config.num_heads
+        self.dropout = model_config.dropout_rate
+
+        self.layer_temporal_encoding = TimePositionalEncoding(self.d_model)
+
+        self.factor_intensity_base = torch.empty([1, self.num_event_types])
+        self.factor_intensity_decay = torch.empty([1, self.num_event_types])
+        nn.init.xavier_normal_(self.factor_intensity_base)
+        nn.init.xavier_normal_(self.factor_intensity_decay)
+
+        # convert hidden vectors into event-type-sized vector
+        self.layer_intensity_hidden = nn.Linear(self.d_model, self.num_event_types)
+        self.softplus = nn.Softplus()
+
+        self.stack_layers = nn.ModuleList(
+            [EncoderLayer(
+                self.d_model,
+                MultiHeadAttention(self.n_head, self.d_model, self.d_model, self.dropout,
+                                   output_linear=False),
+
+                use_residual=False,
+                dropout=self.dropout
+            ) for _ in range(self.n_layers)])
+
+    def forward(self, time_seqs, type_seqs, attention_mask):
+        """Call the model
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], timestamp seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            attention_mask (tensor): [batch_size, seq_len, hidden_size], attention masks.
+
+        Returns:
+            tensor: hidden states at event times.
+        """
+        # [batch_size, seq_len, hidden_size]
+        tem_enc = self.layer_temporal_encoding(time_seqs)
+        enc_output = self.layer_type_emb(type_seqs)
+
+        # [batch_size, seq_len, hidden_size]
+        for enc_layer in self.stack_layers:
+            enc_output += tem_enc
+            enc_output = enc_layer(
+                enc_output,
+                mask=attention_mask)
+
+        return enc_output
+
+    def loglike_loss(self, batch):
+        """Compute the loglike loss.
+
+        Args:
+            batch (tuple, list): batch input.
+
+        Returns:
+            tuple: loglike loss, num events.
+        """
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch
+
+        # 1. compute event-loglik
+        # [batch_size, seq_len, hidden_size]
+        enc_out = self.forward(time_seqs[:, :-1], type_seqs[:, :-1], attention_mask[:, 1:, :-1])
+
+        # [batch_size, seq_len, num_event_types]
+        # update time decay based on Equation (6)
+        # [1, 1, num_event_types]
+        factor_intensity_decay = self.factor_intensity_decay[None, ...]
+        factor_intensity_base = self.factor_intensity_base[None, ...]
+
+        # update time decay based on Equation (6)
+        # [batch_size, seq_len, num_event_types]
+        intensity_states = factor_intensity_decay * time_delta_seqs[:, 1:, None] + self.layer_intensity_hidden(
+            enc_out) + factor_intensity_base
+
+        lambda_at_event = self.softplus(intensity_states)
+
+        # 2. compute non-event-loglik (using MC sampling to compute integral)
+        # 2.1 sample dtimes
+        # [batch_size, seq_len, num_sample]
+        sample_dtimes = self.make_dtime_loss_samples(time_delta_seqs[:, 1:])
+
+        # 2.2 compute intensities at sampled times
+        # [batch_size, num_times = max_len - 1, num_sample, event_num]
+        state_t_sample = self.compute_states_at_sample_times(event_states=enc_out,
+                                                             sample_dtimes=sample_dtimes)
+        lambda_t_sample = self.softplus(state_t_sample)
+
+        event_ll, non_event_ll, num_events = self.compute_loglikelihood(lambda_at_event=lambda_at_event,
+                                                                        lambdas_loss_samples=lambda_t_sample,
+                                                                        time_delta_seq=time_delta_seqs[:, 1:],
+                                                                        seq_mask=batch_non_pad_mask[:, 1:],
+                                                                        lambda_type_mask=type_mask[:, 1:])
+
+        # return enc_inten to compute accuracy
+        loss = - (event_ll - non_event_ll).sum()
+
+        return loss, num_events
+
+    def compute_states_at_sample_times(self, event_states, sample_dtimes):
+        """Compute the hidden states at sampled times.
+
+        Args:
+            event_states (tensor): [batch_size, seq_len, hidden_size].
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples].
+
+        Returns:
+            tensor: hidden state at each sampled time.
+        """
+        # [batch_size, seq_len, 1, hidden_size]
+        event_states = event_states[:, :, None, :]
+
+        # [batch_size, seq_len, num_samples, 1]
+        sample_dtimes = sample_dtimes[..., None]
+
+        # [1, 1, 1, num_event_types]
+        factor_intensity_decay = self.factor_intensity_decay[None, None, ...]
+        factor_intensity_base = self.factor_intensity_base[None, None, ...]
+
+        # update time decay based on Equation (6)
+        # [batch_size, seq_len, num_samples, num_event_types]
+        intensity_states = factor_intensity_decay * sample_dtimes + self.layer_intensity_hidden(
+            event_states) + factor_intensity_base
+
+        return intensity_states
+
+    def compute_intensities_at_sample_times(self,
+                                            time_seqs,
+                                            time_delta_seqs,
+                                            type_seqs,
+                                            sample_dtimes,
+                                            **kwargs):
+        """Compute hidden states at sampled times.
+
+        Args:
+            time_seqs (tensor): [batch_size, seq_len], times seqs.
+            time_delta_seqs (tensor): [batch_size, seq_len], time delta seqs.
+            type_seqs (tensor): [batch_size, seq_len], event type seqs.
+            sample_dtimes (tensor): [batch_size, seq_len, num_samples], sampled inter-event timestamps.
+
+        Returns:
+            tensor: [batch_size, seq_len, num_samples, num_event_types], intensity at all sampled times.
+        """
+
+        attention_mask = kwargs.get('attention_mask', None)
+        compute_last_step_only = kwargs.get('compute_last_step_only', False)
+
+        if attention_mask is None:
+            batch_size, seq_len = time_seqs.size()
+            attention_mask = torch.triu(torch.ones(seq_len, seq_len), diagonal=1).unsqueeze(0)
+            attention_mask = attention_mask.expand(batch_size, -1, -1).to(torch.bool)
+
+        # [batch_size, seq_len, num_samples]
+        enc_out = self.forward(time_seqs, type_seqs, attention_mask)
+
+        # [batch_size, seq_len, num_samples, hidden_size]
+        encoder_output = self.compute_states_at_sample_times(enc_out, sample_dtimes)
+
+        if compute_last_step_only:
+            lambdas = self.softplus(encoder_output[:, -1:, :, :])
+        else:
+            # [batch_size, seq_len, num_samples, num_event_types]
+            lambdas = self.softplus(encoder_output)
+        return lambdas
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thinning.py` & `easy_tpp-0.0.5/easy_tpp/model/torch_model/torch_thinning.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-import torch
-import torch.nn as nn
-
-
-class EventSampler(nn.Module):
-    """Event Sequence Sampler based on thinning algorithm, which corresponds to Algorithm 2 of
-    The Neural Hawkes Process: A Neurally Self-Modulating Multivariate Point Process,
-    https://arxiv.org/abs/1612.09328.
-
-    The implementation uses code from https://github.com/yangalan123/anhp-andtt/blob/master/anhp/esm/thinning.py.
-    """
-
-    def __init__(self, num_sample, num_exp, over_sample_rate, num_samples_boundary, dtime_max, patience_counter):
-        """Initialize the event sampler.
-
-        Args:
-            num_sample (int): number of sampled next event times via thinning algo for computing predictions.
-            num_exp (int): number of i.i.d. Exp(intensity_bound) draws at one time in thinning algorithm
-            over_sample_rate (float): multiplier for the intensity up bound.
-            num_samples_boundary (int): number of sampled event times to compute the boundary of the intensity.
-            dtime_max (float): max value of delta times in sampling
-            patience_counter (int): the maximum iteration used in adaptive thinning.
-        """
-        super(EventSampler, self).__init__()
-        self.num_sample = num_sample
-        self.num_exp = num_exp
-        self.over_sample_rate = over_sample_rate
-        self.num_samples_boundary = num_samples_boundary
-        self.dtime_max = dtime_max
-        self.patience_counter = patience_counter
-
-    def compute_intensity_upper_bound(self, time_seq, time_delta_seq, event_seq, intensity_fn,
-                                      compute_last_step_only):
-        """Compute the upper bound of intensity at each event timestamp.
-
-        Args:
-            time_seq (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seq (tensor): [batch_size, seq_len], time delta seqs.
-            event_seq (tensor): [batch_size, seq_len], event type seqs.
-            intensity_fn (fn): a function that computes the intensity.
-            compute_last_step_only (bool): wheter to compute the last time step pnly.
-
-        Returns:
-            tensor: [batch_size, seq_len]
-        """
-        batch_size, seq_len = time_seq.size()
-
-        # [1, 1, num_samples_boundary]
-        time_for_bound_sampled = torch.linspace(start=0.0,
-                                                end=1.0,
-                                                steps=self.num_samples_boundary)[None, None, :]
-
-        # [batch_size, seq_len, num_sample]
-        dtime_for_bound_sampled = time_delta_seq[:, :, None] * time_for_bound_sampled
-
-        # [batch_size, seq_len, num_sample, event_num]
-        intensities_for_bound = intensity_fn(time_seq,
-                                             time_delta_seq,
-                                             event_seq,
-                                             dtime_for_bound_sampled,
-                                             max_steps=seq_len,
-                                             compute_last_step_only=compute_last_step_only)
-
-        # [batch_size, seq_len]
-        bounds = intensities_for_bound.sum(dim=-1).max(dim=-1)[0] * self.over_sample_rate
-
-        return bounds
-
-    def sample_exp_distribution(self, sample_rate):
-        """Sample an exponential distribution.
-
-        Args:
-            sample_rate (tensor): [batch_size, seq_len], intensity rate.
-
-        Returns:
-            tensor: [batch_size, seq_len, num_exp], exp numbers at each event timestamp.
-        """
-
-        batch_size, seq_len = sample_rate.size()
-
-        # For fast approximation, we reuse the rnd for all samples
-        # [batch_size, seq_len, num_exp]
-        exp_numbers = torch.empty(size=[batch_size, seq_len, self.num_exp],
-                                  dtype=torch.float32)
-
-        # [batch_size, seq_len, num_exp]
-        # exp_numbers.exponential_(1.0)
-        exp_numbers.exponential_(1.0)
-
-        # [batch_size, seq_len, num_exp]
-        # exp_numbers = torch.tile(exp_numbers, [1, 1, self.num_sample, 1])
-
-        # [batch_size, seq_len, num_exp]
-        # div by sample_rate is equivalent to exp(sample_rate),
-        # see https://en.wikipedia.org/wiki/Exponential_distribution
-        exp_numbers = exp_numbers / sample_rate[:, :, None]
-
-        return exp_numbers
-
-    def sample_uniform_distribution(self, intensity_upper_bound):
-        """Sample an uniform distribution
-
-        Args:
-            intensity_upper_bound (tensor): upper bound intensity computed in the previous step.
-
-        Returns:
-            tensor: [batch_size, seq_len, num_sample, num_exp]
-        """
-        batch_size, seq_len = intensity_upper_bound.size()
-
-        unif_numbers = torch.empty(size=[batch_size, seq_len, self.num_sample, self.num_exp],
-                                   dtype=torch.float32)
-        unif_numbers.uniform_(0.0, 1.0)
-
-        return unif_numbers
-
-    def sample_accept(self, unif_numbers, sample_rate, total_intensities):
-        """Do the sample-accept process.
-
-        For each parallel draw, find its min criterion： if that < 1.0, the 1st (i.e. smallest) sampled time
-        with cri < 1.0 is accepted; if none is accepted, use boundary / maxsampletime for that draw
-
-        Args:
-            unif_numbers (tensor): [batch_size, max_len, num_sample, num_exp], sampled uniform random number.
-            sample_rate (tensor): [batch_size, max_len], sample rate (intensity).
-            total_intensities (tensor): [batch_size, seq_len, num_sample, num_exp]
-
-        Returns:
-            list: two tensors,
-            criterion, [batch_size, max_len, num_sample, num_exp]
-            who_has_accepted_times, [batch_size, max_len, num_sample]
-        """
-
-        # [batch_size, max_len, num_sample, num_exp]
-        criterion = unif_numbers * sample_rate[:, :, None, None] / total_intensities
-
-        # [batch_size, max_len, num_sample]
-        min_cri_each_draw, _ = criterion.min(dim=-1)
-
-        # find out unif_numbers * sample_rate < intensity
-        # [batch_size, max_len, num_sample]
-        who_has_accepted_times = min_cri_each_draw < 1.0
-
-        return criterion, who_has_accepted_times
-
-    def draw_next_time_one_step(self, time_seq, time_delta_seq, event_seq, dtime_boundary,
-                                intensity_fn, compute_last_step_only=False):
-        """Compute next event time based on Thinning algorithm.
-
-        Args:
-            time_seq (tensor): [batch_size, seq_len], timestamp seqs.
-            time_delta_seq (tensor): [batch_size, seq_len], time delta seqs.
-            event_seq (tensor): [batch_size, seq_len], event type seqs.
-            dtime_boundary (tensor): [batch_size, seq_len], dtime upper bound.
-            intensity_fn (fn): a function to compute the intensity.
-            compute_last_step_only (bool, optional): whether to compute last event timestep only. Defaults to False.
-
-        Returns:
-            tuple: next event time prediction and weight.
-        """
-        # 1. compute the upper bound of the intensity at each timestamp
-        # the last event has no label (no next event), so we drop it
-        # [batch_size, seq_len=max_len - 1]
-        intensity_upper_bound = self.compute_intensity_upper_bound(time_seq,
-                                                                   time_delta_seq,
-                                                                   event_seq,
-                                                                   intensity_fn,
-                                                                   compute_last_step_only)
-
-        # 2. draw exp distribution with intensity = intensity_upper_bound
-        # we apply fast approximation, i.e., re-use exp sample times for computation
-        # [batch_size, seq_len, num_exp]
-        exp_numbers = self.sample_exp_distribution(intensity_upper_bound)
-
-        # 3. compute intensity at sampled times from exp distribution
-        # [batch_size, seq_len, num_exp, event_num]
-        intensities_at_sampled_times = intensity_fn(time_seq,
-                                                    time_delta_seq,
-                                                    event_seq,
-                                                    exp_numbers,
-                                                    max_steps=time_seq.size(1),
-                                                    compute_last_step_only=compute_last_step_only)
-
-        # [batch_size, seq_len, num_exp]
-        total_intensities = intensities_at_sampled_times.sum(dim=-1)
-
-        # add one dim of num_sample: re-use the intensity for samples for prediction
-        # [batch_size, seq_len, num_sample, num_exp]
-        total_intensities = torch.tile(total_intensities[:, :, None, :], [1, 1, self.num_sample, 1])
-        # [batch_size, seq_len, num_sample, num_exp]
-        exp_numbers = torch.tile(exp_numbers[:, :, None, :], [1, 1, self.num_sample, 1])
-
-        # 4. draw uniform distribution
-        # [batch_size, seq_len, num_sample, num_exp]
-        unif_numbers = self.sample_uniform_distribution(intensity_upper_bound)
-
-        # 5. find out accepted intensities
-        # criterion, [batch_size, max_len, num_sample, num_exp]
-        # who_has_accepted_times, [batch_size, max_len, num_sample]
-        criterion, who_has_accepted_times = self.sample_accept(unif_numbers, intensity_upper_bound,
-                                                               total_intensities)
-
-        # 6. find out accepted dtimes
-        sampled_dtimes_accepted = exp_numbers.clone()
-
-        # for unaccepted, use boundary/maxsampletime for that draw
-        sampled_dtimes_accepted[criterion >= 1.0] = exp_numbers.max() + 1.0
-
-        accepted_times_each_draw, accepted_id_each_draw = sampled_dtimes_accepted.min(dim=-1)
-
-        # 7. fill out result
-        dtime_boundary_ = dtime_boundary[:, -1:] if compute_last_step_only else dtime_boundary
-
-        # [batch_size, seq_len, num_sample]
-        dtime_boundary_ = torch.tile(dtime_boundary_[..., None], [1, 1, self.num_sample])
-
-        # [batch_size, seq_len, num_sample]
-        res = torch.ones_like(dtime_boundary_) * dtime_boundary_
-
-        # [batch_size, seq_len, num_sample]
-        weights = torch.ones_like(dtime_boundary_)
-        weights /= weights.sum(dim=-1, keepdim=True)
-
-        res[who_has_accepted_times] = accepted_times_each_draw[who_has_accepted_times]
-        who_not_accept = ~who_has_accepted_times
-
-        who_reach_further = exp_numbers[..., -1] > dtime_boundary_
-
-        res[who_not_accept & who_reach_further] = exp_numbers[..., -1][who_not_accept & who_reach_further]
-
-        # add a upper bound here in case it explodes, e.g., in ODE models
-        return res.clamp(max=1e5), weights
+import torch
+import torch.nn as nn
+
+
+class EventSampler(nn.Module):
+    """Event Sequence Sampler based on thinning algorithm, which corresponds to Algorithm 2 of
+    The Neural Hawkes Process: A Neurally Self-Modulating Multivariate Point Process,
+    https://arxiv.org/abs/1612.09328.
+
+    The implementation uses code from https://github.com/yangalan123/anhp-andtt/blob/master/anhp/esm/thinning.py.
+    """
+
+    def __init__(self, num_sample, num_exp, over_sample_rate, num_samples_boundary, dtime_max, patience_counter):
+        """Initialize the event sampler.
+
+        Args:
+            num_sample (int): number of sampled next event times via thinning algo for computing predictions.
+            num_exp (int): number of i.i.d. Exp(intensity_bound) draws at one time in thinning algorithm
+            over_sample_rate (float): multiplier for the intensity up bound.
+            num_samples_boundary (int): number of sampled event times to compute the boundary of the intensity.
+            dtime_max (float): max value of delta times in sampling
+            patience_counter (int): the maximum iteration used in adaptive thinning.
+        """
+        super(EventSampler, self).__init__()
+        self.num_sample = num_sample
+        self.num_exp = num_exp
+        self.over_sample_rate = over_sample_rate
+        self.num_samples_boundary = num_samples_boundary
+        self.dtime_max = dtime_max
+        self.patience_counter = patience_counter
+
+    def compute_intensity_upper_bound(self, time_seq, time_delta_seq, event_seq, intensity_fn,
+                                      compute_last_step_only):
+        """Compute the upper bound of intensity at each event timestamp.
+
+        Args:
+            time_seq (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seq (tensor): [batch_size, seq_len], time delta seqs.
+            event_seq (tensor): [batch_size, seq_len], event type seqs.
+            intensity_fn (fn): a function that computes the intensity.
+            compute_last_step_only (bool): wheter to compute the last time step pnly.
+
+        Returns:
+            tensor: [batch_size, seq_len]
+        """
+        batch_size, seq_len = time_seq.size()
+
+        # [1, 1, num_samples_boundary]
+        time_for_bound_sampled = torch.linspace(start=0.0,
+                                                end=1.0,
+                                                steps=self.num_samples_boundary)[None, None, :]
+
+        # [batch_size, seq_len, num_sample]
+        dtime_for_bound_sampled = time_delta_seq[:, :, None] * time_for_bound_sampled
+
+        # [batch_size, seq_len, num_sample, event_num]
+        intensities_for_bound = intensity_fn(time_seq,
+                                             time_delta_seq,
+                                             event_seq,
+                                             dtime_for_bound_sampled,
+                                             max_steps=seq_len,
+                                             compute_last_step_only=compute_last_step_only)
+
+        # [batch_size, seq_len]
+        bounds = intensities_for_bound.sum(dim=-1).max(dim=-1)[0] * self.over_sample_rate
+
+        return bounds
+
+    def sample_exp_distribution(self, sample_rate):
+        """Sample an exponential distribution.
+
+        Args:
+            sample_rate (tensor): [batch_size, seq_len], intensity rate.
+
+        Returns:
+            tensor: [batch_size, seq_len, num_exp], exp numbers at each event timestamp.
+        """
+
+        batch_size, seq_len = sample_rate.size()
+
+        # For fast approximation, we reuse the rnd for all samples
+        # [batch_size, seq_len, num_exp]
+        exp_numbers = torch.empty(size=[batch_size, seq_len, self.num_exp],
+                                  dtype=torch.float32)
+
+        # [batch_size, seq_len, num_exp]
+        # exp_numbers.exponential_(1.0)
+        exp_numbers.exponential_(1.0)
+
+        # [batch_size, seq_len, num_exp]
+        # exp_numbers = torch.tile(exp_numbers, [1, 1, self.num_sample, 1])
+
+        # [batch_size, seq_len, num_exp]
+        # div by sample_rate is equivalent to exp(sample_rate),
+        # see https://en.wikipedia.org/wiki/Exponential_distribution
+        exp_numbers = exp_numbers / sample_rate[:, :, None]
+
+        return exp_numbers
+
+    def sample_uniform_distribution(self, intensity_upper_bound):
+        """Sample an uniform distribution
+
+        Args:
+            intensity_upper_bound (tensor): upper bound intensity computed in the previous step.
+
+        Returns:
+            tensor: [batch_size, seq_len, num_sample, num_exp]
+        """
+        batch_size, seq_len = intensity_upper_bound.size()
+
+        unif_numbers = torch.empty(size=[batch_size, seq_len, self.num_sample, self.num_exp],
+                                   dtype=torch.float32)
+        unif_numbers.uniform_(0.0, 1.0)
+
+        return unif_numbers
+
+    def sample_accept(self, unif_numbers, sample_rate, total_intensities):
+        """Do the sample-accept process.
+
+        For each parallel draw, find its min criterion： if that < 1.0, the 1st (i.e. smallest) sampled time
+        with cri < 1.0 is accepted; if none is accepted, use boundary / maxsampletime for that draw
+
+        Args:
+            unif_numbers (tensor): [batch_size, max_len, num_sample, num_exp], sampled uniform random number.
+            sample_rate (tensor): [batch_size, max_len], sample rate (intensity).
+            total_intensities (tensor): [batch_size, seq_len, num_sample, num_exp]
+
+        Returns:
+            list: two tensors,
+            criterion, [batch_size, max_len, num_sample, num_exp]
+            who_has_accepted_times, [batch_size, max_len, num_sample]
+        """
+
+        # [batch_size, max_len, num_sample, num_exp]
+        criterion = unif_numbers * sample_rate[:, :, None, None] / total_intensities
+
+        # [batch_size, max_len, num_sample]
+        min_cri_each_draw, _ = criterion.min(dim=-1)
+
+        # find out unif_numbers * sample_rate < intensity
+        # [batch_size, max_len, num_sample]
+        who_has_accepted_times = min_cri_each_draw < 1.0
+
+        return criterion, who_has_accepted_times
+
+    def draw_next_time_one_step(self, time_seq, time_delta_seq, event_seq, dtime_boundary,
+                                intensity_fn, compute_last_step_only=False):
+        """Compute next event time based on Thinning algorithm.
+
+        Args:
+            time_seq (tensor): [batch_size, seq_len], timestamp seqs.
+            time_delta_seq (tensor): [batch_size, seq_len], time delta seqs.
+            event_seq (tensor): [batch_size, seq_len], event type seqs.
+            dtime_boundary (tensor): [batch_size, seq_len], dtime upper bound.
+            intensity_fn (fn): a function to compute the intensity.
+            compute_last_step_only (bool, optional): whether to compute last event timestep only. Defaults to False.
+
+        Returns:
+            tuple: next event time prediction and weight.
+        """
+        # 1. compute the upper bound of the intensity at each timestamp
+        # the last event has no label (no next event), so we drop it
+        # [batch_size, seq_len=max_len - 1]
+        intensity_upper_bound = self.compute_intensity_upper_bound(time_seq,
+                                                                   time_delta_seq,
+                                                                   event_seq,
+                                                                   intensity_fn,
+                                                                   compute_last_step_only)
+
+        # 2. draw exp distribution with intensity = intensity_upper_bound
+        # we apply fast approximation, i.e., re-use exp sample times for computation
+        # [batch_size, seq_len, num_exp]
+        exp_numbers = self.sample_exp_distribution(intensity_upper_bound)
+
+        # 3. compute intensity at sampled times from exp distribution
+        # [batch_size, seq_len, num_exp, event_num]
+        intensities_at_sampled_times = intensity_fn(time_seq,
+                                                    time_delta_seq,
+                                                    event_seq,
+                                                    exp_numbers,
+                                                    max_steps=time_seq.size(1),
+                                                    compute_last_step_only=compute_last_step_only)
+
+        # [batch_size, seq_len, num_exp]
+        total_intensities = intensities_at_sampled_times.sum(dim=-1)
+
+        # add one dim of num_sample: re-use the intensity for samples for prediction
+        # [batch_size, seq_len, num_sample, num_exp]
+        total_intensities = torch.tile(total_intensities[:, :, None, :], [1, 1, self.num_sample, 1])
+        # [batch_size, seq_len, num_sample, num_exp]
+        exp_numbers = torch.tile(exp_numbers[:, :, None, :], [1, 1, self.num_sample, 1])
+
+        # 4. draw uniform distribution
+        # [batch_size, seq_len, num_sample, num_exp]
+        unif_numbers = self.sample_uniform_distribution(intensity_upper_bound)
+
+        # 5. find out accepted intensities
+        # criterion, [batch_size, max_len, num_sample, num_exp]
+        # who_has_accepted_times, [batch_size, max_len, num_sample]
+        criterion, who_has_accepted_times = self.sample_accept(unif_numbers, intensity_upper_bound,
+                                                               total_intensities)
+
+        # 6. find out accepted dtimes
+        sampled_dtimes_accepted = exp_numbers.clone()
+
+        # for unaccepted, use boundary/maxsampletime for that draw
+        sampled_dtimes_accepted[criterion >= 1.0] = exp_numbers.max() + 1.0
+
+        accepted_times_each_draw, accepted_id_each_draw = sampled_dtimes_accepted.min(dim=-1)
+
+        # 7. fill out result
+        dtime_boundary_ = dtime_boundary[:, -1:] if compute_last_step_only else dtime_boundary
+
+        # [batch_size, seq_len, num_sample]
+        dtime_boundary_ = torch.tile(dtime_boundary_[..., None], [1, 1, self.num_sample])
+
+        # [batch_size, seq_len, num_sample]
+        res = torch.ones_like(dtime_boundary_) * dtime_boundary_
+
+        # [batch_size, seq_len, num_sample]
+        weights = torch.ones_like(dtime_boundary_)
+        weights /= weights.sum(dim=-1, keepdim=True)
+
+        res[who_has_accepted_times] = accepted_times_each_draw[who_has_accepted_times]
+        who_not_accept = ~who_has_accepted_times
+
+        who_reach_further = exp_numbers[..., -1] > dtime_boundary_
+
+        res[who_not_accept & who_reach_further] = exp_numbers[..., -1][who_not_accept & who_reach_further]
+
+        # add a upper bound here in case it explodes, e.g., in ODE models
+        return res.clamp(max=1e5), weights
```

### Comparing `easy_tpp-0.0.4/easy_tpp/preprocess/data_collator.py` & `easy_tpp-0.0.5/easy_tpp/preprocess/data_collator.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from dataclasses import dataclass
-from typing import Union, Optional
-
-from easy_tpp.preprocess.event_tokenizer import EventTokenizer
-from easy_tpp.utils import PaddingStrategy, TruncationStrategy
-
-
-@dataclass
-class TPPDataCollator:
-    """
-    Data collator that will dynamically pad the inputs of event sequences.
-
-    Args:
-        tokenizer ([`EventTokenizer`]):
-            The tokenizer used for encoding the data.
-        padding (`bool`, `str` or [`~utils.PaddingStrategy`], *optional*, defaults to `True`):
-            Select a strategy to pad the returned sequences (according to the model's padding side and padding index)
-            among:
-
-            - `True` or `'longest'` (default): Pad to the longest sequence in the batch (or no padding if only a single
-              sequence is provided).
-            - `'max_length'`: Pad to a maximum length specified with the argument `max_length` or to the maximum
-              acceptable input length for the model if that argument is not provided.
-            - `False` or `'do_not_pad'`: No padding (i.e., can output a batch with sequences of different lengths).
-        max_length (`int`, *optional*):
-            Maximum length of the returned list and optionally padding length (see above).
-        return_tensors (`str`):
-            The type of Tensor to return. Allowable values are "np", "pt" and "tf".
-    """
-
-    tokenizer: EventTokenizer
-    padding: Union[bool, str, PaddingStrategy] = True
-    max_length: Optional[int] = None
-    truncation: Union[bool, str, TruncationStrategy] = False
-    return_tensors: str = "pt"
-
-    def __call__(self, features, return_tensors=None):
-        if return_tensors is None:
-            return_tensors = self.return_tensors
-
-        batch = self.tokenizer.pad(
-            features,
-            padding=self.padding,
-            max_length=self.max_length,
-            truncation=self.truncation,
-            return_tensors=return_tensors,
-        )
-
-        return batch
+from dataclasses import dataclass
+from typing import Union, Optional
+
+from easy_tpp.preprocess.event_tokenizer import EventTokenizer
+from easy_tpp.utils import PaddingStrategy, TruncationStrategy
+
+
+@dataclass
+class TPPDataCollator:
+    """
+    Data collator that will dynamically pad the inputs of event sequences.
+
+    Args:
+        tokenizer ([`EventTokenizer`]):
+            The tokenizer used for encoding the data.
+        padding (`bool`, `str` or [`~utils.PaddingStrategy`], *optional*, defaults to `True`):
+            Select a strategy to pad the returned sequences (according to the model's padding side and padding index)
+            among:
+
+            - `True` or `'longest'` (default): Pad to the longest sequence in the batch (or no padding if only a single
+              sequence is provided).
+            - `'max_length'`: Pad to a maximum length specified with the argument `max_length` or to the maximum
+              acceptable input length for the model if that argument is not provided.
+            - `False` or `'do_not_pad'`: No padding (i.e., can output a batch with sequences of different lengths).
+        max_length (`int`, *optional*):
+            Maximum length of the returned list and optionally padding length (see above).
+        return_tensors (`str`):
+            The type of Tensor to return. Allowable values are "np", "pt" and "tf".
+    """
+
+    tokenizer: EventTokenizer
+    padding: Union[bool, str, PaddingStrategy] = True
+    max_length: Optional[int] = None
+    truncation: Union[bool, str, TruncationStrategy] = False
+    return_tensors: str = "pt"
+
+    def __call__(self, features, return_tensors=None):
+        if return_tensors is None:
+            return_tensors = self.return_tensors
+
+        batch = self.tokenizer.pad(
+            features,
+            padding=self.padding,
+            max_length=self.max_length,
+            truncation=self.truncation,
+            return_tensors=return_tensors,
+        )
+
+        return batch
```

### Comparing `easy_tpp-0.0.4/easy_tpp/preprocess/data_loader.py` & `easy_tpp-0.0.5/easy_tpp/preprocess/data_loader.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from easy_tpp.preprocess.dataset import TPPDataset
-from easy_tpp.preprocess.dataset import get_data_loader
-from easy_tpp.preprocess.event_tokenizer import EventTokenizer
-from easy_tpp.utils import load_pickle, py_assert
-
-
-class TPPDataLoader:
-    def __init__(self, data_config, backend, **kwargs):
-        """Initialize the dataloader
-
-        Args:
-            data_config (EasyTPP.DataConfig): data config.
-            backend (str): backend engine, e.g., tensorflow or torch.
-        """
-        self.data_config = data_config
-        self.num_event_types = data_config.data_specs.num_event_types
-        self.backend = backend
-        self.kwargs = kwargs
-
-    def build_input_from_pkl(self, source_dir: str, split: str):
-        data = load_pickle(source_dir)
-
-        py_assert(data["dim_process"] == self.num_event_types,
-                  ValueError,
-                  "inconsistent dim_process in different splits?")
-
-        source_data = data[split]
-        time_seqs = [[x["time_since_start"] for x in seq] for seq in source_data]
-        type_seqs = [[x["type_event"] for x in seq] for seq in source_data]
-        time_delta_seqs = [[x["time_since_last_event"] for x in seq] for seq in source_data]
-
-        input_dict = dict({'time_seqs': time_seqs, 'time_delta_seqs': time_delta_seqs, 'type_seqs': type_seqs})
-        return input_dict
-
-    def get_loader(self, split='train', **kwargs):
-        """Get the corresponding data loader.
-
-        Args:
-            split (str, optional): denote the train, valid and test set. Defaults to 'train'.
-            num_event_types (int, optional): num of event types in the data. Defaults to None.
-
-        Raises:
-            NotImplementedError: the input of 'num_event_types' is inconsistent with the data.
-
-        Returns:
-            EasyTPP.DataLoader: the data loader for tpp data.
-        """
-        data_dir = self.data_config.get_data_dir(split)
-        data_source_type = data_dir.split('.')[-1]
-
-        if data_source_type == 'pkl':
-            data = self.build_input_from_pkl(data_dir, split)
-            dataset = TPPDataset(data)
-            tokenizer = EventTokenizer(self.data_config.data_specs)
-            loader = get_data_loader(dataset,
-                                     self.backend,
-                                     tokenizer,
-                                     batch_size=self.kwargs['batch_size'],
-                                     shuffle=self.kwargs['shuffle'],
-                                     **kwargs)
-        else:
-            raise NotImplementedError
-
-        return loader
-
-    def train_loader(self, **kwargs):
-        """Return the train loader
-
-        Returns:
-            EasyTPP.DataLoader: data loader for train set.
-        """
-        return self.get_loader('train', **kwargs)
-
-    def valid_loader(self, **kwargs):
-        """Return the valid loader
-
-        Returns:
-            EasyTPP.DataLoader: data loader for valid set.
-        """
-        return self.get_loader('dev', **kwargs)
-
-    def test_loader(self, **kwargs):
-        """Return the test loader
-
-        Returns:
-            EasyTPP.DataLoader: data loader for test set.
-        """
-        return self.get_loader('test', **kwargs)
+from easy_tpp.preprocess.dataset import TPPDataset
+from easy_tpp.preprocess.dataset import get_data_loader
+from easy_tpp.preprocess.event_tokenizer import EventTokenizer
+from easy_tpp.utils import load_pickle, py_assert
+
+
+class TPPDataLoader:
+    def __init__(self, data_config, backend, **kwargs):
+        """Initialize the dataloader
+
+        Args:
+            data_config (EasyTPP.DataConfig): data config.
+            backend (str): backend engine, e.g., tensorflow or torch.
+        """
+        self.data_config = data_config
+        self.num_event_types = data_config.data_specs.num_event_types
+        self.backend = backend
+        self.kwargs = kwargs
+
+    def build_input_from_pkl(self, source_dir: str, split: str):
+        data = load_pickle(source_dir)
+
+        py_assert(data["dim_process"] == self.num_event_types,
+                  ValueError,
+                  "inconsistent dim_process in different splits?")
+
+        source_data = data[split]
+        time_seqs = [[x["time_since_start"] for x in seq] for seq in source_data]
+        type_seqs = [[x["type_event"] for x in seq] for seq in source_data]
+        time_delta_seqs = [[x["time_since_last_event"] for x in seq] for seq in source_data]
+
+        input_dict = dict({'time_seqs': time_seqs, 'time_delta_seqs': time_delta_seqs, 'type_seqs': type_seqs})
+        return input_dict
+
+    def get_loader(self, split='train', **kwargs):
+        """Get the corresponding data loader.
+
+        Args:
+            split (str, optional): denote the train, valid and test set. Defaults to 'train'.
+            num_event_types (int, optional): num of event types in the data. Defaults to None.
+
+        Raises:
+            NotImplementedError: the input of 'num_event_types' is inconsistent with the data.
+
+        Returns:
+            EasyTPP.DataLoader: the data loader for tpp data.
+        """
+        data_dir = self.data_config.get_data_dir(split)
+        data_source_type = data_dir.split('.')[-1]
+
+        if data_source_type == 'pkl':
+            data = self.build_input_from_pkl(data_dir, split)
+            dataset = TPPDataset(data)
+            tokenizer = EventTokenizer(self.data_config.data_specs)
+            loader = get_data_loader(dataset,
+                                     self.backend,
+                                     tokenizer,
+                                     batch_size=self.kwargs['batch_size'],
+                                     shuffle=self.kwargs['shuffle'],
+                                     **kwargs)
+        else:
+            raise NotImplementedError
+
+        return loader
+
+    def train_loader(self, **kwargs):
+        """Return the train loader
+
+        Returns:
+            EasyTPP.DataLoader: data loader for train set.
+        """
+        return self.get_loader('train', **kwargs)
+
+    def valid_loader(self, **kwargs):
+        """Return the valid loader
+
+        Returns:
+            EasyTPP.DataLoader: data loader for valid set.
+        """
+        return self.get_loader('dev', **kwargs)
+
+    def test_loader(self, **kwargs):
+        """Return the test loader
+
+        Returns:
+            EasyTPP.DataLoader: data loader for test set.
+        """
+        return self.get_loader('test', **kwargs)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/preprocess/dataset.py` & `easy_tpp-0.0.5/easy_tpp/preprocess/dataset.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import math
-from typing import Dict
-
-import numpy as np
-from torch.utils.data import Dataset, DataLoader
-
-from easy_tpp.preprocess.data_collator import TPPDataCollator
-from easy_tpp.preprocess.event_tokenizer import EventTokenizer
-from easy_tpp.utils import py_assert, is_tf_available
-
-
-class TPPDataset(Dataset):
-    def __init__(self, data: Dict):
-        self.data_dict = data
-        self.time_seqs = self.data_dict['time_seqs']
-        self.time_delta_seqs = self.data_dict['time_delta_seqs']
-        self.type_seqs = self.data_dict['type_seqs']
-
-    def __len__(self):
-        """
-
-        Returns: length of the dataset
-
-        """
-
-        py_assert(len(self.time_seqs) == len(self.type_seqs) and len(self.time_delta_seqs) == len(self.type_seqs),
-                  ValueError,
-                  f"Inconsistent lengths for data! time_seq_len:{len(self.time_seqs)}, event_len: "
-                  f"{len(self.type_seqs)}, time_delta_seq_len: {len(self.time_delta_seqs)}")
-
-        return len(self.time_seqs)
-
-    def __getitem__(self, idx):
-        """
-
-        Args:
-            idx: iteration index
-
-        Returns:
-            dict: a dict of time_seqs, time_delta_seqs and type_seqs element
-
-        """
-        return dict({'time_seqs': self.time_seqs[idx], 'time_delta_seqs': self.time_delta_seqs[idx],
-                     'type_seqs': self.type_seqs[idx]})
-
-    def to_tf_dataset(self, data_collator: TPPDataCollator, **kwargs):
-        """Generate a dataset to use in Tensorflow
-
-        Args:
-            data_collator (TPPDataCollator): collator to tokenize the event data.
-
-        Raises:
-            ImportError: Tensorflow is not installed.
-
-        Returns:
-            tf.keras.utils.Sequence: tf Dataset object for TPP data.
-        """
-        if is_tf_available():
-            import tensorflow as tf
-
-            if tf.__version__ >= '2.0':
-                tf = tf.compat.v1
-                tf.disable_v2_behavior()
-        else:
-            raise ImportError("Called a Tensorflow-specific function but Tensorflow is not installed.")
-
-        class TfTPPDataset(tf.keras.utils.Sequence):
-            def __init__(self, time_seqs, time_delta_seqs, type_seqs, **kwargs):
-                """Initialize the class.
-
-                Args:
-                    batch_size (int): size of batch.
-                    shuffle (bool): whether to shuffle the data in each batch.
-
-                """
-                self.time_seqs = time_seqs
-                self.time_delta_seqs = time_delta_seqs
-                self.type_seqs = type_seqs
-                self.data_len = len(self.time_delta_seqs)
-                self.batch_size = kwargs.pop('batch_size')
-                self.shuffle = kwargs.pop('shuffle', False)
-                self.idx = np.arange(self.data_len)
-                self.kwargs = kwargs
-
-            def __getitem__(self, index):
-                # get batch indexes from shuffled indexes
-                batch_idx = self.idx[index * self.batch_size:(index + 1) * self.batch_size]
-                batch = dict({'time_seqs': [self.time_seqs[i] for i in batch_idx],
-                              'time_delta_seqs': [self.time_delta_seqs[i] for i in batch_idx],
-                              'type_seqs': [self.type_seqs[i] for i in batch_idx]})
-
-                batch = data_collator(batch, **self.kwargs)
-                return batch
-
-            def __len__(self):
-                # Denotes the number of batches per epoch
-                return math.ceil(self.data_len / self.batch_size)
-
-            def on_epoch_end(self):
-                # Updates indexes after each epoch
-                self.idx = np.arange(self.data_len)
-                if self.shuffle:
-                    np.random.shuffle(self.idx)
-
-        return TfTPPDataset(self.time_seqs, self.time_delta_seqs, self.type_seqs, **kwargs)
-
-
-def get_data_loader(dataset: TPPDataset, backend: str, tokenizer: EventTokenizer, **kwargs):
-    use_torch = backend == 'torch'
-
-    padding = True if tokenizer.padding_strategy is None else tokenizer.padding_strategy
-    truncation = False if tokenizer.truncation_strategy is None else tokenizer.truncation_strategy
-
-    if use_torch:
-        data_collator = TPPDataCollator(tokenizer=tokenizer,
-                                        return_tensors='pt',
-                                        max_length=tokenizer.model_max_length,
-                                        padding=padding,
-                                        truncation=truncation)
-
-        return DataLoader(dataset,
-                          collate_fn=data_collator,
-                          **kwargs)
-    else:
-        # we pass to placeholders
-        data_collator = TPPDataCollator(tokenizer=tokenizer,
-                                        return_tensors='np',
-                                        max_length=tokenizer.model_max_length,
-                                        padding=padding,
-                                        truncation=truncation)
-
-        return dataset.to_tf_dataset(data_collator, **kwargs)
+import math
+from typing import Dict
+
+import numpy as np
+from torch.utils.data import Dataset, DataLoader
+
+from easy_tpp.preprocess.data_collator import TPPDataCollator
+from easy_tpp.preprocess.event_tokenizer import EventTokenizer
+from easy_tpp.utils import py_assert, is_tf_available
+
+
+class TPPDataset(Dataset):
+    def __init__(self, data: Dict):
+        self.data_dict = data
+        self.time_seqs = self.data_dict['time_seqs']
+        self.time_delta_seqs = self.data_dict['time_delta_seqs']
+        self.type_seqs = self.data_dict['type_seqs']
+
+    def __len__(self):
+        """
+
+        Returns: length of the dataset
+
+        """
+
+        py_assert(len(self.time_seqs) == len(self.type_seqs) and len(self.time_delta_seqs) == len(self.type_seqs),
+                  ValueError,
+                  f"Inconsistent lengths for data! time_seq_len:{len(self.time_seqs)}, event_len: "
+                  f"{len(self.type_seqs)}, time_delta_seq_len: {len(self.time_delta_seqs)}")
+
+        return len(self.time_seqs)
+
+    def __getitem__(self, idx):
+        """
+
+        Args:
+            idx: iteration index
+
+        Returns:
+            dict: a dict of time_seqs, time_delta_seqs and type_seqs element
+
+        """
+        return dict({'time_seqs': self.time_seqs[idx], 'time_delta_seqs': self.time_delta_seqs[idx],
+                     'type_seqs': self.type_seqs[idx]})
+
+    def to_tf_dataset(self, data_collator: TPPDataCollator, **kwargs):
+        """Generate a dataset to use in Tensorflow
+
+        Args:
+            data_collator (TPPDataCollator): collator to tokenize the event data.
+
+        Raises:
+            ImportError: Tensorflow is not installed.
+
+        Returns:
+            tf.keras.utils.Sequence: tf Dataset object for TPP data.
+        """
+        if is_tf_available():
+            import tensorflow as tf
+
+            if tf.__version__ >= '2.0':
+                tf = tf.compat.v1
+                tf.disable_v2_behavior()
+        else:
+            raise ImportError("Called a Tensorflow-specific function but Tensorflow is not installed.")
+
+        class TfTPPDataset(tf.keras.utils.Sequence):
+            def __init__(self, time_seqs, time_delta_seqs, type_seqs, **kwargs):
+                """Initialize the class.
+
+                Args:
+                    batch_size (int): size of batch.
+                    shuffle (bool): whether to shuffle the data in each batch.
+
+                """
+                self.time_seqs = time_seqs
+                self.time_delta_seqs = time_delta_seqs
+                self.type_seqs = type_seqs
+                self.data_len = len(self.time_delta_seqs)
+                self.batch_size = kwargs.pop('batch_size')
+                self.shuffle = kwargs.pop('shuffle', False)
+                self.idx = np.arange(self.data_len)
+                self.kwargs = kwargs
+
+            def __getitem__(self, index):
+                # get batch indexes from shuffled indexes
+                batch_idx = self.idx[index * self.batch_size:(index + 1) * self.batch_size]
+                batch = dict({'time_seqs': [self.time_seqs[i] for i in batch_idx],
+                              'time_delta_seqs': [self.time_delta_seqs[i] for i in batch_idx],
+                              'type_seqs': [self.type_seqs[i] for i in batch_idx]})
+
+                batch = data_collator(batch, **self.kwargs)
+                return batch
+
+            def __len__(self):
+                # Denotes the number of batches per epoch
+                return math.ceil(self.data_len / self.batch_size)
+
+            def on_epoch_end(self):
+                # Updates indexes after each epoch
+                self.idx = np.arange(self.data_len)
+                if self.shuffle:
+                    np.random.shuffle(self.idx)
+
+        return TfTPPDataset(self.time_seqs, self.time_delta_seqs, self.type_seqs, **kwargs)
+
+
+def get_data_loader(dataset: TPPDataset, backend: str, tokenizer: EventTokenizer, **kwargs):
+    use_torch = backend == 'torch'
+
+    padding = True if tokenizer.padding_strategy is None else tokenizer.padding_strategy
+    truncation = False if tokenizer.truncation_strategy is None else tokenizer.truncation_strategy
+
+    if use_torch:
+        data_collator = TPPDataCollator(tokenizer=tokenizer,
+                                        return_tensors='pt',
+                                        max_length=tokenizer.model_max_length,
+                                        padding=padding,
+                                        truncation=truncation)
+
+        return DataLoader(dataset,
+                          collate_fn=data_collator,
+                          **kwargs)
+    else:
+        # we pass to placeholders
+        data_collator = TPPDataCollator(tokenizer=tokenizer,
+                                        return_tensors='np',
+                                        max_length=tokenizer.model_max_length,
+                                        padding=padding,
+                                        truncation=truncation)
+
+        return dataset.to_tf_dataset(data_collator, **kwargs)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/preprocess/event_tokenizer.py` & `easy_tpp-0.0.5/easy_tpp/preprocess/event_tokenizer.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,557 +1,557 @@
-import copy
-from collections import UserDict
-from typing import Optional, Union, Dict, Any, List, Mapping
-
-import numpy as np
-
-from easy_tpp.utils import is_torch_available, is_tf_available, logger, TruncationStrategy, PaddingStrategy, \
-    TensorType, is_torch_device, requires_backends, is_numpy_array, py_assert
-
-
-class BatchEncoding(UserDict):
-    """
-    Holds the output of the [`~event_tokenizer.EventTokenizer.__call__`],
-    [`~event_tokenizer.EventTokenizer.encode_plus`] methods (tokens, attention_masks, etc).
-
-    This class is derived from a python dictionary and can be used as a dictionary.
-
-    Args:
-        data (`dict`):
-            Dictionary of lists/arrays/tensors returned by the `__call__`/`encode_plus`/`batch_encode_plus` methods
-            ('input_ids', 'attention_mask', etc.).
-        tensor_type (`Union[None, str, TensorType]`, *optional*):
-            You can give a tensor_type here to convert the lists of integers in PyTorch/TensorFlow/Numpy Tensors at
-            initialization.
-        prepend_batch_axis (`bool`, *optional*, defaults to `False`):
-            Whether or not to add a batch axis when converting to tensors (see `tensor_type` above).
-        n_sequences (`Optional[int]`, *optional*):
-            You can give a tensor_type here to convert the lists of integers in PyTorch/TensorFlow/Numpy Tensors at
-            initialization.
-    """
-
-    def __init__(
-            self,
-            data: Optional[Dict[str, Any]] = None,
-            tensor_type: Union[None, str, TensorType] = None,
-            prepend_batch_axis: bool = False
-    ):
-        super().__init__(data)
-
-        self.convert_to_tensors(tensor_type=tensor_type, prepend_batch_axis=prepend_batch_axis)
-
-    def keys(self):
-        return self.data.keys()
-
-    def values(self):
-        return list(self.data.values())
-
-    def items(self):
-        return self.data.items()
-
-    def convert_to_tensors(
-            self, tensor_type: Optional[Union[str, TensorType]] = None, prepend_batch_axis: bool = False
-    ):
-        """
-        Convert the inner content to tensors.
-
-        Args:
-            tensor_type (`str` or [`~utils.TensorType`], *optional*):
-                The type of tensors to use. If `str`, should be one of the values of the enum [`~utils.TensorType`]. If
-                `None`, no modification is done.
-            prepend_batch_axis (`int`, *optional*, defaults to `False`):
-                Whether or not to add the batch dimension during the conversion.
-        """
-        if tensor_type is None:
-            return self
-
-        # Convert to TensorType
-        if not isinstance(tensor_type, TensorType):
-            tensor_type = TensorType(tensor_type)
-
-        # Get a function reference for the correct framework
-        if tensor_type == TensorType.TENSORFLOW:
-            if not is_tf_available():
-                raise ImportError(
-                    "Unable to convert output to TensorFlow tensors format, TensorFlow is not installed."
-                )
-            import tensorflow as tf
-
-            as_tensor = tf.constant
-            is_tensor = tf.is_tensor
-        elif tensor_type == TensorType.PYTORCH:
-            if not is_torch_available():
-                raise ImportError("Unable to convert output to PyTorch tensors format, PyTorch is not installed.")
-            import torch
-
-            as_tensor = torch.tensor
-            is_tensor = torch.is_tensor
-        else:
-            as_tensor = np.asarray
-            is_tensor = is_numpy_array
-
-        # Do the tensor conversion in batch
-        for key, value in self.items():
-            try:
-                if prepend_batch_axis:
-                    value = [value]
-
-                if not is_tensor(value):
-                    tensor = as_tensor(value)
-
-                    self[key] = tensor
-            except Exception as e:
-                if key == "overflowing_tokens":
-                    raise ValueError(
-                        "Unable to create tensor returning overflowing tokens of different lengths. "
-                        "Please see if a fast version of this tokenizer is available to have this feature available."
-                    ) from e
-                raise ValueError(
-                    "Unable to create tensor, you should probably activate truncation and/or padding with"
-                    " 'padding=True' 'truncation=True' to have batched tensors with the same length. Perhaps your"
-                    f" features (`{key}` in this case) have excessive nesting (inputs type `list` where type `int` is"
-                    " expected)."
-                ) from e
-
-        return self
-
-    def to(self, device: Union[str, "torch.device"]) -> "BatchEncoding":
-        """
-        Send all values to device by calling `v.to(device)` (PyTorch only).
-
-        Args:
-            device (`str` or `torch.device`): The device to put the tensors on.
-
-        Returns:
-            [`BatchEncoding`]: The same instance after modification.
-        """
-        requires_backends(self, ["torch"])
-
-        # This check catches things like APEX blindly calling "to" on all inputs to a module
-        # Otherwise it passes the casts down and casts the LongTensor containing the token idxs
-        # into a HalfTensor
-        if isinstance(device, str) or is_torch_device(device) or isinstance(device, int):
-            self.data = {k: v.to(device=device) for k, v in self.data.items()}
-        else:
-            logger.warning(f"Attempting to cast a BatchEncoding to type {str(device)}. This is not supported.")
-        return self
-
-
-class EventTokenizer:
-    """
-    Base class for tokenizer event sequences, vendored from huggingface/transformer
-    """
-    padding_side: str = "right"
-    truncation_side: str = "right"
-    model_input_names: List[str] = ["time_seqs", "time_delta_seqs", "type_seqs", "seq_non_pad_mask", "attention_mask",
-                                    "type_mask"]
-
-    def __init__(self, config):
-        config = copy.deepcopy(config)
-        self.num_event_types = config.num_event_types
-        self.pad_token_id = config.pad_token_id
-
-        self.model_max_length = config.max_len
-
-        self.padding_strategy = config.padding_strategy
-        self.truncation_strategy = config.truncation_strategy
-
-        # Padding and truncation side are right by default and overridden in subclasses. If specified in the kwargs, it
-        # is changed.
-        self.padding_side = config.pop("padding_side", self.padding_side)
-        self.truncation_side = config.pop("truncation_side", self.truncation_side)
-        self.model_input_names = config.pop("model_input_names", self.model_input_names)
-
-    def _get_padding_truncation_strategies(
-            self, padding=False, truncation=None, max_length=None, verbose=False, **kwargs
-    ):
-        padding_strategy, truncation_strategy = None, None
-        # If you only set max_length, it activates truncation for max_length
-        if max_length is not None and padding is False and truncation is None:
-            if verbose:
-                logger.warning(
-                    "Truncation was not explicitly activated but `max_length` is provided a specific value, please"
-                    " use `truncation=True` to explicitly truncate examples to max length. Defaulting to"
-                    " 'longest_first' truncation strategy"
-                )
-            truncation = "longest_first"
-
-        # Get padding strategy
-        if padding is False:
-            if max_length is None:
-                padding_strategy = PaddingStrategy.LONGEST
-            else:
-                padding_strategy = PaddingStrategy.MAX_LENGTH
-        elif padding is not False:
-            if padding is True:
-                if verbose:
-                    if max_length is not None and (
-                            truncation is None or truncation is False or truncation == "do_not_truncate"
-                    ):
-                        logger.warn(
-                            "`max_length` is ignored when `padding`=`True` and there is no truncation strategy. "
-                            "To pad to max length, use `padding='max_length'`."
-                        )
-                padding_strategy = PaddingStrategy.LONGEST  # Default to pad to the longest sequence in the batch
-            elif not isinstance(padding, PaddingStrategy):
-                padding_strategy = PaddingStrategy(padding)
-            elif isinstance(padding, PaddingStrategy):
-                padding_strategy = padding
-        else:
-            padding_strategy = PaddingStrategy.DO_NOT_PAD
-
-        # Get truncation strategy
-        if truncation is not None and truncation is not False:
-            if truncation is True:
-                truncation_strategy = (
-                    TruncationStrategy.LONGEST_FIRST
-                )  # Default to truncate the longest sequences in pairs of inputs
-            elif not isinstance(truncation, TruncationStrategy):
-                truncation_strategy = TruncationStrategy(truncation)
-            elif isinstance(truncation, TruncationStrategy):
-                truncation_strategy = truncation
-        else:
-            truncation_strategy = TruncationStrategy.DO_NOT_TRUNCATE
-
-        # Set max length if needed
-        if max_length is None:
-            if padding_strategy == PaddingStrategy.MAX_LENGTH:
-                max_length = self.model_max_length
-            if truncation_strategy != TruncationStrategy.DO_NOT_TRUNCATE:
-                max_length = self.model_max_length
-
-        # Test if we have a padding token
-        if padding_strategy != PaddingStrategy.DO_NOT_PAD and (not self.pad_token_id):
-            raise ValueError(
-                "Asking to pad but the tokenizer does not have a padding token. "
-                "Please select a token to use as `pad_token` `(tokenizer.pad_token = tokenizer.eos_token e.g.)` "
-                "or add a new pad token via `tokenizer.add_special_tokens({'pad_token': '[PAD]'})`."
-            )
-
-        return padding_strategy, truncation_strategy, max_length, kwargs
-
-    def _truncate(self,
-                  encoded_inputs: Union[Dict[str, Any],
-                                        Dict[str, List]],
-                  truncation_strategy: TruncationStrategy,
-                  truncation_side: str,
-                  max_length: Optional[int] = None):
-        if truncation_strategy != TruncationStrategy.DO_NOT_TRUNCATE:
-            py_assert(max_length is not None, ValueError, 'must pass max_length when truncation is activated!')
-            for k, v in encoded_inputs.items():
-                seq_ = [seq[:max_length] for seq in v] if truncation_side == 'right' \
-                    else [seq[-max_length:] for seq in v]
-                encoded_inputs[k] = seq_
-
-        return encoded_inputs
-
-    def pad(
-            self,
-            encoded_inputs: Union[
-                Dict[str, Any],
-                Dict[str, List],
-            ],
-            padding: Union[bool, str, PaddingStrategy] = True,
-            truncation: Union[bool, str, TruncationStrategy] = False,
-            max_length: Optional[int] = None,
-            return_attention_mask: Optional[bool] = None,
-            return_tensors: Optional[Union[str, TensorType]] = None,
-            verbose: bool = False,
-    ) -> BatchEncoding:
-        """
-        Pad a single encoded input or a batch of encoded inputs up to predefined length or to the max sequence length
-        in the batch.
-
-        Padding side (left/right) padding token ids are defined at the tokenizer level (with `self.padding_side`,
-        `self.pad_token_id` and `self.pad_token_type_id`).
-
-        Please note that with a fast tokenizer, using the `__call__` method is faster than using a method to encode the
-        text followed by a call to the `pad` method to get a padded encoding.
-
-        <Tip>
-
-        If the `encoded_inputs` passed are dictionary of numpy arrays, PyTorch tensors or TensorFlow tensors, the
-        result will use the same type unless you provide a different tensor type with `return_tensors`. In the case of
-        PyTorch tensors, you will lose the specific device of your tensors however.
-
-        </Tip>
-
-        Args:
-            encoded_inputs ([`BatchEncoding`], list of [`BatchEncoding`]:
-                Tokenized inputs. Can represent one input ([`BatchEncoding`] or `Dict[str, List[int]]`) or a batch of
-                tokenized inputs (list of [`BatchEncoding`], *Dict[str, List[List[int]]]* or *List[Dict[str,
-                List[int]]]*) so you can use this method during preprocessing as well as in a PyTorch Dataloader
-                collate function.
-
-                Instead of `List[int]` you can have tensors (numpy arrays, PyTorch tensors or TensorFlow tensors), see
-                the note above for the return type.
-            padding (`bool`, `str` or [`~utils.PaddingStrategy`], *optional*, defaults to `True`):
-                 Select a strategy to pad the returned sequences (according to the model's padding side and padding
-                 index) among:
-
-                - `True` or `'longest'`: Pad to the longest sequence in the batch (or no padding if only a single
-                  sequence if provided).
-                - `'max_length'`: Pad to a maximum length specified with the argument `max_length` or to the maximum
-                  acceptable input length for the model if that argument is not provided.
-                - `False` or `'do_not_pad'` (default): No padding (i.e., can output a batch with sequences of different
-                  lengths).
-            max_length (`int`, *optional*):
-                Maximum length of the returned list and optionally padding length (see above).
-            return_attention_mask (`bool`, *optional*):
-                Whether to return the attention mask. If left to the default, will return the attention mask according
-                to the specific tokenizer's default, defined by the `return_outputs` attribute.
-
-            return_tensors (`str` or [`~utils.TensorType`], *optional*):
-                If set, will return tensors instead of list of python integers. Acceptable values are:
-
-                - `'tf'`: Return TensorFlow `tf.constant` objects.
-                - `'pt'`: Return PyTorch `torch.Tensor` objects.
-                - `'np'`: Return Numpy `np.ndarray` objects.
-            verbose (`bool`, *optional*, defaults to `True`):
-                Whether or not to print more information and warnings.
-        """
-
-        # If we have a list of dicts, let's convert it in a dict of lists
-        # We do this to allow using this method as a collate_fn function in PyTorch Dataloader
-        if isinstance(encoded_inputs, (list, tuple)) and isinstance(encoded_inputs[0], Mapping):
-            encoded_inputs = {key: [example[key] for example in encoded_inputs] for key in encoded_inputs[0].keys()}
-
-        # The model's main input name, usually `time_seqs`, has be passed for padding
-        if self.model_input_names[0] not in encoded_inputs:
-            raise ValueError(
-                "You should supply an encoding or a list of encodings to this method "
-                f"that includes {self.model_input_names[0]}, but you provided {list(encoded_inputs.keys())}"
-            )
-
-        required_input = encoded_inputs[self.model_input_names[0]]
-
-        padding_strategy, truncation_strategy, max_length, _ = self._get_padding_truncation_strategies(
-            padding=padding, max_length=max_length, truncation=truncation, verbose=verbose
-        )
-
-        encoded_inputs = self._truncate(encoded_inputs,
-                                        truncation_strategy=truncation_strategy,
-                                        max_length=max_length,
-                                        truncation_side=self.truncation_side)
-
-        batch_size = len(required_input)
-        assert all(
-            len(v) == batch_size for v in encoded_inputs.values()
-        ), "Some items in the output dictionary have a different batch size than others."
-
-        if padding_strategy == PaddingStrategy.LONGEST:
-            max_length = max(len(inputs) for inputs in required_input)
-            padding_strategy = PaddingStrategy.MAX_LENGTH
-
-        batch_output = self._pad(
-            encoded_inputs,
-            max_length=max_length,
-            padding_strategy=padding_strategy,
-            return_attention_mask=return_attention_mask,
-        )
-
-        return BatchEncoding(batch_output, tensor_type=return_tensors)
-
-    def _pad(
-            self,
-            encoded_inputs: Union[Dict[str, Any], BatchEncoding],
-            max_length: Optional[int] = None,
-            padding_strategy: PaddingStrategy = PaddingStrategy.DO_NOT_PAD,
-            return_attention_mask: Optional[bool] = None,
-    ) -> dict:
-        """
-        Pad encoded inputs (on left/right and up to predefined length or max length in the batch)
-
-        Args:
-            encoded_inputs:
-                Dictionary of tokenized inputs (`List[int]`) or batch of tokenized inputs (`List[List[int]]`).
-            max_length: maximum length of the returned list and optionally padding length (see below).
-                Will truncate by taking into account the special tokens.
-            padding_strategy: PaddingStrategy to use for padding.
-
-                - PaddingStrategy.LONGEST Pad to the longest sequence in the batch
-                - PaddingStrategy.MAX_LENGTH: Pad to the max length (default)
-                - PaddingStrategy.DO_NOT_PAD: Do not pad
-                The tokenizer padding sides are defined in self.padding_side:
-
-                    - 'left': pads on the left of the sequences
-                    - 'right': pads on the right of the sequences
-            pad_to_multiple_of: (optional) Integer if set will pad the sequence to a multiple of the provided value.
-                This is especially useful to enable the use of Tensor Core on NVIDIA hardware with compute capability
-                `>= 7.5` (Volta).
-            return_attention_mask:
-                (optional) Set to False to avoid returning attention mask (default: set to model specifics)
-        """
-        # Load from model defaults
-        if return_attention_mask is None:
-            return_attention_mask = "attention_mask" in self.model_input_names
-
-        required_input = encoded_inputs[self.model_input_names[0]]
-
-        if padding_strategy == PaddingStrategy.LONGEST:
-            max_length = len(required_input)
-
-        # check whether we need to pad it
-        is_all_seq_equal_max_length = [len(seq) == max_length for seq in required_input]
-        is_all_seq_equal_max_length = np.prod(is_all_seq_equal_max_length)
-        needs_to_be_padded = padding_strategy != PaddingStrategy.DO_NOT_PAD and ~is_all_seq_equal_max_length
-
-        batch_output = dict()
-
-        if needs_to_be_padded:
-            # time seqs
-            batch_output[self.model_input_names[0]] = self.make_pad_sequence(encoded_inputs[self.model_input_names[0]],
-                                                                             self.pad_token_id,
-                                                                             padding_side=self.padding_side,
-                                                                             max_len=max_length)
-            # time_delta seqs
-            batch_output[self.model_input_names[1]] = self.make_pad_sequence(encoded_inputs[self.model_input_names[1]],
-                                                                             self.pad_token_id,
-                                                                             padding_side=self.padding_side,
-                                                                             max_len=max_length)
-            # type_seqs
-            batch_output[self.model_input_names[2]] = self.make_pad_sequence(encoded_inputs[self.model_input_names[2]],
-                                                                             self.pad_token_id,
-                                                                             padding_side=self.padding_side,
-                                                                             max_len=max_length,
-                                                                             dtype=np.int32)
-        else:
-            batch_output = encoded_inputs
-
-        # non_pad_mask
-        # we must use type seqs to check the mask, because the pad_token_id maybe one of valid values in
-        # time seqs
-        seq_pad_mask = batch_output[self.model_input_names[2]] == self.pad_token_id
-        batch_output[self.model_input_names[3]] = ~ seq_pad_mask
-
-        if return_attention_mask:
-            # attention_mask
-            batch_output[self.model_input_names[4]] = self.make_attn_mask_for_pad_sequence(
-                batch_output[self.model_input_names[2]],
-                self.pad_token_id)
-        else:
-            batch_output[self.model_input_names[4]] = []
-
-        # type_mask
-        batch_output[self.model_input_names[5]] = self.make_type_mask_for_pad_sequence(
-            batch_output[self.model_input_names[2]])
-
-        return batch_output
-
-    @staticmethod
-    def make_pad_sequence(seqs,
-                          pad_token_id,
-                          padding_side,
-                          max_len,
-                          dtype=np.float32,
-                          group_by_event_types=False):
-        """Pad the sequence batch-wise.
-
-        Args:
-            seqs (list): list of sequences with variational length
-            pad_token_id (int, float): optional, a value that used to pad the sequences. If None, then the pad index
-            is set to be the event_num_with_pad
-            max_len (int): optional, the maximum length of the sequence after padding. If None, then the
-            length is set to be the max length of all input sequences.
-            pad_at_end (bool): optional, whether to pad the sequnce at the end. If False,
-            the sequence is pad at the beginning
-
-        Returns:
-            a numpy array of padded sequence
-
-
-        Example:
-        ```python
-        seqs = [[0, 1], [3, 4, 5]]
-        pad_sequence(seqs, 100)
-        >>> [[0, 1, 100], [3, 4, 5]]
-
-        pad_sequence(seqs, 100, max_len=5)
-        >>> [[0, 1, 100, 100, 100], [3, 4, 5, 100, 100]]
-        ```
-
-        """
-        if not group_by_event_types:
-            if padding_side == "right":
-                pad_seq = np.array([seq + [pad_token_id] * (max_len - len(seq)) for seq in seqs], dtype=dtype)
-            else:
-                pad_seq = np.array([[pad_token_id] * (max_len - len(seq)) + seq for seq in seqs], dtype=dtype)
-        else:
-            pad_seq = []
-            for seq in seqs:
-                if padding_side == "right":
-                    pad_seq.append(np.array([s + [pad_token_id] * (max_len - len(s)) for s in seq], dtype=dtype))
-                else:
-                    pad_seq.append(np.array([[pad_token_id] * (max_len - len(s)) + s for s in seqs], dtype=dtype))
-
-            pad_seq = np.array(pad_seq)
-        return pad_seq
-
-    def make_attn_mask_for_pad_sequence(self, pad_seqs, pad_token_id):
-        """Make the attention masks for the sequence.
-
-        Args:
-            pad_seqs (tensor): list of sequences that have been padded with fixed length
-            pad_token_id (int): optional, a value that used to pad the sequences. If None, then the pad index
-            is set to be the event_num_with_pad
-
-        Returns:
-            np.array: a bool matrix of the same size of input, denoting the masks of the
-            sequence (True: non mask, False: mask)
-
-
-        Example:
-        ```python
-        seqs = [[ 1,  6,  0,  7, 12, 12],
-        [ 1,  0,  5,  1, 10,  9]]
-        make_attn_mask_for_pad_sequence(seqs, pad_index=12)
-        >>>
-            batch_non_pad_mask
-            ([[ True,  True,  True,  True, False, False],
-            [ True,  True,  True,  True,  True,  True]])
-            attention_mask
-            [[[ True  True  True  True  True  True]
-              [False  True  True  True  True  True]
-              [False False  True  True  True  True]
-              [False False False  True  True  True]
-              [False False False False  True  True]
-              [False False False False  True  True]]
-
-             [[ True  True  True  True  True  True]
-              [False  True  True  True  True  True]
-              [False False  True  True  True  True]
-              [False False False  True  True  True]
-              [False False False False  True  True]
-              [False False False False False  True]]]
-        ```
-
-
-        """
-
-        seq_num, seq_len = pad_seqs.shape
-
-        # [batch_size, seq_len]
-        seq_pad_mask = pad_seqs == pad_token_id
-
-        # [batch_size, seq_len, seq_len]
-        attention_key_pad_mask = np.tile(seq_pad_mask[:, None, :], (1, seq_len, 1))
-        subsequent_mask = np.tile(np.triu(np.ones((seq_len, seq_len), dtype=bool), k=0)[None, :, :], (seq_num, 1, 1))
-
-        attention_mask = subsequent_mask | attention_key_pad_mask
-
-        return attention_mask
-
-    def make_type_mask_for_pad_sequence(self, pad_seqs):
-        """Make the type mask.
-
-        Args:
-            pad_seqs (tensor): a list of sequence events with equal length (i.e., padded sequence)
-
-        Returns:
-            np.array: a 3-dim matrix, where the last dim (one-hot vector) indicates the type of event
-
-        """
-        type_mask = np.zeros([*pad_seqs.shape, self.num_event_types])
-        for i in range(self.num_event_types):
-            type_mask[:, :, i] = pad_seqs == i
-
-        return type_mask
+import copy
+from collections import UserDict
+from typing import Optional, Union, Dict, Any, List, Mapping
+
+import numpy as np
+
+from easy_tpp.utils import is_torch_available, is_tf_available, logger, TruncationStrategy, PaddingStrategy, \
+    TensorType, is_torch_device, requires_backends, is_numpy_array, py_assert
+
+
+class BatchEncoding(UserDict):
+    """
+    Holds the output of the [`~event_tokenizer.EventTokenizer.__call__`],
+    [`~event_tokenizer.EventTokenizer.encode_plus`] methods (tokens, attention_masks, etc).
+
+    This class is derived from a python dictionary and can be used as a dictionary.
+
+    Args:
+        data (`dict`):
+            Dictionary of lists/arrays/tensors returned by the `__call__`/`encode_plus`/`batch_encode_plus` methods
+            ('input_ids', 'attention_mask', etc.).
+        tensor_type (`Union[None, str, TensorType]`, *optional*):
+            You can give a tensor_type here to convert the lists of integers in PyTorch/TensorFlow/Numpy Tensors at
+            initialization.
+        prepend_batch_axis (`bool`, *optional*, defaults to `False`):
+            Whether or not to add a batch axis when converting to tensors (see `tensor_type` above).
+        n_sequences (`Optional[int]`, *optional*):
+            You can give a tensor_type here to convert the lists of integers in PyTorch/TensorFlow/Numpy Tensors at
+            initialization.
+    """
+
+    def __init__(
+            self,
+            data: Optional[Dict[str, Any]] = None,
+            tensor_type: Union[None, str, TensorType] = None,
+            prepend_batch_axis: bool = False
+    ):
+        super().__init__(data)
+
+        self.convert_to_tensors(tensor_type=tensor_type, prepend_batch_axis=prepend_batch_axis)
+
+    def keys(self):
+        return self.data.keys()
+
+    def values(self):
+        return list(self.data.values())
+
+    def items(self):
+        return self.data.items()
+
+    def convert_to_tensors(
+            self, tensor_type: Optional[Union[str, TensorType]] = None, prepend_batch_axis: bool = False
+    ):
+        """
+        Convert the inner content to tensors.
+
+        Args:
+            tensor_type (`str` or [`~utils.TensorType`], *optional*):
+                The type of tensors to use. If `str`, should be one of the values of the enum [`~utils.TensorType`]. If
+                `None`, no modification is done.
+            prepend_batch_axis (`int`, *optional*, defaults to `False`):
+                Whether or not to add the batch dimension during the conversion.
+        """
+        if tensor_type is None:
+            return self
+
+        # Convert to TensorType
+        if not isinstance(tensor_type, TensorType):
+            tensor_type = TensorType(tensor_type)
+
+        # Get a function reference for the correct framework
+        if tensor_type == TensorType.TENSORFLOW:
+            if not is_tf_available():
+                raise ImportError(
+                    "Unable to convert output to TensorFlow tensors format, TensorFlow is not installed."
+                )
+            import tensorflow as tf
+
+            as_tensor = tf.constant
+            is_tensor = tf.is_tensor
+        elif tensor_type == TensorType.PYTORCH:
+            if not is_torch_available():
+                raise ImportError("Unable to convert output to PyTorch tensors format, PyTorch is not installed.")
+            import torch
+
+            as_tensor = torch.tensor
+            is_tensor = torch.is_tensor
+        else:
+            as_tensor = np.asarray
+            is_tensor = is_numpy_array
+
+        # Do the tensor conversion in batch
+        for key, value in self.items():
+            try:
+                if prepend_batch_axis:
+                    value = [value]
+
+                if not is_tensor(value):
+                    tensor = as_tensor(value)
+
+                    self[key] = tensor
+            except Exception as e:
+                if key == "overflowing_tokens":
+                    raise ValueError(
+                        "Unable to create tensor returning overflowing tokens of different lengths. "
+                        "Please see if a fast version of this tokenizer is available to have this feature available."
+                    ) from e
+                raise ValueError(
+                    "Unable to create tensor, you should probably activate truncation and/or padding with"
+                    " 'padding=True' 'truncation=True' to have batched tensors with the same length. Perhaps your"
+                    f" features (`{key}` in this case) have excessive nesting (inputs type `list` where type `int` is"
+                    " expected)."
+                ) from e
+
+        return self
+
+    def to(self, device: Union[str, "torch.device"]) -> "BatchEncoding":
+        """
+        Send all values to device by calling `v.to(device)` (PyTorch only).
+
+        Args:
+            device (`str` or `torch.device`): The device to put the tensors on.
+
+        Returns:
+            [`BatchEncoding`]: The same instance after modification.
+        """
+        requires_backends(self, ["torch"])
+
+        # This check catches things like APEX blindly calling "to" on all inputs to a module
+        # Otherwise it passes the casts down and casts the LongTensor containing the token idxs
+        # into a HalfTensor
+        if isinstance(device, str) or is_torch_device(device) or isinstance(device, int):
+            self.data = {k: v.to(device=device) for k, v in self.data.items()}
+        else:
+            logger.warning(f"Attempting to cast a BatchEncoding to type {str(device)}. This is not supported.")
+        return self
+
+
+class EventTokenizer:
+    """
+    Base class for tokenizer event sequences, vendored from huggingface/transformer
+    """
+    padding_side: str = "right"
+    truncation_side: str = "right"
+    model_input_names: List[str] = ["time_seqs", "time_delta_seqs", "type_seqs", "seq_non_pad_mask", "attention_mask",
+                                    "type_mask"]
+
+    def __init__(self, config):
+        config = copy.deepcopy(config)
+        self.num_event_types = config.num_event_types
+        self.pad_token_id = config.pad_token_id
+
+        self.model_max_length = config.max_len
+
+        self.padding_strategy = config.padding_strategy
+        self.truncation_strategy = config.truncation_strategy
+
+        # Padding and truncation side are right by default and overridden in subclasses. If specified in the kwargs, it
+        # is changed.
+        self.padding_side = config.pop("padding_side", self.padding_side)
+        self.truncation_side = config.pop("truncation_side", self.truncation_side)
+        self.model_input_names = config.pop("model_input_names", self.model_input_names)
+
+    def _get_padding_truncation_strategies(
+            self, padding=False, truncation=None, max_length=None, verbose=False, **kwargs
+    ):
+        padding_strategy, truncation_strategy = None, None
+        # If you only set max_length, it activates truncation for max_length
+        if max_length is not None and padding is False and truncation is None:
+            if verbose:
+                logger.warning(
+                    "Truncation was not explicitly activated but `max_length` is provided a specific value, please"
+                    " use `truncation=True` to explicitly truncate examples to max length. Defaulting to"
+                    " 'longest_first' truncation strategy"
+                )
+            truncation = "longest_first"
+
+        # Get padding strategy
+        if padding is False:
+            if max_length is None:
+                padding_strategy = PaddingStrategy.LONGEST
+            else:
+                padding_strategy = PaddingStrategy.MAX_LENGTH
+        elif padding is not False:
+            if padding is True:
+                if verbose:
+                    if max_length is not None and (
+                            truncation is None or truncation is False or truncation == "do_not_truncate"
+                    ):
+                        logger.warn(
+                            "`max_length` is ignored when `padding`=`True` and there is no truncation strategy. "
+                            "To pad to max length, use `padding='max_length'`."
+                        )
+                padding_strategy = PaddingStrategy.LONGEST  # Default to pad to the longest sequence in the batch
+            elif not isinstance(padding, PaddingStrategy):
+                padding_strategy = PaddingStrategy(padding)
+            elif isinstance(padding, PaddingStrategy):
+                padding_strategy = padding
+        else:
+            padding_strategy = PaddingStrategy.DO_NOT_PAD
+
+        # Get truncation strategy
+        if truncation is not None and truncation is not False:
+            if truncation is True:
+                truncation_strategy = (
+                    TruncationStrategy.LONGEST_FIRST
+                )  # Default to truncate the longest sequences in pairs of inputs
+            elif not isinstance(truncation, TruncationStrategy):
+                truncation_strategy = TruncationStrategy(truncation)
+            elif isinstance(truncation, TruncationStrategy):
+                truncation_strategy = truncation
+        else:
+            truncation_strategy = TruncationStrategy.DO_NOT_TRUNCATE
+
+        # Set max length if needed
+        if max_length is None:
+            if padding_strategy == PaddingStrategy.MAX_LENGTH:
+                max_length = self.model_max_length
+            if truncation_strategy != TruncationStrategy.DO_NOT_TRUNCATE:
+                max_length = self.model_max_length
+
+        # Test if we have a padding token
+        if padding_strategy != PaddingStrategy.DO_NOT_PAD and (not self.pad_token_id):
+            raise ValueError(
+                "Asking to pad but the tokenizer does not have a padding token. "
+                "Please select a token to use as `pad_token` `(tokenizer.pad_token = tokenizer.eos_token e.g.)` "
+                "or add a new pad token via `tokenizer.add_special_tokens({'pad_token': '[PAD]'})`."
+            )
+
+        return padding_strategy, truncation_strategy, max_length, kwargs
+
+    def _truncate(self,
+                  encoded_inputs: Union[Dict[str, Any],
+                                        Dict[str, List]],
+                  truncation_strategy: TruncationStrategy,
+                  truncation_side: str,
+                  max_length: Optional[int] = None):
+        if truncation_strategy != TruncationStrategy.DO_NOT_TRUNCATE:
+            py_assert(max_length is not None, ValueError, 'must pass max_length when truncation is activated!')
+            for k, v in encoded_inputs.items():
+                seq_ = [seq[:max_length] for seq in v] if truncation_side == 'right' \
+                    else [seq[-max_length:] for seq in v]
+                encoded_inputs[k] = seq_
+
+        return encoded_inputs
+
+    def pad(
+            self,
+            encoded_inputs: Union[
+                Dict[str, Any],
+                Dict[str, List],
+            ],
+            padding: Union[bool, str, PaddingStrategy] = True,
+            truncation: Union[bool, str, TruncationStrategy] = False,
+            max_length: Optional[int] = None,
+            return_attention_mask: Optional[bool] = None,
+            return_tensors: Optional[Union[str, TensorType]] = None,
+            verbose: bool = False,
+    ) -> BatchEncoding:
+        """
+        Pad a single encoded input or a batch of encoded inputs up to predefined length or to the max sequence length
+        in the batch.
+
+        Padding side (left/right) padding token ids are defined at the tokenizer level (with `self.padding_side`,
+        `self.pad_token_id` and `self.pad_token_type_id`).
+
+        Please note that with a fast tokenizer, using the `__call__` method is faster than using a method to encode the
+        text followed by a call to the `pad` method to get a padded encoding.
+
+        <Tip>
+
+        If the `encoded_inputs` passed are dictionary of numpy arrays, PyTorch tensors or TensorFlow tensors, the
+        result will use the same type unless you provide a different tensor type with `return_tensors`. In the case of
+        PyTorch tensors, you will lose the specific device of your tensors however.
+
+        </Tip>
+
+        Args:
+            encoded_inputs ([`BatchEncoding`], list of [`BatchEncoding`]:
+                Tokenized inputs. Can represent one input ([`BatchEncoding`] or `Dict[str, List[int]]`) or a batch of
+                tokenized inputs (list of [`BatchEncoding`], *Dict[str, List[List[int]]]* or *List[Dict[str,
+                List[int]]]*) so you can use this method during preprocessing as well as in a PyTorch Dataloader
+                collate function.
+
+                Instead of `List[int]` you can have tensors (numpy arrays, PyTorch tensors or TensorFlow tensors), see
+                the note above for the return type.
+            padding (`bool`, `str` or [`~utils.PaddingStrategy`], *optional*, defaults to `True`):
+                 Select a strategy to pad the returned sequences (according to the model's padding side and padding
+                 index) among:
+
+                - `True` or `'longest'`: Pad to the longest sequence in the batch (or no padding if only a single
+                  sequence if provided).
+                - `'max_length'`: Pad to a maximum length specified with the argument `max_length` or to the maximum
+                  acceptable input length for the model if that argument is not provided.
+                - `False` or `'do_not_pad'` (default): No padding (i.e., can output a batch with sequences of different
+                  lengths).
+            max_length (`int`, *optional*):
+                Maximum length of the returned list and optionally padding length (see above).
+            return_attention_mask (`bool`, *optional*):
+                Whether to return the attention mask. If left to the default, will return the attention mask according
+                to the specific tokenizer's default, defined by the `return_outputs` attribute.
+
+            return_tensors (`str` or [`~utils.TensorType`], *optional*):
+                If set, will return tensors instead of list of python integers. Acceptable values are:
+
+                - `'tf'`: Return TensorFlow `tf.constant` objects.
+                - `'pt'`: Return PyTorch `torch.Tensor` objects.
+                - `'np'`: Return Numpy `np.ndarray` objects.
+            verbose (`bool`, *optional*, defaults to `True`):
+                Whether or not to print more information and warnings.
+        """
+
+        # If we have a list of dicts, let's convert it in a dict of lists
+        # We do this to allow using this method as a collate_fn function in PyTorch Dataloader
+        if isinstance(encoded_inputs, (list, tuple)) and isinstance(encoded_inputs[0], Mapping):
+            encoded_inputs = {key: [example[key] for example in encoded_inputs] for key in encoded_inputs[0].keys()}
+
+        # The model's main input name, usually `time_seqs`, has be passed for padding
+        if self.model_input_names[0] not in encoded_inputs:
+            raise ValueError(
+                "You should supply an encoding or a list of encodings to this method "
+                f"that includes {self.model_input_names[0]}, but you provided {list(encoded_inputs.keys())}"
+            )
+
+        required_input = encoded_inputs[self.model_input_names[0]]
+
+        padding_strategy, truncation_strategy, max_length, _ = self._get_padding_truncation_strategies(
+            padding=padding, max_length=max_length, truncation=truncation, verbose=verbose
+        )
+
+        encoded_inputs = self._truncate(encoded_inputs,
+                                        truncation_strategy=truncation_strategy,
+                                        max_length=max_length,
+                                        truncation_side=self.truncation_side)
+
+        batch_size = len(required_input)
+        assert all(
+            len(v) == batch_size for v in encoded_inputs.values()
+        ), "Some items in the output dictionary have a different batch size than others."
+
+        if padding_strategy == PaddingStrategy.LONGEST:
+            max_length = max(len(inputs) for inputs in required_input)
+            padding_strategy = PaddingStrategy.MAX_LENGTH
+
+        batch_output = self._pad(
+            encoded_inputs,
+            max_length=max_length,
+            padding_strategy=padding_strategy,
+            return_attention_mask=return_attention_mask,
+        )
+
+        return BatchEncoding(batch_output, tensor_type=return_tensors)
+
+    def _pad(
+            self,
+            encoded_inputs: Union[Dict[str, Any], BatchEncoding],
+            max_length: Optional[int] = None,
+            padding_strategy: PaddingStrategy = PaddingStrategy.DO_NOT_PAD,
+            return_attention_mask: Optional[bool] = None,
+    ) -> dict:
+        """
+        Pad encoded inputs (on left/right and up to predefined length or max length in the batch)
+
+        Args:
+            encoded_inputs:
+                Dictionary of tokenized inputs (`List[int]`) or batch of tokenized inputs (`List[List[int]]`).
+            max_length: maximum length of the returned list and optionally padding length (see below).
+                Will truncate by taking into account the special tokens.
+            padding_strategy: PaddingStrategy to use for padding.
+
+                - PaddingStrategy.LONGEST Pad to the longest sequence in the batch
+                - PaddingStrategy.MAX_LENGTH: Pad to the max length (default)
+                - PaddingStrategy.DO_NOT_PAD: Do not pad
+                The tokenizer padding sides are defined in self.padding_side:
+
+                    - 'left': pads on the left of the sequences
+                    - 'right': pads on the right of the sequences
+            pad_to_multiple_of: (optional) Integer if set will pad the sequence to a multiple of the provided value.
+                This is especially useful to enable the use of Tensor Core on NVIDIA hardware with compute capability
+                `>= 7.5` (Volta).
+            return_attention_mask:
+                (optional) Set to False to avoid returning attention mask (default: set to model specifics)
+        """
+        # Load from model defaults
+        if return_attention_mask is None:
+            return_attention_mask = "attention_mask" in self.model_input_names
+
+        required_input = encoded_inputs[self.model_input_names[0]]
+
+        if padding_strategy == PaddingStrategy.LONGEST:
+            max_length = len(required_input)
+
+        # check whether we need to pad it
+        is_all_seq_equal_max_length = [len(seq) == max_length for seq in required_input]
+        is_all_seq_equal_max_length = np.prod(is_all_seq_equal_max_length)
+        needs_to_be_padded = padding_strategy != PaddingStrategy.DO_NOT_PAD and ~is_all_seq_equal_max_length
+
+        batch_output = dict()
+
+        if needs_to_be_padded:
+            # time seqs
+            batch_output[self.model_input_names[0]] = self.make_pad_sequence(encoded_inputs[self.model_input_names[0]],
+                                                                             self.pad_token_id,
+                                                                             padding_side=self.padding_side,
+                                                                             max_len=max_length)
+            # time_delta seqs
+            batch_output[self.model_input_names[1]] = self.make_pad_sequence(encoded_inputs[self.model_input_names[1]],
+                                                                             self.pad_token_id,
+                                                                             padding_side=self.padding_side,
+                                                                             max_len=max_length)
+            # type_seqs
+            batch_output[self.model_input_names[2]] = self.make_pad_sequence(encoded_inputs[self.model_input_names[2]],
+                                                                             self.pad_token_id,
+                                                                             padding_side=self.padding_side,
+                                                                             max_len=max_length,
+                                                                             dtype=np.int32)
+        else:
+            batch_output = encoded_inputs
+
+        # non_pad_mask
+        # we must use type seqs to check the mask, because the pad_token_id maybe one of valid values in
+        # time seqs
+        seq_pad_mask = batch_output[self.model_input_names[2]] == self.pad_token_id
+        batch_output[self.model_input_names[3]] = ~ seq_pad_mask
+
+        if return_attention_mask:
+            # attention_mask
+            batch_output[self.model_input_names[4]] = self.make_attn_mask_for_pad_sequence(
+                batch_output[self.model_input_names[2]],
+                self.pad_token_id)
+        else:
+            batch_output[self.model_input_names[4]] = []
+
+        # type_mask
+        batch_output[self.model_input_names[5]] = self.make_type_mask_for_pad_sequence(
+            batch_output[self.model_input_names[2]])
+
+        return batch_output
+
+    @staticmethod
+    def make_pad_sequence(seqs,
+                          pad_token_id,
+                          padding_side,
+                          max_len,
+                          dtype=np.float32,
+                          group_by_event_types=False):
+        """Pad the sequence batch-wise.
+
+        Args:
+            seqs (list): list of sequences with variational length
+            pad_token_id (int, float): optional, a value that used to pad the sequences. If None, then the pad index
+            is set to be the event_num_with_pad
+            max_len (int): optional, the maximum length of the sequence after padding. If None, then the
+            length is set to be the max length of all input sequences.
+            pad_at_end (bool): optional, whether to pad the sequnce at the end. If False,
+            the sequence is pad at the beginning
+
+        Returns:
+            a numpy array of padded sequence
+
+
+        Example:
+        ```python
+        seqs = [[0, 1], [3, 4, 5]]
+        pad_sequence(seqs, 100)
+        >>> [[0, 1, 100], [3, 4, 5]]
+
+        pad_sequence(seqs, 100, max_len=5)
+        >>> [[0, 1, 100, 100, 100], [3, 4, 5, 100, 100]]
+        ```
+
+        """
+        if not group_by_event_types:
+            if padding_side == "right":
+                pad_seq = np.array([seq + [pad_token_id] * (max_len - len(seq)) for seq in seqs], dtype=dtype)
+            else:
+                pad_seq = np.array([[pad_token_id] * (max_len - len(seq)) + seq for seq in seqs], dtype=dtype)
+        else:
+            pad_seq = []
+            for seq in seqs:
+                if padding_side == "right":
+                    pad_seq.append(np.array([s + [pad_token_id] * (max_len - len(s)) for s in seq], dtype=dtype))
+                else:
+                    pad_seq.append(np.array([[pad_token_id] * (max_len - len(s)) + s for s in seqs], dtype=dtype))
+
+            pad_seq = np.array(pad_seq)
+        return pad_seq
+
+    def make_attn_mask_for_pad_sequence(self, pad_seqs, pad_token_id):
+        """Make the attention masks for the sequence.
+
+        Args:
+            pad_seqs (tensor): list of sequences that have been padded with fixed length
+            pad_token_id (int): optional, a value that used to pad the sequences. If None, then the pad index
+            is set to be the event_num_with_pad
+
+        Returns:
+            np.array: a bool matrix of the same size of input, denoting the masks of the
+            sequence (True: non mask, False: mask)
+
+
+        Example:
+        ```python
+        seqs = [[ 1,  6,  0,  7, 12, 12],
+        [ 1,  0,  5,  1, 10,  9]]
+        make_attn_mask_for_pad_sequence(seqs, pad_index=12)
+        >>>
+            batch_non_pad_mask
+            ([[ True,  True,  True,  True, False, False],
+            [ True,  True,  True,  True,  True,  True]])
+            attention_mask
+            [[[ True  True  True  True  True  True]
+              [False  True  True  True  True  True]
+              [False False  True  True  True  True]
+              [False False False  True  True  True]
+              [False False False False  True  True]
+              [False False False False  True  True]]
+
+             [[ True  True  True  True  True  True]
+              [False  True  True  True  True  True]
+              [False False  True  True  True  True]
+              [False False False  True  True  True]
+              [False False False False  True  True]
+              [False False False False False  True]]]
+        ```
+
+
+        """
+
+        seq_num, seq_len = pad_seqs.shape
+
+        # [batch_size, seq_len]
+        seq_pad_mask = pad_seqs == pad_token_id
+
+        # [batch_size, seq_len, seq_len]
+        attention_key_pad_mask = np.tile(seq_pad_mask[:, None, :], (1, seq_len, 1))
+        subsequent_mask = np.tile(np.triu(np.ones((seq_len, seq_len), dtype=bool), k=0)[None, :, :], (seq_num, 1, 1))
+
+        attention_mask = subsequent_mask | attention_key_pad_mask
+
+        return attention_mask
+
+    def make_type_mask_for_pad_sequence(self, pad_seqs):
+        """Make the type mask.
+
+        Args:
+            pad_seqs (tensor): a list of sequence events with equal length (i.e., padded sequence)
+
+        Returns:
+            np.array: a 3-dim matrix, where the last dim (one-hot vector) indicates the type of event
+
+        """
+        type_mask = np.zeros([*pad_seqs.shape, self.num_event_types])
+        for i in range(self.num_event_types):
+            type_mask[:, :, i] = pad_seqs == i
+
+        return type_mask
```

### Comparing `easy_tpp-0.0.4/easy_tpp/runner/base_runner.py` & `easy_tpp-0.0.5/easy_tpp/runner/base_runner.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-import logging
-from abc import abstractmethod
-
-from easy_tpp.preprocess import TPPDataLoader
-from easy_tpp.utils import Registrable, Timer, logger, get_unique_id, LogConst, get_stage, RunnerPhase
-
-
-class Runner(Registrable):
-    """Registrable Base Runner class.
-    """
-
-    def __init__(
-            self,
-            runner_config,
-            unique_model_dir=False,
-            **kwargs):
-        """Initialize the base runner.
-
-        Args:
-            runner_config (RunnerConfig): config for the runner.
-            unique_model_dir (bool, optional): whether to give unique dir to save the model. Defaults to False.
-        """
-        self.runner_config = runner_config
-        # re-assign the model_dir
-        if unique_model_dir:
-            runner_config.model_dir = runner_config.base_config.specs['saved_model_dir'] + '_' + get_unique_id()
-
-        self.save_log()
-
-        skip_data_loader = kwargs.get('skip_data_loader', False)
-        if not skip_data_loader:
-            # build data reader
-            data_config = self.runner_config.data_config
-            backend = self.runner_config.base_config.backend
-            kwargs = self.runner_config.trainer_config.get_yaml_config()
-            self._data_loader = TPPDataLoader(
-                data_config=data_config,
-                backend=backend,
-                **kwargs
-            )
-        self.timer = Timer()
-
-    @staticmethod
-    def build_from_config(runner_config, unique_model_dir=False, **kwargs):
-        """Build up the runner from runner config.
-
-        Args:
-            runner_config (RunnerConfig): config for the runner.
-            unique_model_dir (bool, optional): whether to give unique dir to save the model. Defaults to False.
-
-        Returns:
-            Runner: the corresponding runner class.
-        """
-        runner_cls = Runner.by_name(runner_config.base_config.runner_id)
-        return runner_cls(runner_config, unique_model_dir=unique_model_dir, **kwargs)
-
-    def get_config(self):
-        return self.runner_config
-
-    def set_model_dir(self, model_dir):
-        self.runner_config.base_config.specs['saved_model_dir'] = model_dir
-
-    def get_model_dir(self):
-        return self.runner_config.base_config.specs['saved_model_dir']
-
-    def train(
-            self,
-            train_loader=None,
-            valid_loader=None,
-            test_loader=None,
-            **kwargs
-    ):
-        """Train the model.
-
-        Args:
-            train_loader (EasyTPP.DataLoader, optional): data loader for train set. Defaults to None.
-            valid_loader (EasyTPP.DataLoader, optional): data loader for valid set. Defaults to None.
-            test_loader (EasyTPP.DataLoader, optional): data loader for test set. Defaults to None.
-
-        Returns:
-            model: _description_
-        """
-        # no train and valid loader from outside
-        if train_loader is None and valid_loader is None:
-            train_loader = self._data_loader.train_loader()
-            valid_loader = self._data_loader.valid_loader()
-
-        # no test loader from outside and there indeed exits test data in config
-        if test_loader is None and self.runner_config.data_config.test_dir is not None:
-            test_loader = self._data_loader.test_loader()
-
-        logger.info(f'Data \'{self.runner_config.base_config.dataset_id}\' loaded...')
-
-        timer = self.timer
-        timer.start()
-        model_id = self.runner_config.base_config.model_id
-        logger.info(f'Start {model_id} training...')
-        model = self._train_model(
-            train_loader,
-            valid_loader,
-            test_loader=test_loader,
-            **kwargs
-        )
-        logger.info(f'End {model_id} train! Cost time: {timer.end()}')
-        return model
-
-    def evaluate(self, valid_loader=None, **kwargs):
-        if valid_loader is None:
-            valid_loader = self._data_loader.valid_loader()
-
-        logger.info(f'Data \'{self.runner_config.base_config.dataset_id}\' loaded...')
-
-        timer = self.timer
-        timer.start()
-        model_id = self.runner_config.base_config.model_id
-        logger.info(f'Start {model_id} evaluation...')
-
-        metric = self._evaluate_model(
-            valid_loader,
-            **kwargs
-        )
-        logger.info(f'End {model_id} evaluation! Cost time: {timer.end()}')
-        return metric['rmse']  # return a list of scalr for HPO to use
-
-    def gen(self, gen_loader=None, **kwargs):
-        if gen_loader is None:
-            gen_loader = self._data_loader.test_loader()
-
-        logger.info(f'Data \'{self.runner_config.dataset_id}\' loaded...')
-
-        timer = self.timer
-        timer.start()
-        model_name = self.runner_config.model_id
-        logger.info(f'Start {model_name} evaluation...')
-
-        model = self._gen_model(
-            gen_loader,
-            **kwargs
-        )
-        logger.info(f'End {model_name} generation! Cost time: {timer.end()}')
-        return model
-
-    @abstractmethod
-    def _train_model(self, train_loader, valid_loader, **kwargs):
-        pass
-
-    @abstractmethod
-    def _evaluate_model(self, data_loader, **kwargs):
-        pass
-
-    @abstractmethod
-    def _gen_model(self, data_loader, **kwargs):
-        pass
-
-    @abstractmethod
-    def _save_model(self, model_dir, **kwargs):
-        pass
-
-    @abstractmethod
-    def _load_model(self, model_dir, **kwargs):
-        pass
-
-    def save_log(self):
-        """Save log to local files
-        """
-        log_dir = self.runner_config.base_config.specs['saved_log_dir']
-        fh = logging.FileHandler(log_dir)
-        fh.setFormatter(logging.Formatter(LogConst.DEFAULT_FORMAT_LONG))
-        logger.addHandler(fh)
-        logger.info(f'Save the log to {log_dir}')
-        return
-
-    def save(
-            self,
-            model_dir=None,
-            **kwargs
-    ):
-        return self._save_model(model_dir, **kwargs)
-
-    def run(self, **kwargs):
-        """Start the runner.
-
-        Args:
-            **kwargs (dict): optional params.
-
-        Returns:
-            EasyTPP.BaseModel, dict: the results of the process.
-        """
-        current_stage = get_stage(self.runner_config.base_config.stage)
-        if current_stage == RunnerPhase.TRAIN:
-            return self.train(**kwargs)
-        elif current_stage == RunnerPhase.VALIDATE:
-            return self.evaluate(**kwargs)
-        else:
-            return self.gen(**kwargs)
+import logging
+from abc import abstractmethod
+
+from easy_tpp.preprocess import TPPDataLoader
+from easy_tpp.utils import Registrable, Timer, logger, get_unique_id, LogConst, get_stage, RunnerPhase
+
+
+class Runner(Registrable):
+    """Registrable Base Runner class.
+    """
+
+    def __init__(
+            self,
+            runner_config,
+            unique_model_dir=False,
+            **kwargs):
+        """Initialize the base runner.
+
+        Args:
+            runner_config (RunnerConfig): config for the runner.
+            unique_model_dir (bool, optional): whether to give unique dir to save the model. Defaults to False.
+        """
+        self.runner_config = runner_config
+        # re-assign the model_dir
+        if unique_model_dir:
+            runner_config.model_dir = runner_config.base_config.specs['saved_model_dir'] + '_' + get_unique_id()
+
+        self.save_log()
+
+        skip_data_loader = kwargs.get('skip_data_loader', False)
+        if not skip_data_loader:
+            # build data reader
+            data_config = self.runner_config.data_config
+            backend = self.runner_config.base_config.backend
+            kwargs = self.runner_config.trainer_config.get_yaml_config()
+            self._data_loader = TPPDataLoader(
+                data_config=data_config,
+                backend=backend,
+                **kwargs
+            )
+        self.timer = Timer()
+
+    @staticmethod
+    def build_from_config(runner_config, unique_model_dir=False, **kwargs):
+        """Build up the runner from runner config.
+
+        Args:
+            runner_config (RunnerConfig): config for the runner.
+            unique_model_dir (bool, optional): whether to give unique dir to save the model. Defaults to False.
+
+        Returns:
+            Runner: the corresponding runner class.
+        """
+        runner_cls = Runner.by_name(runner_config.base_config.runner_id)
+        return runner_cls(runner_config, unique_model_dir=unique_model_dir, **kwargs)
+
+    def get_config(self):
+        return self.runner_config
+
+    def set_model_dir(self, model_dir):
+        self.runner_config.base_config.specs['saved_model_dir'] = model_dir
+
+    def get_model_dir(self):
+        return self.runner_config.base_config.specs['saved_model_dir']
+
+    def train(
+            self,
+            train_loader=None,
+            valid_loader=None,
+            test_loader=None,
+            **kwargs
+    ):
+        """Train the model.
+
+        Args:
+            train_loader (EasyTPP.DataLoader, optional): data loader for train set. Defaults to None.
+            valid_loader (EasyTPP.DataLoader, optional): data loader for valid set. Defaults to None.
+            test_loader (EasyTPP.DataLoader, optional): data loader for test set. Defaults to None.
+
+        Returns:
+            model: _description_
+        """
+        # no train and valid loader from outside
+        if train_loader is None and valid_loader is None:
+            train_loader = self._data_loader.train_loader()
+            valid_loader = self._data_loader.valid_loader()
+
+        # no test loader from outside and there indeed exits test data in config
+        if test_loader is None and self.runner_config.data_config.test_dir is not None:
+            test_loader = self._data_loader.test_loader()
+
+        logger.info(f'Data \'{self.runner_config.base_config.dataset_id}\' loaded...')
+
+        timer = self.timer
+        timer.start()
+        model_id = self.runner_config.base_config.model_id
+        logger.info(f'Start {model_id} training...')
+        model = self._train_model(
+            train_loader,
+            valid_loader,
+            test_loader=test_loader,
+            **kwargs
+        )
+        logger.info(f'End {model_id} train! Cost time: {timer.end()}')
+        return model
+
+    def evaluate(self, valid_loader=None, **kwargs):
+        if valid_loader is None:
+            valid_loader = self._data_loader.valid_loader()
+
+        logger.info(f'Data \'{self.runner_config.base_config.dataset_id}\' loaded...')
+
+        timer = self.timer
+        timer.start()
+        model_id = self.runner_config.base_config.model_id
+        logger.info(f'Start {model_id} evaluation...')
+
+        metric = self._evaluate_model(
+            valid_loader,
+            **kwargs
+        )
+        logger.info(f'End {model_id} evaluation! Cost time: {timer.end()}')
+        return metric['rmse']  # return a list of scalr for HPO to use
+
+    def gen(self, gen_loader=None, **kwargs):
+        if gen_loader is None:
+            gen_loader = self._data_loader.test_loader()
+
+        logger.info(f'Data \'{self.runner_config.dataset_id}\' loaded...')
+
+        timer = self.timer
+        timer.start()
+        model_name = self.runner_config.model_id
+        logger.info(f'Start {model_name} evaluation...')
+
+        model = self._gen_model(
+            gen_loader,
+            **kwargs
+        )
+        logger.info(f'End {model_name} generation! Cost time: {timer.end()}')
+        return model
+
+    @abstractmethod
+    def _train_model(self, train_loader, valid_loader, **kwargs):
+        pass
+
+    @abstractmethod
+    def _evaluate_model(self, data_loader, **kwargs):
+        pass
+
+    @abstractmethod
+    def _gen_model(self, data_loader, **kwargs):
+        pass
+
+    @abstractmethod
+    def _save_model(self, model_dir, **kwargs):
+        pass
+
+    @abstractmethod
+    def _load_model(self, model_dir, **kwargs):
+        pass
+
+    def save_log(self):
+        """Save log to local files
+        """
+        log_dir = self.runner_config.base_config.specs['saved_log_dir']
+        fh = logging.FileHandler(log_dir)
+        fh.setFormatter(logging.Formatter(LogConst.DEFAULT_FORMAT_LONG))
+        logger.addHandler(fh)
+        logger.info(f'Save the log to {log_dir}')
+        return
+
+    def save(
+            self,
+            model_dir=None,
+            **kwargs
+    ):
+        return self._save_model(model_dir, **kwargs)
+
+    def run(self, **kwargs):
+        """Start the runner.
+
+        Args:
+            **kwargs (dict): optional params.
+
+        Returns:
+            EasyTPP.BaseModel, dict: the results of the process.
+        """
+        current_stage = get_stage(self.runner_config.base_config.stage)
+        if current_stage == RunnerPhase.TRAIN:
+            return self.train(**kwargs)
+        elif current_stage == RunnerPhase.VALIDATE:
+            return self.evaluate(**kwargs)
+        else:
+            return self.gen(**kwargs)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/runner/tpp_runner.py` & `easy_tpp-0.0.5/easy_tpp/runner/tpp_runner.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-from collections import OrderedDict
-
-from easy_tpp.runner.base_runner import Runner
-from easy_tpp.utils import RunnerPhase, logger, MetricsHelper, MetricsTracker, concat_element, save_pickle
-from easy_tpp.utils.const import Backend
-
-
-@Runner.register(name='std_tpp')
-class TPPRunner(Runner):
-    """Standard TPP runner
-    """
-
-    def __init__(self, runner_config, unique_model_dir=False, **kwargs):
-        super(TPPRunner, self).__init__(runner_config, unique_model_dir, **kwargs)
-
-        self.metrics_tracker = MetricsTracker()
-        if self.runner_config.trainer_config.metrics is not None:
-            self.metric_functions = self.runner_config.get_metric_functions()
-
-        self._init_model()
-
-        pretrain_dir = self.runner_config.model_config.pretrained_model_dir
-        if pretrain_dir is not None:
-            self._load_model(pretrain_dir)
-
-    def _init_model(self):
-        """Initialize the model.
-        """
-        self.use_torch = self.runner_config.base_config.backend == Backend.Torch
-
-        if self.use_torch:
-            from easy_tpp.utils import set_seed
-            from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
-            from easy_tpp.torch_wrapper import TorchModelWrapper
-            from easy_tpp.utils import count_model_params
-            set_seed(self.runner_config.trainer_config.seed)
-
-            self.model = TorchBaseModel.generate_model_from_config(model_config=self.runner_config.model_config)
-            self.model_wrapper = TorchModelWrapper(self.model,
-                                                   self.runner_config.base_config,
-                                                   self.runner_config.model_config,
-                                                   self.runner_config.trainer_config)
-            num_params = count_model_params(self.model)
-
-        else:
-            from easy_tpp.utils.tf_utils import set_seed
-            from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
-            from easy_tpp.tf_wrapper import TfModelWrapper
-            from easy_tpp.utils.tf_utils import count_model_params
-            set_seed(self.runner_config.trainer_config.seed)
-
-            self.model = TfBaseModel.generate_model_from_config(model_config=self.runner_config.model_config)
-            self.model_wrapper = TfModelWrapper(self.model,
-                                                self.runner_config.base_config,
-                                                self.runner_config.model_config,
-                                                self.runner_config.trainer_config)
-            num_params = count_model_params()
-
-        info_msg = f'Num of model parameters {num_params}'
-        logger.info(info_msg)
-
-    def _save_model(self, model_dir, **kwargs):
-        """Save the model.
-
-        Args:
-            model_dir (str): the dir for model to save.
-        """
-        if model_dir is None:
-            model_dir = self.runner_config.base_config.specs['saved_model_dir']
-        self.model_wrapper.save(model_dir)
-        logger.critical(f'Save model to {model_dir}')
-        return
-
-    def _load_model(self, model_dir, **kwargs):
-        """Load the model from the dir.
-
-        Args:
-            model_dir (str): the dir for model to load.
-        """
-        self.model_wrapper.restore(model_dir)
-        logger.critical(f'Load model from {model_dir}')
-        return
-
-    def _train_model(self, train_loader, valid_loader, **kwargs):
-        """Train the model.
-
-        Args:
-            train_loader (EasyTPP.DataLoader): data loader for the train set.
-            valid_loader (EasyTPP.DataLoader): data loader for the valid set.
-        """
-        test_loader = kwargs.get('test_loader')
-        for i in range(self.runner_config.trainer_config.max_epoch):
-            train_metrics = self.run_one_epoch(train_loader, RunnerPhase.TRAIN)
-
-            message = f"[ Epoch {i} (train) ]: train " + MetricsHelper.metrics_dict_to_str(train_metrics)
-            logger.info(message)
-
-            self.model_wrapper.write_summary(i, train_metrics, RunnerPhase.TRAIN)
-
-            # evaluate model
-            if i % self.runner_config.trainer_config.valid_freq == 0:
-                valid_metrics = self.run_one_epoch(valid_loader, RunnerPhase.VALIDATE)
-
-                self.model_wrapper.write_summary(i, valid_metrics, RunnerPhase.VALIDATE)
-
-                message = f"[ Epoch {i} (valid) ]:  valid " + MetricsHelper.metrics_dict_to_str(valid_metrics)
-                logger.info(message)
-
-                updated = self.metrics_tracker.update_best("loglike", valid_metrics['loglike'], i)
-
-                message_valid = "current best loglike on valid set is {:.4f} (updated at epoch-{})".format(
-                    self.metrics_tracker.current_best['loglike'], self.metrics_tracker.episode_best)
-
-                if updated:
-                    message_valid += f", best updated at this epoch"
-                    self.model_wrapper.save(self.runner_config.base_config.specs['saved_model_dir'])
-
-                if test_loader is not None:
-                    test_metrics = self.run_one_epoch(test_loader, RunnerPhase.VALIDATE)
-
-                    message = f"[ Epoch {i} (test) ]: test " + MetricsHelper.metrics_dict_to_str(test_metrics)
-                    logger.info(message)
-
-                logger.critical(message_valid)
-
-        self.model_wrapper.close_summary()
-
-        return
-
-    def _evaluate_model(self, data_loader, **kwargs):
-        """Evaluate the model on the valid dataset.
-
-        Args:
-            data_loader (EasyTPP.DataLoader): data loader for the valid set
-
-        Returns:
-            dict: metrics dict.
-        """
-
-        eval_metrics = self.run_one_epoch(data_loader, RunnerPhase.VALIDATE)
-
-        self.model_wrapper.write_summary(0, eval_metrics, RunnerPhase.VALIDATE)
-
-        self.model_wrapper.close_summary()
-
-        message = f"Evaluation result: " + MetricsHelper.metrics_dict_to_str(eval_metrics)
-
-        logger.critical(message)
-
-        return eval_metrics
-
-    def _gen_model(self, data_loader, **kwargs):
-        """Generation of the TPP, one-step and multi-step are both supported.
-        """
-
-        test_result = self.run_one_epoch(data_loader, RunnerPhase.PREDICT)
-
-        # For the moment we save it to a pkl
-
-        message = f'Save the prediction to pickle file pred.pkl'
-
-        logger.critical(message)
-
-        save_pickle('pred.pkl', test_result)
-
-        return
-
-    def run_one_epoch(self, data_loader, phase):
-        """Run one complete epoch.
-
-        Args:
-            data_loader: data loader object defined in model runner
-            phase: enum, [train, dev, test]
-
-        Returns:
-            a dict of metrics
-        """
-        total_loss = 0
-        total_num_event = 0
-        epoch_label = []
-        epoch_pred = []
-        epoch_mask = []
-        pad_index = self.runner_config.data_config.data_specs.pad_token_id
-        metrics_dict = OrderedDict()
-        if phase in [RunnerPhase.TRAIN, RunnerPhase.VALIDATE]:
-            for batch in data_loader:
-                batch_loss, batch_num_event, batch_pred, batch_label, batch_mask = \
-                    self.model_wrapper.run_batch(batch, phase=phase)
-
-                total_loss += batch_loss
-                total_num_event += batch_num_event
-                epoch_pred.append(batch_pred)
-                epoch_label.append(batch_label)
-                epoch_mask.append(batch_mask)
-
-            avg_loss = total_loss / total_num_event
-
-            metrics_dict.update({'loglike': -avg_loss, 'num_events': total_num_event})
-
-        else:
-            for batch in data_loader:
-                batch_pred, batch_label = self.model_wrapper.run_batch(batch, phase=phase)
-                epoch_pred.append(batch_pred)
-                epoch_label.append(batch_label)
-
-        # we need to improve the code here
-        # classify batch_output to list
-        pred_exists, label_exists = False, False
-        if epoch_pred[0][0] is not None:
-            epoch_pred = concat_element(epoch_pred, pad_index)
-            pred_exists = True
-        if len(epoch_label) > 0 and epoch_label[0][0] is not None:
-            epoch_label = concat_element(epoch_label, pad_index)
-            label_exists = True
-            if len(epoch_mask):
-                epoch_mask = concat_element(epoch_mask, False)[0]  # retrieve the first element of concat array
-                epoch_mask = epoch_mask.astype(bool)
-
-        if pred_exists and label_exists:
-            metrics_dict.update(self.metric_functions(epoch_pred, epoch_label, seq_mask=epoch_mask))
-
-        if phase == RunnerPhase.PREDICT:
-            metrics_dict.update({'pred': epoch_pred, 'label': epoch_label})
-
-        return metrics_dict
+from collections import OrderedDict
+
+from easy_tpp.runner.base_runner import Runner
+from easy_tpp.utils import RunnerPhase, logger, MetricsHelper, MetricsTracker, concat_element, save_pickle
+from easy_tpp.utils.const import Backend
+
+
+@Runner.register(name='std_tpp')
+class TPPRunner(Runner):
+    """Standard TPP runner
+    """
+
+    def __init__(self, runner_config, unique_model_dir=False, **kwargs):
+        super(TPPRunner, self).__init__(runner_config, unique_model_dir, **kwargs)
+
+        self.metrics_tracker = MetricsTracker()
+        if self.runner_config.trainer_config.metrics is not None:
+            self.metric_functions = self.runner_config.get_metric_functions()
+
+        self._init_model()
+
+        pretrain_dir = self.runner_config.model_config.pretrained_model_dir
+        if pretrain_dir is not None:
+            self._load_model(pretrain_dir)
+
+    def _init_model(self):
+        """Initialize the model.
+        """
+        self.use_torch = self.runner_config.base_config.backend == Backend.Torch
+
+        if self.use_torch:
+            from easy_tpp.utils import set_seed
+            from easy_tpp.model.torch_model.torch_basemodel import TorchBaseModel
+            from easy_tpp.torch_wrapper import TorchModelWrapper
+            from easy_tpp.utils import count_model_params
+            set_seed(self.runner_config.trainer_config.seed)
+
+            self.model = TorchBaseModel.generate_model_from_config(model_config=self.runner_config.model_config)
+            self.model_wrapper = TorchModelWrapper(self.model,
+                                                   self.runner_config.base_config,
+                                                   self.runner_config.model_config,
+                                                   self.runner_config.trainer_config)
+            num_params = count_model_params(self.model)
+
+        else:
+            from easy_tpp.utils.tf_utils import set_seed
+            from easy_tpp.model.tf_model.tf_basemodel import TfBaseModel
+            from easy_tpp.tf_wrapper import TfModelWrapper
+            from easy_tpp.utils.tf_utils import count_model_params
+            set_seed(self.runner_config.trainer_config.seed)
+
+            self.model = TfBaseModel.generate_model_from_config(model_config=self.runner_config.model_config)
+            self.model_wrapper = TfModelWrapper(self.model,
+                                                self.runner_config.base_config,
+                                                self.runner_config.model_config,
+                                                self.runner_config.trainer_config)
+            num_params = count_model_params()
+
+        info_msg = f'Num of model parameters {num_params}'
+        logger.info(info_msg)
+
+    def _save_model(self, model_dir, **kwargs):
+        """Save the model.
+
+        Args:
+            model_dir (str): the dir for model to save.
+        """
+        if model_dir is None:
+            model_dir = self.runner_config.base_config.specs['saved_model_dir']
+        self.model_wrapper.save(model_dir)
+        logger.critical(f'Save model to {model_dir}')
+        return
+
+    def _load_model(self, model_dir, **kwargs):
+        """Load the model from the dir.
+
+        Args:
+            model_dir (str): the dir for model to load.
+        """
+        self.model_wrapper.restore(model_dir)
+        logger.critical(f'Load model from {model_dir}')
+        return
+
+    def _train_model(self, train_loader, valid_loader, **kwargs):
+        """Train the model.
+
+        Args:
+            train_loader (EasyTPP.DataLoader): data loader for the train set.
+            valid_loader (EasyTPP.DataLoader): data loader for the valid set.
+        """
+        test_loader = kwargs.get('test_loader')
+        for i in range(self.runner_config.trainer_config.max_epoch):
+            train_metrics = self.run_one_epoch(train_loader, RunnerPhase.TRAIN)
+
+            message = f"[ Epoch {i} (train) ]: train " + MetricsHelper.metrics_dict_to_str(train_metrics)
+            logger.info(message)
+
+            self.model_wrapper.write_summary(i, train_metrics, RunnerPhase.TRAIN)
+
+            # evaluate model
+            if i % self.runner_config.trainer_config.valid_freq == 0:
+                valid_metrics = self.run_one_epoch(valid_loader, RunnerPhase.VALIDATE)
+
+                self.model_wrapper.write_summary(i, valid_metrics, RunnerPhase.VALIDATE)
+
+                message = f"[ Epoch {i} (valid) ]:  valid " + MetricsHelper.metrics_dict_to_str(valid_metrics)
+                logger.info(message)
+
+                updated = self.metrics_tracker.update_best("loglike", valid_metrics['loglike'], i)
+
+                message_valid = "current best loglike on valid set is {:.4f} (updated at epoch-{})".format(
+                    self.metrics_tracker.current_best['loglike'], self.metrics_tracker.episode_best)
+
+                if updated:
+                    message_valid += f", best updated at this epoch"
+                    self.model_wrapper.save(self.runner_config.base_config.specs['saved_model_dir'])
+
+                if test_loader is not None:
+                    test_metrics = self.run_one_epoch(test_loader, RunnerPhase.VALIDATE)
+
+                    message = f"[ Epoch {i} (test) ]: test " + MetricsHelper.metrics_dict_to_str(test_metrics)
+                    logger.info(message)
+
+                logger.critical(message_valid)
+
+        self.model_wrapper.close_summary()
+
+        return
+
+    def _evaluate_model(self, data_loader, **kwargs):
+        """Evaluate the model on the valid dataset.
+
+        Args:
+            data_loader (EasyTPP.DataLoader): data loader for the valid set
+
+        Returns:
+            dict: metrics dict.
+        """
+
+        eval_metrics = self.run_one_epoch(data_loader, RunnerPhase.VALIDATE)
+
+        self.model_wrapper.write_summary(0, eval_metrics, RunnerPhase.VALIDATE)
+
+        self.model_wrapper.close_summary()
+
+        message = f"Evaluation result: " + MetricsHelper.metrics_dict_to_str(eval_metrics)
+
+        logger.critical(message)
+
+        return eval_metrics
+
+    def _gen_model(self, data_loader, **kwargs):
+        """Generation of the TPP, one-step and multi-step are both supported.
+        """
+
+        test_result = self.run_one_epoch(data_loader, RunnerPhase.PREDICT)
+
+        # For the moment we save it to a pkl
+
+        message = f'Save the prediction to pickle file pred.pkl'
+
+        logger.critical(message)
+
+        save_pickle('pred.pkl', test_result)
+
+        return
+
+    def run_one_epoch(self, data_loader, phase):
+        """Run one complete epoch.
+
+        Args:
+            data_loader: data loader object defined in model runner
+            phase: enum, [train, dev, test]
+
+        Returns:
+            a dict of metrics
+        """
+        total_loss = 0
+        total_num_event = 0
+        epoch_label = []
+        epoch_pred = []
+        epoch_mask = []
+        pad_index = self.runner_config.data_config.data_specs.pad_token_id
+        metrics_dict = OrderedDict()
+        if phase in [RunnerPhase.TRAIN, RunnerPhase.VALIDATE]:
+            for batch in data_loader:
+                batch_loss, batch_num_event, batch_pred, batch_label, batch_mask = \
+                    self.model_wrapper.run_batch(batch, phase=phase)
+
+                total_loss += batch_loss
+                total_num_event += batch_num_event
+                epoch_pred.append(batch_pred)
+                epoch_label.append(batch_label)
+                epoch_mask.append(batch_mask)
+
+            avg_loss = total_loss / total_num_event
+
+            metrics_dict.update({'loglike': -avg_loss, 'num_events': total_num_event})
+
+        else:
+            for batch in data_loader:
+                batch_pred, batch_label = self.model_wrapper.run_batch(batch, phase=phase)
+                epoch_pred.append(batch_pred)
+                epoch_label.append(batch_label)
+
+        # we need to improve the code here
+        # classify batch_output to list
+        pred_exists, label_exists = False, False
+        if epoch_pred[0][0] is not None:
+            epoch_pred = concat_element(epoch_pred, pad_index)
+            pred_exists = True
+        if len(epoch_label) > 0 and epoch_label[0][0] is not None:
+            epoch_label = concat_element(epoch_label, pad_index)
+            label_exists = True
+            if len(epoch_mask):
+                epoch_mask = concat_element(epoch_mask, False)[0]  # retrieve the first element of concat array
+                epoch_mask = epoch_mask.astype(bool)
+
+        if pred_exists and label_exists:
+            metrics_dict.update(self.metric_functions(epoch_pred, epoch_label, seq_mask=epoch_mask))
+
+        if phase == RunnerPhase.PREDICT:
+            metrics_dict.update({'pred': epoch_pred, 'label': epoch_label})
+
+        return metrics_dict
```

### Comparing `easy_tpp-0.0.4/easy_tpp/tf_wrapper.py` & `easy_tpp-0.0.5/easy_tpp/tf_wrapper.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-""" Initialize a Tf model wrapper that feed into Model Runner   """
-
-import tensorflow as tf
-
-from easy_tpp.utils import RunnerPhase
-from easy_tpp.utils.tf_utils import set_device, set_optimizer
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-class TfModelWrapper:
-    def __init__(self, model, base_config, model_config, trainer_config):
-        """A wrapper class for Tensorflow backends.
-
-        Args:
-            model (BaseModel): a TPP model.
-            base_config (EasyTPP.Config): basic configs.
-            model_config (EasyTPP.Config): model spec configs.
-            trainer_config (EasyTPP.Config): trainer spec configs.
-        """
-        self.model = model
-        self.base_config = base_config
-        self.model_config = model_config
-        self.trainer_config = trainer_config
-        set_device(self.trainer_config.gpu)
-
-        # init session and build model
-        tf.reset_default_graph()
-        self.sess = tf.Session()
-        self.model.build_graph()
-        if self.model_config.is_training:
-            # set up optimizer
-            optimizer = self.trainer_config.optimizer
-            self.learning_rate = self.trainer_config.learning_rate
-            self.opt = set_optimizer(optimizer, self.learning_rate)
-            self.train_op = self.opt.minimize(self.model.loss)
-
-        # set up tensorboard
-        self.use_tfb = self.trainer_config.use_tfb
-        self.train_summary_writer, self.valid_summary_writer = None, None
-        if self.use_tfb:
-            self.train_summary_writer = tf.summary.FileWriter(self.base_config.spec['tfb_train_dir'])
-            self.valid_summary_writer = tf.summary.FileWriter(self.base_config.spec['tfb_valid_dir'])
-
-        # init variable and saver
-        self.sess.run(tf.global_variables_initializer())
-        self.saver = tf.train.Saver()
-
-    def restore(self, ckpt_dir):
-        """Load the checkpoint to restore the model.
-
-        Args:
-            ckpt_dir (str): path for the checkpoint.
-        """
-        self.saver.restore(self.sess, ckpt_dir)
-
-    def save(self, ckpt_dir):
-        """Save the checkpoint for the model.
-
-        Args:
-            ckpt_dir (str): path for the checkpoint.
-        """
-        self.saver.save(self.sess, ckpt_dir)
-
-    def write_summary(self, epoch, kv_pairs, phase):
-        """Write the kv_paris into the tensorboard.
-
-        Args:
-            epoch (int): epoch index in the training.
-            kv_pairs (dict): metrics dict.
-            phase (RunnerPhase): a const that defines the stage of model runner.
-        """
-        if self.use_tfb:
-            summary_writer = None
-            if phase == RunnerPhase.TRAIN:
-                summary_writer = self.train_summary_writer
-            elif phase == RunnerPhase.VALIDATE:
-                summary_writer = self.valid_summary_writer
-            elif phase == RunnerPhase.PREDICT:
-                pass
-
-            metric_summary = tf.Summary()
-            if summary_writer is not None:
-                for k, v in kv_pairs.items():
-                    if k != 'num_events':
-                        metric_summary.value.add(tag=k, simple_value=v)
-                        summary_writer.add_summary(metric_summary, epoch)
-
-                summary_writer.flush()
-        return
-
-    def close_summary(self):
-        """Close the tensorboard summary writer.
-        """
-        if self.train_summary_writer is not None:
-            self.train_summary_writer.close()
-
-        if self.valid_summary_writer is not None:
-            self.valid_summary_writer.close()
-        return
-
-    def run_batch(self, batch, phase):
-        """Run one batch.
-
-        Args:
-            batch (EasyTPP.BatchEncoding): preprocessed batch data that go into the model.
-            phase (RunnerPhase): a const that defines the stage of model runner.
-
-        Returns:
-            tuple: for training and validation we return loss, prediction and labels;
-            for prediction we return prediction.
-        """
-        model = self.model
-        sess = self.sess
-
-        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch.data.values()
-
-        # set mode to train
-        is_training = (phase == RunnerPhase.TRAIN)
-
-        fd = {
-            model.time_seqs: time_seqs,
-            model.time_delta_seqs: time_delta_seqs,
-            model.type_seqs: type_seqs,
-            model.batch_non_pad_mask: batch_non_pad_mask,
-            model.attention_mask: attention_mask,
-            model.type_mask: type_mask,
-            model.is_training: is_training
-
-        }
-
-        # Assume we dont do prediction on train set
-        pred_dtime, pred_type = None, None
-        label_dtime, label_type = time_delta_seqs[:, 1:], type_seqs[:, 1:]
-
-        mask = batch_non_pad_mask[:, 1:]
-
-        if phase in (RunnerPhase.TRAIN, RunnerPhase.VALIDATE):
-            # set mode to train
-            if is_training:
-                _, loss, num_event = sess.run([self.train_op,
-                                               model.loss,
-                                               model.num_event],
-                                              feed_dict=fd)
-            else:
-                loss, num_event = sess.run([model.loss,
-                                            model.num_event],
-                                           feed_dict=fd)
-
-                if self.model.event_sampler:
-                    pred_dtime, pred_type = sess.run([model.dtime_predict_one_step,
-                                                      model.type_predict_one_step],
-                                                     feed_dict=fd)
-            return loss, num_event, (pred_dtime, pred_type), (label_dtime, label_type), (mask,)
-        else:
-            pred_dtime, pred_type = sess.run([model.dtime_generation,
-                                              model.type_generation],
-                                             feed_dict=fd)
-            num_steps = pred_dtime.shape[-1]
-            label_dtime = time_delta_seqs[:, -num_steps:]
-            label_type = type_seqs[:, -num_steps:]
-            return (pred_dtime, pred_type), (label_dtime, label_type)
+""" Initialize a Tf model wrapper that feed into Model Runner   """
+
+import tensorflow as tf
+
+from easy_tpp.utils import RunnerPhase
+from easy_tpp.utils.tf_utils import set_device, set_optimizer
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+class TfModelWrapper:
+    def __init__(self, model, base_config, model_config, trainer_config):
+        """A wrapper class for Tensorflow backends.
+
+        Args:
+            model (BaseModel): a TPP model.
+            base_config (EasyTPP.Config): basic configs.
+            model_config (EasyTPP.Config): model spec configs.
+            trainer_config (EasyTPP.Config): trainer spec configs.
+        """
+        self.model = model
+        self.base_config = base_config
+        self.model_config = model_config
+        self.trainer_config = trainer_config
+        set_device(self.trainer_config.gpu)
+
+        # init session and build model
+        tf.reset_default_graph()
+        self.sess = tf.Session()
+        self.model.build_graph()
+        if self.model_config.is_training:
+            # set up optimizer
+            optimizer = self.trainer_config.optimizer
+            self.learning_rate = self.trainer_config.learning_rate
+            self.opt = set_optimizer(optimizer, self.learning_rate)
+            self.train_op = self.opt.minimize(self.model.loss)
+
+        # set up tensorboard
+        self.use_tfb = self.trainer_config.use_tfb
+        self.train_summary_writer, self.valid_summary_writer = None, None
+        if self.use_tfb:
+            self.train_summary_writer = tf.summary.FileWriter(self.base_config.spec['tfb_train_dir'])
+            self.valid_summary_writer = tf.summary.FileWriter(self.base_config.spec['tfb_valid_dir'])
+
+        # init variable and saver
+        self.sess.run(tf.global_variables_initializer())
+        self.saver = tf.train.Saver()
+
+    def restore(self, ckpt_dir):
+        """Load the checkpoint to restore the model.
+
+        Args:
+            ckpt_dir (str): path for the checkpoint.
+        """
+        self.saver.restore(self.sess, ckpt_dir)
+
+    def save(self, ckpt_dir):
+        """Save the checkpoint for the model.
+
+        Args:
+            ckpt_dir (str): path for the checkpoint.
+        """
+        self.saver.save(self.sess, ckpt_dir)
+
+    def write_summary(self, epoch, kv_pairs, phase):
+        """Write the kv_paris into the tensorboard.
+
+        Args:
+            epoch (int): epoch index in the training.
+            kv_pairs (dict): metrics dict.
+            phase (RunnerPhase): a const that defines the stage of model runner.
+        """
+        if self.use_tfb:
+            summary_writer = None
+            if phase == RunnerPhase.TRAIN:
+                summary_writer = self.train_summary_writer
+            elif phase == RunnerPhase.VALIDATE:
+                summary_writer = self.valid_summary_writer
+            elif phase == RunnerPhase.PREDICT:
+                pass
+
+            metric_summary = tf.Summary()
+            if summary_writer is not None:
+                for k, v in kv_pairs.items():
+                    if k != 'num_events':
+                        metric_summary.value.add(tag=k, simple_value=v)
+                        summary_writer.add_summary(metric_summary, epoch)
+
+                summary_writer.flush()
+        return
+
+    def close_summary(self):
+        """Close the tensorboard summary writer.
+        """
+        if self.train_summary_writer is not None:
+            self.train_summary_writer.close()
+
+        if self.valid_summary_writer is not None:
+            self.valid_summary_writer.close()
+        return
+
+    def run_batch(self, batch, phase):
+        """Run one batch.
+
+        Args:
+            batch (EasyTPP.BatchEncoding): preprocessed batch data that go into the model.
+            phase (RunnerPhase): a const that defines the stage of model runner.
+
+        Returns:
+            tuple: for training and validation we return loss, prediction and labels;
+            for prediction we return prediction.
+        """
+        model = self.model
+        sess = self.sess
+
+        time_seqs, time_delta_seqs, type_seqs, batch_non_pad_mask, attention_mask, type_mask = batch.data.values()
+
+        # set mode to train
+        is_training = (phase == RunnerPhase.TRAIN)
+
+        fd = {
+            model.time_seqs: time_seqs,
+            model.time_delta_seqs: time_delta_seqs,
+            model.type_seqs: type_seqs,
+            model.batch_non_pad_mask: batch_non_pad_mask,
+            model.attention_mask: attention_mask,
+            model.type_mask: type_mask,
+            model.is_training: is_training
+
+        }
+
+        # Assume we dont do prediction on train set
+        pred_dtime, pred_type = None, None
+        label_dtime, label_type = time_delta_seqs[:, 1:], type_seqs[:, 1:]
+
+        mask = batch_non_pad_mask[:, 1:]
+
+        if phase in (RunnerPhase.TRAIN, RunnerPhase.VALIDATE):
+            # set mode to train
+            if is_training:
+                _, loss, num_event = sess.run([self.train_op,
+                                               model.loss,
+                                               model.num_event],
+                                              feed_dict=fd)
+            else:
+                loss, num_event = sess.run([model.loss,
+                                            model.num_event],
+                                           feed_dict=fd)
+
+                if self.model.event_sampler:
+                    pred_dtime, pred_type = sess.run([model.dtime_predict_one_step,
+                                                      model.type_predict_one_step],
+                                                     feed_dict=fd)
+            return loss, num_event, (pred_dtime, pred_type), (label_dtime, label_type), (mask,)
+        else:
+            pred_dtime, pred_type = sess.run([model.dtime_generation,
+                                              model.type_generation],
+                                             feed_dict=fd)
+            num_steps = pred_dtime.shape[-1]
+            label_dtime = time_delta_seqs[:, -num_steps:]
+            label_type = type_seqs[:, -num_steps:]
+            return (pred_dtime, pred_type), (label_dtime, label_type)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/torch_wrapper.py` & `easy_tpp-0.0.5/easy_tpp/torch_wrapper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-""" Initialize a Pytorch model wrapper that feed into Model Runner   """
-
-import torch
-from torch.utils.tensorboard import SummaryWriter
-
-from easy_tpp.utils import RunnerPhase, set_optimizer, set_device
-
-
-class TorchModelWrapper:
-    def __init__(self, model, base_config, model_config, trainer_config):
-        """A wrapper class for Torch backends.
-
-        Args:
-            model (BaseModel): a TPP model.
-            base_config (EasyTPP.Config): basic configs.
-            model_config (EasyTPP.ModelConfig): model spec configs.
-            trainer_config (EasyTPP.TrainerConfig): trainer spec configs.
-        """
-        self.model = model
-        self.base_config = base_config
-        self.model_config = model_config
-        self.trainer_config = trainer_config
-
-        self.model_id = self.base_config.model_id
-        self.device = set_device(self.trainer_config.gpu)
-
-        self.model.to(self.device)
-
-        if self.model_config.is_training:
-            # set up optimizer
-            optimizer = self.trainer_config.optimizer
-            self.learning_rate = self.trainer_config.learning_rate
-            self.opt = set_optimizer(optimizer, self.model.parameters(), self.learning_rate)
-
-        # set up tensorboard
-        self.use_tfb = self.trainer_config.use_tfb
-        self.train_summary_writer, self.valid_summary_writer = None, None
-        if self.use_tfb:
-            self.train_summary_writer = SummaryWriter(log_dir=self.base_config.spec['tfb_train_dir'])
-            self.valid_summary_writer = SummaryWriter(log_dir=self.base_config.spec['tfb_valid_dir'])
-
-    def restore(self, ckpt_dir):
-        """Load the checkpoint to restore the model.
-
-        Args:
-            ckpt_dir (str): path for the checkpoint.
-        """
-
-        self.model.load_state_dict(torch.load(ckpt_dir), strict=False)
-
-    def save(self, ckpt_dir):
-        """Save the checkpoint for the model.
-
-        Args:
-            ckpt_dir (str): path for the checkpoint.
-        """
-        torch.save(self.model.state_dict(), ckpt_dir)
-
-    def write_summary(self, epoch, kv_pairs, phase):
-        """Write the kv_paris into the tensorboard
-
-        Args:
-            epoch (int): epoch index in the training.
-            kv_pairs (dict): metrics dict.
-            phase (RunnerPhase): a const that defines the stage of model runner.
-        """
-        if self.use_tfb:
-            summary_writer = None
-            if phase == RunnerPhase.TRAIN:
-                summary_writer = self.train_summary_writer
-            elif phase == RunnerPhase.VALIDATE:
-                summary_writer = self.valid_summary_writer
-            elif phase == RunnerPhase.PREDICT:
-                pass
-
-            if summary_writer is not None:
-                for k, v in kv_pairs.items():
-                    if k != 'num_events':
-                        summary_writer.add_scalar(k, v, epoch)
-
-                summary_writer.flush()
-        return
-
-    def close_summary(self):
-        """Close the tensorboard summary writer.
-        """
-        if self.train_summary_writer is not None:
-            self.train_summary_writer.close()
-
-        if self.valid_summary_writer is not None:
-            self.valid_summary_writer.close()
-        return
-
-    def run_batch(self, batch, phase):
-        """Run one batch.
-
-        Args:
-            batch (EasyTPP.BatchEncoding): preprocessed batch data that go into the model.
-            phase (RunnerPhase): a const that defines the stage of model runner.
-
-        Returns:
-            tuple: for training and validation we return loss, prediction and labels;
-            for prediction we return prediction.
-        """
-
-        batch = batch.to(self.device).values()
-        if phase in (RunnerPhase.TRAIN, RunnerPhase.VALIDATE):
-            # set mode to train
-            is_training = (phase == RunnerPhase.TRAIN)
-            self.model.train(is_training)
-
-            # FullyRNN needs grad event in validation stage
-            grad_flag = is_training if not self.model_id == 'FullyNN' else True
-            # run model
-            with torch.set_grad_enabled(grad_flag):
-                loss, num_event = self.model.loglike_loss(batch)
-
-            # Assume we dont do prediction on train set
-            pred_dtime, pred_type, label_dtime, label_type, mask = None, None, None, None, None
-
-            # update grad
-            if is_training:
-                self.opt.zero_grad()
-                (loss / num_event).backward()
-                self.opt.step()
-            else:  # by default we do not do evaluation on train set which may take a long time
-                if self.model.event_sampler:
-                    if batch[1] is not None and batch[2] is not None:
-                        label_dtime, label_type = batch[1][:, 1:].cpu().numpy(), batch[2][:, 1:].cpu().numpy()
-                    if batch[3] is not None:
-                        mask = batch[3][:, 1:].cpu().numpy()
-                    pred_dtime, pred_type = self.model.predict_one_step_at_every_event(batch=batch)
-                    pred_dtime = pred_dtime.detach().cpu().numpy()
-                    pred_type = pred_type.detach().cpu().numpy()
-
-            return loss.item(), num_event, (pred_dtime, pred_type), (label_dtime, label_type), (mask,)
-        else:
-            pred_dtime, pred_type, label_dtime, label_type = self.model.predict_multi_step_since_last_event(batch=batch)
-            pred_dtime = pred_dtime.detach().cpu().numpy()
-            pred_type = pred_type.detach().cpu().numpy()
-            label_dtime = label_dtime.detach().cpu().numpy()
-            label_type = label_type.detach().cpu().numpy()
-            return (pred_dtime, pred_type), (label_dtime, label_type)
+""" Initialize a Pytorch model wrapper that feed into Model Runner   """
+
+import torch
+from torch.utils.tensorboard import SummaryWriter
+
+from easy_tpp.utils import RunnerPhase, set_optimizer, set_device
+
+
+class TorchModelWrapper:
+    def __init__(self, model, base_config, model_config, trainer_config):
+        """A wrapper class for Torch backends.
+
+        Args:
+            model (BaseModel): a TPP model.
+            base_config (EasyTPP.Config): basic configs.
+            model_config (EasyTPP.ModelConfig): model spec configs.
+            trainer_config (EasyTPP.TrainerConfig): trainer spec configs.
+        """
+        self.model = model
+        self.base_config = base_config
+        self.model_config = model_config
+        self.trainer_config = trainer_config
+
+        self.model_id = self.base_config.model_id
+        self.device = set_device(self.trainer_config.gpu)
+
+        self.model.to(self.device)
+
+        if self.model_config.is_training:
+            # set up optimizer
+            optimizer = self.trainer_config.optimizer
+            self.learning_rate = self.trainer_config.learning_rate
+            self.opt = set_optimizer(optimizer, self.model.parameters(), self.learning_rate)
+
+        # set up tensorboard
+        self.use_tfb = self.trainer_config.use_tfb
+        self.train_summary_writer, self.valid_summary_writer = None, None
+        if self.use_tfb:
+            self.train_summary_writer = SummaryWriter(log_dir=self.base_config.spec['tfb_train_dir'])
+            self.valid_summary_writer = SummaryWriter(log_dir=self.base_config.spec['tfb_valid_dir'])
+
+    def restore(self, ckpt_dir):
+        """Load the checkpoint to restore the model.
+
+        Args:
+            ckpt_dir (str): path for the checkpoint.
+        """
+
+        self.model.load_state_dict(torch.load(ckpt_dir), strict=False)
+
+    def save(self, ckpt_dir):
+        """Save the checkpoint for the model.
+
+        Args:
+            ckpt_dir (str): path for the checkpoint.
+        """
+        torch.save(self.model.state_dict(), ckpt_dir)
+
+    def write_summary(self, epoch, kv_pairs, phase):
+        """Write the kv_paris into the tensorboard
+
+        Args:
+            epoch (int): epoch index in the training.
+            kv_pairs (dict): metrics dict.
+            phase (RunnerPhase): a const that defines the stage of model runner.
+        """
+        if self.use_tfb:
+            summary_writer = None
+            if phase == RunnerPhase.TRAIN:
+                summary_writer = self.train_summary_writer
+            elif phase == RunnerPhase.VALIDATE:
+                summary_writer = self.valid_summary_writer
+            elif phase == RunnerPhase.PREDICT:
+                pass
+
+            if summary_writer is not None:
+                for k, v in kv_pairs.items():
+                    if k != 'num_events':
+                        summary_writer.add_scalar(k, v, epoch)
+
+                summary_writer.flush()
+        return
+
+    def close_summary(self):
+        """Close the tensorboard summary writer.
+        """
+        if self.train_summary_writer is not None:
+            self.train_summary_writer.close()
+
+        if self.valid_summary_writer is not None:
+            self.valid_summary_writer.close()
+        return
+
+    def run_batch(self, batch, phase):
+        """Run one batch.
+
+        Args:
+            batch (EasyTPP.BatchEncoding): preprocessed batch data that go into the model.
+            phase (RunnerPhase): a const that defines the stage of model runner.
+
+        Returns:
+            tuple: for training and validation we return loss, prediction and labels;
+            for prediction we return prediction.
+        """
+
+        batch = batch.to(self.device).values()
+        if phase in (RunnerPhase.TRAIN, RunnerPhase.VALIDATE):
+            # set mode to train
+            is_training = (phase == RunnerPhase.TRAIN)
+            self.model.train(is_training)
+
+            # FullyRNN needs grad event in validation stage
+            grad_flag = is_training if not self.model_id == 'FullyNN' else True
+            # run model
+            with torch.set_grad_enabled(grad_flag):
+                loss, num_event = self.model.loglike_loss(batch)
+
+            # Assume we dont do prediction on train set
+            pred_dtime, pred_type, label_dtime, label_type, mask = None, None, None, None, None
+
+            # update grad
+            if is_training:
+                self.opt.zero_grad()
+                (loss / num_event).backward()
+                self.opt.step()
+            else:  # by default we do not do evaluation on train set which may take a long time
+                if self.model.event_sampler:
+                    if batch[1] is not None and batch[2] is not None:
+                        label_dtime, label_type = batch[1][:, 1:].cpu().numpy(), batch[2][:, 1:].cpu().numpy()
+                    if batch[3] is not None:
+                        mask = batch[3][:, 1:].cpu().numpy()
+                    pred_dtime, pred_type = self.model.predict_one_step_at_every_event(batch=batch)
+                    pred_dtime = pred_dtime.detach().cpu().numpy()
+                    pred_type = pred_type.detach().cpu().numpy()
+
+            return loss.item(), num_event, (pred_dtime, pred_type), (label_dtime, label_type), (mask,)
+        else:
+            pred_dtime, pred_type, label_dtime, label_type = self.model.predict_multi_step_since_last_event(batch=batch)
+            pred_dtime = pred_dtime.detach().cpu().numpy()
+            pred_type = pred_type.detach().cpu().numpy()
+            label_dtime = label_dtime.detach().cpu().numpy()
+            label_type = label_type.detach().cpu().numpy()
+            return (pred_dtime, pred_type), (label_dtime, label_type)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/const.py` & `easy_tpp-0.0.5/easy_tpp/utils/const.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from enum import Enum
-
-
-class ExplicitEnum(str, Enum):
-    """
-    Enum with more explicit error message for missing values.
-    """
-
-    def __str__(self):
-        return str(self.value)
-
-    @classmethod
-    def _missing_(cls, value):
-        raise ValueError(
-            f"{value} is not a valid {cls.__name__}, please select one of {list(cls._value2member_map_.keys())}"
-        )
-
-
-class PaddingStrategy(ExplicitEnum):
-    """
-    Possible values for the `padding` argument in [`EventTokenizer.__call__`]. Useful for tab-completion in an
-    IDE.
-    """
-
-    LONGEST = "longest"
-    MAX_LENGTH = "max_length"
-    DO_NOT_PAD = "do_not_pad"
-
-
-class TensorType(ExplicitEnum):
-    """
-    Possible values for the `return_tensors` argument in [`EventTokenizerBase.__call__`]. Useful for
-    tab-completion in an IDE.
-    """
-
-    PYTORCH = "pt"
-    TENSORFLOW = "tf"
-    NUMPY = "np"
-
-
-class RunnerPhase(ExplicitEnum):
-    """Model runner phase enum.
-    """
-    TRAIN = 'train'
-    VALIDATE = 'validate'
-    PREDICT = 'predict'
-
-
-class LossFunction(ExplicitEnum):
-    """Loss function for neural TPP model.
-    """
-    LOGLIKE = 'loglike'
-    PARTIAL_TIME_LOSS = 'rmse'
-    PARTIAL_EVENT_LOSS = 'accuracy'
-
-
-class LogConst:
-    """Format for log handler.
-    """
-    DEFAULT_FORMAT = '[%(asctime)s] [%(levelname)s] %(message)s'
-    DEFAULT_FORMAT_LONG = '%(asctime)s - %(filename)s[pid:%(process)d;line:%(lineno)d:%(funcName)s]' \
-                          ' - %(levelname)s: %(message)s'
-
-
-class PredOutputIndex:
-    """Positional index for the output tuple in ModelRunner.
-    """
-    TimePredIndex = 0
-    TypePredIndex = 1
-
-
-class DefaultRunnerConfig:
-    DEFAULT_DATASET_ID = 'conttime'
-
-
-class TruncationStrategy(ExplicitEnum):
-    """
-    Possible values for the `truncation` argument in [`EventTokenizer.__call__`]. Useful for tab-completion in
-    an IDE.
-    """
-
-    LONGEST_FIRST = "longest_first"
-    DO_NOT_TRUNCATE = "do_not_truncate"
-
-
-class Backend(ExplicitEnum):
-    """
-    Possible values for the `truncation` argument in [`EventTokenizer.__call__`]. Useful for tab-completion in
-    an IDE.
-    """
-
-    Torch = 'torch'
-    TF = 'tensorflow'
+from enum import Enum
+
+
+class ExplicitEnum(str, Enum):
+    """
+    Enum with more explicit error message for missing values.
+    """
+
+    def __str__(self):
+        return str(self.value)
+
+    @classmethod
+    def _missing_(cls, value):
+        raise ValueError(
+            f"{value} is not a valid {cls.__name__}, please select one of {list(cls._value2member_map_.keys())}"
+        )
+
+
+class PaddingStrategy(ExplicitEnum):
+    """
+    Possible values for the `padding` argument in [`EventTokenizer.__call__`]. Useful for tab-completion in an
+    IDE.
+    """
+
+    LONGEST = "longest"
+    MAX_LENGTH = "max_length"
+    DO_NOT_PAD = "do_not_pad"
+
+
+class TensorType(ExplicitEnum):
+    """
+    Possible values for the `return_tensors` argument in [`EventTokenizerBase.__call__`]. Useful for
+    tab-completion in an IDE.
+    """
+
+    PYTORCH = "pt"
+    TENSORFLOW = "tf"
+    NUMPY = "np"
+
+
+class RunnerPhase(ExplicitEnum):
+    """Model runner phase enum.
+    """
+    TRAIN = 'train'
+    VALIDATE = 'validate'
+    PREDICT = 'predict'
+
+
+class LossFunction(ExplicitEnum):
+    """Loss function for neural TPP model.
+    """
+    LOGLIKE = 'loglike'
+    PARTIAL_TIME_LOSS = 'rmse'
+    PARTIAL_EVENT_LOSS = 'accuracy'
+
+
+class LogConst:
+    """Format for log handler.
+    """
+    DEFAULT_FORMAT = '[%(asctime)s] [%(levelname)s] %(message)s'
+    DEFAULT_FORMAT_LONG = '%(asctime)s - %(filename)s[pid:%(process)d;line:%(lineno)d:%(funcName)s]' \
+                          ' - %(levelname)s: %(message)s'
+
+
+class PredOutputIndex:
+    """Positional index for the output tuple in ModelRunner.
+    """
+    TimePredIndex = 0
+    TypePredIndex = 1
+
+
+class DefaultRunnerConfig:
+    DEFAULT_DATASET_ID = 'conttime'
+
+
+class TruncationStrategy(ExplicitEnum):
+    """
+    Possible values for the `truncation` argument in [`EventTokenizer.__call__`]. Useful for tab-completion in
+    an IDE.
+    """
+
+    LONGEST_FIRST = "longest_first"
+    DO_NOT_TRUNCATE = "do_not_truncate"
+
+
+class Backend(ExplicitEnum):
+    """
+    Possible values for the `truncation` argument in [`EventTokenizer.__call__`]. Useful for tab-completion in
+    an IDE.
+    """
+
+    Torch = 'torch'
+    TF = 'tensorflow'
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/generic.py` & `easy_tpp-0.0.5/easy_tpp/utils/generic.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import numpy as np
-
-from easy_tpp.utils import is_torch_available, is_tf_available
-
-
-def is_tensor(x):
-    """
-    Tests if `x` is a `torch.Tensor`, `tf.Tensor`, `jaxlib.xla_extension.DeviceArray` or `np.ndarray`.
-    """
-    if is_torch_available():
-        import torch
-
-        if isinstance(x, torch.Tensor):
-            return True
-    if is_tf_available():
-        import tensorflow as tf
-
-        if isinstance(x, tf.Tensor):
-            return True
-
-    return isinstance(x, np.ndarray)
-
-
-def _is_numpy(x):
-    return isinstance(x, np.ndarray)
-
-
-def is_numpy_array(x):
-    """
-    Tests if `x` is a numpy array or not.
-    """
-    return _is_numpy(x)
-
-
-def _is_torch(x):
-    import torch
-
-    return isinstance(x, torch.Tensor)
-
-
-def is_torch_tensor(x):
-    """
-    Tests if `x` is a torch tensor or not. Safe to call even if torch is not installed.
-    """
-    return False if not is_torch_available() else _is_torch(x)
-
-
-def _is_torch_device(x):
-    import torch
-
-    return isinstance(x, torch.device)
-
-
-def is_torch_device(x):
-    """
-    Tests if `x` is a torch device or not. Safe to call even if torch is not installed.
-    """
-    return False if not is_torch_available() else _is_torch_device(x)
-
-
-def _is_torch_dtype(x):
-    import torch
-
-    if isinstance(x, str):
-        if hasattr(torch, x):
-            x = getattr(torch, x)
-        else:
-            return False
-    return isinstance(x, torch.dtype)
-
-
-def is_torch_dtype(x):
-    """
-    Tests if `x` is a torch dtype or not. Safe to call even if torch is not installed.
-    """
-    return False if not is_torch_available() else _is_torch_dtype(x)
-
-
-def _is_tensorflow(x):
-    import tensorflow as tf
-
-    return isinstance(x, tf.Tensor)
-
-
-def is_tf_tensor(x):
-    """
-    Tests if `x` is a tensorflow tensor or not. Safe to call even if tensorflow is not installed.
-    """
-    return False if not is_tf_available() else _is_tensorflow(x)
-
-
-def _is_tf_symbolic_tensor(x):
-    import tensorflow as tf
-
-    # the `is_symbolic_tensor` predicate is only available starting with TF 2.14
-    if hasattr(tf, "is_symbolic_tensor"):
-        return tf.is_symbolic_tensor(x)
-    return type(x) == tf.Tensor
-
-
-def is_tf_symbolic_tensor(x):
-    """
-    Tests if `x` is a tensorflow symbolic tensor or not (ie. not eager). Safe to call even if tensorflow is not
-    installed.
-    """
-    return False if not is_tf_available() else _is_tf_symbolic_tensor(x)
+import numpy as np
+
+from easy_tpp.utils import is_torch_available, is_tf_available
+
+
+def is_tensor(x):
+    """
+    Tests if `x` is a `torch.Tensor`, `tf.Tensor`, `jaxlib.xla_extension.DeviceArray` or `np.ndarray`.
+    """
+    if is_torch_available():
+        import torch
+
+        if isinstance(x, torch.Tensor):
+            return True
+    if is_tf_available():
+        import tensorflow as tf
+
+        if isinstance(x, tf.Tensor):
+            return True
+
+    return isinstance(x, np.ndarray)
+
+
+def _is_numpy(x):
+    return isinstance(x, np.ndarray)
+
+
+def is_numpy_array(x):
+    """
+    Tests if `x` is a numpy array or not.
+    """
+    return _is_numpy(x)
+
+
+def _is_torch(x):
+    import torch
+
+    return isinstance(x, torch.Tensor)
+
+
+def is_torch_tensor(x):
+    """
+    Tests if `x` is a torch tensor or not. Safe to call even if torch is not installed.
+    """
+    return False if not is_torch_available() else _is_torch(x)
+
+
+def _is_torch_device(x):
+    import torch
+
+    return isinstance(x, torch.device)
+
+
+def is_torch_device(x):
+    """
+    Tests if `x` is a torch device or not. Safe to call even if torch is not installed.
+    """
+    return False if not is_torch_available() else _is_torch_device(x)
+
+
+def _is_torch_dtype(x):
+    import torch
+
+    if isinstance(x, str):
+        if hasattr(torch, x):
+            x = getattr(torch, x)
+        else:
+            return False
+    return isinstance(x, torch.dtype)
+
+
+def is_torch_dtype(x):
+    """
+    Tests if `x` is a torch dtype or not. Safe to call even if torch is not installed.
+    """
+    return False if not is_torch_available() else _is_torch_dtype(x)
+
+
+def _is_tensorflow(x):
+    import tensorflow as tf
+
+    return isinstance(x, tf.Tensor)
+
+
+def is_tf_tensor(x):
+    """
+    Tests if `x` is a tensorflow tensor or not. Safe to call even if tensorflow is not installed.
+    """
+    return False if not is_tf_available() else _is_tensorflow(x)
+
+
+def _is_tf_symbolic_tensor(x):
+    import tensorflow as tf
+
+    # the `is_symbolic_tensor` predicate is only available starting with TF 2.14
+    if hasattr(tf, "is_symbolic_tensor"):
+        return tf.is_symbolic_tensor(x)
+    return type(x) == tf.Tensor
+
+
+def is_tf_symbolic_tensor(x):
+    """
+    Tests if `x` is a tensorflow symbolic tensor or not (ie. not eager). Safe to call even if tensorflow is not
+    installed.
+    """
+    return False if not is_tf_available() else _is_tf_symbolic_tensor(x)
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/import_utils.py` & `easy_tpp-0.0.5/easy_tpp/utils/import_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-import importlib.util
-import sys
-from collections import OrderedDict
-from typing import Union, Tuple
-
-from easy_tpp.utils.log_utils import default_logger as logger
-
-if sys.version_info < (3, 8):
-    import importlib_metadata
-else:
-    import importlib.metadata as importlib_metadata
-
-
-def _is_package_available(pkg_name: str, return_version: bool = False) -> Union[Tuple[bool, str], bool]:
-    # Check we're not importing a "pkg_name" directory somewhere but the actual library by trying to grab the version
-    package_exists = importlib.util.find_spec(pkg_name) is not None
-    package_version = "N/A"
-    if package_exists:
-        try:
-            package_version = importlib_metadata.version(pkg_name)
-        except importlib_metadata.PackageNotFoundError:
-            pass
-        logger.debug(f"Detected {pkg_name} version {package_version}")
-    if return_version:
-        return package_exists, package_version
-    else:
-        return package_exists
-
-
-_tf_available = _is_package_available("tensorflow")
-if _tf_available:
-    candidates = (
-        "tensorflow",
-        "tensorflow-cpu",
-        "tensorflow-gpu",
-        "tf-nightly",
-        "tf-nightly-cpu",
-        "tf-nightly-gpu",
-        "intel-tensorflow",
-        "intel-tensorflow-avx512",
-        "tensorflow-rocm",
-        "tensorflow-macos",
-        "tensorflow-aarch64",
-    )
-    _tf_version = None
-    # For the metadata, we have to look for both tensorflow and tensorflow-cpu
-    for pkg in candidates:
-        try:
-            _tf_version = importlib_metadata.version(pkg)
-            break
-        except importlib_metadata.PackageNotFoundError:
-            pass
-    _tf_available = _tf_version is not None
-
-_tensorflow_probability_available = _is_package_available("tensorflow_probability")
-_torchdistx_available = _is_package_available("torchdistx")
-_torchvision_available = _is_package_available("torchvision")
-
-_torch_available, _torch_version = _is_package_available("torch", return_version=True)
-
-
-def is_torch_available():
-    return _torch_available
-
-
-def get_torch_version():
-    return _torch_version
-
-
-def is_torchvision_available():
-    return _torchvision_available
-
-
-def is_torch_cuda_available():
-    if is_torch_available():
-        import torch
-
-        return torch.cuda.is_available()
-    else:
-        return False
-
-
-def is_tf_available():
-    return _tf_available
-
-
-def is_tf_gpu_available():
-    if is_tf_available():
-        import tensorflow as tf
-        if tf.__version__ >= '2.0':
-            return bool(tf.config.list_physical_devices("GPU"))
-        else:
-            from tensorflow.python.client import device_lib
-            local_device_protos = device_lib.list_local_devices()
-            for device in local_device_protos:
-                if device.device_type == 'GPU':
-                    return True
-    else:
-        return False
-
-
-def is_torch_mps_available():
-    if is_torch_available():
-        try:
-            import torch
-            torch.device('mps')
-            return True
-        except RuntimeError:
-            return False
-    else:
-        return False
-
-
-def is_torch_gpu_available():
-    is_cuda_available = is_torch_cuda_available()
-
-    is_mps_available = is_torch_mps_available()
-
-    return is_cuda_available | is_mps_available
-
-
-def is_tensorflow_probability_available():
-    return _tensorflow_probability_available
-
-
-def torch_only_method(fn):
-    def wrapper(*args, **kwargs):
-        if not _torch_available:
-            raise ImportError(
-                "You need to install pytorch to use this method or class, "
-                "or activate it with environment variables USE_TORCH=1 and USE_TF=0."
-            )
-        else:
-            return fn(*args, **kwargs)
-
-    return wrapper
-
-
-# docstyle-ignore
-PYTORCH_IMPORT_ERROR = """
-{0} requires the PyTorch library but it was not found in your environment. Checkout the instructions on the
-installation page: https://pytorch.org/get-started/locally/ and follow the ones that match your environment.
-Please note that you may need to restart your runtime after installation.
-"""
-
-# docstyle-ignore
-TORCHVISION_IMPORT_ERROR = """
-{0} requires the Torchvision library but it was not found in your environment. Checkout the instructions on the
-installation page: https://pytorch.org/get-started/locally/ and follow the ones that match your environment.
-Please note that you may need to restart your runtime after installation.
-"""
-
-# docstyle-ignore
-PYTORCH_IMPORT_ERROR_WITH_TF = """
-{0} requires the PyTorch library but it was not found in your environment.
-However, we were able to find a TensorFlow installation. TensorFlow classes begin
-with "TF", but are otherwise identically named to our PyTorch classes. This
-means that the TF equivalent of the class you tried to import would be "TF{0}".
-If you want to use TensorFlow, please use TF classes instead!
-
-If you really do want to use PyTorch please go to
-https://pytorch.org/get-started/locally/ and follow the instructions that
-match your environment.
-"""
-
-# docstyle-ignore
-TF_IMPORT_ERROR_WITH_PYTORCH = """
-{0} requires the TensorFlow library but it was not found in your environment.
-However, we were able to find a PyTorch installation. PyTorch classes do not begin
-with "TF", but are otherwise identically named to our TF classes.
-If you want to use PyTorch, please use those classes instead!
-
-If you really do want to use TensorFlow, please follow the instructions on the
-installation page https://www.tensorflow.org/install that match your environment.
-"""
-
-# docstyle-ignore
-TENSORFLOW_IMPORT_ERROR = """
-{0} requires the TensorFlow library but it was not found in your environment. Checkout the instructions on the
-installation page: https://www.tensorflow.org/install and follow the ones that match your environment.
-Please note that you may need to restart your runtime after installation.
-"""
-
-# docstyle-ignore
-TENSORFLOW_PROBABILITY_IMPORT_ERROR = """
-{0} requires the tensorflow_probability library but it was not found in your environment. You can install it with pip as
-explained here: https://github.com/tensorflow/probability.
-Please note that you may need to restart your runtime after installation.
-"""
-
-BACKENDS_MAPPING = OrderedDict(
-    [
-        ("tensorflow_probability", (is_tensorflow_probability_available, TENSORFLOW_PROBABILITY_IMPORT_ERROR)),
-        ("tf", (is_tf_available, TENSORFLOW_IMPORT_ERROR)),
-        ("torch", (is_torch_available, PYTORCH_IMPORT_ERROR)),
-        ("torchvision", (is_torchvision_available, TORCHVISION_IMPORT_ERROR))
-    ]
-)
-
-
-def requires_backends(obj, backends):
-    if not isinstance(backends, (list, tuple)):
-        backends = [backends]
-
-    name = obj.__name__ if hasattr(obj, "__name__") else obj.__class__.__name__
-
-    # Raise an error for users who might not realize that classes without "TF" are torch-only
-    if "torch" in backends and "tf" not in backends and not is_torch_available() and is_tf_available():
-        raise ImportError(PYTORCH_IMPORT_ERROR_WITH_TF.format(name))
-
-    # Raise the inverse error for PyTorch users trying to load TF classes
-    if "tf" in backends and "torch" not in backends and is_torch_available() and not is_tf_available():
-        raise ImportError(TF_IMPORT_ERROR_WITH_PYTORCH.format(name))
-
-    checks = (BACKENDS_MAPPING[backend] for backend in backends)
-    failed = [msg.format(name) for available, msg in checks if not available()]
-    if failed:
-        raise ImportError("".join(failed))
+import importlib.util
+import sys
+from collections import OrderedDict
+from typing import Union, Tuple
+
+from easy_tpp.utils.log_utils import default_logger as logger
+
+if sys.version_info < (3, 8):
+    import importlib_metadata
+else:
+    import importlib.metadata as importlib_metadata
+
+
+def _is_package_available(pkg_name: str, return_version: bool = False) -> Union[Tuple[bool, str], bool]:
+    # Check we're not importing a "pkg_name" directory somewhere but the actual library by trying to grab the version
+    package_exists = importlib.util.find_spec(pkg_name) is not None
+    package_version = "N/A"
+    if package_exists:
+        try:
+            package_version = importlib_metadata.version(pkg_name)
+        except importlib_metadata.PackageNotFoundError:
+            pass
+        logger.debug(f"Detected {pkg_name} version {package_version}")
+    if return_version:
+        return package_exists, package_version
+    else:
+        return package_exists
+
+
+_tf_available = _is_package_available("tensorflow")
+if _tf_available:
+    candidates = (
+        "tensorflow",
+        "tensorflow-cpu",
+        "tensorflow-gpu",
+        "tf-nightly",
+        "tf-nightly-cpu",
+        "tf-nightly-gpu",
+        "intel-tensorflow",
+        "intel-tensorflow-avx512",
+        "tensorflow-rocm",
+        "tensorflow-macos",
+        "tensorflow-aarch64",
+    )
+    _tf_version = None
+    # For the metadata, we have to look for both tensorflow and tensorflow-cpu
+    for pkg in candidates:
+        try:
+            _tf_version = importlib_metadata.version(pkg)
+            break
+        except importlib_metadata.PackageNotFoundError:
+            pass
+    _tf_available = _tf_version is not None
+
+_tensorflow_probability_available = _is_package_available("tensorflow_probability")
+_torchdistx_available = _is_package_available("torchdistx")
+_torchvision_available = _is_package_available("torchvision")
+
+_torch_available, _torch_version = _is_package_available("torch", return_version=True)
+
+
+def is_torch_available():
+    return _torch_available
+
+
+def get_torch_version():
+    return _torch_version
+
+
+def is_torchvision_available():
+    return _torchvision_available
+
+
+def is_torch_cuda_available():
+    if is_torch_available():
+        import torch
+
+        return torch.cuda.is_available()
+    else:
+        return False
+
+
+def is_tf_available():
+    return _tf_available
+
+
+def is_tf_gpu_available():
+    if is_tf_available():
+        import tensorflow as tf
+        if tf.__version__ >= '2.0':
+            return bool(tf.config.list_physical_devices("GPU"))
+        else:
+            from tensorflow.python.client import device_lib
+            local_device_protos = device_lib.list_local_devices()
+            for device in local_device_protos:
+                if device.device_type == 'GPU':
+                    return True
+    else:
+        return False
+
+
+def is_torch_mps_available():
+    if is_torch_available():
+        try:
+            import torch
+            torch.device('mps')
+            return True
+        except RuntimeError:
+            return False
+    else:
+        return False
+
+
+def is_torch_gpu_available():
+    is_cuda_available = is_torch_cuda_available()
+
+    is_mps_available = is_torch_mps_available()
+
+    return is_cuda_available | is_mps_available
+
+
+def is_tensorflow_probability_available():
+    return _tensorflow_probability_available
+
+
+def torch_only_method(fn):
+    def wrapper(*args, **kwargs):
+        if not _torch_available:
+            raise ImportError(
+                "You need to install pytorch to use this method or class, "
+                "or activate it with environment variables USE_TORCH=1 and USE_TF=0."
+            )
+        else:
+            return fn(*args, **kwargs)
+
+    return wrapper
+
+
+# docstyle-ignore
+PYTORCH_IMPORT_ERROR = """
+{0} requires the PyTorch library but it was not found in your environment. Checkout the instructions on the
+installation page: https://pytorch.org/get-started/locally/ and follow the ones that match your environment.
+Please note that you may need to restart your runtime after installation.
+"""
+
+# docstyle-ignore
+TORCHVISION_IMPORT_ERROR = """
+{0} requires the Torchvision library but it was not found in your environment. Checkout the instructions on the
+installation page: https://pytorch.org/get-started/locally/ and follow the ones that match your environment.
+Please note that you may need to restart your runtime after installation.
+"""
+
+# docstyle-ignore
+PYTORCH_IMPORT_ERROR_WITH_TF = """
+{0} requires the PyTorch library but it was not found in your environment.
+However, we were able to find a TensorFlow installation. TensorFlow classes begin
+with "TF", but are otherwise identically named to our PyTorch classes. This
+means that the TF equivalent of the class you tried to import would be "TF{0}".
+If you want to use TensorFlow, please use TF classes instead!
+
+If you really do want to use PyTorch please go to
+https://pytorch.org/get-started/locally/ and follow the instructions that
+match your environment.
+"""
+
+# docstyle-ignore
+TF_IMPORT_ERROR_WITH_PYTORCH = """
+{0} requires the TensorFlow library but it was not found in your environment.
+However, we were able to find a PyTorch installation. PyTorch classes do not begin
+with "TF", but are otherwise identically named to our TF classes.
+If you want to use PyTorch, please use those classes instead!
+
+If you really do want to use TensorFlow, please follow the instructions on the
+installation page https://www.tensorflow.org/install that match your environment.
+"""
+
+# docstyle-ignore
+TENSORFLOW_IMPORT_ERROR = """
+{0} requires the TensorFlow library but it was not found in your environment. Checkout the instructions on the
+installation page: https://www.tensorflow.org/install and follow the ones that match your environment.
+Please note that you may need to restart your runtime after installation.
+"""
+
+# docstyle-ignore
+TENSORFLOW_PROBABILITY_IMPORT_ERROR = """
+{0} requires the tensorflow_probability library but it was not found in your environment. You can install it with pip as
+explained here: https://github.com/tensorflow/probability.
+Please note that you may need to restart your runtime after installation.
+"""
+
+BACKENDS_MAPPING = OrderedDict(
+    [
+        ("tensorflow_probability", (is_tensorflow_probability_available, TENSORFLOW_PROBABILITY_IMPORT_ERROR)),
+        ("tf", (is_tf_available, TENSORFLOW_IMPORT_ERROR)),
+        ("torch", (is_torch_available, PYTORCH_IMPORT_ERROR)),
+        ("torchvision", (is_torchvision_available, TORCHVISION_IMPORT_ERROR))
+    ]
+)
+
+
+def requires_backends(obj, backends):
+    if not isinstance(backends, (list, tuple)):
+        backends = [backends]
+
+    name = obj.__name__ if hasattr(obj, "__name__") else obj.__class__.__name__
+
+    # Raise an error for users who might not realize that classes without "TF" are torch-only
+    if "torch" in backends and "tf" not in backends and not is_torch_available() and is_tf_available():
+        raise ImportError(PYTORCH_IMPORT_ERROR_WITH_TF.format(name))
+
+    # Raise the inverse error for PyTorch users trying to load TF classes
+    if "tf" in backends and "torch" not in backends and is_torch_available() and not is_tf_available():
+        raise ImportError(TF_IMPORT_ERROR_WITH_PYTORCH.format(name))
+
+    checks = (BACKENDS_MAPPING[backend] for backend in backends)
+    failed = [msg.format(name) for available, msg in checks if not available()]
+    if failed:
+        raise ImportError("".join(failed))
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/metrics.py` & `easy_tpp-0.0.5/easy_tpp/utils/metrics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from collections import defaultdict
-
-import numpy as np
-
-from easy_tpp.utils.log_utils import default_logger as logger
-
-
-class MetricsHelper:
-    MAXIMIZE = 'maximize'
-    MINIMIZE = 'minimize'
-    _registry_center = defaultdict(tuple)
-
-    @staticmethod
-    def get_metric_function(name):
-        if name in MetricsHelper._registry_center:
-            return MetricsHelper._registry_center[name][0]
-        else:
-            logger.warn(f'Metric is not found: {name}')
-            return None
-
-    @staticmethod
-    def get_metric_direction(name):
-        if name in MetricsHelper._registry_center:
-            return MetricsHelper._registry_center[name][1]
-        else:
-            return None
-
-    @staticmethod
-    def get_all_registered_metric():
-        return MetricsHelper._registry_center.values
-
-    @staticmethod
-    def register(name, direction, overwrite=True):
-        registry_center = MetricsHelper._registry_center
-
-        def _add_metric_to_registry(func):
-            if name in registry_center:
-                if overwrite:
-                    registry_center[name] = (func, direction)
-                else:
-                    logger.warn(f'The metric {name} is already registered, and cannot be overwritten!')
-            else:
-                registry_center[name] = (func, direction)
-            return func
-
-        return _add_metric_to_registry
-
-    @staticmethod
-    def metrics_dict_to_str(metrics_dict):
-        """ Convert metrics to a string to show in console  """
-        eval_info = ''
-        for k, v in metrics_dict.items():
-            eval_info += '{0} is {1}, '.format(k, v)
-
-        return eval_info[:-2]
-
-    @staticmethod
-    def get_metrics_callback_from_names(metric_names):
-        """ Metrics function callbacks    """
-        metric_functions = []
-        metric_names_ = []
-        for name in metric_names:
-            metric = MetricsHelper.get_metric_function(name)
-            if metric is not None:
-                metric_functions.append(metric)
-                metric_names_.append(name)
-
-        def metrics(preds, labels, **kwargs):
-            """ call metrics functions """
-            res = dict()
-            for metric_name, metric_func in zip(metric_names_, metric_functions):
-                res[metric_name.lower()] = metric_func(preds, labels, **kwargs)
-            return res
-
-        return metrics
-
-
-class MetricsTracker:
-    """Track and record the metrics.
-    """
-
-    def __init__(self):
-        self.current_best = {
-            'loglike': np.finfo(float).min,
-            'distance': np.finfo(float).max
-        }
-        self.episode_best = 'NeverUpdated'
-
-    def update_best(self, key, value, epoch):
-        """Update the recorder for the best metrics.
-
-        Args:
-            key (str): metrics key.
-            value (float): metrics value.
-            epoch (int): num of epoch.
-
-        Raises:
-            NotImplementedError: for keys other than 'loglike'.
-
-        Returns:
-            bool: whether the recorder has been updated.
-        """
-        updated = False
-        if key == 'loglike':
-            if value > self.current_best[key]:
-                updated = True
-                self.current_best[key] = value
-                self.episode_best = epoch
-        else:
-            raise NotImplementedError
-
-        return updated
+from collections import defaultdict
+
+import numpy as np
+
+from easy_tpp.utils.log_utils import default_logger as logger
+
+
+class MetricsHelper:
+    MAXIMIZE = 'maximize'
+    MINIMIZE = 'minimize'
+    _registry_center = defaultdict(tuple)
+
+    @staticmethod
+    def get_metric_function(name):
+        if name in MetricsHelper._registry_center:
+            return MetricsHelper._registry_center[name][0]
+        else:
+            logger.warn(f'Metric is not found: {name}')
+            return None
+
+    @staticmethod
+    def get_metric_direction(name):
+        if name in MetricsHelper._registry_center:
+            return MetricsHelper._registry_center[name][1]
+        else:
+            return None
+
+    @staticmethod
+    def get_all_registered_metric():
+        return MetricsHelper._registry_center.values
+
+    @staticmethod
+    def register(name, direction, overwrite=True):
+        registry_center = MetricsHelper._registry_center
+
+        def _add_metric_to_registry(func):
+            if name in registry_center:
+                if overwrite:
+                    registry_center[name] = (func, direction)
+                else:
+                    logger.warn(f'The metric {name} is already registered, and cannot be overwritten!')
+            else:
+                registry_center[name] = (func, direction)
+            return func
+
+        return _add_metric_to_registry
+
+    @staticmethod
+    def metrics_dict_to_str(metrics_dict):
+        """ Convert metrics to a string to show in console  """
+        eval_info = ''
+        for k, v in metrics_dict.items():
+            eval_info += '{0} is {1}, '.format(k, v)
+
+        return eval_info[:-2]
+
+    @staticmethod
+    def get_metrics_callback_from_names(metric_names):
+        """ Metrics function callbacks    """
+        metric_functions = []
+        metric_names_ = []
+        for name in metric_names:
+            metric = MetricsHelper.get_metric_function(name)
+            if metric is not None:
+                metric_functions.append(metric)
+                metric_names_.append(name)
+
+        def metrics(preds, labels, **kwargs):
+            """ call metrics functions """
+            res = dict()
+            for metric_name, metric_func in zip(metric_names_, metric_functions):
+                res[metric_name.lower()] = metric_func(preds, labels, **kwargs)
+            return res
+
+        return metrics
+
+
+class MetricsTracker:
+    """Track and record the metrics.
+    """
+
+    def __init__(self):
+        self.current_best = {
+            'loglike': np.finfo(float).min,
+            'distance': np.finfo(float).max
+        }
+        self.episode_best = 'NeverUpdated'
+
+    def update_best(self, key, value, epoch):
+        """Update the recorder for the best metrics.
+
+        Args:
+            key (str): metrics key.
+            value (float): metrics value.
+            epoch (int): num of epoch.
+
+        Raises:
+            NotImplementedError: for keys other than 'loglike'.
+
+        Returns:
+            bool: whether the recorder has been updated.
+        """
+        updated = False
+        if key == 'loglike':
+            if value > self.current_best[key]:
+                updated = True
+                self.current_best[key] = value
+                self.episode_best = epoch
+        else:
+            raise NotImplementedError
+
+        return updated
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/misc.py` & `easy_tpp-0.0.5/easy_tpp/utils/misc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-import copy
-import os
-import pickle
-
-import numpy as np
-import yaml
-
-from easy_tpp.utils.const import RunnerPhase
-
-
-def py_assert(condition, exception_type, msg):
-    """An assert function that ensures the condition holds, otherwise throws a message.
-
-    Args:
-        condition (bool): a formula to ensure validity.
-        exception_type (_StandardError): Error type, such as ValueError.
-        msg (str): a message to throw out.
-
-    Raises:
-        exception_type: throw an error when the condition does not hold.
-    """
-    if not condition:
-        raise exception_type(msg)
-
-
-def make_config_string(config, max_num_key=4):
-    """Generate a name for config files.
-
-    Args:
-        config (dict): configuration dict.
-        max_num_key (int, optional): max number of keys to concat in the output. Defaults to 4.
-
-    Returns:
-        dict: a concatenated string from config dict.
-    """
-    str_config = ''
-    num_key = 0
-    for k, v in config.items():
-        if num_key < max_num_key:  # for the moment we only record model name
-            if k == 'name':
-                str_config += str(v) + '_'
-                num_key += 1
-    return str_config[:-1]
-
-
-def save_yaml_config(save_dir, config):
-    """A function that saves a dict of config to yaml format file.
-
-    Args:
-        save_dir (str): the path to save config file.
-        config (dict): the target config object.
-    """
-    prt_dir = os.path.dirname(save_dir)
-
-    from collections import OrderedDict
-    # add yaml representer for different type
-    yaml.add_representer(
-        OrderedDict,
-        lambda dumper, data: dumper.represent_mapping('tag:yaml.org,2002:map', data.items())
-    )
-
-    if prt_dir != '' and not os.path.exists(prt_dir):
-        os.makedirs(prt_dir)
-
-    with open(save_dir, 'w') as f:
-        yaml.dump(config, stream=f, default_flow_style=False, sort_keys=False)
-
-    return
-
-
-def load_yaml_config(config_dir):
-    """ Load yaml config file from disk.
-
-    Args:
-        config_dir: str or Path
-            The path of the config file.
-
-    Returns:
-        Config: dict.
-    """
-    with open(config_dir) as config_file:
-        # load configs
-        config = yaml.load(config_file, Loader=yaml.FullLoader)
-
-    return config
-
-
-def get_stage(stage):
-    stage = stage.lower()
-    if stage in ['train', 'training']:
-        return RunnerPhase.TRAIN
-    elif stage in ['valid', 'dev', 'eval']:
-        return RunnerPhase.VALIDATE
-    else:
-        return RunnerPhase.PREDICT
-
-
-def create_folder(*args):
-    """Create path if the folder doesn't exist.
-
-    Returns:
-        str: the created folder's path.
-    """
-    path = os.path.join(*args)
-    if not os.path.exists(path):
-        os.makedirs(path)
-    return path
-
-
-def load_pickle(file_dir):
-    """Load from pickle file.
-
-    Args:
-        file_dir (BinaryIO): dir of the pickle file.
-
-    Returns:
-        any type: the loaded data.
-    """
-    with open(file_dir, 'rb') as file:
-        try:
-            data = pickle.load(file, encoding='latin-1')
-        except Exception:
-            data = pickle.load(file)
-
-    return data
-
-
-def save_pickle(file_dir, object_to_save):
-    """Save the object to a pickle file.
-
-    Args:
-        file_dir (str): dir of the pickle file.
-        object_to_save (any): the target data to be saved.
-    """
-
-    with open(file_dir, "wb") as f_out:
-        pickle.dump(object_to_save, f_out)
-
-    return
-
-
-def has_key(target_dict, target_keys):
-    """Check if the keys exist in the target dict.
-
-    Args:
-        target_dict (dict): a dict.
-        target_keys (str, list): list of keys.
-
-    Returns:
-        bool: True if all the key exist in the dict; False otherwise.
-    """
-    if not isinstance(target_keys, list):
-        target_keys = [target_keys]
-    for k in target_keys:
-        if k not in target_dict:
-            return False
-    return True
-
-
-def array_pad_cols(arr, max_num_cols, pad_index):
-    """Pad the array by columns.
-
-    Args:
-        arr (np.array): target array to be padded.
-        max_num_cols (int): target num cols for padded array.
-        pad_index (int): pad index to fill out the padded elements
-
-    Returns:
-        np.array: the padded array.
-    """
-    res = np.ones((arr.shape[0], max_num_cols)) * pad_index
-
-    res[:, :arr.shape[1]] = arr
-
-    return res
-
-
-def concat_element(arrs, pad_index):
-    """ Concat element from each batch output  """
-
-    n_lens = len(arrs)
-    n_elements = len(arrs[0])
-
-    # found out the max seq len (num cols) in output arrays
-    max_len = max([x[0].shape[1] for x in arrs])
-
-    concated_outputs = []
-    for j in range(n_elements):
-        a_output = []
-        for i in range(n_lens):
-            arrs_ = array_pad_cols(arrs[i][j], max_num_cols=max_len, pad_index=pad_index)
-            a_output.append(arrs_)
-
-        concated_outputs.append(np.concatenate(a_output, axis=0))
-
-    # n_elements * [ [n_lens, dim_of_element] ]
-    return concated_outputs
-
-
-def to_dict(obj, classkey=None):
-    if isinstance(obj, dict):
-        data = {}
-        for (k, v) in obj.items():
-            data[k] = to_dict(v, classkey)
-        return data
-    elif hasattr(obj, "_ast"):
-        return to_dict(obj._ast())
-    elif hasattr(obj, "__iter__"):
-        return [to_dict(v, classkey) for v in obj]
-    elif hasattr(obj, "__dict__"):
-        data = dict([(key, to_dict(value, classkey))
-                     for key, value in obj.__dict__.iteritems()
-                     if not callable(value) and not key.startswith('_') and key not in ['name']])
-        if classkey is not None and hasattr(obj, "__class__"):
-            data[classkey] = obj.__class__.__name__
-        return data
-    else:
-        return obj
-
-
-def dict_deep_update(target, source, is_add_new_key=True):
-    """ Update 'target' dict by 'source' dict deeply, and return a new dict copied from target and source deeply.
-
-    Args:
-        target: dict
-        source: dict
-        is_add_new_key: bool, default True.
-            Identify if add a key that in source but not in target into target.
-
-    Returns:
-        New target: dict. It contains the both target and source values, but keeps the values from source when the key
-        is duplicated.
-    """
-    # deep copy for avoiding to modify the original dict
-    result = copy.deepcopy(target) if target is not None else {}
-
-    if source is None:
-        return result
-
-    for key, value in source.items():
-        if key not in result:
-            if is_add_new_key:
-                result[key] = value
-            continue
-        # both target and source have the same key
-        base_type_list = [int, float, str, tuple, bool]
-        if type(result[key]) in base_type_list or type(source[key]) in base_type_list:
-            result[key] = value
-        else:
-            result[key] = dict_deep_update(result[key], source[key], is_add_new_key=is_add_new_key)
-    return result
+import copy
+import os
+import pickle
+
+import numpy as np
+import yaml
+
+from easy_tpp.utils.const import RunnerPhase
+
+
+def py_assert(condition, exception_type, msg):
+    """An assert function that ensures the condition holds, otherwise throws a message.
+
+    Args:
+        condition (bool): a formula to ensure validity.
+        exception_type (_StandardError): Error type, such as ValueError.
+        msg (str): a message to throw out.
+
+    Raises:
+        exception_type: throw an error when the condition does not hold.
+    """
+    if not condition:
+        raise exception_type(msg)
+
+
+def make_config_string(config, max_num_key=4):
+    """Generate a name for config files.
+
+    Args:
+        config (dict): configuration dict.
+        max_num_key (int, optional): max number of keys to concat in the output. Defaults to 4.
+
+    Returns:
+        dict: a concatenated string from config dict.
+    """
+    str_config = ''
+    num_key = 0
+    for k, v in config.items():
+        if num_key < max_num_key:  # for the moment we only record model name
+            if k == 'name':
+                str_config += str(v) + '_'
+                num_key += 1
+    return str_config[:-1]
+
+
+def save_yaml_config(save_dir, config):
+    """A function that saves a dict of config to yaml format file.
+
+    Args:
+        save_dir (str): the path to save config file.
+        config (dict): the target config object.
+    """
+    prt_dir = os.path.dirname(save_dir)
+
+    from collections import OrderedDict
+    # add yaml representer for different type
+    yaml.add_representer(
+        OrderedDict,
+        lambda dumper, data: dumper.represent_mapping('tag:yaml.org,2002:map', data.items())
+    )
+
+    if prt_dir != '' and not os.path.exists(prt_dir):
+        os.makedirs(prt_dir)
+
+    with open(save_dir, 'w') as f:
+        yaml.dump(config, stream=f, default_flow_style=False, sort_keys=False)
+
+    return
+
+
+def load_yaml_config(config_dir):
+    """ Load yaml config file from disk.
+
+    Args:
+        config_dir: str or Path
+            The path of the config file.
+
+    Returns:
+        Config: dict.
+    """
+    with open(config_dir) as config_file:
+        # load configs
+        config = yaml.load(config_file, Loader=yaml.FullLoader)
+
+    return config
+
+
+def get_stage(stage):
+    stage = stage.lower()
+    if stage in ['train', 'training']:
+        return RunnerPhase.TRAIN
+    elif stage in ['valid', 'dev', 'eval']:
+        return RunnerPhase.VALIDATE
+    else:
+        return RunnerPhase.PREDICT
+
+
+def create_folder(*args):
+    """Create path if the folder doesn't exist.
+
+    Returns:
+        str: the created folder's path.
+    """
+    path = os.path.join(*args)
+    if not os.path.exists(path):
+        os.makedirs(path)
+    return path
+
+
+def load_pickle(file_dir):
+    """Load from pickle file.
+
+    Args:
+        file_dir (BinaryIO): dir of the pickle file.
+
+    Returns:
+        any type: the loaded data.
+    """
+    with open(file_dir, 'rb') as file:
+        try:
+            data = pickle.load(file, encoding='latin-1')
+        except Exception:
+            data = pickle.load(file)
+
+    return data
+
+
+def save_pickle(file_dir, object_to_save):
+    """Save the object to a pickle file.
+
+    Args:
+        file_dir (str): dir of the pickle file.
+        object_to_save (any): the target data to be saved.
+    """
+
+    with open(file_dir, "wb") as f_out:
+        pickle.dump(object_to_save, f_out)
+
+    return
+
+
+def has_key(target_dict, target_keys):
+    """Check if the keys exist in the target dict.
+
+    Args:
+        target_dict (dict): a dict.
+        target_keys (str, list): list of keys.
+
+    Returns:
+        bool: True if all the key exist in the dict; False otherwise.
+    """
+    if not isinstance(target_keys, list):
+        target_keys = [target_keys]
+    for k in target_keys:
+        if k not in target_dict:
+            return False
+    return True
+
+
+def array_pad_cols(arr, max_num_cols, pad_index):
+    """Pad the array by columns.
+
+    Args:
+        arr (np.array): target array to be padded.
+        max_num_cols (int): target num cols for padded array.
+        pad_index (int): pad index to fill out the padded elements
+
+    Returns:
+        np.array: the padded array.
+    """
+    res = np.ones((arr.shape[0], max_num_cols)) * pad_index
+
+    res[:, :arr.shape[1]] = arr
+
+    return res
+
+
+def concat_element(arrs, pad_index):
+    """ Concat element from each batch output  """
+
+    n_lens = len(arrs)
+    n_elements = len(arrs[0])
+
+    # found out the max seq len (num cols) in output arrays
+    max_len = max([x[0].shape[1] for x in arrs])
+
+    concated_outputs = []
+    for j in range(n_elements):
+        a_output = []
+        for i in range(n_lens):
+            arrs_ = array_pad_cols(arrs[i][j], max_num_cols=max_len, pad_index=pad_index)
+            a_output.append(arrs_)
+
+        concated_outputs.append(np.concatenate(a_output, axis=0))
+
+    # n_elements * [ [n_lens, dim_of_element] ]
+    return concated_outputs
+
+
+def to_dict(obj, classkey=None):
+    if isinstance(obj, dict):
+        data = {}
+        for (k, v) in obj.items():
+            data[k] = to_dict(v, classkey)
+        return data
+    elif hasattr(obj, "_ast"):
+        return to_dict(obj._ast())
+    elif hasattr(obj, "__iter__"):
+        return [to_dict(v, classkey) for v in obj]
+    elif hasattr(obj, "__dict__"):
+        data = dict([(key, to_dict(value, classkey))
+                     for key, value in obj.__dict__.iteritems()
+                     if not callable(value) and not key.startswith('_') and key not in ['name']])
+        if classkey is not None and hasattr(obj, "__class__"):
+            data[classkey] = obj.__class__.__name__
+        return data
+    else:
+        return obj
+
+
+def dict_deep_update(target, source, is_add_new_key=True):
+    """ Update 'target' dict by 'source' dict deeply, and return a new dict copied from target and source deeply.
+
+    Args:
+        target: dict
+        source: dict
+        is_add_new_key: bool, default True.
+            Identify if add a key that in source but not in target into target.
+
+    Returns:
+        New target: dict. It contains the both target and source values, but keeps the values from source when the key
+        is duplicated.
+    """
+    # deep copy for avoiding to modify the original dict
+    result = copy.deepcopy(target) if target is not None else {}
+
+    if source is None:
+        return result
+
+    for key, value in source.items():
+        if key not in result:
+            if is_add_new_key:
+                result[key] = value
+            continue
+        # both target and source have the same key
+        base_type_list = [int, float, str, tuple, bool]
+        if type(result[key]) in base_type_list or type(source[key]) in base_type_list:
+            result[key] = value
+        else:
+            result[key] = dict_deep_update(result[key], source[key], is_add_new_key=is_add_new_key)
+    return result
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/multiprocess_utils.py` & `easy_tpp-0.0.5/easy_tpp/utils/multiprocess_utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import os
-import time
-
-
-def is_master_process():
-    """ Check if the process is the master process in all machines.
-
-    Returns:
-        bool
-    """
-    rank = 0 if os.getenv('RANK') is None else int(os.getenv('RANK'))
-    if rank == 0:
-        return True
-    else:
-        return False
-
-
-def is_local_master_process():
-    """ Check if the process is the master process in the local machine.
-
-    Returns:
-        bool
-    """
-    rank = 0 if os.getenv('RANK') is None else int(os.getenv('RANK'))
-    local_world_size = 1 if os.getenv('LOCAL_WORLD_SIZE') is None else int(os.getenv('LOCAL_WORLD_SIZE'))
-    if local_world_size == 0 or rank % local_world_size == 0:
-        return True
-    else:
-        return False
-
-
-def get_now_timestamp_id():
-    """ Get the current timestamp string.
-
-    Returns:
-        A string like yyMMdd_hhmmss
-    """
-    import datetime
-    return datetime.datetime.now().strftime('%y%m%d-%H%M%S')
-
-
-def get_unique_id():
-    """ Generate a unique id string based on process id (pid), thread id and timestamp.
-
-    Returns:
-        Unique id: str
-    """
-    import os
-    import threading
-    pid = os.getpid()
-    tid = threading.currentThread().ident
-    ts_id = get_now_timestamp_id()
-
-    return '{}_{}_{}'.format(pid, tid, ts_id)
-
-
-def parse_uri_to_protocol_and_path(uri):
-    """ Parse a uri into two parts, protocol and path. Set 'file' as default protocol when lack protocol.
-
-    Args:
-        uri: str
-            The uri to identify a resource, whose format is like 'protocol://uri'.
-
-    Returns:
-        Protocol: str. The method to access the resource.
-        URI: str. The location of the resource.
-    """
-
-    if uri is None:
-        return None, None
-    tokens = uri.split('://')
-    if len(tokens) == 2:
-        protocol = tokens[0]
-        path = tokens[1]
-    elif len(tokens) == 1:
-        protocol = 'file'
-        path = tokens[0]
-    else:
-        raise RuntimeError(f'Wrong url format: {uri}')
-
-    return protocol, path
-
-
-class Timer:
-    """Count the elapsing time between start and end.
-    """
-
-    def __init__(self, unit='m'):
-        unit = unit.lower()
-        if unit == 's':
-            self._unit = 1
-        elif unit == 'm':
-            self._unit = 60
-        elif unit == 'h':
-            self._unit = 1440
-        else:
-            raise RuntimeError('Unknown unit:', unit)
-
-        self.unit = unit
-        # default start time is set to the time the object initialized
-        self._start_time = time.time()
-
-    def start(self):
-        self._start_time = time.time()
-
-    def end(self):
-        end_time = time.time()
-        cost = (end_time - self._start_time) / self._unit
-        # reset the start time using the end time
-        self._start_time = end_time
-        return '%.3f%s' % (cost, self.unit)
-
-
-# -------------------------- Singleton Object --------------------------
-default_timer = Timer()
+import os
+import time
+
+
+def is_master_process():
+    """ Check if the process is the master process in all machines.
+
+    Returns:
+        bool
+    """
+    rank = 0 if os.getenv('RANK') is None else int(os.getenv('RANK'))
+    if rank == 0:
+        return True
+    else:
+        return False
+
+
+def is_local_master_process():
+    """ Check if the process is the master process in the local machine.
+
+    Returns:
+        bool
+    """
+    rank = 0 if os.getenv('RANK') is None else int(os.getenv('RANK'))
+    local_world_size = 1 if os.getenv('LOCAL_WORLD_SIZE') is None else int(os.getenv('LOCAL_WORLD_SIZE'))
+    if local_world_size == 0 or rank % local_world_size == 0:
+        return True
+    else:
+        return False
+
+
+def get_now_timestamp_id():
+    """ Get the current timestamp string.
+
+    Returns:
+        A string like yyMMdd_hhmmss
+    """
+    import datetime
+    return datetime.datetime.now().strftime('%y%m%d-%H%M%S')
+
+
+def get_unique_id():
+    """ Generate a unique id string based on process id (pid), thread id and timestamp.
+
+    Returns:
+        Unique id: str
+    """
+    import os
+    import threading
+    pid = os.getpid()
+    tid = threading.currentThread().ident
+    ts_id = get_now_timestamp_id()
+
+    return '{}_{}_{}'.format(pid, tid, ts_id)
+
+
+def parse_uri_to_protocol_and_path(uri):
+    """ Parse a uri into two parts, protocol and path. Set 'file' as default protocol when lack protocol.
+
+    Args:
+        uri: str
+            The uri to identify a resource, whose format is like 'protocol://uri'.
+
+    Returns:
+        Protocol: str. The method to access the resource.
+        URI: str. The location of the resource.
+    """
+
+    if uri is None:
+        return None, None
+    tokens = uri.split('://')
+    if len(tokens) == 2:
+        protocol = tokens[0]
+        path = tokens[1]
+    elif len(tokens) == 1:
+        protocol = 'file'
+        path = tokens[0]
+    else:
+        raise RuntimeError(f'Wrong url format: {uri}')
+
+    return protocol, path
+
+
+class Timer:
+    """Count the elapsing time between start and end.
+    """
+
+    def __init__(self, unit='m'):
+        unit = unit.lower()
+        if unit == 's':
+            self._unit = 1
+        elif unit == 'm':
+            self._unit = 60
+        elif unit == 'h':
+            self._unit = 1440
+        else:
+            raise RuntimeError('Unknown unit:', unit)
+
+        self.unit = unit
+        # default start time is set to the time the object initialized
+        self._start_time = time.time()
+
+    def start(self):
+        self._start_time = time.time()
+
+    def end(self):
+        end_time = time.time()
+        cost = (end_time - self._start_time) / self._unit
+        # reset the start time using the end time
+        self._start_time = end_time
+        return '%.3f%s' % (cost, self.unit)
+
+
+# -------------------------- Singleton Object --------------------------
+default_timer = Timer()
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/registrable.py` & `easy_tpp-0.0.5/easy_tpp/utils/registrable.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-from collections import defaultdict
-
-from .log_utils import default_logger as logger
-
-
-class Registrable:
-    """Any class that inherits from ``Registrable`` gains access to a named registry for its subclasses. To register them, just decorate them with the classmethod ``@BaseClass.register(name)``.
-
-    After which you can call ``BaseClass.list_available()`` to get the keys for the registered subclasses, and ``BaseClass.by_name(name)`` to get the corresponding subclass.
-
-    Note that the registry stores the subclasses themselves; not class instances. In most cases you would then call ``from_params(params)`` on the returned subclass.
-    """
-
-    _registry = defaultdict(dict)
-    _default_impl = None
-
-    @classmethod
-    def register(cls, name, constructor=None, overwrite=False):
-        """Register a class under a particular name.
-        Args:
-            name (str): The name to register the class under.
-            constructor (str): optional (default=None)
-                The name of the method to use on the class to construct the object.  If this is given,
-                we will use this method (which must be a ``classmethod``) instead of the default
-                constructor.
-            overwrite (bool) : optional (default=False)
-                If True, overwrites any existing models registered under ``name``. Else,
-                throws an error if a model is already registered under ``name``.
-
-        # Examples
-        To use this class, you would typically have a base class that inherits from ``Registrable``:
-        ```python
-        class Transform(Registrable):
-            ...
-        ```
-        Then, if you want to register a subclass, you decorate it like this:
-        ```python
-        @Transform.register("shift-transform")
-        class ShiftTransform(Transform):
-            def __init__(self, param1: int, param2: str):
-                ...
-        ```
-        Registering a class like this will let you instantiate a class from a config file, where you
-        give ``"type": "shift-transform"``, and keys corresponding to the parameters of the ``__init__``
-        method (note that for this to work, those parameters must have type annotations).
-        If you want to have the instantiation from a config file call a method other than the
-        constructor, either because you have several different construction paths that could be
-        taken for the same object (as we do in ``Transform``) or because you have logic you want to
-        happen before you get to the constructor, you can register a specific ``@classmethod`` as the constructor to use.
-        """
-        registry = Registrable._registry[cls]
-
-        def add_subclass_to_registry(subclass):
-            # Add to registry, raise an error if key has already been used.
-            if name in registry:
-                if overwrite:
-                    message = (
-                        f"{name} has already been registered as {registry[name][0].__name__}, but "
-                        f"overwrite=True, so overwriting with {cls.__name__}"
-                    )
-                    logger.info(message)
-                else:
-                    message = (
-                        f"Cannot register {name} as {cls.__name__}; "
-                        f"name already in use for {registry[name][0].__name__}"
-                    )
-                    raise RuntimeError(message)
-            registry[name] = (subclass, constructor)
-            return subclass
-
-        return add_subclass_to_registry
-
-    @classmethod
-    def by_name(cls, name):
-        """
-        Returns a callable function that constructs an argument of the registered class.  Because
-        you can register particular functions as constructors for specific names, this isn't
-        necessarily the ``__init__`` method of some class.
-        """
-        logger.debug(f"instantiating registered subclass {name} of {cls}")
-        subclass, constructor = cls.resolve_class_name(name)
-        if not constructor:
-            return subclass
-        else:
-            return getattr(subclass, constructor)
-
-    @classmethod
-    def resolve_class_name(cls, name):
-        """
-        Returns the subclass that corresponds to the given ``name``, along with the name of the
-        method that was registered as a constructor for that ``name``, if any.
-        This method also allows ``name`` to be a fully-specified module name, instead of a name that
-        was already added to the ``Registry``.  In that case, you cannot use a separate function as
-        a constructor (as you need to call ``cls.register()`` in order to tell us what separate
-        function to use).
-        """
-        if name in Registrable._registry[cls]:
-            subclass, constructor = Registrable._registry[cls].get(name)
-            return subclass, constructor
-        else:
-            for base_cls, v in Registrable._registry.items():
-                if name in v:
-                    subclass, constructor = Registrable._registry[base_cls].get(name)
-                    return subclass, constructor
-
-        if "." in name:
-            # This might be a fully qualified class name, so we'll try importing its "module"
-            # and finding it there.
-            parts = name.split(".")
-            submodule = ".".join(parts[:-1])
-            class_name = parts[-1]
-            import importlib
-            try:
-                module = importlib.import_module(submodule)
-            except ModuleNotFoundError:
-                raise RuntimeError(
-                    f"tried to interpret {name} as a path to a class "
-                    f"but unable to import module {submodule}"
-                )
-
-            try:
-                subclass = getattr(module, class_name)
-                constructor = None
-                return subclass, constructor
-            except AttributeError:
-                raise RuntimeError(
-                    f"tried to interpret {name} as a path to a class "
-                    f"but unable to find class {class_name} in {submodule}"
-                )
-
-        else:
-            # is not a qualified class name
-            raise RuntimeError(
-                f"{name} is not a registered name for {cls.__name__}. "
-                "You probably need to use the --include-package flag "
-                "to load your custom code. Alternatively, you can specify your choices "
-                """using fully-qualified paths, e.g. {"model": "my_module.models.MyModel"} """
-                "in which case they will be automatically imported correctly."
-            )
-
-    @classmethod
-    def list_available(cls):
-        """List default first if it exists"""
-        keys = list(Registrable._registry[cls].keys())
-        default = cls._default_impl
-
-        if default is None:
-            return keys
-        elif default not in keys:
-            raise RuntimeError(f"Default implementation {default} is not registered")
-        else:
-            return [default] + [k for k in keys if k != default]
-
-    @classmethod
-    def registry_dict(cls):
-        return Registrable._registry[cls]
+from collections import defaultdict
+
+from .log_utils import default_logger as logger
+
+
+class Registrable:
+    """Any class that inherits from ``Registrable`` gains access to a named registry for its subclasses. To register them, just decorate them with the classmethod ``@BaseClass.register(name)``.
+
+    After which you can call ``BaseClass.list_available()`` to get the keys for the registered subclasses, and ``BaseClass.by_name(name)`` to get the corresponding subclass.
+
+    Note that the registry stores the subclasses themselves; not class instances. In most cases you would then call ``from_params(params)`` on the returned subclass.
+    """
+
+    _registry = defaultdict(dict)
+    _default_impl = None
+
+    @classmethod
+    def register(cls, name, constructor=None, overwrite=False):
+        """Register a class under a particular name.
+        Args:
+            name (str): The name to register the class under.
+            constructor (str): optional (default=None)
+                The name of the method to use on the class to construct the object.  If this is given,
+                we will use this method (which must be a ``classmethod``) instead of the default
+                constructor.
+            overwrite (bool) : optional (default=False)
+                If True, overwrites any existing models registered under ``name``. Else,
+                throws an error if a model is already registered under ``name``.
+
+        # Examples
+        To use this class, you would typically have a base class that inherits from ``Registrable``:
+        ```python
+        class Transform(Registrable):
+            ...
+        ```
+        Then, if you want to register a subclass, you decorate it like this:
+        ```python
+        @Transform.register("shift-transform")
+        class ShiftTransform(Transform):
+            def __init__(self, param1: int, param2: str):
+                ...
+        ```
+        Registering a class like this will let you instantiate a class from a config file, where you
+        give ``"type": "shift-transform"``, and keys corresponding to the parameters of the ``__init__``
+        method (note that for this to work, those parameters must have type annotations).
+        If you want to have the instantiation from a config file call a method other than the
+        constructor, either because you have several different construction paths that could be
+        taken for the same object (as we do in ``Transform``) or because you have logic you want to
+        happen before you get to the constructor, you can register a specific ``@classmethod`` as the constructor to use.
+        """
+        registry = Registrable._registry[cls]
+
+        def add_subclass_to_registry(subclass):
+            # Add to registry, raise an error if key has already been used.
+            if name in registry:
+                if overwrite:
+                    message = (
+                        f"{name} has already been registered as {registry[name][0].__name__}, but "
+                        f"overwrite=True, so overwriting with {cls.__name__}"
+                    )
+                    logger.info(message)
+                else:
+                    message = (
+                        f"Cannot register {name} as {cls.__name__}; "
+                        f"name already in use for {registry[name][0].__name__}"
+                    )
+                    raise RuntimeError(message)
+            registry[name] = (subclass, constructor)
+            return subclass
+
+        return add_subclass_to_registry
+
+    @classmethod
+    def by_name(cls, name):
+        """
+        Returns a callable function that constructs an argument of the registered class.  Because
+        you can register particular functions as constructors for specific names, this isn't
+        necessarily the ``__init__`` method of some class.
+        """
+        logger.debug(f"instantiating registered subclass {name} of {cls}")
+        subclass, constructor = cls.resolve_class_name(name)
+        if not constructor:
+            return subclass
+        else:
+            return getattr(subclass, constructor)
+
+    @classmethod
+    def resolve_class_name(cls, name):
+        """
+        Returns the subclass that corresponds to the given ``name``, along with the name of the
+        method that was registered as a constructor for that ``name``, if any.
+        This method also allows ``name`` to be a fully-specified module name, instead of a name that
+        was already added to the ``Registry``.  In that case, you cannot use a separate function as
+        a constructor (as you need to call ``cls.register()`` in order to tell us what separate
+        function to use).
+        """
+        if name in Registrable._registry[cls]:
+            subclass, constructor = Registrable._registry[cls].get(name)
+            return subclass, constructor
+        else:
+            for base_cls, v in Registrable._registry.items():
+                if name in v:
+                    subclass, constructor = Registrable._registry[base_cls].get(name)
+                    return subclass, constructor
+
+        if "." in name:
+            # This might be a fully qualified class name, so we'll try importing its "module"
+            # and finding it there.
+            parts = name.split(".")
+            submodule = ".".join(parts[:-1])
+            class_name = parts[-1]
+            import importlib
+            try:
+                module = importlib.import_module(submodule)
+            except ModuleNotFoundError:
+                raise RuntimeError(
+                    f"tried to interpret {name} as a path to a class "
+                    f"but unable to import module {submodule}"
+                )
+
+            try:
+                subclass = getattr(module, class_name)
+                constructor = None
+                return subclass, constructor
+            except AttributeError:
+                raise RuntimeError(
+                    f"tried to interpret {name} as a path to a class "
+                    f"but unable to find class {class_name} in {submodule}"
+                )
+
+        else:
+            # is not a qualified class name
+            raise RuntimeError(
+                f"{name} is not a registered name for {cls.__name__}. "
+                "You probably need to use the --include-package flag "
+                "to load your custom code. Alternatively, you can specify your choices "
+                """using fully-qualified paths, e.g. {"model": "my_module.models.MyModel"} """
+                "in which case they will be automatically imported correctly."
+            )
+
+    @classmethod
+    def list_available(cls):
+        """List default first if it exists"""
+        keys = list(Registrable._registry[cls].keys())
+        default = cls._default_impl
+
+        if default is None:
+            return keys
+        elif default not in keys:
+            raise RuntimeError(f"Default implementation {default} is not registered")
+        else:
+            return [default] + [k for k in keys if k != default]
+
+    @classmethod
+    def registry_dict(cls):
+        return Registrable._registry[cls]
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/tf_utils.py` & `easy_tpp-0.0.5/easy_tpp/utils/tf_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import os
-import random
-
-import numpy as np
-import tensorflow as tf
-
-from easy_tpp.utils.import_utils import is_tf_gpu_available
-
-if tf.__version__ >= '2.0':
-    tf = tf.compat.v1
-    tf.disable_v2_behavior()
-
-
-def set_seed(seed=1029):
-    """Setup random seed.
-
-    Args:
-        seed (int, optional): random seed. Defaults to 1029.
-    """
-    random.seed(seed)
-    os.environ["PYTHONHASHSEED"] = str(seed)
-    np.random.seed(seed)
-    tf.random.set_random_seed(seed)
-
-
-def set_device(gpu=-1):
-    """Setup the device.
-
-    Args:
-        gpu (int, optional): Defaults to -1.
-    """
-    if gpu >= 0 and is_tf_gpu_available():
-        os.environ['CUDA_VISIBLE_DEVICES'] = str(gpu)
-    else:
-        os.environ['CUDA_VISIBLE_DEVICES'] = ''
-    return
-
-
-def set_optimizer(optimizer, lr):
-    """Setup the optimizer.
-
-    Args:
-        optimizer (str): name of the optimizer.
-        lr (float): learning rate.
-
-    Raises:
-        NotImplementedError: if the optimizer's name is wrong or the optimizer is not supported,
-        we raise error.
-
-    Returns:
-        tf.train.optimzer: tf optimizer.
-    """
-    optimizer = optimizer.capitalize() + 'Optimizer'
-    try:
-        optimizer = getattr(tf.train, optimizer)(learning_rate=lr)
-    except Exception:
-        raise NotImplementedError("optimizer={} is not supported.".format(optimizer))
-
-    return optimizer
-
-
-def get_shape_list(x):
-    """Deal with dynamic shape in tensorflow cleanly.
-
-    Args:
-        x (tensor): input tensor.
-
-    Returns:
-        list: shape list of the tensor.
-    """
-    static = x.shape.as_list()
-    dynamic = tf.shape(x)
-    return [dynamic[i] if s is None else s for i, s in enumerate(static)]
-
-
-def tensordot(tensor_a, tensor_b):
-    """ Tensor dot function. The last dimension of tensor_a and the first dimension of tensor_b must be the same.
-
-    Args:
-        tensor_a (tensor): input tensor.
-        tensor_b (tensor): input tensor.
-
-    Returns:
-        tensor: the result of tensor_a tensor dot tensor_b.
-    """
-    last_idx_a = len(tensor_a.get_shape().as_list()) - 1
-    return tf.tensordot(tensor_a, tensor_b, [[last_idx_a], [0]])
-
-
-def swap_axes(tensor, axis1, axis2):
-    """Interchange two axes of an tensor.
-    :param tensor:
-    :param axis1: First axis.
-    :param axis2: Second axis.
-    :return:
-    """
-    tensor_perm = list(range(len(tensor.shape.as_list())))
-    tensor_perm[axis1] = axis2
-    tensor_perm[axis2] = axis1
-
-    return tf.transpose(tensor, perm=tensor_perm)
-
-
-def create_tensor(shape, value):
-    """Creates a tensor with all elements set to be the value.
-
-    Args:
-        shape (list): the shape of the target tensor to be created.
-        value (float): value to fill the tensor.
-
-    Returns:
-        tensor: created tensor with target value filled.
-    """
-    tensor_shape = tf.stack(shape)
-    return tf.fill(tensor_shape, value)
-
-
-def count_model_params():
-    """Count the number of params of the model.
-
-    Args:
-        model (tf.keras.Model): a torch model.
-
-    Returns:
-        int: total num of the parameters.
-    """
-    return np.sum([np.prod(v.get_shape().as_list()) for v in tf.trainable_variables()])
+import os
+import random
+
+import numpy as np
+import tensorflow as tf
+
+from easy_tpp.utils.import_utils import is_tf_gpu_available
+
+if tf.__version__ >= '2.0':
+    tf = tf.compat.v1
+    tf.disable_v2_behavior()
+
+
+def set_seed(seed=1029):
+    """Setup random seed.
+
+    Args:
+        seed (int, optional): random seed. Defaults to 1029.
+    """
+    random.seed(seed)
+    os.environ["PYTHONHASHSEED"] = str(seed)
+    np.random.seed(seed)
+    tf.random.set_random_seed(seed)
+
+
+def set_device(gpu=-1):
+    """Setup the device.
+
+    Args:
+        gpu (int, optional): Defaults to -1.
+    """
+    if gpu >= 0 and is_tf_gpu_available():
+        os.environ['CUDA_VISIBLE_DEVICES'] = str(gpu)
+    else:
+        os.environ['CUDA_VISIBLE_DEVICES'] = ''
+    return
+
+
+def set_optimizer(optimizer, lr):
+    """Setup the optimizer.
+
+    Args:
+        optimizer (str): name of the optimizer.
+        lr (float): learning rate.
+
+    Raises:
+        NotImplementedError: if the optimizer's name is wrong or the optimizer is not supported,
+        we raise error.
+
+    Returns:
+        tf.train.optimzer: tf optimizer.
+    """
+    optimizer = optimizer.capitalize() + 'Optimizer'
+    try:
+        optimizer = getattr(tf.train, optimizer)(learning_rate=lr)
+    except Exception:
+        raise NotImplementedError("optimizer={} is not supported.".format(optimizer))
+
+    return optimizer
+
+
+def get_shape_list(x):
+    """Deal with dynamic shape in tensorflow cleanly.
+
+    Args:
+        x (tensor): input tensor.
+
+    Returns:
+        list: shape list of the tensor.
+    """
+    static = x.shape.as_list()
+    dynamic = tf.shape(x)
+    return [dynamic[i] if s is None else s for i, s in enumerate(static)]
+
+
+def tensordot(tensor_a, tensor_b):
+    """ Tensor dot function. The last dimension of tensor_a and the first dimension of tensor_b must be the same.
+
+    Args:
+        tensor_a (tensor): input tensor.
+        tensor_b (tensor): input tensor.
+
+    Returns:
+        tensor: the result of tensor_a tensor dot tensor_b.
+    """
+    last_idx_a = len(tensor_a.get_shape().as_list()) - 1
+    return tf.tensordot(tensor_a, tensor_b, [[last_idx_a], [0]])
+
+
+def swap_axes(tensor, axis1, axis2):
+    """Interchange two axes of an tensor.
+    :param tensor:
+    :param axis1: First axis.
+    :param axis2: Second axis.
+    :return:
+    """
+    tensor_perm = list(range(len(tensor.shape.as_list())))
+    tensor_perm[axis1] = axis2
+    tensor_perm[axis2] = axis1
+
+    return tf.transpose(tensor, perm=tensor_perm)
+
+
+def create_tensor(shape, value):
+    """Creates a tensor with all elements set to be the value.
+
+    Args:
+        shape (list): the shape of the target tensor to be created.
+        value (float): value to fill the tensor.
+
+    Returns:
+        tensor: created tensor with target value filled.
+    """
+    tensor_shape = tf.stack(shape)
+    return tf.fill(tensor_shape, value)
+
+
+def count_model_params():
+    """Count the number of params of the model.
+
+    Args:
+        model (tf.keras.Model): a torch model.
+
+    Returns:
+        int: total num of the parameters.
+    """
+    return np.sum([np.prod(v.get_shape().as_list()) for v in tf.trainable_variables()])
```

### Comparing `easy_tpp-0.0.4/easy_tpp/utils/torch_utils.py` & `easy_tpp-0.0.5/easy_tpp/utils/torch_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import os
-import random
-
-import numpy as np
-import torch
-
-from easy_tpp.utils.import_utils import is_torch_mps_available
-
-
-def set_seed(seed=1029):
-    """Setup random seed.
-
-    Args:
-        seed (int, optional): random seed. Defaults to 1029.
-    """
-    random.seed(seed)
-    os.environ["PYTHONHASHSEED"] = str(seed)
-    np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.backends.cudnn.deterministic = True
-
-
-def set_device(gpu=-1):
-    """Setup the device.
-
-    Args:
-        gpu (int, optional): num of GPU to use. Defaults to -1 (not use GPU, i.e., use CPU).
-    """
-    if gpu >= 0:
-        if torch.cuda.is_available():
-            device = torch.device("cuda:" + str(gpu))
-        elif is_torch_mps_available():
-            device = torch.device("mps")
-    else:
-        device = torch.device("cpu")
-    return device
-
-
-def set_optimizer(optimizer, params, lr):
-    """Setup the optimizer.
-
-    Args:
-        optimizer (str): name of the optimizer.
-        params (dict): dict of params for the optimizer.
-        lr (float): learning rate.
-
-    Raises:
-        NotImplementedError: if the optimizer's name is wrong or the optimizer is not supported,
-        we raise error.
-
-    Returns:
-        torch.optim: torch optimizer.
-    """
-    if isinstance(optimizer, str):
-        if optimizer.lower() == "adam":
-            optimizer = "Adam"
-    try:
-        optimizer = getattr(torch.optim, optimizer)(params, lr=lr)
-    except Exception:
-        raise NotImplementedError("optimizer={} is not supported.".format(optimizer))
-    return optimizer
-
-
-def count_model_params(model):
-    """Count the number of params of the model.
-
-    Args:
-        model (torch.nn.Moduel): a torch model.
-
-    Returns:
-        int: total num of the parameters.
-    """
-    return sum(p.numel() for p in model.parameters())
+import os
+import random
+
+import numpy as np
+import torch
+
+from easy_tpp.utils.import_utils import is_torch_mps_available
+
+
+def set_seed(seed=1029):
+    """Setup random seed.
+
+    Args:
+        seed (int, optional): random seed. Defaults to 1029.
+    """
+    random.seed(seed)
+    os.environ["PYTHONHASHSEED"] = str(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.backends.cudnn.deterministic = True
+
+
+def set_device(gpu=-1):
+    """Setup the device.
+
+    Args:
+        gpu (int, optional): num of GPU to use. Defaults to -1 (not use GPU, i.e., use CPU).
+    """
+    if gpu >= 0:
+        if torch.cuda.is_available():
+            device = torch.device("cuda:" + str(gpu))
+        elif is_torch_mps_available():
+            device = torch.device("mps")
+    else:
+        device = torch.device("cpu")
+    return device
+
+
+def set_optimizer(optimizer, params, lr):
+    """Setup the optimizer.
+
+    Args:
+        optimizer (str): name of the optimizer.
+        params (dict): dict of params for the optimizer.
+        lr (float): learning rate.
+
+    Raises:
+        NotImplementedError: if the optimizer's name is wrong or the optimizer is not supported,
+        we raise error.
+
+    Returns:
+        torch.optim: torch optimizer.
+    """
+    if isinstance(optimizer, str):
+        if optimizer.lower() == "adam":
+            optimizer = "Adam"
+    try:
+        optimizer = getattr(torch.optim, optimizer)(params, lr=lr)
+    except Exception:
+        raise NotImplementedError("optimizer={} is not supported.".format(optimizer))
+    return optimizer
+
+
+def count_model_params(model):
+    """Count the number of params of the model.
+
+    Args:
+        model (torch.nn.Moduel): a torch model.
+
+    Returns:
+        int: total num of the parameters.
+    """
+    return sum(p.numel() for p in model.parameters())
```

### Comparing `easy_tpp-0.0.4/easy_tpp.egg-info/SOURCES.txt` & `easy_tpp-0.0.5/easy_tpp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 easy_tpp/torch_wrapper.py
 easy_tpp.egg-info/PKG-INFO
 easy_tpp.egg-info/SOURCES.txt
 easy_tpp.egg-info/dependency_links.txt
 easy_tpp.egg-info/requires.txt
 easy_tpp.egg-info/top_level.txt
 easy_tpp/config_factory/__init__.py
-easy_tpp/config_factory/base_config.py
 easy_tpp/config_factory/config.py
 easy_tpp/config_factory/data_config.py
 easy_tpp/config_factory/hpo_config.py
 easy_tpp/config_factory/model_config.py
 easy_tpp/config_factory/runner_config.py
 easy_tpp/default_registers/__init__.py
 easy_tpp/default_registers/register_metrics.py
```

### Comparing `easy_tpp-0.0.4/setup.py` & `easy_tpp-0.0.5/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import codecs
-import os
-import re
-from setuptools import find_packages
-from setuptools import setup
-
-
-def readme():
-    with codecs.open('README.md', encoding='utf-8') as f:
-        content = f.read()
-    return content
-
-
-def get_version():
-    version_file = os.path.join(os.path.dirname(__file__), "version.py")
-    version_regex = r"__version__ = ['\"]([^'\"]*)['\"]"
-    with open(version_file, "r") as f:
-        version = re.search(version_regex, f.read(), re.M).group(1)
-        return version
-
-
-def parse_requirements(fname='requirements.txt'):
-    """Parse the package dependencies listed in a requirements file."""
-
-    def parse_line(line):
-        """Parse information from a line in a requirements text file."""
-        if line.startswith('-r '):
-            # Allow specifying requirements in other files
-            target = line.split(' ')[1]
-            for line in parse_require_file(target):
-                yield line
-        else:
-            yield line
-
-    def parse_require_file(fpath):
-        with codecs.open(fpath, 'r') as f:
-            for line in f.readlines():
-                line = line.strip()
-                if line and not line.startswith('#'):
-                    for ll in parse_line(line):
-                        yield ll
-
-    packages = list(parse_require_file(fname))
-    return packages
-
-
-setup(
-    name='easy_tpp',
-    version=get_version(),
-    description='An easy and flexible tool for neural temporal point process',
-    url = 'https://github.com/ant-research/EasyTemporalPointProcess/',
-    # long_description=readme(),
-    author='Alipay',
-    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
-    include_package_data=True,
-    classifiers=[
-        'Programming Language :: Python :: 3'
-    ],
-    install_requires=parse_requirements('requirements.txt'))
+import codecs
+import os
+import re
+from setuptools import find_packages
+from setuptools import setup
+
+
+def readme():
+    with codecs.open('README.md', encoding='utf-8') as f:
+        content = f.read()
+    return content
+
+
+def get_version():
+    version_file = os.path.join(os.path.dirname(__file__), "version.py")
+    version_regex = r"__version__ = ['\"]([^'\"]*)['\"]"
+    with open(version_file, "r") as f:
+        version = re.search(version_regex, f.read(), re.M).group(1)
+        return version
+
+
+def parse_requirements(fname='requirements.txt'):
+    """Parse the package dependencies listed in a requirements file."""
+
+    def parse_line(line):
+        """Parse information from a line in a requirements text file."""
+        if line.startswith('-r '):
+            # Allow specifying requirements in other files
+            target = line.split(' ')[1]
+            for line in parse_require_file(target):
+                yield line
+        else:
+            yield line
+
+    def parse_require_file(fpath):
+        with codecs.open(fpath, 'r') as f:
+            for line in f.readlines():
+                line = line.strip()
+                if line and not line.startswith('#'):
+                    for ll in parse_line(line):
+                        yield ll
+
+    packages = list(parse_require_file(fname))
+    return packages
+
+
+setup(
+    name='easy_tpp',
+    version=get_version(),
+    description='An easy and flexible tool for neural temporal point process',
+    url = 'https://github.com/ant-research/EasyTemporalPointProcess/',
+    # long_description=readme(),
+    author='Alipay',
+    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
+    include_package_data=True,
+    classifiers=[
+        'Programming Language :: Python :: 3'
+    ],
+    install_requires=parse_requirements('requirements.txt'))
```

