# Comparing `tmp/smart_vector-0.1.dev734.tar.gz` & `tmp/smart_vector-0.1.dev735.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-8ucy4gu0/smart_vector-0.1.dev734.tar", last modified: Tue Jul 11 09:56:38 2023, max compression
+gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-zgjrftj4/smart_vector-0.1.dev735.tar", last modified: Tue Jul 11 09:58:09 2023, max compression
```

## Comparing `smart_vector-0.1.dev734.tar` & `smart_vector-0.1.dev735.tar`

### file list

```diff
@@ -1,235 +1,237 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.539659 smart_vector-0.1.dev734/
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.dockerignore
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.300307 smart_vector-0.1.dev734/.github/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.350067 smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.360394 smart_vector-0.1.dev734/.github/workflows/
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/workflows/chroma-release.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/workflows/chroma-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.pre-commit-config.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.361560 smart_vector-0.1.dev734/.vscode/
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/.vscode/settings.json
--rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/Dockerfile
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)      379 2023-07-11 09:56:38.539226 smart_vector-0.1.dev734/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/RELEASE_PROCESS.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.379375 smart_vector-0.1.dev734/bin/
--rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/backup.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/build
--rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/docker_entrypoint.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/generate_cloudformation.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/integration-test
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/restore.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/setup_linux.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/setup_mac.sh
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.380467 smart_vector-0.1.dev734/bin/templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/templates/docker-compose.yml
--rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/test-package.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/test-remote
--rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/test.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/bin/version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.387683 smart_vector-0.1.dev734/chromadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_vector-0.1.dev734/chromadb/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.397169 smart_vector-0.1.dev734/chromadb/api/
--rw-r--r--   0 johnyan    (501) staff       (20)    10943 2023-07-06 08:22:49.000000 smart_vector-0.1.dev734/chromadb/api/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12493 2023-07-07 00:28:31.000000 smart_vector-0.1.dev734/chromadb/api/fastapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17939 2023-07-10 00:46:47.000000 smart_vector-0.1.dev734/chromadb/api/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.400062 smart_vector-0.1.dev734/chromadb/api/models/
--rw-r--r--   0 johnyan    (501) staff       (20)    15101 2023-07-06 06:54:49.000000 smart_vector-0.1.dev734/chromadb/api/models/Collection.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1297 2023-07-10 00:46:47.000000 smart_vector-0.1.dev734/chromadb/api/smartapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_vector-0.1.dev734/chromadb/api/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_vector-0.1.dev734/chromadb/config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.410784 smart_vector-0.1.dev734/chromadb/db/
--rw-r--r--   0 johnyan    (501) staff       (20)     3417 2023-07-07 00:28:30.000000 smart_vector-0.1.dev734/chromadb/db/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6017 2023-07-07 00:28:30.000000 smart_vector-0.1.dev734/chromadb/db/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    22388 2023-07-10 00:46:47.000000 smart_vector-0.1.dev734/chromadb/db/clickhouse.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18856 2023-07-07 03:46:58.000000 smart_vector-0.1.dev734/chromadb/db/duckdb.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.414100 smart_vector-0.1.dev734/chromadb/db/impl/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/db/impl/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6234 2023-07-07 00:28:31.000000 smart_vector-0.1.dev734/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.416687 smart_vector-0.1.dev734/chromadb/db/index/
--rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/db/index/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11087 2023-07-10 00:46:47.000000 smart_vector-0.1.dev734/chromadb/db/index/hnswlib.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/db/migrations.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.420107 smart_vector-0.1.dev734/chromadb/db/mixins/
--rw-r--r--   0 johnyan    (501) staff       (20)     9206 2023-07-07 00:28:30.000000 smart_vector-0.1.dev734/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15571 2023-07-07 00:28:30.000000 smart_vector-0.1.dev734/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17789 2023-07-10 00:46:47.000000 smart_vector-0.1.dev734/chromadb/db/smartdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2669 2023-07-07 00:28:31.000000 smart_vector-0.1.dev734/chromadb/db/system.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/errors.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.421644 smart_vector-0.1.dev734/chromadb/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/ingest/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.423085 smart_vector-0.1.dev734/chromadb/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/segment/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.305033 smart_vector-0.1.dev734/chromadb/segment/impl/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.424059 smart_vector-0.1.dev734/chromadb/segment/impl/manager/
--rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.425074 smart_vector-0.1.dev734/chromadb/segment/impl/metadata/
--rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.426756 smart_vector-0.1.dev734/chromadb/segment/impl/vector/
--rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.428211 smart_vector-0.1.dev734/chromadb/server/
--rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/server/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.430643 smart_vector-0.1.dev734/chromadb/server/fastapi/
--rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.433807 smart_vector-0.1.dev734/chromadb/telemetry/
--rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/telemetry/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/telemetry/events.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.437841 smart_vector-0.1.dev734/chromadb/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/conftest.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.440312 smart_vector-0.1.dev734/chromadb/test/db/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.448648 smart_vector-0.1.dev734/chromadb/test/db/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/test_base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/test_migrations.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/db/test_system.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.449298 smart_vector-0.1.dev734/chromadb/test/hnswlib/
--rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.450322 smart_vector-0.1.dev734/chromadb/test/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.457497 smart_vector-0.1.dev734/chromadb/test/property/
--rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/invariants.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/strategies.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/test_add.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/test_collections.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/test_filtering.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.459056 smart_vector-0.1.dev734/chromadb/test/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/segment/test_vector.py
--rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/test_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/test_chroma.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/test_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.459842 smart_vector-0.1.dev734/chromadb/test/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_vector-0.1.dev734/chromadb/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.463377 smart_vector-0.1.dev734/chromadb/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_vector-0.1.dev734/chromadb/utils/embedding_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/chromadb/utils/messageid.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.320613 smart_vector-0.1.dev734/clients/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.481573 smart_vector-0.1.dev734/clients/js/
--rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/.prettierignore
--rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/.prettierrc.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.316874 smart_vector-0.1.dev734/clients/js/examples/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.488524 smart_vector-0.1.dev734/clients/js/examples/browser/
--rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/browser/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/browser/app.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/browser/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/browser/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.493885 smart_vector-0.1.dev734/clients/js/examples/node/
--rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/node/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/node/app.js
--rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/node/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/node/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/genapi.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/jest.config.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/openapitools.json
--rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/package.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.499413 smart_vector-0.1.dev734/clients/js/src/
--rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/ChromaClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/Collection.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.504351 smart_vector-0.1.dev734/clients/js/src/embeddings/
--rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.510753 smart_vector-0.1.dev734/clients/js/src/generated/
--rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/generated/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/generated/api.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/generated/configuration.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/generated/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/generated/models.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/generated/runtime.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/types.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/src/utils.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.519926 smart_vector-0.1.dev734/clients/js/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/add.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/collection.client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/data.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/get.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/initClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/query.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/update.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/tsconfig.json
--rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/tsconfig.module.json
--rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/js/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.524562 smart_vector-0.1.dev734/clients/python/
--rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/python/README.md
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/python/integration-test.sh
--rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/python/is_thin_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/clients/python/pyproject.toml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.526565 smart_vector-0.1.dev734/config/
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/config/backup_disk.xml
--rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/config/chroma_users.xml
--rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/docker-compose.server.example.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/docker-compose.test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/docker-compose.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.529353 smart_vector-0.1.dev734/examples/
--rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.322822 smart_vector-0.1.dev734/examples/deployments/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.532268 smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/
--rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/local_persistence.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/examples/where_filtering.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/log_config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.324737 smart_vector-0.1.dev734/migrations/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.532763 smart_vector-0.1.dev734/migrations/embeddings_queue/
--rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.533347 smart_vector-0.1.dev734/migrations/metadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.534560 smart_vector-0.1.dev734/migrations/sysdb/
--rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/pull_request_template.md
--rw-r--r--   0 johnyan    (501) staff       (20)      792 2023-07-11 09:50:53.000000 smart_vector-0.1.dev734/pyproject.toml
--rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/requirements.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_vector-0.1.dev734/requirements_dev.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-11 09:56:38.539784 smart_vector-0.1.dev734/setup.cfg
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.535483 smart_vector-0.1.dev734/smart_vector/
--rw-r--r--   0 johnyan    (501) staff       (20)       52 2023-07-11 09:25:53.000000 smart_vector-0.1.dev734/smart_vector/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3417 2023-07-11 09:50:53.000000 smart_vector-0.1.dev734/smart_vector/smart_vector.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:56:38.538675 smart_vector-0.1.dev734/smart_vector.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)      379 2023-07-11 09:56:38.000000 smart_vector-0.1.dev734/smart_vector.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5859 2023-07-11 09:56:38.000000 smart_vector-0.1.dev734/smart_vector.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-11 09:56:38.000000 smart_vector-0.1.dev734/smart_vector.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       11 2023-07-11 09:56:38.000000 smart_vector-0.1.dev734/smart_vector.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       13 2023-07-11 09:56:38.000000 smart_vector-0.1.dev734/smart_vector.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.812942 smart_vector-0.1.dev735/
+-rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.dockerignore
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.529484 smart_vector-0.1.dev735/.github/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.629410 smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.635830 smart_vector-0.1.dev735/.github/workflows/
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/workflows/chroma-release.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/workflows/chroma-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.pre-commit-config.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.636994 smart_vector-0.1.dev735/.vscode/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/.vscode/settings.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/Dockerfile
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)      379 2023-07-11 09:58:09.812071 smart_vector-0.1.dev735/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/RELEASE_PROCESS.md
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.651446 smart_vector-0.1.dev735/bin/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/backup.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/build
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/docker_entrypoint.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/generate_cloudformation.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/integration-test
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/restore.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/setup_linux.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/setup_mac.sh
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.652174 smart_vector-0.1.dev735/bin/templates/
+-rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/test-package.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/test-remote
+-rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/test.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/bin/version
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.659204 smart_vector-0.1.dev735/chromadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_vector-0.1.dev735/chromadb/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.667136 smart_vector-0.1.dev735/chromadb/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10943 2023-07-06 08:22:49.000000 smart_vector-0.1.dev735/chromadb/api/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12493 2023-07-07 00:28:31.000000 smart_vector-0.1.dev735/chromadb/api/fastapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17939 2023-07-10 00:46:47.000000 smart_vector-0.1.dev735/chromadb/api/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.668422 smart_vector-0.1.dev735/chromadb/api/models/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15101 2023-07-06 06:54:49.000000 smart_vector-0.1.dev735/chromadb/api/models/Collection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1297 2023-07-10 00:46:47.000000 smart_vector-0.1.dev735/chromadb/api/smartapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_vector-0.1.dev735/chromadb/api/types.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_vector-0.1.dev735/chromadb/config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.680155 smart_vector-0.1.dev735/chromadb/db/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3417 2023-07-07 00:28:30.000000 smart_vector-0.1.dev735/chromadb/db/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6017 2023-07-07 00:28:30.000000 smart_vector-0.1.dev735/chromadb/db/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    22388 2023-07-10 00:46:47.000000 smart_vector-0.1.dev735/chromadb/db/clickhouse.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18856 2023-07-07 03:46:58.000000 smart_vector-0.1.dev735/chromadb/db/duckdb.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.682871 smart_vector-0.1.dev735/chromadb/db/impl/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/db/impl/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6234 2023-07-07 00:28:31.000000 smart_vector-0.1.dev735/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.686615 smart_vector-0.1.dev735/chromadb/db/index/
+-rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/db/index/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11087 2023-07-10 00:46:47.000000 smart_vector-0.1.dev735/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/db/migrations.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.689638 smart_vector-0.1.dev735/chromadb/db/mixins/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9206 2023-07-07 00:28:30.000000 smart_vector-0.1.dev735/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15571 2023-07-07 00:28:30.000000 smart_vector-0.1.dev735/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17789 2023-07-10 00:46:47.000000 smart_vector-0.1.dev735/chromadb/db/smartdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2669 2023-07-07 00:28:31.000000 smart_vector-0.1.dev735/chromadb/db/system.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/errors.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.690848 smart_vector-0.1.dev735/chromadb/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/ingest/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.691734 smart_vector-0.1.dev735/chromadb/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/segment/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.553918 smart_vector-0.1.dev735/chromadb/segment/impl/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.692701 smart_vector-0.1.dev735/chromadb/segment/impl/manager/
+-rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.693260 smart_vector-0.1.dev735/chromadb/segment/impl/metadata/
+-rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.694169 smart_vector-0.1.dev735/chromadb/segment/impl/vector/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/segment/impl/vector/local_hnsw.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.695191 smart_vector-0.1.dev735/chromadb/server/
+-rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/server/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.696785 smart_vector-0.1.dev735/chromadb/server/fastapi/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.698669 smart_vector-0.1.dev735/chromadb/telemetry/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/telemetry/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/telemetry/events.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.703369 smart_vector-0.1.dev735/chromadb/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/conftest.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.707096 smart_vector-0.1.dev735/chromadb/test/db/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.711924 smart_vector-0.1.dev735/chromadb/test/db/migrations/
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/test_base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/db/test_system.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.712448 smart_vector-0.1.dev735/chromadb/test/hnswlib/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.713260 smart_vector-0.1.dev735/chromadb/test/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.721905 smart_vector-0.1.dev735/chromadb/test/property/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/invariants.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/strategies.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/test_add.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/test_collections.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.724842 smart_vector-0.1.dev735/chromadb/test/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/test_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/test_chroma.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/test_config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.726861 smart_vector-0.1.dev735/chromadb/test/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_vector-0.1.dev735/chromadb/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.731975 smart_vector-0.1.dev735/chromadb/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_vector-0.1.dev735/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/chromadb/utils/messageid.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.601403 smart_vector-0.1.dev735/clients/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.749130 smart_vector-0.1.dev735/clients/js/
+-rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/.prettierignore
+-rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/.prettierrc.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.599820 smart_vector-0.1.dev735/clients/js/examples/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.754914 smart_vector-0.1.dev735/clients/js/examples/browser/
+-rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/browser/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/browser/app.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/browser/index.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/browser/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.758625 smart_vector-0.1.dev735/clients/js/examples/node/
+-rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/node/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/node/app.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/node/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/genapi.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/jest.config.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/openapitools.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/package.json
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.763366 smart_vector-0.1.dev735/clients/js/src/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/Collection.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.770643 smart_vector-0.1.dev735/clients/js/src/embeddings/
+-rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.778178 smart_vector-0.1.dev735/clients/js/src/generated/
+-rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/generated/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/generated/api.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/generated/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/generated/models.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/types.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/src/utils.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.793825 smart_vector-0.1.dev735/clients/js/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/data.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/initClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/tsconfig.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/tsconfig.module.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/js/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.796789 smart_vector-0.1.dev735/clients/python/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/python/README.md
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/python/integration-test.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/python/is_thin_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/clients/python/pyproject.toml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.798773 smart_vector-0.1.dev735/config/
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/config/backup_disk.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/config/chroma_users.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/docker-compose.server.example.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/docker-compose.test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/docker-compose.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.800263 smart_vector-0.1.dev735/examples/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/alternative_embeddings.ipynb
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.602362 smart_vector-0.1.dev735/examples/deployments/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.802847 smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/variables.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/local_persistence.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/examples/where_filtering.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/log_config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.603803 smart_vector-0.1.dev735/migrations/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.803420 smart_vector-0.1.dev735/migrations/embeddings_queue/
+-rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.803922 smart_vector-0.1.dev735/migrations/metadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.805511 smart_vector-0.1.dev735/migrations/sysdb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/pull_request_template.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      792 2023-07-11 09:50:53.000000 smart_vector-0.1.dev735/pyproject.toml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_vector-0.1.dev735/pyproject_chroma.toml
+-rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/requirements.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_vector-0.1.dev735/requirements_dev.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-11 09:58:09.813153 smart_vector-0.1.dev735/setup.cfg
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.808652 smart_vector-0.1.dev735/smart_vector/
+-rw-r--r--   0 johnyan    (501) staff       (20)       52 2023-07-11 09:25:53.000000 smart_vector-0.1.dev735/smart_vector/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2713 2023-07-11 09:50:53.000000 smart_vector-0.1.dev735/smart_vector/readme.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     3417 2023-07-11 09:50:53.000000 smart_vector-0.1.dev735/smart_vector/smart_vector.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-11 09:58:09.811231 smart_vector-0.1.dev735/smart_vector.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)      379 2023-07-11 09:58:09.000000 smart_vector-0.1.dev735/smart_vector.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5904 2023-07-11 09:58:09.000000 smart_vector-0.1.dev735/smart_vector.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-11 09:58:09.000000 smart_vector-0.1.dev735/smart_vector.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       11 2023-07-11 09:58:09.000000 smart_vector-0.1.dev735/smart_vector.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       13 2023-07-11 09:58:09.000000 smart_vector-0.1.dev735/smart_vector.egg-info/top_level.txt
```

### Comparing `smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/bug_report.yaml` & `smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/feature_request.yaml` & `smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `smart_vector-0.1.dev735/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/workflows/chroma-client-integration-test.yml` & `smart_vector-0.1.dev735/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/workflows/chroma-integration-test.yml` & `smart_vector-0.1.dev735/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/workflows/chroma-release-python-client.yml` & `smart_vector-0.1.dev735/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/workflows/chroma-release.yml` & `smart_vector-0.1.dev735/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/workflows/chroma-test.yml` & `smart_vector-0.1.dev735/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.github/workflows/pr-review-checklist.yml` & `smart_vector-0.1.dev735/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.pre-commit-config.yaml` & `smart_vector-0.1.dev735/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/.vscode/settings.json` & `smart_vector-0.1.dev735/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/DEVELOP.md` & `smart_vector-0.1.dev735/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/Dockerfile` & `smart_vector-0.1.dev735/Dockerfile`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/LICENSE` & `smart_vector-0.1.dev735/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/RELEASE_PROCESS.md` & `smart_vector-0.1.dev735/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/bin/backup.sh` & `smart_vector-0.1.dev735/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/bin/generate_cloudformation.py` & `smart_vector-0.1.dev735/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/bin/restore.sh` & `smart_vector-0.1.dev735/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/bin/setup_linux.sh` & `smart_vector-0.1.dev735/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/bin/templates/docker-compose.yml` & `smart_vector-0.1.dev735/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/__init__.py` & `smart_vector-0.1.dev735/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/api/__init__.py` & `smart_vector-0.1.dev735/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/api/fastapi.py` & `smart_vector-0.1.dev735/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/api/local.py` & `smart_vector-0.1.dev735/chromadb/api/local.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/api/models/Collection.py` & `smart_vector-0.1.dev735/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/api/smartapi.py` & `smart_vector-0.1.dev735/chromadb/api/smartapi.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/api/types.py` & `smart_vector-0.1.dev735/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/config.py` & `smart_vector-0.1.dev735/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/__init__.py` & `smart_vector-0.1.dev735/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/base.py` & `smart_vector-0.1.dev735/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/clickhouse.py` & `smart_vector-0.1.dev735/chromadb/db/clickhouse.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/duckdb.py` & `smart_vector-0.1.dev735/chromadb/db/duckdb.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/impl/sqlite.py` & `smart_vector-0.1.dev735/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/index/hnswlib.py` & `smart_vector-0.1.dev735/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/migrations.py` & `smart_vector-0.1.dev735/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/mixins/embeddings_queue.py` & `smart_vector-0.1.dev735/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/mixins/sysdb.py` & `smart_vector-0.1.dev735/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/smartdb.py` & `smart_vector-0.1.dev735/chromadb/db/smartdb.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/db/system.py` & `smart_vector-0.1.dev735/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/errors.py` & `smart_vector-0.1.dev735/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/ingest/__init__.py` & `smart_vector-0.1.dev735/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/segment/__init__.py` & `smart_vector-0.1.dev735/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/segment/impl/manager/local.py` & `smart_vector-0.1.dev735/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/segment/impl/metadata/sqlite.py` & `smart_vector-0.1.dev735/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/segment/impl/vector/local_hnsw.py` & `smart_vector-0.1.dev735/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/server/fastapi/__init__.py` & `smart_vector-0.1.dev735/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/server/fastapi/types.py` & `smart_vector-0.1.dev735/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/telemetry/__init__.py` & `smart_vector-0.1.dev735/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/telemetry/events.py` & `smart_vector-0.1.dev735/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/telemetry/posthog.py` & `smart_vector-0.1.dev735/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/conftest.py` & `smart_vector-0.1.dev735/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/db/test_base.py` & `smart_vector-0.1.dev735/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/db/test_migrations.py` & `smart_vector-0.1.dev735/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/db/test_system.py` & `smart_vector-0.1.dev735/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/hnswlib/test_hnswlib.py` & `smart_vector-0.1.dev735/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/ingest/test_producer_consumer.py` & `smart_vector-0.1.dev735/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/invariants.py` & `smart_vector-0.1.dev735/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/strategies.py` & `smart_vector-0.1.dev735/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/test_add.py` & `smart_vector-0.1.dev735/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/test_collections.py` & `smart_vector-0.1.dev735/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/test_cross_version_persist.py` & `smart_vector-0.1.dev735/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/test_embeddings.py` & `smart_vector-0.1.dev735/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/test_filtering.py` & `smart_vector-0.1.dev735/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/property/test_persist.py` & `smart_vector-0.1.dev735/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/segment/test_metadata.py` & `smart_vector-0.1.dev735/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/segment/test_vector.py` & `smart_vector-0.1.dev735/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/test_api.py` & `smart_vector-0.1.dev735/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/test_chroma.py` & `smart_vector-0.1.dev735/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/test_config.py` & `smart_vector-0.1.dev735/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/test/utils/test_messagid.py` & `smart_vector-0.1.dev735/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/types.py` & `smart_vector-0.1.dev735/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/utils/embedding_functions.py` & `smart_vector-0.1.dev735/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/chromadb/utils/messageid.py` & `smart_vector-0.1.dev735/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/DEVELOP.md` & `smart_vector-0.1.dev735/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/LICENSE` & `smart_vector-0.1.dev735/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/README.md` & `smart_vector-0.1.dev735/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/examples/browser/app.ts` & `smart_vector-0.1.dev735/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/examples/browser/index.html` & `smart_vector-0.1.dev735/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/examples/browser/yarn.lock` & `smart_vector-0.1.dev735/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/examples/node/app.js` & `smart_vector-0.1.dev735/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/examples/node/package-lock.json` & `smart_vector-0.1.dev735/clients/js/examples/node/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/examples/node/yarn.lock` & `smart_vector-0.1.dev735/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/genapi.sh` & `smart_vector-0.1.dev735/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/package-lock.json` & `smart_vector-0.1.dev735/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/package.json` & `smart_vector-0.1.dev735/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/ChromaClient.ts` & `smart_vector-0.1.dev735/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/Collection.ts` & `smart_vector-0.1.dev735/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `smart_vector-0.1.dev735/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `smart_vector-0.1.dev735/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `smart_vector-0.1.dev735/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `smart_vector-0.1.dev735/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/generated/README.md` & `smart_vector-0.1.dev735/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/generated/api.ts` & `smart_vector-0.1.dev735/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/generated/configuration.ts` & `smart_vector-0.1.dev735/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/generated/models.ts` & `smart_vector-0.1.dev735/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/generated/runtime.ts` & `smart_vector-0.1.dev735/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/types.ts` & `smart_vector-0.1.dev735/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/src/utils.ts` & `smart_vector-0.1.dev735/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/add.collections.test.ts` & `smart_vector-0.1.dev735/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/client.test.ts` & `smart_vector-0.1.dev735/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/collection.client.test.ts` & `smart_vector-0.1.dev735/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/collection.test.ts` & `smart_vector-0.1.dev735/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/delete.collection.test.ts` & `smart_vector-0.1.dev735/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/get.collection.test.ts` & `smart_vector-0.1.dev735/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/peek.collection.test.ts` & `smart_vector-0.1.dev735/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/query.collection.test.ts` & `smart_vector-0.1.dev735/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/update.collection.test.ts` & `smart_vector-0.1.dev735/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/test/upsert.collections.test.ts` & `smart_vector-0.1.dev735/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/js/yarn.lock` & `smart_vector-0.1.dev735/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/python/README.md` & `smart_vector-0.1.dev735/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/python/build_python_thin_client.sh` & `smart_vector-0.1.dev735/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/python/integration-test.sh` & `smart_vector-0.1.dev735/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/clients/python/pyproject.toml` & `smart_vector-0.1.dev735/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/docker-compose.server.example.yml` & `smart_vector-0.1.dev735/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/docker-compose.test.yml` & `smart_vector-0.1.dev735/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/docker-compose.yml` & `smart_vector-0.1.dev735/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/examples/alternative_embeddings.ipynb` & `smart_vector-0.1.dev735/examples/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/README.md` & `smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/chroma.tf` & `smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/examples/deployments/google-cloud-compute/startup.sh` & `smart_vector-0.1.dev735/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/examples/local_persistence.ipynb` & `smart_vector-0.1.dev735/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/examples/where_filtering.ipynb` & `smart_vector-0.1.dev735/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `smart_vector-0.1.dev735/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/pyproject.toml` & `smart_vector-0.1.dev735/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/smart_vector/smart_vector.py` & `smart_vector-0.1.dev735/smart_vector/smart_vector.py`

 * *Files identical despite different names*

