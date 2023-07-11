# Comparing `tmp/py4web-1.20230710.1.tar.gz` & `tmp/py4web-1.20230710.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230710.1.tar", last modified: Tue Jul 11 03:59:39 2023, max compression
+gzip compressed data, was "py4web-1.20230710.3.tar", last modified: Tue Jul 11 04:13:33 2023, max compression
```

## Comparing `py4web-1.20230710.1.tar` & `py4web-1.20230710.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.158612 py4web-1.20230710.1/
--rw-r--r--   0 mdp       (1000) mdp       (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230710.1/LICENSE.md
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     7692 2023-07-11 03:59:39.158612 py4web-1.20230710.1/PKG-INFO
--rw-r--r--   0 mdp       (1000) mdp       (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230710.1/README.rst
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.146612 py4web-1.20230710.1/py4web/
--rw-r--r--   0 mdp       (1000) mdp       (1000)      752 2023-07-11 03:58:51.000000 py4web-1.20230710.1/py4web/__init__.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.154612 py4web-1.20230710.1/py4web/assets/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)  2995779 2023-07-11 03:59:32.000000 py4web-1.20230710.1/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 mdp       (1000) mdp       (1000)   187155 2023-07-11 03:59:32.000000 py4web-1.20230710.1/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 mdp       (1000) mdp       (1000)  4356813 2023-07-11 03:59:32.000000 py4web-1.20230710.1/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     5245 2023-07-11 03:59:32.000000 py4web-1.20230710.1/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 mdp       (1000) mdp       (1000)    21524 2023-07-11 03:59:32.000000 py4web-1.20230710.1/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 mdp       (1000) mdp       (1000)  1385465 2023-07-11 03:59:32.000000 py4web-1.20230710.1/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdp       (1000) mdp       (1000)    68251 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/core.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    10117 2023-07-08 16:23:32.000000 py4web-1.20230710.1/py4web/server_adapters.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.158612 py4web-1.20230710.1/py4web/utils/
--rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/__init__.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    69556 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/utils/auth.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.158612 py4web-1.20230710.1/py4web/utils/auth_plugins/
--rw-r--r--   0 mdp       (1000) mdp       (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      513 2023-07-08 16:23:32.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     5082 2023-07-08 16:23:32.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     2849 2023-07-08 16:23:32.000000 py4web-1.20230710.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/cors.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/dbstore.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/downloader.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/factories.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/form.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    69292 2023-07-02 01:47:31.000000 py4web-1.20230710.1/py4web/utils/grid.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1647 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    34928 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/utils/mailer.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/misc.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/param.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/populate.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1692 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/utils/publisher.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     2495 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/utils/recaptcha.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/security.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230710.1/py4web/utils/tags.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     6546 2023-07-08 16:23:33.000000 py4web-1.20230710.1/py4web/utils/url_signer.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.146612 py4web-1.20230710.1/py4web.egg-info/
--rw-r--r--   0 mdp       (1000) mdp       (1000)     7692 2023-07-11 03:59:39.000000 py4web-1.20230710.1/py4web.egg-info/PKG-INFO
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     1847 2023-07-11 03:59:39.000000 py4web-1.20230710.1/py4web.egg-info/SOURCES.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)        1 2023-07-11 03:59:39.000000 py4web-1.20230710.1/py4web.egg-info/dependency_links.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)       43 2023-07-11 03:59:39.000000 py4web-1.20230710.1/py4web.egg-info/entry_points.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)      239 2023-07-11 03:59:39.000000 py4web-1.20230710.1/py4web.egg-info/requires.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)        7 2023-07-11 03:59:39.000000 py4web-1.20230710.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)      843 2023-07-11 03:58:38.000000 py4web-1.20230710.1/pyproject.toml
--rw-rw-r--   0 mdp       (1000) mdp       (1000)      466 2023-05-29 04:13:06.000000 py4web-1.20230710.1/requirements.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)       38 2023-07-11 03:59:39.158612 py4web-1.20230710.1/setup.cfg
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 03:59:39.158612 py4web-1.20230710.1/tests/
--rw-r--r--   0 mdp       (1000) mdp       (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_action.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_auth.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_cache.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_fixture.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_form.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_json.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_main.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_session.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_tags.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_template.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230710.1/tests/test_url.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.198478 py4web-1.20230710.3/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230710.3/LICENSE.md
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     7692 2023-07-11 04:13:33.198478 py4web-1.20230710.3/PKG-INFO
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230710.3/README.rst
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.186478 py4web-1.20230710.3/py4web/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      752 2023-07-11 04:11:53.000000 py4web-1.20230710.3/py4web/__init__.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.194478 py4web-1.20230710.3/py4web/assets/
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)  2995795 2023-07-11 04:13:26.000000 py4web-1.20230710.3/py4web/assets/py4web.app._dashboard.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)   187155 2023-07-11 04:13:26.000000 py4web-1.20230710.3/py4web/assets/py4web.app._default.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)  4356813 2023-07-11 04:13:26.000000 py4web-1.20230710.3/py4web/assets/py4web.app._documentation.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     5245 2023-07-11 04:13:26.000000 py4web-1.20230710.3/py4web/assets/py4web.app._minimal.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)    21524 2023-07-11 04:13:26.000000 py4web-1.20230710.3/py4web/assets/py4web.app._scaffold.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)  1385465 2023-07-11 04:13:26.000000 py4web-1.20230710.3/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    68251 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/core.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    10117 2023-07-08 16:23:32.000000 py4web-1.20230710.3/py4web/server_adapters.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.194478 py4web-1.20230710.3/py4web/utils/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/__init__.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    69556 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/utils/auth.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.198478 py4web-1.20230710.3/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      513 2023-07-08 16:23:32.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     5082 2023-07-08 16:23:32.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2849 2023-07-08 16:23:32.000000 py4web-1.20230710.3/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/cors.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/dbstore.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/downloader.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/factories.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/form.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    69292 2023-07-02 01:47:31.000000 py4web-1.20230710.3/py4web/utils/grid.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1647 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    34928 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/utils/mailer.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/misc.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/param.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/populate.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1692 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/utils/publisher.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2495 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/security.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230710.3/py4web/utils/tags.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6546 2023-07-08 16:23:33.000000 py4web-1.20230710.3/py4web/utils/url_signer.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.186478 py4web-1.20230710.3/py4web.egg-info/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     7692 2023-07-11 04:13:33.000000 py4web-1.20230710.3/py4web.egg-info/PKG-INFO
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     1847 2023-07-11 04:13:33.000000 py4web-1.20230710.3/py4web.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)        1 2023-07-11 04:13:33.000000 py4web-1.20230710.3/py4web.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)       43 2023-07-11 04:13:33.000000 py4web-1.20230710.3/py4web.egg-info/entry_points.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)      239 2023-07-11 04:13:33.000000 py4web-1.20230710.3/py4web.egg-info/requires.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)        7 2023-07-11 04:13:33.000000 py4web-1.20230710.3/py4web.egg-info/top_level.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)      843 2023-07-11 04:12:44.000000 py4web-1.20230710.3/pyproject.toml
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)      466 2023-05-29 04:13:06.000000 py4web-1.20230710.3/requirements.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)       38 2023-07-11 04:13:33.198478 py4web-1.20230710.3/setup.cfg
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-07-11 04:13:33.198478 py4web-1.20230710.3/tests/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_action.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_auth.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_cache.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_fixture.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_form.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_json.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_main.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_session.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_tags.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_template.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230710.3/tests/test_url.py
```

### Comparing `py4web-1.20230710.1/LICENSE.md` & `py4web-1.20230710.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/PKG-INFO` & `py4web-1.20230710.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230710.1
+Version: 1.20230710.3
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230710.1/README.rst` & `py4web-1.20230710.3/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/__init__.py` & `py4web-1.20230710.3/py4web/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20230710.1"
+__version__ = "1.20230710.3"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app._dashboard.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2995779 bytes, number of entries: 379
+Zip file size: 2995795 bytes, number of entries: 379
 -rw-r--r--  3.0 unx     3751 tx defN 23-May-22 05:34 utils.py
 -rw-r--r--  3.0 unx     8089 tx defN 23-May-08 00:39 static/components/mtable.js
 -rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
