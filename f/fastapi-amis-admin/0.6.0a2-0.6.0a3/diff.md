# Comparing `tmp/fastapi_amis_admin-0.6.0a2.tar.gz` & `tmp/fastapi_amis_admin-0.6.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin-0.6.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_amis_admin-0.6.0a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin-0.6.0a2.tar` & `fastapi_amis_admin-0.6.0a3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0    11773 2023-07-06 09:39:50.967857 fastapi_amis_admin-0.6.0a2/README.md
--rw-r--r--   0        0        0      603 2023-07-07 13:07:25.765268 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/__init__.py
--rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/__init__.py
--rw-r--r--   0        0        0    58253 2023-07-07 12:00:05.711251 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/admin.py
--rw-r--r--   0        0        0     3488 2023-07-07 10:00:42.574847 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/handlers.py
--rw-r--r--   0        0        0    13378 2023-07-06 08:54:37.120798 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/parser.py
--rw-r--r--   0        0        0     1765 2023-07-06 09:24:02.534616 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/settings.py
--rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/site.py
--rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/README.md
--rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/__init__.py
--rw-r--r--   0        0        0   151935 2023-06-13 06:14:32.628539 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/components.py
--rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/constants.py
--rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/app.html
--rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/page.html
--rw-r--r--   0        0        0     5096 2023-07-06 03:10:47.448565 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/types.py
--rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/utils.py
--rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/README.md
--rw-r--r--   0        0        0      309 2023-07-06 09:27:57.925619 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/__init__.py
--rw-r--r--   0        0        0    23526 2023-07-07 09:32:50.000249 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/_sqlalchemy.py
--rw-r--r--   0        0        0      419 2023-07-07 10:02:58.918305 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/_sqlmodel.py
--rw-r--r--   0        0        0     8077 2023-07-06 03:28:47.353316 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/base.py
--rw-r--r--   0        0        0    14025 2023-07-07 11:46:10.395305 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/parser.py
--rw-r--r--   0        0        0     1950 2023-04-06 13:53:04.589440 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/schema.py
--rw-r--r--   0        0        0     3985 2023-07-07 10:02:58.926300 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/utils.py
--rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/base.pot
--rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      156 2023-07-06 03:28:44.283974 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/__init__.py
--rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/enums.py
--rw-r--r--   0        0        0     2964 2023-07-06 03:28:22.246379 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/fields.py
--rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/functools.py
--rw-r--r--   0        0        0     1905 2023-07-06 03:28:44.284973 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/translation.py
--rw-r--r--   0        0        0     2772 2023-07-07 08:06:42.191567 fastapi_amis_admin-0.6.0a2/pyproject.toml
--rw-r--r--   0        0        0    13732 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11789 2023-07-11 03:47:06.502739 fastapi_amis_admin-0.6.0a3/README.md
+-rw-r--r--   0        0        0      603 2023-07-11 07:33:58.136031 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/__init__.py
+-rw-r--r--   0        0        0    58282 2023-07-11 03:47:06.507727 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/admin.py
+-rw-r--r--   0        0        0     3488 2023-07-07 10:00:42.574847 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/handlers.py
+-rw-r--r--   0        0        0    13955 2023-07-11 06:10:11.932836 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/parser.py
+-rw-r--r--   0        0        0     2446 2023-07-11 03:47:06.509725 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/settings.py
+-rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/site.py
+-rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/README.md
+-rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/__init__.py
+-rw-r--r--   0        0        0   151906 2023-07-11 06:13:30.848484 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/components.py
+-rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/constants.py
+-rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/templates/app.html
+-rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/templates/page.html
+-rw-r--r--   0        0        0     4977 2023-07-11 06:11:29.701954 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/types.py
+-rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/utils.py
+-rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/README.md
+-rw-r--r--   0        0        0      211 2023-07-08 02:15:45.947633 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/__init__.py
+-rw-r--r--   0        0        0    23573 2023-07-11 07:17:21.176358 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/_sqlalchemy.py
+-rw-r--r--   0        0        0      419 2023-07-07 10:02:58.918305 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/_sqlmodel.py
+-rw-r--r--   0        0        0     8079 2023-07-11 03:47:06.514737 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/base.py
+-rw-r--r--   0        0        0    14942 2023-07-11 07:17:54.338835 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/parser.py
+-rw-r--r--   0        0        0     1689 2023-07-11 06:16:01.658379 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/schema.py
+-rw-r--r--   0        0        0     1698 2023-07-11 07:17:41.394255 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/utils.py
+-rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/base.pot
+-rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      156 2023-07-06 03:28:44.283974 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/models/__init__.py
+-rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/models/enums.py
+-rw-r--r--   0        0        0     2964 2023-07-06 03:28:22.246379 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/models/fields.py
+-rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/utils/functools.py
+-rw-r--r--   0        0        0     8435 2023-07-11 07:11:39.547326 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/utils/pydantic.py
+-rw-r--r--   0        0        0     1905 2023-07-06 03:28:44.284973 fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/utils/translation.py
+-rw-r--r--   0        0        0     2820 2023-07-11 07:17:31.634284 fastapi_amis_admin-0.6.0a3/pyproject.toml
+-rw-r--r--   0        0        0    13828 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.0a3/PKG-INFO
```

### Comparing `fastapi_amis_admin-0.6.0a2/README.md` & `fastapi_amis_admin-0.6.0a3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 Base = declarative_base()
 
 
 # Create an SQLAlchemy model, see document for details: https://docs.sqlalchemy.org/en/14/orm/tutorial.html
 class Category(Base):
     __tablename__ = 'category'
     # Specify the Schema class corresponding to the model. It is recommended to specify it. If omitted, it can be automatically generated.
-    __schema__ = CategorySchema
+    __pydantic_model__ = CategorySchema
 
     id = Column(Integer, primary_key=True, nullable=False)
     name = Column(String(100), unique=True, index=True, nullable=False)
     description = Column(String(255), default='')
 ```
 
 - Method 3: Create model through `SQLAlchemy 2.0`.
@@ -169,15 +169,15 @@
     pass
 
 
 # Create an SQLAlchemy 2.0 model, see document for details: https://docs.sqlalchemy.org/en/20/orm/quickstart.html
 class Category(Base):
     __tablename__ = "category"
     # Specify the Schema class corresponding to the model. It is recommended to specify it. If omitted, it can be automatically generated.
-    __schema__ = CategorySchema
+    __pydantic_model__ = CategorySchema
 
     id: Mapped[int] = mapped_column(primary_key=True, nullable=False)
     name: Mapped[str] = mapped_column(String(100), unique=True, index=True, nullable=False)
     description: Mapped[str] = mapped_column(String(255), default="")
 ```
 
 - If you create a model through `sqlalchemy`, it is recommended to create a corresponding pydantic model at the same
```

#### html2text {}

```diff
@@ -59,37 +59,38 @@
 Field(default='', title='Description', max_length=255) ``` - Method 2: Create
 model through `SQLAlchemy`. ```python from sqlalchemy import Column, Integer,
 String from sqlalchemy.ext.declarative import declarative_base Base =
 declarative_base() # Create an SQLAlchemy model, see document for details:
 https://docs.sqlalchemy.org/en/14/orm/tutorial.html class Category(Base):
 __tablename__ = 'category' # Specify the Schema class corresponding to the
 model. It is recommended to specify it. If omitted, it can be automatically
