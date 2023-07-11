# Comparing `tmp/heatmap_cli-0.1.1.tar.gz` & `tmp/heatmap_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.1.1.tar", last modified: Sat Jul  8 16:37:06 2023, max compression
+gzip compressed data, was "heatmap_cli-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `heatmap_cli-0.1.1.tar` & `heatmap_cli-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      143 2023-07-08 15:37:49.950263 heatmap_cli-0.1.1/.coveragerc
--rw-r--r--   0        0        0     3101 2023-07-08 15:39:47.014546 heatmap_cli-0.1.1/.gitignore
--rw-r--r--   0        0        0     2411 2023-07-08 16:32:44.037058 heatmap_cli-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2023-07-08 15:37:49.950263 heatmap_cli-0.1.1/.prettierignore
--rw-r--r--   0        0        0       29 2023-07-08 15:37:49.950263 heatmap_cli-0.1.1/.python-version
--rw-r--r--   0        0        0      447 2023-07-08 16:34:28.286319 heatmap_cli-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1738 2023-07-08 15:37:49.982263 heatmap_cli-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-08 15:37:49.954263 heatmap_cli-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      445 2023-07-08 16:09:00.508282 heatmap_cli-0.1.1/Pipfile
--rw-r--r--   0        0        0    70216 2023-07-08 16:07:54.727800 heatmap_cli-0.1.1/Pipfile.lock
--rw-r--r--   0        0        0     1927 2023-07-08 15:53:56.097660 heatmap_cli-0.1.1/README.md
--rw-r--r--   0        0        0      638 2023-07-08 15:37:49.954263 heatmap_cli-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2023-07-08 15:37:49.982263 heatmap_cli-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      779 2023-07-08 16:35:06.210774 heatmap_cli-0.1.1/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      837 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/heatmap_cli/__main__.py
--rw-r--r--   0        0        0     5395 2023-07-08 15:47:19.744050 heatmap_cli-0.1.1/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1077 2023-07-08 16:35:58.655379 heatmap_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 15:37:49.966263 heatmap_cli-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     5810 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      303 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/test_debug_flag.py
--rw-r--r--   0        0        0      326 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/test_help_flag.py
--rw-r--r--   0        0        0      545 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      306 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/tests/test_version_flag.py
--rw-r--r--   0        0        0      674 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/tox.ini
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 heatmap_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.coveragerc
+-rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.gitignore
+-rw-r--r--   0        0        0     2411 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.python-version
+-rw-r--r--   0        0        0      712 2023-07-10 16:30:45.947135 heatmap_cli-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2002 2023-07-10 15:30:51.824917 heatmap_cli-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      489 2023-07-10 15:32:42.498460 heatmap_cli-0.1.2/Pipfile
+-rw-r--r--   0        0        0   100071 2023-07-10 15:28:50.451408 heatmap_cli-0.1.2/Pipfile.lock
+-rw-r--r--   0        0        0     1927 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/README.md
+-rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0      779 2023-07-10 16:31:31.987887 heatmap_cli-0.1.2/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0     5395 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1077 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      303 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_help_flag.py
+-rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_version_flag.py
+-rw-r--r--   0        0        0      673 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tox.ini
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 heatmap_cli-0.1.2/PKG-INFO
```

### Comparing `heatmap_cli-0.1.1/.gitignore` & `heatmap_cli-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/.pre-commit-config.yaml` & `heatmap_cli-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/CONTRIBUTING.md` & `heatmap_cli-0.1.2/CONTRIBUTING.md`

 * *Files 27% similar despite different names*

```diff
@@ -6,28 +6,37 @@
 
 ```console
 git clone https://github.com/kianmeng/heatmap_cli
 cd heatmap_cli
 ```
 
 To set up different Python environments, we need to install all supported
-Python version using <https://github.com/pyenv/pyenv>. Once you've installed
-Pyenv, run the command below:
+Python version using <https://github.com/pyenv/pyenv>.
+
+Once you've installed Pyenv, install these additional Pyenv plugins:
 
 ```console
+git clone https://github.com/pyenv/pyenv-doctor.git "$(pyenv root)/plugins/pyenv-doctor"
+pyenv doctor
+
+git clone https://github.com/pyenv/pyenv-update.git $(pyenv root)/plugins/pyenv-update
 pyenv update
+```
+
+Run the command below to install all Python versions:
+
+```console
 pyenv install $(cat .python-version)
 ```
 
 Install necessary packages:
 
 ```console
-python -m pip install --upgrade pip pipenv pre-commit
+python -m pip install --upgrade pip pipenv
 pipenv install --dev
-pipenv install "-e ."
 ```
 
 Spawn a shell in virtual environment for your development:
 
 ```console
 pipenv shell
 ```
@@ -88,9 +97,10 @@
 git push origin my-new-feature
 ```
 
 Create new Pull Request in GitHub.
 
 ## License
 
-By contributing to heatmap_cli, you agree that your contributions will be licensed
-under the LICENSE.md file in the root directory of this source tree.
+By contributing to `heatmap_cli`, you agree that your contributions will be
+licensed under the [LICENSE.md)(./LICENSE.md) file in the root directory of
+this source tree.
```

### Comparing `heatmap_cli-0.1.1/LICENSE.md` & `heatmap_cli-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/Pipfile.lock` & `heatmap_cli-0.1.2/Pipfile.lock`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9543662437588494%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'635ce0c287e6f94d9a88fb77f2ebeeb34743e7f7b9aedf2ef1a8b76b66a7b2e7'}}",*

 * * "'default'": "{'pillow': {'hashes': {insert: [(3, "*

 * *              "'sha256:1ce91b6ec08d866b14413d3f0bbdea7e24dfdc8e59f562bb77bc3fe60b6144ca'), (33, "*

 * *              "'sha256:bc2ec7c7b5d66b8ec9ce9f720dbb5fa4bace0f545acd34870eff4a369b44bf37')]}}, "*

 * *              "'zipp': {'hashes': "*

 * *              "['sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941', "*

 * *              "'s […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "3ca75a6c9f5bce3c824dd0760065a90f1eeaca903a3e7dc06672fb64b1c2c046"
