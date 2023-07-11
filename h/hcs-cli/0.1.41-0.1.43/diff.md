# Comparing `tmp/hcs-cli-0.1.41.tar.gz` & `tmp/hcs-cli-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.41.tar", last modified: Wed Jul  5 20:00:57 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.43.tar", last modified: Tue Jul 11 08:16:26 2023, max compression
```

## Comparing `hcs-cli-0.1.41.tar` & `hcs-cli-0.1.43.tar`

### file list

```diff
@@ -1,259 +1,287 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.374784 hcs-cli-0.1.41/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.41/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.041105 hcs-cli-0.1.41/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     2564 2023-07-05 08:21:14.000000 hcs-cli-0.1.41/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)       49 2023-06-30 00:59:55.000000 hcs-cli-0.1.41/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.41/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.41/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.41/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.41/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.41/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-03 19:19:46.000000 hcs-cli-0.1.41/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.41/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     2495 2023-07-05 20:00:57.373960 hcs-cli-0.1.41/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1642 2023-06-24 01:22:59.000000 hcs-cli-0.1.41/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.046884 hcs-cli-0.1.41/doc/
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.41/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.41/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6394 2023-07-03 19:03:00.000000 hcs-cli-0.1.41/doc/hcs-cli-cheatsheet.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.056078 hcs-cli-0.1.41/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2495 2023-07-05 20:00:56.000000 hcs-cli-0.1.41/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     5934 2023-07-05 20:00:56.000000 hcs-cli-0.1.41/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-05 20:00:56.000000 hcs-cli-0.1.41/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-05 20:00:56.000000 hcs-cli-0.1.41/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:00:56.000000 hcs-cli-0.1.41/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-05 20:00:56.000000 hcs-cli-0.1.41/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:56.977017 hcs-cli-0.1.41/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.059711 hcs-cli-0.1.41/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.41/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 19:59:48.000000 hcs-cli-0.1.41/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:00:30.000000 hcs-cli-0.1.41/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-05 20:00:57.375043 hcs-cli-0.1.41/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-05 20:00:53.000000 hcs-cli-0.1.41/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.062991 hcs-cli-0.1.41/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.41/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.066799 hcs-cli-0.1.41/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.068214 hcs-cli-0.1.41/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.074454 hcs-cli-0.1.41/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.079486 hcs-cli-0.1.41/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.082414 hcs-cli-0.1.41/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     6151 2023-07-05 19:50:01.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.41/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.086219 hcs-cli-0.1.41/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.41/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.090159 hcs-cli-0.1.41/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.096833 hcs-cli-0.1.41/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.098125 hcs-cli-0.1.41/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.099519 hcs-cli-0.1.41/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.103862 hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.104976 hcs-cli-0.1.41/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.111234 hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.112978 hcs-cli-0.1.41/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.118075 hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     2335 2023-07-05 08:38:57.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/plan.py
--rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/validate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.130504 hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-05 16:13:46.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1378 2023-07-05 16:11:32.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     4991 2023-07-05 18:15:55.000000 hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.143327 hcs-cli-0.1.41/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.41/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.41/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.41/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.145380 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.161446 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.174640 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6631 2023-07-05 07:47:22.000000 hcs-cli-0.1.41/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:56.989051 hcs-cli-0.1.41/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.184295 hcs-cli-0.1.41/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.41/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.41/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.188157 hcs-cli-0.1.41/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.41/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.41/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.199176 hcs-cli-0.1.41/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.41/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.203989 hcs-cli-0.1.41/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.41/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1745 2023-07-05 16:15:40.000000 hcs-cli-0.1.41/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1328 2023-07-05 16:15:58.000000 hcs-cli-0.1.41/vhcs/cli/cmds/plan/destroy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.207070 hcs-cli-0.1.41/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.41/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.208907 hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.213917 hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.41/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.218597 hcs-cli-0.1.41/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.244524 hcs-cli-0.1.41/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.41/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.41/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.41/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.249202 hcs-cli-0.1.41/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.41/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3977 2023-07-05 08:26:35.000000 hcs-cli-0.1.41/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.41/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.41/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.41/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.41/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.41/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5163 2023-07-05 08:33:15.000000 hcs-cli-0.1.41/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.41/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.41/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6258 2023-07-05 06:26:16.000000 hcs-cli-0.1.41/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.41/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.266393 hcs-cli-0.1.41/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4494 2023-07-05 08:39:50.000000 hcs-cli-0.1.41/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.41/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     4823 2023-07-05 08:20:04.000000 hcs-cli-0.1.41/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     1013 2023-07-05 08:10:55.000000 hcs-cli-0.1.41/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.41/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)     1307 2023-07-05 07:59:02.000000 hcs-cli-0.1.41/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     7955 2023-07-05 06:01:37.000000 hcs-cli-0.1.41/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.272304 hcs-cli-0.1.41/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.41/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.278837 hcs-cli-0.1.41/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.41/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     8453 2023-07-05 19:47:30.000000 hcs-cli-0.1.41/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     3864 2023-07-05 15:51:06.000000 hcs-cli-0.1.41/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     4229 2023-06-30 00:23:11.000000 hcs-cli-0.1.41/vhcs/plan/helper.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.280158 hcs-cli-0.1.41/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.41/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.286271 hcs-cli-0.1.41/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.41/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3071 2023-06-30 01:10:54.000000 hcs-cli-0.1.41/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.41/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1114 2023-06-30 01:27:22.000000 hcs-cli-0.1.41/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)      917 2023-06-29 23:12:33.000000 hcs-cli-0.1.41/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1169 2023-06-30 01:28:00.000000 hcs-cli-0.1.41/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.290316 hcs-cli-0.1.41/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.41/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.41/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1074 2023-07-05 18:09:41.000000 hcs-cli-0.1.41/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.298090 hcs-cli-0.1.41/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.41/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.41/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:23.000000 hcs-cli-0.1.41/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:27.000000 hcs-cli-0.1.41/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:29.000000 hcs-cli-0.1.41/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)      714 2023-06-30 00:56:32.000000 hcs-cli-0.1.41/vhcs/plan/provider/hcs/pool_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.303246 hcs-cli-0.1.41/vhcs/plan/provider/runtime/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.41/vhcs/plan/provider/runtime/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.41/vhcs/plan/provider/runtime/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 08:57:56.000000 hcs-cli-0.1.41/vhcs/plan/provider/runtime/daas_tenant_calculation.py
--rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.41/vhcs/plan/provider/runtime/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.306486 hcs-cli-0.1.41/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.41/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.313743 hcs-cli-0.1.41/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.41/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1184 2023-06-27 20:24:06.000000 hcs-cli-0.1.41/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)      940 2023-06-21 23:40:00.000000 hcs-cli-0.1.41/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.41/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.41/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-06-23 02:28:44.000000 hcs-cli-0.1.41/vhcs/service/admin/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.316176 hcs-cli-0.1.41/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.41/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.41/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.320835 hcs-cli-0.1.41/vhcs/service/ims_catalog/
--rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.41/vhcs/service/ims_catalog/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-06-27 20:17:07.000000 hcs-cli-0.1.41/vhcs/service/ims_catalog/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-22 15:43:13.000000 hcs-cli-0.1.41/vhcs/service/ims_catalog/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.41/vhcs/service/ims_catalog/images.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.326445 hcs-cli-0.1.41/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.41/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.41/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.41/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.329934 hcs-cli-0.1.41/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.41/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.41/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.41/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.336779 hcs-cli-0.1.41/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.41/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.41/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.339443 hcs-cli-0.1.41/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-28 15:59:32.000000 hcs-cli-0.1.41/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      879 2023-06-28 16:01:23.000000 hcs-cli-0.1.41/vhcs/service/portal/pools.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.342181 hcs-cli-0.1.41/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.41/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.41/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.344842 hcs-cli-0.1.41/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.41/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.354012 hcs-cli-0.1.41/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.41/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     8430 2023-07-05 16:09:13.000000 hcs-cli-0.1.41/vhcs/support/daas/deployer.py
--rw-r--r--   0 nanw       (501) staff       (20)     4100 2023-07-05 16:09:49.000000 hcs-cli-0.1.41/vhcs/support/daas/destroyer.py
--rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.41/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1813 2023-06-22 21:16:24.000000 hcs-cli-0.1.41/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.41/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.012862 hcs-cli-0.1.41/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.361077 hcs-cli-0.1.41/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.41/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.41/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-05 18:16:30.000000 hcs-cli-0.1.41/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      240 2023-07-05 18:16:48.000000 hcs-cli-0.1.41/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.41/vhcs/support/daas/tenant.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.41/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 20:00:57.370874 hcs-cli-0.1.41/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.41/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-06-22 01:50:10.000000 hcs-cli-0.1.41/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.41/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.619199 hcs-cli-0.1.43/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.43/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.346150 hcs-cli-0.1.43/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     2599 2023-07-11 06:28:37.000000 hcs-cli-0.1.43/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.43/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.43/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.43/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.43/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.43/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.43/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.43/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.43/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:16:26.618469 hcs-cli-0.1.43/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.43/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.350768 hcs-cli-0.1.43/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.43/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.43/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.43/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.43/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2984 2023-07-11 07:26:34.000000 hcs-cli-0.1.43/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.355760 hcs-cli-0.1.43/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     6644 2023-07-11 08:16:26.000000 hcs-cli-0.1.43/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-11 08:16:25.000000 hcs-cli-0.1.43/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.302491 hcs-cli-0.1.43/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.357048 hcs-cli-0.1.43/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.43/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.43/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.43/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-11 08:16:26.619392 hcs-cli-0.1.43/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 08:16:22.000000 hcs-cli-0.1.43/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.359916 hcs-cli-0.1.43/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.43/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.361964 hcs-cli-0.1.43/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.363293 hcs-cli-0.1.43/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.368590 hcs-cli-0.1.43/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.371116 hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.374162 hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.378533 hcs-cli-0.1.43/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.43/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.383257 hcs-cli-0.1.43/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.388505 hcs-cli-0.1.43/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.389931 hcs-cli-0.1.43/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.391295 hcs-cli-0.1.43/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.395353 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.398004 hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.401722 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.405285 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.406346 hcs-cli-0.1.43/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.43/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.409955 hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.411744 hcs-cli-0.1.43/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.419267 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2272 2023-07-07 17:19:46.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/validate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.423496 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4917 2023-07-07 17:46:45.000000 hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.435818 hcs-cli-0.1.43/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.43/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.43/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.43/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.444487 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.43/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.447979 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.454503 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.463487 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.43/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.313988 hcs-cli-0.1.43/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.465894 hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.468230 hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.474251 hcs-cli-0.1.43/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.478606 hcs-cli-0.1.43/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1745 2023-07-05 16:15:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1533 2023-07-05 20:40:38.000000 hcs-cli-0.1.43/vhcs/cli/cmds/plan/destroy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.480914 hcs-cli-0.1.43/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.484526 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.487980 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.490384 hcs-cli-0.1.43/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.43/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.491859 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.495573 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.43/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.500846 hcs-cli-0.1.43/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.518582 hcs-cli-0.1.43/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.43/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.43/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.43/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.522138 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.43/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.43/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.43/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.43/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.43/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5285 2023-07-06 00:57:57.000000 hcs-cli-0.1.43/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.43/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.43/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.43/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.43/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.532053 hcs-cli-0.1.43/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.43/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.43/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.43/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.43/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.43/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.43/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.43/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.534714 hcs-cli-0.1.43/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.43/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.539135 hcs-cli-0.1.43/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.43/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    13207 2023-07-11 08:05:18.000000 hcs-cli-0.1.43/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4754 2023-07-11 00:52:21.000000 hcs-cli-0.1.43/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.43/vhcs/plan/helper.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.540598 hcs-cli-0.1.43/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.43/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.551422 hcs-cli-0.1.43/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4432 2023-07-11 02:03:42.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1196 2023-07-11 02:17:50.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1669 2023-07-11 02:11:35.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1181 2023-07-11 01:23:30.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 01:23:47.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-07-11 01:23:57.000000 hcs-cli-0.1.43/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.554931 hcs-cli-0.1.43/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.43/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.43/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.43/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.561670 hcs-cli-0.1.43/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1027 2023-07-11 06:48:15.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1293 2023-07-11 07:14:46.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1212 2023-07-11 01:24:36.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.43/vhcs/plan/provider/hcs/pool_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.566512 hcs-cli-0.1.43/vhcs/plan/provider/runtime/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3396 2023-07-11 07:11:55.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/daas_tenant_calculation.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.43/vhcs/plan/provider/runtime/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.568685 hcs-cli-0.1.43/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.43/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.574813 hcs-cli-0.1.43/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.43/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.43/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.43/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.43/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.43/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.43/vhcs/service/admin/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.576816 hcs-cli-0.1.43/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.43/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.43/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.582374 hcs-cli-0.1.43/vhcs/service/ims_catalog/
+-rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.43/vhcs/service/ims_catalog/images.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.584388 hcs-cli-0.1.43/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.43/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.43/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.587817 hcs-cli-0.1.43/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.43/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.43/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.43/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.591294 hcs-cli-0.1.43/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.43/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.43/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.43/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.593499 hcs-cli-0.1.43/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.43/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.43/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.596707 hcs-cli-0.1.43/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-07-11 03:25:14.000000 hcs-cli-0.1.43/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1264 2023-07-11 03:23:26.000000 hcs-cli-0.1.43/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1236 2023-07-10 08:19:02.000000 hcs-cli-0.1.43/vhcs/service/portal/pool.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.598886 hcs-cli-0.1.43/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.43/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.43/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.601103 hcs-cli-0.1.43/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.43/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.606041 hcs-cli-0.1.43/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.43/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.43/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.43/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.43/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.328231 hcs-cli-0.1.43/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.610529 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3610 2023-07-11 07:19:41.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      224 2023-07-06 23:02:54.000000 hcs-cli-0.1.43/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.43/vhcs/support/daas/tenant.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.43/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-11 08:16:26.617338 hcs-cli-0.1.43/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.43/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.43/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.43/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.41/.gitignore` & `hcs-cli-0.1.43/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/.vscode/launch.json` & `hcs-cli-0.1.43/.vscode/launch.json`

 * *Files 6% similar despite different names*

```diff
@@ -9,62 +9,62 @@
             "type": "python",
             "request": "launch",
             "program": "${file}",
             "console": "integratedTerminal",
             "justMyCode": true
         },
         {
-            "name": "hcs login",
+            "name": "hcs login -di",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
-            "justMyCode": false,
+            "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["login"]
+            "args" : ["login", "-di"]
         },
         {
-            "name": "hcs login -di",
+            "name": "hcs tenant plan",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["login", "-di"]
+            "args" : ["daas", "tenant", "plan", "nanw",]
         },
         {
-            "name": "hcs tenant plan",
+            "name": "hcs profile use",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["daas", "tenant", "plan", "nanw",]
+            "args" : ["profile", "use"]
         },
         {
             "name": "hcs plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-n", "nanw"]