-generated. __schema__ = CategorySchema id = Column(Integer, primary_key=True,
-nullable=False) name = Column(String(100), unique=True, index=True,
-nullable=False) description = Column(String(255), default='') ``` - Method 3:
-Create model through `SQLAlchemy 2.0`. ```python from sqlalchemy import String
-from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column class Base
-(DeclarativeBase): pass # Create an SQLAlchemy 2.0 model, see document for
-details: https://docs.sqlalchemy.org/en/20/orm/quickstart.html class Category
-(Base): __tablename__ = "category" # Specify the Schema class corresponding to
-the model. It is recommended to specify it. If omitted, it can be automatically
-generated. __schema__ = CategorySchema id: Mapped[int] = mapped_column
-(primary_key=True, nullable=False) name: Mapped[str] = mapped_column(String
-(100), unique=True, index=True, nullable=False) description: Mapped[str] =
-mapped_column(String(255), default="") ``` - If you create a model through
-`sqlalchemy`, it is recommended to create a corresponding pydantic model at the
-same time, and set `orm_mode=True`. ```python from pydantic import BaseModel,
-Field class CategorySchema(BaseModel): id: int = Field(default=None,
-primary_key=True, nullable=False) name: str = Field(title="CategoryName")
-description: str = Field(default="", title="CategoryDescription") class Config:
-orm_mode = True ``` ### Register ModelAdmin ```python from fastapi import
-FastAPI from sqlmodel import SQLModel from fastapi_amis_admin.admin.settings
-import Settings from fastapi_amis_admin.admin.site import AdminSite from
-fastapi_amis_admin.admin import admin # create FastAPI application app =
-FastAPI() # create AdminSite instance site = AdminSite(settings=Settings
+generated. __pydantic_model__ = CategorySchema id = Column(Integer,
+primary_key=True, nullable=False) name = Column(String(100), unique=True,
+index=True, nullable=False) description = Column(String(255), default='') ``` -
+Method 3: Create model through `SQLAlchemy 2.0`. ```python from sqlalchemy
+import String from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
+class Base(DeclarativeBase): pass # Create an SQLAlchemy 2.0 model, see
+document for details: https://docs.sqlalchemy.org/en/20/orm/quickstart.html
+class Category(Base): __tablename__ = "category" # Specify the Schema class
+corresponding to the model. It is recommended to specify it. If omitted, it can
+be automatically generated. __pydantic_model__ = CategorySchema id: Mapped[int]
+= mapped_column(primary_key=True, nullable=False) name: Mapped[str] =
+mapped_column(String(100), unique=True, index=True, nullable=False)
+description: Mapped[str] = mapped_column(String(255), default="") ``` - If you
+create a model through `sqlalchemy`, it is recommended to create a
+corresponding pydantic model at the same time, and set `orm_mode=True`.
+```python from pydantic import BaseModel, Field class CategorySchema
+(BaseModel): id: int = Field(default=None, primary_key=True, nullable=False)
+name: str = Field(title="CategoryName") description: str = Field(default="",
+title="CategoryDescription") class Config: orm_mode = True ``` ### Register
+ModelAdmin ```python from fastapi import FastAPI from sqlmodel import SQLModel
+from fastapi_amis_admin.admin.settings import Settings from
+fastapi_amis_admin.admin.site import AdminSite from fastapi_amis_admin.admin
+import admin # create FastAPI application app = FastAPI() # create AdminSite
+instance site = AdminSite(settings=Settings
 (database_url_async='sqlite+aiosqlite:///amisadmin.db')) # register ModelAdmin
 @site.register_admin class CategoryAdmin(admin.ModelAdmin): page_schema =
 'Category' # set model model = Category # mount AdminSite instance
 site.mount_app(app) # create initial database table @app.on_event("startup")
 async def startup(): await site.db.async_run_sync(Base.metadata.create_all,
 is_session=False) if __name__ == '__main__': import uvicorn uvicorn.run(app)
 ``` ## FormAdmin Example ```python from typing import Any from fastapi import
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/__init__.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0a2"
+__version__ = "0.6.0a3"
 __url__ = "https://github.com/amisadmin/fastapi_amis_admin"
 
 import gettext
 import os
 
 from .utils.translation import i18n
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/admin.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     Type,
     TypeVar,
     Union,
 )
 
 from fastapi import Body, Depends, FastAPI, HTTPException, Request
 from pydantic import BaseModel
-from pydantic.fields import ModelField
 from pydantic.utils import deep_update
 from sqlalchemy import Column, Table, delete, insert
 from sqlalchemy.orm import InstrumentedAttribute, RelationshipProperty
 from sqlalchemy.sql.elements import Label
 from sqlalchemy.util import md5_hex
 from sqlalchemy_database import AsyncDatabase, Database
 from starlette import status
@@ -74,17 +73,17 @@
 )
 from fastapi_amis_admin.crud.schema import BaseApiOut, CrudEnum, Paginator
 from fastapi_amis_admin.crud.utils import (
     IdStrQuery,
     SqlalchemyDatabase,
     get_engine_db,
     parser_str_set_list,
-    schema_create_by_schema,
 )
 from fastapi_amis_admin.utils.functools import cached_property
+from fastapi_amis_admin.utils.pydantic import ModelField, create_model_by_model, model_fields
 from fastapi_amis_admin.utils.translation import i18n as _
 
 BaseAdminT = TypeVar("BaseAdminT", bound="BaseAdmin")
 PageSchemaAdminT = TypeVar("PageSchemaAdminT", bound="PageSchemaAdmin")
 ActionT = Union[Action, Awaitable[Action]]
 
 
@@ -549,15 +548,15 @@
         form.initApi = AmisAPI(method="GET", url=f"{self.router_path}{self.form_path}") if self.form_init else None
         form.title = ""
         actions = await self.get_actions(request, flag="item")
         if actions:
             form.actions = actions
         form.body = []
         if self.schema:
-            for modelfield in self.schema.__fields__.values():
+            for modelfield in model_fields(self.schema).values():
                 formitem = await self.get_form_item(request, modelfield)
                 if formitem:
                     form.body.append(formitem)
         return form
 
     def register_router(self):
         super().register_router()
@@ -565,15 +564,15 @@
             self.form_path,
             self.route_submit,
             methods=["POST"],
             response_model=BaseApiOut[self.schema_submit_out],
             dependencies=[Depends(self.page_permission_depend)],
         )
         if self.form_init:
-            self.schema_init_out = self.schema_init_out or schema_create_by_schema(
+            self.schema_init_out = self.schema_init_out or create_model_by_model(
                 self.schema, f"{self.__class__.__name__}InitOut", set_none=True
             )
             self.router.add_api_route(
                 self.form_path,
                 self.route_init,
                 methods=["GET"],
                 response_model=BaseApiOut[self.schema_init_out],
@@ -647,35 +646,34 @@
                 None,
                 [LinkModelForm.bind_model_admin(self, insfield) for insfield in self.link_model_fields],
             )
         )
         return self.link_model_forms
 
     async def get_list_display(self, request: Request) -> List[Union[SqlaField, TableColumn]]:
-        return self.list_display or list(self.schema_list.__fields__.values())
+        return self.list_display or list(model_fields(self.schema_list).values())
 
     async def get_list_filter(self, request: Request) -> List[Union[SqlaField, FormItem]]:
-        return self.list_filter or list(self.schema_filter.__fields__.values())
+        return self.list_filter or list(model_fields(self.schema_filter).values())
 
     async def get_column_quick_edit(self, request: Request, modelfield: ModelField) -> Optional[Dict[str, Any]]:
         item = await self.get_form_item(request, modelfield, action=CrudEnum.update)
         if not isinstance(item, (dict, BaseModel)):
             return None
         if isinstance(item, BaseModel):
             item = item.dict(exclude_none=True, by_alias=True, exclude={"name", "label"})
         item.update({"saveImmediately": True})
         if item.get("type") == "switch":
             item.update({"mode": "inline"})
         return item
 
     async def get_list_column(self, request: Request, modelfield: ModelField) -> TableColumn:
         column = self.amis_parser.as_table_column(modelfield)
-        if (
-            await self.has_update_permission(request, None, None)  # type: ignore
-            and modelfield.name in self.schema_update.__fields__
+        if await self.has_update_permission(request, None, None) and modelfield.name in model_fields(  # type: ignore
+            self.schema_update
         ):
             column.quickEdit = await self.get_column_quick_edit(request, modelfield)
         return column
 
     async def get_list_columns(self, request: Request) -> List[TableColumn]:
         columns = []
         for field in await self.get_list_display(request):
@@ -844,15 +842,15 @@
                 ),
                 Action(actionType="submit", label=_("Search"), level=LevelEnum.primary),
             ],
             trimValues=True,
         )
 
     async def get_create_form(self, request: Request, bulk: bool = False) -> Form:
-        fields = [field for field in self.schema_create.__fields__.values() if field.name != self.pk_name]
+        fields = [field for field in model_fields(self.schema_create).values() if field.name != self.pk_name]
         if not bulk:
             return Form(
                 api=f"post:{self.router_path}/item",
                 name=CrudEnum.create,
                 body=await self._conv_modelfields_to_formitems(request, fields, CrudEnum.create),
             )
         columns, keys = [], {}
@@ -883,15 +881,15 @@
             ],
         )
 
     async def get_update_form(self, request: Request, bulk: bool = False) -> Form:
         extra = {}
         if not bulk:
             api = f"put:{self.router_path}/item/${self.pk_name}"
-            fields = self.schema_update.__fields__.values()
+            fields = model_fields(self.schema_update).values()
             if self.schema_read:
                 extra["initApi"] = f"get:{self.router_path}/item/${self.pk_name}"
         else:
             api = f"put:{self.router_path}/item/" + "${ids|raw}"
             fields = self.bulk_update_fields
         return Form(
             api=api,
@@ -902,15 +900,15 @@
             **extra,
         )
 
     async def get_read_form(self, request: Request) -> Form:
         return Form(
             initApi=f"get:{self.router_path}/item/${self.pk_name}",
             name=CrudEnum.read,
-            body=await self._conv_modelfields_to_formitems(request, self.schema_read.__fields__.values(), CrudEnum.read),
+            body=await self._conv_modelfields_to_formitems(request, model_fields(self.schema_read).values(), CrudEnum.read),
             submitText=None,
             static=True,
         )
 
     async def get_read_action(self, request: Request) -> Optional[Action]:
         if not self.schema_read:
             return None
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/handlers.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/parser.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import datetime
 from enum import Enum
 from typing import Any, Generator, Iterable, Type, TypeVar, Union
 
+from fastapi._compat import Undefined, field_annotation_is_scalar_sequence, field_annotation_is_sequence
 from pydantic import BaseModel, Json
-from pydantic.fields import ModelField
 from pydantic.utils import deep_update, smart_deepcopy
-from typing_extensions import get_origin
 
 from fastapi_amis_admin import amis
 from fastapi_amis_admin.amis import AmisNode
 from fastapi_amis_admin.amis.components import (
     Form,
     FormItem,
     InputArray,
     Remark,
     TableColumn,
     Validation,
 )
 from fastapi_amis_admin.amis.constants import LabelEnum
 from fastapi_amis_admin.models.enums import Choices
+from fastapi_amis_admin.utils.pydantic import (
+    PYDANTIC_V2,
+    ModelField,
+    annotation_outer_type,
+    field_allow_none,
+    field_json_schema_extra,
+    field_outer_type,
+    model_config_attr,
+    model_fields,
+    scalar_sequence_inner_type,
+)
 from fastapi_amis_admin.utils.translation import i18n as _
 
 _T = TypeVar("_T")
 
 
 class AmisParser:
     """AmisParser,used to parse pydantic fields to amis form item or table column.
@@ -100,83 +110,86 @@
         Args:
             model: Pydantic model
             set_default: Is set default value
             is_filter: Is filter form
         Returns:
             amis.Form
         """
-        form = amis.Form(title=getattr(model.Config, "title", None), size="lg")  # type: ignore
+        form = amis.Form(title=model_config_attr(model, "title", None), size="lg")  # type: ignore
         form.body = [
             self.as_form_item(modelfield, set_default=set_default, is_filter=is_filter)
-            for modelfield in model.__fields__.values()
+            for modelfield in model_fields(model).values()
         ]
         # InputSubForm
         return form
 
     def update_common_attrs(
         self,
         modelfield: ModelField,
         item: Union[FormItem, TableColumn],
         set_default: bool = False,
         is_filter: bool = False,
     ):
         """Set common attributes for FormItem and TableColumn."""
         field_info = modelfield.field_info
         if not is_filter:
-            if field_info.max_length:
-                item.maxLength = field_info.max_length
-            if field_info.min_length:
-                item.minLength = field_info.min_length
-            item.required = modelfield.required and not issubclass(modelfield.type_, bool)
-            if set_default:
+            if not PYDANTIC_V2:
+                if field_info.max_length:
+                    item.maxLength = field_info.max_length
+                if field_info.min_length:
+                    item.minLength = field_info.min_length
+            type_ = annotation_outer_type(modelfield.type_)
+            item.required = modelfield.required and not issubclass(type_, bool)
+            if set_default and modelfield.default is not Undefined:
                 item.value = modelfield.default
         item.name = modelfield.alias
         item.label = _(field_info.title) if field_info.title else _(modelfield.name)  # The use of I18N
         label_name = "labelRemark" if isinstance(item, FormItem) else "remark"
         if getattr(item, label_name, None) is None:
             label = Remark(content=_(field_info.description)) if field_info.description else None  # The use of I18N
             setattr(item, label_name, label)
         return item
 
     def _get_form_item_from_kwargs(self, modelfield: ModelField, is_filter: bool = False) -> FormItem:
         formitem = self.get_field_amis_extra(modelfield, ["amis_form_item", "amis_filter_item"][is_filter])
         # List type parse to InputArray
-        if issubclass(modelfield.type_, (list, set)) or (
-            modelfield.outer_type_ and get_origin(modelfield.outer_type_) in {list, set}
-        ):
+        outer_type = field_outer_type(modelfield) or modelfield.type_
+        if field_annotation_is_sequence(outer_type):
             if not isinstance(formitem, FormItem):
                 formitem = InputArray(**formitem)
             elif not isinstance(formitem, InputArray):
                 return formitem
             # Parse the internal type of the list.
