# Comparing `tmp/hcs-cli-0.1.43.tar.gz` & `tmp/hcs-cli-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.43.tar", last modified: Tue Jul 11 08:16:26 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.44.tar", last modified: Tue Jul 11 08:49:07 2023, max compression
```

## Comparing `hcs-cli-0.1.43.tar` & `hcs-cli-0.1.44.tar`

### file list

```diff
@@ -1,287 +1,288 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.619199 hcs-cli-0.1.43/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.43/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.346150 hcs-cli-0.1.43/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     2599 2023-07-11 06:28:37.000000 hcs-cli-0.1.43/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.43/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.43/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.43/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.43/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.43/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.43/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.43/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.43/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:16:26.618469 hcs-cli-0.1.43/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.43/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.350768 hcs-cli-0.1.43/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.43/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.43/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.43/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.43/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     2984 2023-07-11 07:26:34.000000 hcs-cli-0.1.43/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.355760 hcs-cli-0.1.43/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     6644 2023-07-11 08:16:26.000000 hcs-cli-0.1.43/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.302491 hcs-cli-0.1.43/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.357048 hcs-cli-0.1.43/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.43/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.43/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.43/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-11 08:16:26.619392 hcs-cli-0.1.43/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 08:16:22.000000 hcs-cli-0.1.43/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.359916 hcs-cli-0.1.43/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.43/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.361964 hcs-cli-0.1.43/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.363293 hcs-cli-0.1.43/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.368590 hcs-cli-0.1.43/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.371116 hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.374162 hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.378533 hcs-cli-0.1.43/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.43/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.383257 hcs-cli-0.1.43/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.388505 hcs-cli-0.1.43/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.389931 hcs-cli-0.1.43/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.391295 hcs-cli-0.1.43/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.395353 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.398004 hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.401722 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.405285 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.406346 hcs-cli-0.1.43/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.43/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.409955 hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.411744 hcs-cli-0.1.43/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.419267 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     2272 2023-07-07 17:19:46.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/plan.py
--rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/validate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.423496 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     4917 2023-07-07 17:46:45.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.435818 hcs-cli-0.1.43/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.43/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.43/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.43/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.444487 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.447979 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.454503 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.463487 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.43/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.313988 hcs-cli-0.1.43/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.465894 hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.468230 hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.474251 hcs-cli-0.1.43/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.478606 hcs-cli-0.1.43/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1745 2023-07-05 16:15:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1533 2023-07-05 20:40:38.000000 hcs-cli-0.1.43/vhcs/cli/cmds/plan/destroy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.480914 hcs-cli-0.1.43/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.484526 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.487980 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.490384 hcs-cli-0.1.43/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.43/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.491859 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.495573 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.43/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.500846 hcs-cli-0.1.43/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.518582 hcs-cli-0.1.43/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.43/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.43/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.43/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.522138 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.43/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.43/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.43/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.43/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.43/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5285 2023-07-06 00:57:57.000000 hcs-cli-0.1.43/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.43/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.43/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.43/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.43/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.532053 hcs-cli-0.1.43/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.43/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.43/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.43/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.43/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.43/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.43/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.43/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.534714 hcs-cli-0.1.43/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.43/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.539135 hcs-cli-0.1.43/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.43/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)    13207 2023-07-11 08:05:18.000000 hcs-cli-0.1.43/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     4754 2023-07-11 00:52:21.000000 hcs-cli-0.1.43/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.43/vhcs/plan/helper.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.540598 hcs-cli-0.1.43/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.43/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.551422 hcs-cli-0.1.43/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4432 2023-07-11 02:03:42.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1196 2023-07-11 02:17:50.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1669 2023-07-11 02:11:35.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1181 2023-07-11 01:23:30.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 01:23:47.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-07-11 01:23:57.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.554931 hcs-cli-0.1.43/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.43/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.43/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.43/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.561670 hcs-cli-0.1.43/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1027 2023-07-11 06:48:15.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1293 2023-07-11 07:14:46.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)     1212 2023-07-11 01:24:36.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/pool_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.566512 hcs-cli-0.1.43/vhcs/plan/provider/runtime/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     3396 2023-07-11 07:11:55.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/daas_tenant_calculation.py
--rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.568685 hcs-cli-0.1.43/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.574813 hcs-cli-0.1.43/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.43/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.43/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.43/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.43/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.43/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.43/vhcs/service/admin/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.576816 hcs-cli-0.1.43/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.43/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.43/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.582374 hcs-cli-0.1.43/vhcs/service/ims_catalog/
--rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/images.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.584388 hcs-cli-0.1.43/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.43/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.43/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.587817 hcs-cli-0.1.43/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.43/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.43/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.43/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.591294 hcs-cli-0.1.43/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.43/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.43/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.43/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.593499 hcs-cli-0.1.43/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.43/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.43/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.596707 hcs-cli-0.1.43/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-07-11 03:25:14.000000 hcs-cli-0.1.43/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1264 2023-07-11 03:23:26.000000 hcs-cli-0.1.43/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1236 2023-07-10 08:19:02.000000 hcs-cli-0.1.43/vhcs/service/portal/pool.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.598886 hcs-cli-0.1.43/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.43/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.43/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.601103 hcs-cli-0.1.43/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.43/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.606041 hcs-cli-0.1.43/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.43/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.43/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.43/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.43/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.328231 hcs-cli-0.1.43/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.610529 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3610 2023-07-11 07:19:41.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      224 2023-07-06 23:02:54.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.43/vhcs/support/daas/tenant.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.43/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.617338 hcs-cli-0.1.43/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.43/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.326897 hcs-cli-0.1.44/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.44/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.032033 hcs-cli-0.1.44/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     2552 2023-07-11 08:44:46.000000 hcs-cli-0.1.44/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.44/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.44/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.44/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.44/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.44/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.44/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.44/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.44/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:49:07.325355 hcs-cli-0.1.44/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.44/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.040411 hcs-cli-0.1.44/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.44/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.44/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.44/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.44/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2984 2023-07-11 07:26:34.000000 hcs-cli-0.1.44/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.045237 hcs-cli-0.1.44/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     6687 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-11 08:49:06.000000 hcs-cli-0.1.44/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:06.971597 hcs-cli-0.1.44/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.046337 hcs-cli-0.1.44/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.44/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.44/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.44/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-11 08:49:07.327459 hcs-cli-0.1.44/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 08:46:55.000000 hcs-cli-0.1.44/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.048289 hcs-cli-0.1.44/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.44/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.049528 hcs-cli-0.1.44/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.050659 hcs-cli-0.1.44/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.056552 hcs-cli-0.1.44/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.059623 hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.062137 hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.064769 hcs-cli-0.1.44/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.44/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.068410 hcs-cli-0.1.44/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.072290 hcs-cli-0.1.44/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.073408 hcs-cli-0.1.44/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.074446 hcs-cli-0.1.44/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.078529 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.080959 hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.085839 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.090368 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.091476 hcs-cli-0.1.44/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.44/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.093642 hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.094732 hcs-cli-0.1.44/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.099094 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2272 2023-07-07 17:19:46.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/validate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.102834 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4917 2023-07-07 17:46:45.000000 hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.106401 hcs-cli-0.1.44/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.44/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.44/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.44/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.112104 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.44/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.113301 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.119489 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.130802 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.44/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:06.986245 hcs-cli-0.1.44/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.134175 hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.137877 hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.148221 hcs-cli-0.1.44/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.159370 hcs-cli-0.1.44/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1911 2023-07-11 08:31:05.000000 hcs-cli-0.1.44/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1699 2023-07-11 08:31:16.000000 hcs-cli-0.1.44/vhcs/cli/cmds/plan/destroy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.162689 hcs-cli-0.1.44/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.171748 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      976 2023-07-11 08:42:49.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.179510 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.183674 hcs-cli-0.1.44/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.44/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.185166 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.190207 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.44/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.195442 hcs-cli-0.1.44/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.213706 hcs-cli-0.1.44/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.44/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.44/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.44/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.217753 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.44/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.44/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.44/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.44/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.44/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.44/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.44/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.44/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.44/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.44/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.228906 hcs-cli-0.1.44/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.44/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.44/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.44/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.44/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.44/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.44/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.44/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.232121 hcs-cli-0.1.44/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.44/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.238954 hcs-cli-0.1.44/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.44/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    13210 2023-07-11 08:32:49.000000 hcs-cli-0.1.44/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4754 2023-07-11 00:52:21.000000 hcs-cli-0.1.44/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.44/vhcs/plan/helper.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.240843 hcs-cli-0.1.44/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.44/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.250881 hcs-cli-0.1.44/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4432 2023-07-11 02:03:42.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1196 2023-07-11 02:17:50.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1669 2023-07-11 02:11:35.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1181 2023-07-11 01:23:30.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 01:23:47.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-07-11 01:23:57.000000 hcs-cli-0.1.44/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.255704 hcs-cli-0.1.44/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.44/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.44/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.44/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.263432 hcs-cli-0.1.44/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1027 2023-07-11 06:48:15.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1326 2023-07-11 08:39:38.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1212 2023-07-11 01:24:36.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.268516 hcs-cli-0.1.44/vhcs/plan/provider/runtime/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3396 2023-07-11 07:11:55.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/daas_tenant_calculation.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.44/vhcs/plan/provider/runtime/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.270896 hcs-cli-0.1.44/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.44/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.278195 hcs-cli-0.1.44/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.44/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.44/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.44/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.44/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.44/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.44/vhcs/service/admin/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.280697 hcs-cli-0.1.44/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.44/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.44/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.285477 hcs-cli-0.1.44/vhcs/service/ims_catalog/
+-rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.44/vhcs/service/ims_catalog/images.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.288672 hcs-cli-0.1.44/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.44/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.44/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.292171 hcs-cli-0.1.44/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.44/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.44/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.44/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.295575 hcs-cli-0.1.44/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.44/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.44/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.44/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.297745 hcs-cli-0.1.44/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.44/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.44/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.300968 hcs-cli-0.1.44/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-07-11 03:25:14.000000 hcs-cli-0.1.44/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-07-11 08:42:42.000000 hcs-cli-0.1.44/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1236 2023-07-10 08:19:02.000000 hcs-cli-0.1.44/vhcs/service/portal/pool.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.303477 hcs-cli-0.1.44/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.44/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.44/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.305732 hcs-cli-0.1.44/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.44/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.311116 hcs-cli-0.1.44/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.44/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.44/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.44/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.44/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.008191 hcs-cli-0.1.44/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.316880 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-07-11 08:43:59.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      224 2023-07-06 23:02:54.000000 hcs-cli-0.1.44/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.44/vhcs/support/daas/tenant.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.44/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:49:07.323999 hcs-cli-0.1.44/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.44/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.44/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.44/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.43/.gitignore` & `hcs-cli-0.1.44/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/.vscode/launch.json` & `hcs-cli-0.1.44/.vscode/launch.json`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             "name": "hcs plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "nanw.plan.yml", "--sequential", "--resource", "myEntitlement"]
+            "args" : ["plan", "deploy", "-f", "nanw.plan.yml"]
         },
         {
             "name": "hcs destroy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
```

