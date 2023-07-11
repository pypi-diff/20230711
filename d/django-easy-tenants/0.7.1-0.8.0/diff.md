# Comparing `tmp/django-easy-tenants-0.7.1.tar.gz` & `tmp/django_easy_tenants-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-tenants-0.7.1.tar", max compression
+gzip compressed data, was "django_easy_tenants-0.8.0.tar", max compression
```

## Comparing `django-easy-tenants-0.7.1.tar` & `django_easy_tenants-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1072 2022-09-05 19:24:18.723891 django-easy-tenants-0.7.1/LICENSE
--rw-r--r--   0        0        0     5224 2022-09-05 19:24:18.723891 django-easy-tenants-0.7.1/README.md
--rw-r--r--   0        0        0      202 2022-09-05 19:24:18.723891 django-easy-tenants-0.7.1/easy_tenants/__init__.py
--rw-r--r--   0        0        0      561 2022-09-05 19:24:18.723891 django-easy-tenants-0.7.1/easy_tenants/apps.py
--rw-r--r--   0        0        0      262 2022-09-05 19:24:18.723891 django-easy-tenants-0.7.1/easy_tenants/conf.py
--rw-r--r--   0        0        0       39 2022-09-05 19:24:18.727892 django-easy-tenants-0.7.1/easy_tenants/exceptions.py
--rw-r--r--   0        0        0     1746 2022-09-05 19:24:18.727892 django-easy-tenants-0.7.1/easy_tenants/models.py
--rw-r--r--   0        0        0     1383 2022-09-05 19:24:18.727892 django-easy-tenants-0.7.1/easy_tenants/storage.py
--rw-r--r--   0        0        0      924 2022-09-05 19:24:18.727892 django-easy-tenants-0.7.1/easy_tenants/utils.py
--rw-r--r--   0        0        0     1452 2022-09-05 19:24:20.932051 django-easy-tenants-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 django-easy-tenants-0.7.1/setup.py
--rw-r--r--   0        0        0     6302 1970-01-01 00:00:00.000000 django-easy-tenants-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5224 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/README.md
+-rw-r--r--   0        0        0      202 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/easy_tenants/__init__.py
+-rw-r--r--   0        0        0      561 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/easy_tenants/apps.py
+-rw-r--r--   0        0        0      284 2023-07-11 17:25:46.056916 django_easy_tenants-0.8.0/easy_tenants/conf.py
+-rw-r--r--   0        0        0       39 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/easy_tenants/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-11 17:25:46.056916 django_easy_tenants-0.8.0/easy_tenants/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 17:25:46.056916 django_easy_tenants-0.8.0/easy_tenants/management/commands/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-11 17:25:46.057916 django_easy_tenants-0.8.0/easy_tenants/management/commands/shell_tenant.py
+-rw-r--r--   0        0        0     1780 2023-07-11 13:24:27.787285 django_easy_tenants-0.8.0/easy_tenants/models.py
+-rw-r--r--   0        0        0     1383 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/easy_tenants/storage.py
+-rw-r--r--   0        0        0      924 2022-12-20 19:55:35.443992 django_easy_tenants-0.8.0/easy_tenants/utils.py
+-rw-r--r--   0        0        0     1636 2023-07-11 17:25:46.058916 django_easy_tenants-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 django_easy_tenants-0.8.0/PKG-INFO
```

### Comparing `django-easy-tenants-0.7.1/LICENSE` & `django_easy_tenants-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-tenants-0.7.1/README.md` & `django_easy_tenants-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `django-easy-tenants-0.7.1/easy_tenants/apps.py` & `django_easy_tenants-0.8.0/easy_tenants/apps.py`

 * *Files identical despite different names*

### Comparing `django-easy-tenants-0.7.1/easy_tenants/models.py` & `django_easy_tenants-0.8.0/easy_tenants/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,21 @@
             return queryset
 
         field = getattr(self.model, field_name).field.target_field
         filter_kwargs = {field_name: CurrentTenant(output_field=field)}
 
         return queryset.filter(**filter_kwargs)
 
-    def bulk_create(self, objs):
+    def bulk_create(self, objs, *args, **kwargs):
         tenant = get_current_tenant()
 
         for obj in objs:
             setattr(obj, field_name, tenant)
 
-        return super().bulk_create(objs)
+        return super().bulk_create(objs, *args, **kwargs)
 
 
 class TenantAwareAbstract(models.Model):
     """Abstract model that implements the model save defining a tenant"""
 
     class Meta:
         abstract = True
