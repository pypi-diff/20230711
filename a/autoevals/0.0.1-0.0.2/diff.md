# Comparing `tmp/autoevals-0.0.1.tar.gz` & `tmp/autoevals-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoevals-0.0.1.tar", last modified: Mon Jul 10 22:53:28 2023, max compression
+gzip compressed data, was "autoevals-0.0.2.tar", last modified: Tue Jul 11 06:41:46 2023, max compression
```

## Comparing `autoevals-0.0.1.tar` & `autoevals-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-10 22:53:28.560704 autoevals-0.0.1/
--rw-r--r--   0 ankur      (501) staff       (20)      471 2023-07-10 22:53:28.560561 autoevals-0.0.1/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-06-12 14:02:51.000000 autoevals-0.0.1/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       31 2023-06-12 13:36:29.000000 autoevals-0.0.1/pyproject.toml
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-10 22:53:28.560739 autoevals-0.0.1/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1596 2023-07-10 22:53:10.000000 autoevals-0.0.1/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-10 22:53:28.559325 autoevals-0.0.1/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-10 22:53:28.559864 autoevals-0.0.1/src/autoevals/
--rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-12 13:43:04.000000 autoevals-0.0.1/src/autoevals/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-12 13:36:54.000000 autoevals-0.0.1/src/autoevals/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-10 22:53:28.560413 autoevals-0.0.1/src/autoevals.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      471 2023-07-10 22:53:28.000000 autoevals-0.0.1/src/autoevals.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-10 22:53:28.000000 autoevals-0.0.1/src/autoevals.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-10 22:53:28.000000 autoevals-0.0.1/src/autoevals.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)      251 2023-07-10 22:53:28.000000 autoevals-0.0.1/src/autoevals.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-10 22:53:28.000000 autoevals-0.0.1/src/autoevals.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 06:41:46.194748 autoevals-0.0.2/
+-rw-r--r--   0 ankur      (501) staff       (20)     3285 2023-07-11 06:41:46.194646 autoevals-0.0.2/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)     2790 2023-07-11 06:35:51.000000 autoevals-0.0.2/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-11 06:26:06.000000 autoevals-0.0.2/pyproject.toml
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-11 06:41:46.194783 autoevals-0.0.2/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1559 2023-07-11 06:26:29.000000 autoevals-0.0.2/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 06:41:46.193035 autoevals-0.0.2/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 06:41:46.193995 autoevals-0.0.2/src/autoevals/
+-rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-11 06:26:29.000000 autoevals-0.0.2/src/autoevals/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1271 2023-07-11 06:26:29.000000 autoevals-0.0.2/src/autoevals/base.py
+-rw-r--r--   0 ankur      (501) staff       (20)     5456 2023-07-11 06:26:29.000000 autoevals-0.0.2/src/autoevals/llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      464 2023-07-11 06:26:29.000000 autoevals-0.0.2/src/autoevals/string.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-11 06:26:29.000000 autoevals-0.0.2/src/autoevals/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-11 06:40:36.000000 autoevals-0.0.2/src/autoevals/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 06:41:46.194519 autoevals-0.0.2/src/autoevals.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)     3285 2023-07-11 06:41:46.000000 autoevals-0.0.2/src/autoevals.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      357 2023-07-11 06:41:46.000000 autoevals-0.0.2/src/autoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-11 06:41:46.000000 autoevals-0.0.2/src/autoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-11 06:41:46.000000 autoevals-0.0.2/src/autoevals.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-11 06:41:46.000000 autoevals-0.0.2/src/autoevals.egg-info/top_level.txt
```

### Comparing `autoevals-0.0.1/setup.py` & `autoevals-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 version_contents = {}
 with open(os.path.join(dir_name, "src", "autoevals", "version.py"), encoding="utf-8") as f:
     exec(f.read(), version_contents)
 
 with open(os.path.join(dir_name, "README.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
-install_requires = ["openai", "GitPython", "requests"]
+install_requires = ["chevron", "guidance", "openai", "levenshtein", "pyyaml"]
 
 extras_require = {
     "dev": [
         "black",
         "build",
         "flake8",
         "flake8-isort",
         "IPython",
-        "isort==5.10.1",
+        "isort==5.12.0",
         "pre-commit",
         "pytest",
         "twine",
     ],
     "doc": ["pydoc-markdown[novella]"],
 }
 
 extras_require["all"] = sorted({package for packages in extras_require.values() for package in packages})
 
 setuptools.setup(
     name="autoevals",
     version=version_contents["VERSION"],
     author="BrainTrust",
     author_email="info@braintrustdata.com",
-    description="Universal library for working with LLMs",
+    description="Universal library for evaluating AI models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.braintrustdata.com",
-    # project_urls={
-    #    "Bug Tracker": "https://github.com/TODO/issues",
-    # },
+    project_urls={
+        "Bug Tracker": "https://github.com/braintrustdata/autoevals",
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7.0",
-    entry_points={},  # {"console_scripts": ["braintrust = braintrust.cli.__main__:main"]},
+    python_requires=">=3.9.0",
+    entry_points={},
     install_requires=install_requires,
     extras_require=extras_require,
 )
```