--rw-r--r--  3.0 unx    10467 tx defN 23-May-08 00:39 static/js/index.js
+-rw-r--r--  3.0 unx    10462 tx defN 23-Jul-11 04:08 static/js/index.js
 -rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 static/js/ace/ext-themelist.js
 -rw-r--r--  3.0 unx     8367 tx defN 23-May-08 00:39 static/js/ace/mode-prolog.js
 -rw-r--r--  3.0 unx    26620 tx defN 23-May-08 00:39 static/js/ace/mode-lsl.js
 -rw-r--r--  3.0 unx    20332 tx defN 23-May-08 00:39 static/js/ace/mode-gobstones.js
 -rw-r--r--  3.0 unx     2087 tx defN 23-May-08 00:39 static/js/ace/mode-textile.js
 -rw-r--r--  3.0 unx     2585 tx defN 23-May-08 00:39 static/js/ace/theme-textmate.js
 -rw-r--r--  3.0 unx     5712 tx defN 23-May-08 00:39 static/js/ace/mode-logiql.js
@@ -367,15 +367,15 @@
 -rw-r--r--  3.0 unx  1010153 bx defN 23-May-08 00:39 static/images/widget.gif
 -rw-r--r--  3.0 unx    13380 bx defN 23-May-08 00:39 static/images/alert-yellow.gif
 -rw-r--r--  3.0 unx    12025 bx defN 23-May-08 00:39 static/images/alert-red.gif
 -rw-r--r--  3.0 unx    11068 bx defN 23-May-08 00:39 static/images/alert-green.gif
 -rw-r--r--  3.0 unx     7927 bx defN 23-May-08 00:39 static/images/forkme.png
 -rw-r--r--  3.0 unx    13366 bx defN 23-May-08 00:39 static/images/alert-orange.gif
 -rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 translations/README.md
--rw-r--r--  3.0 unx    20612 tx defN 23-May-22 05:34 __init__.py
+-rw-r--r--  3.0 unx    20644 tx defN 23-Jul-11 04:08 __init__.py
 -rw-r--r--  3.0 unx     6493 tx defN 23-May-08 00:39 diff2kryten.py
 -rw-r--r--  3.0 unx     4849 tx defN 23-May-08 00:39 templates/gitlog.html
 -rw-r--r--  3.0 unx     1141 tx defN 23-May-08 00:39 templates/ticket.html
 -rw-r--r--  3.0 unx      993 tx defN 23-May-08 00:39 templates/dbadmin.html
 -rw-r--r--  3.0 unx     2994 tx defN 23-May-08 00:39 templates/translations.html
 -rw-r--r--  3.0 unx    13851 tx defN 23-May-08 00:39 templates/index.html
