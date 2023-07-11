# Comparing `tmp/scml-0.6.0.tar.gz` & `tmp/scml-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scml-0.6.0.tar", last modified: Sun Jul  9 07:24:53 2023, max compression
+gzip compressed data, was "scml-0.6.1.tar", last modified: Tue Jul 11 06:46:46 2023, max compression
```

## Comparing `scml-0.6.0.tar` & `scml-0.6.1.tar`

### file list

```diff
@@ -1,129 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.853773 scml-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-09 07:24:38.000000 scml-0.6.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-09 07:24:38.000000 scml-0.6.0/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-09 07:24:38.000000 scml-0.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-09 07:24:38.000000 scml-0.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-09 07:24:38.000000 scml-0.6.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-09 07:24:38.000000 scml-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-09 07:24:38.000000 scml-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-09 07:24:38.000000 scml-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-09 07:24:38.000000 scml-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-09 07:24:38.000000 scml-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-09 07:24:53.853773 scml-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-09 07:24:38.000000 scml-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 07:24:53.853773 scml-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-09 07:24:38.000000 scml-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.813773 scml-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.821773 scml-0.6.0/src/scml/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107706 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    68914 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/cliadv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.825773 scml-0.6.0/src/scml/oneshot/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.829773 scml-0.6.0/src/scml/oneshot/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/aspiration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    26977 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/awi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/sysagents.py
--rw-r--r--   0 runner    (1001) docker     (123)    34415 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/ufun.py
--rw-r--r--   0 runner    (1001) docker     (123)    91353 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.833773 scml-0.6.0/src/scml/scml2019/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6797 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14622 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20378 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/awi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11709 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/bank.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57378 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23664 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/consumers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.833773 scml-0.6.0/src/scml/scml2019/factory_managers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/factory_managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38211 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/factory_managers/builtins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7189 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/insurance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8335 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/miners.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29300 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46524 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/simulators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59571 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/visualizers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   106856 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.833773 scml-0.6.0/src/scml/scml2020/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.837773 scml-0.6.0/src/scml/scml2020/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/bcse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/decentralizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/indneg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/moving.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/reactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    28174 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/satisficer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/awi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.841773 scml-0.6.0/src/scml/scml2020/components/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/negotiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20521 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/trading.py
--rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.841773 scml-0.6.0/src/scml/scml2020/services/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/services/controllers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27153 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/services/simulators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   130704 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   132429 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.841773 scml-0.6.0/src/scml/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.845773 scml-0.6.0/src/scml/vendor/quick/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29363 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/quick.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.821773 scml-0.6.0/src/scml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.853773 scml-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:38.000000 scml-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-09 07:24:38.000000 scml-0.6.0/tests/switches.py
--rw-r--r--   0 runner    (1001) docker     (123)    19023 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_can_run_tutorial2.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17344 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_factory2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_oneshot_do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_oneshot_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_oneshot_ufun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20339 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scheduler2019.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2019.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12090 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2019factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2019tournaments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2020factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2020tournaments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2021.py
--rw-r--r--   0 runner    (1001) docker     (123)    34967 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2021oneshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2021tournaments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2023.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2023oneshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_sync_jackson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-09 07:24:38.000000 scml-0.6.0/tox.ini
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.675560 scml-0.6.1/
+-rw-r--r--   0 yasser     (501) staff       (20)      483 2023-07-11 06:43:28.000000 scml-0.6.1/.bumpversion.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)     2769 2022-04-11 08:05:27.000000 scml-0.6.1/.cookiecutterrc
+-rw-r--r--   0 yasser     (501) staff       (20)      172 2022-04-11 08:05:27.000000 scml-0.6.1/.coveragerc
+-rw-r--r--   0 yasser     (501) staff       (20)      217 2022-04-11 08:05:27.000000 scml-0.6.1/.editorconfig
+-rw-r--r--   0 yasser     (501) staff       (20)     1190 2022-04-11 08:05:27.000000 scml-0.6.1/.travis.yml
+-rw-r--r--   0 yasser     (501) staff       (20)       61 2022-04-11 08:05:27.000000 scml-0.6.1/AUTHORS.rst
+-rw-r--r--   0 yasser     (501) staff       (20)    16685 2023-07-11 06:46:27.000000 scml-0.6.1/CHANGELOG.rst
+-rw-r--r--   0 yasser     (501) staff       (20)     2663 2022-04-11 08:05:27.000000 scml-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 yasser     (501) staff       (20)      740 2022-04-11 08:05:27.000000 scml-0.6.1/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)      524 2022-04-11 08:05:27.000000 scml-0.6.1/MANIFEST.in
+-rw-r--r--   0 yasser     (501) staff       (20)    18852 2023-07-11 06:46:46.675656 scml-0.6.1/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     4160 2023-07-11 06:43:28.000000 scml-0.6.1/README.rst
+-rw-r--r--   0 yasser     (501) staff       (20)      573 2023-07-11 06:46:46.680419 scml-0.6.1/setup.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)     2775 2023-07-11 06:43:28.000000 scml-0.6.1/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.378071 scml-0.6.1/src/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.397903 scml-0.6.1/src/scml/
+-rw-r--r--   0 yasser     (501) staff       (20)      212 2023-07-11 06:43:28.000000 scml-0.6.1/src/scml/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)      356 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/__main__.py
+-rw-r--r--   0 yasser     (501) staff       (20)   107717 2023-07-11 06:09:44.000000 scml-0.6.1/src/scml/cli.py
+-rw-r--r--   0 yasser     (501) staff       (20)    68869 2023-07-11 05:54:39.000000 scml-0.6.1/src/scml/cliadv.py
+-rw-r--r--   0 yasser     (501) staff       (20)     8932 2023-04-25 01:36:09.000000 scml-0.6.1/src/scml/common.py
+-rw-r--r--   0 yasser     (501) staff       (20)    12675 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/experiment.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.406646 scml-0.6.1/src/scml/oneshot/
+-rw-r--r--   0 yasser     (501) staff       (20)      787 2023-07-11 05:39:08.000000 scml-0.6.1/src/scml/oneshot/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     2041 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/oneshot/adapter.py
+-rw-r--r--   0 yasser     (501) staff       (20)    21864 2023-07-09 07:02:51.000000 scml-0.6.1/src/scml/oneshot/agent.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.409857 scml-0.6.1/src/scml/oneshot/agents/
+-rw-r--r--   0 yasser     (501) staff       (20)      175 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/oneshot/agents/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     5898 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/oneshot/agents/aspiration.py
+-rw-r--r--   0 yasser     (501) staff       (20)    14583 2023-07-09 07:02:51.000000 scml-0.6.1/src/scml/oneshot/agents/greedy.py
+-rw-r--r--   0 yasser     (501) staff       (20)      534 2023-07-09 07:02:51.000000 scml-0.6.1/src/scml/oneshot/agents/nothing.py
+-rw-r--r--   0 yasser     (501) staff       (20)     6467 2023-07-09 07:02:51.000000 scml-0.6.1/src/scml/oneshot/agents/random.py
+-rw-r--r--   0 yasser     (501) staff       (20)    25308 2023-07-11 05:59:46.000000 scml-0.6.1/src/scml/oneshot/awi.py
+-rw-r--r--   0 yasser     (501) staff       (20)    10834 2023-07-11 06:14:50.000000 scml-0.6.1/src/scml/oneshot/common.py
+-rw-r--r--   0 yasser     (501) staff       (20)     7161 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/oneshot/helper.py
+-rw-r--r--   0 yasser     (501) staff       (20)     2340 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/oneshot/mixins.py
+-rw-r--r--   0 yasser     (501) staff       (20)     4223 2023-07-10 00:47:48.000000 scml-0.6.1/src/scml/oneshot/policy.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.415100 scml-0.6.1/src/scml/oneshot/rl/
+-rw-r--r--   0 yasser     (501) staff       (20)      216 2023-07-10 22:07:06.000000 scml-0.6.1/src/scml/oneshot/rl/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    13100 2023-07-11 05:25:14.000000 scml-0.6.1/src/scml/oneshot/rl/action.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3978 2023-07-10 08:38:02.000000 scml-0.6.1/src/scml/oneshot/rl/agent.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1313 2023-07-11 01:03:45.000000 scml-0.6.1/src/scml/oneshot/rl/common.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3797 2023-07-11 00:57:53.000000 scml-0.6.1/src/scml/oneshot/rl/env.py
+-rw-r--r--   0 yasser     (501) staff       (20)    19196 2023-07-11 06:07:00.000000 scml-0.6.1/src/scml/oneshot/rl/factory.py
+-rw-r--r--   0 yasser     (501) staff       (20)    14937 2023-07-11 06:37:22.000000 scml-0.6.1/src/scml/oneshot/rl/observation.py
+-rw-r--r--   0 yasser     (501) staff       (20)     5933 2023-07-10 04:00:15.000000 scml-0.6.1/src/scml/oneshot/sysagents.py
+-rw-r--r--   0 yasser     (501) staff       (20)    34415 2023-03-09 00:25:27.000000 scml-0.6.1/src/scml/oneshot/ufun.py
+-rw-r--r--   0 yasser     (501) staff       (20)    91704 2023-07-11 06:03:16.000000 scml-0.6.1/src/scml/oneshot/world.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.433935 scml-0.6.1/src/scml/scml2019/
+-rwxr-xr-x   0 yasser     (501) staff       (20)     6797 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2019/__init__.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    14622 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2019/agent.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    20378 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2019/awi.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    11709 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2019/bank.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    57378 2023-07-09 08:43:43.000000 scml-0.6.1/src/scml/scml2019/common.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    23664 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2019/consumers.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.434904 scml-0.6.1/src/scml/scml2019/factory_managers/
+-rw-r--r--   0 yasser     (501) staff       (20)       52 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2019/factory_managers/__init__.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    38211 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2019/factory_managers/builtins.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     1027 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2019/helpers.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     7189 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2019/insurance.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     8335 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2019/miners.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    29300 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2019/schedulers.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    46524 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2019/simulators.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    59571 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2019/utils.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     2341 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2019/visualizers.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)   106856 2023-03-03 08:24:02.000000 scml-0.6.1/src/scml/scml2019/world.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.437813 scml-0.6.1/src/scml/scml2020/
+-rw-r--r--   0 yasser     (501) staff       (20)      883 2023-07-11 06:07:35.000000 scml-0.6.1/src/scml/scml2020/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    22600 2023-07-10 07:50:23.000000 scml-0.6.1/src/scml/scml2020/agent.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.442082 scml-0.6.1/src/scml/scml2020/agents/
+-rw-r--r--   0 yasser     (501) staff       (20)      389 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2020/agents/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)      901 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2020/agents/bcse.py
+-rw-r--r--   0 yasser     (501) staff       (20)     4599 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/agents/decentralizing.py
+-rw-r--r--   0 yasser     (501) staff       (20)     2012 2023-07-11 06:11:43.000000 scml-0.6.1/src/scml/scml2020/agents/do_nothing.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3838 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2020/agents/indneg.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1120 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2020/agents/moving.py
+-rw-r--r--   0 yasser     (501) staff       (20)      578 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/agents/random.py
+-rw-r--r--   0 yasser     (501) staff       (20)     2291 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2020/agents/reactive.py
+-rw-r--r--   0 yasser     (501) staff       (20)    28241 2023-07-11 06:11:16.000000 scml-0.6.1/src/scml/scml2020/agents/satisficer.py
+-rw-r--r--   0 yasser     (501) staff       (20)    29821 2023-03-03 08:24:01.000000 scml-0.6.1/src/scml/scml2020/awi.py
+-rw-r--r--   0 yasser     (501) staff       (20)     6306 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2020/common.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.445897 scml-0.6.1/src/scml/scml2020/components/
+-rw-r--r--   0 yasser     (501) staff       (20)      309 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2020/components/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    32796 2023-07-11 06:08:30.000000 scml-0.6.1/src/scml/scml2020/components/negotiation.py
+-rw-r--r--   0 yasser     (501) staff       (20)    20521 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/components/prediction.py
+-rw-r--r--   0 yasser     (501) staff       (20)    13383 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/components/production.py
+-rw-r--r--   0 yasser     (501) staff       (20)     8483 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/components/signing.py
+-rw-r--r--   0 yasser     (501) staff       (20)     2728 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2020/components/simulation.py
+-rw-r--r--   0 yasser     (501) staff       (20)    23305 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/components/trading.py
+-rw-r--r--   0 yasser     (501) staff       (20)    21723 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/scml2020/factory.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.447085 scml-0.6.1/src/scml/scml2020/services/
+-rw-r--r--   0 yasser     (501) staff       (20)      276 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/scml2020/services/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    16071 2023-07-09 07:02:51.000000 scml-0.6.1/src/scml/scml2020/services/controllers.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    27160 2023-07-11 06:08:57.000000 scml-0.6.1/src/scml/scml2020/services/simulators.py
+-rw-r--r--   0 yasser     (501) staff       (20)   132429 2023-03-03 08:24:02.000000 scml-0.6.1/src/scml/scml2020/world.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)   130704 2023-07-11 06:05:01.000000 scml-0.6.1/src/scml/utils.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.447598 scml-0.6.1/src/scml/vendor/
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/vendor/__init__.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.450317 scml-0.6.1/src/scml/vendor/quick/
+-rw-r--r--   0 yasser     (501) staff       (20)    35147 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/vendor/quick/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)     2452 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/vendor/quick/README.md
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/vendor/quick/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    29363 2023-03-03 08:21:07.000000 scml-0.6.1/src/scml/vendor/quick/quick.py
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:05:28.000000 scml-0.6.1/src/scml/vendor/quick/requirements.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.401534 scml-0.6.1/src/scml.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)    18852 2023-07-11 06:46:45.000000 scml-0.6.1/src/scml.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     3770 2023-07-11 06:46:45.000000 scml-0.6.1/src/scml.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-07-11 06:46:45.000000 scml-0.6.1/src/scml.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       64 2023-07-11 06:46:45.000000 scml-0.6.1/src/scml.egg-info/entry_points.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2022-04-14 23:48:08.000000 scml-0.6.1/src/scml.egg-info/not-zip-safe
+-rw-r--r--   0 yasser     (501) staff       (20)      189 2023-07-11 06:46:45.000000 scml-0.6.1/src/scml.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        5 2023-07-11 06:46:45.000000 scml-0.6.1/src/scml.egg-info/top_level.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.476069 scml-0.6.1/tests/
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:05:28.000000 scml-0.6.1/tests/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1727 2022-04-18 23:23:28.000000 scml-0.6.1/tests/switches.py
+-rw-r--r--   0 yasser     (501) staff       (20)    19030 2023-07-11 06:14:04.000000 scml-0.6.1/tests/test_can_run_tutorial2.py
+-rw-r--r--   0 yasser     (501) staff       (20)      213 2022-04-11 08:05:28.000000 scml-0.6.1/tests/test_cli.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    17344 2023-03-03 08:24:01.000000 scml-0.6.1/tests/test_factory2019.py
+-rw-r--r--   0 yasser     (501) staff       (20)      747 2022-04-11 08:05:28.000000 scml-0.6.1/tests/test_jupyter.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1057 2023-07-09 07:02:51.000000 scml-0.6.1/tests/test_oneshot_do_nothing.py
+-rw-r--r--   0 yasser     (501) staff       (20)     5165 2023-03-03 08:21:07.000000 scml-0.6.1/tests/test_oneshot_sync.py
+-rw-r--r--   0 yasser     (501) staff       (20)     4082 2023-03-03 08:21:07.000000 scml-0.6.1/tests/test_oneshot_ufun.py
+-rw-r--r--   0 yasser     (501) staff       (20)     2581 2023-07-11 06:38:24.000000 scml-0.6.1/tests/test_rl.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    20339 2023-03-03 08:21:07.000000 scml-0.6.1/tests/test_scheduler2019.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)      551 2022-04-11 08:05:28.000000 scml-0.6.1/tests/test_scml2019.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    12090 2023-03-03 08:24:01.000000 scml-0.6.1/tests/test_scml2019factory.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     2624 2023-03-03 08:24:01.000000 scml-0.6.1/tests/test_scml2019tournaments.py
+-rw-r--r--   0 yasser     (501) staff       (20)    11164 2023-03-03 08:21:07.000000 scml-0.6.1/tests/test_scml2020.py
+-rw-r--r--   0 yasser     (501) staff       (20)     6264 2023-07-11 06:12:41.000000 scml-0.6.1/tests/test_scml2020factory.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     3960 2023-07-11 06:14:02.000000 scml-0.6.1/tests/test_scml2020tournaments.py
+-rw-r--r--   0 yasser     (501) staff       (20)    19579 2023-07-11 06:14:03.000000 scml-0.6.1/tests/test_scml2021.py
+-rw-r--r--   0 yasser     (501) staff       (20)    34942 2023-07-11 06:14:05.000000 scml-0.6.1/tests/test_scml2021oneshot.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     8391 2023-07-11 06:14:02.000000 scml-0.6.1/tests/test_scml2021tournaments.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3651 2023-07-11 06:14:05.000000 scml-0.6.1/tests/test_scml2023.py
+-rw-r--r--   0 yasser     (501) staff       (20)     5097 2023-07-11 06:14:02.000000 scml-0.6.1/tests/test_scml2023oneshot.py
+-rw-r--r--   0 yasser     (501) staff       (20)    16854 2023-07-09 07:02:51.000000 scml-0.6.1/tests/test_sync_jackson.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.389469 scml-0.6.1/tests/tmp_notebooks/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-11 06:46:46.675115 scml-0.6.1/tests/tmp_notebooks/tutorials/
+-rw-r--r--   0 yasser     (501) staff       (20)  2014485 2023-07-11 06:44:22.000000 scml-0.6.1/tests/tmp_notebooks/tutorials/01.run_scml2020.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)   938509 2023-07-11 06:46:23.000000 scml-0.6.1/tests/tmp_notebooks/tutorials/02.develop_agent_scml2020_oneshot.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)  3070242 2023-07-11 06:45:23.000000 scml-0.6.1/tests/tmp_notebooks/tutorials/03.develop_agent_scml2020.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)  1253745 2023-07-11 06:44:32.000000 scml-0.6.1/tests/tmp_notebooks/tutorials/04.experiments.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)    54842 2023-07-11 06:44:43.000000 scml-0.6.1/tests/tmp_notebooks/tutorials/05.logs_and_stats.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)    22584 2023-07-11 06:44:46.000000 scml-0.6.1/tests/tmp_notebooks/tutorials/06.ideas.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)     1858 2022-04-11 08:05:28.000000 scml-0.6.1/tox.ini
```

### Comparing `scml-0.6.0/.cookiecutterrc` & `scml-0.6.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/.travis.yml` & `scml-0.6.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/CHANGELOG.rst` & `scml-0.6.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+0.6.1 (2023.7.9)
+----------------
+
+* Moving scml.scml2020.utils to scml.utils (to avoid a circular import in rl/factory)
+* This is an initial effort to have RL work for scml. Currently we are disabling the extra checks on observation and
+  world construction because they lead to failures. This needs to be rectified later.
+* Added the concept of a WorldFactory to generate worlds with predefined characteristics from the point of view of the learning agent.
+* Now environments, action managers, and observation managers all receive WorldFactory objects and automatically check for compatibility.
+
 0.6.0 (2023.7.9)
 ----------------
 
 * Upgrading to be compatible with NegMAS 0.10.0
 * Adding step_with() to oneshot allowing for single counter-offer set stepping of the simulation (to be used to expose the simulation as RL and MARL environments later).
 * Adding current_negotiation_details to OneShotAWI to get details of running negotiation
 * Adding managed sales, supplies, total_sales, total_supplies, needed_sales, and needed_supplies to the OneShotAWI
