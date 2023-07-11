# Comparing `tmp/aleph-sdk-python-0.7.0.tar.gz` & `tmp/aleph-sdk-python-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-sdk-python-0.7.0.tar", last modified: Tue Jul 11 15:23:34 2023, max compression
+gzip compressed data, was "aleph-sdk-python-0.7.0b1.tar", last modified: Tue May 16 13:19:44 2023, max compression
```

## Comparing `aleph-sdk-python-0.7.0.tar` & `aleph-sdk-python-0.7.0b1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.990914 aleph-sdk-python-0.7.0/
--rw-r--r--   0 user      (1000) user      (1000)      592 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/.coveragerc
--rw-r--r--   0 user      (1000) user      (1000)       54 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/.dockerignore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.985914 aleph-sdk-python-0.7.0/.github/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.986914 aleph-sdk-python-0.7.0/.github/workflows/
--rw-r--r--   0 user      (1000) user      (1000)     1657 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/.github/workflows/build-wheels.yml
--rw-r--r--   0 user      (1000) user      (1000)     1035 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/.github/workflows/code-quality.yml
--rw-r--r--   0 user      (1000) user      (1000)     1597 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0/.github/workflows/pytest-docker.yml
--rw-r--r--   0 user      (1000) user      (1000)      537 2023-03-02 13:32:56.000000 aleph-sdk-python-0.7.0/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      159 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/AUTHORS.rst
--rw-r--r--   0 user      (1000) user      (1000)       82 2023-01-25 17:30:47.000000 aleph-sdk-python-0.7.0/CHANGELOG.rst
--rw-r--r--   0 user      (1000) user      (1000)     1080 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)     1905 2023-07-11 15:23:34.990914 aleph-sdk-python-0.7.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1190 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.987914 aleph-sdk-python-0.7.0/docker/
--rw-r--r--   0 user      (1000) user      (1000)     1152 2023-07-11 11:31:36.000000 aleph-sdk-python-0.7.0/docker/python-3.10.dockerfile
--rw-r--r--   0 user      (1000) user      (1000)     1140 2023-07-11 11:31:36.000000 aleph-sdk-python-0.7.0/docker/python-3.11.dockerfile
--rw-r--r--   0 user      (1000) user      (1000)     1151 2023-07-11 11:31:36.000000 aleph-sdk-python-0.7.0/docker/python-3.9.dockerfile
--rw-r--r--   0 user      (1000) user      (1000)     1236 2023-07-11 11:31:36.000000 aleph-sdk-python-0.7.0/docker/ubuntu-20.04.dockerfile
--rw-r--r--   0 user      (1000) user      (1000)     1236 2023-07-11 11:31:36.000000 aleph-sdk-python-0.7.0/docker/ubuntu-22.04.dockerfile
--rw-r--r--   0 user      (1000) user      (1000)      888 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/docker/with-ipfs.dockerfile
--rwxr-xr-x   0 user      (1000) user      (1000)      346 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docker/with-ipfs.entrypoint.sh
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.987914 aleph-sdk-python-0.7.0/docs/
--rw-r--r--   0 user      (1000) user      (1000)     7622 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/docs/Makefile
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.987914 aleph-sdk-python-0.7.0/docs/_static/
--rw-r--r--   0 user      (1000) user      (1000)       18 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docs/_static/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)     2774 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docs/_static/logo.svg
--rw-r--r--   0 user      (1000) user      (1000)       41 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docs/authors.rst
--rw-r--r--   0 user      (1000) user      (1000)       43 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docs/changelog.rst
--rw-r--r--   0 user      (1000) user      (1000)     9768 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/docs/conf.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.987914 aleph-sdk-python-0.7.0/docs/content/
--rw-r--r--   0 user      (1000) user      (1000)     3241 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0/docs/content/account.rst
--rw-r--r--   0 user      (1000) user      (1000)     2347 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0/docs/content/aggregates.rst
--rw-r--r--   0 user      (1000) user      (1000)     1543 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0/docs/content/async_notes.rst
--rw-r--r--   0 user      (1000) user      (1000)     1924 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0/docs/content/cli.rst
--rw-r--r--   0 user      (1000) user      (1000)     2604 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docs/content/introduction.rst
--rw-r--r--   0 user      (1000) user      (1000)     1402 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0/docs/content/posts.rst
--rw-r--r--   0 user      (1000) user      (1000)     1159 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0/docs/content/programs.rst
--rw-r--r--   0 user      (1000) user      (1000)     1482 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/docs/index.rst
--rw-r--r--   0 user      (1000) user      (1000)       67 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/docs/license.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.987914 aleph-sdk-python-0.7.0/examples/
--rw-r--r--   0 user      (1000) user      (1000)     2004 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/examples/httpgateway.py
--rw-r--r--   0 user      (1000) user      (1000)     1911 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/examples/metrics.py
--rw-r--r--   0 user      (1000) user      (1000)     4075 2023-07-10 22:15:26.000000 aleph-sdk-python-0.7.0/examples/mqtt.py
--rw-r--r--   0 user      (1000) user      (1000)     3391 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/examples/store.py
--rw-r--r--   0 user      (1000) user      (1000)     2467 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/mypy.ini
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.988914 aleph-sdk-python-0.7.0/scripts/
--rw-r--r--   0 user      (1000) user      (1000)      333 2023-07-11 12:21:24.000000 aleph-sdk-python-0.7.0/scripts/build-and-shell.sh
--rw-r--r--   0 user      (1000) user      (1000)      468 2023-07-11 12:21:24.000000 aleph-sdk-python-0.7.0/scripts/build-and-test.sh
--rw-r--r--   0 user      (1000) user      (1000)      419 2023-07-11 12:21:24.000000 aleph-sdk-python-0.7.0/scripts/build-to-publish.sh
--rw-r--r--   0 user      (1000) user      (1000)     2143 2023-07-11 15:23:34.991914 aleph-sdk-python-0.7.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      572 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.986914 aleph-sdk-python-0.7.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.988914 aleph-sdk-python-0.7.0/src/aleph/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/src/aleph/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.988914 aleph-sdk-python-0.7.0/src/aleph/sdk/
--rw-r--r--   0 user      (1000) user      (1000)      472 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2177 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/account.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.988914 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     4275 2023-07-11 11:11:57.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/common.py
--rw-r--r--   0 user      (1000) user      (1000)     2583 2023-07-10 23:09:39.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/cosmos.py
--rw-r--r--   0 user      (1000) user      (1000)     2672 2023-05-22 09:23:22.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/ethereum.py
--rw-r--r--   0 user      (1000) user      (1000)     9356 2023-05-16 10:29:19.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/nuls1.py
--rw-r--r--   0 user      (1000) user      (1000)     1958 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/nuls2.py
--rw-r--r--   0 user      (1000) user      (1000)     2351 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/remote.py
--rw-r--r--   0 user      (1000) user      (1000)     2849 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/sol.py
--rw-r--r--   0 user      (1000) user      (1000)     1474 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/substrate.py
--rw-r--r--   0 user      (1000) user      (1000)     2345 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/chains/tezos.py
--rw-r--r--   0 user      (1000) user      (1000)    51059 2023-07-11 11:11:57.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/client.py
--rw-r--r--   0 user      (1000) user      (1000)     1794 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/conf.py
--rw-r--r--   0 user      (1000) user      (1000)      753 2023-05-16 10:28:27.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)      354 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/models.py
--rw-r--r--   0 user      (1000) user      (1000)      893 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/types.py
--rw-r--r--   0 user      (1000) user      (1000)     3148 2023-07-11 11:11:57.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.989914 aleph-sdk-python-0.7.0/src/aleph/sdk/vm/
--rw-r--r--   0 user      (1000) user      (1000)       70 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/vm/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2645 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/vm/app.py
--rw-r--r--   0 user      (1000) user      (1000)     4581 2023-07-10 22:26:19.000000 aleph-sdk-python-0.7.0/src/aleph/sdk/vm/cache.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.989914 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1905 2023-07-11 15:23:34.000000 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2587 2023-07-11 15:23:34.000000 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-11 15:23:34.000000 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-25 18:58:13.000000 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/not-zip-safe
--rw-r--r--   0 user      (1000) user      (1000)      712 2023-07-11 15:23:34.000000 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        6 2023-07-11 15:23:34.000000 aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.989914 aleph-sdk-python-0.7.0/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/tests/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.989914 aleph-sdk-python-0.7.0/tests/integration/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/tests/integration/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      118 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/tests/integration/config.py
--rw-r--r--   0 user      (1000) user      (1000)      579 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/integration/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)     2610 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/integration/itest_aggregates.py
--rw-r--r--   0 user      (1000) user      (1000)     4399 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/integration/itest_forget.py
--rw-r--r--   0 user      (1000) user      (1000)     1958 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/integration/itest_posts.py
--rw-r--r--   0 user      (1000) user      (1000)       35 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/tests/integration/pytest.ini
--rw-r--r--   0 user      (1000) user      (1000)      607 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/integration/toolkit.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.990914 aleph-sdk-python-0.7.0/tests/unit/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/tests/unit/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1157 2023-07-10 23:09:39.000000 aleph-sdk-python-0.7.0/tests/unit/conftest.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-11 15:23:34.990914 aleph-sdk-python-0.7.0/tests/unit/test_app/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0/tests/unit/test_app/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      291 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_app/main.py
--rw-r--r--   0 user      (1000) user      (1000)     4891 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_asynchronous.py
--rw-r--r--   0 user      (1000) user      (1000)     2564 2023-05-16 12:21:38.000000 aleph-sdk-python-0.7.0/tests/unit/test_asynchronous_get.py
--rw-r--r--   0 user      (1000) user      (1000)     3632 2023-05-22 09:23:22.000000 aleph-sdk-python-0.7.0/tests/unit/test_chain_ethereum.py
--rw-r--r--   0 user      (1000) user      (1000)     1389 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_chain_nuls1.py
--rw-r--r--   0 user      (1000) user      (1000)     4580 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_chain_nuls1_compat.py
--rw-r--r--   0 user      (1000) user      (1000)     3580 2023-05-22 09:23:22.000000 aleph-sdk-python-0.7.0/tests/unit/test_chain_solana.py
--rw-r--r--   0 user      (1000) user      (1000)     2167 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0/tests/unit/test_chain_tezos.py
--rw-r--r--   0 user      (1000) user      (1000)      608 2023-07-11 11:11:57.000000 aleph-sdk-python-0.7.0/tests/unit/test_chains.py
--rw-r--r--   0 user      (1000) user      (1000)       85 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_init.py
--rw-r--r--   0 user      (1000) user      (1000)     2164 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_remote_account.py
--rw-r--r--   0 user      (1000) user      (1000)      522 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_synchronous_get.py
--rw-r--r--   0 user      (1000) user      (1000)      915 2023-07-11 11:11:57.000000 aleph-sdk-python-0.7.0/tests/unit/test_utils.py
--rw-r--r--   0 user      (1000) user      (1000)      765 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_vm_app.py
--rw-r--r--   0 user      (1000) user      (1000)     1034 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0/tests/unit/test_vm_cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/
+-rw-r--r--   0 user      (1000) user      (1000)      592 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/.coveragerc
+-rw-r--r--   0 user      (1000) user      (1000)       54 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/.dockerignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.748700 aleph-sdk-python-0.7.0b1/.github/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.749700 aleph-sdk-python-0.7.0b1/.github/workflows/
+-rw-r--r--   0 user      (1000) user      (1000)     1657 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1035 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/.github/workflows/code-quality.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1597 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/.github/workflows/pytest-docker.yml
+-rw-r--r--   0 user      (1000) user      (1000)      537 2023-03-02 13:32:56.000000 aleph-sdk-python-0.7.0b1/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      159 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/AUTHORS.rst
+-rw-r--r--   0 user      (1000) user      (1000)       82 2023-01-25 17:30:47.000000 aleph-sdk-python-0.7.0b1/CHANGELOG.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1080 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1907 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1190 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.750700 aleph-sdk-python-0.7.0b1/docker/
+-rw-r--r--   0 user      (1000) user      (1000)     1152 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/python-3.10.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1140 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/docker/python-3.11.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1151 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/python-3.9.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1236 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/ubuntu-20.04.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1236 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/ubuntu-22.04.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)      888 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/with-ipfs.dockerfile
+-rwxr-xr-x   0 user      (1000) user      (1000)      346 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docker/with-ipfs.entrypoint.sh
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.750700 aleph-sdk-python-0.7.0b1/docs/
+-rw-r--r--   0 user      (1000) user      (1000)     7622 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docs/Makefile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.750700 aleph-sdk-python-0.7.0b1/docs/_static/
+-rw-r--r--   0 user      (1000) user      (1000)       18 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/_static/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)     2774 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/_static/logo.svg
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/authors.rst
+-rw-r--r--   0 user      (1000) user      (1000)       43 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/changelog.rst
+-rw-r--r--   0 user      (1000) user      (1000)     9768 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docs/conf.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/docs/content/
+-rw-r--r--   0 user      (1000) user      (1000)     3241 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/account.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2347 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/aggregates.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1543 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/async_notes.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1924 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/cli.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2604 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/content/introduction.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1402 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/posts.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1159 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/programs.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1482 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docs/index.rst
+-rw-r--r--   0 user      (1000) user      (1000)       67 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/license.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/examples/
+-rw-r--r--   0 user      (1000) user      (1000)     2004 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/httpgateway.py
+-rw-r--r--   0 user      (1000) user      (1000)     1911 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/metrics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4075 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/mqtt.py
+-rw-r--r--   0 user      (1000) user      (1000)     3391 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/store.py
+-rw-r--r--   0 user      (1000) user      (1000)     2467 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/mypy.ini
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/scripts/
+-rw-r--r--   0 user      (1000) user      (1000)      322 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/scripts/build-and-shell.sh
+-rw-r--r--   0 user      (1000) user      (1000)      457 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/scripts/build-and-test.sh
+-rw-r--r--   0 user      (1000) user      (1000)      419 2023-05-16 13:01:37.000000 aleph-sdk-python-0.7.0b1/scripts/build-to-publish.sh
+-rw-r--r--   0 user      (1000) user      (1000)     2130 2023-05-16 13:19:44.759700 aleph-sdk-python-0.7.0b1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      572 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.749700 aleph-sdk-python-0.7.0b1/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/src/aleph/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/src/aleph/sdk/
+-rw-r--r--   0 user      (1000) user      (1000)      472 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2177 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/account.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3757 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/common.py
+-rw-r--r--   0 user      (1000) user      (1000)     2583 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/cosmos.py
+-rw-r--r--   0 user      (1000) user      (1000)     2653 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/ethereum.py
+-rw-r--r--   0 user      (1000) user      (1000)     9356 2023-05-16 10:29:19.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls1.py
+-rw-r--r--   0 user      (1000) user      (1000)     1958 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2351 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/remote.py
+-rw-r--r--   0 user      (1000) user      (1000)     2849 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/sol.py
+-rw-r--r--   0 user      (1000) user      (1000)     1474 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/substrate.py
+-rw-r--r--   0 user      (1000) user      (1000)     2345 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/tezos.py
+-rw-r--r--   0 user      (1000) user      (1000)    51023 2023-05-16 12:59:50.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/client.py
+-rw-r--r--   0 user      (1000) user      (1000)     1794 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/conf.py
+-rw-r--r--   0 user      (1000) user      (1000)      753 2023-05-16 10:28:27.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)      354 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/models.py
+-rw-r--r--   0 user      (1000) user      (1000)      893 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/types.py
+-rw-r--r--   0 user      (1000) user      (1000)     2680 2023-05-16 12:59:50.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/
+-rw-r--r--   0 user      (1000) user      (1000)       70 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2645 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/app.py
+-rw-r--r--   0 user      (1000) user      (1000)     4093 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1907 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2587 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-25 18:58:13.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      699 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        6 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/tests/integration/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/integration/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      118 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/integration/config.py
+-rw-r--r--   0 user      (1000) user      (1000)      579 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)     2610 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/itest_aggregates.py
+-rw-r--r--   0 user      (1000) user      (1000)     4399 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/itest_forget.py
+-rw-r--r--   0 user      (1000) user      (1000)     1958 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/itest_posts.py
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/integration/pytest.ini
+-rw-r--r--   0 user      (1000) user      (1000)      607 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/toolkit.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/tests/unit/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/unit/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1157 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/conftest.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/tests/unit/test_app/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_app/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      291 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_app/main.py
+-rw-r--r--   0 user      (1000) user      (1000)     4891 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous.py
+-rw-r--r--   0 user      (1000) user      (1000)     2564 2023-05-16 12:21:38.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous_get.py
+-rw-r--r--   0 user      (1000) user      (1000)     2582 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_ethereum.py
+-rw-r--r--   0 user      (1000) user      (1000)     1389 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1.py
+-rw-r--r--   0 user      (1000) user      (1000)     4580 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1_compat.py
+-rw-r--r--   0 user      (1000) user      (1000)     3286 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_solana.py
+-rw-r--r--   0 user      (1000) user      (1000)     2167 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_tezos.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chains.py
+-rw-r--r--   0 user      (1000) user      (1000)       85 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_init.py
+-rw-r--r--   0 user      (1000) user      (1000)     2164 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_remote_account.py
+-rw-r--r--   0 user      (1000) user      (1000)      522 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_synchronous_get.py
+-rw-r--r--   0 user      (1000) user      (1000)      596 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)      765 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_vm_app.py
+-rw-r--r--   0 user      (1000) user      (1000)     1034 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_vm_cache.py
```

### Comparing `aleph-sdk-python-0.7.0/.coveragerc` & `aleph-sdk-python-0.7.0b1/.coveragerc`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/.github/workflows/build-wheels.yml` & `aleph-sdk-python-0.7.0b1/.github/workflows/build-wheels.yml`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/.github/workflows/code-quality.yml` & `aleph-sdk-python-0.7.0b1/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/.github/workflows/pytest-docker.yml` & `aleph-sdk-python-0.7.0b1/.github/workflows/pytest-docker.yml`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/.gitignore` & `aleph-sdk-python-0.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/LICENSE.txt` & `aleph-sdk-python-0.7.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/PKG-INFO` & `aleph-sdk-python-0.7.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-sdk-python
-Version: 0.7.0
+Version: 0.7.0b1
 Summary: Lightweight Python Client library for the Aleph.im network
 Home-page: https://github.com/aleph-im/aleph-sdk-python
 Author: Aleph.im Team
 Author-email: hello@aleph.im
 License: mit
 Project-URL: Documentation, https://aleph.im/
 Platform: any
```

