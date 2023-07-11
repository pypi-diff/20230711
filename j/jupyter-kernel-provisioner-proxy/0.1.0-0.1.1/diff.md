# Comparing `tmp/jupyter_kernel_provisioner_proxy-0.1.0.tar.gz` & `tmp/jupyter_kernel_provisioner_proxy-0.1.1.tar.gz`

## Comparing `jupyter_kernel_provisioner_proxy-0.1.0.tar` & `jupyter_kernel_provisioner_proxy-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/__init__.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/cli.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/client.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/connect.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/message.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/README.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/__init__.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/cli.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/client.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/connect.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/message.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/README.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyter_kernel_provisioner_proxy-0.1.1/PKG-INFO
```

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/cli.py` & `jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/client.py` & `jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/connect.py` & `jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/connect.py`

 * *Files identical despite different names*

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/jupyter_kernel_provisioner_proxy/message.py` & `jupyter_kernel_provisioner_proxy-0.1.1/jupyter_kernel_provisioner_proxy/message.py`

 * *Files identical despite different names*

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/LICENSE` & `jupyter_kernel_provisioner_proxy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/README.md` & `jupyter_kernel_provisioner_proxy-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 ## Usage
 
 ### Main server side
 
 Install jupyter-kernel-provisioner-proxy:
 
-```bash
+```console
 pip install jupyter-kernel-provisioner-proxy
 ```
 
 Then install a kernelspec with the `jupyter-kernel-provisioner-proxy install` command.
 
-```bash
+```console
 $ jupyter-kernel-provisioner-proxy install --help
 
  Usage: jupyter-kernel-provisioner-proxy install [OPTIONS]
 
 ╭─ Options ────────────────────────────────────────────╮
 │ --display     TEXT  The kernel's display name        │
 │ --language    TEXT  The kernel's language name       │
@@ -32,18 +32,18 @@
 
 ### Kernel server side
 
 You can use [jupyter-server](https://github.com/jupyter-server/jupyter_server) or [jupyverse](https://github.com/jupyter-server/jupyverse) to serve remote kernels.
 
 #### Using jupyter-server
 
-```bash
+```console
 pip install jupyter-server
 jupyter server --ServerApp.token='' --ServerApp.password='' --ServerApp.disable_check_xsrf=True --no-browser --port=8000
 ```
 
 #### Using jupyverse
 
-```bash
-pip install jupyverse[jupyterlab,noauth]
+```console
+pip install fps-kernels fps-noauth fps-frontend ipykernel
 jupyverse
 ```
```

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/pyproject.toml` & `jupyter_kernel_provisioner_proxy-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_kernel_provisioner_proxy-0.1.0/PKG-INFO` & `jupyter_kernel_provisioner_proxy-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-kernel-provisioner-proxy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jupyter kernel provisioner proxy
 Project-URL: Homepage, https://github.com/davidbrochart/jupyter-kernel-provisioner-proxy
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -30,21 +30,21 @@
 
 ## Usage
 
 ### Main server side
 
 Install jupyter-kernel-provisioner-proxy:
 
-```bash
+```console
 pip install jupyter-kernel-provisioner-proxy
 ```
 
 Then install a kernelspec with the `jupyter-kernel-provisioner-proxy install` command.
 
-```bash
+```console
 $ jupyter-kernel-provisioner-proxy install --help
 
  Usage: jupyter-kernel-provisioner-proxy install [OPTIONS]
 
 ╭─ Options ────────────────────────────────────────────╮
 │ --display     TEXT  The kernel's display name        │
 │ --language    TEXT  The kernel's language name       │
@@ -58,18 +58,18 @@
 
 ### Kernel server side
 
 You can use [jupyter-server](https://github.com/jupyter-server/jupyter_server) or [jupyverse](https://github.com/jupyter-server/jupyverse) to serve remote kernels.
 
 #### Using jupyter-server
 
-```bash
+```console
 pip install jupyter-server
 jupyter server --ServerApp.token='' --ServerApp.password='' --ServerApp.disable_check_xsrf=True --no-browser --port=8000
 ```
 
 #### Using jupyverse
 
-```bash
-pip install jupyverse[jupyterlab,noauth]
+```console
+pip install fps-kernels fps-noauth fps-frontend ipykernel
 jupyverse
 ```
```