```

### Comparing `scml-0.6.0/CONTRIBUTING.rst` & `scml-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/LICENSE` & `scml-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/MANIFEST.in` & `scml-0.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/PKG-INFO` & `scml-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.6.0
+Version: 0.6.1
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: gui
-Provides-Extra: rl
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
@@ -85,14 +84,23 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.6.1 (2023.7.9)
+----------------
+
+* Moving scml.scml2020.utils to scml.utils (to avoid a circular import in rl/factory)
+* This is an initial effort to have RL work for scml. Currently we are disabling the extra checks on observation and
+  world construction because they lead to failures. This needs to be rectified later.
+* Added the concept of a WorldFactory to generate worlds with predefined characteristics from the point of view of the learning agent.
+* Now environments, action managers, and observation managers all receive WorldFactory objects and automatically check for compatibility.
+
 0.6.0 (2023.7.9)
 ----------------
 
 * Upgrading to be compatible with NegMAS 0.10.0
 * Adding step_with() to oneshot allowing for single counter-offer set stepping of the simulation (to be used to expose the simulation as RL and MARL environments later).
 * Adding current_negotiation_details to OneShotAWI to get details of running negotiation
 * Adding managed sales, supplies, total_sales, total_supplies, needed_sales, and needed_supplies to the OneShotAWI