-379 files, 8019993 bytes uncompressed, 2924821 bytes compressed:  63.5%
+379 files, 8020020 bytes uncompressed, 2924837 bytes compressed:  63.5%
```

#### static/js/index.js

##### js-beautify {}

```diff
@@ -93,15 +93,15 @@
             app.editor.$blockScrolling = Infinity;
             if (!force && path in app.vue.files) {
                 app.activate_editor(path, app.vue.files[path]);
             } else {
                 var url = '../load/' + path;
                 if (app.vue.selected_type != 'text') url = '../load_bytes/' + path;
                 fetch(url).then(r => r.json()).then(r => {
-                    app.activate_editor(path, r.data.payload);
+                    app.activate_editor(path, r.payload);
                 });
             }
         }
         app.vue.selected_filename = path;
     };
     app.modal_dismiss = () => {
         app.vue.modal = null;
```

#### __init__.py

```diff
@@ -59,15 +59,15 @@
                 field.update = make_safe_field(field.update)
 
 
 def run(command, project):
     """for runing git commands inside an app (project)"""
     return subprocess.check_output(
         command.split(), cwd=os.path.join(FOLDER, project)
-    ).decode()
+    ).decode(errors="ignore")
 
 
 def get_commits(project):
     """list of git commits for the project"""
     output = run("git log", project)
     commits = []
     for line in output.split("\n"):
@@ -273,15 +273,15 @@
         return {"payload": store[top], "status": "success"}
 
     @action("load/<path:path>")
     @session_secured
     def load(path):
         """Loads a text file"""
         path = safe_join(FOLDER, path) or abort()
-        content = open(path, "rb").read().decode("utf8")
+        content = open(path, "rb").read().decode("utf8", errors="ignore")
         return {"payload": content, "status": "success"}
 
     @action("load_bytes/<path:path>")
     @session_secured
     def load_bytes(path):
         """Loads a binary file"""
         path = safe_join(FOLDER, path) or abort()
```

### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app._documentation.zip`

 * *Format-specific differences are supported for ZIP archives but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Zip archive data, at least v2.0 to extract, compression method=deflate*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

 * *Files 0% similar despite different names*

```diff
@@ -1521,15 +1521,15 @@
 00005f00: 3207 1e7f 9e18 7201 8781 421f e07f 34c7  2.....r...B...4.
 00005f10: 39f9 b458 2cc2 fe60 ac15 66d2 76ca b459  9..X,..`..f.v..Y
 00005f20: c770 363b 864b 32fb 0b50 4b03 0414 0000  .p6;.K2..PK.....
 00005f30: 0008 0075 95a7 566b 3525 4804 0700 0068  ...u..Vk5%H....h
 00005f40: 1200 0025 001c 0073 7461 7469 632f 656e  ...%...static/en
 00005f50: 2f5f 7374 6174 6963 2f73 7068 696e 785f  /_static/sphinx_
 00005f60: 6869 6768 6c69 6768 742e 6a73 5554 0900  highlight.jsUT..
-00005f70: 03ce 5358 64ff 2374 6475 780b 0001 04e8  ..SXd.#tdux.....
+00005f70: 03ce 5358 64a4 d3ac 6475 780b 0001 04e8  ..SXd...dux.....
 00005f80: 0300 0004 e803 0000 9d58 5993 db36 0c7e  .........XY..6.~
 00005f90: f7af 60d4 9954 deb8 f2b6 7ddb 8db7 b387  ..`..T....}.....
 00005fa0: 1b6f e3d8 9995 d363 da8e 8796 688b 894c  .o.....c....h..L
 00005fb0: aa22 e563 d2fd ef05 481d 94f6 68da ccac  .".c....H...h...
 00005fc0: 6d91 2000 021f 804f 199e 9009 df24 29fc  m. ....O.....$).
 00005fd0: 692e 36a4 d03c e59a 3345 d632 2761 9670  i.6..<..3E.2'a.p
 00005fe0: 7120 93c5 bb29 8965 546c 99d0 5473 2902  q ...).eTl..Ts).
@@ -1836,15 +1836,15 @@
 000072b0: fc02 528a 9e2e 8e21 158c c916 cd0c 3ce9  ..R....!......<.
 000072c0: 760e 07ad 357e cb2a 6e53 6311 58fd 4f56  v...5~.*nSc.X.OV
 000072d0: a4e1 0650 69ec 9b34 a33c e93f 7e20 4d9e  ...Pi..4.<.?~ M.
 000072e0: ae7e 2eeb 9c12 9a00 504b 0304 1400 0000  .~......PK......
 000072f0: 0800 aa99 a756 0ec6 325d 5378 0000 9d5d  .....V..2]Sx...]
 00007300: 0100 1b00 1c00 7374 6174 6963 2f65 6e2f  ......static/en/
 00007310: 5f73 7461 7469 632f 6a71 7565 7279 2e6a  _static/jquery.j
-00007320: 7355 5409 0003 bf5a 5864 ff23 7464 7578  sUT....ZXd.#tdux
+00007320: 7355 5409 0003 bf5a 5864 a4d3 ac64 7578  sUT....ZXd...dux
 00007330: 0b00 0104 e803 0000 04e8 0300 00ac 5be9  ..............[.
 00007340: 76db 3896 fe3f 4f21 b132 0a61 c1b4 9474  v.8..?O!.2.a...t
 00007350: 3227 b411 9d94 ed54 d29d ad23 5755 774b  2'.....T...#WUwK
 00007360: 4a1d 5a84 6c26 32a9 9090 9798 aa67 efef  J.Z.l&2......g..
 00007370: 02dc 4555 aa67 c639 3149 2c17 77c3 dd00  ..EU.g.91I,.w...
 00007380: 1fec 753b 9fff be96 f15d e7fa b1f3 d419  ..u;.....]......
 00007390: 74d2 8e3d 679d f72b 19fe 75dc 7919 ad43  t..=g..+..u.y..C
@@ -16859,15 +16859,15 @@
 00041da0: 7d1e 38f4 2add 86b9 0000 0000 4945 4e44  }.8.*.......IEND
 00041db0: ae42 6082 504b 0304 1400 0000 0800 aa99  .B`.PK..........
 00041dc0: a756 6c0e d52c fd05 0000 c110 0000 3900  .Vl..,........9.
 00041dd0: 1c00 7374 6174 6963 2f65 6e2f 5f73 7461  ..static/en/_sta
 00041de0: 7469 632f 5f73 7068 696e 785f 6a61 7661  tic/_sphinx_java
 00041df0: 7363 7269 7074 5f66 7261 6d65 776f 726b  script_framework
 00041e00: 735f 636f 6d70 6174 2e6a 7355 5409 0003  s_compat.jsUT...
