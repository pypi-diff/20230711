# Comparing `tmp/th2_grpc_act_template-4.0.1.dev0.tar.gz` & `tmp/th2_grpc_act_template-4.1.0.dev5521707556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_template-4.0.1.dev0.tar", last modified: Wed Mar  1 09:09:56 2023, max compression
+gzip compressed data, was "dist/th2_grpc_act_template-4.1.0.dev5521707556.tar", last modified: Tue Jul 11 15:11:56 2023, max compression
```

## Comparing `th2_grpc_act_template-4.0.1.dev0.tar` & `th2_grpc_act_template-4.1.0.dev5521707556.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-03-01 09:09:37.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4763 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-11 15:11:34.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/PKG-INFO` & `th2_grpc_act_template-4.1.0.dev5521707556/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_template
-Version: 4.0.1.dev0
+Version: 4.1.0.dev5521707556
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
         
-        This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j"). See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for details. <br>
-        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
+        This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that
+        are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j").
+        See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for
+        details. <br>
+        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
+        repositories.
         
         ## How to transform the template
-        1. Create a directory with the same name as the project name (use underscores instead of dashes) under `src/main/proto` directory (remove other files and directories if they exist).
-        2. Place your custom `.proto` files in the created directory. Pay attention to both the `package` specifier and to the `import` statements.
+        
+        1. Create a directory with the same name as the project name (use underscores instead of dashes) under `src/main/proto`
+           directory (remove other files and directories if they exist).
+        2. Place your custom `.proto` files in the created directory. Pay attention to both the `package` specifier and to
+           the `import` statements.
         3. Edit `release_version` and `vcs_url` properties in `gradle.properties` file.
         4. Edit `rootProject.name` variable in `settings.gradle` file. This will be the name of the Java package.