```

### Comparing `scml-0.6.0/README.rst` & `scml-0.6.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/scml
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/scml.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/scml
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.6.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.6.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/yasserfarouk/scml/compare/v0.6.0...master
+    :target: https://github.com/yasserfarouk/scml/compare/v0.6.1...master
 
 .. |CI| image:: https://github.com/yasserfarouk/scml/workflows/CI/badge.svg
     :target: https://www.github.com/yasserfarouk/scml
     :alt: Build Status
 
 .. |PyPiPublished| image:: https://github.com/yasserfarouk/scml/workflows/PyPI/badge.svg
     :target: https://pypi.python.org/pypi/scml
```

### Comparing `scml-0.6.0/setup.cfg` & `scml-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/setup.py` & `scml-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="scml",
-    version="0.6.0",
+    version="0.6.1",
     description="ANAC Supply Chain Management League Platform",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -63,24 +63,25 @@
         'dataclasses; python_version < "3.7"',
         "click",
         "pytest",
         "hypothesis",
         "prettytable",
         "pulp",
         "python-constraint",
-        "negmas>=0.9.5",
+        "negmas>=0.10.0",
         "tqdm",
         "joblib",
         "jupyter",
         "gif",
         "mip",
+        "gymnasium[extra]",
+        "stable-baselines3",
     ],
     extras_require={
         "gui": ["pyqt5"],
-        "rl": ["gymnasium"],
     },
     setup_requires=["pytest-runner"],
     entry_points={
         "console_scripts": [
             "scml = scml.cli:main",
             "cliadv = scml.cliadv:cli",
         ]
```

### Comparing `scml-0.6.0/src/scml/cli.py` & `scml-0.6.1/src/scml/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 from scml.scml2019 import FactoryManager, SCML2019World
 from scml.scml2019.utils import (
     DefaultGreedyManager,
     anac2019_collusion,
     anac2019_sabotage,
     anac2019_std,
 )
-from scml.scml2020 import SCML2020Agent, is_system_agent
-from scml.scml2020.utils import (
+from scml.scml2020.agent import SCML2020Agent
+from scml.scml2020.common import is_system_agent
+from scml.scml2020.world import SCML2020World, SCML2021World, SCML2023World
+from scml.utils import (
     anac2020_collusion,
     anac2020_std,
     anac2021_collusion,
     anac2021_oneshot,
     anac2021_std,
     anac2023_collusion,
     anac2023_oneshot,
     anac2023_std,
 )
-from scml.scml2020.world import SCML2020World, SCML2021World, SCML2023World
 
 try:
     from scml.vendor.quick.quick import gui_option
 except:
 
     def gui_option(x):
         return x
@@ -692,15 +693,15 @@
     else:
         non_competitors = non_competitors.split(";")
         for i, cp in enumerate(non_competitors):
             if "." not in cp:
                 non_competitors[i] = ("scml.scml2020.agents.") + cp
 
     if non_competitors is None:
-        non_competitors = scml.scml2020.utils.DefaultAgents
+        non_competitors = scml.utils.DefaultAgents
         non_competitor_params = tuple({} for _ in range(len(non_competitors)))
     print(f"Tournament will be run between {len(all_competitors)} agents: ")
     pprint(all_competitors)
     print("Non-competitors are: ")
     pprint(non_competitors)
     runner = anac2020_std if ttype == "std" else anac2020_collusion
     parallelism = "parallel" if parallel else "serial"
@@ -2616,15 +2617,15 @@
     else:
         non_competitors = non_competitors.split(";")
         for i, cp in enumerate(non_competitors):
             if "." not in cp:
                 non_competitors[i] = ("scml.scml2020.agents.") + cp
 
     if non_competitors is None:
-        non_competitors = scml.scml2020.utils.DefaultAgents
+        non_competitors = scml.utils.DefaultAgents
         non_competitor_params = tuple({} for _ in range(len(non_competitors)))
     print(f"Tournament will be run between {len(all_competitors)} agents: ")
     pprint(all_competitors)
     print("Non-competitors are: ")
     pprint(non_competitors)
     runner = anac2020_std if ttype == "std" else anac2020_collusion
     parallelism = "parallel" if parallel else "serial"
```

### Comparing `scml-0.6.0/src/scml/cliadv.py` & `scml-0.6.1/src/scml/cliadv.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     anac2019_assigner,
     anac2019_config_generator,
     anac2019_sabotage_assigner,
     anac2019_sabotage_config_generator,
     anac2019_world_generator,
     sabotage_effectiveness,
 )
-from scml.scml2020.utils import (
+from scml.utils import (
     anac2020_world_generator,
     anac_assigner_std,
     anac_config_generator_std,
 )
 
 try:
     from .vendor.quick.quick import gui_option
@@ -737,15 +737,15 @@
             log_negotiations=log_negs,
             ignore_agent_exceptions=not raise_exceptions,
             ignore_contract_execution_exceptions=not raise_exceptions,
             **kwargs,
         )
     elif ttype.lower() == "anac2020std":
         if non_competitors is None:
-            non_competitors = scml.scml2020.utils.DefaultAgents
+            non_competitors = scml.utils.DefaultAgents
             non_competitor_params = tuple({} for _ in range(len(non_competitors)))
         print(f"Tournament will be run between {len(all_competitors)} agents: ")
         pprint(all_competitors)
         print("Non-competitors are: ")
         pprint(non_competitors)
         results = create_tournament(
             competitors=all_competitors,
@@ -760,15 +760,15 @@
             total_timeout=timeout,
             name=name,
             verbose=verbosity > 0,
             n_agents_per_competitor=1,
             world_generator=anac2020_world_generator,
             config_generator=anac_config_generator_std,
             config_assigner=anac_assigner_std,
-            score_calculator=scml.scml2020.utils.balance_calculator2020,
+            score_calculator=scml.utils.balance_calculator2020,
             min_factories_per_level=factories[0],
             max_factories_per_level=factories[1],
             compact=compact,
             n_steps=steps,
             log_ufuns=log_ufuns,
             log_negotiations=log_negs,
             ignore_agent_exceptions=not raise_exceptions,
@@ -807,15 +807,15 @@
             log_negotiations=log_negs,
             ignore_agent_exceptions=not raise_exceptions,
             ignore_contract_execution_exceptions=not raise_exceptions,
             **kwargs,
         )
     elif ttype.lower() in ("anac2020collusion", "anac2020"):
         if non_competitors is None:
-            non_competitors = scml.scml2020.utils.DefaultAgents
+            non_competitors = scml.utils.DefaultAgents
             non_competitor_params = tuple({} for _ in range(len(non_competitors)))
         print(f"Tournament will be run between {len(all_competitors)} agents: ")
         pprint(all_competitors)
         print("Non-competitors are: ")
         pprint(non_competitors)
         results = create_tournament(
             competitors=all_competitors,
@@ -830,15 +830,15 @@
             total_timeout=timeout,
             name=name,
             verbose=verbosity > 0,
             n_agents_per_competitor=agents,
             world_generator=anac2019_world_generator,
             config_generator=anac2019_config_generator,
             config_assigner=anac2019_assigner,
-            score_calculator=scml.scml2020.utils.balance_calculator2020,
+            score_calculator=scml.utils.balance_calculator2020,
             min_factories_per_level=factories[0],
             max_factories_per_level=factories[1],
             compact=compact,
             n_steps=steps,
             log_ufuns=log_ufuns,
             log_negotiations=log_negs,
             ignore_agent_exceptions=not raise_exceptions,
```

### Comparing `scml-0.6.0/src/scml/common.py` & `scml-0.6.1/src/scml/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/experiment.py` & `scml-0.6.1/src/scml/experiment.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/__init__.py` & `scml-0.6.1/src/scml/oneshot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .agent import *
 from .agents import *
 from .awi import *
 from .common import *
 from .policy import *
+from .rl import *
 from .sysagents import *
 from .ufun import *
 from .world import *
 
 
 def builtin_agent_types(as_str=False):
     """
@@ -28,9 +29,10 @@
     common.__all__
     + world.__all__
     + ufun.__all__
     + agent.__all__
     + policy.__all__
     + agents.__all__
     + awi.__all__
+    + rl.__all__
     + ["builtin_agent_types"]
 )
```

### Comparing `scml-0.6.0/src/scml/oneshot/adapter.py` & `scml-0.6.1/src/scml/oneshot/adapter.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/agent.py` & `scml-0.6.1/src/scml/oneshot/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/agents/aspiration.py` & `scml-0.6.1/src/scml/oneshot/agents/aspiration.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/agents/greedy.py` & `scml-0.6.1/src/scml/oneshot/agents/greedy.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/agents/nothing.py` & `scml-0.6.1/src/scml/oneshot/agents/nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/agents/random.py` & `scml-0.6.1/src/scml/oneshot/agents/random.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/awi.py` & `scml-0.6.1/src/scml/oneshot/awi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
 Implements the one shot version of the Agent-World Interface.
 
 """
 from __future__ import annotations
 
+import itertools
 from collections import defaultdict
-from typing import Any, Dict, List, Literal, Optional, Tuple
+from typing import Any, Literal
 
 import numpy as np
 from negmas import AgentWorldInterface
 from negmas.outcomes import DiscreteCartesianOutcomeSpace, Issue, make_os
 from negmas.sao import SAOState
 
-from ..scml2020 import FinancialReport, is_system_agent
-from .common import NegotiationDetails, OneShotProfile, OneShotState
+from .common import (
+    FinancialReport,
+    NegotiationDetails,
+    OneShotProfile,
+    OneShotState,
+    is_system_agent,
+)
 
 __all__ = ["OneShotAWI"]
 
 
 class OneShotAWI(AgentWorldInterface):
     """
     The agent world interface for the one-shot game.
@@ -43,14 +49,16 @@
           - *is_exogenous_forced*: Are exogenous contracts always forced or can the
             agent decide not to sign them.
           - *current_step*: Current simulation step (inherited from `negmas.situated.AgentWorldInterface` ).
           - *n_steps*: Number of simulation steps (inherited from `negmas.situated.AgentWorldInterface` ).
           - *relative_time*: fraction of the simulation completed (inherited from `negmas.situated.AgentWorldInterface`).
           - *state*: The full state of the agent ( `OneShotState` ).
           - *settings* The system settings (inherited from `negmas.situated.AgentWorldInterface` ).
+          - *quantity_range* The maximum quantity in all negotiation agendas (new in 0.6.1)
+          - *price_range* The maximum number of different prices in any negotiation agenda (new in 0.6.1)
 
         B. Agent Information:
           - *profile*: Gives the agent profile including its production cost, number
             of production lines, input product index, mean of its delivery
             penalties, mean of its disposal costs, standard deviation of its
             shortfall penalties and standard deviation of its disposal costs.
             See `OneShotProfile` for full description. This information is private
@@ -152,14 +160,28 @@
 
     # ================================================================
     # Static World Information (does not change during the simulation)
     # ================================================================
 
     # Market information
     # ------------------
+    @property
+    def max_n_lines(self) -> int:
+        """Maximum number of lines in the whole system"""
+        return self._world._max_n_lines
+
+    @property
+    def quantity_range(self) -> int:
+        """The maximum cardinality of the quantity issue in all negotiations"""
+        return self.max_n_lines
+
+    @property
+    def price_range(self) -> int:
+        """The maximum cardinality of the quantity issue in all negotiations"""
+        return 2
 
     @property
     def n_products(self) -> int:
         """Returns the number of products in the system"""
         return len(self._world.catalog_prices)
 
     @property
@@ -316,76 +338,31 @@
         """Returns a list of IDs for all the agent's consumers
         (agents that can consume at least one product it may produce).
 
         """
         return self.all_consumers[self.level + 1]
 
     @property
+    def my_partners(self) -> list[str]:
+        """Returns a list of IDs for all of the agent's partners starting with suppliers"""
+        return [
+            _
+            for _ in itertools.chain(self.my_suppliers, self.my_consumers)
+            if not self.is_system(_)
+        ]
+
+    @property
     def penalties_scale(self) -> Literal["trading", "catalog", "unit", "none"]:
         return self._world.penalties_scale
 
     # =========================================================
     # Dynamic Agent Information (changes during the simulation)
     # =========================================================
-    def default_encoded_state(
-        self, mechanism_states: dict[str, SAOState]
-    ) -> OneShotState:
-        all_agents = [_ for _ in self._world.agents.keys() if self.is_system(_)]
-
-        return OneShotState(
-            exogenous_input_quantity=self.current_exogenous_input_quantity,
-            exogenous_input_price=self.current_exogenous_input_price,
-            exogenous_output_quantity=self.current_exogenous_output_quantity,
-            exogenous_output_price=self.current_exogenous_output_price,
-            disposal_cost=self.current_disposal_cost,
-            shortfall_penalty=self.current_shortfall_penalty,
-            current_balance=self.current_balance,
-            total_sales=self.total_sales,
-            total_supplies=self.total_supplies,
-            n_products=self.n_products,
-            n_processes=self.n_processes,
-            n_competitors=self.n_competitors,
-            all_suppliers=self.all_suppliers,
-            all_consumers=self.all_consumers,
-            catalog_prices=self.catalog_prices.tolist(),
-            price_multiplier=self.price_multiplier,
-            is_exogenous_forced=self.is_exogenous_forced,
-            current_step=self.current_step,
-            n_steps=self.n_steps,
-            relative_simulation_time=self.relative_time,
-            profile=self.profile,
-            n_lines=self.n_lines,
-            is_first_level=self.is_first_level,
-            is_last_level=self.is_last_level,
-            is_middle_level=self.is_middle_level,
-            my_input_product=self.my_input_product,
-            my_output_product=self.my_output_product,
-            level=self.level,
-            my_suppliers=self.my_suppliers,
-            my_consumers=self.my_consumers,
-            penalties_scale=self.penalties_scale,
-            n_input_negotiations=self.n_input_negotiations,
-            n_output_negotiations=self.n_output_negotiations,
-            trading_prices=self.trading_prices.tolist(),
-            exogenous_contract_summary=self.exogenous_contract_summary,
-            current_input_outcome_space=self.current_input_outcome_space,
-            current_output_outcome_space=self.current_output_outcome_space,
-            current_negotiation_details=self.current_negotiation_details,
-            sales=self.sales,
-            supplies=self.supplies,
-            needed_sales=self.needed_sales,
-            needed_supplies=self.needed_supplies,
-            bankrupt_agents=[_ for _ in all_agents if self.is_bankrupt(_)],
-            reports_of_agents=dict(
-                zip(all_agents, [self.reports_of_agent(_) for _ in all_agents])
-            ),
-            running_negotiations=mechanism_states,
-        )
-
-    def state(self) -> Any:
+    @property
+    def state(self) -> OneShotState:
         all_agents = [_ for _ in self._world.agents.keys() if self.is_system(_)]
 
         return OneShotState(
             exogenous_input_quantity=self.current_exogenous_input_quantity,
             exogenous_input_price=self.current_exogenous_input_price,
             exogenous_output_quantity=self.current_exogenous_output_quantity,
             exogenous_output_price=self.current_exogenous_output_price,
@@ -395,14 +372,15 @@
             total_sales=self.total_sales,
             total_supplies=self.total_supplies,
             n_products=self.n_products,
             n_processes=self.n_processes,
             n_competitors=self.n_competitors,
             all_suppliers=self.all_suppliers,
             all_consumers=self.all_consumers,
+            my_partners=self.my_partners,
             catalog_prices=self.catalog_prices.tolist(),
             price_multiplier=self.price_multiplier,
             is_exogenous_forced=self.is_exogenous_forced,
             current_step=self.current_step,
             n_steps=self.n_steps,
             relative_simulation_time=self.relative_time,
             profile=self.profile,
@@ -427,15 +405,15 @@
             supplies=self.supplies,
             needed_sales=self.needed_sales,
             needed_supplies=self.needed_supplies,
             bankrupt_agents=[_ for _ in all_agents if self.is_bankrupt(_)],
             reports_of_agents=dict(
                 zip(all_agents, [self.reports_of_agent(_) for _ in all_agents])
             ),
-            running_negotiations=dict(),
+            # running_negotiations=dict(),
         )
 
     @property
     def current_balance(self):
         return self._world.current_balance(self.agent.id)
 
     @property
```

### Comparing `scml-0.6.0/src/scml/oneshot/common.py` & `scml-0.6.1/src/scml/oneshot/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,116 @@
+import sys
 from dataclasses import dataclass
 from typing import Literal
 
 from attr import define
 from negmas import SAONMI
 from negmas.common import define
 from negmas.outcomes import DiscreteCartesianOutcomeSpace
 from negmas.sao.common import SAOState
 
-from ..scml2019.common import FinancialReport
-from ..scml2020.common import QUANTITY, TIME, UNIT_PRICE
-
 __all__ = [
     "QUANTITY",
     "UNIT_PRICE",
     "TIME",
     "OneShotState",
     "OneShotExogenousContract",
     "OneShotProfile",
+    "FinancialReport",
+    "is_system_agent",
+    "INFINITE_COST",
+    "SYSTEM_BUYER_ID",
+    "SYSTEM_SELLER_ID",
+    "is_system_agent",
 ]
 
 
+QUANTITY = 0
+"""Index of quantity in negotiation issues"""
+
+
+TIME = 1
+"""Index of time in negotiation issues"""
+
+
+UNIT_PRICE = 2
+"""Index of unit price in negotiation issues"""
+
+INFINITE_COST = sys.maxsize // 2
+"""A constant indicating an invalid cost for lines incapable of running some process"""
+
+SYSTEM_SELLER_ID = "SELLER"
+"""ID of the system seller agent"""
+
+SYSTEM_BUYER_ID = "BUYER"
+"""ID of the system buyer agent"""
+
+COMPENSATION_ID = "COMPENSATOR"
+"""ID of the takeover agent"""
+
+
+def is_system_agent(aid: str) -> bool:
+    """
+    Checks whether an agent is a system agent or not
+
+    Args:
+
+        aid: Agent ID
+
+    Returns:
+
+        True if the ID is for a system agent.
+    """
+    return (
+        aid.startswith(SYSTEM_SELLER_ID)
+        or aid.startswith(SYSTEM_BUYER_ID)
+        or aid.startswith(COMPENSATION_ID)
+    )
+
+
+@dataclass
+class FinancialReport:
+    """A report published periodically by the system showing the financial standing of an agent"""
+
+    __slots__ = [
+        "agent_id",
+        "step",
+        "cash",
+        "assets",
+        "breach_prob",
+        "breach_level",
+        "is_bankrupt",
+        "agent_name",
+    ]
+    agent_id: str
+    """Agent ID"""
+    step: int
+    """Simulation step at the beginning of which the report was published."""
+    cash: int
+    """Cash in the agent's wallet. Negative numbers indicate liabilities."""
+    assets: int
+    """Value of the products in the agent's inventory @ catalog prices. """
+    breach_prob: float
+    """Number of times the agent breached a contract over the total number of contracts it signed."""
+    breach_level: float
+    """Sum of the agent's breach levels so far divided by the number of contracts it signed."""
+    is_bankrupt: bool
+    """Whether the agent is already bankrupt (i.e. incapable of doing any more transactions)."""
+    agent_name: str
+    """Agent name for printing purposes"""
+
+    def __str__(self):
+        bankrupt = "BANKRUPT" if self.is_bankrupt else ""
+        return (
+            f"{self.agent_name} @ {self.step} {bankrupt}: Cash: {self.cash}, Assets: {self.assets}, "
+            f"breach_prob: {self.breach_prob}, breach_level: {self.breach_level} "
+            f"{'(BANKRUPT)' if self.is_bankrupt else ''}"
+        )
+
+
 @dataclass
 class OneShotExogenousContract:
     """Exogenous contract information"""
 
     __slots__ = [
         "quantity",
         "unit_price",
@@ -157,14 +244,16 @@
     """The output product from the factory controlled by the agent."""
     level: int
     """The production level which is numerically the same as the input product."""
     my_suppliers: list[str]
     """A list of IDs for all suppliers to the agent (i.e. agents that can sell the input product of the agent)."""
     my_consumers: list[str]
     """A list of IDs for all consumers to the agent (i.e. agents that can buy the output product of the agent)."""
+    my_partners: list[str]
+    """A list of IDs for all negotiation partners of the agent (in the order suppliers then consumers)."""
     penalties_scale: Literal["trading", "catalog", "unit", "none"]
     """The scale at which to calculate disposal cost/delivery penalties.
     "trading" and "catalog" mean trading and catalog prices. "unit" means the
     contract's unit price while "none" means that disposal cost/shortfall penalty are absolute."""
     n_input_negotiations: int
     """Number of negotiations with suppliers."""
     n_output_negotiations: int
@@ -187,9 +276,9 @@
     """Today's sales per customer so far."""
     supplies: dict[str, int]
     """Today's supplies per supplier so far."""
     needed_sales: int
     """Today's needed sales as of now (exogenous input - exogenous output - total sales so far)."""
     needed_supplies: int
     """Today's needed supplies  as of now (exogenous output - exogenous input - total supplies)."""
-    running_negotiations: dict[str, SAOState]
-    """Maps partner ID to the state of the running negotiation with it (if any)"""
+    # running_negotiations: dict[str, SAOState]
+    # """Maps partner ID to the state of the running negotiation with it (if any)"""
```

### Comparing `scml-0.6.0/src/scml/oneshot/helper.py` & `scml-0.6.1/src/scml/oneshot/helper.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/mixins.py` & `scml-0.6.1/src/scml/oneshot/mixins.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/sysagents.py` & `scml-0.6.1/src/scml/oneshot/sysagents.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,30 +36,38 @@
           the SCML2020OneShotAgent.
     """
 
     def make_ufun(self, add_exogenous: bool):
         return super().make_ufun(add_exogenous, in_adapter=False)
 
     def on_negotiation_failure(self, partners, annotation, mechanism, state):
-        return self._obj.on_negotiation_failure(partners, annotation, mechanism, state)
+        result = self._obj.on_negotiation_failure(
+            partners, annotation, mechanism, state
+        )
+        # for k in ("sell", "buy"):
+        #     self.awi._world._agent_negotiations[self._obj.id][k].pop(mechanism.id, None)
+        return result
 
     def on_negotiation_success(self, contract: Contract, mechanism):
         if contract.annotation["buyer"] == self.id:
             self.awi._register_supply(
                 contract.annotation["seller"], contract.agreement["quantity"]
             )
         elif contract.annotation["seller"] == self.id:
             self.awi._register_sale(
                 contract.annotation["buyer"], contract.agreement["quantity"]
             )
         else:
             raise ValueError(
                 f"{self.id} received a  contract for which it is not a buyer nor a seller: {contract=}"
             )
-        return self._obj.on_negotiation_success(contract, mechanism)
+        result = self._obj.on_negotiation_success(contract, mechanism)
+        # for k in ("sell", "buy"):
+        #     self.awi._world._agent_negotiations[self._obj.id][k].pop(mechanism.id, None)
+        return result
 
     def on_contract_executed(self, contract: Contract) -> None:
         pass
 
     def on_contract_breached(
         self, contract: Contract, breaches: List[Breach], resolution: Optional[Contract]
     ) -> None:
```

### Comparing `scml-0.6.0/src/scml/oneshot/ufun.py` & `scml-0.6.1/src/scml/oneshot/ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/oneshot/world.py` & `scml-0.6.1/src/scml/oneshot/world.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,33 +30,36 @@
     SAOResponse,
     TimeInAgreementMixin,
     World,
     make_issue,
 )
 from negmas.helpers import get_class, get_full_type_name, instantiate, unique_name
 from negmas.sao import ControlledSAONegotiator, SAOController, SAONegotiator
+from negmas.situated import NegotiationInfo
 
 from ..common import (
     distribute_quantities,
     integer_cut,
     intin,
     make_array,
     realin,
     strin,
 )
-from ..scml2020 import FinancialReport
-from ..scml2020.common import (
+from .adapter import OneShotSCML2020Adapter
+from .agent import OneShotAgent
+from .common import (
     INFINITE_COST,
     SYSTEM_BUYER_ID,
     SYSTEM_SELLER_ID,
+    FinancialReport,
+    NegotiationDetails,
+    OneShotExogenousContract,
+    OneShotProfile,
     is_system_agent,
 )
-from .adapter import OneShotSCML2020Adapter
-from .agent import OneShotAgent
-from .common import NegotiationDetails, OneShotExogenousContract, OneShotProfile
 from .sysagents import DefaultOneShotAdapter, _SystemAgent
 
 __all__ = [
     "SCML2020OneShotWorld",
     "SCML2021OneShotWorld",
     "SCML2022OneShotWorld",
     "SCML2023OneShotWorld",
@@ -735,17 +738,17 @@
         Returns:
 
             world configuration as a Dict[str, Any]. A world can be generated from this dict by calling SCML2020World(**d)
 
         Remarks:
 
             - There are two general ways to use this generator:
-                1. Pass `random_agent_types = True`, and pass `agent_types`, `agent_processes` to control placement of each
+                1. Pass `random_agent_types = False`, and pass `agent_types`, `agent_processes` to control placement of each
                    agent in each level of the production graph.
-                2. Pass `random_agent_types = False` and pass `agent_types`, `n_agents_per_process` to make the system randomly
+                2. Pass `random_agent_types = True` and pass `agent_types`, `n_agents_per_process` to make the system randomly
                    place the specified number of agents in each production level
             - Most parameters (i.e. `process_inputs` , `process_outputs` , `n_agents_per_process` , `costs` ) can
               take a single value, a tuple of two values, or a list of values.
               If it has a single value, it is repeated for all processes/factories as appropriate. If it is a
               tuple of two numbers $(i, j)$, each process will take a number sampled from a uniform distribution
               supported on $[i, j]$ inclusive. If it is a list of values, of the length `n_processes` , it is used as
               it is otherwise, it is used to sample values for each process.
@@ -1308,32 +1311,43 @@
             - Every step advances all negotiations one step.
             - Negotiators belonging to the given agents are never called as long as a corresponding
               action (response) is given in the agents dict.
             - The world MUST be created with `one_offer_per_step` passed as `True` (default is `False`).
         """
         from scml.oneshot.awi import OneShotAWI
 
-        actions = dict()
+        neg_actions = dict()
+        existing = {
+            _.mechanism.id
+            for _ in self._negotiations.values()
+            if _ is not None and _.mechanism is not None
+        }
         for agent, responses in actions.items():
             awi: OneShotAWI = self.agents[agent].awi  # type: ignore
             negotiations = awi.current_negotiation_details["buy"].copy()
             negotiations.update(awi.current_negotiation_details["sell"])
             for partner, neg in negotiations.items():
                 neg: NegotiationDetails
                 mynegs = [
                     _ for _ in neg.nmi.mechanism.negotiators if _.owner.id == agent
                 ]
-                assert len(mynegs) == 0
-                assert neg.nmi.mechanism.one_offer_per_step  # type: ignore
+                assert len(mynegs) == 1
+                assert neg.nmi.mechanism._one_offer_per_step  # type: ignore
                 response = responses.get(partner, None)
+                mid = neg.nmi.mechanism.id
+                if mid not in existing:
+                    continue
+                # assert (
+                #     mid in existing
+                # ), f"{mid} mechanism (with {partner}) does not exist for {agent}"
                 if response is not None:
-                    actions[neg.nmi.mechanism.id] = {mynegs[0]: response}
+                    neg_actions[mid] = {mynegs[0].id: response}
                 else:
                     warnings.warn(f"{agent=} has no response for partner {partner}")
-        return self.step(n_neg_steps=int(not init), actions=actions)
+        return self.step(n_neg_steps=int(not init), neg_actions=neg_actions)
 
     def simulation_step(self, stage):
         s = self.current_step
 
         if stage == 0:
             self._update_exogenous(s)
 
@@ -1864,15 +1878,15 @@
         quantity: int | tuple[int, int],
         unit_price: int | tuple[int, int],
         time: int | tuple[int, int],
         partner: str,
         negotiator: SAONegotiator,
         extra: dict[str, Any] | None = None,
         consumer_starts: bool = True,
-    ) -> bool:
+    ) -> NegotiationInfo:
         """
         Requests a negotiation
 
         Args:
 
             product: The product to negotiate about
             quantity: The minimum and maximum quantities. Passing a single value q is equivalent to passing (q,q)
@@ -1958,16 +1972,14 @@
             )
             self._agent_negotiations[buyer]["buy"][seller] = NegotiationDetails(
                 seller=seller,
                 buyer=buyer,
                 nmi=result.mechanism.nmi,  # type: ignore
                 product=product,
             )
-        # if result:
-        #     self._registered_negs.add(tuple(sorted([partner, agent_id])))
         return result
 
     def _make_issues(
         self, product
     ) -> tuple[tuple[int, int], tuple[int, int], tuple[int, int]]:
         """
         Creates the negotiation agendas
```

### Comparing `scml-0.6.0/src/scml/scml2019/__init__.py` & `scml-0.6.1/src/scml/scml2019/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/agent.py` & `scml-0.6.1/src/scml/scml2019/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/awi.py` & `scml-0.6.1/src/scml/scml2019/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/bank.py` & `scml-0.6.1/src/scml/scml2019/bank.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/common.py` & `scml-0.6.1/src/scml/scml2019/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/consumers.py` & `scml-0.6.1/src/scml/scml2019/consumers.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/factory_managers/builtins.py` & `scml-0.6.1/src/scml/scml2019/factory_managers/builtins.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/helpers.py` & `scml-0.6.1/src/scml/scml2019/helpers.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/insurance.py` & `scml-0.6.1/src/scml/scml2019/insurance.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/miners.py` & `scml-0.6.1/src/scml/scml2019/miners.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/schedulers.py` & `scml-0.6.1/src/scml/scml2019/schedulers.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/simulators.py` & `scml-0.6.1/src/scml/scml2019/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/utils.py` & `scml-0.6.1/src/scml/scml2019/utils.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/visualizers.py` & `scml-0.6.1/src/scml/scml2019/visualizers.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2019/world.py` & `scml-0.6.1/src/scml/scml2019/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/__init__.py` & `scml-0.6.1/src/scml/scml2020/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 The detailed description of this world simulation can be found here_.
 
 .. _here: http://www.yasserm.com/scml/scml2020.pdf
 
 """
 
+from .agent import *
+from .agents import *
+from .awi import *
 from .common import *
+from .components import *
 from .factory import *
-from .awi import *
 from .world import *
-from .agent import *
-from .components import *
-from .agents import *
-from . import utils
-from .utils import *
 
 
 def builtin_agent_types(as_str=False):
     """
     Returns all built-in agents.
 
     Args:
@@ -37,9 +35,8 @@
     common.__all__
     + agents.__all__
     + world.__all__
     + components.__all__
     + factory.__all__
     + awi.__all__
     + agent.__all__
-    + ["utils"]
 )