### Comparing `aleph-sdk-python-0.7.0/README.md` & `aleph-sdk-python-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docker/python-3.10.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/python-3.9.dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.10-bullseye
+FROM python:3.9-bullseye
 MAINTAINER The aleph.im project
 
 RUN apt-get update && apt-get -y upgrade && apt-get install -y \
      libsecp256k1-dev \
      && rm -rf /var/lib/apt/lists/*
 
 RUN useradd -s /bin/bash --create-home user
@@ -16,15 +16,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.4.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
```

### Comparing `aleph-sdk-python-0.7.0/docker/python-3.11.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/python-3.11.dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.4.0' pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
```

### Comparing `aleph-sdk-python-0.7.0/docker/python-3.9.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/python-3.10.dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.9-bullseye
+FROM python:3.10-bullseye
 MAINTAINER The aleph.im project
 
 RUN apt-get update && apt-get -y upgrade && apt-get install -y \
      libsecp256k1-dev \
      && rm -rf /var/lib/apt/lists/*
 
 RUN useradd -s /bin/bash --create-home user
@@ -16,15 +16,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.4.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
```

### Comparing `aleph-sdk-python-0.7.0/docker/ubuntu-20.04.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/ubuntu-20.04.dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.4.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
```

### Comparing `aleph-sdk-python-0.7.0/docker/ubuntu-22.04.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/ubuntu-22.04.dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.4.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
```

### Comparing `aleph-sdk-python-0.7.0/docker/with-ipfs.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/with-ipfs.dockerfile`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/Makefile` & `aleph-sdk-python-0.7.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/_static/logo.svg` & `aleph-sdk-python-0.7.0b1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/conf.py` & `aleph-sdk-python-0.7.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/account.rst` & `aleph-sdk-python-0.7.0b1/docs/content/account.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/aggregates.rst` & `aleph-sdk-python-0.7.0b1/docs/content/aggregates.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/async_notes.rst` & `aleph-sdk-python-0.7.0b1/docs/content/async_notes.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/cli.rst` & `aleph-sdk-python-0.7.0b1/docs/content/cli.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/introduction.rst` & `aleph-sdk-python-0.7.0b1/docs/content/introduction.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/posts.rst` & `aleph-sdk-python-0.7.0b1/docs/content/posts.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/content/programs.rst` & `aleph-sdk-python-0.7.0b1/docs/content/programs.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/docs/index.rst` & `aleph-sdk-python-0.7.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/examples/httpgateway.py` & `aleph-sdk-python-0.7.0b1/examples/httpgateway.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/examples/metrics.py` & `aleph-sdk-python-0.7.0b1/examples/metrics.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/examples/mqtt.py` & `aleph-sdk-python-0.7.0b1/examples/mqtt.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/examples/store.py` & `aleph-sdk-python-0.7.0b1/examples/store.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/mypy.ini` & `aleph-sdk-python-0.7.0b1/mypy.ini`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/setup.cfg` & `aleph-sdk-python-0.7.0b1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 	coincurve; python_version<"3.11"
 	coincurve>=17.0.0; python_version>="3.11"   # Technically, this should be >=18.0.0 but there is a conflict with eciespy
 	aiohttp>=3.8.3
 	eciespy; python_version<"3.11"
 	eciespy>=0.3.13; python_version>="3.11"
 	typing_extensions
 	typer
-	aleph-message==0.4.0
+	aleph-message~=0.3.2
 	eth_account>=0.4.0
 	eth_abi==4.0.0b2; python_version>="3.11"
 	python-magic
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
-	aiomqtt<=0.1.3
+	aiomqtt
 	psutil
 	pytest
 	pytest-cov
 	pytest-asyncio
 	pytest-mock
 	mypy
 	secp256k1
@@ -57,19 +57,19 @@
 	aleph-pytezos==0.1.1
 	types-certifi
 	types-setuptools
 	black
 	isort
 	flake8
 mqtt = 
-	aiomqtt<=0.1.3
+	aiomqtt
 	certifi
 	Click
 nuls2 = 
-	aleph-nuls2
+	nuls2-python
 ethereum = 
 	eth_account>=0.4.0
 	eth_abi==4.0.0b2; python_version>="3.11"
 polkadot = 
 	substrate-interface==1.3.4
 cosmos = 
 	cosmospy
```

### Comparing `aleph-sdk-python-0.7.0/setup.py` & `aleph-sdk-python-0.7.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/account.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/account.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/common.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-import logging
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Dict, Optional
 
 from coincurve.keys import PrivateKey
 from ecies import decrypt, encrypt
 
 from aleph.sdk.conf import settings
-from aleph.sdk.utils import enum_as_str
-
-logger = logging.getLogger(__name__)
 
 
 def get_verification_buffer(message: Dict) -> bytes:
     """
     Returns the verification buffer that Aleph nodes use to verify the signature of a message.
     Note:
         The verification buffer is a string of the following format:
         b"{chain}\\n{sender}\\n{type}\\n{item_hash}"
     Args:
         message: Message to get the verification buffer for
     Returns:
         bytes: Verification buffer
     """
-
-    # Convert Enum values to strings
-    return "\n".join(
-        (
-            enum_as_str(message["chain"]),
-            message["sender"],
-            enum_as_str(message["type"]),
-            message["item_hash"],
-        )
-    ).encode()
+    return "{chain}\n{sender}\n{type}\n{item_hash}".format(**message).encode("utf-8")
 
 
 def get_public_key(private_key):
     privkey = PrivateKey(private_key)
     return privkey.public_key.format()
 
 
@@ -129,17 +116,11 @@
         private_key = path.read_bytes()
     else:
         private_key = generate_key()
         path.parent.mkdir(exist_ok=True, parents=True)
         path.write_bytes(private_key)
 
         default_key_path = path.parent / "default.key"
-
-        # If the symlink exists but does not point to a file, delete it.
-        if default_key_path.is_symlink() and not default_key_path.resolve().exists():
-            default_key_path.unlink()
-            logger.warning("The symlink to the private key is broken")
-
-        # Create a symlink to use this key by default
         if not default_key_path.exists():
+            # Create a symlink to use this key by default
             default_key_path.symlink_to(path)
     return private_key
```

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/cosmos.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/cosmos.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/ethereum.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/ethereum.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     public_key: Union[bytes, str],
     message: Union[bytes, str],
 ):
     """
     Verifies a signature.
     Args:
         signature: The signature to verify. Can be a hex encoded string or bytes.
-        public_key: The sender's public key to use for verification. Can be a checksum, hex encoded string or bytes.
+        public_key: The sender's public key to use for verification. Can be a checksummed, hex encoded string or bytes.
         message: The message to verify. Can be an utf-8 string or bytes.
     Raises:
         BadSignatureError: If the signature is invalid.
     """
     if isinstance(signature, str):
         if signature.startswith("0x"):
             signature = signature[2:]
@@ -71,11 +71,11 @@
         public_key = "0x" + public_key.hex()
     if isinstance(message, bytes):
         message = message.decode("utf-8")
 
     message_hash = encode_defunct(text=message)
     try:
         address = Account.recover_message(message_hash, signature=signature)
-        if address.casefold() != public_key.casefold():
+        if address != public_key:
             raise BadSignatureError
     except (EthBadSignatureError, BadSignatureError) as e:
         raise BadSignatureError from e
```

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/nuls1.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls1.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/nuls2.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls2.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/remote.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/remote.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/sol.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/sol.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/substrate.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/substrate.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/chains/tezos.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/tezos.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/client.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,23 @@
 from aleph_message.models import (
     AggregateContent,
     AggregateMessage,
     AlephMessage,
     ForgetContent,
     ForgetMessage,
     ItemType,
+    Message,
     MessageType,
     PostContent,
     PostMessage,
-    ProgramContent,
     ProgramMessage,
     StoreContent,
     StoreMessage,
-    parse_message,
 )
-from aleph_message.models.execution.base import Encoding
+from aleph_message.models.program import Encoding, ProgramContent
 from aleph_message.status import MessageStatus
 from pydantic import ValidationError
 
 from aleph.sdk.types import Account, GenericMessage, StorageEnum
 
 from .conf import settings
 from .exceptions import (
@@ -442,15 +441,15 @@
 
 class AlephClient:
     api_server: str
     http_session: aiohttp.ClientSession
 
     def __init__(
         self,
-        api_server: Optional[str] = None,
+        api_server: Optional[str],
         api_unix_socket: Optional[str] = None,
         allow_unix_sockets: bool = True,
         timeout: Optional[aiohttp.ClientTimeout] = None,
     ):
         """AlephClient can use HTTP(S) or HTTP over Unix sockets.
         Unix sockets are used when running inside a virtual machine,
         and can be shared across containers in a more secure way than TCP ports.
@@ -710,15 +709,15 @@
             messages_raw = response_json["messages"]
 
             # All messages may not be valid according to the latest specification in
             # aleph-message. This allows the user to specify how errors should be handled.
             messages: List[AlephMessage] = []
             for message_raw in messages_raw:
                 try:
-                    message = parse_message(message_raw)
+                    message = Message(**message_raw)
                     messages.append(message)
                 except KeyError as e:
                     if not ignore_invalid_messages:
                         raise e
                     logger.log(
                         level=invalid_messages_log_level,
                         msg=f"KeyError: Field '{e.args[0]}' not found",
@@ -832,15 +831,15 @@
             async for msg in ws:
                 if msg.type == aiohttp.WSMsgType.TEXT:
                     if msg.data == "close cmd":
                         await ws.close()
                         break
                     else:
                         data = json.loads(msg.data)
-                        yield parse_message(data)
+                        yield Message(**data)
                 elif msg.type == aiohttp.WSMsgType.ERROR:
                     break
 
 
 class AuthenticatedAlephClient(AlephClient):
     account: Account
 
@@ -1384,15 +1383,15 @@
                 assert storage_engine == StorageEnum.storage
                 message_dict["item_hash"] = await self.storage_push(
                     content=content,
                 )
                 message_dict["item_type"] = ItemType.storage
 
         message_dict = await self.account.sign_message(message_dict)
-        return parse_message(message_dict)
+        return Message(**message_dict)
 
     async def submit(
         self,
         content: Dict[str, Any],
         message_type: MessageType,
         channel: Optional[str] = None,
         storage_engine: StorageEnum = StorageEnum.storage,
```

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/conf.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/conf.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/exceptions.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/types.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/types.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/utils.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import errno
 import logging
 import os
-from enum import Enum
 from pathlib import Path
 from shutil import make_archive
-from typing import Tuple, Type, Union
+from typing import Tuple, Type
 from zipfile import BadZipFile, ZipFile
 
 from aleph_message.models import MessageType
-from aleph_message.models.execution.program import Encoding
+from aleph_message.models.program import Encoding
 
 from aleph.sdk.conf import settings
 from aleph.sdk.types import GenericMessage
 
 logger = logging.getLogger(__name__)
 
 try:
@@ -73,22 +72,7 @@
     if not path.is_socket():
         raise FileNotFoundError(
             errno.ENOTSOCK,
             os.strerror(errno.ENOENT),
             unix_socket_path,
         )
     return True
-
-
-def enum_as_str(obj: Union[str, Enum]) -> str:
-    """Returns the value of an Enum, or the string itself when passing a string.
-
-    Python 3.11 adds a new formatting of string enums.
-    `str(MyEnum.value)` becomes `MyEnum.value` instead of `value`.
-    """
-    if not isinstance(obj, str):
-        raise TypeError(f"Unsupported enum type: {type(obj)}")
-
-    if isinstance(obj, Enum):
-        return obj.value
-
-    return obj
```

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/vm/app.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/app.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph/sdk/vm/cache.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 from typing import Any, Dict, List, NewType, Optional, Union
 
 import aiohttp
 from pydantic import AnyHttpUrl
 
 from ..conf import settings
-from ..utils import check_unix_socket_valid
 
 CacheKey = NewType("CacheKey", str)
 
 
 def sanitize_cache_key(key: str) -> CacheKey:
     if not re.match(r"^\w+$", key):
         raise ValueError("Key may only contain letters, numbers and underscore")
@@ -49,30 +48,16 @@
     cache: Dict[str, bytes]
     api_host: str
 
     def __init__(
         self,
         session: Optional[aiohttp.ClientSession] = None,
         connector_url: Optional[AnyHttpUrl] = None,
-        unix_socket: Optional[str] = None,
     ):
-        if session:
-            self.session = session
-        else:
-            unix_socket_path = unix_socket or settings.API_UNIX_SOCKET
-            if unix_socket_path:
-                check_unix_socket_valid(unix_socket_path)
-                connector = aiohttp.UnixConnector(path=unix_socket_path)
-            else:
-                connector = None
-
-            self.session = aiohttp.ClientSession(
-                base_url=connector_url, connector=connector
-            )
-
+        self.session = session or aiohttp.ClientSession(base_url=connector_url)
         self.cache = {}
         self.api_host = connector_url if connector_url else settings.API_HOST
 
     async def get(self, key: str) -> Optional[bytes]:
         sanitized_key = sanitize_cache_key(key)
         async with self.session.get(f"{self.api_host}/cache/{sanitized_key}") as resp:
             if resp.status == 404:
```

### Comparing `aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/PKG-INFO` & `aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-sdk-python
-Version: 0.7.0
+Version: 0.7.0b1
 Summary: Lightweight Python Client library for the Aleph.im network
 Home-page: https://github.com/aleph-im/aleph-sdk-python
 Author: Aleph.im Team
 Author-email: hello@aleph.im
 License: mit
 Project-URL: Documentation, https://aleph.im/
 Platform: any
```

### Comparing `aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/SOURCES.txt` & `aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/src/aleph_sdk_python.egg-info/requires.txt` & `aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 aiohttp>=3.8.3
 typing_extensions
 typer
-aleph-message==0.4.0
+aleph-message~=0.3.2
 eth_account>=0.4.0
 python-magic
 
 [:python_version < "3.11"]
 coincurve
 eciespy
 
@@ -23,30 +23,30 @@
 [ethereum]
 eth_account>=0.4.0
 
 [ethereum:python_version >= "3.11"]
 eth_abi==4.0.0b2
 
 [mqtt]
-aiomqtt<=0.1.3
+aiomqtt
 certifi
 Click
 
 [nuls2]
-aleph-nuls2
+nuls2-python
 
 [polkadot]
 substrate-interface==1.3.4
 
 [solana]
 pynacl
 base58
 
 [testing]
-aiomqtt<=0.1.3
+aiomqtt
 psutil
 pytest
 pytest-cov
 pytest-asyncio
 pytest-mock
 mypy
 secp256k1
```

### Comparing `aleph-sdk-python-0.7.0/tests/integration/conftest.py` & `aleph-sdk-python-0.7.0b1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/integration/itest_aggregates.py` & `aleph-sdk-python-0.7.0b1/tests/integration/itest_aggregates.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/integration/itest_forget.py` & `aleph-sdk-python-0.7.0b1/tests/integration/itest_forget.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/integration/itest_posts.py` & `aleph-sdk-python-0.7.0b1/tests/integration/itest_posts.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/integration/toolkit.py` & `aleph-sdk-python-0.7.0b1/tests/integration/toolkit.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/conftest.py` & `aleph-sdk-python-0.7.0b1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_asynchronous.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_asynchronous_get.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous_get.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_chain_nuls1.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_chain_nuls1_compat.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1_compat.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_chain_solana.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_solana.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,18 +56,14 @@
     verif = verify_key.verify(
         verification_buffer, signature=base58.b58decode(signature["signature"])
     )
 
     assert verif == verification_buffer
     assert message["sender"] == signature["publicKey"]
 
-    pubkey = solana_account.get_public_key()
-    assert type(pubkey) == str
-    assert len(pubkey) == 64
-
 
 @pytest.mark.asyncio
 async def test_decrypt_curve25516(solana_account):
     assert solana_account.CURVE == "curve25519"
     content = b"SomeContent"
 
     encrypted = await solana_account.encrypt(content)
@@ -90,21 +86,14 @@
     await solana_account.sign_message(message)
     assert message["signature"]
     raw_signature = json.loads(message["signature"])["signature"]
     assert type(raw_signature) == str
 
     verify_signature(raw_signature, message["sender"], get_verification_buffer(message))
 
-    # as bytes
-    verify_signature(
-        base58.b58decode(raw_signature),
-        base58.b58decode(message["sender"]),
-        get_verification_buffer(message).decode("utf-8"),
-    )
-
 
 @pytest.mark.asyncio
 async def test_verify_signature_with_forged_signature(solana_account):
     message = asdict(
         Message(
             "SOL",
             solana_account.get_address(),
```

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_chain_tezos.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_tezos.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_remote_account.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_remote_account.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_synchronous_get.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_synchronous_get.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_vm_app.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_vm_app.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.7.0/tests/unit/test_vm_cache.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_vm_cache.py`

 * *Files identical despite different names*

