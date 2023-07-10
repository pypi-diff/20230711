# Comparing `tmp/slingshot_ai-0.0.14.tar.gz` & `tmp/slingshot_ai-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.14.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.15.tar", max compression
```

## Comparing `slingshot_ai-0.0.14.tar` & `slingshot_ai-0.0.15.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      828 2023-07-10 21:30:31.398110 slingshot_ai-0.0.14/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-20 09:58:42.891207 slingshot_ai-0.0.14/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738131 slingshot_ai-0.0.14/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17919 2023-07-10 15:40:42.647885 slingshot_ai-0.0.14/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     2091 2023-06-27 10:21:25.506818 slingshot_ai-0.0.14/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     6421 2023-07-05 17:23:48.992824 slingshot_ai-0.0.14/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     5916 2023-06-23 10:00:55.765161 slingshot_ai-0.0.14/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5263 2023-06-27 10:21:25.507053 slingshot_ai-0.0.14/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 16:54:38.738871 slingshot_ai-0.0.14/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-13 14:12:37.848609 slingshot_ai-0.0.14/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738965 slingshot_ai-0.0.14/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-20 09:58:42.891910 slingshot_ai-0.0.14/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13774 2023-06-27 10:21:25.507213 slingshot_ai-0.0.14/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0     1234 2023-06-08 16:54:38.739227 slingshot_ai-0.0.14/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1123 2023-06-27 10:21:25.507291 slingshot_ai-0.0.14/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     5323 2023-07-05 17:23:48.992981 slingshot_ai-0.0.14/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 16:54:38.739428 slingshot_ai-0.0.14/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     1951 2023-06-30 17:31:08.610192 slingshot_ai-0.0.14/src/slingshot/cli/machine.py
--rw-r--r--   0        0        0     2759 2023-07-05 17:23:48.993098 slingshot_ai-0.0.14/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     2433 2023-07-03 15:58:05.510535 slingshot_ai-0.0.14/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.739665 slingshot_ai-0.0.14/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     8920 2023-07-07 09:11:42.963260 slingshot_ai-0.0.14/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 16:54:38.739947 slingshot_ai-0.0.14/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3845 2023-07-05 17:23:48.993362 slingshot_ai-0.0.14/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 16:54:38.740233 slingshot_ai-0.0.14/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-23 10:00:55.765417 slingshot_ai-0.0.14/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7029 2023-06-20 09:58:42.892817 slingshot_ai-0.0.14/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740473 slingshot_ai-0.0.14/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      191 2023-06-08 16:54:38.740573 slingshot_ai-0.0.14/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     5985 2023-07-07 09:11:42.964178 slingshot_ai-0.0.14/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 16:54:38.740763 slingshot_ai-0.0.14/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740862 slingshot_ai-0.0.14/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 16:54:38.741013 slingshot_ai-0.0.14/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741087 slingshot_ai-0.0.14/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-20 09:58:42.893069 slingshot_ai-0.0.14/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-20 09:58:42.893206 slingshot_ai-0.0.14/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 16:54:38.741497 slingshot_ai-0.0.14/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741599 slingshot_ai-0.0.14/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741656 slingshot_ai-0.0.14/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26670 2023-07-10 20:40:20.793233 slingshot_ai-0.0.14/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741863 slingshot_ai-0.0.14/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10181 2023-06-27 10:21:25.507893 slingshot_ai-0.0.14/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    15236 2023-07-10 20:40:20.793400 slingshot_ai-0.0.14/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    19518 2023-07-10 20:40:20.793564 slingshot_ai-0.0.14/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0      125 2023-07-07 09:11:36.011571 slingshot_ai-0.0.14/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    45606 2023-07-10 20:40:20.793788 slingshot_ai-0.0.14/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     2217 2023-06-08 16:54:38.742780 slingshot_ai-0.0.14/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     2073 2023-06-27 10:21:25.508229 slingshot_ai-0.0.14/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     1856 2023-06-20 09:58:42.894424 slingshot_ai-0.0.14/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     2372 2023-07-07 09:11:36.011656 slingshot_ai-0.0.14/src/slingshot/sdk/data_collector.py
--rw-r--r--   0        0        0     5334 2023-06-08 16:54:38.743055 slingshot_ai-0.0.14/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 16:54:38.743167 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-08 16:54:38.743260 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    18027 2023-06-27 10:21:25.508389 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.743421 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 16:54:38.743578 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-06-08 16:54:38.743672 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 16:54:38.743759 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3671 2023-06-08 16:54:38.743873 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5247 2023-06-27 10:21:25.508545 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744004 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2416 2023-07-07 09:11:42.964546 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     3578 2023-06-08 16:54:38.744228 slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744264 slingshot_ai-0.0.14/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    48216 2023-07-10 20:40:20.794010 slingshot_ai-0.0.14/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    52406 2023-07-10 20:40:20.794271 slingshot_ai-0.0.14/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     5420 2023-06-08 16:54:38.744840 slingshot_ai-0.0.14/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2862 2023-06-08 16:54:38.744928 slingshot_ai-0.0.14/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     2876 2023-06-20 09:58:42.895639 slingshot_ai-0.0.14/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4361 2023-07-05 17:23:48.994648 slingshot_ai-0.0.14/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745196 slingshot_ai-0.0.14/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745256 slingshot_ai-0.0.14/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     6308 2023-06-29 15:16:46.917807 slingshot_ai-0.0.14/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-07-10 21:33:19.634870 slingshot_ai-0.0.14/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745526 slingshot_ai-0.0.14/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-29 15:13:56.504338 slingshot_ai-0.0.14/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     1090 2023-06-08 16:54:38.745977 slingshot_ai-0.0.14/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.746012 slingshot_ai-0.0.14/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 slingshot_ai-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0      827 2023-07-10 21:48:51.271390 slingshot_ai-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-20 09:58:42.891207 slingshot_ai-0.0.15/src/slingshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738131 slingshot_ai-0.0.15/src/slingshot/cli/__init__.py
+-rw-r--r--   0        0        0    17919 2023-07-10 15:40:42.647885 slingshot_ai-0.0.15/src/slingshot/cli/add.py
+-rw-r--r--   0        0        0     2091 2023-06-27 10:21:25.506818 slingshot_ai-0.0.15/src/slingshot/cli/apply.py
+-rw-r--r--   0        0        0     6421 2023-07-05 17:23:48.992824 slingshot_ai-0.0.15/src/slingshot/cli/apps.py
+-rw-r--r--   0        0        0     5916 2023-06-23 10:00:55.765161 slingshot_ai-0.0.15/src/slingshot/cli/artifact.py
+-rw-r--r--   0        0        0     5263 2023-06-27 10:21:25.507053 slingshot_ai-0.0.15/src/slingshot/cli/auth.py
+-rw-r--r--   0        0        0      970 2023-06-08 16:54:38.738871 slingshot_ai-0.0.15/src/slingshot/cli/code.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:12:37.848609 slingshot_ai-0.0.15/src/slingshot/cli/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738965 slingshot_ai-0.0.15/src/slingshot/cli/config/py.typed
+-rw-r--r--   0        0        0      850 2023-06-20 09:58:42.891910 slingshot_ai-0.0.15/src/slingshot/cli/config/sentry_setup.py
+-rw-r--r--   0        0        0    13774 2023-06-27 10:21:25.507213 slingshot_ai-0.0.15/src/slingshot/cli/config/slingshot_cli.py
+-rw-r--r--   0        0        0     1234 2023-06-08 16:54:38.739227 slingshot_ai-0.0.15/src/slingshot/cli/dev.py
+-rw-r--r--   0        0        0     1123 2023-06-27 10:21:25.507291 slingshot_ai-0.0.15/src/slingshot/cli/environment.py
+-rw-r--r--   0        0        0     5323 2023-07-05 17:23:48.992981 slingshot_ai-0.0.15/src/slingshot/cli/inference.py
+-rw-r--r--   0        0        0     3059 2023-06-08 16:54:38.739428 slingshot_ai-0.0.15/src/slingshot/cli/logs.py
+-rw-r--r--   0        0        0     1951 2023-06-30 17:31:08.610192 slingshot_ai-0.0.15/src/slingshot/cli/machine.py
+-rw-r--r--   0        0        0     2759 2023-07-05 17:23:48.993098 slingshot_ai-0.0.15/src/slingshot/cli/main.py
+-rw-r--r--   0        0        0     2433 2023-07-03 15:58:05.510535 slingshot_ai-0.0.15/src/slingshot/cli/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.739665 slingshot_ai-0.0.15/src/slingshot/cli/py.typed
+-rw-r--r--   0        0        0     8920 2023-07-07 09:11:42.963260 slingshot_ai-0.0.15/src/slingshot/cli/run.py
+-rw-r--r--   0        0        0     3648 2023-06-08 16:54:38.739947 slingshot_ai-0.0.15/src/slingshot/cli/secret.py
+-rw-r--r--   0        0        0     3845 2023-07-05 17:23:48.993362 slingshot_ai-0.0.15/src/slingshot/cli/session.py
+-rw-r--r--   0        0        0       67 2023-06-08 16:54:38.740233 slingshot_ai-0.0.15/src/slingshot/cli/shared/__init__.py
+-rw-r--r--   0        0        0     6260 2023-06-23 10:00:55.765417 slingshot_ai-0.0.15/src/slingshot/cli/shared/code_sync.py
+-rw-r--r--   0        0        0     7029 2023-06-20 09:58:42.892817 slingshot_ai-0.0.15/src/slingshot/cli/shared/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740473 slingshot_ai-0.0.15/src/slingshot/cli/shared/py.typed
+-rw-r--r--   0        0        0      191 2023-06-08 16:54:38.740573 slingshot_ai-0.0.15/src/slingshot/cli/shared/settings.py
+-rw-r--r--   0        0        0     5985 2023-07-07 09:11:42.964178 slingshot_ai-0.0.15/src/slingshot/cli/shared/utils.py
+-rw-r--r--   0        0        0     1388 2023-06-08 16:54:38.740763 slingshot_ai-0.0.15/src/slingshot/cli/volume.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740862 slingshot_ai-0.0.15/src/slingshot/code/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 16:54:38.741013 slingshot_ai-0.0.15/src/slingshot/code/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741087 slingshot_ai-0.0.15/src/slingshot/code/py.typed
+-rw-r--r--   0        0        0       56 2023-06-20 09:58:42.893069 slingshot_ai-0.0.15/src/slingshot/inference_model/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-20 09:58:42.893206 slingshot_ai-0.0.15/src/slingshot/inference_model/inference_model.py
+-rw-r--r--   0        0        0      205 2023-06-08 16:54:38.741497 slingshot_ai-0.0.15/src/slingshot/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741599 slingshot_ai-0.0.15/src/slingshot/schemas/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741656 slingshot_ai-0.0.15/src/slingshot/schemas/generated/py.typed
+-rw-r--r--   0        0        0    26670 2023-07-10 20:40:20.793233 slingshot_ai-0.0.15/src/slingshot/schemas/generated/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741863 slingshot_ai-0.0.15/src/slingshot/schemas/py.typed
+-rw-r--r--   0        0        0    10181 2023-06-27 10:21:25.507893 slingshot_ai-0.0.15/src/slingshot/schemas/schema_extensions.py
+-rw-r--r--   0        0        0    15236 2023-07-10 20:40:20.793400 slingshot_ai-0.0.15/src/slingshot/schemas/slingshot-schema.config.json
+-rw-r--r--   0        0        0    19518 2023-07-10 20:40:20.793564 slingshot_ai-0.0.15/src/slingshot/schemas/slingshot_schema.py
+-rw-r--r--   0        0        0      125 2023-07-07 09:11:36.011571 slingshot_ai-0.0.15/src/slingshot/sdk/__init__.py
+-rw-r--r--   0        0        0    45606 2023-07-10 20:40:20.793788 slingshot_ai-0.0.15/src/slingshot/sdk/apply.py
+-rw-r--r--   0        0        0     2217 2023-06-08 16:54:38.742780 slingshot_ai-0.0.15/src/slingshot/sdk/auth.py
+-rw-r--r--   0        0        0     2073 2023-06-27 10:21:25.508229 slingshot_ai-0.0.15/src/slingshot/sdk/config.py
+-rw-r--r--   0        0        0     1856 2023-06-20 09:58:42.894424 slingshot_ai-0.0.15/src/slingshot/sdk/config_utils.py
+-rw-r--r--   0        0        0     2372 2023-07-07 09:11:36.011656 slingshot_ai-0.0.15/src/slingshot/sdk/data_collector.py
+-rw-r--r--   0        0        0     5334 2023-06-08 16:54:38.743055 slingshot_ai-0.0.15/src/slingshot/sdk/errors.py
+-rw-r--r--   0        0        0      126 2023-06-08 16:54:38.743167 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-08 16:54:38.743260 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/base_graphql.py
+-rw-r--r--   0        0        0    18027 2023-06-27 10:21:25.508389 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/fragments.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.743421 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/py.typed
+-rw-r--r--   0        0        0      138 2023-06-08 16:54:38.743578 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/__init__.py
+-rw-r--r--   0        0        0     5265 2023-06-08 16:54:38.743672 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/apps.py
+-rw-r--r--   0        0        0      986 2023-06-08 16:54:38.743759 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/deployment.py
+-rw-r--r--   0        0        0     3671 2023-06-08 16:54:38.743873 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/environment.py
+-rw-r--r--   0        0        0     5247 2023-06-27 10:21:25.508545 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744004 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/py.typed
+-rw-r--r--   0        0        0     2416 2023-07-07 09:11:42.964546 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/run.py
+-rw-r--r--   0        0        0     3578 2023-06-08 16:54:38.744228 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/storage.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744264 slingshot_ai-0.0.15/src/slingshot/sdk/py.typed
+-rw-r--r--   0        0        0    48216 2023-07-10 20:40:20.794010 slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_api.py
+-rw-r--r--   0        0        0    52406 2023-07-10 20:40:20.794271 slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_sdk.py
+-rw-r--r--   0        0        0     5420 2023-06-08 16:54:38.744840 slingshot_ai-0.0.15/src/slingshot/sdk/sync.py
+-rw-r--r--   0        0        0     2862 2023-06-08 16:54:38.744928 slingshot_ai-0.0.15/src/slingshot/sdk/upload_download_utils.py
+-rw-r--r--   0        0        0     2876 2023-06-20 09:58:42.895639 slingshot_ai-0.0.15/src/slingshot/sdk/utils.py
+-rw-r--r--   0        0        0     4361 2023-07-05 17:23:48.994648 slingshot_ai-0.0.15/src/slingshot/sdk/web_path_util.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745196 slingshot_ai-0.0.15/src/slingshot/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745256 slingshot_ai-0.0.15/src/slingshot/shared/py.typed
+-rw-r--r--   0        0        0     6308 2023-06-29 15:16:46.917807 slingshot_ai-0.0.15/src/slingshot/shared/utils.py
+-rw-r--r--   0        0        0       23 2023-07-10 21:49:00.875930 slingshot_ai-0.0.15/src/slingshot/slingshot_version.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745526 slingshot_ai-0.0.15/src/slingshot/templates/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-29 15:13:56.504338 slingshot_ai-0.0.15/src/slingshot/templates/inference_template.py
+-rw-r--r--   0        0        0     1090 2023-06-08 16:54:38.745977 slingshot_ai-0.0.15/src/slingshot/templates/label_studio_data_export_template.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.746012 slingshot_ai-0.0.15/src/slingshot/templates/py.typed
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 slingshot_ai-0.0.15/PKG-INFO
```

### Comparing `slingshot_ai-0.0.14/pyproject.toml` & `slingshot_ai-0.0.15/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [project]
 name = "slingshot-ai"