-00041e10: bf5a 5864 ff23 7464 7578 0b00 0104 e803  .ZXd.#tdux......
+00041e10: bf5a 5864 a4d3 ac64 7578 0b00 0104 e803  .ZXd...dux......
 00041e20: 0000 04e8 0300 00a5 576d 6fdb 3610 feee  ........Wmo.6...
 00041e30: 5f71 f380 5a4a 3c2a 6dbf c5cb 8a26 1d8a  _q..ZJ<*m....&..
 00041e40: 0e7d d9e2 b6fb e006 0125 d116 5359 d448  .}.......%..SY.H
 00041e50: ca2f 6bf2 df77 474a b29c 2869 d009 412c  ./k..wGJ..(i..A,
 00041e60: 91f7 7ecf 1d8f d101 9ca9 65c9 2d8f 652e  ..~.......e.-.e.
 00041e70: ed16 4c26 9730 571a aefe aa84 de02 2f52  ..L&.0W......./R
 00041e80: a88a 5468 9328 2d0c bb32 6c00 07f8 877c  ..Th.(-..2l....|
@@ -136474,15 +136474,15 @@
 00215190: f32c 0bd0 2532 071e 7f9e 1872 0187 8142  .,..%2.....r...B
 002151a0: 1fe0 7f34 c739 f9b4 582c c2fe 60ac 1566  ...4.9..X,..`..f
 002151b0: d276 cab4 59c7 7036 3b86 4b32 fb0b 504b  .v..Y.p6;.K2..PK
 002151c0: 0304 1400 0000 0800 7595 a756 6b35 2548  ........u..Vk5%H
 002151d0: 0407 0000 6812 0000 2500 1c00 7374 6174  ....h...%...stat
 002151e0: 6963 2f70 742f 5f73 7461 7469 632f 7370  ic/pt/_static/sp
 002151f0: 6869 6e78 5f68 6967 686c 6967 6874 2e6a  hinx_highlight.j
-00215200: 7355 5409 0003 ce53 5864 ff23 7464 7578  sUT....SXd.#tdux
+00215200: 7355 5409 0003 ce53 5864 a4d3 ac64 7578  sUT....SXd...dux
 00215210: 0b00 0104 e803 0000 04e8 0300 009d 5859  ..............XY
 00215220: 93db 360c 7ef7 af60 d499 54de b8f2 b67d  ..6.~..`..T....}
 00215230: db8d b7b3 871b 6fe3 d899 95d3 63da 8e87  ......o.....c...
 00215240: 9668 8b89 4caa 22e5 63d2 fdef 0548 1d94  .h..L.".c....H..
 00215250: f668 dacc ac6d 9120 0002 1f80 4f19 9e90  .h...m. ....O...
 00215260: 09df 2429 fc69 2e36 a4d0 3ce5 9a33 45d6  ..$).i.6..<..3E.
 00215270: 3227 6196 7071 2093 c5bb 2989 6554 6c99  2'a.pq ...).eTl.
@@ -136901,15 +136901,15 @@
 00216c40: 8cc9 16cd 0c3c e976 0e07 ad35 7ecb 2a6e  .....<.v...5~.*n
 00216c50: 5363 1158 fd4f 56a4 e106 5069 ec9b 34a3  Sc.X.OV...Pi..4.
 00216c60: 3ce9 3f7e 204d 9eae 7e2e eb9c 129a 0050  <.?~ M..~......P
 00216c70: 4b03 0414 0000 0008 00ac 99a7 560e c632  K...........V..2
 00216c80: 5d53 7800 009d 5d01 001b 001c 0073 7461  ]Sx...]......sta
 00216c90: 7469 632f 7074 2f5f 7374 6174 6963 2f6a  tic/pt/_static/j
 00216ca0: 7175 6572 792e 6a73 5554 0900 03c4 5a58  query.jsUT....ZX
-00216cb0: 64ff 2374 6475 780b 0001 04e8 0300 0004  d.#tdux.........
+00216cb0: 64a4 d3ac 6475 780b 0001 04e8 0300 0004  d...dux.........
 00216cc0: e803 0000 ac5b e976 db38 96fe 3f4f 21b1  .....[.v.8..?O!.
 00216cd0: 320a 61c1 b494 7432 27b4 119d 94ed 54d2  2.a...t2'.....T.
 00216ce0: 9dad 2357 5577 4b4a 1d5a 846c 2632 a990  ..#WUwKJ.Z.l&2..
 00216cf0: 9097 98aa 67ef ef02 dc45 55aa 67c6 3931  ....g....EU.g.91
 00216d00: 492c 1777 c3dd 001f ec75 3b9f ffbe 96f1  I,.w.....u;.....
 00216d10: 5de7 fab1 f3d4 1974 d28e 3d67 9df7 2b19  ]......t..=g..+.
 00216d20: fe75 dc79 19ad 43df 5341 1476 bcd0 ef44  .u.y..C.SA.v...D