+            "args" : ["plan", "deploy", "-f", "nanw.plan.yml", "--sequential", "--resource", "myEntitlement"]
         },
         {
             "name": "hcs destroy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "destroy", "-f", "nanw.vars.yml", "-f", "daas-tenant.blueprint.yml"]
+            "args" : ["plan", "destroy", "-f", "nanw.plan.yml"]
         },
         {
             "name": "hcs admin template list",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
```

### Comparing `hcs-cli-0.1.41/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.43/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.43/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/GOVERNANCE.md` & `hcs-cli-0.1.43/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/LICENSE` & `hcs-cli-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/Makefile` & `hcs-cli-0.1.43/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 buildrelease:
 	python3 setup.py sdist bdist_wheel
 
 uninstall:
 	pip3 uninstall -y hcs-cli
 
 devinstall:
+	pip3 uninstall -y hcs-cli
 	export SCM_REV=$(shell git rev-parse --short HEAD); \
 	pip3 install -e .
 
 dev: clean uninstall lint build devinstall
 
 SHELL := /bin/bash
 test:
```

### Comparing `hcs-cli-0.1.41/PKG-INFO` & `hcs-cli-0.1.43/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.41
+Version: 0.1.43
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: NOTICE
 
 # horizon-cloud-service-cli
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
 
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
@@ -37,27 +38,50 @@
 
 #### Mac & Linux
 
 Install the tool
 ```
 pip3 install hcs-cli
 ```
-Initialize a profile with interactively, with credential. 
+Use with default public HCS service. 
 ```
-hcs profile init
+hcs login
+```
+Run a command, for example, list templates:
+```
+hcs admin template list
 ```
 
-To get a valid token to use with the CLI, refer to doc [Get CSP User API Token](doc/get-csp-user-api-token.md).
+## Authentication Methods
 
+For the first time with each profile, it needs authentication.
+There are three ways to authenticate:
 
-Run a command, for example, list templates:
+| Example                                | Purpose                                |
+|----------------------------------------|----------------------------------------|
+| hcs login                              | Login with configured credentials, otherwise do an interactive login using browser. |
+| hcs login --api-token \<csp-api-token\> | Login with CSP API token. Reference: [Get CSP User API Token](doc/get-csp-user-api-token.md). |
+| hcs login --client-id \<client-id\> --client-secret \<client-secret\> [--org \<org-id\>] | Login with OAuth client id/secret. |
+
+To get the current authentication information:
 ```
-hcs admin template list
+hcs login -d
 ```
 
+## Working with Development Environments
+To work with development environments, first create default profiles:
+```
+hcs profile init --dev
+```
+Switch between profiles:
+```
+hcs profile use
+```
+
+
 ## Documentation
 
 * [HCS CLI Cheatsheet](doc/hcs-cli-cheatsheet.md)
 
 * [Development Setup](doc/dev-setup.md)
 
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
```

### Comparing `hcs-cli-0.1.41/doc/dev-setup.md` & `hcs-cli-0.1.43/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.43/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.43/doc/hcs-cli-cheatsheet.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 | hcs profile init --name \<name\>       | Initialize a profile with a custom name. | 
 | hcs profile list	                     | List existing profiles. |
 | hcs profile get \[name\]	             | Get the current profile, or a specific profile by name. |
 | hcs profile use \<name\>	             | Switch to a profile. |
 | hcs profile delete \<name\>            | Delete a profile. |
 | vi $(hcs profile file)                 | Edit the current profile file directly. |
 | hcs profile file \[name\]              | Show the file path of a profile, current or by name. So you can use the file directly. |
+| hcs profile copy -f \<name1\> -t \<name2\> | Copy a profile. |
 
 ### Login Commands
 
 The login command works with the current profile and will update the current profile. If no token is specified, a browser will be launched to login interactively.
 
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
-| hcs login                              | Interactive login with browser. |
-| hcs login -di                          | Get authentication details. |
-| hcs login --api-token <your-csp-api-token> | Programmatically login with API token. |
-| hcs login --refresh-token <your-csp-api-token> | Programmatically login with OAuth2 refresh token. |
-| hcs login --client-id <client-id> --client-secret <client-secret> | Programmatically login with OAuth client id/secret. |
-| hcs login --bearer <bearer-token> | Programmatically login with bearer token. |
+| hcs login                              | Login with configured credentials, otherwise do an interactive login using browser. |
+| hcs login -d                         | Get authentication details. |
+| hcs login --api-token \<csp-api-token\> | Programmatically login with CSP API token. |
+| hcs login --client-id \<client-id\> --client-secret \<client-secret\> | Programmatically login with OAuth client id/secret. |
 
 
 ### Context Commands
 * Context is a state store backed by disk files. Context is associated with a profile. Different profiles have different contexts. Context is for supporting automation. E.g. the authentication state is cached using context.
 * Context is similar to the environment variable, and context template utility is like the envsubst command. The difference is, context is persisted and can be reused.
 * Context is internally used to support some complex subcommands which has orchestration and has the need to support break-and-resume.
 
@@ -51,25 +50,33 @@
 The CLI framework provides a utility to facilitate template-based processing, with context variables. So in an automation scenario, downstream operations can easily access results from upstream operations, by sharing the states stored in the context.
 
 There are two scenarios:
 
 In side HCS CLI command implementation, context is accessible.
 In a script that uses HCS CLI, the "hcs context" command can be used to access the context values.
 
-Example: WIP
+### Plan Commands
+
+Plan is a resource management engine, which deploy/destroy resources using a blueprint.
+
+| Example                                | Purpose                                |
+|----------------------------------------|----------------------------------------|
+| hcs plan deploy -f \<plan-file-name\>  | Deploy resources according to a plan. |
+| hcs plan destroy -f \<plan-fil-ename\> | Delete all resources related to a plan. |
+
 
 ## Service Commands
 
 ### Admin
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
-| hcs admin edge list | List edges. |
-| hcs admin edge get \<id\> | Get a specific edge by ID. |
+| hcs admin edge list                    | List edges. |
+| hcs admin edge get \<id\>              | Get a specific edge by ID. |
 | hcs admin template list --template-search "providerLocation $eq westus2" | List templates by query. | 
-| hcs admin template get \<id\> | Get a template by ID. |
+| hcs admin template get \<id\>          | Get a template by ID. |
 
 ### VmHub
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
 | hcs vmhub otp request                  |                                        |
 | hcs vmhub otp redeem                   |                                        |
```

### Comparing `hcs-cli-0.1.41/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.43/hcs_cli.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.41
+Version: 0.1.43
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: NOTICE
 
 # horizon-cloud-service-cli
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
 
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
@@ -37,27 +38,50 @@
 
 #### Mac & Linux
 
 Install the tool
 ```
 pip3 install hcs-cli
 ```
-Initialize a profile with interactively, with credential. 
+Use with default public HCS service. 
 ```
-hcs profile init
+hcs login
+```
+Run a command, for example, list templates:
+```
+hcs admin template list
 ```
 
-To get a valid token to use with the CLI, refer to doc [Get CSP User API Token](doc/get-csp-user-api-token.md).
+## Authentication Methods
 
+For the first time with each profile, it needs authentication.
+There are three ways to authenticate:
 
-Run a command, for example, list templates:
+| Example                                | Purpose                                |
+|----------------------------------------|----------------------------------------|
+| hcs login                              | Login with configured credentials, otherwise do an interactive login using browser. |
+| hcs login --api-token \<csp-api-token\> | Login with CSP API token. Reference: [Get CSP User API Token](doc/get-csp-user-api-token.md). |
+| hcs login --client-id \<client-id\> --client-secret \<client-secret\> [--org \<org-id\>] | Login with OAuth client id/secret. |
+
+To get the current authentication information:
 ```
-hcs admin template list
+hcs login -d
 ```
 
+## Working with Development Environments
+To work with development environments, first create default profiles:
+```
+hcs profile init --dev
+```
+Switch between profiles:
+```
+hcs profile use
+```
+
+
 ## Documentation
 
 * [HCS CLI Cheatsheet](doc/hcs-cli-cheatsheet.md)
 
 * [Development Setup](doc/dev-setup.md)
 
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
```

### Comparing `hcs-cli-0.1.41/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.43/hcs_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 mypy.ini
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
 .vscode/launch.json
 .vscode/settings.json
+doc/az-cheatsheet.md
 doc/dev-setup.md
 doc/get-csp-user-api-token.md
 doc/hcs-cli-cheatsheet.md
+doc/hcs-plan.md
 hcs_cli.egg-info/PKG-INFO
 hcs_cli.egg-info/SOURCES.txt
 hcs_cli.egg-info/dependency_links.txt
 hcs_cli.egg-info/entry_points.txt
 hcs_cli.egg-info/requires.txt
 hcs_cli.egg-info/top_level.txt
 payload/lcm/zero.json
@@ -45,31 +47,39 @@
 vhcs/cli/cmds/login.py
 vhcs/cli/cmds/upgrade.py
 vhcs/cli/cmds/admin/__init__.py
 vhcs/cli/cmds/admin/azure-infra/main.py
 vhcs/cli/cmds/admin/edge/__init__.py
 vhcs/cli/cmds/admin/edge/get.py
 vhcs/cli/cmds/admin/edge/list.py
+vhcs/cli/cmds/admin/provider/get.py
 vhcs/cli/cmds/admin/provider/list.py
 vhcs/cli/cmds/admin/template/__init__.py
 vhcs/cli/cmds/admin/template/get.py
 vhcs/cli/cmds/admin/template/list.py
+vhcs/cli/cmds/admin/template/vm/__init__.py
+vhcs/cli/cmds/admin/template/vm/get.py
+vhcs/cli/cmds/admin/template/vm/list.py
+vhcs/cli/cmds/auth/__init__.py
+vhcs/cli/cmds/auth/admin/__init__.py
+vhcs/cli/cmds/auth/admin/get_org_idp_map.py
 vhcs/cli/cmds/daas/__init__.py
 vhcs/cli/cmds/daas/infra/__init__.py
 vhcs/cli/cmds/daas/infra/basic.py
 vhcs/cli/cmds/daas/infra/plan.py
 vhcs/cli/cmds/daas/infra/validate.py
 vhcs/cli/cmds/daas/tenant/__init__.py
 vhcs/cli/cmds/daas/tenant/basic.py
-vhcs/cli/cmds/daas/tenant/deploy.py
-vhcs/cli/cmds/daas/tenant/destroy.py
 vhcs/cli/cmds/daas/tenant/plan.py
 vhcs/cli/cmds/ims/__init__.py
 vhcs/cli/cmds/ims/list.py
 vhcs/cli/cmds/ims/list_copies.py
+vhcs/cli/cmds/inventory/__init__.py
+vhcs/cli/cmds/inventory/get.py
+vhcs/cli/cmds/inventory/list.py
 vhcs/cli/cmds/lcm/__init__.py
 vhcs/cli/cmds/lcm/provider/__init__.py
 vhcs/cli/cmds/lcm/provider/delete.py
 vhcs/cli/cmds/lcm/provider/get.py
 vhcs/cli/cmds/lcm/provider/list.py
 vhcs/cli/cmds/lcm/template/__init__.py
 vhcs/cli/cmds/lcm/template/create.py
@@ -86,14 +96,21 @@
 vhcs/cli/cmds/pki/get_org_cert.py
 vhcs/cli/cmds/pki/get_root_ca.py
 vhcs/cli/cmds/pki/sign_resource_cert.py
 vhcs/cli/cmds/pki/test.py
 vhcs/cli/cmds/plan/__init__.py
 vhcs/cli/cmds/plan/deploy.py
 vhcs/cli/cmds/plan/destroy.py
+vhcs/cli/cmds/portal/__init__.py
+vhcs/cli/cmds/portal/entitlement/__init__.py
+vhcs/cli/cmds/portal/entitlement/get.py
+vhcs/cli/cmds/portal/entitlement/list.py
+vhcs/cli/cmds/portal/pool/__init__.py
+vhcs/cli/cmds/portal/pool/get.py
+vhcs/cli/cmds/portal/pool/list.py
 vhcs/cli/cmds/profile/__init__.py
 vhcs/cli/cmds/profile/init.py
 vhcs/cli/cmds/vmhub/__init__.py
 vhcs/cli/cmds/vmhub/otp/__init__.py
 vhcs/cli/cmds/vmhub/otp/redeem.py
 vhcs/cli/cmds/vmhub/otp/request.py
 vhcs/common/__init__.py
@@ -130,14 +147,16 @@
 vhcs/plan/core.py
 vhcs/plan/dag.py
 vhcs/plan/helper.py
 vhcs/plan/provider/__init__.py
 vhcs/plan/provider/azure/__init__.py
 vhcs/plan/provider/azure/_az_facade.py
 vhcs/plan/provider/azure/_prepare.py
+vhcs/plan/provider/azure/aad_group.py
+vhcs/plan/provider/azure/aad_user.py
 vhcs/plan/provider/azure/nsg.py
 vhcs/plan/provider/azure/resource_group.py
 vhcs/plan/provider/azure/subnet.py
 vhcs/plan/provider/dev/__init__.py
 vhcs/plan/provider/dev/_prepare.py
 vhcs/plan/provider/dev/dummy.py
 vhcs/plan/provider/hcs/__init__.py
@@ -160,31 +179,32 @@
 vhcs/service/admin/template.py
 vhcs/service/auth/__init__.py
 vhcs/service/auth/admin.py
 vhcs/service/ims_catalog/__init__.py
 vhcs/service/ims_catalog/helper.py
 vhcs/service/ims_catalog/image_copies.py
 vhcs/service/ims_catalog/images.py
+vhcs/service/inventory/__init__.py
+vhcs/service/inventory/vm.py
 vhcs/service/lcm/__init__.py
 vhcs/service/lcm/provider.py
 vhcs/service/lcm/template.py
 vhcs/service/org_service/__init__.py
 vhcs/service/org_service/datacenter.py
 vhcs/service/org_service/details.py
 vhcs/service/pki/__init__.py
 vhcs/service/pki/certificate.py
 vhcs/service/portal/__init__.py
-vhcs/service/portal/pools.py
+vhcs/service/portal/entitlement.py
+vhcs/service/portal/pool.py
 vhcs/service/vmhub/__init__.py
 vhcs/service/vmhub/otp.py
 vhcs/support/__init__.py
 vhcs/support/profile.py
 vhcs/support/daas/__init__.py
-vhcs/support/daas/deployer.py
-vhcs/support/daas/destroyer.py
 vhcs/support/daas/helper.py
 vhcs/support/daas/infra.py
 vhcs/support/daas/template.py
 vhcs/support/daas/tenant.py
 vhcs/support/daas/templates/v1/infra.blueprint.yml
 vhcs/support/daas/templates/v1/infra.vars.yml
 vhcs/support/daas/templates/v1/tenant.blueprint.yml
```

### Comparing `hcs-cli-0.1.41/payload/lcm/zero.json` & `hcs-cli-0.1.43/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/pyproject.toml` & `hcs-cli-0.1.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/setup.py` & `hcs-cli-0.1.43/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.41"
+VERSION = "0.1.43"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.41/tests/conftest.py` & `hcs-cli-0.1.43/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/tests/test_utils.py` & `hcs-cli-0.1.43/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.43/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.43/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,75 +14,115 @@
 """
 
 import yaml
 import os
 import re
 import unittest
 from test_utils import CliTest
+from vhcs.common import util
 
 class _blueprints:
     d10_basic = """
 deploymentId: d10
 resources:
-- kind: dev/dummy
-  name: r1
+  r1:
+    kind: dev/dummy
 """
 
     d11_basic_dep = """
 deploymentId: d11
 vars:
     guestName: Alice
 resources:
-- kind: dev/dummy
-  name: r1
-  data:
-    text: ${vars.guestName}
-    delay: 1s
-- kind: dev/dummy
-  name: r2
-  data:
-    text: ${r1.outputText}
+  r1:
+    kind: dev/dummy
+    data:
+        text: ${vars.guestName}
+        delay: 1s
+  r2:
+    kind: dev/dummy
+    data:
+        text: ${r1.outputText}
 """
 
     d12_basic_parallel = """
 deploymentId: d12
 resources:
-- kind: dev/dummy
-  name: r1
-  data:
-    delay: 1s
-- kind: dev/dummy
-  name: r2
+  r1:
+    kind: dev/dummy
+    data:
+        delay: 1s
+  r2:
+    kind: dev/dummy
 """
 
     d13_basic_error_sequential = """
 deploymentId: d13
 resources:
-- kind: dev/dummy
-  name: r1
-  data:
-    error: A simulated error
-- kind: dev/dummy
-  name: r2
-  data:
-    text: ${r1.outputText}
+  r1:
+    kind: dev/dummy
+    data:
+        error: A simulated error
+  r2:
+    kind: dev/dummy
+    data:
+        text: ${r1.outputText}
 """
 
     d14_basic_error_parallel = """
 deploymentId: d14
 resources:
-- kind: dev/dummy
-  name: r1
-  data:
-    error: A simulated error
-    delay: 1s
-- kind: dev/dummy
-  name: r2
+  r1:
+    kind: dev/dummy
+    data:
+        error: A simulated error
+        delay: 1s
+  r2:
+    kind: dev/dummy
 """
 
+    d30_basic_statement_after = """
+deploymentId: d30
+resources:
+  r1:
+    kind: dev/dummy
+    data:
+        delay: 1s
+  r2:
+    kind: dev/dummy
+    after:
+    - r1
+"""
+
+    d40_basic_statement_for = """
+deploymentId: d40
+vars:
+  userEmails:
+    - a@t.com
+    - b@t.com
+resources:
+  r1:
+    kind: dev/dummy
+    for: text in vars.userEmails
+"""
+    d50_list_map_expression = """
+deploymentId: d50
+vars:
+  userEmails:
+    - a@t.com
+    - b@t.com
+resources:
+  r1:
+    kind: dev/dummy
+    for: text in vars.userEmails
+  r2:
+    kind: dev/dummy
+    data:
+      agg: "${[for r in r1: r.outputText]}"
+"""
 class TestPlan(CliTest):
     @classmethod
     def setUpClass(cls):
         _cleanup_states()
 
     @classmethod
     def tearDownClass(cls):
@@ -98,28 +138,54 @@
         self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d11_basic_dep, expected_data='', expect_stderr_empty=False)
         self.verify_execution_log('d11', 'destroy', "r2 must be destroyed before r1", precise_order=['start/r2', 'success/r2', 'start/r1', 'success/r1'])
 
     def test12_basic_parallel(self):
         self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d12_basic_parallel, expected_data='', expect_stderr_empty=False)
         self.verify_execution_log('d12', 'deploy', "success of r2 must before success of r1", partial_order=['success/r2', 'success/r1'])
         self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d12_basic_parallel, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d12', 'deploy', "both r1 and r2 must be destroyed", any_order=['success/r2', 'success/r1'])
+        self.verify_execution_log('d12', 'destroy', "both r1 and r2 must be destroyed", any_order=['success/r2', 'success/r1'])
         
     def test13_basic_error_sequential(self):
         self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d13_basic_error_sequential, expected_data='', expected_return_code=1, expect_stderr_empty=False)
         self.verify_execution_log('d13', 'deploy', "r2 must not be deployed, due to failure in r1", precise_order=['start/r1', 'error/r1'])
         self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d13_basic_error_sequential, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d13', 'destroy', "r2 must not be destroyed, since it's not deployed", precise_order=['start/r1', 'success/r1'])
+        self.verify_execution_log('d13', 'destroy', "r2 must not be destroyed, since it's not deployed", precise_order=['skipped/r2', 'start/r1', 'success/r1'])
 
     def test14_basic_error_parallel(self):
         self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d14_basic_error_parallel, expected_data='', expected_return_code=1, expect_stderr_empty=False)
         self.verify_execution_log('d14', 'deploy', "success of r2 must before error of r1", partial_order=['success/r2', 'error/r1'])
         self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d14_basic_error_parallel, expected_data='', expect_stderr_empty=False)
         self.verify_execution_log('d14', 'destroy', "both r1 and r2 must be cleaned up", any_order=['success/r2', 'success/r1'])
 
+    def test30_basic_statement_after(self):
+        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d30_basic_statement_after, expected_data='', expect_stderr_empty=False)
+        self.verify_execution_log('d30', 'deploy', "r2 must be deployed after r1", precise_order=['start/r1', 'success/r1', 'start/r2', 'success/r2'])
+        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d30_basic_statement_after, expected_data='', expect_stderr_empty=False)
+        self.verify_execution_log('d30', 'destroy', "r2 must be destroyed before r1", precise_order=['start/r2', 'success/r2', 'start/r1', 'success/r1'])
+
+
+    def test40_basic_statement_for(self):
+        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d40_basic_statement_for, expected_data='', expect_stderr_empty=False)
+        self.verify_execution_log('d40', 'deploy', "r1 must be deployed twice", partial_order=['success/r1', 'success/r1'])
+        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d40_basic_statement_for, expected_data='', expect_stderr_empty=False)
+        self.verify_execution_log('d40', 'destroy', "r1 must be destroyed twice", any_order=['success/r1', 'success/r1'])
+
+    def test50_list_map_expression(self):
+        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d50_list_map_expression, expected_data='', expect_stderr_empty=False)
+        self.verify_execution_log('d50', 'deploy', "two r1 instances must be created before r2 start", partial_order=['success/r1', 'success/r1', 'start/r2', 'success/r2'])
+        self.verify_output('d50', "output.r2.agg", ['a@t.com', 'b@t.com'])
+        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d50_list_map_expression, expected_data='', expect_stderr_empty=False)
+        self.verify_execution_log('d50', 'destroy', "two r1 must be deleted after r2", partial_order=['start/r2', 'success/r2', 'start/r1', 'start/r1'])
+
+    def verify_output(self, deployment_id: str, res_path: str, expected_value):
+        with open(f'{deployment_id}.state.yml', 'rt') as file:
+            state = yaml.safe_load(file)
+        v = util.deep_get_attr(state, res_path)
+        self.assertEqual(v, expected_value)
+
     def verify_execution_log(self, deployment_id: str, method: str, description: str, precise_order: list[str] = None, partial_order: list[str] = None, any_order: list[str] = None):
         with open(f'{deployment_id}.state.yml', 'rt') as file:
             state = yaml.safe_load(file)
         exec_logs = state['log'][method]
 
         actual_execution_order = []
         for entry in exec_logs:
```

### Comparing `hcs-cli-0.1.41/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.43/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/__main__.py` & `hcs-cli-0.1.43/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,7 +8,9 @@
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
+help = "Pool commands."
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import questionary
-from typing import Callable
 import vhcs.common.ctxp as ctxp
 from vhcs.common.ctxp import panic, choose
 from vhcs.plan.provider.azure import _az_facade
 from vhcs.support.daas import infra
 from vhcs.service import admin
 
 
@@ -47,15 +45,15 @@
     if len(providers) == 1:
         p = providers[0]
         click.echo("There's only one provider configured, and will be used: " + fn_provider_text(p))
     else:
         p = choose("Select region and provider", providers, fn_provider_text)
         if not p:
             return
-    data['providerInstanceId'] = p['id']
+    data['id'] = p['id']
 
 def _input_azure_sp(data):
     data['applicationId'] = click.prompt("Input Azure service principle application ID:", default=data['applicationId'])
     data['applicationSecret'] = click.prompt("Input Azure service principle application secret:", default=data['applicationSecret'])
 
 def _select_vnet(data):
     vnets = _az_facade.list_vnets()
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/infra/validate.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/infra/validate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/basic.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/deploy.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/get.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import yaml
 import click
-import vhcs.plan as plan
+from vhcs.service.lcm import template
 
-@click.command()
-@click.option("--file", "-f", type=click.File("rt"), required=True, help="The plan file to deploy.")
-def deploy(file):
-    """Deploy a tenant"""
 
-    with file:
-        payload = file.read()
-    data = yaml.safe_load(payload)
-    try:
-        return plan.deploy(data)
-    except (FileNotFoundError, plan.PlanException) as e:
-        return str(e), 1
-    
+@click.command()
+@click.argument("id", type=str, required=True)
+def get(id: str):
+    """Get template by ID"""
+    ret = template.get(id)
+    if ret:
+        return ret
+    return ret, 1
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/destroy.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/provider/get.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,29 +9,21 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import yaml
 import click
-from vhcs.support.daas import destroyer
-from vhcs.common.ctxp import context, panic
+from vhcs.service import admin
+from vhcs.common.sglib.util import option_org_id, get_org_id
 
-@click.command()
-@click.option("--file", "-f", type=str, required=True)
-@click.option("--confirm/--no-confirm", "-c", type=bool, required=False, help="Confirm destroy of the tenant.")
-def destroy(file: str, confirm: bool):
-    """Delete a tenant"""
-
-    if not confirm:
-        panic("The destroy operation will delete all resources allocated for the tenant. Specify additional parameter '--confirm' to proceed.")
-
-    with open(file, "r") as file:
-        payload = file.read()
-    tenant_request = yaml.safe_load(payload)
-    deployment_id = tenant_request['deploymentId']
 
-    print('Destroying tenant:', deployment_id)
-
-    return destroyer.destroy(tenant_request)
+@click.command()
+@click.argument("id", type=str, required=True)
+@click.option("--label", type=str, required=False, default="azure")
+def get(label: str, id: str):
+    """Get template by ID"""
+    ret = admin.provider.get(label, id)
+    if ret:
+        return ret
+    return "", 1
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from vhcs.common import util as data_util
 from vhcs.support.daas import infra, template
 
 
 _surfix = '.plan.yml'
 
 @click.command()
-@click.argument("tenant_id", type=str, required=True)
-def plan(tenant_id: str):
+@click.argument("name", type=str, required=True)
+def plan(name: str):
     """Interactive command to request a DaaS tenant"""
     
-    if tenant_id.endswith(_surfix):
-        tenant_id = tenant_id[:-len(_surfix)]
+    if name.endswith(_surfix):
+        name = name[:-len(_surfix)]
 
-    data = _load_data(tenant_id)
+    data = _load_data(name)
     
     vars = data['vars']
     _config_desktop(vars)
     _input_user_emails(vars)
 
     _save_plan(data)
 
@@ -43,43 +43,41 @@
     deployment_id = vars['deploymentId']
     file_name = _get_file_name(deployment_id)
     blueprint_file = 'v1/tenant.blueprint.yml'
     blueprint = template.get(blueprint_file)
     text = "\n".join([
         yaml.safe_dump(vars, sort_keys=False),
         "",
-        "# ----------------------------------"
+        "# ----------------------------------",
         "# Blueprint: " + blueprint_file,
         "",
         yaml.safe_dump(blueprint, sort_keys=False)
     ])
 
     with open(file_name, "w") as file:
         file.write(text)
 
     print("Plan saved as file: " + file_name)
     print(f"To deploy the plan, use 'hcs plan deploy --file {file_name}'")
 
-def _load_data(tenant_id):
+def _load_data(deployment_id):
 
     data = template.get('v1/tenant.vars.yml')
     if not data['deploymentId']:
-        data['deploymentId'] = tenant_id
+        data['deploymentId'] = deployment_id
     data['vars']['orgId'] = _get_org_id()
 
-    _apply_previous_input(data, tenant_id)
+    _apply_previous_input(data, deployment_id)
 
     # Add defaults from shared infra config, if anything missing
-    data_util.deep_apply_defaults(vars, infra.all())
+    data_util.deep_apply_defaults(data['vars'], infra.all())
 
     return data
 
 def _apply_previous_input(data: dict, tenant_id: str):
-
-
     file_name = _get_file_name(tenant_id)
     prev = data_util.load_data_file(file_name)
     if not prev:
         return
     prev_vars = prev.get('vars')
     if not prev_vars:
         return
@@ -94,15 +92,15 @@
 def _get_file_name(customer_id: str) -> str:
     return customer_id + '.plan.yml'
 
 
 def _config_desktop(data):
 
     def _select_image_and_vm_sku(data):
-        images = ims_catalog.helper.get_images_by_provider_instance_with_asset_details(data['provider']['providerInstanceId'])
+        images = ims_catalog.helper.get_images_by_provider_instance_with_asset_details(data['provider']['id'])
         fn_get_text = lambda d: f"{d['name']}: {d['description']}"
         prev_selected_image = None
         if data['desktop']['streamId']:
             for i in images:
                 if i['id'] == data['desktop']['streamId']:
                     prev_selected_image = i
                     break
@@ -111,27 +109,26 @@
 
         fn_get_text = lambda m: f"{m['name']}"
         selected_marker = choose("Select marker:", selected_image['markers'], fn_get_text)
         data['desktop']['markerId'] = selected_marker['id']
 
         image_asset_details = selected_image['_assetDetails']['data']
 
-        vm_skus = admin.azure_infra.get_compute_vm_skus(data['provider']['providerInstanceId'], search=f"capabilities.HyperVGenerations $in {image_asset_details['generationType']}")
+        search = f"capabilities.HyperVGenerations $in {image_asset_details['generationType']}"
+        vm_skus = admin.azure_infra.get_compute_vm_skus(data['provider']['id'], limit=200, search=search)
         prev_selected_vm_sku = None
         if data['desktop']['vmSkuName']:
             selected_vm_sku_name = data['desktop']['vmSkuName']
         else:
             selected_vm_sku_name = image_asset_details['vmSize']
         if selected_vm_sku_name:
             for sku in vm_skus:
                 if sku['id'] == selected_vm_sku_name:
                     prev_selected_vm_sku = sku
                     break
-        #import json
-        #print(json.dumps(vm_skus, indent=4))
 
         fn_get_text = lambda d: f"{d['data']['name']} (CPU: {d['data']['capabilities']['vCPUs']}, RAM: {d['data']['capabilities']['MemoryGB']})"
 
         selected = choose("Select VM size:", vm_skus, fn_get_text, selected=prev_selected_vm_sku)
         data['desktop']['vmSkuName'] = selected['data']['name']
 
     def _select_desktop_type(data):
@@ -139,8 +136,8 @@
         data['desktop']['templateType'] = choose("Desktop type:", types)
 
 
     _select_image_and_vm_sku(data)
     _select_desktop_type(data)
 
 def _input_user_emails(data):
-    data['userEmails'] = cli_util.input_array("User emails", default=data['userEmails'])
+    data['userEmails'] = cli_util.input_array("User emails", default=data['userEmails'])
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/pki/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,18 +10,13 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.lcm import template
+from vhcs.service.pki import certificate
 
 
-@click.command()
-@click.argument("id", type=str, required=True)
-def get(id: str):
-    """Get template by ID"""
-    ret = template.get(id)
-    if ret:
-        return ret
-    return ret, 1
+@click.command(hidden=True)
+def test():
+    return certificate.test()
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/login.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,119 +39,130 @@
 # 3.2. As a user, I want to get the access token, so I can use it with REST API.
 
 @click.command()
 @click.option("--org", type=str, required=False, help="The CSP organization to login. If not specified, the user's default organization will be used.")
 @click.option("--api-token", type=str, required=False, help="Login with a user CSP API token.")
 @click.option("--client-id", type=str, required=False, help="Login with OAuth client ID/secret.")
 @click.option("--client-secret", type=str, required=False, help="The OAuth client secret, used with --client-id.")
+@click.option("--browser/--auto", type=bool, default=False, help="Login with browser and remove other configured credentials.")
 @click.option("--details/--no-details", "-d", default=False, help="If specified, return the detailed information about the authentication information, otherwise return only the access token.")
 @click.option("--refresh/--no-refresh", "-r", default=False, help="Used only in non-interactive mode. If specified, forcefully refresh the cached access token.")
-@click.option("--info-only/--do-login", "-i", default=False, help="In info-only mode, only display the auth token and avoid login, if the token is not expired.")
-def login(org: str, api_token: str, client_id: str, client_secret: str, details: bool, refresh: bool, info_only: bool):
+def login(org: str, api_token: str, client_id: str, client_secret: str, browser: bool, details: bool, refresh: bool):
     """Login Horizon Cloud Service. 
     
     This command works with the current profile and will update the current profile. If no token is specified, a browser will be launched to login interactively.
 
     \b
     Examples:
-        1. Interactive login using browser:
+        1. Login with configured credentials, otherwise do an interactive login using browser:
             hcs login
-        2. Get login details
-            hcs login -di
-        3. Get access token only
-            hcs login -i
-        4. Login with CSP user API token:
+        2. Get login details:
+            hcs login -d
+        3. Login with CSP user API token:
             hcs login --api-token <your-csp-user-api-token>
-        5. Login with OAuth client id/secret:
+        4. Login with OAuth client id/secret:
             hcs login --client-id <oauth-client-id> --client-secret <oauth-client-secret>
     """
 
     current_profile = _ensure_current_profile()
     csp = current_profile.csp
 
-    err = _validate_auth_method(org=org, api_token=api_token, client_id=client_id, client_secret=client_secret, csp_url=csp.url)
+    err = _validate_auth_method(org=org, api_token=api_token, client_id=client_id, client_secret=client_secret, browser=browser)
     if err:
         return err
     
     # if org is specified
     if org:
         # update the profile
         csp.orgId = org
     else:   # no org id is specified.
         # try using the org_id from profile
         org = csp.orgId
 
-    org_text = org if org else '<default>'
 
     if api_token:
-        _clear_existing_auth(csp)
+        _clear_credentials(csp)
         csp.apiToken = api_token
-        interactive = False
     elif client_id:
-        _clear_existing_auth(csp)
+        _clear_credentials(csp)
         csp.clientId = client_id
         csp.clientSecret = client_secret
-        interactive = False
+    elif browser:
+        _clear_credentials(csp)
     else:
-        interactive = True
+        # auto detect mode.
+        pass
 
-    if info_only or not interactive:
-        oauth_token = sglib.auth.login(force_refresh=refresh)
-        if not oauth_token:
-            return ctxp.error("Login failed")
-    else:
-        def _echo(msg):
-            click.echo(click.style(msg, fg='yellow'), err=True)
-        _echo(f"Logging to HCS...")
-        _echo(f"  CSP:          {csp.url}")
-        _echo(f"  Organization: {org_text}")
-        _echo(f"  Profile:      {ctxp.profile.name()}")
-        _echo(f"A web browser has been opened at {csp.url}. Continue the login in the web browser, and return to this terminal.")
-        oauth_token = login_support.login_via_browser(csp.url, org)
+    interactive = not csp.apiToken and not csp.clientId
+
+    # If this is interactive login, it's not ready on production yet. Raise error
+    if interactive and not login_support.identify_client_id(csp.url):
+        return ctxp.error(f"The interactive login on the specified stack is not yet available. Try a different authentication method.")
+
+    oauth_token = sglib.auth.login(force_refresh=refresh)
+    if not oauth_token:
+        if interactive:
+            oauth_token = _do_browser_login()
+            if oauth_token:
+                sglib.auth.use_oauth_token(oauth_token)
         if not oauth_token:
             return ctxp.error("Login failed")
-        sglib.auth.use_oauth_token(oauth_token)            
-        _clear_existing_auth(csp)
+    # else: the token still works
+    
+    ctxp.profile.save()
 
     auth_details = sglib.auth.details(get_org_details=details)
     if csp.orgId and auth_details.org.id != csp.orgId:
         return ctxp.error("Org ID does not match config. This should be a regression bug in the CLI.")
 
-    ctxp.profile.save()
 
     return auth_details if details else oauth_token['access_token']
 
+def _do_browser_login():
+    csp_config = ctxp.profile.current().csp
+    org_id = csp_config.orgId
+    def _echo(msg):
+        click.echo(click.style(msg, fg='yellow'), err=True)
+    _echo(f"Logging to HCS...")
+    _echo(f"  CSP:          {csp_config.url}")
+    _echo(f"  Organization: {org_id if org_id else '<default>'}")
+    _echo(f"  Profile:      {ctxp.profile.name()}")
+    _echo(f"A web browser has been opened at {csp_config.url}. Continue the login in the web browser, and return to this terminal.")
+    return login_support.login_via_browser(csp_config.url, org_id)
+
+
 def _ensure_current_profile():
     profile = ctxp.profile
     data = profile.current(exit_on_failure = False)
     if not data:
         profile_support.ensure_default_production_profile()
     return profile.current()
 
-def _clear_existing_auth(csp):
+def _clear_credentials(csp):
     csp.apiToken = None
     csp.clientId = None
     csp.clientSecret = None
 
-def _validate_auth_method(org: str, api_token: str, client_id: str, client_secret: str, csp_url: str):
+def _validate_auth_method(org: str, api_token: str, client_id: str, client_secret: str, browser: bool):
 
     # validation: API-token and org ID must not be specified together
     if org and api_token:
-        return "Invalid arguments. CSP API user token is org-scoped. --org can not be used together with --api-token", 1
+        return "Invalid arguments. CSP API user token is org-scoped. --org is not needed with --api-token.", 1
 
     # validation: must not specify duplicated auth methods
     ret = {}
     if api_token:
-        ret['api_token'] = api_token
+        ret['api_token'] = 1
     if client_id:
-        ret['client_id'] = client_id
+        ret['client_id/secret'] = 1
+    if browser:
+        ret['browser'] = 1
     
     if len(ret) > 1:
-        return ctxp.error(f"Specify only one authenticate method. Currently specified: {ret.keys()}")
+        return ctxp.error(f"Specify only one authenticate method. Currently specified: {list(ret.keys())}")
 
+    if client_id and not client_secret or not client_id and client_secret:
+        return ctxp.error("--client-id and --client-secret must be used in pair.")
+    
     if client_id and not client_secret:
         return ctxp.error(f"Missing --client-secret, when --client-id is specified.")
-    
-    # If this is interactive login, it's not ready on production yet. Raise error
-    if not login_support.identify_client_id(csp_url):
-        return ctxp.error(f"The interactive login on the specified stack is not yet available. Try a different authentication method.")
-
+
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.pki import certificate
+from vhcs.service import portal
+from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
-@click.command(hidden=True)
-def test():
-    return certificate.test()
+@click.command()
+@option_org_id
+def list(org: str, **kwargs):
+    """List entitlements"""
+    return portal.entitlement.list(org_id=get_org_id(org), **kwargs)
+
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/plan/deploy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/plan/destroy.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import click
 import yaml
 import vhcs.plan as plan
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=True, help="Specified the combined plan file.")
+@click.option("--force/--fail-fast", type=bool, default=True, required=False, help="Force mode: try deleting everything and continue on error. Fail-fast mode: Stop on the first error.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-def destroy(file, resource: str, parallel: bool):
-
+def destroy(file, resource: str, parallel: bool, force: bool):
 
     with file:
         payload = file.read()
     data = yaml.safe_load(payload)
     try:
-        return plan.destroy(data, resource, 10 if parallel else 1)
+        return plan.destroy(data, force, resource, 10 if parallel else 1)
     except (FileNotFoundError, plan.PlanException) as e:
         return str(e), 1
```

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/cli/main.py` & `hcs-cli-0.1.43/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.43/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             if profile.use(ret) == None:
                 panic("No such profile: " + name)
         else:
             # aborted
             return "", 1
     
 @profile_cmd_group.command()
-@click.argument("from-name", required=True)
-@click.argument("to-name", required=True)
+@click.option("--from-name", "-f", required=True)
+@click.option("--to-name", "-t", required=True)
 def copy(from_name: str, to_name: str):
     """Copy profile."""
     
     data = profile.get(from_name)
     if not data:
         panic("No such profile: " + from_name)
     if profile.exists(to_name):
```

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         save_data_file(_data, file(name()))
 
 def name() -> str:
     """Get the current active profile name"""
     global _active_profile_name
     if not _active_profile_name:
         _active_profile_name = state.get('active_profile', default='default')
+        if not exists(_active_profile_name):
+            _set_active_profile_name('default')
     return _active_profile_name
 
 
 def use(name: str) -> str:
     """Use to the specified profile"""
 
     profile_exists = name in names()
@@ -100,15 +102,17 @@
 
     _set_active_profile_name(name)
     return name
 
 
 def names() -> list[str]:
     """List profile names"""
-    return [f for f in os.listdir(_repo_path) if os.path.isdir(os.path.join(_repo_path, f))]
+    ret = [f for f in os.listdir(_repo_path) if os.path.isdir(os.path.join(_repo_path, f))]
+    ret.sort()
+    return ret
 
 
 def delete(profile_name: str = None) -> None:
     """Delete a profile"""
 
     if profile_name is None:
         profile_name = name()
```

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,21 @@
             return items[i]
     raise Exception("This is a bug and should not happen")
 
 def input_array(prompt: str, default: list[str] = None):
     default_value = ",".join(default) if default else None
     
     input_value = click.prompt(prompt, default_value)
-    return input_value.split(",") if input_value else []
+    if not input_value:
+        return []
+    parts = input_value.split(",")
+    ret = []
+    for p in parts:
+        ret.append(p.strip())
+    return ret
 
 option_verbose = click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
     help="Print debug logs",
```

### Comparing `hcs-cli-0.1.41/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.43/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/duration.py` & `hcs-cli-0.1.43/vhcs/common/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/logger.py` & `hcs-cli-0.1.43/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.43/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.43/vhcs/common/sglib/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 from vhcs.common.ctxp import profile, context, panic, jsondot
 from .csp import CspClient
 from .login_support import create_oauth_client, refresh_oauth_token
 
 log = logging.getLogger(__name__)
 
 
-def _validate_profile_readiness():
-    csp_config = profile.current().csp
-    if not csp_config:
-        panic(f"Profile property missing: profile.csp. Current profile: {profile.name()}")
-    if csp_config.apiToken:
-        return
-    if csp_config.clientId and csp_config.clientSecret:
-        return
+# def _validate_profile_readiness():
+#     csp_config = profile.current().csp
+#     if not csp_config:
+#         panic(f"Profile property missing: profile.csp. Current profile: {profile.name()}")
+#     if csp_config.apiToken:
+#         return
+#     if csp_config.clientId and csp_config.clientSecret:
+#         return
     
-    # This could be interactive login.
-    # Check existance of the previous login.
-    if _get_auth_data():
-        return
+#     # This could be interactive login.
+#     # Check existance of the previous login.
+#     if _get_auth_data():
+#         return
     
-    panic(
-        f"Profile not ready. Perform an interactive login using 'hcs login', or use 'hcs profile edit' to update profile.csp.apiToken or profile.csp.clientId/clientSecret. Current profile: {profile.name()}"
-    )
+#     panic(
+#         f"Profile not ready. Perform an interactive login using 'hcs login', or use 'hcs profile edit' to update profile.csp.apiToken or profile.csp.clientId/clientSecret. Current profile: {profile.name()}"
+#     )
 
 
 def _get_profile_auth_hash():
     csp = profile.current().csp
     text = json.dumps(csp, default=vars)
     return profile.name() + '#' + hashlib.md5(text.encode("ascii")).hexdigest()
 
@@ -65,20 +65,21 @@
 def _get_auth_data():
     return context.get(".auth", default=dict())
 
 
 def login(force_refresh: bool = False):
     """Ensure login state, using credentials from the current profile. Return oauth token."""
 
-    _validate_profile_readiness()
+    # _validate_profile_readiness()
 
     auth_data = _get_auth_data()
     if force_refresh or not _is_auth_valid(auth_data):
         oauth_token = _get_new_oauth_token(auth_data.token)
-        use_oauth_token(oauth_token)
+        if oauth_token:
+            use_oauth_token(oauth_token)
     else:
         oauth_token = auth_data.token
     return oauth_token
 
 def _get_new_oauth_token(old_oauth_token):
     csp_config = profile.current().csp
     
@@ -89,18 +90,22 @@
     if csp_config.apiToken:
         oauth_token = csp_client.login_with_api_token(csp_config.apiToken)
     elif csp_config.clientId:
         oauth_token = csp_client.login_with_client_id_and_secret(csp_config.clientId, csp_config.clientSecret, csp_config.orgId)
     else:
         # This should be a config from interactive login. 
         # Use existing oauth_token to refresh.
-        oauth_token = refresh_oauth_token(old_oauth_token, csp_config.url)
+        if old_oauth_token:
+            oauth_token = refresh_oauth_token(old_oauth_token, csp_config.url)
+        else:
+            oauth_token = None
     return oauth_token
 
 def oauth_client():
+    login(False)
     oauth_token = _get_auth_data().token
     csp_url = profile.current().csp.url
     def fn_on_new_oauth_token(token, refresh_token=None, access_token=None):
         use_oauth_token(token)
     return create_oauth_client(oauth_token, csp_url, fn_on_new_oauth_token)
```

### Comparing `hcs-cli-0.1.41/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.43/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.43/vhcs/common/sglib/ez_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,28 +64,28 @@
         text = _try_formatting_json(response.text)
         log.debug(text)
     log.debug("\n")
 
 
 def _parse_resp(resp: httpx.Response):
     if not resp.content:
-        return None
+        return
     content_type = resp.headers["Content-Type"]
     if content_type.startswith("text"):
         return resp.text
     if len(resp.content) > 3:
         try:
             data = resp.json()
             return jsondot.dotify(data)
         except:
             log.info("--- Fail parsing json. Dump content ---")
             log.info(resp.content)
             raise
     else:
-        return None
+        return
 
 def _is_404(e: httpx.HTTPStatusError) -> bool:
     return e.response.status_code == 404
 
 def on404ReturnNone(func):
     try:
         resp = func()
@@ -93,67 +93,75 @@
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 404:
             return None
         raise
 
 
 class EzClient:
-    def __init__(self, base_url: str, oauth_client: OAuth2Client) -> None:
-
+    def __init__(self, base_url: str, oauth_client: OAuth2Client = None, lazy_oauth_client: Callable = None) -> None:
         #self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
-        self._client = oauth_client
-        oauth_client.base_url = base_url
-        oauth_client.timeout = 30
-        request_hooks = oauth_client.event_hooks['request']
-        response_hooks = oauth_client.event_hooks['response']
-        if _log_request not in request_hooks:
-            request_hooks.append(_log_request)
-        if _log_response not in response_hooks:
-            response_hooks.append(_log_response)
-        if _raise_on_4xx_5xx not in response_hooks:
-            response_hooks.append(_raise_on_4xx_5xx)
-
+        self._base_url = base_url
+        self._client_impl = oauth_client
+        self._lazy_oauth_client = lazy_oauth_client
+
+    def _client(self):
+        if not self._client_impl:
+            client = self._lazy_oauth_client()
+            client.base_url = self._base_url
+            client.timeout = 30
+            request_hooks = client.event_hooks['request']
+            response_hooks = client.event_hooks['response']
+            if _log_request not in request_hooks:
+                request_hooks.append(_log_request)
+            if _log_response not in response_hooks:
+                response_hooks.append(_log_response)
+            if _raise_on_4xx_5xx not in response_hooks:
+                response_hooks.append(_raise_on_4xx_5xx)
+            self._client_impl = client
+        return self._client_impl
+    
     def post(self, url: str, json: dict = None, text: str = None, headers: dict = None):
         if text:
-            resp = self._client.post(url, content=text, headers=headers)
+            resp = self._client().post(url, content=text, headers=headers)
         else:
-            resp = self._client.post(url, json=json)
+            resp = self._client().post(url, json=json)
         return _parse_resp(resp)
 
     def get(self, url: str, raise_on_404: bool = False):
         try:
-            resp = self._client.get(url)
+            resp = self._client().get(url)
             return _parse_resp(resp)
         except httpx.HTTPStatusError as e:
             if _is_404(e):
                 if raise_on_404:
                     raise e
                 else:
                     pass
             else:
                 raise
 
     def patch(self, url: str, json: dict):
-        resp = self._client.patch(url, json=json)
+        resp = self._client().patch(url, json=json)
         return _parse_resp(resp)
 
     def delete(self, url: str, raise_on_404: bool = False):
         try:
-            return self._client.delete(url)
+            resp = self._client().delete(url)
+            return _parse_resp(resp)
         except httpx.HTTPStatusError as e:
             if _is_404(e):
                 if raise_on_404: 
                     raise
                 else:
                     pass
             else:
                 raise
 
     def put(self, url: str, json: dict):
-        resp = self._client.put(url, json=json)
+        resp = self._client().put(url, json=json)
         return _parse_resp(resp)
 
     def close(self):
-        self._client.close()
+        self._client().close()
 
     def dump_response(self, response: HTTPResponse):
         log.info("response text: " + response.text())
```

### Comparing `hcs-cli-0.1.41/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.43/vhcs/service/ims_catalog/image_copies.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,23 +9,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.common.ctxp import profile
-from .ez_client import EzClient
-from . import auth as auth
+from .._util import hdc_service_client
+from vhcs.util.query_util import PageRequest
 
-_oauth_client = None
+_client = hdc_service_client("ims-catalog")
 
-def hcs_client(url: str) -> EzClient:
-    if not url:
-        url = profile.current().hcs.url
-    if url.endswith("/"):
-        url = url[:-1]
 
-    global _oauth_client
-    if not _oauth_client:
-        _oauth_client = auth.oauth_client()
-    return EzClient(url, oauth_client = _oauth_client)
+def list(**kwargs):
+    def _get_page(query_string):
+        url = f"/v1/image-copies?{query_string}"
+        return _client.get(url)
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.41/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.43/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/common/util.py` & `hcs-cli-0.1.43/vhcs/common/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from os import path
-from typing import Tuple
+from typing import Tuple, Any
 import json
 import yaml
 import re
 
 def load_data(file_name: str, class_type: str):
     data = load_data_file(file_name)
     if data == None:
@@ -17,20 +17,21 @@
     with open(file_name, encoding='utf-8') as file:
         text = file.read()
 
     _, ext = path.splitext(file_name)
     if ext == ".json" or format == 'json':
         if format != 'auto' and format != 'json':
             raise Exception(f'File extension does not match specified format. File={file_name}, format={format}')
-        return json.loads(text)
+        data = json.loads(text)
+        return default if data == None else data    # handle empty file
     if ext == ".yaml" or ext == ".yml" or format == 'yml' or format == 'yaml':
         if format != 'auto' and format != 'yaml' and format != 'yml':
             raise Exception(f'File extension does not match specified format. File={file_name}, format={format}')
-        return yaml.safe_load(text)
-    
+        data = yaml.safe_load(text)
+        return default if data == None else data    # handle empty file
     return text
 
 def save_data_file(data: dict | list, file_name: str, format: str = 'yaml'):
     with open(file_name, "w") as file:
         if format == 'yaml':
             # TODO
             #yaml.safe_dump(data, file, sort_keys=False)
@@ -170,17 +171,23 @@
             deep_iterate(v, fn_on_value)
     else:
         fn_on_value(obj)
 
 def deep_find_variables(obj):
     collector = set()
     def fn_on_value(v):
+        if not v or not isinstance(v, str):
+            return
         m = _pattern_var.match(v)
         if m:
-            collector.add(m.group(1))
+            m2 = _pattern_var_list.match(v)
+            if m2:
+                collector.add(m2.group(2))
+            else:
+                collector.add(m.group(1))
     deep_iterate(obj, fn_on_value)
     return collector
 
 def process_variables(obj: dict, fn_get_var = None):
     if fn_get_var == None:
         def _fn_get_var(name):
             try:
@@ -197,46 +204,82 @@
             return {
                 'data': ret['data'],
                 'changed': total_changed,
                 'pending': ret['pending'],
             }
 
 _pattern_var = re.compile('.*?\$\{(.+?)\}.*')
+_pattern_var_list = re.compile('\$\{\s*\[\s*for\s+(.+?)\s+in\s+(.+?)\s*\:\s*(.+)\s*]\s*\}')
 def _process_variables_impl(obj: dict, fn_get_var = None):
     changed = {}
     pending = {}
 
     def fn_change(path, v):
-        if not isinstance(v, str):
-            return v
-        
-        m = _pattern_var.match(v)
-        if not m:
-            return v
-        var_name = m.group(1)
-        replacement, found = fn_get_var(var_name)
-        if not found:
-            pending[path] = var_name
-            return v
-        if isinstance(replacement, str):
-            changed[path] = var_name
-            return v.replace('${' + var_name + '}', replacement)
-        # replacement is an object. Make sure this var is the entire value.
-        if len(v) != len(var_name) + 3:
-            raise Exception(f"Invalid replacing variable with object. attr_path={path}, var_name={var_name}, replacement={str(replacement)}")
-        changed[path] = var_name
-        return replacement  #replace the entire value using the new value.
-    
+        resolved, pending_var = resolve_expression(v, fn_get_var)
+        if pending_var:
+            pending[path] = pending_var
+        elif resolved != v:
+            changed[path] = v
+        return resolved
+
     data = deep_update_object_value(obj, fn_change)
     return {
         'changed': changed,
         'pending': pending,
         'data': data
     }
 
+def resolve_expression(expr, fn_get_value) -> Tuple[Any, str]:
+    """Try resolving expression. Returned updated value and None, or value and pending var name"""
+    
+    if not isinstance(expr, str):
+        return expr, None
+    # get variable names from expr
+    m1 = _pattern_var.match(expr)
+    if not m1:
+        return expr, None
+    m2 = _pattern_var_list.match(expr)
+    if m2:
+        # expression match
+        tmp_var_name = m2.group(1)
+        src_var_name = m2.group(2)
+        mapped_value = m2.group(3)
+
+        target_value, found = fn_get_value(src_var_name)
+        if not found:
+            return expr, src_var_name
+        if not isinstance(target_value, list):
+            raise Exception(f"Invalid variable value for expression. Expect list, actual {type(replacement).__name__}. attr_path={path}, src_var_name={src_var_name}")
+        if not mapped_value.startswith(tmp_var_name + '.'):
+            raise Exception(f"Unsupported expression. attr_path={path}, src_var_name={src_var_name}")
+        new_attr_path = mapped_value[len(tmp_var_name) + 1:]
+        ret = []
+        for i in target_value:
+            item = deep_get_attr(i, new_attr_path)
+            ret.append(item)
+        return ret, None  #replace the entire value using the new value.
+    else:
+        var_name = m1.group(1)
+        # string replacement
+        actual_value, found = fn_get_value(var_name)
+        if not found:
+            return expr, var_name
+        if isinstance(actual_value, str):
+            return expr.replace('${' + var_name + '}', actual_value), None
+        # replacement is an object. Make sure this var is the entire value.
+        if len(expr) != len(var_name) + 3:
+            raise Exception(f"Invalid replacing variable with object. attr_path={attr_path}, var_name={var_name}, replacement={str(value)}")
+        return actual_value, None
+        
 def to_json(o) -> str:
     class SetEncoder(json.JSONEncoder):
         def default(self, obj):
             if isinstance(obj, set):
                 return list(obj)
             return json.JSONEncoder.default(self, obj)
-    return json.dumps(o, cls=SetEncoder, indent=4)
+    return json.dumps(o, cls=SetEncoder, indent=4)
+
+def get_common_items(iter1, iter2):
+    set1 = set(iter1)
+    set2 = set(iter2)
+    common_items = set1.intersection(set2)
+    return common_items
```

### Comparing `hcs-cli-0.1.41/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.43/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/plan/dag.py` & `hcs-cli-0.1.43/vhcs/plan/dag.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,37 +37,61 @@
 
 
     def validate(self):
         all_keys = self.data.keys()
         for k, v in self.graph.items():
             for d in v:
                 if d not in all_keys:
-                    raise Exception(f"Target dpendency not found: from={k}, target={d}")
+                    raise Exception(f"Blueprint error: target dpendency not found: from={k}, target={d}")
     
 def process_blueprint(blueprint, fn_process_node: Callable, concurrency: int = 3):
     dag = _build_graph(blueprint)
     return _walkthrough(dag, fn_process_node, concurrency)
 
+def reverse_traverse(blueprint, fn_process_node):
+    # TODO: this is sequential so far
+    dag = _build_graph(blueprint)
+    dag.validate()
+
+    topological_sorter = TopologicalSorter(dag.graph)
+    sequence = list(topological_sorter.static_order())
+    sequence.reverse()
+
+    for node_name in sequence:
+        stop = fn_process_node(node_name, dag.data[node_name])
+        if stop == True:
+            break
+
 def _build_graph(blueprint):
     dag = DAG()
 
     def add_node(name, obj):
         data = obj.get('data')
         dependencies = set()
         if data:
             variables = util.deep_find_variables(data)
             for v in variables:
-                dependencies.add(v[:v.index('.')])
+                i = v.find('.')
+                resource_name = v if i < 0 else v[:i]
+                dependencies.add(resource_name)
         after = obj.get('after')
         if after:
-            dependencies |= after
+            def _add(t):
+                if t in dependencies:
+                    raise Exception("Invalid blueprint: statement after contains a dependency that is already implicitly created. This is not necessary. Key: " + t)
+                dependencies.add(t)
+            if isinstance(after, str):
+                _add(after)
+            else:
+                for v in after:
+                    _add(v)
         dag.add(name, obj, dependencies)
     
-    for r in blueprint['resources']:
-        add_node(r['name'], r)
+    for k,v in blueprint['resources'].items():
+        add_node(k, v)
     defaults = blueprint.get('defaults')
     if defaults:
         add_node('defaults', defaults)
     providers = blueprint.get('providers')
     if providers:
         for p in providers:
             add_node(p['type'], p)
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/helper.py` & `hcs-cli-0.1.43/vhcs/plan/helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -47,51 +47,80 @@
     return bp, pending
 
 def _validate_blueprint(blueprint: dict):
     _validate_resource_id_no_dup(blueprint)
     _validate_resource_id_not_conflict_to_reserved_names(blueprint)
     _validate_resource_id_not_conflict_to_provider_types(blueprint)
     _validate_no_duplicate_provider_config(blueprint)
+    _validate_statement_after(blueprint)
+
+def _get_duplicates(lst):
+    return [item for item in set(lst) if lst.count(item) > 1]
+
+def _validate_statement_after(blueprint: dict):
+
+    def _raise(owner, reason):
+        raise PlanException(f"Invalid statement: after. Owner={owner}, reason={reason}.")
+    
+    def _validate_after(target_name, owner_resource_name):
+        if not isinstance(target_name, str):
+            _raise(owner_resource_name, f"Invalid value type: {type(target_name).__name__}")
+    
+        if target_name not in blueprint['resources']:
+            _raise(owner_resource_name, "Target not found: " + target_name)
+
+    for k, v in blueprint['resources'].items():
+        after = v.get('after')
+        if after:
+            if isinstance(after, list):
+                for a in after:
+                    _validate_after(a, k)
+
+                dup = _get_duplicates(after)
+                if dup:
+                    _raise(k, 'Duplicated keys: ' + dup)
+            elif isinstance(after, str):
+                _validate_after(after, k)
+            else:
+                _raise(k, "Invalid type, expect str or list, got: " + type(after).__name__)
 
 def _validate_no_duplicate_provider_config(blueprint: dict):
     providers = blueprint.get('providers')
     if not providers:
         return
     known_types = []
     for r in providers:
         t = r['type']
         if t in known_types:
             raise PlanException("Invalid blueprint. Duplicated provider config: " + r['type'])
         known_types.append(t)
 
 def _validate_resource_id_not_conflict_to_provider_types(blueprint: dict):
     provider_names = set()
-    for r in blueprint['resources']:
-        name, _ = r['kind'].split('/')
+    for k, v in blueprint['resources'].items():
+        name, _ = v['kind'].split('/')
         provider_names.add(name)
-    for r in blueprint['resources']:
-        name = r['name']
+    for name in blueprint['resources']:
         if name in provider_names:
             raise PlanException("Invalid blueprint. Invalid resource name due to conflict to provider type. Name: " + name)
         
 def _validate_resource_id_no_dup(blueprint: dict):
     resource_names = set()
-    for r in blueprint['resources']:
-        name = r['name']
+    for name in blueprint['resources']:
         if name in resource_names:
             raise PlanException("Invalid blueprint. Duplicated resource name: " + name)
         resource_names.add(name)
 
 def _validate_resource_id_not_conflict_to_reserved_names(blueprint: dict):
-    reserved_names_for_state = ['output', 'pending']
-    reserved_names_for_blueprint = ['defaults', 'vars', 'providers']
+    reserved_names_for_state = ['result', 'pending', 'log', 'destroy_output']
+    reserved_names_for_blueprint = ['defaults', 'vars', 'providers', 'resources']
+    reserved_names_for_function = ['profile', 'context']
     existing_names_top_level = blueprint.keys()
-    reserved_names = set([*existing_names_top_level, *reserved_names_for_blueprint, *reserved_names_for_state])
-    for r in blueprint['resources']:
-        name = r['name']
+    reserved_names = set([*existing_names_top_level, *reserved_names_for_blueprint, *reserved_names_for_state, *reserved_names_for_function])
+    for name in blueprint['resources']:
         if name in reserved_names:
             raise PlanException("Invalid blueprint. Resource name conflicts to a reserved name: " + name)
 
 def _smart_load_file(file: str):
     if not os.path.exists(file):
         raise Exception("File not found: " + file)
     if not os.path.isfile(file):
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.43/vhcs/plan/provider/azure/_prepare.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.43/vhcs/plan/provider/azure/nsg.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     name = data['name']
     location = data['location']
     resourceGroup = data['resourceGroup']
     tags = data.get('tags')
 
     return az.create_nsg(resourceGroup, name, location, tags)
 
-def destroy(data: dict, prev: dict) -> dict:
-    if prev.get('NewNSG'):
-        id = prev.get('NewNSG')['id']
+def refresh(data: dict, state: dict) -> dict:
+    return state
+
+def destroy(data: dict, state: dict) -> dict:
+    if state.get('NewNSG'):
+        id = state.get('NewNSG')['id']
         return az.delete_nsg_by_id(id)
     name = data['name']
     resourceGroup = data['resourceGroup']
     return az.delete_nsg(name, resourceGroup)
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.43/vhcs/plan/provider/azure/resource_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,10 +17,13 @@
 
 def deploy(data: dict) -> dict:
     name = data['name']
     location = data['location']
     tags = data.get('tags')
     return az.create_resource_group(name, location, tags)
 
-def destroy(data: dict, prev: dict) -> dict:
+def refresh(data: dict, state: dict) -> dict:
+    return state
+
+def destroy(data: dict, state: dict) -> dict:
     name = data['name']
     return az.delete_resource_group(name)
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.43/vhcs/plan/provider/azure/subnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,19 @@
     resourceGroup = data['resourceGroup']
     vNetName = data['vNetName']
     cidr = data['cidr']
     nsgName = data['nsgName']
 
     return az.create_subnet(resourceGroup, vNetName, name, cidr, nsgName)
 
-def destroy(data: dict, prev: dict) -> dict:
-    id = prev.get('id')
+def refresh(data: dict, state: dict) -> dict:
+    return state
+
+def destroy(data: dict, state: dict) -> dict:
+    id = state.get('id')
     if id:
         return az.delete_subnet_by_id(id)
     name = data['name']
     resourceGroup = data['resourceGroup']
     vNetName = data['vNetName']
     az.delete_subnet(resourceGroup, vNetName, name)
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.43/vhcs/plan/provider/dev/dummy.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,29 +10,38 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
+from copy import deepcopy
+from typing import Callable
 import vhcs.common.duration as duration
 from vhcs.plan import PlanException
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, save_state: Callable) -> dict:
 
     text = data.get('text')
     error = data.get('error')
-
     delay = data.get('delay')
+    error_before_save = data.get('error_before_save')
+
     delay_seconds = duration.to_seconds(delay)
     if delay_seconds:
         time.sleep(delay_seconds)
+    ret = deepcopy(data)
+    ret['outputText'] = text
+
+    if not error_before_save:
+        save_state(ret)
 
     if error:
         raise PlanException(error)
-    
-    return {
-        'outputText': text
-    }
+        
+    return ret
+
+def refresh(data: dict, state: dict) -> dict:
+    return state
 
-def destroy(data: dict, prev: dict) -> dict:
+def destroy(data: dict, state: dict) -> dict:
     return {}
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-def deploy(data: dict) -> dict:
-    return {}
-
-def destroy(data: dict, prev: dict) -> dict:
-    return {}
+help = "VM commands."
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-def deploy(data: dict) -> dict:
-    return {}
-
-def destroy(data: dict, prev: dict) -> dict:
-    return {}
+help = "Auth service admin sub-commands."
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-def deploy(data: dict) -> dict:
-    return {}
-
-def destroy(data: dict, prev: dict) -> dict:
-    return {}
+help = "Pool commands."
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.43/vhcs/service/ims_catalog/images.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,12 +9,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-def deploy(data: dict) -> dict:
-    return {'id':'t1'}
+from .._util import hdc_service_client
+from vhcs.util.query_util import PageRequest
 
-def destroy(data: dict, prev: dict) -> dict:
-    return {}
+_client = hdc_service_client("ims-catalog")
+
+
+def list(**kwargs):
+    def _get_page(query_string):
+        url = f"/v1/images?{query_string}"
+        return _client.get(url)
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/runtime/daas_tenant_calculation.py` & `hcs-cli-0.1.43/vhcs/plan/provider/runtime/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/plan/provider/runtime/dummy.py` & `hcs-cli-0.1.43/vhcs/support/daas/helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,44 +8,32 @@
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 import logging
-import vhcs.service.admin as admin
 from vhcs.plan.provider.azure import _az_facade as az
-from vhcs.plan import PlanException
-
-log = logging.getLogger(__name__)
+from vhcs.service import admin
+log = logging.getLogger(__file__)
 
-def deploy(data: dict) -> dict:
-    provider = data['provider']
+def prep_az_cli(tenant_request):
+    provider = tenant_request['provider']
     providerInstanceId = provider['providerInstanceId']
-    log.info('Provider: %s', providerInstanceId)
+    print('Provider:', providerInstanceId)
     providerInstance = admin.provider.get('azure', providerInstanceId)
-    if not providerInstance:
-        raise PlanException('Provider not found: ' + providerInstanceId)
     subscription_id = providerInstance['providerDetails']['data']['subscriptionId']
     directory_id = providerInstance['providerDetails']['data']['directoryId']
     application_id = providerInstance['providerDetails']['data']['applicationId']
     region = providerInstance['providerDetails']['data']['region']
-    log.info('Subscription: %s', subscription_id)
-    log.info('Directory: %s', directory_id)
-    log.info('ApplicationId: %s', application_id)
-    log.info('Region: %s', region)
-
-    return {
-        'location': 'westus2',
-        'cidr': _calculate_cidr(),
-        'vNet': az.get_vnet(data['network']['vNetId']),
-        'providerInstance': providerInstance
-    }
-
-def _calculate_cidr():
-    #TODO
-    cidr = "10.200.1.0/24"
-    return cidr
+    print('Subscription:', subscription_id)
+    print('Directory:', directory_id)
+    print('ApplicationId:', application_id)
+    print('Region:', region)
+    if application_id != provider['applicationId']:
+        log.warning("Configured application ID for CLI does not match application ID for provider.")
+    
+    az.login(provider['applicationId'], provider['applicationSecret'], directory_id)
+    az.set_subscription(subscription_id)
 
-def destroy(data: dict, prev: dict):
-    return
```

### Comparing `hcs-cli-0.1.41/vhcs/service/_util.py` & `hcs-cli-0.1.43/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.43/vhcs/service/admin/azure_infra.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
 
 def get_compute_vm_skus(provider_instance_id: str, **kwargs):
     def _get_page(query_string):
         url = f"/v2/providers/azure/instances/{provider_instance_id}/compute-vm-skus?" + query_string
-        return _client.get(url)
+        ret = _client.get(url)
+        
+        return ret
 
     return PageRequest(_get_page, **kwargs).get()
 
 
 def get_networks(providerInstanceId: str, **kwargs):
     url = f"/v2/providers/azure/instances/{providerInstanceId}/preferences/networks"
     return _client.get(url)
```

### Comparing `hcs-cli-0.1.41/vhcs/service/admin/edge.py` & `hcs-cli-0.1.43/vhcs/service/org_service/details.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("admin")
+_client = hdc_service_client("org-service")
+
 
-@staticmethod
 def get(id: str, **kwargs):
-    url = with_query(f"/v2/edge-deployments/{id}", **kwargs)
+    url = with_query(f"/v1/org-details/{id}", **kwargs)
     return _client.get(url)
 
-@staticmethod
-def list():
-    return _client.get("/v2/edge-deployments")
+def list(**kwargs):
+    def _get_page(query_string):
+        url = "/v1/org-details?" + query_string
+        return _client.get(url)
+
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.41/vhcs/service/admin/helper.py` & `hcs-cli-0.1.43/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/admin/provider.py` & `hcs-cli-0.1.43/vhcs/service/admin/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/admin/template.py` & `hcs-cli-0.1.43/vhcs/service/portal/pool.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,35 +9,32 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import logging
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("admin")
+log = logging.getLogger(__name__)
+_client = hdc_service_client("portal")
 
-def get(id: str, **kwargs):
-    url = with_query(f"/v2/templates/{id}", **kwargs)
+
+def create(payload: dict):
+    url = "/v2/pools"
+    return _client.post(url, payload)
+
+def get(id: str, org_id: str):
+    url = f"/v2/pools/{id}?org_id={org_id}"
     return _client.get(url)
 
 def list(**kwargs):
     def _get_page(query_string):
-        url = "/v2/templates?" + query_string
+        url = "/v2/pools?" + query_string
         return _client.get(url)
-
     return PageRequest(_get_page, **kwargs).get()
 
-def deploy(payload):
-    return _client.post("/v2/templates?ignore_warnings=true", json=payload)
-
-def delete(id: str, force: bool = True):
-    return _client.delete(f"/v2/templates/{id}?force={force}") 
-
-def wait_for_template_deleted(id: str, timeout_seconds: int = 60):
-    print("TODO: wait_for_template_deleted")
-
-
-def wait_for_template_ready(id: str, timeout_seconds: int = 60):
-    print("TODO: wait_for_template_ready")
+def delete(id: str):
+    url = "/v2/pools/" + id
+    return _client.delete(url)
```

### Comparing `hcs-cli-0.1.41/vhcs/service/auth/admin.py` & `hcs-cli-0.1.43/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/ims_catalog/helper.py` & `hcs-cli-0.1.43/vhcs/service/ims_catalog/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/ims_catalog/image_copies.py` & `hcs-cli-0.1.43/vhcs/service/admin/edge.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .._util import hdc_service_client
-from vhcs.util.query_util import PageRequest
+from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("ims-catalog")
+_client = hdc_service_client("admin")
 
+def get(id: str, **kwargs):
+    url = with_query(f"/v2/edge-deployments/{id}", **kwargs)
+    return _client.get(url)
 
 def list(**kwargs):
     def _get_page(query_string):
-        url = f"/v1/image-copies?{query_string}"
+        url = "/v2/edge-deployments?" + query_string
         return _client.get(url)
-    return PageRequest(_get_page, **kwargs).get()
+
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.41/vhcs/service/ims_catalog/images.py` & `hcs-cli-0.1.43/vhcs/service/org_service/datacenter.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .._util import hdc_service_client
-from vhcs.util.query_util import PageRequest
+from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("ims-catalog")
+_client = hdc_service_client("org-service")
 
 
+def get(id: str, **kwargs):
+    url = with_query(f"/v1/datacenters/{id}", **kwargs)
+    return _client.get(url)
+
 def list(**kwargs):
-    def _get_page(query_string):
-        url = f"/v1/images?{query_string}"
-        return _client.get(url)
-    return PageRequest(_get_page, **kwargs).get()
+    url = with_query(f"/v1/datacenters", **kwargs)
+    return _client.get(url)
+
+def find_by_org(orgId, **kwargs):
+    url = with_query(f"/v1/datacenters/orgs/{orgId}", **kwargs)
+    return _client.get(url)
+
```

### Comparing `hcs-cli-0.1.41/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.43/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/lcm/template.py` & `hcs-cli-0.1.43/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/org_service/details.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/inventory/list.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,23 +9,20 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
-from vhcs.util.query_util import with_query, PageRequest
-
-_client = hdc_service_client("org-service")
-
-
-def get(id: str, **kwargs):
-    url = with_query(f"/v1/org-details/{id}", **kwargs)
-    return _client.get(url)
-
-def list(**kwargs):
-    def _get_page(query_string):
-        url = "/v1/org-details?" + query_string
-        return _client.get(url)
-
-    return PageRequest(_get_page, **kwargs).get()
+import click
+from vhcs.service import inventory
+from vhcs.common.sglib.util import option_org_id, get_org_id
+
+@click.command()
+@click.argument("template", type=str, required=True)
+@option_org_id
+def list(template: str, org: str):
+    """List template VMs"""
+    ret = inventory.list(template, get_org_id(org))
+    if ret:
+        return ret
+    return ret, 1
```

### Comparing `hcs-cli-0.1.41/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.43/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/service/portal/pools.py` & `hcs-cli-0.1.43/vhcs/cli/cmds/admin/edge/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import logging
-from .._util import hdc_service_client
-from vhcs.util.query_util import with_query, PageRequest
+import click
+from vhcs.service import admin
+from vhcs.common.sglib.util import option_org_id, get_org_id
 
-log = logging.getLogger(__name__)
-_client = hdc_service_client("portal")
 
+@click.command()
+@option_org_id
+def list(org: str, **kwargs):
+    """List edges"""
+    return admin.edge.list(org_id=get_org_id(org), **kwargs)
 
-def create_pool(payload: dict):
-    url = "/v2/pools"
-    return _client.post(url, payload)
```

### Comparing `hcs-cli-0.1.41/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.43/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/support/daas/infra.py` & `hcs-cli-0.1.43/vhcs/support/daas/infra.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 def _with_default(target : dict, default : dict) -> dict:
     ret = dict(default)
     ret.update(target)
     return ret
 
 _config_template = {
 	"provider": {
-		"providerInstanceId": "",
+		"id": "",
 		"applicationId": "",
 		"applicationSecret": ""
 	},
 	"network": {
 		"vNetId": "",
 		"tenantCIDRs": []
 	},
```

### Comparing `hcs-cli-0.1.41/vhcs/support/daas/tenant.py` & `hcs-cli-0.1.43/vhcs/support/daas/tenant.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/support/profile.py` & `hcs-cli-0.1.43/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/util/check_license.py` & `hcs-cli-0.1.43/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/util/duration.py` & `hcs-cli-0.1.43/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/util/pki_util.py` & `hcs-cli-0.1.43/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.41/vhcs/util/query_util.py` & `hcs-cli-0.1.43/vhcs/util/query_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,39 +25,41 @@
             del obj[k]
     return obj
 
 
 def with_query(url: str, **kwargs: Any) -> str:
     qs = urlencode(_remove_none(dict(kwargs)))
     if qs:
-        url += "?" + qs
+        if url.find('?') < 0:
+            url += '?'
+        url += qs
     return url
 
 
 class PageRequest:
     def __init__(self, fn_get_page: Callable, **kwargs):
         limit = kwargs.get('limit')
         self.limit = int(limit) if limit else 10
         self.fn_get_page = fn_get_page
         self.query = _remove_none(dict(kwargs))
+        if int(self.query.get("size", 0)) < 1:
+            self.query['size'] = 20
+        
 
     def get(self) -> list:
         ret = []
         page_index = 0
 
         while True:
-            page_size = self.limit - len(ret)
-            if page_size < 1:
-                break
-            if page_size > 200:
-                page_size = 200
-            self.query["size"] = page_size
             self.query["page"] = page_index
             
             query_string = urlencode(self.query)
             page = self.fn_get_page(query_string)
             if not page or not page.content:
                 break
             ret += page.content
+            if len(ret) > self.limit:
+                ret = ret[:self.limit]
+                break
             page_index += 1
 
         return ret
```

### Comparing `hcs-cli-0.1.41/vhcs/util/versions.py` & `hcs-cli-0.1.43/vhcs/util/versions.py`

 * *Files identical despite different names*