```

### Comparing `scml-0.6.0/src/scml/scml2020/agent.py` & `scml-0.6.1/src/scml/scml2020/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,15 @@
             is_last_level=self.is_last_level,
             is_middle_level=self.is_middle_level,
             my_input_product=self.my_input_product,
             my_output_product=self.my_output_product,
             level=self.level,
             my_suppliers=self.my_suppliers,
             my_consumers=self.my_consumers,
+            my_partners=self.my_partners,
             penalties_scale=self.penalties_scale,
             n_input_negotiations=self.n_input_negotiations,
             n_output_negotiations=self.n_output_negotiations,
             trading_prices=self.trading_prices.tolist(),
             exogenous_contract_summary=self.exogenous_contract_summary,
             current_input_outcome_space=self.current_input_outcome_space,
             current_output_outcome_space=self.current_output_outcome_space,
```

### Comparing `scml-0.6.0/src/scml/scml2020/agents/bcse.py` & `scml-0.6.1/src/scml/scml2020/agents/bcse.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/agents/decentralizing.py` & `scml-0.6.1/src/scml/scml2020/agents/decentralizing.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/agents/do_nothing.py` & `scml-0.6.1/src/scml/scml2020/agents/do_nothing.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     Contract,
     Issue,
     MechanismState,
     Negotiator,
     NegotiatorMechanismInterface,
 )
 