### Comparing `hcs-cli-0.1.43/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.44/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.44/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/GOVERNANCE.md` & `hcs-cli-0.1.44/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/LICENSE` & `hcs-cli-0.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/Makefile` & `hcs-cli-0.1.44/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/PKG-INFO` & `hcs-cli-0.1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.43
+Version: 0.1.44
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.43/README.md` & `hcs-cli-0.1.44/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/doc/az-cheatsheet.md` & `hcs-cli-0.1.44/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/doc/dev-setup.md` & `hcs-cli-0.1.44/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.44/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.44/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/doc/hcs-plan.md` & `hcs-cli-0.1.44/doc/hcs-plan.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.44/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.43
+Version: 0.1.44
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.43/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.44/hcs_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 vhcs/cli/cmds/pki/sign_resource_cert.py
 vhcs/cli/cmds/pki/test.py
 vhcs/cli/cmds/plan/__init__.py
 vhcs/cli/cmds/plan/deploy.py
 vhcs/cli/cmds/plan/destroy.py
 vhcs/cli/cmds/portal/__init__.py
 vhcs/cli/cmds/portal/entitlement/__init__.py
+vhcs/cli/cmds/portal/entitlement/delete.py
 vhcs/cli/cmds/portal/entitlement/get.py
 vhcs/cli/cmds/portal/entitlement/list.py
 vhcs/cli/cmds/portal/pool/__init__.py
 vhcs/cli/cmds/portal/pool/get.py
 vhcs/cli/cmds/portal/pool/list.py
 vhcs/cli/cmds/profile/__init__.py
 vhcs/cli/cmds/profile/init.py
