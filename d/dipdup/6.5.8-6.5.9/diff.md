# Comparing `tmp/dipdup-6.5.8.tar.gz` & `tmp/dipdup-6.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-6.5.8.tar", max compression
+gzip compressed data, was "dipdup-6.5.9.tar", max compression
```

## Comparing `dipdup-6.5.8.tar` & `dipdup-6.5.9.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0     1067 2023-06-28 13:08:44.629710 dipdup-6.5.8/LICENSE
--rw-r--r--   0        0        0     3992 2023-06-28 13:08:44.633710 dipdup-6.5.8/README.md
--rw-r--r--   0        0        0     2784 2023-06-28 13:08:44.673709 dipdup-6.5.8/pyproject.toml
--rw-r--r--   0        0        0      213 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/__init__.py
--rw-r--r--   0        0        0      106 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/__main__.py
--rw-r--r--   0        0        0      585 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/baking_bad.py
--rw-r--r--   0        0        0    19164 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/cli.py
--rw-r--r--   0        0        0    22413 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/codegen.py
--rw-r--r--   0        0        0    70122 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/config.py
--rw-r--r--   0        0        0    25902 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/context.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.673709 dipdup-6.5.8/src/dipdup/datasources/coinbase/__init__.py
--rw-r--r--   0        0        0     2387 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/coinbase/datasource.py
--rw-r--r--   0        0        0     1309 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/coinbase/models.py
--rw-r--r--   0        0        0     6291 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/datasource.py
--rw-r--r--   0        0        0     2420 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/factory.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/ipfs/__init__.py
--rw-r--r--   0        0        0      688 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/ipfs/datasource.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/metadata/__init__.py
--rw-r--r--   0        0        0     1773 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/metadata/datasource.py
--rw-r--r--   0        0        0      161 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/metadata/enums.py
--rw-r--r--   0        0        0     2172 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/subscription.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/tzkt/__init__.py
--rw-r--r--   0        0        0    46886 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/tzkt/datasource.py
--rw-r--r--   0        0        0     9895 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/datasources/tzkt/models.py
--rw-r--r--   0        0        0    25010 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     2013 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/enums.py
--rw-r--r--   0        0        0     2192 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/env.py
--rw-r--r--   0        0        0     9500 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     2734 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/fetcher.py
--rw-r--r--   0        0        0    25590 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/hasura.py
--rw-r--r--   0        0        0     9884 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/http.py
--rw-r--r--   0        0        0     7414 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/big_map/__init__.py
--rw-r--r--   0        0        0     3033 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/big_map/fetcher.py
--rw-r--r--   0        0        0     7103 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/big_map/index.py
--rw-r--r--   0        0        0     2131 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/big_map/matcher.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/event/__init__.py
--rw-r--r--   0        0        0     1402 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/event/fetcher.py
--rw-r--r--   0        0        0     5324 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/event/index.py
--rw-r--r--   0        0        0     3297 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/event/matcher.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/head/__init__.py
--rw-r--r--   0        0        0     2320 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/head/index.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/operation/__init__.py
--rw-r--r--   0        0        0    19397 2023-06-28 13:08:44.677709 dipdup-6.5.8/src/dipdup/indexes/operation/fetcher.py
--rw-r--r--   0        0        0    13470 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/indexes/operation/index.py
--rw-r--r--   0        0        0     8314 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/indexes/operation/matcher.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/indexes/token_transfer/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/indexes/token_transfer/fetcher.py
--rw-r--r--   0        0        0     5377 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/indexes/token_transfer/index.py
--rw-r--r--   0        0        0     1791 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/indexes/token_transfer/matcher.py
--rwxr-xr-x   0        0        0     8269 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/install.py
--rw-r--r--   0        0        0    22702 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/models.py
--rw-r--r--   0        0        0    10978 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/project.py
--rw-r--r--   0        0        0      203 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0     2097 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0      431 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/Dockerfile.j2
--rw-r--r--   0        0        0      474 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      489 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/dipdup.dev.yml.j2
--rw-r--r--   0        0        0      481 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/dipdup.prod.yml.j2
--rw-r--r--   0        0        0     2907 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/docker-compose.swarm.yml.j2
--rw-r--r--   0        0        0     1341 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/docker-compose.yml.j2
--rw-r--r--   0        0        0       37 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/replay.json.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0      197 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
--rw-r--r--   0        0        0      128 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/blank/dipdup.yml.j2
--rw-r--r--   0        0        0       95 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-auction.json
--rw-r--r--   0        0        0       98 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-big-maps.json
--rw-r--r--   0        0        0       83 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-dao.json
--rw-r--r--   0        0        0       83 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-dex.json
--rw-r--r--   0        0        0       95 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-domains.json
--rw-r--r--   0        0        0       92 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-events.json
--rw-r--r--   0        0        0      101 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-factories.json
--rw-r--r--   0        0        0       86 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-head.json
--rw-r--r--   0        0        0      119 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-nft-marketplace.json
--rw-r--r--   0        0        0       83 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-raw.json
--rw-r--r--   0        0        0      119 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-token-transfers.json
--rw-r--r--   0        0        0       89 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo-token.json
--rw-r--r--   0        0        0     1116 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_auction/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      918 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1624 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      853 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1524 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      779 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      847 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1713 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      840 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      702 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dao/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      416 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     4878 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0     1842 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1769 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      587 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1642 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1689 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1039 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      960 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1868 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1795 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      581 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1636 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1655 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1160 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      956 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      948 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      900 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_domains/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.681709 dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      564 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      536 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1475 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      819 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      592 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_events/dipdup.yml.j2
--rw-r--r--   0        0        0      976 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_factories/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      716 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
--rw-r--r--   0        0        0      416 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      333 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_head/dipdup.yml.j2
--rw-r--r--   0        0        0     1230 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      586 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1018 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      949 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      866 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1382 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      486 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_raw/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      350 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      235 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      787 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      453 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      647 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      945 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      456 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      550 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      822 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     1226 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/linters_default/Makefile.j2
--rw-r--r--   0        0        0     1032 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/linters_default/pyproject.toml.j2
--rw-r--r--   0        0        0      923 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/linters_none/Makefile.j2
--rw-r--r--   0        0        0      552 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/projects/linters_none/pyproject.toml.j2
--rw-r--r--   0        0        0     4008 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/py.typed
--rw-r--r--   0        0        0     4845 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     6041 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0      227 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0      157 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/templates/models.py.j2
--rw-r--r--   0        0        0     3271 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/transactions.py
--rw-r--r--   0        0        0     4760 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/utils/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/utils/codegen.py
--rw-r--r--   0        0        0    11504 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/utils/database.py
--rw-r--r--   0        0        0     2044 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/utils/sys.py
--rw-r--r--   0        0        0     4513 2023-06-28 13:08:44.685709 dipdup-6.5.8/src/dipdup/yaml.py
--rw-r--r--   0        0        0     5896 1970-01-01 00:00:00.000000 dipdup-6.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-11 14:03:03.119680 dipdup-6.5.9/LICENSE
+-rw-r--r--   0        0        0     3992 2023-07-11 14:03:03.119680 dipdup-6.5.9/README.md
+-rw-r--r--   0        0        0     2786 2023-07-11 14:03:03.147680 dipdup-6.5.9/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      106 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      585 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/baking_bad.py
+-rw-r--r--   0        0        0    19164 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/cli.py
+-rw-r--r--   0        0        0    22413 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/codegen.py
+-rw-r--r--   0        0        0    70122 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/config.py
+-rw-r--r--   0        0        0    25902 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/context.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/coinbase/__init__.py
+-rw-r--r--   0        0        0     2387 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/coinbase/datasource.py
+-rw-r--r--   0        0        0     1309 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/coinbase/models.py
+-rw-r--r--   0        0        0     6291 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/datasource.py
+-rw-r--r--   0        0        0     2420 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/factory.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/ipfs/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/ipfs/datasource.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/metadata/__init__.py
+-rw-r--r--   0        0        0     1773 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/metadata/datasource.py
+-rw-r--r--   0        0        0      161 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/metadata/enums.py
+-rw-r--r--   0        0        0     2172 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/tzkt/__init__.py
+-rw-r--r--   0        0        0    47179 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/tzkt/datasource.py
+-rw-r--r--   0        0        0     9895 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/tzkt/models.py
+-rw-r--r--   0        0        0    25010 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     2013 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/enums.py
+-rw-r--r--   0        0        0     2192 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/env.py
+-rw-r--r--   0        0        0     9500 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     2734 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0    25590 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/hasura.py
+-rw-r--r--   0        0        0     9884 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/http.py
+-rw-r--r--   0        0        0     7414 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/__init__.py
+-rw-r--r--   0        0        0     3033 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/fetcher.py
+-rw-r--r--   0        0        0     7103 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/index.py
+-rw-r--r--   0        0        0     2131 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/__init__.py
+-rw-r--r--   0        0        0     1402 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/fetcher.py
+-rw-r--r--   0        0        0     5324 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/index.py
+-rw-r--r--   0        0        0     3297 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/head/__init__.py
+-rw-r--r--   0        0        0     2320 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/head/index.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/__init__.py
+-rw-r--r--   0        0        0    19397 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/fetcher.py
+-rw-r--r--   0        0        0    13470 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/index.py
+-rw-r--r--   0        0        0     8314 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/__init__.py
+-rw-r--r--   0        0        0     1357 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/fetcher.py
+-rw-r--r--   0        0        0     5377 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/index.py
+-rw-r--r--   0        0        0     1791 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/matcher.py
+-rwxr-xr-x   0        0        0     8269 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/install.py
+-rw-r--r--   0        0        0    22702 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/models.py
+-rw-r--r--   0        0        0    10978 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/project.py
+-rw-r--r--   0        0        0      203 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0     2097 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0      431 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/Dockerfile.j2
+-rw-r--r--   0        0        0      474 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      489 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/dipdup.dev.yml.j2
+-rw-r--r--   0        0        0      481 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/dipdup.prod.yml.j2
+-rw-r--r--   0        0        0     2907 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/docker-compose.swarm.yml.j2
+-rw-r--r--   0        0        0     1341 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/docker-compose.yml.j2
+-rw-r--r--   0        0        0       37 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/replay.json.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0      197 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
+-rw-r--r--   0        0        0      128 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/blank/dipdup.yml.j2
+-rw-r--r--   0        0        0       95 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-auction.json
+-rw-r--r--   0        0        0       98 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-big-maps.json
+-rw-r--r--   0        0        0       83 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-dao.json
+-rw-r--r--   0        0        0       83 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-dex.json
+-rw-r--r--   0        0        0       95 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-domains.json
+-rw-r--r--   0        0        0       92 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-events.json
+-rw-r--r--   0        0        0      101 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-factories.json
+-rw-r--r--   0        0        0       86 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-head.json
+-rw-r--r--   0        0        0      119 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-nft-marketplace.json
+-rw-r--r--   0        0        0       83 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-raw.json
+-rw-r--r--   0        0        0      119 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-token-transfers.json
+-rw-r--r--   0        0        0       89 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-token.json
+-rw-r--r--   0        0        0     1116 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      918 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1624 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      853 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1524 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      779 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      847 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1713 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      840 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      702 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      416 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     4878 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dex/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0     1842 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1769 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      587 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1642 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1689 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1039 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      960 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1868 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1795 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      581 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1636 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1655 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1160 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      956 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      948 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      900 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      564 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      536 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1475 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      819 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      592 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_events/dipdup.yml.j2
+-rw-r--r--   0        0        0      976 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      716 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
+-rw-r--r--   0        0        0      416 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      333 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_head/dipdup.yml.j2
+-rw-r--r--   0        0        0     1230 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      586 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1018 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      949 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      866 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1382 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      486 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      350 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      235 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      787 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      453 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      647 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      945 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      456 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      550 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      822 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     1226 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_default/Makefile.j2
+-rw-r--r--   0        0        0     1032 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_default/pyproject.toml.j2
+-rw-r--r--   0        0        0      923 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_none/Makefile.j2
+-rw-r--r--   0        0        0      552 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_none/pyproject.toml.j2
+-rw-r--r--   0        0        0     4008 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/py.typed
+-rw-r--r--   0        0        0     4845 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     6041 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0      227 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0      157 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/templates/models.py.j2
+-rw-r--r--   0        0        0     3271 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     4760 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/codegen.py
+-rw-r--r--   0        0        0    11504 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/database.py
+-rw-r--r--   0        0        0     2044 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/sys.py
+-rw-r--r--   0        0        0     4513 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/yaml.py
+-rw-r--r--   0        0        0     5904 1970-01-01 00:00:00.000000 dipdup-6.5.9/PKG-INFO
```

### Comparing `dipdup-6.5.8/LICENSE` & `dipdup-6.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/README.md` & `dipdup-6.5.9/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/pyproject.toml` & `dipdup-6.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "6.5.8"
+version = "6.5.9"
 license = "MIT"
 authors = [
     "Lev Gorodetskiy <dipdup@drsr.io>",
     "Michael Zaikin <mz@baking-bad.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/dipdup-io/dipdup"
@@ -26,17 +26,17 @@
 packages = [
     { include = "dipdup", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 
-asyncpg = "0.27.0"
-datamodel-code-generator = "0.20.0"
-pydantic = "1.10.9"
+asyncpg = "0.28.0"
+datamodel-code-generator = "0.21.1"
+pydantic = "1.10.11"
 tortoise-orm = "0.19.3"
 
 aiohttp = "^3.8.1"
 aiolimiter = "^1.0.0"
 anyio = "^3.3.2"
 APScheduler = "^3.8.0"
 asyncclick = "^8.0.1"
@@ -46,15 +46,15 @@
 pysignalr = "0.2.0"
 python-dotenv = "^0.19.0"
 "ruamel.yaml" = "^0.17.2"
 sentry-sdk = "^1.4.3"
 sqlparse = "^0.4.2"
 tabulate = "^0.9.0"
 
-pytezos = {version = "3.10.0", optional = true}
+pytezos = {version = "^3.10.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 diff-cover = "*"
 docker = "*"
 ruff = "*"
 isort = "*"
```

### Comparing `dipdup-6.5.8/src/dipdup/baking_bad.py` & `dipdup-6.5.9/src/dipdup/baking_bad.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/cli.py` & `dipdup-6.5.9/src/dipdup/cli.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/codegen.py` & `dipdup-6.5.9/src/dipdup/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/config.py` & `dipdup-6.5.9/src/dipdup/config.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/context.py` & `dipdup-6.5.9/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/coinbase/datasource.py` & `dipdup-6.5.9/src/dipdup/datasources/coinbase/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/coinbase/models.py` & `dipdup-6.5.9/src/dipdup/datasources/coinbase/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/datasource.py` & `dipdup-6.5.9/src/dipdup/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/factory.py` & `dipdup-6.5.9/src/dipdup/datasources/factory.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/ipfs/datasource.py` & `dipdup-6.5.9/src/dipdup/datasources/ipfs/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/metadata/datasource.py` & `dipdup-6.5.9/src/dipdup/datasources/metadata/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/subscription.py` & `dipdup-6.5.9/src/dipdup/datasources/subscription.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/datasources/tzkt/datasource.py` & `dipdup-6.5.9/src/dipdup/datasources/tzkt/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,14 +574,15 @@
             first_level,
             last_level,
             offset,
             limit,
             TRANSACTION_OPERATION_FIELDS,
             cursor=True,
             status='applied',
+            sort='level',
         )
         if addresses and not code_hashes:
             params[f'{field}.in'] = ','.join(addresses)
         elif code_hashes and not addresses:
             params[f'{field}CodeHash.in'] = ','.join(str(h) for h in code_hashes)
 
         raw_transactions = await self.request(
@@ -827,14 +828,15 @@
         self,
         first_level: int | None = None,
         last_level: int | None = None,
         offset: int | None = None,
         limit: int | None = None,
         select: tuple[str, ...] | None = None,
         cursor: bool = False,
+        sort: str | None = None,
         **kwargs: Any,
     ) -> dict[str, Any]:
         params: dict[str, Any] = {
             'limit': limit or self.request_limit,
         }
         if first_level:
             params['level.ge'] = first_level
@@ -843,14 +845,21 @@
         if offset:
             if cursor:
                 params['offset.cr'] = offset
             else:
                 params['offset'] = offset
         if select:
             params['select'] = ','.join(select)
+        if sort:
+            if sort.startswith('-'):
+                sort_param_name = 'sort.desc'
+                sort = sort[1:]
+            else:
+                sort_param_name = 'sort'
+            params[sort_param_name] = sort
         return {
             **params,
             **kwargs,
         }
 
     async def _iter_batches(
         self,
```

### Comparing `dipdup-6.5.8/src/dipdup/datasources/tzkt/models.py` & `dipdup-6.5.9/src/dipdup/datasources/tzkt/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/dipdup.py` & `dipdup-6.5.9/src/dipdup/dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/enums.py` & `dipdup-6.5.9/src/dipdup/enums.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/env.py` & `dipdup-6.5.9/src/dipdup/env.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/exceptions.py` & `dipdup-6.5.9/src/dipdup/exceptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/fetcher.py` & `dipdup-6.5.9/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/hasura.py` & `dipdup-6.5.9/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/http.py` & `dipdup-6.5.9/src/dipdup/http.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/index.py` & `dipdup-6.5.9/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/big_map/fetcher.py` & `dipdup-6.5.9/src/dipdup/indexes/big_map/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/big_map/index.py` & `dipdup-6.5.9/src/dipdup/indexes/big_map/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/big_map/matcher.py` & `dipdup-6.5.9/src/dipdup/indexes/big_map/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/event/fetcher.py` & `dipdup-6.5.9/src/dipdup/indexes/event/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/event/index.py` & `dipdup-6.5.9/src/dipdup/indexes/event/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/event/matcher.py` & `dipdup-6.5.9/src/dipdup/indexes/event/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/head/index.py` & `dipdup-6.5.9/src/dipdup/indexes/head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/operation/fetcher.py` & `dipdup-6.5.9/src/dipdup/indexes/operation/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/operation/index.py` & `dipdup-6.5.9/src/dipdup/indexes/operation/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/operation/matcher.py` & `dipdup-6.5.9/src/dipdup/indexes/operation/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/token_transfer/fetcher.py` & `dipdup-6.5.9/src/dipdup/indexes/token_transfer/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/token_transfer/index.py` & `dipdup-6.5.9/src/dipdup/indexes/token_transfer/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/indexes/token_transfer/matcher.py` & `dipdup-6.5.9/src/dipdup/indexes/token_transfer/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/install.py` & `dipdup-6.5.9/src/dipdup/install.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/models.py` & `dipdup-6.5.9/src/dipdup/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/project.py` & `dipdup-6.5.9/src/dipdup/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,16 +282,16 @@
             name='hasura_image',
             description=(
                 'Choose Hasura version\n'
                 'Test new releases before using in production; new versions may break compatibility.'
             ),
             default=0,
             choices=(
-                'hasura/graphql-engine:v2.28.0',
-                'hasura/graphql-engine:v2.28.0',
+                'hasura/graphql-engine:v2.29.0',
+                'hasura/graphql-engine:v2.29.0',
             ),
             comments=(
                 'stable',
                 'beta',
             ),
         ),
         NotifyQuestion(
```

### Comparing `dipdup-6.5.8/src/dipdup/projects/base/.gitignore.j2` & `dipdup-6.5.9/src/dipdup/projects/base/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/base/docker-compose.swarm.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/base/docker-compose.swarm.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/base/docker-compose.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/base/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_auction/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_auction/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_big_maps/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dao/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dao/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_domains/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_domains/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_events/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_events/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_factories/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_factories/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_token/dipdup.yml.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_token/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2` & `dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/linters_default/Makefile.j2` & `dipdup-6.5.9/src/dipdup/projects/linters_default/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/linters_default/pyproject.toml.j2` & `dipdup-6.5.9/src/dipdup/projects/linters_default/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/linters_none/Makefile.j2` & `dipdup-6.5.9/src/dipdup/projects/linters_none/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/projects/linters_none/pyproject.toml.j2` & `dipdup-6.5.9/src/dipdup/projects/linters_none/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/prometheus.py` & `dipdup-6.5.9/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/scheduler.py` & `dipdup-6.5.9/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/sentry.py` & `dipdup-6.5.9/src/dipdup/sentry.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/sql/truncate_schema.sql` & `dipdup-6.5.9/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/transactions.py` & `dipdup-6.5.9/src/dipdup/transactions.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/utils/__init__.py` & `dipdup-6.5.9/src/dipdup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/utils/codegen.py` & `dipdup-6.5.9/src/dipdup/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/utils/database.py` & `dipdup-6.5.9/src/dipdup/utils/database.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/utils/sys.py` & `dipdup-6.5.9/src/dipdup/utils/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/src/dipdup/yaml.py` & `dipdup-6.5.9/src/dipdup/yaml.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.8/PKG-INFO` & `dipdup-6.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipdup
-Version: 6.5.8
+Version: 6.5.9
 Summary: Modular framework for creating selective indexers and featureful backends for dapps
 Home-page: https://dipdup.io/
 License: MIT
 Keywords: tezos,blockchain,sdk,michelson,indexers,tzkt,cryptocurrencies,smart-contracts
 Author: Lev Gorodetskiy
 Author-email: dipdup@drsr.io
 Requires-Python: >=3.10,<3.11
@@ -22,22 +22,22 @@
 Classifier: Typing :: Typed
 Provides-Extra: pytezos
 Requires-Dist: APScheduler (>=3.8.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
 Requires-Dist: anyio (>=3.3.2,<4.0.0)
 Requires-Dist: asyncclick (>=8.0.1,<9.0.0)
-Requires-Dist: asyncpg (==0.27.0)
-Requires-Dist: datamodel-code-generator (==0.20.0)
+Requires-Dist: asyncpg (==0.28.0)
+Requires-Dist: datamodel-code-generator (==0.21.1)
 Requires-Dist: orjson (>=3.6.6,<4.0.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
-Requires-Dist: pydantic (==1.10.9)
+Requires-Dist: pydantic (==1.10.11)
 Requires-Dist: pyhumps (>=3.0.2,<4.0.0)
 Requires-Dist: pysignalr (==0.2.0)
-Requires-Dist: pytezos (==3.10.0) ; extra == "pytezos"
+Requires-Dist: pytezos (>=3.10.0,<4.0.0) ; extra == "pytezos"
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: ruamel.yaml (>=0.17.2,<0.18.0)
 Requires-Dist: sentry-sdk (>=1.4.3,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tortoise-orm (==0.19.3)
 Project-URL: Repository, https://github.com/dipdup-io/dipdup
```