@@ -152022,15 +152022,15 @@
 00251d50: 2add 86b9 0000 0000 4945 4e44 ae42 6082  *.......IEND.B`.
 00251d60: 504b 0304 1400 0000 0800 ac99 a756 6c0e  PK...........Vl.
 00251d70: d52c fd05 0000 c110 0000 3900 1c00 7374  .,........9...st
 00251d80: 6174 6963 2f70 742f 5f73 7461 7469 632f  atic/pt/_static/
 00251d90: 5f73 7068 696e 785f 6a61 7661 7363 7269  _sphinx_javascri
 00251da0: 7074 5f66 7261 6d65 776f 726b 735f 636f  pt_frameworks_co
 00251db0: 6d70 6174 2e6a 7355 5409 0003 c45a 5864  mpat.jsUT....ZXd
-00251dc0: ff23 7464 7578 0b00 0104 e803 0000 04e8  .#tdux..........
+00251dc0: a4d3 ac64 7578 0b00 0104 e803 0000 04e8  ...dux..........
 00251dd0: 0300 00a5 576d 6fdb 3610 feee 5f71 f380  ....Wmo.6..._q..
 00251de0: 5a4a 3c2a 6dbf c5cb 8a26 1d8a 0e7d d9e2  ZJ<*m....&...}..
 00251df0: b6fb e006 0125 d116 5359 d448 ca2f 6bf2  .....%..SY.H./k.
 00251e00: df77 474a b29c 2869 d009 412c 91f7 7ecf  .wGJ..(i..A,..~.
 00251e10: 1d8f d101 9ca9 65c9 2d8f 652e ed16 4c26  ......e.-.e...L&
 00251e20: 9730 571a aefe aa84 de02 2f52 a88a 5468  .0W......./R..Th
 00251e30: 9328 2d0c bb32 6c00 07f8 877c e556 cb45  .(-..2l....|.V.E
```

#### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app._documentation.zip`

```diff
@@ -1521,15 +1521,15 @@
 00005f00: 3207 1e7f 9e18 7201 8781 421f e07f 34c7  2.....r...B...4.
 00005f10: 39f9 b458 2cc2 fe60 ac15 66d2 76ca b459  9..X,..`..f.v..Y
 00005f20: c770 363b 864b 32fb 0b50 4b03 0414 0000  .p6;.K2..PK.....
 00005f30: 0008 0075 95a7 566b 3525 4804 0700 0068  ...u..Vk5%H....h
 00005f40: 1200 0025 001c 0073 7461 7469 632f 656e  ...%...static/en
 00005f50: 2f5f 7374 6174 6963 2f73 7068 696e 785f  /_static/sphinx_
 00005f60: 6869 6768 6c69 6768 742e 6a73 5554 0900  highlight.jsUT..
-00005f70: 03ce 5358 64ff 2374 6475 780b 0001 04e8  ..SXd.#tdux.....
+00005f70: 03ce 5358 64a4 d3ac 6475 780b 0001 04e8  ..SXd...dux.....
 00005f80: 0300 0004 e803 0000 9d58 5993 db36 0c7e  .........XY..6.~
 00005f90: f7af 60d4 9954 deb8 f2b6 7ddb 8db7 b387  ..`..T....}.....
 00005fa0: 1b6f e3d8 9995 d363 da8e 8796 688b 894c  .o.....c....h..L
 00005fb0: aa22 e563 d2fd ef05 481d 94f6 68da ccac  .".c....H...h...
 00005fc0: 6d91 2000 021f 804f 199e 9009 df24 29fc  m. ....O.....$).
 00005fd0: 692e 36a4 d03c e59a 3345 d632 2761 9670  i.6..<..3E.2'a.p
 00005fe0: 7120 93c5 bb29 8965 546c 99d0 5473 2902  q ...).eTl..Ts).
@@ -1836,15 +1836,15 @@
 000072b0: fc02 528a 9e2e 8e21 158c c916 cd0c 3ce9  ..R....!......<.
 000072c0: 760e 07ad 357e cb2a 6e53 6311 58fd 4f56  v...5~.*nSc.X.OV
 000072d0: a4e1 0650 69ec 9b34 a33c e93f 7e20 4d9e  ...Pi..4.<.?~ M.
 000072e0: ae7e 2eeb 9c12 9a00 504b 0304 1400 0000  .~......PK......
 000072f0: 0800 aa99 a756 0ec6 325d 5378 0000 9d5d  .....V..2]Sx...]
 00007300: 0100 1b00 1c00 7374 6174 6963 2f65 6e2f  ......static/en/
 00007310: 5f73 7461 7469 632f 6a71 7565 7279 2e6a  _static/jquery.j
-00007320: 7355 5409 0003 bf5a 5864 ff23 7464 7578  sUT....ZXd.#tdux
+00007320: 7355 5409 0003 bf5a 5864 a4d3 ac64 7578  sUT....ZXd...dux
 00007330: 0b00 0104 e803 0000 04e8 0300 00ac 5be9  ..............[.
 00007340: 76db 3896 fe3f 4f21 b132 0a61 c1b4 9474  v.8..?O!.2.a...t
 00007350: 3227 b411 9d94 ed54 d29d ad23 5755 774b  2'.....T...#WUwK
 00007360: 4a1d 5a84 6c26 32a9 9090 9798 aa67 efef  J.Z.l&2......g..
 00007370: 02dc 4555 aa67 c639 3149 2c17 77c3 dd00  ..EU.g.91I,.w...
 00007380: 1fec 753b 9fff be96 f15d e7fa b1f3 d419  ..u;.....]......
 00007390: 74d2 8e3d 679d f72b 19fe 75dc 7919 ad43  t..=g..+..u.y..C
@@ -16859,15 +16859,15 @@
 00041da0: 7d1e 38f4 2add 86b9 0000 0000 4945 4e44  }.8.*.......IEND
 00041db0: ae42 6082 504b 0304 1400 0000 0800 aa99  .B`.PK..........
 00041dc0: a756 6c0e d52c fd05 0000 c110 0000 3900  .Vl..,........9.
 00041dd0: 1c00 7374 6174 6963 2f65 6e2f 5f73 7461  ..static/en/_sta
 00041de0: 7469 632f 5f73 7068 696e 785f 6a61 7661  tic/_sphinx_java
 00041df0: 7363 7269 7074 5f66 7261 6d65 776f 726b  script_framework
 00041e00: 735f 636f 6d70 6174 2e6a 7355 5409 0003  s_compat.jsUT...
