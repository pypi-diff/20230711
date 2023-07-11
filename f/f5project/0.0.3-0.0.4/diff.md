# Comparing `tmp/f5project-0.0.3.tar.gz` & `tmp/f5project-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f5project-0.0.3.tar", last modified: Mon Jul 10 23:54:07 2023, max compression
+gzip compressed data, was "f5project-0.0.4.tar", last modified: Tue Jul 11 00:16:46 2023, max compression
```

## Comparing `f5project-0.0.3.tar` & `f5project-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-10 23:54:07.786023 f5project-0.0.3/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.3/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     5176 2023-07-10 23:54:07.785899 f5project-0.0.3/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     4727 2023-07-10 23:53:10.000000 f5project-0.0.3/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-10 23:54:07.785191 f5project-0.0.3/f5project/
--rw-r--r--   0 j3ymac     (501) staff       (20)    11747 2023-07-10 23:27:29.000000 f5project-0.0.3/f5project/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-10 23:54:07.785745 f5project-0.0.3/f5project.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     5176 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      180 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-10 23:54:07.786062 f5project-0.0.3/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      701 2023-07-10 23:51:11.000000 f5project-0.0.3/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:16:46.490113 f5project-0.0.4/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.4/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     5277 2023-07-11 00:16:46.489933 f5project-0.0.4/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)     4828 2023-07-11 00:16:09.000000 f5project-0.0.4/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:16:46.488977 f5project-0.0.4/f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)    11747 2023-07-10 23:27:29.000000 f5project-0.0.4/f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:16:46.489711 f5project-0.0.4/f5project.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     5277 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      180 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-11 00:16:46.000000 f5project-0.0.4/f5project.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-11 00:16:46.490176 f5project-0.0.4/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      701 2023-07-11 00:16:31.000000 f5project-0.0.4/setup.py
```

### Comparing `f5project-0.0.3/LICENSE` & `f5project-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `f5project-0.0.3/PKG-INFO` & `f5project-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5project
-Version: 0.0.3
+Version: 0.0.4
 Summary: F5 project
 Home-page: https://github.com/thejimmylin/f5project
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,36 +14,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # F5 Project
 
 Finlab Fugle for financial freedom.
 
-This library is designed to make it easier to use Finlab/Fugle. It also combines them with Google Cloud Function and Github Actions, making the iteration of your trading strategy faster. It fits my workflow, and I hope it fits yours too. Otherwise, you can always fork it and make it your own.
-
 # Install
 
-Install it with pip:
-
 ```
 pip install f5project
 ```
 
-# Usages
+# Why?
 
-This project is designed to be used Finlab/Fugle with GCF and Github Actions together.
+This library makes it easier to use Finlab/Fugle with other tools together, such as GCF and Github Action.
 
-You want to focus on your trading strategy, letting `f5project` handle config and all the boring stuff for you, including:
+When deploying your code on GCF. Some troubles come up and you can't just do it like you do on your local machine. This library helps you to solve these problems. It helps you:
 
 - Read config from json file or environment variables.
-- Extract Fugle config and certificate from json file or environment variables, dynamically generate them as needed in proper locations.
-- Sync Github secrets with local config.
-- Login Finlab/Fugle with config.
+- Extract Fugle config and certificate from json file or environment variables, dynamically generate them as needed.
+- Login Finlab/Fugle with config, which is a little bit annoying because Fugle SDK asks them as files.
+- Provide a decorator to make your function a GCF endpoint, without worrying about the request/response format.
 - Simulate GCF request locally.
-- Provide a decorator to make your function a GCF endpoint.
+- Sync Github secrets with local config, make CI/CD easier.
+
+Then you can focus on your trading strategy and iterate faster.
+
+# Usages
 
 main.py
 
 ```python
 """Main entrypoint of the project.
 
 - This file is the entrypoint of Google Cloud Function.
@@ -159,8 +159,13 @@
             FUGLE_CERT_PASSWORD=${{ secrets.FUGLE_CERT_PASSWORD }},
             FUGLE_API_ENTRY=${{ secrets.FUGLE_API_ENTRY }},
             FUGLE_API_KEY=${{ secrets.FUGLE_API_KEY }},
             FUGLE_API_SECRET=${{ secrets.FUGLE_API_SECRET }},
             FUGLE_MARKET_API_KEY=${{ secrets.FUGLE_MARKET_API_KEY }},
 ```
 
+# TODO
+
+- Use `pipx` to make it easier to have a quickstart template.
+- Dynamically generate `CI/CD` pipeline YAML file, so we can focus on the code.
+
```

### Comparing `f5project-0.0.3/README.md` & `f5project-0.0.4/f5project.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,49 @@
+Metadata-Version: 2.1
+Name: f5project
+Version: 0.0.4
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
 
-This library is designed to make it easier to use Finlab/Fugle. It also combines them with Google Cloud Function and Github Actions, making the iteration of your trading strategy faster. It fits my workflow, and I hope it fits yours too. Otherwise, you can always fork it and make it your own.
-
 # Install
 
-Install it with pip:
-
 ```
 pip install f5project
 ```
 
-# Usages
+# Why?
 
-This project is designed to be used Finlab/Fugle with GCF and Github Actions together.
+This library makes it easier to use Finlab/Fugle with other tools together, such as GCF and Github Action.
 
-You want to focus on your trading strategy, letting `f5project` handle config and all the boring stuff for you, including:
+When deploying your code on GCF. Some troubles come up and you can't just do it like you do on your local machine. This library helps you to solve these problems. It helps you:
 
 - Read config from json file or environment variables.
-- Extract Fugle config and certificate from json file or environment variables, dynamically generate them as needed in proper locations.
-- Sync Github secrets with local config.
-- Login Finlab/Fugle with config.
+- Extract Fugle config and certificate from json file or environment variables, dynamically generate them as needed.
+- Login Finlab/Fugle with config, which is a little bit annoying because Fugle SDK asks them as files.
+- Provide a decorator to make your function a GCF endpoint, without worrying about the request/response format.
 - Simulate GCF request locally.
-- Provide a decorator to make your function a GCF endpoint.
+- Sync Github secrets with local config, make CI/CD easier.
+
+Then you can focus on your trading strategy and iterate faster.
+
+# Usages
 
 main.py
 
 ```python
 """Main entrypoint of the project.
 
 - This file is the entrypoint of Google Cloud Function.
