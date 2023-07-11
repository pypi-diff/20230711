# Comparing `tmp/exem-vault-1.0.0.tar.gz` & `tmp/exem-vault-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exem-vault-1.0.0.tar", last modified: Fri Jun 23 09:58:40 2023, max compression
+gzip compressed data, was "exem-vault-1.1.1.tar", last modified: Tue Jul 11 08:21:26 2023, max compression
```

## Comparing `exem-vault-1.0.0.tar` & `exem-vault-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:58:40.803612 exem-vault-1.0.0/
--rw-rw-rw-   0        0        0     1495 2023-06-23 09:58:40.803612 exem-vault-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-06-23 09:58:23.000000 exem-vault-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 09:58:40.803612 exem-vault-1.0.0/exem_vault.egg-info/
--rw-rw-rw-   0        0        0     1495 2023-06-23 09:58:40.000000 exem-vault-1.0.0/exem_vault.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-23 09:58:40.000000 exem-vault-1.0.0/exem_vault.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:58:40.000000 exem-vault-1.0.0/exem_vault.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-23 09:58:40.000000 exem-vault-1.0.0/exem_vault.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 09:58:40.000000 exem-vault-1.0.0/exem_vault.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      711 2023-05-10 14:29:56.000000 exem-vault-1.0.0/policy.py
--rw-rw-rw-   0        0        0       42 2023-06-23 09:58:40.803612 exem-vault-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-06-23 09:58:23.000000 exem-vault-1.0.0/setup.py
--rw-rw-rw-   0        0        0     1399 2023-05-17 07:32:24.000000 exem-vault-1.0.0/vault.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:21:26.265901 exem-vault-1.1.1/
+-rw-rw-rw-   0        0        0     1676 2023-07-11 08:21:26.265901 exem-vault-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1300 2023-07-11 08:19:43.000000 exem-vault-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:21:26.265901 exem-vault-1.1.1/exem_vault.egg-info/
+-rw-rw-rw-   0        0        0     1676 2023-07-11 08:21:26.000000 exem-vault-1.1.1/exem_vault.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-07-11 08:21:26.000000 exem-vault-1.1.1/exem_vault.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:21:26.000000 exem-vault-1.1.1/exem_vault.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-11 08:21:26.000000 exem-vault-1.1.1/exem_vault.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 08:21:26.000000 exem-vault-1.1.1/exem_vault.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      711 2023-05-10 14:29:56.000000 exem-vault-1.1.1/policy.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:21:26.265901 exem-vault-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-07-11 08:19:10.000000 exem-vault-1.1.1/setup.py
+-rw-rw-rw-   0        0        0     1424 2023-06-26 15:00:45.000000 exem-vault-1.1.1/vault.py
```

### Comparing `exem-vault-1.0.0/PKG-INFO` & `exem-vault-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exem-vault
-Version: 1.0.0
+Version: 1.1.1
 Summary: All secrets now at reach.
 Home-page: https://gitlab.com/exem2/libraries/api/vault
 Author: Félix BOULE--REIFF
 Author-email: boulereiff@exem.fr
 License: BSD 2-clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -65,7 +65,14 @@
 ```
 
 And add it to the vault with:
 
 ```
 vault.add_policy("your_policy_name", policy)
 ```
+
+If your version of python is >= 3.6 do the following before installing exem-vault:
+
+    pip uninstall ply
+    pip uninstall pyhcl
+    pip install ply
+    pip install pyhcl
```

### Comparing `exem-vault-1.0.0/README.md` & `exem-vault-1.1.1/exem_vault.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: exem-vault
+Version: 1.1.1
+Summary: All secrets now at reach.
+Home-page: https://gitlab.com/exem2/libraries/api/vault
+Author: Félix BOULE--REIFF
+Author-email: boulereiff@exem.fr
+License: BSD 2-clause
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/markdown
+
 # Vault
 
 This project provides a simple, object-oriented Python API for interacting with an HashiCorp's Vault 
 using the hvac library.
 
 ## How to
 
@@ -53,7 +65,14 @@
 ```
 
 And add it to the vault with:
 
 ```
 vault.add_policy("your_policy_name", policy)
 ```
+
+If your version of python is >= 3.6 do the following before installing exem-vault:
+
+    pip uninstall ply
+    pip uninstall pyhcl
+    pip install ply
+    pip install pyhcl
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exem-vault-1.0.0/policy.py` & `exem-vault-1.1.1/policy.py`

 * *Files identical despite different names*

### Comparing `exem-vault-1.0.0/setup.py` & `exem-vault-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='exem-vault',
-    version='1.0.0',
+    version='1.1.1',
     description='All secrets now at reach.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/exem2/libraries/api/vault',
     author='Félix BOULE--REIFF',
     author_email='boulereiff@exem.fr',
     license='BSD 2-clause',
     install_requires=[
       "hvac",
     ],
-    py_modules=[  # Ajoute des scripts de la racine
+    py_modules=[
         'vault',
         'policy'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: BSD License'
     ],
```

### Comparing `exem-vault-1.0.0/vault.py` & `exem-vault-1.1.1/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import hvac
 
 
 class Vault:
 
     @staticmethod
     def unseal(host="http://localhost:8200", keys=None):
@@ -14,15 +15,15 @@
         return not client.sys.is_sealed()
 
     def __init__(self, token, host="http://localhost:8200"):
         self.token = token
         self.client = hvac.Client(url=host, token=token, timeout=120)
 
     def read(self, mount_point, path):
-        return self.client.secrets.kv.v2.read_secret_version(path=path, mount_point=mount_point)["data"]["data"]
+        return json.loads(self.client.secrets.kv.v2.read_secret_version(path=path, mount_point=mount_point)["data"]["data"])
 
     def write(self, mount_point, path, data):
         return self.client.secrets.kv.v2.patch(mount_point, path, data)
 
     def delete(self, mount_point, path, key):
         data = self.read(mount_point, path).pop(key)
         return self.client.secrets.kv.v2.create_or_update_secret(mount_point, path, data)
```

