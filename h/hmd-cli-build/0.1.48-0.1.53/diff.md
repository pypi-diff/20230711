# Comparing `tmp/hmd_cli_build-0.1.48-py3-none-any.whl.zip` & `tmp/hmd_cli_build-0.1.53-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5265 bytes, number of entries: 6
--rw-rw-rw-  2.0 unx        0 b- defN 23-May-18 16:45 hmd_cli_build/__init__.py
--rw-rw-rw-  2.0 unx     8418 b- defN 23-May-18 16:45 hmd_cli_build/controller.py
--rw-rw-rw-  2.0 unx     4268 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       14 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      489 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/RECORD
-6 files, 13281 bytes uncompressed, 4371 bytes compressed:  67.1%
+Zip file size: 5288 bytes, number of entries: 6
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jun-29 13:20 hmd_cli_build/__init__.py
+-rw-rw-rw-  2.0 unx     8560 b- defN 23-Jun-29 13:20 hmd_cli_build/controller.py
+-rw-rw-rw-  2.0 unx     4268 b- defN 23-Jun-29 13:21 hmd_cli_build-0.1.53.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jun-29 13:21 hmd_cli_build-0.1.53.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       14 b- defN 23-Jun-29 13:21 hmd_cli_build-0.1.53.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      489 b- defN 23-Jun-29 13:21 hmd_cli_build-0.1.53.dist-info/RECORD
+6 files, 13423 bytes uncompressed, 4394 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: hmd_cli_build/__init__.py
 Comment: 
 
 Filename: hmd_cli_build/controller.py
 Comment: 
 
-Filename: hmd_cli_build-0.1.48.dist-info/METADATA
+Filename: hmd_cli_build-0.1.53.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_build-0.1.48.dist-info/WHEEL
+Filename: hmd_cli_build-0.1.53.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_build-0.1.48.dist-info/top_level.txt
+Filename: hmd_cli_build-0.1.53.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_build-0.1.48.dist-info/RECORD
+Filename: hmd_cli_build-0.1.53.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_build/controller.py

```diff
@@ -133,15 +133,22 @@
                         content_item_path_from_spec(content_item_path)[0],
                         dir_or_dirs,
                     )
             if self.app.pargs.prebuild_download_only:
                 return
 
             shutil.copytree(Path("meta-data"), build_path / "meta-data")
-            standard_dirs = ["docs", "test", "src/opa-bundles", "src/mickey"]
+            standard_dirs = [
+                "docs",
+                "test",
+                "src/opa-bundles",
+                "src/mickey",
+                "src/entities",
+                "src/schemas",
+            ]
             for path in standard_dirs:
                 if os.path.exists(Path(path)):
                     shutil.copytree(Path(path), build_path / path)
 
             for tool in manifest["build"]["commands"]:
                 if len(tool) < 3:
                     tool = tool + defaults[-(3 - len(tool)) :]
```

## Comparing `hmd_cli_build-0.1.48.dist-info/METADATA` & `hmd_cli_build-0.1.53.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-build
-Version: 0.1.48
+Version: 0.1.53
 Summary: Generic build tool.
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -27,20 +27,20 @@
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
-Requires-Dist: hmd-cli-app (~=1.1.595)
-Requires-Dist: hmd-cli-tools (~=1.1.228)
-Requires-Dist: hmd-entity-storage (~=0.1.224)
-Requires-Dist: hmd-graphql-client (~=0.1.105)
+Requires-Dist: hmd-cli-app (~=1.1.597)
+Requires-Dist: hmd-cli-tools (~=1.1.229)
+Requires-Dist: hmd-entity-storage (~=0.1.225)
+Requires-Dist: hmd-graphql-client (~=0.1.106)
 Requires-Dist: hmd-lib-auth (~=0.1.75)
-Requires-Dist: hmd-lib-librarian-client (~=0.1.53)
+Requires-Dist: hmd-lib-librarian-client (~=0.1.54)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
@@ -50,15 +50,15 @@
 Requires-Dist: markupsafe (==2.1.0)
 Requires-Dist: multidict (==6.0.2)
 Requires-Dist: nest-asyncio (==1.5.4)
 Requires-Dist: oauthlib (==3.2.2)
 Requires-Dist: okta-jwt-verifier (==0.2.3)
 Requires-Dist: pfzy (==0.3.4)
 Requires-Dist: prompt-toolkit (==3.0.38)
-Requires-Dist: psycopg2-binary (==2.9.3)
+Requires-Dist: psycopg2-binary (==2.9.6)
 Requires-Dist: py (==1.11.0)
 Requires-Dist: pyasn1 (==0.4.8)
 Requires-Dist: pyasn1-modules (==0.2.8)
 Requires-Dist: pyrsistent (==0.18.1)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: python-dotenv (==0.19.2)
 Requires-Dist: python-jose (==3.3.0)
```