-version = "0.0.14"
+version = "0.0.15"
 
 [tool.poetry]
 name = "slingshot-ai"
-version = "0.0.14"
+version = "0.0.15"
 description = ""
 authors = ["Slingshot AI <service-account@slingshot.xyz>"]
 packages = [ { include = "slingshot", from = "src" } ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiohttp = ">=3.8.1"
-urllib3 = ">=1.26.11"
-pydantic = ">=1.9"
-typer = {extras = ["all"], version = ">=0.7.0"}
-requests = ">=2.28.1"
-sh = ">=1.14.3"
-pyyaml = ">=6.0"
-"ruamel.yaml" = ">=0.17.0"
-simple-term-menu = ">=1.6.0"
-deepdiff = ">=6.3.0"
-fastapi = ">=0.88.0"
-uvicorn = {extras = ["standard"], version = ">=0.18.0"}
-tqdm = ">=4.63.0"
-sentry-sdk = ">=1.13.0"
-backoff = ">=2.0.0"
-openai = ">=0.27.8"
+aiohttp = "~=3.8.1"
+urllib3 = "~=1.26.11"
+pydantic = "==1.9"
+typer = {extras = ["all"], version = "~0.7.0"}
+requests = "~=2.28.1"
+sh = "~=1.14.3"
+pyyaml = "~=6.0"
+"ruamel.yaml" = "~=0.17.0"
+simple-term-menu = "~=1.6.0"
+deepdiff = "~=6.3.0"
+fastapi = "~=0.88.0"
+uvicorn = {extras = ["standard"], version = "~=0.18.0"}
+tqdm = "~=4.63.0"
+sentry-sdk = "~=1.13.0"
+backoff = "~=2.0.0"
+openai = "~=0.27.8"
 
 [tool.poetry.scripts]
 slingshot = "slingshot.cli.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/add.py` & `slingshot_ai-0.0.15/src/slingshot/cli/add.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/apply.py` & `slingshot_ai-0.0.15/src/slingshot/cli/apply.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.15/src/slingshot/cli/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/artifact.py` & `slingshot_ai-0.0.15/src/slingshot/cli/artifact.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.15/src/slingshot/cli/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/code.py` & `slingshot_ai-0.0.15/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.15/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.15/src/slingshot/cli/config/slingshot_cli.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.15/src/slingshot/cli/dev.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.15/src/slingshot/cli/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/inference.py` & `slingshot_ai-0.0.15/src/slingshot/cli/inference.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.15/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/machine.py` & `slingshot_ai-0.0.15/src/slingshot/cli/machine.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/main.py` & `slingshot_ai-0.0.15/src/slingshot/cli/main.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/project.py` & `slingshot_ai-0.0.15/src/slingshot/cli/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/run.py` & `slingshot_ai-0.0.15/src/slingshot/cli/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.15/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/session.py` & `slingshot_ai-0.0.15/src/slingshot/cli/session.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.15/src/slingshot/cli/shared/code_sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.15/src/slingshot/cli/shared/prompt.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.15/src/slingshot/cli/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.15/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.15/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.15/src/slingshot/schemas/generated/schemas.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.15/src/slingshot/schemas/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.15/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.15/src/slingshot/schemas/slingshot_schema.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/apply.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/apply.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/config.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/config.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/config_utils.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/config_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/data_collector.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/fragments.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_api.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_sdk.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/upload_download_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/utils.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.15/src/slingshot/sdk/web_path_util.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.15/src/slingshot/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.15/src/slingshot/templates/inference_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.14/src/slingshot/templates/label_studio_data_export_template.py` & `slingshot_ai-0.0.15/src/slingshot/templates/label_studio_data_export_template.py`

 * *Files identical despite different names*