```

### Comparing `django-easy-tenants-0.7.1/easy_tenants/storage.py` & `django_easy_tenants-0.8.0/easy_tenants/storage.py`

 * *Files identical despite different names*

### Comparing `django-easy-tenants-0.7.1/easy_tenants/utils.py` & `django_easy_tenants-0.8.0/easy_tenants/utils.py`

 * *Files identical despite different names*

### Comparing `django-easy-tenants-0.7.1/pyproject.toml` & `django_easy_tenants-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-easy-tenants"
-version = "0.7.1"
+version = "0.8.0"
 description = "Easy to create applications that use tenants in django"
 authors = ["Cleiton Lima <cleiton.limapin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CleitonDeLima/django-easy-tenants"
 homepage = "https://github.com/CleitonDeLima/django-easy-tenants"
 classifiers = [
@@ -18,29 +18,27 @@
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
 ]
 packages = [
     {include = "easy_tenants"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = "^3.7"
 django-appconf = "^1.0.4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-django = "^4.5.2"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 ipython = "^7.34.0"
-tox = "^3.25.1"
-tox-gh-actions = "^2.9.1"
-django = ">=3.2"
 django-environ = "^0.9.0"
-black = "^22.8"
+black = "^22.12"
 isort = "^5.8.0"
 flake8 = "^5.0.4"
+psycopg2-binary = "^2.9.6"
 
 [tool.black]
 line-length = 80
 exclude = '''
 /(
     \.git
   | \.hg
@@ -58,10 +56,25 @@
 [tool.isort]
 profile = "black"
 line_length = 80
 multi_line_output = 3
 include_trailing_comma = true
 skip = "migrations"
 
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = """\
+    --strict-config
+    --strict-markers
+    --ds=tests.settings
+    """
+testpaths = [
+    "tests",
+]
+python_files = [
+    "tests.py",
+    "test_*.py",
+]
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django-easy-tenants-0.7.1/setup.py` & `django_easy_tenants-0.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,191 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-easy-tenants
+Version: 0.8.0
+Summary: Easy to create applications that use tenants in django
+Home-page: https://github.com/CleitonDeLima/django-easy-tenants
+License: MIT
+Author: Cleiton Lima
+Author-email: cleiton.limapin@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Dist: django-appconf (>=1.0.4,<2.0.0)
+Project-URL: Repository, https://github.com/CleitonDeLima/django-easy-tenants
+Description-Content-Type: text/markdown
 
-packages = \
-['easy_tenants']
+# easy-tenants
 
-package_data = \
-{'': ['*']}
+![Tests](https://github.com/CleitonDeLima/django-easy-tenants/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/CleitonDeLima/django-easy-tenants/branch/master/graph/badge.svg)](https://codecov.io/gh/CleitonDeLima/django-easy-tenants)
+[![PyPI Version](https://img.shields.io/pypi/v/django-easy-tenants.svg)](https://pypi.org/project/django-easy-tenants/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/django-easy-tenants.svg)](https://img.shields.io/pypi/dm/django-easy-tenants.svg)
 
-install_requires = \
-['django-appconf>=1.0.4,<2.0.0']
-
-setup_kwargs = {
-    'name': 'django-easy-tenants',
-    'version': '0.7.1',
-    'description': 'Easy to create applications that use tenants in django',
-    'long_description': '# easy-tenants\n\n![Tests](https://github.com/CleitonDeLima/django-easy-tenants/workflows/Tests/badge.svg)\n[![codecov](https://codecov.io/gh/CleitonDeLima/django-easy-tenants/branch/master/graph/badge.svg)](https://codecov.io/gh/CleitonDeLima/django-easy-tenants)\n[![PyPI Version](https://img.shields.io/pypi/v/django-easy-tenants.svg)](https://pypi.org/project/django-easy-tenants/)\n[![PyPI downloads](https://img.shields.io/pypi/dm/django-easy-tenants.svg)](https://img.shields.io/pypi/dm/django-easy-tenants.svg)\n\n\nThis is a Django app for managing multiple tenants on the same project\ninstance using a shared approach.\n\n\n## Background\n\nThere are typically three solutions for solving the multitenancy problem:\n\n1. Isolated Approach: Separate Databases. Each tenant has it’s own database.\n2. Semi Isolated Approach: Shared Database, Separate Schemas.\nOne database for all tenants, but one schema per tenant.\n3. Shared Approach: Shared Database, Shared Schema. All tenants share\nthe same database and schema. There is a main tenant-table, where all\nother tables have a foreign key pointing to.\n\nThis application implements the third approach,  which in our opinion,\nis the best solution for a large amount of tenants.\n\nFor more information: [Building Multi Tenant Applications with Django\n](https://books.agiliq.com/projects/django-multi-tenant/en/latest/)\n\nBelow is a demonstration of the features in each approach for an application\nwith 5000 tenants.\n\nApproach       | Number of DB | Number of Schemas | Django migration time | Public access\n-------------- | ------------ | ----------------- | --------------------- | ---------------\nIsolated       | 5000         | 5000              | slow (1/DB)           | No\nSemi Isolated  | 1            | 5000              | slow (1/Schema)       | Yes\nShared         | 1            | 1                 | fast (1)              | Yes\n\n\n## Installation\nAssuming you have django installed, the first step is to install `django-easy-tenants`.\n```bash\npython -m pip install django-easy-tenants\n```\nNow you can import the tenancy module in your Django project.\n\n\n## Setup\nIt is recommended to install this app at the beginning of a project.\nIn an existing project, depending on the structure of the models,\nthe data migration can be hard.\n\nAdd `easy_tenants` to your `INSTALLED_APPS` on `settings.py`.\n\n`settings.py`\n```python\nINSTALLED_APPS = [\n    ...,\n    \'easy_tenants\',\n]\n```\n\nCreate a model which will be the tenant of the application.\n\n`yourapp/models.py`\n```python\nfrom django.db import models\n\nclass Customer(models.Model):\n    ...\n```\n\nYour models, which must have isolated data per tenant, we need to add the foreign field from the Customer model.\nand objects need to be replaced with `TenantManager()`.\n\n\n```python\nfrom django.db import models\nfrom easy_tenants.models import TenantManager\n\nclass Product(models.Model):\n    tenant = models.ForeignKey(Customer, on_delete=models.CASCADE, editable=False)\n    name = models.CharField(max_length=10)\n\n    objects = TenantManager()\n```\n\nIf you prefer you can use `TenantAwareAbstract` to implement the save method for you,\nso when saving an object the tenant will be automatically defined.\n\n```python\nclass Product(TenantAwareAbstract):\n    tenant = models.ForeignKey(Customer, on_delete=models.CASCADE, editable=False)\n    name = models.CharField(max_length=10)\n\n    objects = TenantManager()\n```\n\n\nIf your foreign field has a name other than `tenant` you can change it with a settings. (default is `"tenant"`)\n\n```python\n# models.py\nclass Product(TenantAwareAbstract):\n    customer = models.ForeignKey(Customer, on_delete=models.CASCADE, editable=False)\n    name = models.CharField(max_length=10)\n\n    objects = TenantManager()\n\n# settings.py\nEASY_TENANTS_TENANT_FIELD = "customer"\n```\n\nTo obtain the data for each tenant, it is necessary to define which tenant will be used:\n\n```python\nfrom easy_tenants import tenant_context\n\nwith tenant_context(customer):\n    Product.objects.all()  # filter by customer\n```\n\nTo define the tenant to be used, this will depend on the business rule used. Here is an example for creating middleware that defines a tenant:\n\n```python\nfrom django.http import HttpResponse\nfrom easy_tenants import tenant_context\n\nclass TenantMiddleware:\n    def __init__(self, get_response):\n        self.get_response = get_response\n\n    def __call__(self, request):\n        customer = get_customer_by_request(request)\n\n        if not customer:\n            return HttpResponse("Select tenant")\n\n        with tenant_context(customer):\n            return self.get_response(request)\n```\n\nIf you want to separate the upload files by tenant, you need to change the `DEFAULT_FILE_STORAGE`\nconfiguration (only available for local files).\n\n```python\nDEFAULT_FILE_STORAGE = \'easy_tenants.storage.TenantFileSystemStorage\'\n```\n\n\n## Running the example project\n```bash\npython manage.py migrate\npython manage.py createsuperuser\npython manage.py runserver\n```\nAccess the page `/admin/`, create a `Customer`.\n\n## Motivation\n[django-tenant-schemas](https://github.com/bernardopires/django-tenant-schemas)\n\n[django-tenants](https://github.com/tomturner/django-tenants)\n\n[django-scopes](https://github.com/raphaelm/django-scopes)\n',
-    'author': 'Cleiton Lima',
-    'author_email': 'cleiton.limapin@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/CleitonDeLima/django-easy-tenants',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
 
+This is a Django app for managing multiple tenants on the same project
+instance using a shared approach.
+
+
+## Background
+
+There are typically three solutions for solving the multitenancy problem:
+
+1. Isolated Approach: Separate Databases. Each tenant has it’s own database.
+2. Semi Isolated Approach: Shared Database, Separate Schemas.
+One database for all tenants, but one schema per tenant.
+3. Shared Approach: Shared Database, Shared Schema. All tenants share
+the same database and schema. There is a main tenant-table, where all
+other tables have a foreign key pointing to.
+
+This application implements the third approach,  which in our opinion,
+is the best solution for a large amount of tenants.
+
+For more information: [Building Multi Tenant Applications with Django
+](https://books.agiliq.com/projects/django-multi-tenant/en/latest/)
+
+Below is a demonstration of the features in each approach for an application
+with 5000 tenants.
+
+Approach       | Number of DB | Number of Schemas | Django migration time | Public access
+-------------- | ------------ | ----------------- | --------------------- | ---------------
+Isolated       | 5000         | 5000              | slow (1/DB)           | No
+Semi Isolated  | 1            | 5000              | slow (1/Schema)       | Yes
+Shared         | 1            | 1                 | fast (1)              | Yes
+
+
+## Installation
+Assuming you have django installed, the first step is to install `django-easy-tenants`.
+```bash
+python -m pip install django-easy-tenants
+```
+Now you can import the tenancy module in your Django project.
+
+
+## Setup
+It is recommended to install this app at the beginning of a project.
+In an existing project, depending on the structure of the models,
+the data migration can be hard.
+
+Add `easy_tenants` to your `INSTALLED_APPS` on `settings.py`.
+
+`settings.py`
+```python
+INSTALLED_APPS = [
+    ...,
+    'easy_tenants',
+]
+```
+
+Create a model which will be the tenant of the application.
+
+`yourapp/models.py`
+```python
+from django.db import models
+
+class Customer(models.Model):
+    ...
+```
+
+Your models, which must have isolated data per tenant, we need to add the foreign field from the Customer model.
+and objects need to be replaced with `TenantManager()`.
+
+
+```python
+from django.db import models
+from easy_tenants.models import TenantManager
+
+class Product(models.Model):
+    tenant = models.ForeignKey(Customer, on_delete=models.CASCADE, editable=False)
+    name = models.CharField(max_length=10)
+
+    objects = TenantManager()
+```
+
+If you prefer you can use `TenantAwareAbstract` to implement the save method for you,
+so when saving an object the tenant will be automatically defined.
+
+```python
+class Product(TenantAwareAbstract):
+    tenant = models.ForeignKey(Customer, on_delete=models.CASCADE, editable=False)
+    name = models.CharField(max_length=10)
+
+    objects = TenantManager()
+```
+
+
+If your foreign field has a name other than `tenant` you can change it with a settings. (default is `"tenant"`)
+
+```python
+# models.py
+class Product(TenantAwareAbstract):
+    customer = models.ForeignKey(Customer, on_delete=models.CASCADE, editable=False)
+    name = models.CharField(max_length=10)
+
+    objects = TenantManager()
+
+# settings.py
+EASY_TENANTS_TENANT_FIELD = "customer"
+```
+
+To obtain the data for each tenant, it is necessary to define which tenant will be used:
+
+```python
+from easy_tenants import tenant_context
+
+with tenant_context(customer):
+    Product.objects.all()  # filter by customer
+```
+
+To define the tenant to be used, this will depend on the business rule used. Here is an example for creating middleware that defines a tenant:
+
+```python
+from django.http import HttpResponse
+from easy_tenants import tenant_context
+
+class TenantMiddleware:
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        customer = get_customer_by_request(request)
+
+        if not customer:
+            return HttpResponse("Select tenant")
+
+        with tenant_context(customer):
+            return self.get_response(request)
+```
+
+If you want to separate the upload files by tenant, you need to change the `DEFAULT_FILE_STORAGE`
+configuration (only available for local files).
+
+```python
+DEFAULT_FILE_STORAGE = 'easy_tenants.storage.TenantFileSystemStorage'
+```
+
+
+## Running the example project
+```bash
+python manage.py migrate
+python manage.py createsuperuser
+python manage.py runserver
+```
+Access the page `/admin/`, create a `Customer`.
+
+## Motivation
+[django-tenant-schemas](https://github.com/bernardopires/django-tenant-schemas)
+
+[django-tenants](https://github.com/tomturner/django-tenants)
+
+[django-scopes](https://github.com/raphaelm/django-scopes)
 
-setup(**setup_kwargs)
```