-00041e10: bf5a 5864 ff23 7464 7578 0b00 0104 e803  .ZXd.#tdux......
+00041e10: bf5a 5864 a4d3 ac64 7578 0b00 0104 e803  .ZXd...dux......
 00041e20: 0000 04e8 0300 00a5 576d 6fdb 3610 feee  ........Wmo.6...
 00041e30: 5f71 f380 5a4a 3c2a 6dbf c5cb 8a26 1d8a  _q..ZJ<*m....&..
 00041e40: 0e7d d9e2 b6fb e006 0125 d116 5359 d448  .}.......%..SY.H
 00041e50: ca2f 6bf2 df77 474a b29c 2869 d009 412c  ./k..wGJ..(i..A,
 00041e60: 91f7 7ecf 1d8f d101 9ca9 65c9 2d8f 652e  ..~.......e.-.e.
 00041e70: ed16 4c26 9730 571a aefe aa84 de02 2f52  ..L&.0W......./R
 00041e80: a88a 5468 9328 2d0c bb32 6c00 07f8 877c  ..Th.(-..2l....|
@@ -136474,15 +136474,15 @@
 00215190: f32c 0bd0 2532 071e 7f9e 1872 0187 8142  .,..%2.....r...B
 002151a0: 1fe0 7f34 c739 f9b4 582c c2fe 60ac 1566  ...4.9..X,..`..f
 002151b0: d276 cab4 59c7 7036 3b86 4b32 fb0b 504b  .v..Y.p6;.K2..PK
 002151c0: 0304 1400 0000 0800 7595 a756 6b35 2548  ........u..Vk5%H
 002151d0: 0407 0000 6812 0000 2500 1c00 7374 6174  ....h...%...stat
 002151e0: 6963 2f70 742f 5f73 7461 7469 632f 7370  ic/pt/_static/sp
 002151f0: 6869 6e78 5f68 6967 686c 6967 6874 2e6a  hinx_highlight.j
-00215200: 7355 5409 0003 ce53 5864 ff23 7464 7578  sUT....SXd.#tdux
+00215200: 7355 5409 0003 ce53 5864 a4d3 ac64 7578  sUT....SXd...dux
 00215210: 0b00 0104 e803 0000 04e8 0300 009d 5859  ..............XY
 00215220: 93db 360c 7ef7 af60 d499 54de b8f2 b67d  ..6.~..`..T....}
 00215230: db8d b7b3 871b 6fe3 d899 95d3 63da 8e87  ......o.....c...
 00215240: 9668 8b89 4caa 22e5 63d2 fdef 0548 1d94  .h..L.".c....H..
 00215250: f668 dacc ac6d 9120 0002 1f80 4f19 9e90  .h...m. ....O...
 00215260: 09df 2429 fc69 2e36 a4d0 3ce5 9a33 45d6  ..$).i.6..<..3E.
 00215270: 3227 6196 7071 2093 c5bb 2989 6554 6c99  2'a.pq ...).eTl.
@@ -136901,15 +136901,15 @@
 00216c40: 8cc9 16cd 0c3c e976 0e07 ad35 7ecb 2a6e  .....<.v...5~.*n
 00216c50: 5363 1158 fd4f 56a4 e106 5069 ec9b 34a3  Sc.X.OV...Pi..4.
 00216c60: 3ce9 3f7e 204d 9eae 7e2e eb9c 129a 0050  <.?~ M..~......P
 00216c70: 4b03 0414 0000 0008 00ac 99a7 560e c632  K...........V..2
 00216c80: 5d53 7800 009d 5d01 001b 001c 0073 7461  ]Sx...]......sta
 00216c90: 7469 632f 7074 2f5f 7374 6174 6963 2f6a  tic/pt/_static/j
 00216ca0: 7175 6572 792e 6a73 5554 0900 03c4 5a58  query.jsUT....ZX
-00216cb0: 64ff 2374 6475 780b 0001 04e8 0300 0004  d.#tdux.........
+00216cb0: 64a4 d3ac 6475 780b 0001 04e8 0300 0004  d...dux.........
 00216cc0: e803 0000 ac5b e976 db38 96fe 3f4f 21b1  .....[.v.8..?O!.
 00216cd0: 320a 61c1 b494 7432 27b4 119d 94ed 54d2  2.a...t2'.....T.
 00216ce0: 9dad 2357 5577 4b4a 1d5a 846c 2632 a990  ..#WUwKJ.Z.l&2..
 00216cf0: 9097 98aa 67ef ef02 dc45 55aa 67c6 3931  ....g....EU.g.91
 00216d00: 492c 1777 c3dd 001f ec75 3b9f ffbe 96f1  I,.w.....u;.....
 00216d10: 5de7 fab1 f3d4 1974 d28e 3d67 9df7 2b19  ]......t..=g..+.
 00216d20: fe75 dc79 19ad 43df 5341 1476 bcd0 ef44  .u.y..C.SA.v...D