@@ -142,7 +158,14 @@
             FUGLE_CERT=${{ secrets.FUGLE_CERT }},
             FUGLE_CERT_PASSWORD=${{ secrets.FUGLE_CERT_PASSWORD }},
             FUGLE_API_ENTRY=${{ secrets.FUGLE_API_ENTRY }},
             FUGLE_API_KEY=${{ secrets.FUGLE_API_KEY }},
             FUGLE_API_SECRET=${{ secrets.FUGLE_API_SECRET }},
             FUGLE_MARKET_API_KEY=${{ secrets.FUGLE_MARKET_API_KEY }},
 ```
+
+# TODO
+
+- Use `pipx` to make it easier to have a quickstart template.
+- Dynamically generate `CI/CD` pipeline YAML file, so we can focus on the code.
+
+
```

### Comparing `f5project-0.0.3/f5project/__init__.py` & `f5project-0.0.4/f5project/__init__.py`

 * *Files identical despite different names*

### Comparing `f5project-0.0.3/f5project.egg-info/PKG-INFO` & `f5project-0.0.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,33 @@
-Metadata-Version: 2.1
-Name: f5project
-Version: 0.0.3
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
 
-This library is designed to make it easier to use Finlab/Fugle. It also combines them with Google Cloud Function and Github Actions, making the iteration of your trading strategy faster. It fits my workflow, and I hope it fits yours too. Otherwise, you can always fork it and make it your own.
-
 # Install
 
-Install it with pip:
-
 ```
 pip install f5project
 ```
 
-# Usages
+# Why?
 
-This project is designed to be used Finlab/Fugle with GCF and Github Actions together.
+This library makes it easier to use Finlab/Fugle with other tools together, such as GCF and Github Action.
 
-You want to focus on your trading strategy, letting `f5project` handle config and all the boring stuff for you, including:
+When deploying your code on GCF. Some troubles come up and you can't just do it like you do on your local machine. This library helps you to solve these problems. It helps you:
 
 - Read config from json file or environment variables.
-- Extract Fugle config and certificate from json file or environment variables, dynamically generate them as needed in proper locations.
-- Sync Github secrets with local config.
-- Login Finlab/Fugle with config.
+- Extract Fugle config and certificate from json file or environment variables, dynamically generate them as needed.
+- Login Finlab/Fugle with config, which is a little bit annoying because Fugle SDK asks them as files.
+- Provide a decorator to make your function a GCF endpoint, without worrying about the request/response format.
 - Simulate GCF request locally.
-- Provide a decorator to make your function a GCF endpoint.
+- Sync Github secrets with local config, make CI/CD easier.
+
+Then you can focus on your trading strategy and iterate faster.
+
+# Usages
 
 main.py
 
 ```python
 """Main entrypoint of the project.
 
 - This file is the entrypoint of Google Cloud Function.
@@ -159,8 +143,11 @@
             FUGLE_CERT_PASSWORD=${{ secrets.FUGLE_CERT_PASSWORD }},
             FUGLE_API_ENTRY=${{ secrets.FUGLE_API_ENTRY }},
             FUGLE_API_KEY=${{ secrets.FUGLE_API_KEY }},
             FUGLE_API_SECRET=${{ secrets.FUGLE_API_SECRET }},
             FUGLE_MARKET_API_KEY=${{ secrets.FUGLE_MARKET_API_KEY }},
 ```
 
+# TODO
 
+- Use `pipx` to make it easier to have a quickstart template.
+- Dynamically generate `CI/CD` pipeline YAML file, so we can focus on the code.
```

### Comparing `f5project-0.0.3/setup.py` & `f5project-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="f5project",
-    version="0.0.3",
+    version="0.0.4",
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="F5 project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/f5project",
     packages=setuptools.find_packages(),
```

