# Comparing `tmp/f5project-0.0.4.tar.gz` & `tmp/f5project-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f5project-0.0.4.tar", last modified: Tue Jul 11 00:16:46 2023, max compression
+gzip compressed data, was "f5project-0.0.5.tar", last modified: Tue Jul 11 00:42:08 2023, max compression
```

## Comparing `f5project-0.0.4.tar` & `f5project-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:16:46.490113 f5project-0.0.4/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.4/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     5277 2023-07-11 00:16:46.489933 f5project-0.0.4/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     4828 2023-07-11 00:16:09.000000 f5project-0.0.4/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:16:46.488977 f5project-0.0.4/f5project/
--rw-r--r--   0 j3ymac     (501) staff       (20)    11747 2023-07-10 23:27:29.000000 f5project-0.0.4/f5project/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:16:46.489711 f5project-0.0.4/f5project.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     5277 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      180 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-11 00:16:46.490176 f5project-0.0.4/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      701 2023-07-11 00:16:31.000000 f5project-0.0.4/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:42:08.532599 f5project-0.0.5/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.5/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-11 00:42:08.532440 f5project-0.0.5/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)     6646 2023-07-11 00:40:13.000000 f5project-0.0.5/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:42:08.531663 f5project-0.0.5/f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)    11747 2023-07-10 23:27:29.000000 f5project-0.0.5/f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:42:08.532279 f5project-0.0.5/f5project.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      212 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/requires.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-11 00:42:08.532639 f5project-0.0.5/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      763 2023-07-11 00:40:25.000000 f5project-0.0.5/setup.py
```

### Comparing `f5project-0.0.4/LICENSE` & `f5project-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `f5project-0.0.4/PKG-INFO` & `f5project-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,15 @@
-Metadata-Version: 2.1
-Name: f5project
-Version: 0.0.4
-Summary: F5 project
-Home-page: https://github.com/thejimmylin/f5project
-Author: thejimmylin
-Author-email: b00502013@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # F5 Project
 
 Finlab Fugle for financial freedom.
 
+This library is not ready for production. It's still under development. The document is not complete, either.
+
+You may need to read the source code sometimes.
+
 # Install
 
 ```
 pip install f5project
 ```
 
 # Why?
@@ -37,14 +25,41 @@
 - Simulate GCF request locally.
 - Sync Github secrets with local config, make CI/CD easier.
 
 Then you can focus on your trading strategy and iterate faster.
 
 # Usages
 
+Put all your secrets in `.secrets/index.json` file and ignore it in `.gitignore`. It will be synced to Github later.
+
+.secrets/index.json
+
+```json
+{
+  "finlab_api_token": "your_finlab_api_token", // Get it from https://ai.finlab.tw/member_info
+  "fugle_account": "your_fugle_account", // Your Fugle account. It shows in Fugle API config downloaded from https://fugletradingapi.esunsec.com.tw/keys/apikey/APIKeyManagement
+  "fugle_password": "your_fugle_password", // Your Fugle password. It's what you use to login https://www.fugle.tw/
+  "fugle_cert": "./fugle-cert.p12", // Put your certificate in this file. Download it from https://fugletradingapi.esunsec.com.tw/keys/apikey/APIKeyManagement
+  "fugle_cert_password": "fugle_cert_password", // The password of your certificate.
+  "fugle_api_entry": "https://fugletradingapi.esunsec.com.tw/api/v1", // Fugle API entrypoint. It usually doesn't change. It shows in Fugle API config, too.
+  "fugle_api_key": "your_fugle_api_key", // Shown in Fugle API config.
+  "fugle_api_secret": "your_fugle_api_secret", // Shown in Fugle API config.
+  "fugle_market_api_key": "your_fugle_market_api_key", // Apply it from https://developer.fugle.tw/docs/key/. Note the version should be `v0.3`.
+  "gcf_service_account": {
+    // Your GCF service account json, you can get it from GCP console.
+  },
+  // Export a Github PAT to makes it possible to sync all these secrets to Github easily.
+  "repo_synced": {
+    "owner": "your_github_username",
+    "repo": "your_github_repo_name",
+    "pat": "your_github_personal_access_token"
+  }
+}
+```
+
 main.py
 
 ```python
 """Main entrypoint of the project.
 
 - This file is the entrypoint of Google Cloud Function.
 - It also provides a CLI to run the function locally.
@@ -60,15 +75,15 @@
 BASE_DIR = Path(__file__).resolve().parent
 
 
 # Let `F5Project` handle all the boring stuff.
 project = F5Project(config=F5ProjectConfig.from_json_or_env(BASE_DIR / ".secrets" / "index.json"))
 
 
-# Decorate our `create_orders` function to make it a Google Cloud Function.
+# Decorate our `create_orders` function to make it a GCF endpoint
 @project.gcf_endpoint
 def create_orders(view_only: bool = True, fund: int = 30000, odd_lot: bool = True) -> list[dict]:
     # Login project first
     project.login()
     # Get backtest report with some strategy
     report = my_strategies.tibetan_mastiff()
     # Use it to create stock position we should own
@@ -83,14 +98,16 @@
 
 
 if __name__ == "__main__":
     # This makes it possible to develop locally. See the `run` method for more details.
     project.run_locally(with_server=True, params={"view_only": True, "fund": 10000, "odd_lot": True})
 ```
 
+Add this script and make it a Git pre-push hook. It will sync secrets from local to Github.
+
 scripts/sync_github_secrets.py
 
 ```python
 #!.venv/bin/python
 """Sync secrets from local to GitHub.
 
 Install it as a Git pre-push hook by:
@@ -163,9 +180,7 @@
             FUGLE_MARKET_API_KEY=${{ secrets.FUGLE_MARKET_API_KEY }},
 ```
 
 # TODO
 
 - Use `pipx` to make it easier to have a quickstart template.
 - Dynamically generate `CI/CD` pipeline YAML file, so we can focus on the code.
-
-
```

### Comparing `f5project-0.0.4/README.md` & `f5project-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,31 @@
+Metadata-Version: 2.1
+Name: f5project
+Version: 0.0.5
+Summary: F5 project
+Home-page: https://github.com/thejimmylin/f5project
+Author: thejimmylin
+Author-email: b00502013@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # F5 Project
 
 Finlab Fugle for financial freedom.
 
+This library is not ready for production. It's still under development. The document is not complete, either.
+
+You may need to read the source code sometimes.
+
 # Install
 
 ```
 pip install f5project
 ```
 
 # Why?
@@ -21,14 +41,41 @@
 - Simulate GCF request locally.
 - Sync Github secrets with local config, make CI/CD easier.
 
 Then you can focus on your trading strategy and iterate faster.
 
 # Usages
 
+Put all your secrets in `.secrets/index.json` file and ignore it in `.gitignore`. It will be synced to Github later.
+
+.secrets/index.json
+
+```json
+{
+  "finlab_api_token": "your_finlab_api_token", // Get it from https://ai.finlab.tw/member_info
+  "fugle_account": "your_fugle_account", // Your Fugle account. It shows in Fugle API config downloaded from https://fugletradingapi.esunsec.com.tw/keys/apikey/APIKeyManagement
+  "fugle_password": "your_fugle_password", // Your Fugle password. It's what you use to login https://www.fugle.tw/
+  "fugle_cert": "./fugle-cert.p12", // Put your certificate in this file. Download it from https://fugletradingapi.esunsec.com.tw/keys/apikey/APIKeyManagement
+  "fugle_cert_password": "fugle_cert_password", // The password of your certificate.
+  "fugle_api_entry": "https://fugletradingapi.esunsec.com.tw/api/v1", // Fugle API entrypoint. It usually doesn't change. It shows in Fugle API config, too.
+  "fugle_api_key": "your_fugle_api_key", // Shown in Fugle API config.
+  "fugle_api_secret": "your_fugle_api_secret", // Shown in Fugle API config.
+  "fugle_market_api_key": "your_fugle_market_api_key", // Apply it from https://developer.fugle.tw/docs/key/. Note the version should be `v0.3`.
+  "gcf_service_account": {
+    // Your GCF service account json, you can get it from GCP console.
+  },
+  // Export a Github PAT to makes it possible to sync all these secrets to Github easily.
+  "repo_synced": {
+    "owner": "your_github_username",
+    "repo": "your_github_repo_name",
+    "pat": "your_github_personal_access_token"
+  }
+}
+```
+
 main.py
 
 ```python
 """Main entrypoint of the project.
 
 - This file is the entrypoint of Google Cloud Function.
 - It also provides a CLI to run the function locally.
@@ -44,15 +91,15 @@
 BASE_DIR = Path(__file__).resolve().parent
 
 
 # Let `F5Project` handle all the boring stuff.
 project = F5Project(config=F5ProjectConfig.from_json_or_env(BASE_DIR / ".secrets" / "index.json"))
 
 
-# Decorate our `create_orders` function to make it a Google Cloud Function.
+# Decorate our `create_orders` function to make it a GCF endpoint
 @project.gcf_endpoint
 def create_orders(view_only: bool = True, fund: int = 30000, odd_lot: bool = True) -> list[dict]:
     # Login project first
     project.login()
     # Get backtest report with some strategy
     report = my_strategies.tibetan_mastiff()
     # Use it to create stock position we should own
@@ -67,14 +114,16 @@
 
 
 if __name__ == "__main__":
     # This makes it possible to develop locally. See the `run` method for more details.
     project.run_locally(with_server=True, params={"view_only": True, "fund": 10000, "odd_lot": True})
 ```
 
+Add this script and make it a Git pre-push hook. It will sync secrets from local to Github.
+
 scripts/sync_github_secrets.py
 
 ```python
 #!.venv/bin/python
 """Sync secrets from local to GitHub.
 
 Install it as a Git pre-push hook by:
@@ -147,7 +196,9 @@
             FUGLE_MARKET_API_KEY=${{ secrets.FUGLE_MARKET_API_KEY }},
 ```
 
 # TODO
 
 - Use `pipx` to make it easier to have a quickstart template.
 - Dynamically generate `CI/CD` pipeline YAML file, so we can focus on the code.
+
+
```

### Comparing `f5project-0.0.4/f5project/__init__.py` & `f5project-0.0.5/f5project/__init__.py`

 * *Files identical despite different names*

### Comparing `f5project-0.0.4/setup.py` & `f5project-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from pathlib import Path
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="f5project",
-    version="0.0.4",
+    version="0.0.5",
+    install_requires=[
+        "github-secret-syncer",
+    ],
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="F5 project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/f5project",
     packages=setuptools.find_packages(),
```