```

### Comparing `hcs-cli-0.1.43/payload/lcm/zero.json` & `hcs-cli-0.1.44/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/pyproject.toml` & `hcs-cli-0.1.44/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/setup.py` & `hcs-cli-0.1.44/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.43"
+VERSION = "0.1.44"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.43/tests/conftest.py` & `hcs-cli-0.1.44/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/tests/test_utils.py` & `hcs-cli-0.1.44/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.44/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.44/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.44/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/__main__.py` & `hcs-cli-0.1.44/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/auth/admin/get_org_idp_map.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/validate.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/infra/validate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/basic.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/inventory/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/inventory/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/plan/deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,31 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import vhcs.plan as plan
 import yaml
+from vhcs.common.ctxp import profile
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=True, help="Specified the combined plan file.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
 def deploy(file, resource: str, parallel: bool):
 
     with file:
         payload = file.read()
     data = yaml.safe_load(payload)
     try:
-        return plan.deploy(data, resource, 10 if parallel else 1)
+        concurrency = 10 if parallel else 1
+        extra = {
+            'profile': profile.current(exclude_secret=True)
+        }
+        return plan.deploy(data, resource, concurrency, extra)
     except (FileNotFoundError, plan.PlanException) as e:
         return str(e), 1
 
 # def _identify_files(file: list[str], name: str):
 #     if not file and not name:
 #         panic("Either --file or --name must be specified")
 #     if file and name:
```

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/plan/destroy.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,28 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import yaml
 import vhcs.plan as plan
+from vhcs.common.ctxp import profile
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=True, help="Specified the combined plan file.")
 @click.option("--force/--fail-fast", type=bool, default=True, required=False, help="Force mode: try deleting everything and continue on error. Fail-fast mode: Stop on the first error.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
 def destroy(file, resource: str, parallel: bool, force: bool):
 
     with file:
         payload = file.read()
     data = yaml.safe_load(payload)
     try:
-        return plan.destroy(data, force, resource, 10 if parallel else 1)
+        concurrency = 10 if parallel else 1
+        extra = {
+            'profile': profile.current(exclude_secret=True)
+        }
+        return plan.destroy(data, force, resource, concurrency, extra)
     except (FileNotFoundError, plan.PlanException) as e:
         return str(e), 1
```

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/portal/pool/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.44/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/cli/main.py` & `hcs-cli-0.1.44/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.44/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,23 +62,30 @@
         raise CtxpException('Profile already exists: ' + to_name)
     data = get(from_name)
     if not data:
         raise CtxpException('Profile does not exist: ' + from_name)
     create(to_name, deepcopy(data), auto_use=False)
 
 
-def current(reload: bool = False, exit_on_failure=True) -> dict:
+def current(reload: bool = False, exit_on_failure=True, exclude_secret: bool = False) -> dict:
     """Get content of the current active profile"""
     profile_name = name()
     data = get(profile_name, reload)
 
     if data is None and exit_on_failure:
         panic(
             "Profile not set. Use 'hcs profile use [profile-name]' to choose one, or use 'hcs profile init' to create default profiles."
         )
+
+    if exclude_secret:
+        data = dotdict(dict(data))
+        csp_config = dict(data['csp'])
+        csp_config['apiToken'] = None
+        csp_config['clientSecret'] = None
+        data['csp'] = csp_config
     return data
 
 def save():
     """Save the current profile"""
     global _data
     if _data != None:
         save_data_file(_data, file(name()))
```

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.44/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/duration.py` & `hcs-cli-0.1.44/vhcs/common/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/logger.py` & `hcs-cli-0.1.44/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.44/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.44/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.44/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.44/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.44/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.44/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/sglib/util.py` & `hcs-cli-0.1.44/vhcs/common/sglib/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/common/util.py` & `hcs-cli-0.1.44/vhcs/common/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.44/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/core.py` & `hcs-cli-0.1.44/vhcs/plan/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,27 +28,28 @@
 from importlib import import_module
 
 import logging
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 def _prepare_data(data: dict, additional_context: dict):
+    if additional_context:
+        common_items = util.get_common_items(additional_context.keys(), data.keys())
+        if common_items:
+            raise PlanException("blueprint and context have conflict keys: " + str(common_items))
+        data.update(additional_context)
     blueprint, pending = helper.process_template(data)
     deployment_id = blueprint['deploymentId']
     state_file = deployment_id + '.state.yml'
     prev = _load_state(state_file)
     state = {'pending': pending}
     state.update(blueprint)
     state.update(prev)
     state['log']['deploy'] = []    # clear log
-    if additional_context:
-        common_items = util.get_common_items(additional_context.keys(), state.keys())
-        if common_items:
-            raise PlanException("blueprint and context have conflict keys: " + str(common_items))
-        state.update(additional_context)
+    
     return blueprint, state, state_file
 
 def deploy(data: dict, resource_name: str = None, concurrency: int = 4, additional_context: dict = None):
     
     blueprint, state, state_file = _prepare_data(data, additional_context)
 
     def process_resource(name: str, res_data: dict):
```