-            kwargs = self.get_field_amis_form_item_type(type_=modelfield.type_, is_filter=is_filter)
+            type_ = scalar_sequence_inner_type(outer_type)
+            kwargs = self.get_field_amis_form_item_type(type_=type_, is_filter=is_filter)
             update = formitem.items.amis_dict() if formitem.items else {}
             if update:
                 kwargs = deep_update(kwargs, update)
             formitem.items = FormItem(**kwargs)
         if isinstance(formitem, FormItem):
             return formitem
         # other type parse to FormItem
         kwargs = self.get_field_amis_form_item_type(
             type_=modelfield.type_,
             is_filter=is_filter,
-            required=modelfield.required and not modelfield.allow_none,
+            required=modelfield.required and not field_allow_none(modelfield),
         )
         return FormItem(**kwargs).update_from_dict(formitem)
 
     def _get_table_column_from_kwargs(self, modelfield: ModelField) -> TableColumn:
         table_column = self.get_field_amis_extra(modelfield, "amis_table_column")
         if isinstance(table_column, TableColumn):
             return table_column
         kwargs = self.get_field_amis_table_column_type(modelfield.type_)
         return TableColumn(**kwargs).update_from_dict(table_column)
 
     def get_field_amis_table_column_type(self, type_: Type) -> dict:
         """Get amis table column type from pydantic model field type."""
         kwargs = {}