### Comparing `smart_vector-0.1.dev734/smart_vector.egg-info/SOURCES.txt` & `smart_vector-0.1.dev735/smart_vector.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 RELEASE_PROCESS.md
 docker-compose.server.example.yml
 docker-compose.test.yml
 docker-compose.yml
 log_config.yml
 pull_request_template.md
 pyproject.toml
+pyproject_chroma.toml
 requirements.txt
 requirements_dev.txt
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/feature_request.yaml
 .github/ISSUE_TEMPLATE/installation_trouble.yaml
 .github/workflows/chroma-client-integration-test.yml
 .github/workflows/chroma-integration-test.yml
@@ -169,13 +170,14 @@
 examples/deployments/google-cloud-compute/startup.sh
 examples/deployments/google-cloud-compute/variables.tf
 migrations/embeddings_queue/00001-embeddings.sqlite.sql
 migrations/metadb/00001-embedding-metadata.sqlite.sql
 migrations/sysdb/00001-collections.sqlite.sql
 migrations/sysdb/00002-segments.sqlite.sql
 smart_vector/__init__.py
+smart_vector/readme.md
 smart_vector/smart_vector.py
 smart_vector.egg-info/PKG-INFO
 smart_vector.egg-info/SOURCES.txt
 smart_vector.egg-info/dependency_links.txt
 smart_vector.egg-info/requires.txt
 smart_vector.egg-info/top_level.txt
```