-        5. Edit `package_info.json` file in order to specify its name and its version for Python package (create the file in case it's absent).
-        6. Edit parameters of `setup.py` in `setup` function invocation such as: `author`, `author_email`, `url`. Do not edit the other's parameters.
+        5. Edit `package_info.json` file in order to specify its name and its version for Python package (create the file in
+           case it's absent).
+        6. Edit parameters of `setup.py` in `setup` function invocation such as: `author`, `author_email`, `url`. Do not edit
+           the other's parameters.
         7. Edit `README.md` file according to the new project.
         
         Note that the name of the created directory under `src/main/proto` directory is used in Python (it's a package name).
         
         ## How to maintain a project
+        
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
         3. Update the package version of Python in `package_info.json` file.
         4. Commit everything.
         
         ## How to run project
         
         ### Java
+        
         If you wish to manually create and publish a package for Java, run the following command:
+        
         ```
         gradle --no-daemon clean build publish artifactoryPublish \
                -Purl=${URL} \ 
                -Puser=${USER} \
                -Ppassword=${PASSWORD}
         ```
+        
         `URL`, `USER` and `PASSWORD` are parameters for publishing.
         
         ### Python
+        
         If you wish to manually create and publish a package for Python:
+        
         1. Generate services with `Gradle`:
             ```
                gradle --no-daemon clean generateProto
             ```
            You can find the generated files by following path: `src/gen/main/services/python`
         2. Generate code from `.proto` files and publish everything using `twine`:
             ```
@@ -55,47 +70,57 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
-        ### 4.0.1
-        + Dependency check pipeline step added
+        ### 4.1.0
+        
+        + Update to `th2-grpc-common` version `4.2.0`
+        + Update to `th2-bom` version `4.4.0`
+        + Update to `th2-grpc-service-genrator` version `3.4.0`
         
         ### 4.0.0
         
-        + Update to `th2-grpc-common` version `4.2.0`
+        + Update to `th2-grpc-common` version `4.0.0`
         + Marked deprecated fields as `reserved`
         
+        ### 3.12.0
+        
+        + grpc version bump to `1.48.2`
+        + protobuf version bump to `3.21.7`
+        + serviceGenerator version bump to `3.3.1`
+        + Add dependency check pipeline step.
+        + Add dev-release workflow.
+        
         ### 3.11.0
         
         + Add `multiSendMessage` method for sending several messages at once
         
         ### 3.10.0
         
         + Add `placeOrderCancelReplaceRequest` method for sending `OrderCancelReplaceRequest`
-        + Rename `placeCancelFIX` to `placeOrderCancelRequest` 
+        + Rename `placeCancelFIX` to `placeOrderCancelRequest`
         
         ### 3.9.0
         
         + Update to `th2-grpc-common` version `3.11.1`
         
-        
         ### 3.8.0
         
         + Update to `th2-grpc-common` version `3.9.0`
         
         ### 3.7.0
         
         + Add new method for sending `SecurityStatusRequest`
         
         ### 3.6.0
         
-        + Add new method for sending `OrderCancelRequest` 
+        + Add new method for sending `OrderCancelRequest`
         
         ### 3.5.0
         
         + Update to `th2-grpc-common` version `3.8.0`
         
         ### 3.4.0
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/README.md` & `th2_grpc_act_template-4.1.0.dev5521707556/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 # th2 gRPC act template library (4.0.1)
 
-This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j"). See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for details. <br>
-Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
+This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that
+are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j").
+See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for
+details. <br>
+Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
+repositories.
 
 ## How to transform the template
-1. Create a directory with the same name as the project name (use underscores instead of dashes) under `src/main/proto` directory (remove other files and directories if they exist).
-2. Place your custom `.proto` files in the created directory. Pay attention to both the `package` specifier and to the `import` statements.
+
+1. Create a directory with the same name as the project name (use underscores instead of dashes) under `src/main/proto`
+   directory (remove other files and directories if they exist).
+2. Place your custom `.proto` files in the created directory. Pay attention to both the `package` specifier and to
+   the `import` statements.
 3. Edit `release_version` and `vcs_url` properties in `gradle.properties` file.
 4. Edit `rootProject.name` variable in `settings.gradle` file. This will be the name of the Java package.
-5. Edit `package_info.json` file in order to specify its name and its version for Python package (create the file in case it's absent).
-6. Edit parameters of `setup.py` in `setup` function invocation such as: `author`, `author_email`, `url`. Do not edit the other's parameters.
+5. Edit `package_info.json` file in order to specify its name and its version for Python package (create the file in
+   case it's absent).
+6. Edit parameters of `setup.py` in `setup` function invocation such as: `author`, `author_email`, `url`. Do not edit
+   the other's parameters.
 7. Edit `README.md` file according to the new project.
 
 Note that the name of the created directory under `src/main/proto` directory is used in Python (it's a package name).
 
 ## How to maintain a project
+
 1. Perform the necessary changes.
 2. Update the package version of Java in `gradle.properties` file.
 3. Update the package version of Python in `package_info.json` file.
 4. Commit everything.
 
 ## How to run project
 
 ### Java
+
 If you wish to manually create and publish a package for Java, run the following command:
+
 ```
 gradle --no-daemon clean build publish artifactoryPublish \
        -Purl=${URL} \ 
        -Puser=${USER} \
        -Ppassword=${PASSWORD}
 ```
+
 `URL`, `USER` and `PASSWORD` are parameters for publishing.
 
 ### Python
+
 If you wish to manually create and publish a package for Python:
+
 1. Generate services with `Gradle`:
     ```
        gradle --no-daemon clean generateProto
     ```
    You can find the generated files by following path: `src/gen/main/services/python`
 2. Generate code from `.proto` files and publish everything using `twine`:
     ```
@@ -47,47 +62,57 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
-### 4.0.1
-+ Dependency check pipeline step added
+### 4.1.0
+
++ Update to `th2-grpc-common` version `4.2.0`
++ Update to `th2-bom` version `4.4.0`
++ Update to `th2-grpc-service-genrator` version `3.4.0`
 
 ### 4.0.0
 
-+ Update to `th2-grpc-common` version `4.2.0`
++ Update to `th2-grpc-common` version `4.0.0`
 + Marked deprecated fields as `reserved`
 
+### 3.12.0
+
++ grpc version bump to `1.48.2`
++ protobuf version bump to `3.21.7`
++ serviceGenerator version bump to `3.3.1`
++ Add dependency check pipeline step.
++ Add dev-release workflow.
+
 ### 3.11.0
 
 + Add `multiSendMessage` method for sending several messages at once
 
 ### 3.10.0
 
 + Add `placeOrderCancelReplaceRequest` method for sending `OrderCancelReplaceRequest`
-+ Rename `placeCancelFIX` to `placeOrderCancelRequest` 
++ Rename `placeCancelFIX` to `placeOrderCancelRequest`
 
 ### 3.9.0
 
 + Update to `th2-grpc-common` version `3.11.1`
 
-
 ### 3.8.0
 
 + Update to `th2-grpc-common` version `3.9.0`
 
 ### 3.7.0
 
 + Add new method for sending `SecurityStatusRequest`
 
 ### 3.6.0
 
-+ Add new method for sending `OrderCancelRequest` 
++ Add new method for sending `OrderCancelRequest`
 
 ### 3.5.0
 
 + Update to `th2-grpc-common` version `3.8.0`
 
 ### 3.4.0
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/setup.py` & `th2_grpc_act_template-4.1.0.dev5521707556/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-act-template',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-common==4.1.0.dev4105266708',
-        'mypy-protobuf==3.2'
+        'th2-grpc-common==4.3.0.dev5378777004',
+        'mypy-protobuf==3.4'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_service.py` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template.proto` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.py` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: th2_grpc_act_template/act_template.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from th2_grpc_common import common_pb2 as th2__grpc__common_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(th2_grpc_act_template/act_template.proto\x1a\x1cth2_grpc_common/common.proto\"Y\n\x13SendMessageResponse\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.RequestStatus\x12\"\n\rcheckpoint_id\x18\x02 \x01(\x0b\x32\x0b.Checkpoint\"n\n\x13PlaceMessageRequest\x12\x19\n\x07message\x18\x01 \x01(\x0b\x32\x08.Message\x12!\n\x0fparent_event_id\x18\x04 \x01(\x0b\x32\x08.EventID\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\tJ\x04\x08\x02\x10\x03\"~\n\x14PlaceMessageResponse\x12\"\n\x10response_message\x18\x01 \x01(\x0b\x32\x08.Message\x12\x1e\n\x06status\x18\x02 \x01(\x0b\x32\x0e.RequestStatus\x12\"\n\rcheckpoint_id\x18\x03 \x01(\x0b\x32\x0b.Checkpoint\"z\n\x10MultiSendRequest\x12\x1a\n\x08messages\x18\x01 \x03(\x0b\x32\x08.Message\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x12\n\nskip_order\x18\x04 \x01(\x08\x32\x8f\x06\n\x03\x41\x63t\x12>\n\rplaceOrderFIX\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12H\n\x17placeOrderCancelRequest\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12O\n\x1eplaceOrderCancelReplaceRequest\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12;\n\x0bsendMessage\x12\x14.PlaceMessageRequest\x1a\x14.SendMessageResponse\"\x00\x12\x45\n\x14placeQuoteRequestFIX\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12>\n\rplaceQuoteFIX\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12O\n\x1eplaceOrderMassCancelRequestFIX\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12\x44\n\x13placeQuoteCancelFIX\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12\x46\n\x15placeQuoteResponseFIX\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12K\n\x1aplaceSecurityStatusRequest\x12\x14.PlaceMessageRequest\x1a\x15.PlaceMessageResponse\"\x00\x12=\n\x10multiSendMessage\x12\x11.MultiSendRequest\x1a\x14.SendMessageResponse\"\x00\x42\x1d\n\x19\x63om.exactpro.th2.act.grpcP\x01\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'th2_grpc_act_template.act_template_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'th2_grpc_act_template.act_template_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\031com.exactpro.th2.act.grpcP\001'
-  _SENDMESSAGERESPONSE._serialized_start=74
-  _SENDMESSAGERESPONSE._serialized_end=163
-  _PLACEMESSAGEREQUEST._serialized_start=165
-  _PLACEMESSAGEREQUEST._serialized_end=275
-  _PLACEMESSAGERESPONSE._serialized_start=277
-  _PLACEMESSAGERESPONSE._serialized_end=403
-  _MULTISENDREQUEST._serialized_start=405
-  _MULTISENDREQUEST._serialized_end=527
-  _ACT._serialized_start=530
-  _ACT._serialized_end=1313
+  _globals['_SENDMESSAGERESPONSE']._serialized_start=74
+  _globals['_SENDMESSAGERESPONSE']._serialized_end=163
+  _globals['_PLACEMESSAGEREQUEST']._serialized_start=165
+  _globals['_PLACEMESSAGEREQUEST']._serialized_end=275
+  _globals['_PLACEMESSAGERESPONSE']._serialized_start=277
+  _globals['_PLACEMESSAGERESPONSE']._serialized_end=403
+  _globals['_MULTISENDREQUEST']._serialized_start=405
+  _globals['_MULTISENDREQUEST']._serialized_end=527
+  _globals['_ACT']._serialized_start=530
+  _globals['_ACT']._serialized_end=1313
 # @@protoc_insertion_point(module_scope)
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.pyi` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,129 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
+
+Copyright 2020-2023 Exactpro (Exactpro Systems Limited)
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
+import sys
 import th2_grpc_common.common_pb2
-import typing
-import typing_extensions
+
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class SendMessageResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     STATUS_FIELD_NUMBER: builtins.int
     CHECKPOINT_ID_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
     @property
     def checkpoint_id(self) -> th2_grpc_common.common_pb2.Checkpoint: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
-        checkpoint_id: typing.Optional[th2_grpc_common.common_pb2.Checkpoint] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["checkpoint_id",b"checkpoint_id","status",b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["checkpoint_id",b"checkpoint_id","status",b"status"]) -> None: ...
+        status: th2_grpc_common.common_pb2.RequestStatus | None = ...,
+        checkpoint_id: th2_grpc_common.common_pb2.Checkpoint | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["checkpoint_id", b"checkpoint_id", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["checkpoint_id", b"checkpoint_id", "status", b"status"]) -> None: ...
+
 global___SendMessageResponse = SendMessageResponse
 
+@typing_extensions.final
 class PlaceMessageRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGE_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     @property
     def message(self) -> th2_grpc_common.common_pb2.Message: ...
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
-    description: typing.Text
-    def __init__(self,
+    description: builtins.str
+    def __init__(
+        self,
         *,
-        message: typing.Optional[th2_grpc_common.common_pb2.Message] = ...,
-        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
-        description: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["message",b"message","parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description",b"description","message",b"message","parent_event_id",b"parent_event_id"]) -> None: ...
+        message: th2_grpc_common.common_pb2.Message | None = ...,
+        parent_event_id: th2_grpc_common.common_pb2.EventID | None = ...,
+        description: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["message", b"message", "parent_event_id", b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "message", b"message", "parent_event_id", b"parent_event_id"]) -> None: ...
+
 global___PlaceMessageRequest = PlaceMessageRequest
 
+@typing_extensions.final
 class PlaceMessageResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     RESPONSE_MESSAGE_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     CHECKPOINT_ID_FIELD_NUMBER: builtins.int
     @property
     def response_message(self) -> th2_grpc_common.common_pb2.Message: ...
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
     @property
     def checkpoint_id(self) -> th2_grpc_common.common_pb2.Checkpoint: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        response_message: typing.Optional[th2_grpc_common.common_pb2.Message] = ...,
-        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
-        checkpoint_id: typing.Optional[th2_grpc_common.common_pb2.Checkpoint] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["checkpoint_id",b"checkpoint_id","response_message",b"response_message","status",b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["checkpoint_id",b"checkpoint_id","response_message",b"response_message","status",b"status"]) -> None: ...
+        response_message: th2_grpc_common.common_pb2.Message | None = ...,
+        status: th2_grpc_common.common_pb2.RequestStatus | None = ...,
+        checkpoint_id: th2_grpc_common.common_pb2.Checkpoint | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["checkpoint_id", b"checkpoint_id", "response_message", b"response_message", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["checkpoint_id", b"checkpoint_id", "response_message", b"response_message", "status", b"status"]) -> None: ...
+
 global___PlaceMessageResponse = PlaceMessageResponse
 
+@typing_extensions.final
 class MultiSendRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGES_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     SKIP_ORDER_FIELD_NUMBER: builtins.int
     @property
     def messages(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[th2_grpc_common.common_pb2.Message]: ...
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
-    description: typing.Text
+    description: builtins.str
     skip_order: builtins.bool
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        messages: typing.Optional[typing.Iterable[th2_grpc_common.common_pb2.Message]] = ...,
-        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
-        description: typing.Text = ...,
+        messages: collections.abc.Iterable[th2_grpc_common.common_pb2.Message] | None = ...,
+        parent_event_id: th2_grpc_common.common_pb2.EventID | None = ...,
+        description: builtins.str = ...,
         skip_order: builtins.bool = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description",b"description","messages",b"messages","parent_event_id",b"parent_event_id","skip_order",b"skip_order"]) -> None: ...
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["parent_event_id", b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "messages", b"messages", "parent_event_id", b"parent_event_id", "skip_order", b"skip_order"]) -> None: ...
+
 global___MultiSendRequest = MultiSendRequest
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2_grpc.py` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/PKG-INFO` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-template
-Version: 4.0.1.dev0
+Version: 4.1.0.dev5521707556
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
         
-        This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j"). See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for details. <br>
-        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
+        This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that
+        are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j").
+        See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for
+        details. <br>
+        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
+        repositories.
         
         ## How to transform the template
-        1. Create a directory with the same name as the project name (use underscores instead of dashes) under `src/main/proto` directory (remove other files and directories if they exist).
-        2. Place your custom `.proto` files in the created directory. Pay attention to both the `package` specifier and to the `import` statements.
+        
+        1. Create a directory with the same name as the project name (use underscores instead of dashes) under `src/main/proto`
+           directory (remove other files and directories if they exist).
+        2. Place your custom `.proto` files in the created directory. Pay attention to both the `package` specifier and to
+           the `import` statements.
         3. Edit `release_version` and `vcs_url` properties in `gradle.properties` file.
         4. Edit `rootProject.name` variable in `settings.gradle` file. This will be the name of the Java package.
-        5. Edit `package_info.json` file in order to specify its name and its version for Python package (create the file in case it's absent).
-        6. Edit parameters of `setup.py` in `setup` function invocation such as: `author`, `author_email`, `url`. Do not edit the other's parameters.
+        5. Edit `package_info.json` file in order to specify its name and its version for Python package (create the file in
+           case it's absent).
+        6. Edit parameters of `setup.py` in `setup` function invocation such as: `author`, `author_email`, `url`. Do not edit
+           the other's parameters.
         7. Edit `README.md` file according to the new project.
         
         Note that the name of the created directory under `src/main/proto` directory is used in Python (it's a package name).
         
         ## How to maintain a project
+        
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
         3. Update the package version of Python in `package_info.json` file.
         4. Commit everything.
         
         ## How to run project
         
         ### Java
+        
         If you wish to manually create and publish a package for Java, run the following command:
+        
         ```
         gradle --no-daemon clean build publish artifactoryPublish \
                -Purl=${URL} \ 
                -Puser=${USER} \
                -Ppassword=${PASSWORD}
         ```
+        
         `URL`, `USER` and `PASSWORD` are parameters for publishing.
         
         ### Python
+        
         If you wish to manually create and publish a package for Python:
+        
         1. Generate services with `Gradle`:
             ```
                gradle --no-daemon clean generateProto
             ```
            You can find the generated files by following path: `src/gen/main/services/python`
         2. Generate code from `.proto` files and publish everything using `twine`:
             ```
@@ -55,47 +70,57 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
-        ### 4.0.1
-        + Dependency check pipeline step added
+        ### 4.1.0
+        
+        + Update to `th2-grpc-common` version `4.2.0`
+        + Update to `th2-bom` version `4.4.0`
+        + Update to `th2-grpc-service-genrator` version `3.4.0`
         
         ### 4.0.0
         
-        + Update to `th2-grpc-common` version `4.2.0`
+        + Update to `th2-grpc-common` version `4.0.0`
         + Marked deprecated fields as `reserved`
         
+        ### 3.12.0
+        
+        + grpc version bump to `1.48.2`
+        + protobuf version bump to `3.21.7`
+        + serviceGenerator version bump to `3.3.1`
+        + Add dependency check pipeline step.
+        + Add dev-release workflow.
+        
         ### 3.11.0
         
         + Add `multiSendMessage` method for sending several messages at once
         
         ### 3.10.0
         
         + Add `placeOrderCancelReplaceRequest` method for sending `OrderCancelReplaceRequest`
-        + Rename `placeCancelFIX` to `placeOrderCancelRequest` 
+        + Rename `placeCancelFIX` to `placeOrderCancelRequest`
         
         ### 3.9.0
         
         + Update to `th2-grpc-common` version `3.11.1`
         
-        
         ### 3.8.0
         
         + Update to `th2-grpc-common` version `3.9.0`
         
         ### 3.7.0
         
         + Add new method for sending `SecurityStatusRequest`
         
         ### 3.6.0
         
-        + Add new method for sending `OrderCancelRequest` 
+        + Add new method for sending `OrderCancelRequest`
         
         ### 3.5.0
         
         + Update to `th2-grpc-common` version `3.8.0`
         
         ### 3.4.0
```

### Comparing `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/SOURCES.txt` & `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