-from scml.scml2020 import Failure, SCML2020Agent
+from scml.scml2020.agent import SCML2020Agent
+from scml.scml2020.common import Failure
 
 __all__ = ["DoNothingAgent"]
 
 
 class DoNothingAgent(SCML2020Agent):
     """An agent that does nothing for the whole length of the simulation"""
```

### Comparing `scml-0.6.0/src/scml/scml2020/agents/indneg.py` & `scml-0.6.1/src/scml/scml2020/agents/indneg.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/agents/moving.py` & `scml-0.6.1/src/scml/scml2020/agents/moving.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/agents/random.py` & `scml-0.6.1/src/scml/scml2020/agents/random.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/agents/reactive.py` & `scml-0.6.1/src/scml/scml2020/agents/reactive.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/agents/satisficer.py` & `scml-0.6.1/src/scml/scml2020/agents/satisficer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     Negotiator,
     NegotiatorMechanismInterface,
     Outcome,
     ResponseType,
 )
 from negmas.sao import SAONMI, SAONegotiator, SAOState
 
-from scml.scml2020 import AWI, NO_COMMAND, QUANTITY, TIME, UNIT_PRICE, SCML2020Agent
+from scml.scml2020.agent import SCML2020Agent
+from scml.scml2020.awi import AWI
+from scml.scml2020.common import NO_COMMAND, QUANTITY, TIME, UNIT_PRICE
 
 __all__ = ["SatisficerAgent"]
 
 
 class ObedientNegotiator(SAONegotiator):
     """
     A negotiator that controls a single negotiation with a single partner.
```

### Comparing `scml-0.6.0/src/scml/scml2020/awi.py` & `scml-0.6.1/src/scml/scml2020/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/common.py` & `scml-0.6.1/src/scml/scml2020/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/components/negotiation.py` & `scml-0.6.1/src/scml/scml2020/components/negotiation.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     SAONegotiator,
     UtilityFunction,
     make_issue,
 )
 from negmas.helpers import get_class, instantiate
 from negmas.outcomes.issue_ops import enumerate_issues
 
-from scml.scml2020 import AWI
+from scml.scml2020.awi import AWI
 from scml.scml2020.common import TIME
 from scml.scml2020.components.prediction import MeanERPStrategy
 from scml.scml2020.services.controllers import StepController, SyncController
 
 __all__ = [
     "NegotiationManager",
     "StepNegotiationManager",
@@ -451,15 +451,14 @@
     def respond_to_negotiation_request(
         self,
         initiator: str,
         issues: List[Issue],
         annotation: Dict[str, Any],
         mechanism: NegotiatorMechanismInterface,
     ) -> Optional[Negotiator]:
-
         # find negotiation parameters
         is_seller = annotation["seller"] == self.id
         tmin, tmax = issues[TIME].min_value, issues[TIME].max_value + 1
         # find the time-step for which this negotiation should be added
         step = max(0, tmin - 1) if is_seller else min(self.awi.n_steps - 1, tmax + 1)
         # find the corresponding controller.
         controller_info: ControllerInfo
```

### Comparing `scml-0.6.0/src/scml/scml2020/components/prediction.py` & `scml-0.6.1/src/scml/scml2020/components/prediction.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/components/production.py` & `scml-0.6.1/src/scml/scml2020/components/production.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/components/signing.py` & `scml-0.6.1/src/scml/scml2020/components/signing.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/components/simulation.py` & `scml-0.6.1/src/scml/scml2020/components/simulation.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/components/trading.py` & `scml-0.6.1/src/scml/scml2020/components/trading.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/factory.py` & `scml-0.6.1/src/scml/scml2020/factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/services/controllers.py` & `scml-0.6.1/src/scml/scml2020/services/controllers.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/services/simulators.py` & `scml-0.6.1/src/scml/scml2020/services/simulators.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import defaultdict
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
-from scml.scml2020 import ANY_LINE, ANY_STEP, NO_COMMAND, FactoryProfile
+from scml.scml2020.common import ANY_LINE, ANY_STEP, NO_COMMAND, FactoryProfile
 
 __all__ = ["FactorySimulator", "transaction", "temporary_transaction"]
 
 
 @dataclass
 class _Bookmark:
     id: int
```

### Comparing `scml-0.6.0/src/scml/scml2020/utils.py` & `scml-0.6.1/src/scml/utils.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/scml2020/world.py` & `scml-0.6.1/src/scml/scml2020/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/vendor/quick/LICENSE` & `scml-0.6.1/src/scml/vendor/quick/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/vendor/quick/README.md` & `scml-0.6.1/src/scml/vendor/quick/README.md`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml/vendor/quick/quick.py` & `scml-0.6.1/src/scml/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/src/scml.egg-info/PKG-INFO` & `scml-0.6.1/src/scml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.6.0
+Version: 0.6.1
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: gui
-Provides-Extra: rl
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
@@ -85,14 +84,23 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.6.1 (2023.7.9)
+----------------
+
+* Moving scml.scml2020.utils to scml.utils (to avoid a circular import in rl/factory)
+* This is an initial effort to have RL work for scml. Currently we are disabling the extra checks on observation and
+  world construction because they lead to failures. This needs to be rectified later.
+* Added the concept of a WorldFactory to generate worlds with predefined characteristics from the point of view of the learning agent.
+* Now environments, action managers, and observation managers all receive WorldFactory objects and automatically check for compatibility.
+
 0.6.0 (2023.7.9)
 ----------------
 
 * Upgrading to be compatible with NegMAS 0.10.0
 * Adding step_with() to oneshot allowing for single counter-offer set stepping of the simulation (to be used to expose the simulation as RL and MARL environments later).
 * Adding current_negotiation_details to OneShotAWI to get details of running negotiation
 * Adding managed sales, supplies, total_sales, total_supplies, needed_sales, and needed_supplies to the OneShotAWI
```

### Comparing `scml-0.6.0/src/scml.egg-info/SOURCES.txt` & `scml-0.6.1/src/scml.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 tox.ini
 src/scml/__init__.py
 src/scml/__main__.py
 src/scml/cli.py
 src/scml/cliadv.py
 src/scml/common.py
 src/scml/experiment.py
+src/scml/utils.py
 src/scml.egg-info/PKG-INFO
 src/scml.egg-info/SOURCES.txt
 src/scml.egg-info/dependency_links.txt
 src/scml.egg-info/entry_points.txt
 src/scml.egg-info/not-zip-safe
 src/scml.egg-info/requires.txt
 src/scml.egg-info/top_level.txt
@@ -37,14 +38,21 @@
 src/scml/oneshot/ufun.py
 src/scml/oneshot/world.py
 src/scml/oneshot/agents/__init__.py
 src/scml/oneshot/agents/aspiration.py
 src/scml/oneshot/agents/greedy.py
 src/scml/oneshot/agents/nothing.py
 src/scml/oneshot/agents/random.py
+src/scml/oneshot/rl/__init__.py
+src/scml/oneshot/rl/action.py
+src/scml/oneshot/rl/agent.py
+src/scml/oneshot/rl/common.py
+src/scml/oneshot/rl/env.py
+src/scml/oneshot/rl/factory.py
+src/scml/oneshot/rl/observation.py
 src/scml/scml2019/__init__.py
 src/scml/scml2019/agent.py
 src/scml/scml2019/awi.py
 src/scml/scml2019/bank.py
 src/scml/scml2019/common.py
 src/scml/scml2019/consumers.py
 src/scml/scml2019/helpers.py
@@ -58,15 +66,14 @@
 src/scml/scml2019/factory_managers/__init__.py
 src/scml/scml2019/factory_managers/builtins.py
 src/scml/scml2020/__init__.py
 src/scml/scml2020/agent.py
 src/scml/scml2020/awi.py
 src/scml/scml2020/common.py
 src/scml/scml2020/factory.py
-src/scml/scml2020/utils.py
 src/scml/scml2020/world.py
 src/scml/scml2020/agents/__init__.py
 src/scml/scml2020/agents/bcse.py
 src/scml/scml2020/agents/decentralizing.py
 src/scml/scml2020/agents/do_nothing.py
 src/scml/scml2020/agents/indneg.py
 src/scml/scml2020/agents/moving.py
@@ -94,20 +101,27 @@
 tests/test_can_run_tutorial2.py
 tests/test_cli.py
 tests/test_factory2019.py
 tests/test_jupyter.py
 tests/test_oneshot_do_nothing.py
 tests/test_oneshot_sync.py
 tests/test_oneshot_ufun.py
+tests/test_rl.py
 tests/test_scheduler2019.py
 tests/test_scml2019.py
 tests/test_scml2019factory.py
 tests/test_scml2019tournaments.py
 tests/test_scml2020.py
 tests/test_scml2020factory.py
 tests/test_scml2020tournaments.py
 tests/test_scml2021.py
 tests/test_scml2021oneshot.py
 tests/test_scml2021tournaments.py
 tests/test_scml2023.py
 tests/test_scml2023oneshot.py
-tests/test_sync_jackson.py
+tests/test_sync_jackson.py
+tests/tmp_notebooks/tutorials/01.run_scml2020.ipynb
+tests/tmp_notebooks/tutorials/02.develop_agent_scml2020_oneshot.ipynb
+tests/tmp_notebooks/tutorials/03.develop_agent_scml2020.ipynb
+tests/tmp_notebooks/tutorials/04.experiments.ipynb
+tests/tmp_notebooks/tutorials/05.logs_and_stats.ipynb
+tests/tmp_notebooks/tutorials/06.ideas.ipynb
```

### Comparing `scml-0.6.0/tests/switches.py` & `scml-0.6.1/tests/switches.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_can_run_tutorial2.py` & `scml-0.6.1/tests/test_can_run_tutorial2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from negmas.genius.gnegotiators import NiceTitForTat
 from negmas.outcomes import Outcome
 from negmas.preferences import LinearAdditiveUtilityFunction, LinearUtilityFunction
 from negmas.preferences.value_fun import AffineFun, IdentityFun
 
 from scml.oneshot import *
 from scml.oneshot import OneShotIndNegotiatorsAgent
-from scml.scml2020 import is_system_agent
+from scml.scml2020.common import is_system_agent
 
 from .switches import *
 
 
 def try_agent(agent_type, n_processes=2):
     """Runs an agent in a world simulation against a randomly behaving agent"""
     return try_agents([RandomOneShotAgent, agent_type], n_processes)
```

### Comparing `scml-0.6.0/tests/test_factory2019.py` & `scml-0.6.1/tests/test_factory2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_jupyter.py` & `scml-0.6.1/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_oneshot_do_nothing.py` & `scml-0.6.1/tests/test_oneshot_do_nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_oneshot_sync.py` & `scml-0.6.1/tests/test_oneshot_sync.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_oneshot_ufun.py` & `scml-0.6.1/tests/test_oneshot_ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_scheduler2019.py` & `scml-0.6.1/tests/test_scheduler2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_scml2019.py` & `scml-0.6.1/tests/test_scml2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_scml2019factory.py` & `scml-0.6.1/tests/test_scml2019factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_scml2019tournaments.py` & `scml-0.6.1/tests/test_scml2019tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_scml2020.py` & `scml-0.6.1/tests/test_scml2020.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tests/test_scml2020factory.py` & `scml-0.6.1/tests/test_scml2020factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import hypothesis.strategies as st
 import numpy as np
 import pytest
 from hypothesis import example, given
 from hypothesis.stateful import Bundle, RuleBasedStateMachine, rule
 
-from scml.scml2020 import NO_COMMAND, Factory, FactoryProfile, FactoryState
+from scml.scml2020.common import NO_COMMAND, FactoryProfile, FactoryState
 from scml.scml2020.components.simulation import FactorySimulator
+from scml.scml2020.factory import Factory
 
 PROCESSES = 5
 LINES = 10
 STEPS = 50
 INITIAL = 1000
```

### Comparing `scml-0.6.0/tests/test_scml2020tournaments.py` & `scml-0.6.1/tests/test_scml2020tournaments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import pytest
 
 from scml.scml2020.agents import DoNothingAgent
-from scml.scml2020.utils import (
+from scml.utils import (
     anac2020_collusion,
     anac2020_std,
     anac2021_collusion,
     anac2021_std,
 )
 from tests.switches import (
     SCML_RUN2020,
```

### Comparing `scml-0.6.0/tests/test_scml2021.py` & `scml-0.6.1/tests/test_scml2021.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     IndependentNegotiationsAgent,
     RandomAgent,
     SatisficerAgent,
     SCML2021World,
     is_system_agent,
 )
 from scml.scml2020.agents.decentralizing import DecentralizingAgent
-from scml.scml2020.utils import anac2021_collusion
+from scml.utils import anac2021_collusion
 
 from .switches import SCML_ON_GITHUB, SCML_RUN2021_STD
 
 random.seed(0)
 
 COMPACT = True
 NOLOGS = True
```

### Comparing `scml-0.6.0/tests/test_scml2021oneshot.py` & `scml-0.6.1/tests/test_scml2021oneshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 from scml.oneshot.agent import (
     OneShotAgent,
     OneShotIndNegotiatorsAgent,
     OneShotSyncAgent,
 )
 from scml.oneshot.agents import GreedySyncAgent, RandomOneShotAgent
 from scml.oneshot.awi import OneShotAWI
-from scml.oneshot.common import QUANTITY, TIME, UNIT_PRICE
+from scml.oneshot.common import QUANTITY, TIME, UNIT_PRICE, is_system_agent
 from scml.oneshot.ufun import OneShotUFun
-from scml.scml2020 import is_system_agent
 
 from .switches import SCML_ON_GITHUB
 
 random.seed(0)
 
 COMPACT = True
 NOLOGS = True
```

### Comparing `scml-0.6.0/tests/test_scml2021tournaments.py` & `scml-0.6.1/tests/test_scml2021tournaments.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import hypothesis.strategies as st
 import numpy as np
 import pytest
 from hypothesis import given
 
 from scml.oneshot.agents import RandomOneShotAgent
-from scml.scml2020.utils import anac2021_oneshot, truncated_mean
+from scml.utils import anac2021_oneshot, truncated_mean
 
 from .switches import SCML_RUN2021_ONESHOT, SCML_RUN_STD_TOURNAMENTS
 
 
 class MyAgent0(RandomOneShotAgent):
     pass
```

### Comparing `scml-0.6.0/tests/test_scml2023.py` & `scml-0.6.1/tests/test_scml2023.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pprint import pprint
 
 import matplotlib.pyplot as plt
 from negmas import ResponseType
 from negmas.sao import SAOResponse
 
 from scml.oneshot import *
-from scml.scml2020 import is_system_agent
+from scml.scml2020.common import is_system_agent
 
 
 def try_agent(agent_type, n_processes=2, **kwargs):
     """Runs an agent in a world simulation against a randomly behaving agent"""
     return try_agents([RandomOneShotAgent, agent_type], n_processes, **kwargs)
```

### Comparing `scml-0.6.0/tests/test_scml2023oneshot.py` & `scml-0.6.1/tests/test_scml2023oneshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from scml.oneshot.agents import (
     GreedyOneShotAgent,
     GreedySingleAgreementAgent,
     GreedySyncAgent,
     RandomOneShotAgent,
 )
 from scml.oneshot.world import SCML2023OneShotWorld
-from scml.scml2020.utils import (
+from scml.utils import (
     anac2023_oneshot_world_generator,
     anac_assigner_oneshot,
     anac_config_generator_oneshot,
 )
 
 
 def test_equal_exogenous_supply():
@@ -112,26 +112,31 @@
     )
     agents = list(random.choices(list(world.agents.values()), k=1))
     world.step_with(actions=dict(), init=True)
 
     def make_actions():
         actions = dict()
         for agent in agents:
-            responses = dict()
+            negotiator, responses = None, dict()
             for t in ["buy", "sell"]:
                 for partner, neg in agent.awi.current_negotiation_details[t].items():  # type: ignore
                     assert agent.id in (neg.buyer, neg.seller)
                     partner2 = neg.buyer if agent.id == neg.seller else neg.seller
                     assert partner2 == partner
                     negotiator = [
                         _.id
                         for _ in neg.nmi.mechanism.negotiators
                         if _.owner.id == agent.id
                     ][0]
-                    responses[partner] = {
+                    partner = [
+                        _.id
+                        for _ in neg.nmi.mechanism.negotiators
+                        if _.owner.id != agent.id
+                    ][0]
+                    responses[neg.nmi.mechanism.id] = {
                         negotiator: SAOResponse(
                             ResponseType.REJECT_OFFER, neg.nmi.random_outcome()
                         )
                     }
 
             actions[agent.id] = responses
         return actions
```

### Comparing `scml-0.6.0/tests/test_sync_jackson.py` & `scml-0.6.1/tests/test_sync_jackson.py`

 * *Files identical despite different names*

### Comparing `scml-0.6.0/tox.ini` & `scml-0.6.1/tox.ini`

 * *Files identical despite different names*