@@ -152022,15 +152022,15 @@
 00251d50: 2add 86b9 0000 0000 4945 4e44 ae42 6082  *.......IEND.B`.
 00251d60: 504b 0304 1400 0000 0800 ac99 a756 6c0e  PK...........Vl.
 00251d70: d52c fd05 0000 c110 0000 3900 1c00 7374  .,........9...st
 00251d80: 6174 6963 2f70 742f 5f73 7461 7469 632f  atic/pt/_static/
 00251d90: 5f73 7068 696e 785f 6a61 7661 7363 7269  _sphinx_javascri
 00251da0: 7074 5f66 7261 6d65 776f 726b 735f 636f  pt_frameworks_co
 00251db0: 6d70 6174 2e6a 7355 5409 0003 c45a 5864  mpat.jsUT....ZXd
-00251dc0: ff23 7464 7578 0b00 0104 e803 0000 04e8  .#tdux..........
+00251dc0: a4d3 ac64 7578 0b00 0104 e803 0000 04e8  ...dux..........
 00251dd0: 0300 00a5 576d 6fdb 3610 feee 5f71 f380  ....Wmo.6..._q..
 00251de0: 5a4a 3c2a 6dbf c5cb 8a26 1d8a 0e7d d9e2  ZJ<*m....&...}..
 00251df0: b6fb e006 0125 d116 5359 d448 ca2f 6bf2  .....%..SY.H./k.
 00251e00: df77 474a b29c 2869 d009 412c 91f7 7ecf  .wGJ..(i..A,..~.
 00251e10: 1d8f d101 9ca9 65c9 2d8f 652e ed16 4c26  ......e.-.e...L&
 00251e20: 9730 571a aefe aa84 de02 2f52 a88a 5468  .0W......./R..Th
 00251e30: 9328 2d0c bb32 6c00 07f8 877c e556 cb45  .(-..2l....|.V.E
```

### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app.showcase.zip`

 * *Format-specific differences are supported for ZIP archives but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Zip archive data, at least v2.0 to extract, compression method=deflate*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

 * *Files 0% similar despite different names*

```diff
@@ -6156,15 +6156,15 @@
 000180b0: 3baa fe0a 1c82 921c 2bfc 4976 aa0b 2c7f  ;.......+.Iv..,.
 000180c0: 2c5e 1b57 92a6 04b6 ee3b b6c6 8146 7b10  ,^.W.....;...F{.
 000180d0: 69c4 ab3b 431e 4b74 7173 3f7f 0050 4b03  i..;C.Ktqs?..PK.
 000180e0: 040a 0000 0000 00f6 8ca7 5600 0000 0000  ..........V.....
 000180f0: 0000 0000 0000 0029 001c 0073 7461 7469  .......)...stati
 00018100: 632f 636f 6d70 6f6e 656e 7473 2f73 7461  c/components/sta
 00018110: 7272 6174 6572 2f73 7461 7272 6174 6572  rrater/starrater
-00018120: 2e63 7373 5554 0900 03d0 4458 64ff 2374  .cssUT....DXd.#t
+00018120: 2e63 7373 5554 0900 03d0 4458 64a4 d3ac  .cssUT....DXd...
 00018130: 6475 780b 0001 04e8 0300 0004 e803 0000  dux.............
 00018140: 504b 0304 1400 0000 0800 f68c a756 dc21  PK...........V.!
 00018150: 6d0c 9400 0000 3401 0000 2a00 1c00 7374  m.....4...*...st
 00018160: 6174 6963 2f63 6f6d 706f 6e65 6e74 732f  atic/components/
 00018170: 7374 6172 7261 7465 722f 7374 6172 7261  starrater/starra
 00018180: 7465 722e 6874 6d6c 5554 0900 03d0 4458  ter.htmlUT....DX
 00018190: 6487 d3ac 6475 780b 0001 04e8 0300 0004  d...dux.........
@@ -83469,15 +83469,15 @@
 001460c0: 1b57 92a6 04b6 ee3b b6c6 8146 7b10 69c4  .W.....;...F{.i.
 001460d0: ab3b 431e 4b74 7173 3f7f 0050 4b03 040a  .;C.Ktqs?..PK...
 001460e0: 0000 0000 00f6 8ca7 5600 0000 0000 0000  ........V.......
 001460f0: 0000 0000 002f 001c 0073 7461 7469 632f  ...../...static/
 00146100: 636f 6d70 6f6e 656e 7473 2d62 756c 6d61  components-bulma
 00146110: 2f73 7461 7272 6174 6572 2f73 7461 7272  /starrater/starr
 00146120: 6174 6572 2e63 7373 5554 0900 03d0 4458  ater.cssUT....DX
-00146130: 64ff 2374 6475 780b 0001 04e8 0300 0004  d.#tdux.........
+00146130: 64a4 d3ac 6475 780b 0001 04e8 0300 0004  d...dux.........
 00146140: e803 0000 504b 0304 1400 0000 0800 f68c  ....PK..........
 00146150: a756 dc21 6d0c 9400 0000 3401 0000 3000  .V.!m.....4...0.
 00146160: 1c00 7374 6174 6963 2f63 6f6d 706f 6e65  ..static/compone
 00146170: 6e74 732d 6275 6c6d 612f 7374 6172 7261  nts-bulma/starra
 00146180: 7465 722f 7374 6172 7261 7465 722e 6874  ter/starrater.ht
 00146190: 6d6c 5554 0900 03d0 4458 6487 d3ac 6475  mlUT....DXd...du
 001461a0: 780b 0001 04e8 0300 0004 e803 0000 7dcf  x.............}.
```