+        type_ = annotation_outer_type(type_)
         if type_ in {str, Any}:
             pass
         elif issubclass(type_, bool):
             kwargs["type"] = "switch"
             kwargs["filterable"] = {
                 "options": [
                     {"label": _("YES"), "value": True},
@@ -195,25 +208,26 @@
             kwargs["filterable"] = {"options": [{"label": v, "value": k} for k, v in items]}
             kwargs["map"] = {
                 k: f"<span class='label label-{label.value}'>{v}</span>"
                 for (k, v), label in zip(items, cyclic_generator(LabelEnum))
             }
         elif issubclass(type_, (dict, Json)):
             kwargs["type"] = "json"
-        elif issubclass(type_, (list, set)):
+        elif field_annotation_is_scalar_sequence(type_):
             kwargs["type"] = "each"
             kwargs["items"] = {
                 "type": "tpl",
                 "tpl": "<span class='label label-info m-l-sm'><%= this.item %></span>",
             }
         return kwargs
 
     def get_field_amis_form_item_type(self, type_: Any, is_filter: bool, required: bool = False) -> dict:
         """Get amis form item type from pydantic model field type."""
         kwargs = {}
+        type_ = annotation_outer_type(type_)
         if type_ in {str, Any}:
             kwargs["type"] = "input-text"
         elif issubclass(type_, Enum):
             items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
             kwargs.update(
                 {
                     "type": "select",
@@ -259,29 +273,29 @@
             kwargs["format"] = "HH:mm:ss"
         elif issubclass(type_, (dict, Json)):
             kwargs["type"] = "json-editor"
         elif issubclass(type_, BaseModel):
             # pydantic model parse to InputSubForm
             kwargs["type"] = "input-sub-form"
             kwargs["labelField"] = get_model_label_field_name(type_)
-            kwargs["btnLabel"] = getattr(type_.Config, "title", None)
+            kwargs["btnLabel"] = model_config_attr(type_, "title", None)
             kwargs["form"] = self.as_amis_form(type_, is_filter=is_filter).amis_dict()
         else:
             kwargs["type"] = "input-text"
         return kwargs
 
     def get_field_amis_extra(
         self,
         modelfield: ModelField,
         name: str,
     ) -> Union[FormItem, TableColumn, dict]:
         """Get amis extra from pydantic model field.
         You can pass amis configuration through the extra parameter of the pydantic model field.
         """
-        extra = modelfield.field_info.extra.get(name, {})
+        extra = field_json_schema_extra(modelfield).get(name, {})
         if not extra:
             return {}
         if callable(extra):
             return extra()
         extra = smart_deepcopy(extra)
         if isinstance(extra, (AmisNode, dict)):
             pass
@@ -295,14 +309,14 @@
 def cyclic_generator(iterable: Iterable[_T]) -> Generator[_T, None, None]:
     while True:
         yield from iterable
 
 
 def get_model_label_field_name(model: Type[BaseModel]) -> str:
     """Get model label field name. The label field is used to display the model name in the form."""
-    label_field_name = getattr(model.Config, "label_field_name", None)
+    label_field_name = model_config_attr(model, "label_field_name", None)
     if label_field_name:
         return label_field_name
-    for filed in model.__fields__.values():
+    for filed in model_fields(model).values():
         if filed.alias in ["name", "title", "label"]:
             return filed.alias
     return "id"
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/site.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/README.md` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/components.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,14 @@
     type: str = "input-text"  # Specify the form item type
     className: str = None  # The outermost class name of the form
     inputClassName: str = None  # Form controller class name
     labelClassName: str = None  # class name of label
     name: str = None  # Field name, specifying the key when the form item is submitted
     label: Template = None  # form item label template or false
     labelAlign: str = None  # "right" # Form item label alignment, default right alignment, only effective when mode is
-    value: Union[int, str] = None  # field value
     labelRemark: RemarkT = None  # Form item label description
     description: Template = None  # Form item description
     placeholder: str = None  # Form item description
     inline: bool = None  # whether it is inline mode
     submitOnChange: bool = None  # whether to submit the current form when the value of the form item changes.
     disabled: bool = None  # whether the current form item is disabled
     disabledOn: Expression = None  # The condition for whether the current form item is disabled
@@ -1551,15 +1550,15 @@
         icon: str = None  # Icon name, support fontawesome v4 or use url (priority is higher than color)
         className: str = None  # Custom CSS class name
 
     type: str = "steps"
     steps: List[StepItem] = None  # default [], List of Steps
     source: API = None  # Data source, you can obtain current variables through data mapping, or configure API objects
     name: str = None  # Associated context variable
-    value: Union[int, str] = None  # default -, Set the default value, expressions are not supported
+    value: Union[int, str, None] = None  # default -, Set the default value, expressions are not supported
     status: Union[StepStatusEnum, dict] = None  # default -, State of the steps
     className: str = None  # Custom CSS class name
     mode: Literal["vertical", "horizontal"] = "horizontal"  # Specifies the step bar direction.
     labelPlacement: Literal["vertical", "horizontal"] = "horizontal"  # Specify the label placement position.
     # The default is to place it horizontally to the right of the icon, and optional (vertical) below the icon.
     progressDot: bool = None  # Default False, show dotted step bar
 
@@ -2704,27 +2703,27 @@
 
     type: str = "spinner"
 
 
 class TableCRUD(CRUD, Table):
     """Form Table CRUD"""
 
-    mode = "table"
+    mode: str = "table"
 
 
 class CardCRUD(CRUD, Cards):
     """Form Card CRUD"""
 
-    mode = "cards"
+    mode: str = "cards"
 
 
 class ListCRUD(CRUD, ListDisplay):
     """Form Card CRUD"""
 
-    mode = "list"
+    mode: str = "list"
 
 
 class Avatar(AmisNode):
     """avatar"""
 
     type: str = "avatar"
     className: str = None  # The class name of the outer dom
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/constants.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/app.html` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/templates/app.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/page.html` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/templates/page.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/types.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/amis/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 from typing import Any, Dict, List, Union
 
-from pydantic import BaseModel, Extra
-
-try:
-    import ujson as json
-except ImportError:
-    import json
+from fastapi_amis_admin.utils.pydantic import AllowExtraModelMixin
 
 Expression = str
-Template = Union[str, "Tpl"]
-SchemaNode = Union[Template, "AmisNode", List["AmisNode"], Dict[str, Any], List[Dict[str, Any]]]
+
+
 OptionsNode = Union[List[Dict[str, Any]], List[str]]
 
 
-class BaseAmisModel(BaseModel):
-    class Config:
-        extra = Extra.allow
-        json_loads = json.loads
-        json_dumps = json.dumps
+class BaseAmisModel(AllowExtraModelMixin):
+    """Base model for amis"""
 
     def amis_json(self):
         return self.json(exclude_none=True, by_alias=True)
 
     def amis_dict(self):
         return self.dict(exclude_none=True, by_alias=True)
 
@@ -53,16 +45,19 @@
     id: str = None
     name: str = None  # In other components, when used as a variable map
     value: Any = None  # The value of the component
     onEvent: dict = None
     events: Dict[str, Any] = None  # Specifies the amis behavior triggered by the component
 
 
+SchemaNode = Union[str, AmisNode, List[AmisNode], Dict[str, Any], List[Dict[str, Any]]]
+
+
 class AmisAPI(BaseAmisModel):
-    url: Template  # Current interface API address
+    url: str  # Current interface API address
     method: str = None  # 'GET' # Request method: get, post, put, delete
     data: Union[str, dict] = None  # The requested data body, supports data mapping
     dataType: str = None  # The default is json and can be configured as form or form-data.
     # When data contains files, it will automatically use form-data (multipart/form-data) format.
     # When configured as form, the format is application/x-www-form-urlencoded.
     qsOptions: Union[str, dict] = None  # Useful when dataType is form or form-data.
     # For specific parameters, please refer to here, the default setting is: { arrayFormat: 'indices',
@@ -94,14 +89,17 @@
 
 class Tpl(AmisNode):
     type: str = "tpl"  # Specify as Tpl component
     tpl: str  # configuration template
     className: str = None  # The class name of the outer Dom
 
 
+Template = Union[str, Tpl]
+
+
 class Event(BaseAmisModel):
     actionType: str = None  # Action name
     args: dict = None  # Action parameter {key:value}, support data mapping
     preventDefault: Union[bool, Expression] = None  # "False" # Prevent event default behavior, > 1.10.0 and above
     # support expressions
     stopPropagation: Union[bool, Expression] = None  # "False" # Stop subsequent action execution, > 1.10.0 and above
     # supports expressions
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/README.md` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/_sqlalchemy.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/_sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import re
 from enum import Enum
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
@@ -10,30 +9,38 @@
     List,
     Optional,
     Pattern,
     Tuple,
     Type,
     Union,
 )
-from uuid import UUID
 
 from fastapi import APIRouter, Body, Depends
-from fastapi.encoders import DictIntStrAny, SetIntStr
-from pydantic import EmailStr, Extra, IPvAnyAddress, Json
-from pydantic.fields import ModelField
-from pydantic.utils import ValueItems
+from fastapi._compat import field_annotation_is_scalar
+from fastapi.types import IncEx
+from pydantic import Extra
 from sqlalchemy import Column, Table, func
 from sqlalchemy.engine import Result
 from sqlalchemy.future import select
 from sqlalchemy.orm import InstrumentedAttribute, Session, object_session
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import BinaryExpression, Label, UnaryExpression
 from starlette.requests import Request
 from typing_extensions import Literal
 
+from fastapi_amis_admin.utils.pydantic import (
+    PYDANTIC_V2,
+    ModelField,
+    ValueItems,
+    annotation_outer_type,
+    create_model_by_fields,
+    field_allow_none,
+    model_fields,
+)
+
 try:
     from functools import cached_property
 except ImportError:
     from sqlalchemy.util.langhelpers import memoized_property as cached_property
 
 from .base import (
     BaseCrud,
@@ -57,15 +64,14 @@
 from .schema import BaseApiOut, ItemListSchema
 from .utils import (
     IdStrQuery,
     ItemIdListDepend,
     SqlalchemyDatabase,
     get_engine_db,
     parser_str_set_list,
-    schema_create_by_modelfield,
 )
 
 sql_operator_pattern: Pattern = re.compile(r"^\[(=|<=|<|>|>=|!|!=|<>|\*|!\*|~|!~|-)]")
 sql_operator_map: Dict[str, str] = {
     "=": "__eq__",
     "<=": "__le__",
     "<": "__lt__",
@@ -232,19 +238,19 @@
 
 
 class SqlalchemyCrud(
     BaseCrud[SchemaModelT, SchemaListT, SchemaFilterT, SchemaCreateT, SchemaReadT, SchemaUpdateT], SqlalchemySelector[TableModelT]
 ):
     engine: SqlalchemyDatabase = None  # sqlalchemy engine
     create_fields: List[SqlaInsAttr] = []  # Create item data field
-    create_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None
+    create_exclude: Optional[IncEx] = None
     """create exclude fields, such as: {'id', 'key', 'name'} or {'id': True, 'category': {'id', 'name'}}."""
     update_fields: List[SqlaPropertyField] = []
     """model update fields;support model property and relationship field."""
-    update_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None
+    update_exclude: Optional[IncEx] = None
     """update exclude fields, such as: {'id', 'key', 'name'} or {'id': True, 'category': {'id', 'name'}}."""
     read_fields: List[SqlaPropertyField] = []
     """Model read fields; used in route_read, note the difference between readonly_fields and read_fields.
     default is None, means not use read route."""
 
     def __init__(
         self,
@@ -275,83 +281,85 @@
             self._select_entities.values(),
             save_class=(
                 Label,
                 ModelField,
             ),
         )
         # Create the schema using the model fields
-        return schema_create_by_modelfield(
-            schema_name=f"{self.schema_name_prefix}List",
-            modelfields=modelfields,
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}List",
+            fields=modelfields,
             set_none=True,
             extra=Extra.allow,
         )
 
     def _create_schema_filter(self) -> Type[SchemaFilterT]:
         # Get the filter fields from the list filter or select entities
         list_filter = self.list_filter or self._select_entities.values()
         # Filter out the model fields from the filter fields
         modelfields = self.parser.filter_modelfield(list_filter, save_class=(Label,))
         # Modify the modelfields if necessary
         for modelfield in modelfields:
-            if not issubclass(modelfield.type_, (Enum, bool)) and issubclass(
-                modelfield.type_,
-                (int, float, datetime.datetime, datetime.date, datetime.time, Json, EmailStr, IPvAnyAddress, UUID),
-            ):
+            type_ = annotation_outer_type(modelfield.type_)
+            if field_annotation_is_scalar(modelfield.type_) and issubclass(type_, (Enum, bool, str)):
+                continue
+            if PYDANTIC_V2:
+                modelfield.field_info.annotation = str
+            else:
                 modelfield.type_ = str
                 modelfield.outer_type_ = str
                 modelfield.validators = []
         # Create the schema using the model fields
-        return schema_create_by_modelfield(
-            schema_name=f"{self.schema_name_prefix}Filter",
-            modelfields=modelfields,
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Filter",
+            fields=modelfields,
             set_none=True,
         )
 
     def _create_schema_read(self) -> Optional[Type[SchemaReadT]]:
         if not self.read_fields:
             return None
         # Filter out any non-model fields from the read fields
         modelfields = self.parser.filter_modelfield(self.read_fields)
         # Create the schema using the model fields
-        return schema_create_by_modelfield(
-            f"{self.schema_name_prefix}Read",
-            modelfields,
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Read",
+            fields=modelfields,
             orm_mode=True,
         )
 
     def _create_schema_update(self) -> Type[SchemaUpdateT]:
         # Set the update fields to the model insfields if not provided
         self.update_fields = self.update_fields or self.model_insfields
         # Exclude certain fields if specified
         exclude = {k for k, v in ValueItems.merge(self.update_exclude, {}).items() if not isinstance(v, (dict, list, set))} or {
             self.pk_name
         }
         # Filter out any non-model fields from the update fields
         modelfields = self.parser.filter_modelfield(self.update_fields, exclude=exclude)
         # Create the schema using the model fields
-        return schema_create_by_modelfield(
-            f"{self.schema_name_prefix}Update",
-            modelfields,
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Update",
+            fields=modelfields,
             set_none=True,
         )
 
     def _create_schema_create(self) -> Type[SchemaCreateT]:
         # Set the create fields to the model insfields if not provided
         self.create_fields = self.create_fields or self.model_insfields
         # Exclude certain fields if specified
         exclude = {k for k, v in ValueItems.merge(self.create_exclude, {}).items() if not isinstance(v, (dict, list, set))} or {
             self.pk_name
         }
         # Filter out any non-model fields from the create fields
         modelfields = self.parser.filter_modelfield(self.create_fields, exclude=exclude)
         # Create the schema using the model fields
-        return schema_create_by_modelfield(
-            f"{self.schema_name_prefix}Create",
-            modelfields,
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Create",
+            fields=modelfields,
         )
 
     def create_item(self, item: Dict[str, Any]) -> TableModelT:
         """Create a database orm object through a dictionary."""
         return self.model(**item)
 
     def read_item(self, obj: TableModelT) -> SchemaReadT:
@@ -433,15 +441,15 @@
         self,
         request: Request,
         obj: SchemaUpdateT,
         item_id: Union[List[str], List[int]],
         **kwargs,
     ) -> Dict[str, Any]:
         data = obj.dict(exclude=self.update_exclude, exclude_unset=True, by_alias=True)
-        data = {key: val for key, val in data.items() if val is not None or self.model.__fields__[key].allow_none}
+        data = {key: val for key, val in data.items() if val is not None or field_allow_none(model_fields(self.model)[key])}
         return data
 
     async def on_filter_pre(self, request: Request, obj: SchemaFilterT, **kwargs) -> Dict[str, Any]:
         return obj and {k: v for k, v in obj.dict(exclude_unset=True, by_alias=True).items() if v is not None}
 
     async def on_list_after(self, request: Request, result: Result, data: ItemListSchema, **kwargs) -> ItemListSchema:
         """Parse the database data query result dictionary into schema_list."""
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/base.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from fastapi import APIRouter, Depends
 from pydantic import BaseModel
 from sqlalchemy.exc import IntegrityError
 from starlette import status
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 
+from ..utils.pydantic import create_model_by_model
 from .schema import BaseApiOut, CrudEnum, ItemListSchema, Paginator
-from .utils import schema_create_by_schema
 
 SchemaModelT = TypeVar("SchemaModelT", bound=BaseModel)
 SchemaListT = TypeVar("SchemaListT", bound=BaseModel)
 SchemaFilterT = TypeVar("SchemaFilterT", bound=BaseModel)
 SchemaCreateT = TypeVar("SchemaCreateT", bound=BaseModel)
 SchemaReadT = TypeVar("SchemaReadT", bound=BaseModel)
 SchemaUpdateT = TypeVar("SchemaUpdateT", bound=BaseModel)
@@ -128,29 +128,29 @@
         )
         return self
 
     def _create_schema_list(self) -> Type[SchemaListT]:
         return self.schema_model
 
     def _create_schema_filter(self) -> Type[SchemaFilterT]:
-        return schema_create_by_schema(self.schema_list, f"{self.schema_name_prefix}Filter", set_none=True)
+        return create_model_by_model(self.schema_list, f"{self.schema_name_prefix}Filter", set_none=True)
 
     def _create_schema_read(self) -> Optional[Type[SchemaReadT]]:
         return None
 
     def _create_schema_update(self) -> Type[SchemaUpdateT]:
-        return schema_create_by_schema(
+        return create_model_by_model(
             self.schema_model,
             f"{self.schema_name_prefix}Update",
             exclude={self.pk_name},
             set_none=True,
         )
 
     def _create_schema_create(self) -> Type[SchemaCreateT]:
-        return schema_create_by_schema(
+        return create_model_by_model(
             self.schema_model,
             f"{self.schema_name_prefix}Create",
             exclude={self.pk_name},
         )
 
     @property
     def route_list(self) -> Callable[..., Any]:
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/parser.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import datetime
 from functools import lru_cache
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 
 import sqlalchemy
-from fastapi.utils import create_cloned_field
+from fastapi.utils import create_cloned_field, create_response_field
 from pydantic import BaseConfig, BaseModel
-from pydantic.datetime_parse import parse_date, parse_datetime
-from pydantic.fields import Field, FieldInfo, ModelField
+from pydantic.fields import Field, FieldInfo
 from sqlalchemy import Column, String, Table
 from sqlalchemy.engine import Row
 from sqlalchemy.orm import ColumnProperty, DeclarativeMeta, InstrumentedAttribute, RelationshipProperty
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import Label
 
 from fastapi_amis_admin.crud.base import SchemaModelT
-from fastapi_amis_admin.crud.utils import schema_create_by_modelfield
+from fastapi_amis_admin.utils.pydantic import (
+    PYDANTIC_V2,
+    ModelField,
+    create_model_by_fields,
+    model_config_attr,
+    model_fields,
+    parse_date,
+    parse_datetime,
+)
 
 SqlaInsAttr = Union[str, InstrumentedAttribute]
 SqlaField = Union[SqlaInsAttr, Label]
 SqlaPropertyField = Union[SqlaInsAttr, "PropertyField"]
 ModelFieldType = Union[ModelField, "ModelFieldProxy"]
 SchemaT = TypeVar("SchemaT", bound=BaseModel)
 TableModel = DeclarativeMeta
@@ -42,23 +49,33 @@
     """
 
     def __init__(self, modelfield: ModelField, update: Dict[str, Any] = None):
         self.__dict__["_modelfield"] = modelfield
         self.__dict__["_update"] = update or {}
 
     def __getattr__(self, item):
-        if item == "new_model_field":
+        if item == "cloned_field":
             return self.__dict__[item]
         return self.__dict__["_update"].get(item, getattr(self.__dict__["_modelfield"], item))
 
     def __setattr__(self, key, value):
         self.__dict__["_update"][key] = value
 
     def cloned_field(self):
         modelfield = create_cloned_field(self.__dict__["_modelfield"])
+        if PYDANTIC_V2:
+            kwargs = self.__dict__["_update"]
+            name = kwargs.get("name", modelfield.name)
+            alias = kwargs.get("alias", None)
+            if alias:
+                kwargs.setdefault("validation_alias", alias)
+                kwargs.setdefault("serialization_alias", alias)
+            field_info = FieldInfo.merge_field_infos(modelfield.field_info, **kwargs)
+            field_info.annotation = modelfield.field_info.annotation
+            return ModelField(field_info=field_info, name=name, mode=modelfield.mode)
         for k, v in self.__dict__["_update"].items():
             setattr(modelfield, k, v)
         return modelfield
 
 
 class TableModelParser:
     _name_format = "{model_name}_{field_name}"
@@ -74,40 +91,35 @@
     def get_table_model_insfields(table_model: Type[TableModelT]) -> Dict[str, InstrumentedAttribute]:
         """Get sqlalchemy InstrumentedAttribute from InspecTable."""
         return {name: field for name, field in table_model.__dict__.items() if isinstance(field, InstrumentedAttribute)}
 
     @staticmethod
     def get_table_model_fields(table_model: Type[TableModelT]) -> Dict[str, ModelField]:
         """Get pydantic ModelField from sqlalchemy InspecTable."""
-        if hasattr(table_model, "__fields__"):
-            return table_model.__fields__
-        elif hasattr(table_model, "__schema__") and issubclass(table_model.__schema__, BaseModel):
-            return table_model.__schema__.__fields__
+        if issubclass(table_model, BaseModel):
+            return model_fields(table_model)
+        elif hasattr(table_model, "__pydantic_model__") and issubclass(table_model.__pydantic_model__, BaseModel):
+            return model_fields(table_model.__pydantic_model__)
         return {}
 
     @staticmethod
     def get_table_model_schema(table_model: Type[TableModelT]) -> Optional[Type[BaseModel]]:
         """Get pydantic schema from sqlalchemy InspecTable."""
 
         if issubclass(table_model, BaseModel):
             return table_model
-        elif hasattr(table_model, "__schema__") and issubclass(table_model.__schema__, BaseModel):
-            return table_model.__schema__
-        elif hasattr(table_model, "__fields__"):
-            table_model.__schema__ = schema_create_by_modelfield(
-                table_model.__name__, table_model.__fields__.values(), orm_mode=True
-            )
-            return table_model.__schema__
+        elif hasattr(table_model, "__pydantic_model__") and issubclass(table_model.__pydantic_model__, BaseModel):
+            return table_model.__pydantic_model__
         insfields = TableModelParser.get_table_model_insfields(table_model)
         if not insfields:
             return None
         modelfields = [insfield_to_modelfield(insfield) for insfield in insfields.values()]
         modelfields = list(filter(None, modelfields))
-        table_model.__schema__ = schema_create_by_modelfield(table_model.__name__, modelfields, orm_mode=True)
-        return table_model.__schema__
+        table_model.__pydantic_model__ = create_model_by_fields(table_model.__name__, modelfields, orm_mode=True)
+        return table_model.__pydantic_model__
 
     def get_modelfield(self, field: Union[ModelField, SqlaInsAttr, Label], clone: bool = False) -> Optional[ModelFieldType]:
         """Get pydantic ModelField from sqlmodel field.
         Args:
             field:  ModelField, SQLModelField or Label
             clone:  Whether to return a cloned of the original ModelField.
 
@@ -115,15 +127,15 @@
         """
         modelfield = None
         update = {}
         if isinstance(field, InstrumentedAttribute):
             modelfield = self.get_table_model_fields(field.class_).get(field.key, None)
             if not modelfield:  # Maybe it's a declared_attr or column_property.
                 return None
-            if field.class_.__table__ is not self.__fields__:
+            if field.class_.__table__ is not self.__table__:
                 update = {
                     "name": self.get_name(field),
                     "alias": self.get_alias(field),
                 }
         elif isinstance(field, str) and field in self.__fields__:
             modelfield = self.__fields__[field]
         elif isinstance(field, ModelField):
@@ -245,31 +257,31 @@
         return str
 
 
 def _get_label_modelfield(label: Label) -> ModelField:
     modelfield = getattr(label, "__ModelField__", None)
     if modelfield is None:
         try:
-            python_type = label.expression.type.python_type
+            type_ = label.expression.type.python_type
         except NotImplementedError:
-            python_type = str
-        modelfield = ModelField(
+            type_ = str
+        modelfield = create_response_field(
             name=label.key,
-            type_=python_type,
-            class_validators={},
-            model_config=BaseConfig,
+            type_=type_,
         )
         label.__ModelField__ = modelfield
     return modelfield
 
 
-def LabelField(label: Label, field: FieldInfo) -> Label:
+def LabelField(label: Label, field: FieldInfo, type_: type = str) -> Label:
     """Use for adding FieldInfo to sqlalchemy Label type"""
     modelfield = _get_label_modelfield(label)
     field.alias = label.key
+    if PYDANTIC_V2:
+        field.annotation = type_
     modelfield.field_info = field
     label.__ModelField__ = modelfield
     return label
 
 
 class PropertyField(ModelField):
     """Use this to quickly initialize a ModelField, mainly used in schema_read and schema_update"""
@@ -279,17 +291,23 @@
         *,
         name: str,
         type_: Type[Any],
         required: bool = False,
         field_info: Optional[FieldInfo] = None,
         **kwargs: Any,
     ) -> None:
-        kwargs.setdefault("class_validators", {})
-        kwargs.setdefault("model_config", BaseConfig)
-        super().__init__(name=name, type_=type_, required=required, field_info=field_info, **kwargs)
+        if PYDANTIC_V2:
+            field_info = field_info or FieldInfo(default=None)
+            field_info.annotation = type_
+        else:
+            kwargs.setdefault("type_", type_)
+            kwargs.setdefault("required", required)
+            kwargs.setdefault("class_validators", {})
+            kwargs.setdefault("model_config", BaseConfig)
+        super().__init__(name=name, field_info=field_info, **kwargs)
 
 
 def get_insfield_by_key(table_model: Type[TableModelT], key: str) -> Optional[InstrumentedAttribute]:
     """Get the field of the model according to the alias"""
     for insfield in table_model.__dict__.values():
         if isinstance(insfield, InstrumentedAttribute) and insfield.key == key:
             return insfield
@@ -303,15 +321,16 @@
         if field.alias == alias:
             return field
     return None
 
 
 def parse_obj_to_schema(obj: SchemaModelT, schema: Type[SchemaT]) -> SchemaT:
     """parse obj to schema"""
-    parse = schema.from_orm if getattr(schema.Config, "orm_mode", False) else schema.parse_obj
+    orm_mode = model_config_attr(schema, "orm_mode", False) or model_config_attr(schema, "from_attributes", False)
+    parse = schema.from_orm if orm_mode else schema.parse_obj
     return parse(obj)
 
 
 def insfield_to_modelfield(insfield: InstrumentedAttribute) -> Optional[ModelField]:
     """InstrumentedAttribute to ModelField"""
     if not isinstance(insfield.property, ColumnProperty):
         return None
@@ -328,18 +347,21 @@
         elif expression.default.is_callable:
             field_info_kwargs["default_factory"] = expression.default.arg
             required = False
     if isinstance(expression.type, String):
         field_info_kwargs["max_length"] = expression.type.length
     if "default_factory" not in field_info_kwargs:
         field_info_kwargs["default"] = default
-    return ModelField(
-        name=insfield.key,
-        type_=expression.type.python_type,
-        required=required,
-        class_validators={},
-        model_config=BaseConfig,
-        field_info=Field(
-            title=expression.comment,
-            **field_info_kwargs,
-        ),
+    type_ = expression.type.python_type
+    if PYDANTIC_V2:
+        field_info_kwargs["annotation"] = type_
+    return create_response_field(
+        name=insfield.key, type_=type_, required=required, field_info=Field(title=expression.comment, **field_info_kwargs)
     )
+
+
+def register_model(schema: Type[SchemaT]):
+    def decorator(model: Type[TableModelT]) -> Type[TableModelT]:
+        model.__pydantic_model__ = schema
+        return model
+
+    return decorator
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/schema.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/crud/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,33 @@
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 
-from pydantic import BaseModel, Extra
-from pydantic.generics import GenericModel
-
-try:
-    import ujson as json
-except ImportError:
-    import json
+from fastapi_amis_admin.utils.pydantic import AllowExtraModelMixin, GenericModel
 
 _T = TypeVar("_T")
 
 
-class BaseApiSchema(BaseModel):
-    class Config:
-        extra = Extra.allow
-        json_loads = json.loads
-        json_dumps = json.dumps
-        json_encoders = {
-            datetime: lambda v: v.strftime("%Y-%m-%d %H:%M:%S"),
-        }
+class BaseApiSchema(AllowExtraModelMixin):
+    pass
 
 
-class BaseApiOut(GenericModel, Generic[_T], BaseApiSchema):
+class BaseApiOut(BaseApiSchema, GenericModel, Generic[_T]):
     status: int = 0
     msg: str = "success"
     data: Optional[_T] = None
-    code: int = None
+    code: Optional[int] = None
 
 
-class ItemListSchema(GenericModel, Generic[_T], BaseApiSchema):
+class ItemListSchema(BaseApiSchema, GenericModel, Generic[_T]):
     """Data list query return format."""
 
     items: List[_T] = []  # Data list
-    total: int = None  # Data total
-    query: Dict[str, Any] = None
-    filter: Dict[str, Any] = None
+    total: Optional[int] = None  # Data total
+    query: Optional[Dict[str, Any]] = None
+    filter: Optional[Dict[str, Any]] = None
 
 
 class CrudEnum(str, Enum):
     list = "list"
     create = "create"
     read = "read"
     update = "update"
```

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/base.pot` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/base.pot`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/enums.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/models/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/fields.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/models/fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/functools.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/utils/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/translation.py` & `fastapi_amis_admin-0.6.0a3/fastapi_amis_admin/utils/translation.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a2/pyproject.toml` & `fastapi_amis_admin-0.6.0a3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "fastapi>=0.97.0",
+    "fastapi>=0.100.0",
+    "pydantic>1.7.4",
     "sqlalchemy>=1.4.0",
     "python-multipart>=0.0.5",
     "sqlalchemy-database>=0.1.0,<0.2.0",
     "aiofiles>=0.17.0",
 ]
 
 
@@ -62,14 +63,15 @@
     "pytest >=6.2.4",
     "aiosqlite>=0.15.0",
     "pytest-asyncio>=0.17",
     "httpx>=0.24.0,<1.0",
     "jinja2 >=2.11.2,<4.0.0",
     "ujson>=4.0.1",
     "requests>=2.28.1",
+    "sqlmodel>=0.0.7",
 ]
 dev = [
     "pre-commit>=2.20.0",
     "ruff>=0.0.261",
 ]
 cli = [
     "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
```

### Comparing `fastapi_amis_admin-0.6.0a2/PKG-INFO` & `fastapi_amis_admin-0.6.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin
-Version: 0.6.0a2
+Version: 0.6.0a3
 Summary: FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. 
 Keywords: fastapi,fastapi-admin,fastapi-amis-admin,django-admin,sqlmodel,sqlalchemy
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
@@ -14,15 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi>=0.97.0
+Requires-Dist: fastapi>=0.100.0
+Requires-Dist: pydantic>1.7.4
 Requires-Dist: sqlalchemy>=1.4.0
 Requires-Dist: python-multipart>=0.0.5
 Requires-Dist: sqlalchemy-database>=0.1.0,<0.2.0
 Requires-Dist: aiofiles>=0.17.0
 Requires-Dist: fastapi-amis-admin-cli>=0.1.3,<0.2.0 ; extra == "cli"
 Requires-Dist: pre-commit>=2.20.0 ; extra == "dev"
 Requires-Dist: ruff>=0.0.261 ; extra == "dev"
@@ -34,14 +35,15 @@
 Requires-Dist: pytest >=6.2.4 ; extra == "test"
 Requires-Dist: aiosqlite>=0.15.0 ; extra == "test"
 Requires-Dist: pytest-asyncio>=0.17 ; extra == "test"
 Requires-Dist: httpx>=0.24.0,<1.0 ; extra == "test"
 Requires-Dist: jinja2 >=2.11.2,<4.0.0 ; extra == "test"
 Requires-Dist: ujson>=4.0.1 ; extra == "test"
 Requires-Dist: requests>=2.28.1 ; extra == "test"
+Requires-Dist: sqlmodel>=0.0.7 ; extra == "test"
 Project-URL: Documentation, http://docs.amis.work/
 Project-URL: Source, https://github.com/amisadmin/fastapi_amis_admin
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: sqlmodel
 Provides-Extra: standard
 Provides-Extra: test
@@ -195,15 +197,15 @@
 Base = declarative_base()
 
 
 # Create an SQLAlchemy model, see document for details: https://docs.sqlalchemy.org/en/14/orm/tutorial.html
 class Category(Base):
     __tablename__ = 'category'
     # Specify the Schema class corresponding to the model. It is recommended to specify it. If omitted, it can be automatically generated.
-    __schema__ = CategorySchema
+    __pydantic_model__ = CategorySchema
 
     id = Column(Integer, primary_key=True, nullable=False)
     name = Column(String(100), unique=True, index=True, nullable=False)
     description = Column(String(255), default='')
 ```
 
 - Method 3: Create model through `SQLAlchemy 2.0`.
@@ -217,15 +219,15 @@
     pass
 
 
 # Create an SQLAlchemy 2.0 model, see document for details: https://docs.sqlalchemy.org/en/20/orm/quickstart.html
 class Category(Base):
     __tablename__ = "category"
     # Specify the Schema class corresponding to the model. It is recommended to specify it. If omitted, it can be automatically generated.
-    __schema__ = CategorySchema
+    __pydantic_model__ = CategorySchema
 
     id: Mapped[int] = mapped_column(primary_key=True, nullable=False)
     name: Mapped[str] = mapped_column(String(100), unique=True, index=True, nullable=False)
     description: Mapped[str] = mapped_column(String(255), default="")
 ```
 
 - If you create a model through `sqlalchemy`, it is recommended to create a corresponding pydantic model at the same
```

