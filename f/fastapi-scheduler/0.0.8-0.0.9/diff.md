# Comparing `tmp/fastapi_scheduler-0.0.8.tar.gz` & `tmp/fastapi_scheduler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_scheduler-0.0.8.tar", last modified: Fri Sep 23 14:26:48 2022, max compression
+gzip compressed data, was "fastapi_scheduler-0.0.9.tar", last modified: Tue Sep 27 15:28:03 2022, max compression
```

## Comparing `fastapi_scheduler-0.0.8.tar` & `fastapi_scheduler-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2385 2022-06-10 14:19:52.997637 fastapi_scheduler-0.0.8/README.md
--rw-r--r--   0        0        0      494 2022-09-23 08:44:55.963927 fastapi_scheduler-0.0.8/fastapi_scheduler/__init__.py
--rw-r--r--   0        0        0    10007 2022-09-23 08:52:17.717314 fastapi_scheduler-0.0.8/fastapi_scheduler/admin.py
--rw-r--r--   0        0        0     1631 2022-05-22 10:43:09.701716 fastapi_scheduler-0.0.8/fastapi_scheduler/locale/base.pot
--rw-r--r--   0        0        0     1386 2022-05-22 15:52:35.878915 fastapi_scheduler-0.0.8/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2126 2022-05-22 15:52:35.879915 fastapi_scheduler-0.0.8/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1726 2022-09-23 09:01:17.046780 fastapi_scheduler-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 fastapi_scheduler-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2385 2022-06-10 14:19:52.997637 fastapi_scheduler-0.0.9/README.md
+-rw-r--r--   0        0        0      494 2022-09-27 15:26:26.927465 fastapi_scheduler-0.0.9/fastapi_scheduler/__init__.py
+-rw-r--r--   0        0        0    10049 2022-09-27 15:26:03.627570 fastapi_scheduler-0.0.9/fastapi_scheduler/admin.py
+-rw-r--r--   0        0        0     1631 2022-05-22 10:43:09.701716 fastapi_scheduler-0.0.9/fastapi_scheduler/locale/base.pot
+-rw-r--r--   0        0        0     1386 2022-05-22 15:52:35.878915 fastapi_scheduler-0.0.9/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2126 2022-05-22 15:52:35.879915 fastapi_scheduler-0.0.9/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1680 2022-09-27 15:25:13.952638 fastapi_scheduler-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 fastapi_scheduler-0.0.9/PKG-INFO
```

### Comparing `fastapi_scheduler-0.0.8/README.md` & `fastapi_scheduler-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_scheduler-0.0.8/fastapi_scheduler/admin.py` & `fastapi_scheduler-0.0.9/fastapi_scheduler/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from apscheduler.job import Job
 from apscheduler.jobstores.memory import MemoryJobStore
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from apscheduler.schedulers.base import BaseScheduler
 from fastapi import Body, Depends
 from fastapi_amis_admin import admin
-from fastapi_amis_admin.admin import AdminApp, AmisParser
+from fastapi_amis_admin.admin import AdminApp
 from fastapi_amis_admin.amis import (
     Action,
     ActionType,
     Dialog,
     Form,
     FormItem,
     InputDatetime,
@@ -133,15 +133,17 @@
             quickSaveItemApi=f"{self.router_path}/item/$id",
         )
         return page
 
     async def get_list_columns(self, request: Request) -> List[TableColumn]:
         columns = []
         for modelfield in self.JobModel.__fields__.values():
-            column = AmisParser(modelfield).as_table_column(quick_edit=modelfield.name in self.schema_update.__fields__)
+            column = self.site.amis_parser.as_table_column(
+                modelfield, quick_edit=modelfield.name in self.schema_update.__fields__
+            )
             if column:
                 columns.append(column)
         return columns
 
     async def get_actions_on_item(self, request: Request) -> List[Action]:
         actions = [
             await self.get_job_action(request, bulk=False, action="resume"),
@@ -207,15 +209,15 @@
                 confirmText=_("Are you sure you want to %s the selected task?") % label,
                 api=f"{self.router_path}/item/$id?action={action}",
             )
         )
 
     async def get_form_item(self, request: Request, modelfield: ModelField, action: CrudEnum) -> Union[FormItem, SchemaNode]:
         is_filter = action == CrudEnum.list
-        return AmisParser(modelfield).as_form_item(is_filter=is_filter)
+        return self.site.amis_parser.as_form_item(modelfield, is_filter=is_filter)
 
     def register_router(self):
         @self.router.get(
             "/list",
             response_model=BaseApiOut[ItemListSchema[self.JobModel]],
             include_in_schema=True,
         )
```

### Comparing `fastapi_scheduler-0.0.8/fastapi_scheduler/locale/base.pot` & `fastapi_scheduler-0.0.9/fastapi_scheduler/locale/base.pot`

 * *Files identical despite different names*

### Comparing `fastapi_scheduler-0.0.8/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_scheduler-0.0.9/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_scheduler-0.0.8/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_scheduler-0.0.9/fastapi_scheduler/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_scheduler-0.0.8/pyproject.toml` & `fastapi_scheduler-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 classifiers = [
     "Framework :: FastAPI",
     "Environment :: Web Environment",
     "Topic :: System :: Systems Administration",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "fastapi-amis-admin>=0.2.2,<0.3.0",
+    "fastapi-amis-admin>=0.2.3,<0.3.0",
     "APScheduler>=3.8.0",
 ]
 
 [project.urls]
 Source = "https://github.com/amisadmin/fastapi_scheduler"
 FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi_amis_admin"
```

### Comparing `fastapi_scheduler-0.0.8/PKG-INFO` & `fastapi_scheduler-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: fastapi_scheduler
-Version: 0.0.8
+Version: 0.0.9
 Summary: FastAPI-Scheduler is a simple scheduled task management FastAPI extension based on APScheduler.
 Keywords: FastAPI-Amis-Admin,FastAPI-APScheduler,fastapi-scheduler,APScheduler
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
 Classifier: Environment :: Web Environment
 Classifier: Topic :: System :: Systems Administration
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: fastapi-amis-admin>=0.2.2,<0.3.0
+Requires-Dist: fastapi-amis-admin>=0.2.3,<0.3.0
 Requires-Dist: APScheduler>=3.8.0
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
 Project-URL: FastAPI-Amis-Admin, https://github.com/amisadmin/fastapi_amis_admin
 Project-URL: Source, https://github.com/amisadmin/fastapi_scheduler
 Provides-Extra: test
 
 <h2 align="center">
```

