# Comparing `tmp/idem-vault-0.4.0.tar.gz` & `tmp/idem-vault-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-vault-0.4.0.tar", last modified: Fri Apr 28 14:32:27 2023, max compression
+gzip compressed data, was "idem-vault-0.4.1.tar", last modified: Tue Jul 11 18:47:51 2023, max compression
```

## Comparing `idem-vault-0.4.0.tar` & `idem-vault-0.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/
--rw-r--r--   0 root         (0) root         (0)    11338 2023-04-28 14:32:14.000000 idem-vault-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4431 2023-04-28 14:32:27.894988 idem-vault-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3596 2023-04-28 14:32:14.000000 idem-vault-0.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/acct/backend/
--rw-r--r--   0 root         (0) root         (0)     2915 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/acct/backend/vault.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/hvac/
--rw-r--r--   0 root         (0) root         (0)      571 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/exec/hvac/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v1/
--rw-r--r--   0 root         (0) root         (0)     1119 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v1/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v2/
--rw-r--r--   0 root         (0) root         (0)     1257 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v2/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/source/
--rw-r--r--   0 root         (0) root         (0)     1221 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/source/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/
--rw-r--r--   0 root         (0) root         (0)      173 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/
--rw-r--r--   0 root         (0) root         (0)     5986 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/key.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v2/
--rw-r--r--   0 root         (0) root         (0)     8035 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v2/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/tool/hvac/
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/tool/hvac/client.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/tool/hvac/resolve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/tool/vault/
--rw-r--r--   0 root         (0) root         (0)      684 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/tool/vault/secret.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4431 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      696 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 14:32:27.898988 idem-vault-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2715 2023-04-28 14:32:14.000000 idem-vault-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)    11338 2023-07-11 18:47:36.000000 idem-vault-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-07-11 18:47:51.924913 idem-vault-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-11 18:47:36.000000 idem-vault-0.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/acct/backend/
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/acct/backend/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/hvac/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/exec/hvac/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v1/
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v1/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v2/
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v2/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/source/
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/source/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/
+-rw-r--r--   0 root         (0) root         (0)     5986 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/key.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v2/
+-rw-r--r--   0 root         (0) root         (0)     8035 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v2/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/tool/hvac/
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/tool/hvac/client.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/tool/hvac/resolve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/tool/vault/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/tool/vault/secret.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-11 18:47:51.924913 idem-vault-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-07-11 18:47:36.000000 idem-vault-0.4.1/setup.py
```

### Comparing `idem-vault-0.4.0/LICENSE` & `idem-vault-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/PKG-INFO` & `idem-vault-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-vault
-Version: 0.4.0
+Version: 0.4.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-vault
 Author: VMware Inc.
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -132,21 +132,21 @@
 
 In order to run the idem-vault tests, you need a development vault environment to be running locally.
 
 Run the vault server with docker enabling kv_v1.
 
 .. code-block:: bash
 
-    $ docker run -p 8201:8201 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8201" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk"  vault server -dev -dev-kv-v1
+    $ docker run -p 8201:8201 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8201" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk"  hashicorp/vault server -dev -dev-kv-v1
 
 Start a second docker vault server enabling kv_v2
 
 .. code-block:: bash
 
-    $ docker run -p 8200:8200 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8200" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk" vault
+    $ docker run -p 8200:8200 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8200" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk" hashicorp/vault
 
 Add the default credentials.yml to your environment.
 
 .. code-block:: bash
 
     $ export ACCT_FILE="$PWD/example/credentials.yml"
```

### Comparing `idem-vault-0.4.0/README.rst` & `idem-vault-0.4.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -108,21 +108,21 @@
 
 In order to run the idem-vault tests, you need a development vault environment to be running locally.
 
 Run the vault server with docker enabling kv_v1.
 
 .. code-block:: bash
 
-    $ docker run -p 8201:8201 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8201" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk"  vault server -dev -dev-kv-v1
+    $ docker run -p 8201:8201 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8201" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk"  hashicorp/vault server -dev -dev-kv-v1
 
 Start a second docker vault server enabling kv_v2
 
 .. code-block:: bash
 
-    $ docker run -p 8200:8200 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8200" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk" vault
+    $ docker run -p 8200:8200 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8200" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk" hashicorp/vault
 
 Add the default credentials.yml to your environment.
 
 .. code-block:: bash
 
     $ export ACCT_FILE="$PWD/example/credentials.yml"
```

### Comparing `idem-vault-0.4.0/idem_vault/acct/backend/vault.py` & `idem-vault-0.4.1/idem_vault/acct/backend/vault.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/conf.py` & `idem-vault-0.4.1/idem_vault/conf.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/exec/hvac/init.py` & `idem-vault-0.4.1/idem_vault/exec/hvac/init.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v1/secret.py` & `idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v1/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v2/secret.py` & `idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v2/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/source/vault.py` & `idem-vault-0.4.1/idem_vault/source/vault.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/key.py` & `idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/key.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/secret.py` & `idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v2/secret.py` & `idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v2/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/tool/hvac/client.py` & `idem-vault-0.4.1/idem_vault/tool/hvac/client.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/tool/hvac/resolve.py` & `idem-vault-0.4.1/idem_vault/tool/hvac/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault/tool/vault/secret.py` & `idem-vault-0.4.1/idem_vault/tool/vault/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/idem_vault.egg-info/PKG-INFO` & `idem-vault-0.4.1/idem_vault.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-vault
-Version: 0.4.0
+Version: 0.4.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-vault
 Author: VMware Inc.
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -132,21 +132,21 @@
 
 In order to run the idem-vault tests, you need a development vault environment to be running locally.
 
 Run the vault server with docker enabling kv_v1.
 
 .. code-block:: bash
 
-    $ docker run -p 8201:8201 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8201" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk"  vault server -dev -dev-kv-v1
+    $ docker run -p 8201:8201 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8201" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk"  hashicorp/vault server -dev -dev-kv-v1
 
 Start a second docker vault server enabling kv_v2
 
 .. code-block:: bash
 
-    $ docker run -p 8200:8200 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8200" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk" vault
+    $ docker run -p 8200:8200 -e VAULT_DEV_LISTEN_ADDRESS="0.0.0.0:8200" -e VAULT_DEV_ROOT_TOKEN_ID="abcdefghijk" hashicorp/vault
 
 Add the default credentials.yml to your environment.
 
 .. code-block:: bash
 
     $ export ACCT_FILE="$PWD/example/credentials.yml"
```

### Comparing `idem-vault-0.4.0/idem_vault.egg-info/SOURCES.txt` & `idem-vault-0.4.1/idem_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.0/setup.py` & `idem-vault-0.4.1/setup.py`

 * *Files identical despite different names*