+            "sha256": "635ce0c287e6f94d9a88fb77f2ebeeb34743e7f7b9aedf2ef1a8b76b66a7b2e7"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.8"
         },
         "sources": [
             {
@@ -316,14 +316,15 @@
             "version": "==2.0.3"
         },
         "pillow": {
             "hashes": [
                 "sha256:00e65f5e822decd501e374b0650146063fbb30a7264b4d2744bdd7b913e0cab5",
                 "sha256:040586f7d37b34547153fa383f7f9aed68b738992380ac911447bb78f2abe530",
                 "sha256:0b6eb5502f45a60a3f411c63187db83a3d3107887ad0d036c13ce836f8a36f1d",
+                "sha256:1ce91b6ec08d866b14413d3f0bbdea7e24dfdc8e59f562bb77bc3fe60b6144ca",
                 "sha256:1f62406a884ae75fb2f818694469519fb685cc7eaff05d3451a9ebe55c646891",
                 "sha256:22c10cc517668d44b211717fd9775799ccec4124b9a7f7b3635fc5386e584992",
                 "sha256:3400aae60685b06bb96f99a21e1ada7bc7a413d5f49bce739828ecd9391bb8f7",
                 "sha256:349930d6e9c685c089284b013478d6f76e3a534e36ddfa912cde493f235372f3",
                 "sha256:368ab3dfb5f49e312231b6f27b8820c823652b7cd29cfbd34090565a015e99ba",
                 "sha256:38250a349b6b390ee6047a62c086d3817ac69022c127f8a5dc058c31ccef17f3",
                 "sha256:3a684105f7c32488f7153905a4e3015a3b6c7182e106fe3c37fbb5ef3e6994c3",
@@ -345,14 +346,15 @@
                 "sha256:9211e7ad69d7c9401cfc0e23d49b69ca65ddd898976d660a2fa5904e3d7a9baa",
                 "sha256:92be919bbc9f7d09f7ae343c38f5bb21c973d2576c1d45600fce4b74bafa7ac0",
                 "sha256:9c82b5b3e043c7af0d95792d0d20ccf68f61a1fec6b3530e718b688422727396",
                 "sha256:9f7c16705f44e0504a3a2a14197c1f0b32a95731d251777dcb060aa83022cb2d",
                 "sha256:9fb218c8a12e51d7ead2a7c9e101a04982237d4855716af2e9499306728fb485",
                 "sha256:a74ba0c356aaa3bb8e3eb79606a87669e7ec6444be352870623025d75a14a2bf",
                 "sha256:b4f69b3700201b80bb82c3a97d5e9254084f6dd5fb5b16fc1a7b974260f89f43",
+                "sha256:bc2ec7c7b5d66b8ec9ce9f720dbb5fa4bace0f545acd34870eff4a369b44bf37",
                 "sha256:c189af0545965fa8d3b9613cfdb0cd37f9d71349e0f7750e1fd704648d475ed2",
                 "sha256:c1fbe7621c167ecaa38ad29643d77a9ce7311583761abf7836e1510c580bf3dd",
                 "sha256:c7cf14a27b0d6adfaebb3ae4153f1e516df54e47e42dcc073d7b3d76111a8d86",
                 "sha256:c9f72a021fbb792ce98306ffb0c348b3c9cb967dce0f12a49aa4c3d3fdefa967",
                 "sha256:cd25d2a9d2b36fcb318882481367956d2cf91329f6892fe5d385c346c0649629",
                 "sha256:ce543ed15570eedbb85df19b0a1a7314a9c8141a36ce089c0a894adbfccb4568",
                 "sha256:ce7b031a6fc11365970e6a5686d7ba8c63e4c1cf1ea143811acbb524295eabed",
@@ -420,19 +422,19 @@
                 "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
             ],
             "markers": "python_version >= '2'",
             "version": "==2023.3"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941",
+                "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==3.15.0"
+            "version": "==3.16.0"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -541,14 +543,59 @@
                 "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
                 "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
                 "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==3.2.0"
         },
+        "contourpy": {
+            "hashes": [
+                "sha256:052cc634bf903c604ef1a00a5aa093c54f81a2612faedaa43295809ffdde885e",
+                "sha256:084eaa568400cfaf7179b847ac871582199b1b44d5699198e9602ecbbb5f6104",
+                "sha256:0b6616375d7de55797d7a66ee7d087efe27f03d336c27cf1f32c02b8c1a5ac70",
+                "sha256:0b7b04ed0961647691cfe5d82115dd072af7ce8846d31a5fac6c142dcce8b882",
+                "sha256:143dde50520a9f90e4a2703f367cf8ec96a73042b72e68fcd184e1279962eb6f",
+                "sha256:17cfaf5ec9862bc93af1ec1f302457371c34e688fbd381f4035a06cd47324f48",
+                "sha256:181cbace49874f4358e2929aaf7ba84006acb76694102e88dd15af861996c16e",
+                "sha256:189ceb1525eb0655ab8487a9a9c41f42a73ba52d6789754788d1883fb06b2d8a",
+                "sha256:18a64814ae7bce73925131381603fff0116e2df25230dfc80d6d690aa6e20b37",
+                "sha256:1f0cbd657e9bde94cd0e33aa7df94fb73c1ab7799378d3b3f902eb8eb2e04a3a",
+                "sha256:1f795597073b09d631782e7245016a4323cf1cf0b4e06eef7ea6627e06a37ff2",
+                "sha256:25ae46595e22f93592d39a7eac3d638cda552c3e1160255258b695f7b58e5655",
+                "sha256:27bc79200c742f9746d7dd51a734ee326a292d77e7d94c8af6e08d1e6c15d545",
+                "sha256:2b836d22bd2c7bb2700348e4521b25e077255ebb6ab68e351ab5aa91ca27e027",
+                "sha256:30f511c05fab7f12e0b1b7730ebdc2ec8deedcfb505bc27eb570ff47c51a8f15",
+                "sha256:317267d915490d1e84577924bd61ba71bf8681a30e0d6c545f577363157e5e94",
+                "sha256:397b0ac8a12880412da3551a8cb5a187d3298a72802b45a3bd1805e204ad8439",
+                "sha256:438ba416d02f82b692e371858143970ed2eb6337d9cdbbede0d8ad9f3d7dd17d",
+                "sha256:53cc3a40635abedbec7f1bde60f8c189c49e84ac180c665f2cd7c162cc454baa",
+                "sha256:5d123a5bc63cd34c27ff9c7ac1cd978909e9c71da12e05be0231c608048bb2ae",
+                "sha256:62013a2cf68abc80dadfd2307299bfa8f5aa0dcaec5b2954caeb5fa094171103",
+                "sha256:89f06eff3ce2f4b3eb24c1055a26981bffe4e7264acd86f15b97e40530b794bc",
+                "sha256:90c81f22b4f572f8a2110b0b741bb64e5a6427e0a198b2cdc1fbaf85f352a3aa",
+                "sha256:911ff4fd53e26b019f898f32db0d4956c9d227d51338fb3b03ec72ff0084ee5f",
+                "sha256:9382a1c0bc46230fb881c36229bfa23d8c303b889b788b939365578d762b5c18",
+                "sha256:9f2931ed4741f98f74b410b16e5213f71dcccee67518970c42f64153ea9313b9",
+                "sha256:a67259c2b493b00e5a4d0f7bfae51fb4b3371395e47d079a4446e9b0f4d70e76",
+                "sha256:a698c6a7a432789e587168573a864a7ea374c6be8d4f31f9d87c001d5a843493",
+                "sha256:bc00bb4225d57bff7ebb634646c0ee2a1298402ec10a5fe7af79df9a51c1bfd9",
+                "sha256:bcb41692aa09aeb19c7c213411854402f29f6613845ad2453d30bf421fe68fed",
+                "sha256:d4f26b25b4f86087e7d75e63212756c38546e70f2a92d2be44f80114826e1cd4",
+                "sha256:d551f3a442655f3dcc1285723f9acd646ca5858834efeab4598d706206b09c9f",
+                "sha256:dffcc2ddec1782dd2f2ce1ef16f070861af4fb78c69862ce0aab801495dda6a3",
+                "sha256:e53046c3863828d21d531cc3b53786e6580eb1ba02477e8681009b6aa0870b21",
+                "sha256:e5cec36c5090e75a9ac9dbd0ff4a8cf7cecd60f1b6dc23a374c7d980a1cd710e",
+                "sha256:e7a117ce7df5a938fe035cad481b0189049e8d92433b4b33aa7fc609344aafa1",
+                "sha256:e94bef2580e25b5fdb183bf98a2faa2adc5b638736b2c0a4da98691da641316a",
+                "sha256:ed614aea8462735e7d70141374bd7650afd1c3f3cb0c2dbbcbe44e14331bf002",
+                "sha256:fb3b7d9e6243bfa1efb93ccfe64ec610d85cfe5aec2c25f97fbbd2e58b531256"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==1.1.0"
+        },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
                 "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
                 "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
@@ -610,14 +657,22 @@
                 "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
                 "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==7.2.7"
         },
+        "cycler": {
+            "hashes": [
+                "sha256:3a27e95f763a428a739d2add979fa7494c912a32c17c4c38c4d5f082cad165a3",
+                "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==0.11.0"
+        },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
@@ -635,19 +690,19 @@
                 "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.2"
         },
         "execnet": {
             "hashes": [
-                "sha256:9e30983ff42c20bac5b18807910512058b12a79f6bccddd9ce813bf22b079a9c",
-                "sha256:c98d4317b0c8ddcfea75523d6ace65c694b606d00d74e7a22e5209093bb94798"
+                "sha256:88256416ae766bc9e8895c76a87928c0012183da3cc4fc18016e6f050e025f41",
+                "sha256:cc59bc4423742fd71ad227122eb0dd44db51efb3dc4095b45ac9a08c770096af"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.0"
+            "version": "==2.0.2"
         },
         "filelock": {
             "hashes": [
                 "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
                 "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
@@ -665,14 +720,58 @@
             "hashes": [
                 "sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba",
                 "sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.9.0"
         },
+        "fonttools": {
+            "hashes": [
+                "sha256:00ab569b2a3e591e00425023ade87e8fef90380c1dde61be7691cb524ca5f743",
+                "sha256:022c4a16b412293e7f1ce21b8bab7a6f9d12c4ffdf171fdc67122baddb973069",
+                "sha256:05171f3c546f64d78569f10adc0de72561882352cac39ec7439af12304d8d8c0",
+                "sha256:14037c31138fbd21847ad5e5441dfdde003e0a8f3feb5812a1a21fd1c255ffbd",
+                "sha256:15abb3d055c1b2dff9ce376b6c3db10777cb74b37b52b78f61657634fd348a0d",
+                "sha256:18ea64ac43e94c9e0c23d7a9475f1026be0e25b10dda8f236fc956188761df97",
+                "sha256:1a003608400dd1cca3e089e8c94973c6b51a4fb1ef00ff6d7641617b9242e637",
+                "sha256:1bc4c5b147be8dbc5df9cc8ac5e93ee914ad030fe2a201cc8f02f499db71011d",
+                "sha256:200729d12461e2038700d31f0d49ad5a7b55855dec7525074979a06b46f88505",
+                "sha256:337b6e83d7ee73c40ea62407f2ce03b07c3459e213b6f332b94a69923b9e1cb9",
+                "sha256:37467cee0f32cada2ec08bc16c9c31f9b53ea54b2f5604bf25a1246b5f50593a",
+                "sha256:425b74a608427499b0e45e433c34ddc350820b6f25b7c8761963a08145157a66",
+                "sha256:530c5d35109f3e0cea2535742d6a3bc99c0786cf0cbd7bb2dc9212387f0d908c",
+                "sha256:56d4d85f5374b45b08d2f928517d1e313ea71b4847240398decd0ab3ebbca885",
+                "sha256:5e00334c66f4e83535384cb5339526d01d02d77f142c23b2f97bd6a4f585497a",
+                "sha256:5fdf60f8a5c6bcce7d024a33f7e4bc7921f5b74e8ea13bccd204f2c8b86f3470",
+                "sha256:6a8d71b9a5c884c72741868e845c0e563c5d83dcaf10bb0ceeec3b4b2eb14c67",
+                "sha256:6d5adf4ba114f028fc3f5317a221fd8b0f4ef7a2e5524a2b1e0fd891b093791a",
+                "sha256:7449e5e306f3a930a8944c85d0cbc8429cba13503372a1a40f23124d6fb09b58",
+                "sha256:7961575221e3da0841c75da53833272c520000d76f7f71274dbf43370f8a1065",
+                "sha256:7f6e3fa3da923063c286320e728ba2270e49c73386e3a711aa680f4b0747d692",
+                "sha256:882983279bf39afe4e945109772c2ffad2be2c90983d6559af8b75c19845a80a",
+                "sha256:8a917828dbfdb1cbe50cf40eeae6fbf9c41aef9e535649ed8f4982b2ef65c091",
+                "sha256:8c4305b171b61040b1ee75d18f9baafe58bd3b798d1670078efe2c92436bfb63",
+                "sha256:91784e21a1a085fac07c6a407564f4a77feb471b5954c9ee55a4f9165151f6c1",
+                "sha256:94c915f6716589f78bc00fbc14c5b8de65cfd11ee335d32504f1ef234524cb24",
+                "sha256:97d95b8301b62bdece1af943b88bcb3680fd385f88346a4a899ee145913b414a",
+                "sha256:a954b90d1473c85a22ecf305761d9fd89da93bbd31dae86e7dea436ad2cb5dc9",
+                "sha256:aa83b3f151bc63970f39b2b42a06097c5a22fd7ed9f7ba008e618de4503d3895",
+                "sha256:b802dcbf9bcff74672f292b2466f6589ab8736ce4dcf36f48eb994c2847c4b30",
+                "sha256:bae8c13abbc2511e9a855d2142c0ab01178dd66b1a665798f357da0d06253e0d",
+                "sha256:c55f1b4109dbc3aeb496677b3e636d55ef46dc078c2a5e3f3db4e90f1c6d2907",
+                "sha256:eb52c10fda31159c22c7ed85074e05f8b97da8773ea461706c273e31bcbea836",
+                "sha256:ec468c022d09f1817c691cf884feb1030ef6f1e93e3ea6831b0d8144c06480d1"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==4.40.0"
+        },
+        "heatmap-cli": {
+            "editable": true,
+            "path": "."
+        },
         "identify": {
             "hashes": [
                 "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
                 "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.5.24"
@@ -697,14 +796,22 @@
             "hashes": [
                 "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
                 "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
             ],
             "markers": "python_version < '3.10'",
             "version": "==6.8.0"
         },
+        "importlib-resources": {
+            "hashes": [
+                "sha256:4cf94875a8368bd89531a756df9a9ebe1f150e0f885030b461237bc7f2d905f2",
+                "sha256:d952faee11004c045f785bb5636e8f885bed30dc3c940d5d42798a2a4541c185"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==6.0.0"
+        },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
@@ -713,14 +820,88 @@
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
+        "kiwisolver": {
+            "hashes": [
+                "sha256:02f79693ec433cb4b5f51694e8477ae83b3205768a6fb48ffba60549080e295b",
+                "sha256:03baab2d6b4a54ddbb43bba1a3a2d1627e82d205c5cf8f4c924dc49284b87166",
+                "sha256:1041feb4cda8708ce73bb4dcb9ce1ccf49d553bf87c3954bdfa46f0c3f77252c",
+                "sha256:10ee06759482c78bdb864f4109886dff7b8a56529bc1609d4f1112b93fe6423c",
+                "sha256:1d1573129aa0fd901076e2bfb4275a35f5b7aa60fbfb984499d661ec950320b0",
+                "sha256:283dffbf061a4ec60391d51e6155e372a1f7a4f5b15d59c8505339454f8989e4",
+                "sha256:28bc5b299f48150b5f822ce68624e445040595a4ac3d59251703779836eceff9",
+                "sha256:2a66fdfb34e05b705620dd567f5a03f239a088d5a3f321e7b6ac3239d22aa286",
+                "sha256:2e307eb9bd99801f82789b44bb45e9f541961831c7311521b13a6c85afc09767",
+                "sha256:2e407cb4bd5a13984a6c2c0fe1845e4e41e96f183e5e5cd4d77a857d9693494c",
+                "sha256:2f5e60fabb7343a836360c4f0919b8cd0d6dbf08ad2ca6b9cf90bf0c76a3c4f6",
+                "sha256:36dafec3d6d6088d34e2de6b85f9d8e2324eb734162fba59d2ba9ed7a2043d5b",
+                "sha256:3fe20f63c9ecee44560d0e7f116b3a747a5d7203376abeea292ab3152334d004",
+                "sha256:41dae968a94b1ef1897cb322b39360a0812661dba7c682aa45098eb8e193dbdf",
+                "sha256:4bd472dbe5e136f96a4b18f295d159d7f26fd399136f5b17b08c4e5f498cd494",
+                "sha256:4ea39b0ccc4f5d803e3337dd46bcce60b702be4d86fd0b3d7531ef10fd99a1ac",
+                "sha256:5853eb494c71e267912275e5586fe281444eb5e722de4e131cddf9d442615626",
+                "sha256:5bce61af018b0cb2055e0e72e7d65290d822d3feee430b7b8203d8a855e78766",
+                "sha256:6295ecd49304dcf3bfbfa45d9a081c96509e95f4b9d0eb7ee4ec0530c4a96514",
+                "sha256:62ac9cc684da4cf1778d07a89bf5f81b35834cb96ca523d3a7fb32509380cbf6",
+                "sha256:70e7c2e7b750585569564e2e5ca9845acfaa5da56ac46df68414f29fea97be9f",
+                "sha256:7577c1987baa3adc4b3c62c33bd1118c3ef5c8ddef36f0f2c950ae0b199e100d",
+                "sha256:75facbe9606748f43428fc91a43edb46c7ff68889b91fa31f53b58894503a191",
+                "sha256:787518a6789009c159453da4d6b683f468ef7a65bbde796bcea803ccf191058d",
+                "sha256:78d6601aed50c74e0ef02f4204da1816147a6d3fbdc8b3872d263338a9052c51",
+                "sha256:7c43e1e1206cd421cd92e6b3280d4385d41d7166b3ed577ac20444b6995a445f",
+                "sha256:81e38381b782cc7e1e46c4e14cd997ee6040768101aefc8fa3c24a4cc58e98f8",
+                "sha256:841293b17ad704d70c578f1f0013c890e219952169ce8a24ebc063eecf775454",
+                "sha256:872b8ca05c40d309ed13eb2e582cab0c5a05e81e987ab9c521bf05ad1d5cf5cb",
+                "sha256:877272cf6b4b7e94c9614f9b10140e198d2186363728ed0f701c6eee1baec1da",
+                "sha256:8c808594c88a025d4e322d5bb549282c93c8e1ba71b790f539567932722d7bd8",
+                "sha256:8ed58b8acf29798b036d347791141767ccf65eee7f26bde03a71c944449e53de",
+                "sha256:91672bacaa030f92fc2f43b620d7b337fd9a5af28b0d6ed3f77afc43c4a64b5a",
+                "sha256:968f44fdbf6dd757d12920d63b566eeb4d5b395fd2d00d29d7ef00a00582aac9",
+                "sha256:9f85003f5dfa867e86d53fac6f7e6f30c045673fa27b603c397753bebadc3008",
+                "sha256:a553dadda40fef6bfa1456dc4be49b113aa92c2a9a9e8711e955618cd69622e3",
+                "sha256:a68b62a02953b9841730db7797422f983935aeefceb1679f0fc85cbfbd311c32",
+                "sha256:abbe9fa13da955feb8202e215c4018f4bb57469b1b78c7a4c5c7b93001699938",
+                "sha256:ad881edc7ccb9d65b0224f4e4d05a1e85cf62d73aab798943df6d48ab0cd79a1",
+                "sha256:b1792d939ec70abe76f5054d3f36ed5656021dcad1322d1cc996d4e54165cef9",
+                "sha256:b428ef021242344340460fa4c9185d0b1f66fbdbfecc6c63eff4b7c29fad429d",
+                "sha256:b533558eae785e33e8c148a8d9921692a9fe5aa516efbdff8606e7d87b9d5824",
+                "sha256:ba59c92039ec0a66103b1d5fe588fa546373587a7d68f5c96f743c3396afc04b",
+                "sha256:bc8d3bd6c72b2dd9decf16ce70e20abcb3274ba01b4e1c96031e0c4067d1e7cd",
+                "sha256:bc9db8a3efb3e403e4ecc6cd9489ea2bac94244f80c78e27c31dcc00d2790ac2",
+                "sha256:bf7d9fce9bcc4752ca4a1b80aabd38f6d19009ea5cbda0e0856983cf6d0023f5",
+                "sha256:c2dbb44c3f7e6c4d3487b31037b1bdbf424d97687c1747ce4ff2895795c9bf69",
+                "sha256:c79ebe8f3676a4c6630fd3f777f3cfecf9289666c84e775a67d1d358578dc2e3",
+                "sha256:c97528e64cb9ebeff9701e7938653a9951922f2a38bd847787d4a8e498cc83ae",
+                "sha256:d0611a0a2a518464c05ddd5a3a1a0e856ccc10e67079bb17f265ad19ab3c7597",
+                "sha256:d06adcfa62a4431d404c31216f0f8ac97397d799cd53800e9d3efc2fbb3cf14e",
+                "sha256:d41997519fcba4a1e46eb4a2fe31bc12f0ff957b2b81bac28db24744f333e955",
+                "sha256:d5b61785a9ce44e5a4b880272baa7cf6c8f48a5180c3e81c59553ba0cb0821ca",
+                "sha256:da152d8cdcab0e56e4f45eb08b9aea6455845ec83172092f09b0e077ece2cf7a",
+                "sha256:da7e547706e69e45d95e116e6939488d62174e033b763ab1496b4c29b76fabea",
+                "sha256:db5283d90da4174865d520e7366801a93777201e91e79bacbac6e6927cbceede",
+                "sha256:db608a6757adabb32f1cfe6066e39b3706d8c3aa69bbc353a5b61edad36a5cb4",
+                "sha256:e0ea21f66820452a3f5d1655f8704a60d66ba1191359b96541eaf457710a5fc6",
+                "sha256:e7da3fec7408813a7cebc9e4ec55afed2d0fd65c4754bc376bf03498d4e92686",
+                "sha256:e92a513161077b53447160b9bd8f522edfbed4bd9759e4c18ab05d7ef7e49408",
+                "sha256:ecb1fa0db7bf4cff9dac752abb19505a233c7f16684c5826d1f11ebd9472b871",
+                "sha256:efda5fc8cc1c61e4f639b8067d118e742b812c930f708e6667a5ce0d13499e29",
+                "sha256:f0a1dbdb5ecbef0d34eb77e56fcb3e95bbd7e50835d9782a45df81cc46949750",
+                "sha256:f0a71d85ecdd570ded8ac3d1c0f480842f49a40beb423bb8014539a9f32a5897",
+                "sha256:f4f270de01dd3e129a72efad823da90cc4d6aafb64c410c9033aba70db9f1ff0",
+                "sha256:f6cb459eea32a4e2cf18ba5fcece2dbdf496384413bc1bae15583f19e567f3b2",
+                "sha256:f8ad8285b01b0d4695102546b342b493b3ccc6781fc28c8c6a1bb63e95d22f09",
+                "sha256:f9f39e2f049db33a908319cf46624a569b36983c7c78318e9726a4cb8923b26c"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.4.4"
+        },
         "markdown-it-py": {
             "hashes": [
                 "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
                 "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.0.0"
@@ -777,14 +958,61 @@
                 "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
                 "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
                 "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.1.3"
         },
+        "matplotlib": {
+            "hashes": [
+                "sha256:070f8dddd1f5939e60aacb8fa08f19551f4b0140fab16a3669d5cd6e9cb28fc8",
+                "sha256:0c3cca3e842b11b55b52c6fb8bd6a4088693829acbfcdb3e815fa9b7d5c92c1b",
+                "sha256:0f506a1776ee94f9e131af1ac6efa6e5bc7cb606a3e389b0ccb6e657f60bb676",
+                "sha256:12f01b92ecd518e0697da4d97d163b2b3aa55eb3eb4e2c98235b3396d7dad55f",
+                "sha256:152ee0b569a37630d8628534c628456b28686e085d51394da6b71ef84c4da201",
+                "sha256:1c308b255efb9b06b23874236ec0f10f026673ad6515f602027cc8ac7805352d",
+                "sha256:1cd120fca3407a225168238b790bd5c528f0fafde6172b140a2f3ab7a4ea63e9",
+                "sha256:20f844d6be031948148ba49605c8b96dfe7d3711d1b63592830d650622458c11",
+                "sha256:23fb1750934e5f0128f9423db27c474aa32534cec21f7b2153262b066a581fd1",
+                "sha256:2699f7e73a76d4c110f4f25be9d2496d6ab4f17345307738557d345f099e07de",
+                "sha256:26bede320d77e469fdf1bde212de0ec889169b04f7f1179b8930d66f82b30cbc",
+                "sha256:2ecb5be2b2815431c81dc115667e33da0f5a1bcf6143980d180d09a717c4a12e",
+                "sha256:2f8e4a49493add46ad4a8c92f63e19d548b2b6ebbed75c6b4c7f46f57d36cdd1",
+                "sha256:305e3da477dc8607336ba10bac96986d6308d614706cae2efe7d3ffa60465b24",
+                "sha256:30e1409b857aa8a747c5d4f85f63a79e479835f8dffc52992ac1f3f25837b544",
+                "sha256:318c89edde72ff95d8df67d82aca03861240512994a597a435a1011ba18dbc7f",
+                "sha256:35d74ebdb3f71f112b36c2629cf32323adfbf42679e2751252acd468f5001c07",
+                "sha256:50e0a55ec74bf2d7a0ebf50ac580a209582c2dd0f7ab51bc270f1b4a0027454e",
+                "sha256:5dea00b62d28654b71ca92463656d80646675628d0828e08a5f3b57e12869e13",
+                "sha256:60c521e21031632aa0d87ca5ba0c1c05f3daacadb34c093585a0be6780f698e4",
+                "sha256:6515e878f91894c2e4340d81f0911857998ccaf04dbc1bba781e3d89cbf70608",
+                "sha256:6d2ff3c984b8a569bc1383cd468fc06b70d7b59d5c2854ca39f1436ae8394117",
+                "sha256:71667eb2ccca4c3537d9414b1bc00554cb7f91527c17ee4ec38027201f8f1603",
+                "sha256:717157e61b3a71d3d26ad4e1770dc85156c9af435659a25ee6407dc866cb258d",
+                "sha256:71f7a8c6b124e904db550f5b9fe483d28b896d4135e45c4ea381ad3b8a0e3256",
+                "sha256:936bba394682049919dda062d33435b3be211dc3dcaa011e09634f060ec878b2",
+                "sha256:a1733b8e84e7e40a9853e505fe68cc54339f97273bdfe6f3ed980095f769ddc7",
+                "sha256:a2c1590b90aa7bd741b54c62b78de05d4186271e34e2377e0289d943b3522273",
+                "sha256:a7e28d6396563955f7af437894a36bf2b279462239a41028323e04b85179058b",
+                "sha256:a8035ba590658bae7562786c9cc6ea1a84aa49d3afab157e414c9e2ea74f496d",
+                "sha256:a8cdb91dddb04436bd2f098b8fdf4b81352e68cf4d2c6756fcc414791076569b",
+                "sha256:ac60daa1dc83e8821eed155796b0f7888b6b916cf61d620a4ddd8200ac70cd64",
+                "sha256:af4860132c8c05261a5f5f8467f1b269bf1c7c23902d75f2be57c4a7f2394b3e",
+                "sha256:bc221ffbc2150458b1cd71cdd9ddd5bb37962b036e41b8be258280b5b01da1dd",
+                "sha256:ce55289d5659b5b12b3db4dc9b7075b70cef5631e56530f14b2945e8836f2d20",
+                "sha256:d9881356dc48e58910c53af82b57183879129fa30492be69058c5b0d9fddf391",
+                "sha256:dbcf59334ff645e6a67cd5f78b4b2cdb76384cdf587fa0d2dc85f634a72e1a3e",
+                "sha256:ebf577c7a6744e9e1bd3fee45fc74a02710b214f94e2bde344912d85e0c9af7c",
+                "sha256:f081c03f413f59390a80b3e351cc2b2ea0205839714dbc364519bcf51f4b56ca",
+                "sha256:fdbb46fad4fb47443b5b8ac76904b2e7a66556844f33370861b4788db0f8816a",
+                "sha256:fdcd28360dbb6203fb5219b1a5658df226ac9bebc2542a9e8f457de959d713d0"
+            ],
+            "index": "pypi",
+            "version": "==3.7.2"
+        },
         "mdit-py-plugins": {
             "hashes": [
                 "sha256:b51b3bb70691f57f974e257e367107857a93b36f322a9e6d44ca5bf28ec2def9",
                 "sha256:d8ab27e9aed6c38aa716819fedfde15ca275715955f8a185a8e1cf90fb1d2c1b"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.4.0"
@@ -809,22 +1037,149 @@
             "hashes": [
                 "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
                 "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==1.8.0"
         },
+        "numpy": {
+            "hashes": [
+                "sha256:04640dab83f7c6c85abf9cd729c5b65f1ebd0ccf9de90b270cd61935eef0197f",
+                "sha256:1452241c290f3e2a312c137a9999cdbf63f78864d63c79039bda65ee86943f61",
+                "sha256:222e40d0e2548690405b0b3c7b21d1169117391c2e82c378467ef9ab4c8f0da7",
+                "sha256:2541312fbf09977f3b3ad449c4e5f4bb55d0dbf79226d7724211acc905049400",
+                "sha256:31f13e25b4e304632a4619d0e0777662c2ffea99fcae2029556b17d8ff958aef",
+                "sha256:4602244f345453db537be5314d3983dbf5834a9701b7723ec28923e2889e0bb2",
+                "sha256:4979217d7de511a8d57f4b4b5b2b965f707768440c17cb70fbf254c4b225238d",
+                "sha256:4c21decb6ea94057331e111a5bed9a79d335658c27ce2adb580fb4d54f2ad9bc",
+                "sha256:6620c0acd41dbcb368610bb2f4d83145674040025e5536954782467100aa8835",
+                "sha256:692f2e0f55794943c5bfff12b3f56f99af76f902fc47487bdfe97856de51a706",
+                "sha256:7215847ce88a85ce39baf9e89070cb860c98fdddacbaa6c0da3ffb31b3350bd5",
+                "sha256:79fc682a374c4a8ed08b331bef9c5f582585d1048fa6d80bc6c35bc384eee9b4",
+                "sha256:7ffe43c74893dbf38c2b0a1f5428760a1a9c98285553c89e12d70a96a7f3a4d6",
+                "sha256:80f5e3a4e498641401868df4208b74581206afbee7cf7b8329daae82676d9463",
+                "sha256:95f7ac6540e95bc440ad77f56e520da5bf877f87dca58bd095288dce8940532a",
+                "sha256:9667575fb6d13c95f1b36aca12c5ee3356bf001b714fc354eb5465ce1609e62f",
+                "sha256:a5425b114831d1e77e4b5d812b69d11d962e104095a5b9c3b641a218abcc050e",
+                "sha256:b4bea75e47d9586d31e892a7401f76e909712a0fd510f58f5337bea9572c571e",
+                "sha256:b7b1fc9864d7d39e28f41d089bfd6353cb5f27ecd9905348c24187a768c79694",
+                "sha256:befe2bf740fd8373cf56149a5c23a0f601e82869598d41f8e188a0e9869926f8",
+                "sha256:c0bfb52d2169d58c1cdb8cc1f16989101639b34c7d3ce60ed70b19c63eba0b64",
+                "sha256:d11efb4dbecbdf22508d55e48d9c8384db795e1b7b51ea735289ff96613ff74d",
+                "sha256:dd80e219fd4c71fc3699fc1dadac5dcf4fd882bfc6f7ec53d30fa197b8ee22dc",
+                "sha256:e2926dac25b313635e4d6cf4dc4e51c8c0ebfed60b801c799ffc4c32bf3d1254",
+                "sha256:e98f220aa76ca2a977fe435f5b04d7b3470c0a2e6312907b37ba6068f26787f2",
+                "sha256:ed094d4f0c177b1b8e7aa9cba7d6ceed51c0e569a5318ac0ca9a090680a6a1b1",
+                "sha256:f136bab9c2cfd8da131132c2cf6cc27331dd6fae65f95f69dcd4ae3c3639c810",
+                "sha256:f3a86ed21e4f87050382c7bc96571755193c4c1392490744ac73d660e8f564a9"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==1.24.4"
+        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
+        "pandas": {
+            "hashes": [
+                "sha256:04dbdbaf2e4d46ca8da896e1805bc04eb85caa9a82e259e8eed00254d5e0c682",
+                "sha256:1168574b036cd8b93abc746171c9b4f1b83467438a5e45909fed645cf8692dbc",
+                "sha256:1994c789bf12a7c5098277fb43836ce090f1073858c10f9220998ac74f37c69b",
+                "sha256:258d3624b3ae734490e4d63c430256e716f488c4fcb7c8e9bde2d3aa46c29089",
+                "sha256:32fca2ee1b0d93dd71d979726b12b61faa06aeb93cf77468776287f41ff8fdc5",
+                "sha256:37673e3bdf1551b95bf5d4ce372b37770f9529743d2498032439371fc7b7eb26",
+                "sha256:3ef285093b4fe5058eefd756100a367f27029913760773c8bf1d2d8bebe5d210",
+                "sha256:5247fb1ba347c1261cbbf0fcfba4a3121fbb4029d95d9ef4dc45406620b25c8b",
+                "sha256:5ec591c48e29226bcbb316e0c1e9423622bc7a4eaf1ef7c3c9fa1a3981f89641",
+                "sha256:694888a81198786f0e164ee3a581df7d505024fbb1f15202fc7db88a71d84ebd",
+                "sha256:69d7f3884c95da3a31ef82b7618af5710dba95bb885ffab339aad925c3e8ce78",
+                "sha256:6a21ab5c89dcbd57f78d0ae16630b090eec626360085a4148693def5452d8a6b",
+                "sha256:81af086f4543c9d8bb128328b5d32e9986e0c84d3ee673a2ac6fb57fd14f755e",
+                "sha256:9e4da0d45e7f34c069fe4d522359df7d23badf83abc1d1cef398895822d11061",
+                "sha256:9eae3dc34fa1aa7772dd3fc60270d13ced7346fcbcfee017d3132ec625e23bb0",
+                "sha256:9ee1a69328d5c36c98d8e74db06f4ad518a1840e8ccb94a4ba86920986bb617e",
+                "sha256:b084b91d8d66ab19f5bb3256cbd5ea661848338301940e17f4492b2ce0801fe8",
+                "sha256:b9cb1e14fdb546396b7e1b923ffaeeac24e4cedd14266c3497216dd4448e4f2d",
+                "sha256:ba619e410a21d8c387a1ea6e8a0e49bb42216474436245718d7f2e88a2f8d7c0",
+                "sha256:c02f372a88e0d17f36d3093a644c73cfc1788e876a7c4bcb4020a77512e2043c",
+                "sha256:ce0c6f76a0f1ba361551f3e6dceaff06bde7514a374aa43e33b588ec10420183",
+                "sha256:d9cd88488cceb7635aebb84809d087468eb33551097d600c6dad13602029c2df",
+                "sha256:e4c7c9f27a4185304c7caf96dc7d91bc60bc162221152de697c98eb0b2648dd8",
+                "sha256:f167beed68918d62bffb6ec64f2e1d8a7d297a038f86d4aed056b9493fca407f",
+                "sha256:f3421a7afb1a43f7e38e82e844e2bca9a6d793d66c1a7f9f0ff39a795bbc5e02"
+            ],
+            "index": "pypi",
+            "version": "==2.0.3"
+        },
+        "pillow": {
+            "hashes": [
+                "sha256:00e65f5e822decd501e374b0650146063fbb30a7264b4d2744bdd7b913e0cab5",
+                "sha256:040586f7d37b34547153fa383f7f9aed68b738992380ac911447bb78f2abe530",
+                "sha256:0b6eb5502f45a60a3f411c63187db83a3d3107887ad0d036c13ce836f8a36f1d",
+                "sha256:1ce91b6ec08d866b14413d3f0bbdea7e24dfdc8e59f562bb77bc3fe60b6144ca",
+                "sha256:1f62406a884ae75fb2f818694469519fb685cc7eaff05d3451a9ebe55c646891",
+                "sha256:22c10cc517668d44b211717fd9775799ccec4124b9a7f7b3635fc5386e584992",
+                "sha256:3400aae60685b06bb96f99a21e1ada7bc7a413d5f49bce739828ecd9391bb8f7",
+                "sha256:349930d6e9c685c089284b013478d6f76e3a534e36ddfa912cde493f235372f3",
+                "sha256:368ab3dfb5f49e312231b6f27b8820c823652b7cd29cfbd34090565a015e99ba",
+                "sha256:38250a349b6b390ee6047a62c086d3817ac69022c127f8a5dc058c31ccef17f3",
+                "sha256:3a684105f7c32488f7153905a4e3015a3b6c7182e106fe3c37fbb5ef3e6994c3",
+                "sha256:3a82c40d706d9aa9734289740ce26460a11aeec2d9c79b7af87bb35f0073c12f",
+                "sha256:3b08d4cc24f471b2c8ca24ec060abf4bebc6b144cb89cba638c720546b1cf538",
+                "sha256:3ed64f9ca2f0a95411e88a4efbd7a29e5ce2cea36072c53dd9d26d9c76f753b3",
+                "sha256:3f07ea8d2f827d7d2a49ecf1639ec02d75ffd1b88dcc5b3a61bbb37a8759ad8d",
+                "sha256:520f2a520dc040512699f20fa1c363eed506e94248d71f85412b625026f6142c",
+                "sha256:5c6e3df6bdd396749bafd45314871b3d0af81ff935b2d188385e970052091017",
+                "sha256:608bfdee0d57cf297d32bcbb3c728dc1da0907519d1784962c5f0c68bb93e5a3",
+                "sha256:685ac03cc4ed5ebc15ad5c23bc555d68a87777586d970c2c3e216619a5476223",
+                "sha256:76de421f9c326da8f43d690110f0e79fe3ad1e54be811545d7d91898b4c8493e",
+                "sha256:76edb0a1fa2b4745fb0c99fb9fb98f8b180a1bbceb8be49b087e0b21867e77d3",
+                "sha256:7be600823e4c8631b74e4a0d38384c73f680e6105a7d3c6824fcf226c178c7e6",
+                "sha256:81ff539a12457809666fef6624684c008e00ff6bf455b4b89fd00a140eecd640",
+                "sha256:88af2003543cc40c80f6fca01411892ec52b11021b3dc22ec3bc9d5afd1c5334",
+                "sha256:8c11160913e3dd06c8ffdb5f233a4f254cb449f4dfc0f8f4549eda9e542c93d1",
+                "sha256:8f8182b523b2289f7c415f589118228d30ac8c355baa2f3194ced084dac2dbba",
+                "sha256:9211e7ad69d7c9401cfc0e23d49b69ca65ddd898976d660a2fa5904e3d7a9baa",
+                "sha256:92be919bbc9f7d09f7ae343c38f5bb21c973d2576c1d45600fce4b74bafa7ac0",
+                "sha256:9c82b5b3e043c7af0d95792d0d20ccf68f61a1fec6b3530e718b688422727396",
+                "sha256:9f7c16705f44e0504a3a2a14197c1f0b32a95731d251777dcb060aa83022cb2d",
+                "sha256:9fb218c8a12e51d7ead2a7c9e101a04982237d4855716af2e9499306728fb485",
+                "sha256:a74ba0c356aaa3bb8e3eb79606a87669e7ec6444be352870623025d75a14a2bf",
+                "sha256:b4f69b3700201b80bb82c3a97d5e9254084f6dd5fb5b16fc1a7b974260f89f43",
+                "sha256:bc2ec7c7b5d66b8ec9ce9f720dbb5fa4bace0f545acd34870eff4a369b44bf37",
+                "sha256:c189af0545965fa8d3b9613cfdb0cd37f9d71349e0f7750e1fd704648d475ed2",
+                "sha256:c1fbe7621c167ecaa38ad29643d77a9ce7311583761abf7836e1510c580bf3dd",
+                "sha256:c7cf14a27b0d6adfaebb3ae4153f1e516df54e47e42dcc073d7b3d76111a8d86",
+                "sha256:c9f72a021fbb792ce98306ffb0c348b3c9cb967dce0f12a49aa4c3d3fdefa967",
+                "sha256:cd25d2a9d2b36fcb318882481367956d2cf91329f6892fe5d385c346c0649629",
+                "sha256:ce543ed15570eedbb85df19b0a1a7314a9c8141a36ce089c0a894adbfccb4568",
+                "sha256:ce7b031a6fc11365970e6a5686d7ba8c63e4c1cf1ea143811acbb524295eabed",
+                "sha256:d35e3c8d9b1268cbf5d3670285feb3528f6680420eafe35cccc686b73c1e330f",
+                "sha256:d50b6aec14bc737742ca96e85d6d0a5f9bfbded018264b3b70ff9d8c33485551",
+                "sha256:d5d0dae4cfd56969d23d94dc8e89fb6a217be461c69090768227beb8ed28c0a3",
+                "sha256:d5db32e2a6ccbb3d34d87c87b432959e0db29755727afb37290e10f6e8e62614",
+                "sha256:d72e2ecc68a942e8cf9739619b7f408cc7b272b279b56b2c83c6123fcfa5cdff",
+                "sha256:d737a602fbd82afd892ca746392401b634e278cb65d55c4b7a8f48e9ef8d008d",
+                "sha256:d80cf684b541685fccdd84c485b31ce73fc5c9b5d7523bf1394ce134a60c6883",
+                "sha256:db24668940f82321e746773a4bc617bfac06ec831e5c88b643f91f122a785684",
+                "sha256:dbc02381779d412145331789b40cc7b11fdf449e5d94f6bc0b080db0a56ea3f0",
+                "sha256:dffe31a7f47b603318c609f378ebcd57f1554a3a6a8effbc59c3c69f804296de",
+                "sha256:edf4392b77bdc81f36e92d3a07a5cd072f90253197f4a52a55a8cec48a12483b",
+                "sha256:efe8c0681042536e0d06c11f48cebe759707c9e9abf880ee213541c5b46c5bf3",
+                "sha256:f31f9fdbfecb042d046f9d91270a0ba28368a723302786c0009ee9b9f1f60199",
+                "sha256:f88a0b92277de8e3ca715a0d79d68dc82807457dae3ab8699c758f07c20b3c51",
+                "sha256:faaf07ea35355b01a35cb442dd950d8f1bb5b040a7787791a535de13db15ed90"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==10.0.0"
+        },
         "platformdirs": {
             "hashes": [
                 "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c",
                 "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.8.1"
@@ -857,14 +1212,22 @@
             "hashes": [
                 "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
+        "pyparsing": {
+            "hashes": [
+                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
+                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+            ],
+            "markers": "python_full_version >= '3.6.8'",
+            "version": "==3.0.9"
+        },
         "pytest": {
             "hashes": [
                 "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
             "version": "==7.4.0"
@@ -889,14 +1252,22 @@
             "hashes": [
                 "sha256:d5ee0520eb1b7bcca50a60a518ab7a7707992812c578198f8b44fdfac78e8c93",
                 "sha256:ff9daa7793569e6a68544850fd3927cd257cc03a7ef76c95e86915355e82b5f2"
             ],
             "index": "pypi",
             "version": "==3.3.1"
         },
+        "python-dateutil": {
+            "hashes": [
+                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
+                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==2.8.2"
+        },
         "pytz": {
             "hashes": [
                 "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
                 "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
             "version": "==2023.3"
         },
@@ -950,14 +1321,22 @@
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.31.0"
         },
+        "seaborn": {
+            "hashes": [
+                "sha256:374645f36509d0dcab895cba5b47daf0586f77bfe3b36c97c607db7da5be0139",
+                "sha256:ebf15355a4dba46037dfd65b7350f014ceb1f13c05e814eda2c9f5fd731afc08"
+            ],
+            "index": "pypi",
+            "version": "==0.12.2"
+        },
         "setuptools": {
             "hashes": [
                 "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
                 "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==68.0.0"
@@ -1077,14 +1456,22 @@
             "hashes": [
                 "sha256:916c2213577aec0b3b5452c5bfb32fd077f3a3196f50a81ad57d7ef3fc2599e4",
                 "sha256:e470c18af115fe52eeff95e7e3cdd0793613eca19709966fc2724b79d55246cb"
             ],
             "index": "pypi",
             "version": "==1.1.0"
         },
+        "tzdata": {
+            "hashes": [
+                "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a",
+                "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
+            ],
+            "markers": "python_version >= '2'",
+            "version": "==2023.3"
+        },
         "urllib3": {
             "hashes": [
                 "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
                 "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.3"
@@ -1095,15 +1482,15 @@
                 "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==20.23.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941",
+                "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==3.15.0"
+            "version": "==3.16.0"
         }
     }
 }
```

### Comparing `heatmap_cli-0.1.1/README.md` & `heatmap_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/docs/Makefile` & `heatmap_cli-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/docs/make.bat` & `heatmap_cli-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/docs/source/_static/logo.jpg` & `heatmap_cli-0.1.2/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/docs/source/conf.py` & `heatmap_cli-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/heatmap_cli/__init__.py` & `heatmap_cli-0.1.2/heatmap_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `heatmap_cli-0.1.1/heatmap_cli/__main__.py` & `heatmap_cli-0.1.2/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/heatmap_cli/cli.py` & `heatmap_cli-0.1.2/heatmap_cli/cli.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/pyproject.toml` & `heatmap_cli-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/tests/conftest.py` & `heatmap_cli-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/tests/fixtures/sample.csv` & `heatmap_cli-0.1.2/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/tests/test_verbose_flag.py` & `heatmap_cli-0.1.2/tests/test_verbose_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.1/tox.ini` & `heatmap_cli-0.1.2/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 [testenv:doc]
 description = generate sphinx documentation in html
 basepython = python3.11
 deps = pipenv
 commands =
     pipenv install --dev
-    pipenv run sphinx-build {toxinidir}/docs/source/ {toxinidir}/docs/_build/html
+    pipenv run sphinx-build {toxinidir}/docs/source/ {toxinidir}/docs/build/html
```

### Comparing `heatmap_cli-0.1.1/PKG-INFO` & `heatmap_cli-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatmap_cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A console program that generates yearly calendar heatmap.
 Keywords: heatmap,cli
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