### Comparing `hcs-cli-0.1.43/vhcs/plan/dag.py` & `hcs-cli-0.1.44/vhcs/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/helper.py` & `hcs-cli-0.1.44/vhcs/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/_az_facade.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/_az_facade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/_prepare.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/aad_user.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/nsg.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/resource_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.44/vhcs/plan/provider/azure/subnet.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.44/vhcs/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.44/vhcs/plan/provider/hcs/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.44/vhcs/plan/provider/hcs/launch_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     for u in users:
         horizonId = str(ULID())
         login_hint = u['userPrincipalName']
         launch_items.append({
             'user': u,
             'launchUrl': f"{stackUrl}/appblast/webclient/?horizonId={horizonId}&entitlementId={entitlementId}&domainName={domainName}&action=start-session&login_hint={login_hint}#/desktop"
         })
+        
+    return launch_items
     
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
 def destroy(data: dict, state: dict) -> dict:
     return {}
```

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.44/vhcs/plan/provider/hcs/pool_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/runtime/daas_tenant_calculation.py` & `hcs-cli-0.1.44/vhcs/plan/provider/runtime/daas_tenant_calculation.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/plan/provider/runtime/dummy.py` & `hcs-cli-0.1.44/vhcs/plan/provider/runtime/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/_util.py` & `hcs-cli-0.1.44/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.44/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/admin/edge.py` & `hcs-cli-0.1.44/vhcs/service/admin/edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/admin/helper.py` & `hcs-cli-0.1.44/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/admin/provider.py` & `hcs-cli-0.1.44/vhcs/service/admin/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/admin/template.py` & `hcs-cli-0.1.44/vhcs/service/admin/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/auth/admin.py` & `hcs-cli-0.1.44/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/ims_catalog/helper.py` & `hcs-cli-0.1.44/vhcs/service/ims_catalog/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/ims_catalog/image_copies.py` & `hcs-cli-0.1.44/vhcs/service/ims_catalog/image_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/ims_catalog/images.py` & `hcs-cli-0.1.44/vhcs/service/ims_catalog/images.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.44/vhcs/service/inventory/vm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.44/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/lcm/template.py` & `hcs-cli-0.1.44/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.44/vhcs/service/org_service/datacenter.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/org_service/details.py` & `hcs-cli-0.1.44/vhcs/service/org_service/details.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.44/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/portal/entitlement.py` & `hcs-cli-0.1.44/vhcs/service/portal/entitlement.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 
 def list(**kwargs):
     def _get_page(query_string):
         url = "/v2/entitlements?" + query_string
         return _client.get(url)
     return PageRequest(_get_page, **kwargs).get()
 
-def delete(id: str):
+def delete(id: str, org_id: str):
     url = "/v2/entitlements/" + id
     return _client.delete(url)
```

### Comparing `hcs-cli-0.1.43/vhcs/service/portal/pool.py` & `hcs-cli-0.1.44/vhcs/service/portal/pool.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.44/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/support/daas/helper.py` & `hcs-cli-0.1.44/vhcs/support/daas/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/support/daas/infra.py` & `hcs-cli-0.1.44/vhcs/support/daas/infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.44/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,18 @@
     kind: hcs/entitlement
     data:
       orgId: ${vars.orgId}
       poolIds:
       - ${myPoolGroup.id}
       resourceDetails:
       - poolId: ${myPoolGroup.id}
-      userIds: ${[for u in myAADUser: u.id]}
+      userIds: "${[for u in myAADUser: u.id]}"
 
   myLaunchItem:
     kind: hcs/launch-item
     data:
       users: ${myAADUser}
       entitlementId: ${myPoolGroup.name}
-      domainName: ${myRuntime.orgIdMap.idpTenantDomain}
+      domainName: ${myRuntime.orgIdpMap.idpTenantDomain}
       stackUrl: ${profile.hcs.url}
+    after:
+    - myEntitlement
```

### Comparing `hcs-cli-0.1.43/vhcs/support/daas/tenant.py` & `hcs-cli-0.1.44/vhcs/support/daas/tenant.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/support/profile.py` & `hcs-cli-0.1.44/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/util/check_license.py` & `hcs-cli-0.1.44/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/util/duration.py` & `hcs-cli-0.1.44/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/util/pki_util.py` & `hcs-cli-0.1.44/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/util/query_util.py` & `hcs-cli-0.1.44/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.43/vhcs/util/versions.py` & `hcs-cli-0.1.44/vhcs/util/versions.py`

 * *Files identical despite different names*