#### Comparing `py4web-1.20230710.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230710.3/py4web/assets/py4web.app.showcase.zip`

```diff
@@ -6156,15 +6156,15 @@
 000180b0: 3baa fe0a 1c82 921c 2bfc 4976 aa0b 2c7f  ;.......+.Iv..,.
 000180c0: 2c5e 1b57 92a6 04b6 ee3b b6c6 8146 7b10  ,^.W.....;...F{.
 000180d0: 69c4 ab3b 431e 4b74 7173 3f7f 0050 4b03  i..;C.Ktqs?..PK.
 000180e0: 040a 0000 0000 00f6 8ca7 5600 0000 0000  ..........V.....
 000180f0: 0000 0000 0000 0029 001c 0073 7461 7469  .......)...stati
 00018100: 632f 636f 6d70 6f6e 656e 7473 2f73 7461  c/components/sta
 00018110: 7272 6174 6572 2f73 7461 7272 6174 6572  rrater/starrater
-00018120: 2e63 7373 5554 0900 03d0 4458 64ff 2374  .cssUT....DXd.#t
+00018120: 2e63 7373 5554 0900 03d0 4458 64a4 d3ac  .cssUT....DXd...
 00018130: 6475 780b 0001 04e8 0300 0004 e803 0000  dux.............
 00018140: 504b 0304 1400 0000 0800 f68c a756 dc21  PK...........V.!
 00018150: 6d0c 9400 0000 3401 0000 2a00 1c00 7374  m.....4...*...st
 00018160: 6174 6963 2f63 6f6d 706f 6e65 6e74 732f  atic/components/
 00018170: 7374 6172 7261 7465 722f 7374 6172 7261  starrater/starra
 00018180: 7465 722e 6874 6d6c 5554 0900 03d0 4458  ter.htmlUT....DX
 00018190: 6487 d3ac 6475 780b 0001 04e8 0300 0004  d...dux.........
@@ -83469,15 +83469,15 @@
 001460c0: 1b57 92a6 04b6 ee3b b6c6 8146 7b10 69c4  .W.....;...F{.i.
 001460d0: ab3b 431e 4b74 7173 3f7f 0050 4b03 040a  .;C.Ktqs?..PK...
 001460e0: 0000 0000 00f6 8ca7 5600 0000 0000 0000  ........V.......
 001460f0: 0000 0000 002f 001c 0073 7461 7469 632f  ...../...static/
 00146100: 636f 6d70 6f6e 656e 7473 2d62 756c 6d61  components-bulma
 00146110: 2f73 7461 7272 6174 6572 2f73 7461 7272  /starrater/starr
 00146120: 6174 6572 2e63 7373 5554 0900 03d0 4458  ater.cssUT....DX
-00146130: 64ff 2374 6475 780b 0001 04e8 0300 0004  d.#tdux.........
+00146130: 64a4 d3ac 6475 780b 0001 04e8 0300 0004  d...dux.........
 00146140: e803 0000 504b 0304 1400 0000 0800 f68c  ....PK..........
 00146150: a756 dc21 6d0c 9400 0000 3401 0000 3000  .V.!m.....4...0.
 00146160: 1c00 7374 6174 6963 2f63 6f6d 706f 6e65  ..static/compone
 00146170: 6e74 732d 6275 6c6d 612f 7374 6172 7261  nts-bulma/starra
 00146180: 7465 722f 7374 6172 7261 7465 722e 6874  ter/starrater.ht
 00146190: 6d6c 5554 0900 03d0 4458 6487 d3ac 6475  mlUT....DXd...du
 001461a0: 780b 0001 04e8 0300 0004 e803 0000 7dcf  x.............}.
```

### Comparing `py4web-1.20230710.1/py4web/core.py` & `py4web-1.20230710.3/py4web/core.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/server_adapters.py` & `py4web-1.20230710.3/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth.py` & `py4web-1.20230710.3/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230710.3/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/cors.py` & `py4web-1.20230710.3/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/dbstore.py` & `py4web-1.20230710.3/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/downloader.py` & `py4web-1.20230710.3/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/factories.py` & `py4web-1.20230710.3/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/form.py` & `py4web-1.20230710.3/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/grid.py` & `py4web-1.20230710.3/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/jsonrpc.py` & `py4web-1.20230710.3/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/mailer.py` & `py4web-1.20230710.3/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/misc.py` & `py4web-1.20230710.3/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/populate.py` & `py4web-1.20230710.3/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/publisher.py` & `py4web-1.20230710.3/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/recaptcha.py` & `py4web-1.20230710.3/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/security.py` & `py4web-1.20230710.3/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web/utils/url_signer.py` & `py4web-1.20230710.3/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/py4web.egg-info/PKG-INFO` & `py4web-1.20230710.3/py4web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230710.1
+Version: 1.20230710.3
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230710.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20230710.3/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/pyproject.toml` & `py4web-1.20230710.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20230710.1"
+version = "1.20230710.3"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20230710.1/tests/test_action.py` & `py4web-1.20230710.3/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_auth.py` & `py4web-1.20230710.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_cache.py` & `py4web-1.20230710.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_fixture.py` & `py4web-1.20230710.3/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_form.py` & `py4web-1.20230710.3/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_get_error_snapshot.py` & `py4web-1.20230710.3/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_json.py` & `py4web-1.20230710.3/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_main.py` & `py4web-1.20230710.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_session.py` & `py4web-1.20230710.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230710.1/tests/test_tags.py` & `py4web-1.20230710.3/tests/test_tags.py`

 * *Files identical despite different names*

