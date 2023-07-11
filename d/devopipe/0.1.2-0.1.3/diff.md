# Comparing `tmp/devopipe-0.1.2.tar.gz` & `tmp/devopipe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopipe-0.1.2.tar", max compression
+gzip compressed data, was "devopipe-0.1.3.tar", max compression
```

## Comparing `devopipe-0.1.2.tar` & `devopipe-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1321 2023-07-11 18:14:44.200899 devopipe-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-11 18:14:35.450899 devopipe-0.1.2/devopipe/__init__.py
--rwxr-xr-x   0        0        0    17351 2023-07-11 18:11:19.682759 devopipe-0.1.2/devopipe/src/main.py
--rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.2/devopipe/src/setup_template.yaml
--rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.2/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
--rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.2/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
--rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.2/devopipe/src/templates/IaC/aws/blueprints.tf
--rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.2/devopipe/src/templates/IaC/aws/create-namespace.yaml
--rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.2/devopipe/src/templates/IaC/aws/create-vcluster.yaml
--rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.2/devopipe/src/templates/IaC/aws/developer-role.tf
--rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.2/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
--rwxr-xr-x   0        0        0     1818 2023-07-08 07:27:31.748556 devopipe-0.1.2/devopipe/src/templates/IaC/aws/main.tf
--rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.2/devopipe/src/templates/IaC/aws/values/argocd.yaml
--rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.2/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
--rwxr-xr-x   0        0        0      191 2023-07-08 07:28:37.216100 devopipe-0.1.2/devopipe/src/templates/IaC/aws/variables.tf
--rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.2/devopipe/src/templates/IaC/aws/vpc-module.tf
--rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.2/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
--rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.2/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
--rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.2/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
--rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.2/devopipe/src/templates/ci-pipeline/get-artifact.yaml
--rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.2/devopipe/src/templates/ci-pipeline/set-artifact.yaml
--rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/deployment.yaml
--rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
--rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
--rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
--rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
--rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.2/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
--rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.2/devopipe/src/templates/kubernetes/aws/service-account.yaml
--rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.2/devopipe/src/templates/kubernetes/aws/storage.yaml
--rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.2/devopipe/src/templates/tests/database-sonarqube.yaml
--rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.2/devopipe/src/templates/tests/deployment-sonarqube.yaml
--rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.2/devopipe/src/templates/tests/storage_sonarqube.yaml
--rw-r--r--   0        0        0      486 2023-07-11 18:14:37.290899 devopipe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 devopipe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-11 19:39:10.970575 devopipe-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 19:39:10.970575 devopipe-0.1.3/devopipe/__init__.py
+-rwxr-xr-x   0        0        0    17349 2023-07-11 18:15:53.521255 devopipe-0.1.3/devopipe/src/main.py
+-rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.3/devopipe/src/setup_template.yaml
+-rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.3/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
+-rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.3/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
+-rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.3/devopipe/src/templates/IaC/aws/blueprints.tf
+-rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.3/devopipe/src/templates/IaC/aws/create-namespace.yaml
+-rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.3/devopipe/src/templates/IaC/aws/create-vcluster.yaml
+-rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.3/devopipe/src/templates/IaC/aws/developer-role.tf
+-rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.3/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
+-rwxr-xr-x   0        0        0     1818 2023-07-08 07:27:31.748556 devopipe-0.1.3/devopipe/src/templates/IaC/aws/main.tf
+-rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.3/devopipe/src/templates/IaC/aws/values/argocd.yaml
+-rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.3/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
+-rwxr-xr-x   0        0        0      191 2023-07-08 07:28:37.216100 devopipe-0.1.3/devopipe/src/templates/IaC/aws/variables.tf
+-rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.3/devopipe/src/templates/IaC/aws/vpc-module.tf
+-rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.3/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
+-rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.3/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
+-rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.3/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
+-rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.3/devopipe/src/templates/ci-pipeline/get-artifact.yaml
+-rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.3/devopipe/src/templates/ci-pipeline/set-artifact.yaml
+-rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/deployment.yaml
+-rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
+-rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
+-rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
+-rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
+-rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.3/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
+-rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.3/devopipe/src/templates/kubernetes/aws/service-account.yaml
+-rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.3/devopipe/src/templates/kubernetes/aws/storage.yaml
+-rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.3/devopipe/src/templates/tests/database-sonarqube.yaml
+-rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.3/devopipe/src/templates/tests/deployment-sonarqube.yaml
+-rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.3/devopipe/src/templates/tests/storage_sonarqube.yaml
+-rw-r--r--   0        0        0      486 2023-07-11 19:39:13.100575 devopipe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.3/PKG-INFO
```

### Comparing `devopipe-0.1.2/devopipe/src/main.py` & `devopipe-0.1.3/devopipe/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, Optional
 
 import typer
 import os
 import shutil
 from pathlib import Path
 from string import Template
-#from jinja2 import Environment, FileSystemLoader
-#import yaml
+from jinja2 import Environment, FileSystemLoader
+import yaml
 
 
 app = typer.Typer()
 
 
 @app.command()
 def version():
```

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/argocd/argocd.yaml` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/argocd/argocd.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/blueprints.tf` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/blueprints.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/developer-role.tf` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/developer-role.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/kubernetes-addons.tf` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/kubernetes-addons.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/main.tf` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/main.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/IaC/aws/vpc-module.tf` & `devopipe-0.1.3/devopipe/src/templates/IaC/aws/vpc-module.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml` & `devopipe-0.1.3/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml` & `devopipe-0.1.3/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml` & `devopipe-0.1.3/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/ci-pipeline/get-artifact.yaml` & `devopipe-0.1.3/devopipe/src/templates/ci-pipeline/get-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/ci-pipeline/set-artifact.yaml` & `devopipe-0.1.3/devopipe/src/templates/ci-pipeline/set-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/deployment.yaml` & `devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/deployment.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml` & `devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/deployment_database.yaml` & `devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/deployment_database.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml` & `devopipe-0.1.3/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml` & `devopipe-0.1.3/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/tests/database-sonarqube.yaml` & `devopipe-0.1.3/devopipe/src/templates/tests/database-sonarqube.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.2/devopipe/src/templates/tests/deployment-sonarqube.yaml` & `devopipe-0.1.3/devopipe/src/templates/tests/deployment-sonarqube.yaml`

 * *Files identical despite different names*

