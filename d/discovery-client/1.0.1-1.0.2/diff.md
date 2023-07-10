# Comparing `tmp/discovery-client-1.0.1.tar.gz` & `tmp/discovery-client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-client-1.0.1.tar", last modified: Sun Dec 11 21:23:34 2022, max compression
+gzip compressed data, was "discovery-client-1.0.2.tar", last modified: Mon Jul 10 22:35:25 2023, max compression
```

## Comparing `discovery-client-1.0.1.tar` & `discovery-client-1.0.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.894875 discovery-client-1.0.1/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)    11326 2020-03-06 17:38:20.000000 discovery-client-1.0.1/LICENSE
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2902 2022-12-11 21:23:34.894875 discovery-client-1.0.1/PKG-INFO
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1299 2022-12-09 11:40:34.000000 discovery-client-1.0.1/README.md
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.882875 discovery-client-1.0.1/discovery/
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      514 2022-12-11 21:23:16.000000 discovery-client-1.0.1/discovery/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)       68 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/__main__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)       98 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/_logger.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.886875 discovery-client-1.0.1/discovery/api/
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1206 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      920 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/abc.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1652 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/acl.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      194 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/acl_link.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3980 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/agent.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2507 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/area.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3311 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/auth_method.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2143 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/autopilot.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      180 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/behavior.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2581 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/binding_rule.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1187 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/ca.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5780 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/catalog.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      216 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/check_status.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2652 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/checks.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1669 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/config.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1515 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/connect.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1397 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/coordinate.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1175 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/events.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     4012 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/health.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      237 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/health_state.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2928 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/intention.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      214 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/intention_by.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      497 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/intention_filter.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      180 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/intentions_action.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1494 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/keyring.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      503 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/kind.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3016 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/kv.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      989 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/license.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      257 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/loglevel.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1931 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/namespace.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      750 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/operator.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2635 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/policy.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3916 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/query.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1200 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/raft.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3132 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/role.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      474 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/segment.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2630 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/service.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3066 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/session.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      741 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/snapshot.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      723 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/status.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5149 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/token.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      181 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/token_locality.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      492 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/token_type.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      471 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/api/txn.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3206 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/checks.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.886875 discovery-client-1.0.1/discovery/cli/
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     4030 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/cli/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5003 2022-12-11 21:23:16.000000 discovery-client-1.0.1/discovery/client.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.886875 discovery-client-1.0.1/discovery/engine/
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      234 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1312 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/abc.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.886875 discovery-client-1.0.1/discovery/engine/aiohttp/
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      120 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/aiohttp/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2233 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/aiohttp/engine.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      937 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/aiohttp/response.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      849 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/base_response.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.886875 discovery-client-1.0.1/discovery/engine/httpx/
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      112 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/httpx/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2277 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/httpx/engine.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1005 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/httpx/response.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      860 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/engine/response.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      146 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/exceptions.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2233 2022-12-09 11:40:34.000000 discovery-client-1.0.1/discovery/utils.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.890875 discovery-client-1.0.1/discovery_client.egg-info/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2902 2022-12-11 21:23:34.000000 discovery-client-1.0.1/discovery_client.egg-info/PKG-INFO
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3176 2022-12-11 21:23:34.000000 discovery-client-1.0.1/discovery_client.egg-info/SOURCES.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        1 2022-12-11 21:23:34.000000 discovery-client-1.0.1/discovery_client.egg-info/dependency_links.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       53 2022-12-11 21:23:34.000000 discovery-client-1.0.1/discovery_client.egg-info/entry_points.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      225 2022-12-11 21:23:34.000000 discovery-client-1.0.1/discovery_client.egg-info/requires.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       16 2022-12-11 21:23:34.000000 discovery-client-1.0.1/discovery_client.egg-info/top_level.txt
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)       91 2022-12-09 11:40:34.000000 discovery-client-1.0.1/pyproject.toml
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2416 2022-12-11 21:23:34.894875 discovery-client-1.0.1/setup.cfg
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)       38 2022-12-09 11:40:34.000000 discovery-client-1.0.1/setup.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.890875 discovery-client-1.0.1/tests/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2020-09-26 11:54:13.000000 discovery-client-1.0.1/tests/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1933 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/conftest.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.890875 discovery-client-1.0.1/tests/unit/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2020-09-26 11:54:13.000000 discovery-client-1.0.1/tests/unit/__init__.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.894875 discovery-client-1.0.1/tests/unit/api/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2020-09-26 11:54:13.000000 discovery-client-1.0.1/tests/unit/api/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1893 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_acl.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     6808 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_agent.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3279 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_area.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3522 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_auth_method.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3985 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_autopilot.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2913 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_binding_rule.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3988 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_ca.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5582 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_catalog.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3522 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_checks.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1809 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_config.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5081 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_connect.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1995 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_coordinate.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1008 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_event.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5364 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_health.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3777 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_intention.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1952 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_keyring.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1118 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_kv.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1666 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_license.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5977 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_namespace.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      785 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_operator.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2720 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_policy.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     5728 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_query.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1099 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_raft.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3486 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_role.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      280 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_segment.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     7105 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_service.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1790 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_session.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1982 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_snapshot.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      643 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_status.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3014 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_token.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     3389 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/api/test_txn.py
-drwxrwxr-x   0 amenezes  (1000) amenezes  (1000)        0 2022-12-11 21:23:34.894875 discovery-client-1.0.1/tests/unit/engine/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2020-09-26 11:54:13.000000 discovery-client-1.0.1/tests/unit/engine/__init__.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1316 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/engine/test_aio.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1727 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/engine/test_httpx.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      905 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/engine/test_response.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     1169 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/setup.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     4029 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/test_client.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)     2686 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/test_service_module.py
--rw-rw-r--   0 amenezes  (1000) amenezes  (1000)      847 2022-12-09 11:40:34.000000 discovery-client-1.0.1/tests/unit/test_utils.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.201079 discovery-client-1.0.2/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)    11326 2023-02-21 00:36:05.000000 discovery-client-1.0.2/LICENSE
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2902 2023-07-10 22:35:25.201079 discovery-client-1.0.2/PKG-INFO
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1299 2023-02-21 00:36:05.000000 discovery-client-1.0.2/README.md
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.189079 discovery-client-1.0.2/discovery/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      514 2023-07-10 21:53:24.000000 discovery-client-1.0.2/discovery/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       68 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/__main__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       98 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/_logger.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/discovery/api/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1206 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      920 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/abc.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1652 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/acl.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      194 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/acl_link.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3980 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/agent.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2507 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/area.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3311 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/auth_method.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2143 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/autopilot.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      180 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/behavior.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2581 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/binding_rule.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1187 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/ca.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5780 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/catalog.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      216 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/check_status.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2652 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/checks.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1669 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/config.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1515 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/connect.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1397 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/coordinate.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1175 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/events.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4012 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/health.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      237 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/health_state.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2928 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/intention.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      214 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/intention_by.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      497 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/intention_filter.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      180 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/intentions_action.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1494 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/keyring.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      503 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/kind.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3016 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/kv.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      989 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/license.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      257 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/loglevel.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1931 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/namespace.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      750 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/operator.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2635 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/policy.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3916 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/query.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1200 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/raft.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3132 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/role.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      474 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/segment.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2630 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/service.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3066 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/session.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      741 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/snapshot.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      723 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/status.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5149 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/token.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      181 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/token_locality.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      492 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/token_type.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      471 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/api/txn.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3206 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/checks.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/discovery/cli/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5529 2023-07-10 22:28:16.000000 discovery-client-1.0.2/discovery/cli/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5053 2023-07-10 21:52:12.000000 discovery-client-1.0.2/discovery/client.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/discovery/engine/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      234 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1312 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/abc.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/discovery/engine/aiohttp/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      120 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/aiohttp/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2233 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/aiohttp/engine.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      937 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/aiohttp/response.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      849 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/base_response.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/discovery/engine/httpx/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      112 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/httpx/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2277 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/httpx/engine.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1005 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/httpx/response.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      860 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/engine/response.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      330 2023-07-10 21:50:41.000000 discovery-client-1.0.2/discovery/exceptions.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2233 2023-02-21 00:36:05.000000 discovery-client-1.0.2/discovery/utils.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/discovery_client.egg-info/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2902 2023-07-10 22:35:25.000000 discovery-client-1.0.2/discovery_client.egg-info/PKG-INFO
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3176 2023-07-10 22:35:25.000000 discovery-client-1.0.2/discovery_client.egg-info/SOURCES.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        1 2023-07-10 22:35:25.000000 discovery-client-1.0.2/discovery_client.egg-info/dependency_links.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       53 2023-07-10 22:35:25.000000 discovery-client-1.0.2/discovery_client.egg-info/entry_points.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      225 2023-07-10 22:35:25.000000 discovery-client-1.0.2/discovery_client.egg-info/requires.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       16 2023-07-10 22:35:25.000000 discovery-client-1.0.2/discovery_client.egg-info/top_level.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       91 2023-02-21 00:36:05.000000 discovery-client-1.0.2/pyproject.toml
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2416 2023-07-10 22:35:25.201079 discovery-client-1.0.2/setup.cfg
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       38 2023-02-21 00:36:05.000000 discovery-client-1.0.2/setup.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/tests/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1933 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/conftest.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.197079 discovery-client-1.0.2/tests/unit/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/__init__.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.201079 discovery-client-1.0.2/tests/unit/api/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1893 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_acl.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     6808 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_agent.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3279 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_area.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3522 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_auth_method.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3985 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_autopilot.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2913 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_binding_rule.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3988 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_ca.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5582 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_catalog.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3522 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_checks.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1809 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_config.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5081 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_connect.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1995 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_coordinate.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1008 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_event.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5364 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_health.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3777 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_intention.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1952 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_keyring.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1118 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_kv.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1666 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_license.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5977 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_namespace.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      785 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_operator.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2720 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_policy.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     5728 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_query.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1099 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_raft.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3486 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_role.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      280 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_segment.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     7105 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_service.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1790 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_session.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1982 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_snapshot.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      643 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_status.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3014 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_token.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3389 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/api/test_txn.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-07-10 22:35:25.201079 discovery-client-1.0.2/tests/unit/engine/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/engine/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1316 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/engine/test_aio.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1727 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/engine/test_httpx.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      905 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/engine/test_response.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1169 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/setup.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4029 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/test_client.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2686 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/test_service_module.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      847 2023-02-21 00:36:05.000000 discovery-client-1.0.2/tests/unit/test_utils.py
```

### Comparing `discovery-client-1.0.1/LICENSE` & `discovery-client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/PKG-INFO` & `discovery-client-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: async consul client
 Home-page: https://github.com/amenezes/discovery-client
 Author: Alexandre Menezes
 Author-email: alexandre.fmenezes@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://discovery-client.amenezes.net
 Project-URL: Code, https://github.com/amenezes/discovery-client
