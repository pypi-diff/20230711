# Comparing `tmp/lightdash_ops-0.2.1.tar.gz` & `tmp/lightdash_ops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_ops-0.2.1.tar", last modified: Thu Jul  6 00:32:13 2023, max compression
+gzip compressed data, was "lightdash_ops-0.2.2.tar", last modified: Tue Jul 11 05:10:53 2023, max compression
```

## Comparing `lightdash_ops-0.2.1.tar` & `lightdash_ops-0.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      103 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.env.template
--rw-r--r--   0        0        0      804 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1836 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2310 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1134 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1845 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.gitignore
--rw-r--r--   0        0        0     1383 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14060 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.pylintrc
--rw-r--r--   0        0        0      150 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.pypirc
--rw-r--r--   0        0        0        8 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.python-version
--rw-r--r--   0        0        0      183 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/.yamllint
--rw-r--r--   0        0        0    11357 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/LICENSE
--rw-r--r--   0        0        0      876 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/Makefile
--rw-r--r--   0        0        0     1536 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/README.md
--rw-r--r--   0        0        0     1047 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/dev/lint.sh
--rw-r--r--   0        0        0      994 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1391 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/dev/publish.sh
--rwxr-xr-x   0        0        0     1396 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/dev/setup.sh
--rwxr-xr-x   0        0        0     1170 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/dev/test_python.sh
--rw-r--r--   0        0        0     1283 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/dev/update_resources.sh
--rw-r--r--   0        0        0     4992 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/docs/cli.md
--rw-r--r--   0        0        0      879 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/__init__.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/cli/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/cli/main.py
--rw-r--r--   0        0        0     3533 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/cli/organization_v1.py
--rw-r--r--   0        0        0     8980 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/cli/project_v1.py
--rw-r--r--   0        0        0     1165 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/cli/settings.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/lightdash/__init__.py
--rw-r--r--   0        0        0     1239 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/lightdash/client.py
--rw-r--r--   0        0        0     3328 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/lightdash/organization.py
--rw-r--r--   0        0        0     3628 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/lightdash/project.py
--rw-r--r--   0        0        0     5168 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/lightdash/space.py
--rw-r--r--   0        0        0     5351 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/lightdash/user_group.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/__init__.py
--rw-r--r--   0        0        0     1098 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/base_user.py
--rw-r--r--   0        0        0     2533 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/organization.py
--rw-r--r--   0        0        0     2625 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/project.py
--rw-r--r--   0        0        0     2854 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/project_member.py
--rw-r--r--   0        0        0     2297 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/settings.py
--rw-r--r--   0        0        0     3312 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/space.py
--rw-r--r--   0        0        0     1856 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/models/user_group.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/operators/__init__.py
--rw-r--r--   0        0        0     4895 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/operators/organization_v1.py
--rw-r--r--   0        0        0     7739 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/operators/project_v1.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/__init__.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/lightdash/__init__.py
--rw-r--r--   0        0        0     1932 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/lightdash/test_organization.py
--rw-r--r--   0        0        0     1604 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/lightdash/test_project.py
--rw-r--r--   0        0        0      794 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/models/__init__.py
--rw-r--r--   0        0        0     1385 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/models/test_lightdash_user.py
--rw-r--r--   0        0        0     2072 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/models/test_manager_settings.py
--rw-r--r--   0        0        0     1279 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/models/test_project_member.py
--rw-r--r--   0        0        0     1389 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/models/test_space.py
--rw-r--r--   0        0        0     3035 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/models/test_user_group.py
--rw-r--r--   0        0        0      219 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/resources/test-organization-config-v1.yml
--rw-r--r--   0        0        0      764 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/resources/test-project-config-v1.yml
--rw-r--r--   0        0        0      325 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/resources/test-user-group-config-v1.yml
--rw-r--r--   0        0        0     2122 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/test_utils.py
--rw-r--r--   0        0        0     1932 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/tests/utils.py
--rw-r--r--   0        0        0     3615 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/lightdash_ops/utils.py
--rw-r--r--   0        0        0     2044 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      830 2023-07-06 00:32:13.000000 lightdash_ops-0.2.1/setup.py
--rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 lightdash_ops-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.env.template
+-rw-r--r--   0        0        0      804 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1836 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2310 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1134 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1845 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1383 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14060 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.pylintrc
+-rw-r--r--   0        0        0      150 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.pypirc
+-rw-r--r--   0        0        0        8 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.python-version
+-rw-r--r--   0        0        0      183 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/.yamllint
+-rw-r--r--   0        0        0    11357 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/LICENSE
+-rw-r--r--   0        0        0      876 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/Makefile
+-rw-r--r--   0        0        0     1579 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/README.md
+-rw-r--r--   0        0        0     1047 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/dev/lint.sh
+-rw-r--r--   0        0        0      994 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1391 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/dev/publish.sh
+-rwxr-xr-x   0        0        0     1396 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/dev/setup.sh
+-rwxr-xr-x   0        0        0     1170 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/dev/test_python.sh
+-rw-r--r--   0        0        0     1283 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/dev/update_resources.sh
+-rw-r--r--   0        0        0     4992 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/docs/cli.md
+-rw-r--r--   0        0        0      879 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/cli/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/cli/main.py
+-rw-r--r--   0        0        0     3533 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/cli/organization_v1.py
+-rw-r--r--   0        0        0     8980 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/cli/project_v1.py
+-rw-r--r--   0        0        0     1165 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/cli/settings.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/lightdash/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/lightdash/client.py
+-rw-r--r--   0        0        0     3328 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/lightdash/organization.py
+-rw-r--r--   0        0        0     3628 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/lightdash/project.py
+-rw-r--r--   0        0        0     5168 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/lightdash/space.py
+-rw-r--r--   0        0        0     5351 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/lightdash/user_group.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/__init__.py
+-rw-r--r--   0        0        0     1098 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/base_user.py
+-rw-r--r--   0        0        0     2533 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/organization.py
+-rw-r--r--   0        0        0     2625 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/project.py
+-rw-r--r--   0        0        0     2854 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/project_member.py
+-rw-r--r--   0        0        0     2297 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/settings.py
+-rw-r--r--   0        0        0     3312 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/space.py
+-rw-r--r--   0        0        0     1856 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/models/user_group.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/operators/__init__.py
+-rw-r--r--   0        0        0     4895 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/operators/organization_v1.py
+-rw-r--r--   0        0        0     7739 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/operators/project_v1.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/lightdash/__init__.py
+-rw-r--r--   0        0        0     1932 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/lightdash/test_organization.py
+-rw-r--r--   0        0        0     1604 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/lightdash/test_project.py
+-rw-r--r--   0        0        0      794 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/models/__init__.py
+-rw-r--r--   0        0        0     1385 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/models/test_lightdash_user.py
+-rw-r--r--   0        0        0     2072 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/models/test_manager_settings.py
+-rw-r--r--   0        0        0     1279 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/models/test_project_member.py
+-rw-r--r--   0        0        0     1389 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/models/test_space.py
+-rw-r--r--   0        0        0     3035 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/models/test_user_group.py
+-rw-r--r--   0        0        0      219 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/resources/test-organization-config-v1.yml
+-rw-r--r--   0        0        0      764 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/resources/test-project-config-v1.yml
+-rw-r--r--   0        0        0      325 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/resources/test-user-group-config-v1.yml
+-rw-r--r--   0        0        0     2122 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/test_utils.py
+-rw-r--r--   0        0        0     1932 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/tests/utils.py
+-rw-r--r--   0        0        0     3615 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/lightdash_ops/utils.py
+-rw-r--r--   0        0        0     2044 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-07-11 05:10:53.000000 lightdash_ops-0.2.2/setup.py
+-rw-r--r--   0        0        0     3681 1970-01-01 00:00:00.000000 lightdash_ops-0.2.2/PKG-INFO
```

### Comparing `lightdash_ops-0.2.1/.github/CODEOWNERS` & `lightdash_ops-0.2.2/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/.github/workflows/publish.yml` & `lightdash_ops-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/.github/workflows/test-publish.yml` & `lightdash_ops-0.2.2/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/.github/workflows/test.yml` & `lightdash_ops-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/.gitignore` & `lightdash_ops-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/.pre-commit-config.yaml` & `lightdash_ops-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/.pylintrc` & `lightdash_ops-0.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/LICENSE` & `lightdash_ops-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/Makefile` & `lightdash_ops-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/README.md` & `lightdash_ops-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 We can configure the API endpoint and so on with environment variables.
 We can also take advantage of an `.env` file.
 The template is located at [.env.template](.env.template).
 
 ```commandline
 # .env
-LIGHTDASH_BASE_URL=https://localhost:8000
+LIGHTDASH_URL=https://localhost:8000
 ...
 ```
 
 ### How to use
 
 The CLI requires a personal access token to call the Lightdash APIs.
 [The official documentation](https://docs.lightdash.com/references/personal_tokens/) describes how to get personal access tokens.
@@ -30,14 +30,15 @@
 The CLI provides many sub commands.
 Please refer to the detailed documentation in [docs/cli.ms](./docs/cli.md).
 
 #### Example
 The subsequent command is used to get all members in an organization.
 
 ```commandline
+$ export LIGHTDASH_URL="https://localhost:8000"
 $ export LIGHTDASH_API_KEY="YOUR-LIGHTDASH-PERSONAL-ACCESS-TOKEN"
 $ lightdash-ops organization get-members
 [
   {
     "member_uuid": "ade0aef5-bca8-4cbe-819b-07803390ffb0",
     "email": "lightdash-member@example.com",
     "role": "member"
```

### Comparing `lightdash_ops-0.2.1/dev/lint.sh` & `lightdash_ops-0.2.2/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/dev/lint_python.sh` & `lightdash_ops-0.2.2/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/dev/publish.sh` & `lightdash_ops-0.2.2/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/dev/setup.sh` & `lightdash_ops-0.2.2/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/dev/test_python.sh` & `lightdash_ops-0.2.2/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/dev/update_resources.sh` & `lightdash_ops-0.2.2/dev/update_resources.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/docs/cli.md` & `lightdash_ops-0.2.2/docs/cli.md`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/__init__.py` & `lightdash_ops-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-"""
-The CLI enables us to operate resources on Lightdash.
-"""
 #  Licensed to the Apache Software Foundation (ASF) under one or more
 #  contributor license agreements.  See the NOTICE file distributed with
 #  this work for additional information regarding copyright ownership.
 #  The ASF licenses this file to You under the Apache License, Version 2.0
 #  (the "License"); you may not use this file except in compliance with
 #  the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
+from setuptools import setup
 
-__version__ = '0.2.1'
+setup()
```

### Comparing `lightdash_ops-0.2.1/lightdash_ops/cli/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/cli/main.py` & `lightdash_ops-0.2.2/lightdash_ops/cli/main.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/cli/organization_v1.py` & `lightdash_ops-0.2.2/lightdash_ops/cli/organization_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/cli/project_v1.py` & `lightdash_ops-0.2.2/lightdash_ops/cli/project_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/cli/settings.py` & `lightdash_ops-0.2.2/lightdash_ops/cli/settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/lightdash/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/lightdash/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/lightdash/client.py` & `lightdash_ops-0.2.2/lightdash_ops/lightdash/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/lightdash/organization.py` & `lightdash_ops-0.2.2/lightdash_ops/lightdash/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/lightdash/project.py` & `lightdash_ops-0.2.2/lightdash_ops/lightdash/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/lightdash/space.py` & `lightdash_ops-0.2.2/lightdash_ops/lightdash/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/lightdash/user_group.py` & `lightdash_ops-0.2.2/lightdash_ops/lightdash/user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/base_user.py` & `lightdash_ops-0.2.2/lightdash_ops/models/base_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/organization.py` & `lightdash_ops-0.2.2/lightdash_ops/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/project.py` & `lightdash_ops-0.2.2/lightdash_ops/models/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/project_member.py` & `lightdash_ops-0.2.2/lightdash_ops/models/project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/settings.py` & `lightdash_ops-0.2.2/lightdash_ops/models/settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/space.py` & `lightdash_ops-0.2.2/lightdash_ops/models/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/models/user_group.py` & `lightdash_ops-0.2.2/lightdash_ops/models/user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/operators/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/operators/organization_v1.py` & `lightdash_ops-0.2.2/lightdash_ops/operators/organization_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/operators/project_v1.py` & `lightdash_ops-0.2.2/lightdash_ops/operators/project_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/lightdash/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/lightdash/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/lightdash/test_organization.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/lightdash/test_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/lightdash/test_project.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/lightdash/test_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/models/__init__.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/models/test_lightdash_user.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/models/test_lightdash_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/models/test_manager_settings.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/models/test_manager_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/models/test_project_member.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/models/test_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/models/test_space.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/models/test_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/models/test_user_group.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/models/test_user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/resources/test-project-config-v1.yml` & `lightdash_ops-0.2.2/lightdash_ops/tests/resources/test-project-config-v1.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/test_utils.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/tests/utils.py` & `lightdash_ops-0.2.2/lightdash_ops/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/lightdash_ops/utils.py` & `lightdash_ops-0.2.2/lightdash_ops/utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.2.1/pyproject.toml` & `lightdash_ops-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 dependencies = [
     "pydantic[dotenv] >=1.9,<2.0",
     "loguru >=0.7.0,<1.0.0",
     "typer>=0.9.0,<1.0.0",
     "email-validator>=1.1.3,<2.0.0",
     "ruamel.yaml >=0.17,<0.18",
     # NOTE Yu created the python-based client for lightdash by generating from the swagger spec.
-    "lightdash-client-python==0.640.1",
+    "lightdash-client-python==0.651.2",
 ]
 
 [project.urls]
 Home = "https://github.com/yu-iskw/lightdash-ops"
 
 [project.scripts]
 lightdash-ops = "lightdash_ops.cli.main:app"
```

### Comparing `lightdash_ops-0.2.1/setup.py` & `lightdash_ops-0.2.2/lightdash_ops/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""
+The CLI enables us to operate resources on Lightdash.
+"""
 #  Licensed to the Apache Software Foundation (ASF) under one or more
 #  contributor license agreements.  See the NOTICE file distributed with
 #  this work for additional information regarding copyright ownership.
 #  The ASF licenses this file to You under the Apache License, Version 2.0
 #  (the "License"); you may not use this file except in compliance with
 #  the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from setuptools import setup
+#
 
-setup()
+__version__ = '0.2.2'
```

### Comparing `lightdash_ops-0.2.1/PKG-INFO` & `lightdash_ops-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-ops
-Version: 0.2.1
+Version: 0.2.2
 Summary: The CLI enables us to operate resources on Lightdash.
 Author: yu-iskw
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Dist: pydantic[dotenv] >=1.9,<2.0
 Requires-Dist: loguru >=0.7.0,<1.0.0
 Requires-Dist: typer>=0.9.0,<1.0.0
 Requires-Dist: email-validator>=1.1.3,<2.0.0
 Requires-Dist: ruamel.yaml >=0.17,<0.18
-Requires-Dist: lightdash-client-python==0.640.1
+Requires-Dist: lightdash-client-python==0.651.2
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: types-PyYAML >=6.0,<7.0 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
 Requires-Dist: pre-commit >=2.15.0 ; extra == "dev"
@@ -62,15 +62,15 @@
 
 We can configure the API endpoint and so on with environment variables.
 We can also take advantage of an `.env` file.
 The template is located at [.env.template](.env.template).
 
 ```commandline
 # .env
-LIGHTDASH_BASE_URL=https://localhost:8000
+LIGHTDASH_URL=https://localhost:8000
 ...
 ```
 
 ### How to use
 
 The CLI requires a personal access token to call the Lightdash APIs.
 [The official documentation](https://docs.lightdash.com/references/personal_tokens/) describes how to get personal access tokens.
@@ -78,14 +78,15 @@
 The CLI provides many sub commands.
 Please refer to the detailed documentation in [docs/cli.ms](./docs/cli.md).
 
 #### Example
 The subsequent command is used to get all members in an organization.
 
 ```commandline
+$ export LIGHTDASH_URL="https://localhost:8000"
 $ export LIGHTDASH_API_KEY="YOUR-LIGHTDASH-PERSONAL-ACCESS-TOKEN"
 $ lightdash-ops organization get-members
 [
   {
     "member_uuid": "ade0aef5-bca8-4cbe-819b-07803390ffb0",
     "email": "lightdash-member@example.com",
     "role": "member"
```