```

### Comparing `discovery-client-1.0.1/README.md` & `discovery-client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/__init__.py` & `discovery-client-1.0.2/discovery/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     LogLevel,
     TokenLocality,
     TokenType,
     kind,
 )
 from .client import Consul
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __all__ = [
     "Consul",
     "HealthState",
     "LogLevel",
     "TokenType",
     "checks",
     "utils",
```

### Comparing `discovery-client-1.0.1/discovery/api/__init__.py` & `discovery-client-1.0.2/discovery/api/__init__.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/abc.py` & `discovery-client-1.0.2/discovery/api/abc.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/acl.py` & `discovery-client-1.0.2/discovery/api/acl.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/agent.py` & `discovery-client-1.0.2/discovery/api/agent.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/area.py` & `discovery-client-1.0.2/discovery/api/area.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/auth_method.py` & `discovery-client-1.0.2/discovery/api/auth_method.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/autopilot.py` & `discovery-client-1.0.2/discovery/api/autopilot.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/binding_rule.py` & `discovery-client-1.0.2/discovery/api/binding_rule.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/ca.py` & `discovery-client-1.0.2/discovery/api/ca.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/catalog.py` & `discovery-client-1.0.2/discovery/api/catalog.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/checks.py` & `discovery-client-1.0.2/discovery/api/checks.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/config.py` & `discovery-client-1.0.2/discovery/api/config.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/connect.py` & `discovery-client-1.0.2/discovery/api/connect.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/coordinate.py` & `discovery-client-1.0.2/discovery/api/coordinate.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/events.py` & `discovery-client-1.0.2/discovery/api/events.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/health.py` & `discovery-client-1.0.2/discovery/api/health.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/intention.py` & `discovery-client-1.0.2/discovery/api/intention.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/keyring.py` & `discovery-client-1.0.2/discovery/api/keyring.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/kv.py` & `discovery-client-1.0.2/discovery/api/kv.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/license.py` & `discovery-client-1.0.2/discovery/api/license.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/namespace.py` & `discovery-client-1.0.2/discovery/api/namespace.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/operator.py` & `discovery-client-1.0.2/discovery/api/operator.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/policy.py` & `discovery-client-1.0.2/discovery/api/policy.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/query.py` & `discovery-client-1.0.2/discovery/api/query.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/raft.py` & `discovery-client-1.0.2/discovery/api/raft.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/role.py` & `discovery-client-1.0.2/discovery/api/role.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/service.py` & `discovery-client-1.0.2/discovery/api/service.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/session.py` & `discovery-client-1.0.2/discovery/api/session.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/snapshot.py` & `discovery-client-1.0.2/discovery/api/snapshot.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/status.py` & `discovery-client-1.0.2/discovery/api/status.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/api/token.py` & `discovery-client-1.0.2/discovery/api/token.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/checks.py` & `discovery-client-1.0.2/discovery/checks.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/cli/__init__.py` & `discovery-client-1.0.2/discovery/cli/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import os
 
 import click
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
 from discovery import Consul, __version__
@@ -20,36 +21,45 @@
 def cli():
     pass
 
 
 @cli.command()
 @click.option("-l", "--leader", is_flag=True, help="Get Raft Leader.")
 @click.option("-p", "--peers", is_flag=True, help="List Raft Peers.")
-def status(leader, peers):
+@click.option("-v", "--verbose", is_flag=True, help="Extend output info.")
+def status(leader, peers, verbose):
     """Status API."""
+    if verbose:
+        _show_verbose()
+
     try:
         if leader:
             resp = loop.run_until_complete(consul.status.leader())
         elif peers:
             resp = loop.run_until_complete(consul.status.leader())
-    except Exception:
-        click.echo("<error>[!]</error> Falha ao realizar a operação.")
-    click.echo(resp)
+    except Exception as err:
+        console.print(f"[red][*][/red] Failed to process request: [details='{err}']")
+        raise SystemExit
+    console.print(resp)
 
 
 @cli.command()
 @click.option("-s", "--services", is_flag=True, help="List services catalog.")
 @click.option("-d", "--datacenters", is_flag=True, help="List datacenters.")
 @click.option("-n", "--nodes", is_flag=True, help="List nodes.")
-def catalog(services, datacenters, nodes):
+@click.option("-v", "--verbose", is_flag=True, help="Extend output info.")
+def catalog(services, datacenters, nodes, verbose):
     """Catalog API."""
     table = Table.grid(padding=(0, 1))
     table.add_column(style="cyan", justify="right")
     table.add_column(style="magenta")
 
+    if verbose:
+        _show_verbose()
+
     try:
         if services:
             resp = loop.run_until_complete(consul.catalog.list_services())
             for i, svc in enumerate(resp, start=1):
                 table.add_row(f"{i}[yellow]:[/yellow]", svc)
         elif datacenters:
             resp = loop.run_until_complete(consul.catalog.list_datacenters())
@@ -66,54 +76,87 @@
                         node["Address"],
                         "[yellow][bold]leader[/bold][/yellow]",
                     )
                 else:
                     table.add_row(
                         f"{i}[yellow]:[/yellow]", node["Node"], node["Address"]
                     )
-    except Exception:
-        click.echo("<error>[!]</error> Falha ao realizar a operação.")
+    except Exception as err:
+        console.print(f"[red][*][/red] Failed to process request: [details='{err}']")
+        raise SystemExit
     console.print(
         Panel(
             table,
             border_style="yellow",
             expand=True,
         )
     )
 
 
 @cli.command()
 @click.option("-n", "--node", help="Node name.")
 @click.option("-s", "--service", help="Service name.")
 @click.option("--state", help="State name.")
-def health(node, service, state):
+@click.option("-v", "--verbose", is_flag=True, help="Extend output info.")
+def health(node, service, state, verbose):
     """Health API."""
+    if verbose:
+        _show_verbose()
+
     try:
         if node:
             resp = loop.run_until_complete(consul.health.checks_for_node(node))
         elif service:
             resp = loop.run_until_complete(consul.health.checks_for_service(service))
         elif state:
             resp = loop.run_until_complete(consul.health.checks_in_state(state))
-    except Exception:
-        click.echo("<error>[!]</error> Falha ao realizar a operação.")
-        raise SystemExit(1)
-    click.echo(
+    except Exception as err:
+        console.print(f"[red][*][/red] Failed to process request: [details='{err}']")
+        raise SystemExit
+    console.print(
         resp
         # f"{highlight(json.dumps(resp, indent=4, sort_keys=True), JsonLexer(), TerminalFormatter())}"
     )
 
 
 @cli.command()
 @click.option("-r", "--read", is_flag=True, help="Read configuration.")
 @click.option("-d", "--delete", help="Delete raft peer.")
-def raft(read, delete):
+@click.option("-v", "--verbose", is_flag=True, help="Extend output info.")
+def raft(read, delete, verbose):
     """Raft API."""
+    if verbose:
+        _show_verbose()
+
     try:
         if read:
             resp = loop.run_until_complete(consul.operator.raft.read_configuration())
-            click.echo(resp)
+            console.print(resp)
         elif delete:
             resp = loop.run_until_complete(consul.operator.raft.delete_peer())
-            click.echo(resp)
-    except Exception:
-        click.echo("<error>[!]</error> Falha ao realizar a operação.")
+            console.print(resp)
+    except Exception as err:
+        console.print(f"[red][*][/red] Failed to process request: [details='{err}']")
+        raise SystemExit
+
+
+def _show_verbose():
+    engine, *_ = repr(consul.client).split("(")
+
+    table = Table.grid(padding=(0, 1))
+    table.add_column(style="cyan", justify="right")
+    table.add_column(style="magenta")
+
+    table.add_row("engine[yellow]:[/yellow] ", f"{engine}")
+    table.add_row("scheme[yellow]:[/yellow] ", f"{consul.client.scheme}")
+    table.add_row("host[yellow]:[/yellow] ", f"{consul.client.host}")
+    table.add_row("port[yellow]:[/yellow] ", f"{consul.client.port}")
+    table.add_row("URL[yellow]:[/yellow] ", f"{consul.client.url}")
+    table.add_row("reconnect timeout[yellow]:[/yellow] ", f"{consul.reconnect_timeout}")
+    console.print(
+        Panel(
+            table,
+            title="[bold yellow]client details[/bold yellow]",
+            border_style="yellow",
+            expand=True,
+        )
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `discovery-client-1.0.1/discovery/client.py` & `discovery-client-1.0.2/discovery/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,32 +54,32 @@
     def current_leader_id(self) -> Optional[str]:
         return self._leader_id
 
     async def leader_ip(self, *args, **kwargs) -> str:
         try:
             current_leader = await self.status.leader(*args, **kwargs)
             leader_ip, _ = current_leader.split(":")
-        except Exception:
-            raise NoConsulLeaderException
+        except Exception as err:
+            raise NoConsulLeaderException(details=str(err))
         return leader_ip
 
     async def leader_id(self, **kwargs) -> str:
         leader_ip = await self.leader_ip(**kwargs.get("leader_options", {}))
         instances = await self.health.service_instances(
             "consul", **kwargs.get("instance_options", {})
         )
         current_id = [
             instance["Node"]["ID"]
             for instance in instances
             if instance["Node"]["Address"] == leader_ip
         ][0]
         try:
             return str(current_id)
-        except Exception:
-            raise NoConsulLeaderException
+        except Exception as err:
+            raise NoConsulLeaderException(details=str(err))
 
     async def find_services(self, name: str) -> List[dict]:
         return await self.catalog.list_nodes_for_service(name)  # type: ignore
 
     async def find_service(
         self, name: str, fn: Callable = utils.select_one_rr, *args, **kwargs
     ) -> Optional[dict]:
```

### Comparing `discovery-client-1.0.1/discovery/engine/abc.py` & `discovery-client-1.0.2/discovery/engine/abc.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/engine/aiohttp/engine.py` & `discovery-client-1.0.2/discovery/engine/aiohttp/engine.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/engine/aiohttp/response.py` & `discovery-client-1.0.2/discovery/engine/aiohttp/response.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/engine/base_response.py` & `discovery-client-1.0.2/discovery/engine/base_response.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/engine/httpx/engine.py` & `discovery-client-1.0.2/discovery/engine/httpx/engine.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/engine/httpx/response.py` & `discovery-client-1.0.2/discovery/engine/httpx/response.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/engine/response.py` & `discovery-client-1.0.2/discovery/engine/response.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery/utils.py` & `discovery-client-1.0.2/discovery/utils.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/discovery_client.egg-info/PKG-INFO` & `discovery-client-1.0.2/discovery_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: async consul client
 Home-page: https://github.com/amenezes/discovery-client
 Author: Alexandre Menezes
 Author-email: alexandre.fmenezes@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://discovery-client.amenezes.net
 Project-URL: Code, https://github.com/amenezes/discovery-client
```

### Comparing `discovery-client-1.0.1/discovery_client.egg-info/SOURCES.txt` & `discovery-client-1.0.2/discovery_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/setup.cfg` & `discovery-client-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/conftest.py` & `discovery-client-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_acl.py` & `discovery-client-1.0.2/tests/unit/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_agent.py` & `discovery-client-1.0.2/tests/unit/api/test_agent.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_area.py` & `discovery-client-1.0.2/tests/unit/api/test_area.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_auth_method.py` & `discovery-client-1.0.2/tests/unit/api/test_auth_method.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_autopilot.py` & `discovery-client-1.0.2/tests/unit/api/test_autopilot.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_binding_rule.py` & `discovery-client-1.0.2/tests/unit/api/test_binding_rule.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_ca.py` & `discovery-client-1.0.2/tests/unit/api/test_ca.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_catalog.py` & `discovery-client-1.0.2/tests/unit/api/test_catalog.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_checks.py` & `discovery-client-1.0.2/tests/unit/api/test_checks.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_config.py` & `discovery-client-1.0.2/tests/unit/api/test_config.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_connect.py` & `discovery-client-1.0.2/tests/unit/api/test_connect.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_coordinate.py` & `discovery-client-1.0.2/tests/unit/api/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_event.py` & `discovery-client-1.0.2/tests/unit/api/test_event.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_health.py` & `discovery-client-1.0.2/tests/unit/api/test_health.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_intention.py` & `discovery-client-1.0.2/tests/unit/api/test_intention.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_keyring.py` & `discovery-client-1.0.2/tests/unit/api/test_keyring.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_kv.py` & `discovery-client-1.0.2/tests/unit/api/test_kv.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_license.py` & `discovery-client-1.0.2/tests/unit/api/test_license.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_namespace.py` & `discovery-client-1.0.2/tests/unit/api/test_namespace.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_operator.py` & `discovery-client-1.0.2/tests/unit/api/test_operator.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_policy.py` & `discovery-client-1.0.2/tests/unit/api/test_policy.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_query.py` & `discovery-client-1.0.2/tests/unit/api/test_query.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_raft.py` & `discovery-client-1.0.2/tests/unit/api/test_raft.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_role.py` & `discovery-client-1.0.2/tests/unit/api/test_role.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_service.py` & `discovery-client-1.0.2/tests/unit/api/test_service.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_session.py` & `discovery-client-1.0.2/tests/unit/api/test_session.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_snapshot.py` & `discovery-client-1.0.2/tests/unit/api/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_status.py` & `discovery-client-1.0.2/tests/unit/api/test_status.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_token.py` & `discovery-client-1.0.2/tests/unit/api/test_token.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/api/test_txn.py` & `discovery-client-1.0.2/tests/unit/api/test_txn.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/engine/test_aio.py` & `discovery-client-1.0.2/tests/unit/engine/test_aio.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/engine/test_httpx.py` & `discovery-client-1.0.2/tests/unit/engine/test_httpx.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/engine/test_response.py` & `discovery-client-1.0.2/tests/unit/engine/test_response.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/setup.py` & `discovery-client-1.0.2/tests/unit/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/test_client.py` & `discovery-client-1.0.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/test_service_module.py` & `discovery-client-1.0.2/tests/unit/test_service_module.py`

 * *Files identical despite different names*

### Comparing `discovery-client-1.0.1/tests/unit/test_utils.py` & `discovery-client-1.0.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

