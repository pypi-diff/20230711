# Comparing `tmp/djangorestframework_emailuser-0.2.1.dev0.tar.gz` & `tmp/djangorestframework_emailuser-0.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djangorestframework_emailuser-0.2.1.dev0.tar", last modified: Tue Dec 24 01:19:23 2019, max compression
+gzip compressed data, was "djangorestframework_emailuser-0.3.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `djangorestframework_emailuser-0.2.1.dev0.tar` & `djangorestframework_emailuser-0.3.0.dev0.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxrwxrwx   0        0        0        0 2019-12-24 01:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/
--rw-rw-rw-   0        0        0     1085 2019-07-31 04:07:22.000000 djangorestframework_emailuser-0.2.1.dev0/LICENSE
--rw-rw-rw-   0        0        0       91 2019-08-14 17:15:26.000000 djangorestframework_emailuser-0.2.1.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     5659 2019-12-24 01:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     3460 2019-12-24 01:18:17.000000 djangorestframework_emailuser-0.2.1.dev0/README.rst
-drwxrwxrwx   0        0        0        0 2019-12-24 01:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/djangorestframework_emailuser.egg-info/
--rw-rw-rw-   0        0        0     5659 2019-12-24 01:19:22.000000 djangorestframework_emailuser-0.2.1.dev0/djangorestframework_emailuser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2019-12-24 01:19:22.000000 djangorestframework_emailuser-0.2.1.dev0/djangorestframework_emailuser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-12-24 01:19:22.000000 djangorestframework_emailuser-0.2.1.dev0/djangorestframework_emailuser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2019-12-24 01:19:22.000000 djangorestframework_emailuser-0.2.1.dev0/djangorestframework_emailuser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-12-24 01:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/
--rw-rw-rw-   0        0        0       53 2019-08-25 23:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/__init__.py
--rw-rw-rw-   0        0        0      924 2019-07-23 13:31:23.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/admin.py
--rw-rw-rw-   0        0        0       98 2019-08-25 21:55:42.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/apps.py
--rw-rw-rw-   0        0        0      381 2019-07-23 03:33:07.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/forms.py
--rw-rw-rw-   0        0        0     1017 2019-08-12 13:40:47.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/managers.py
-drwxrwxrwx   0        0        0        0 2019-12-24 01:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/migrations/
--rw-rw-rw-   0        0        0     1752 2019-12-24 00:45:12.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2019-12-24 00:45:12.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/migrations/__init__.py
--rw-rw-rw-   0        0        0      767 2019-07-23 12:56:43.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/models.py
--rw-rw-rw-   0        0        0      400 2019-07-26 00:18:10.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/permissions.py
--rw-rw-rw-   0        0        0      970 2019-08-12 13:40:47.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/serializers.py
--rw-rw-rw-   0        0        0      388 2019-08-16 22:18:29.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/urls.py
--rw-rw-rw-   0        0        0      637 2019-07-30 03:19:11.000000 djangorestframework_emailuser-0.2.1.dev0/emailuser/views.py
--rw-rw-rw-   0        0        0       42 2019-12-24 01:19:23.000000 djangorestframework_emailuser-0.2.1.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1391 2019-12-24 01:18:21.000000 djangorestframework_emailuser-0.2.1.dev0/setup.py
+-rw-r--r--   0        0        0     1064 2023-07-10 10:50:28.322536 djangorestframework_emailuser-0.3.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3378 2023-07-10 20:08:21.978863 djangorestframework_emailuser-0.3.0.dev0/README.rst
+-rw-r--r--   0        0        0     2192 2023-07-10 10:50:28.322536 djangorestframework_emailuser-0.3.0.dev0/conftest.py
+-rw-r--r--   0        0        0      346 2023-07-10 14:41:28.750659 djangorestframework_emailuser-0.3.0.dev0/migrations_script.py
+-rw-r--r--   0        0        0     1610 2023-07-10 21:26:02.038436 djangorestframework_emailuser-0.3.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1352 2023-07-10 19:40:52.799011 djangorestframework_emailuser-0.3.0.dev0/setup.py
+-rw-r--r--   0        0        0       80 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/__init__.py
+-rw-r--r--   0        0        0      961 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/admin.py
+-rw-r--r--   0        0        0       93 2023-07-10 17:39:40.739671 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/apps.py
+-rw-r--r--   0        0        0      398 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/forms.py
+-rw-r--r--   0        0        0      984 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/managers.py
+-rw-r--r--   0        0        0     1719 2023-07-10 17:39:40.739671 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:39:40.739671 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/migrations/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-10 20:08:21.978863 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/models.py
+-rw-r--r--   0        0        0      395 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/permissions.py
+-rw-r--r--   0        0        0      935 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/serializers.py
+-rw-r--r--   0        0        0      407 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/urls.py
+-rw-r--r--   0        0        0      580 2023-07-10 21:19:15.378476 djangorestframework_emailuser-0.3.0.dev0/src/emailuser/views.py
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 djangorestframework_emailuser-0.3.0.dev0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangorestframework_emailuser-0.2.1.dev0/README.rst` & `djangorestframework_emailuser-0.3.0.dev0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-djangorestframework_emailuser
-=============================
-
-.. image:: https://travis-ci.org/simlist/django-rest-framework-emailuser.svg?branch=master
-    :target: https://travis-ci.org/simlist/django-rest-framework-emailuser
-
-.. image:: https://coveralls.io/repos/github/simlist/django-rest-framework-emailuser/badge.svg?branch=master
-    :target: https://coveralls.io/github/simlist/django-rest-framework-emailuser?branch=master
-
-Overview
---------
-
-A user for djangorestframework that uses an email as the username.
-
-Features
---------
-
-* Use email as username for loging in
-* One name field instead of first name and last name
-* Endpoints for creating an account, viewing, and updating accounts
-* Django admin to work with EmailUser model.
-
-Requirements
-------------
-
-- Python 3.5+
-- Django 2.2+
-- Djangorestframework 3.10+
-
-Installation and Configuration
-------------------------------
-
-Install using ``pip``:
-
-.. code-block:: sh
-
-  $ pip install djangorestframework_emailuser
-
-Add ``'emailuser'`` to ``INSTALLED_APPS``:
-
-.. code-block:: Python
-
-  # mysite/settings.py
-  INSTALLED_APPS = [
-      ...
-      'emailuser',
-  ]
-
-Add the following line to ``settings.py`` to override django's default User
-model with the 'EmailUser' model:
-
-.. code-block:: Python
-
-  # mysite/settings.py
-  AUTH_USER_MODEL = 'emailuser.EmailUser'
-
-Add urls to url conf:
-
-.. code-block:: Python
-
-  # mysite/urls.py
-  from django.urls import path, include
-  urlpatterns = [
-    ...
-    path('accounts/', include('emailuser.urls')),
-  ]
-
-Using
------
-To create a user programatically:
-
-.. code-block:: Python
-
-  from django.contrib.auth import get_user_model
-
-  normal_user = get_user_model().objects.create_user(
-      email='me@example.com',
-      name='My Name',
-      password='MyPassword'
-  )
-
-  superuser = get_user_model().objects.create_superuser(
-      email='admin@example.com',
-      name='Super Name',
-      password='MySuperPassword'
-  )
-
-Using Endpoints:
-~~~~~~~~~~~~~~~~
-Assuming emailuser urls were set to ``/accounts/``:
-
-Creating user
-?????????????
-``POST`` ``{"email": email, "name": name, "password": password}``
-to ``/accounts/users/register``
-
-Updating User
-?????????????
-``PUT`` ``{"email": email, "name": name, "password": password}``
-to ``/accounts/users/<int:pk>/``
-or
-``PATCH`` the attribute you want to change
-to ``/accounts/users/<int:pk>/``
-
-Referencing User
-????????????????
-To reference user object in your code as a string (As for foreign keys):
-
-.. code-block:: Python
-
-  from django.conf import settings
-
-  user_model = settings.AUTH_USER_MODEL
-
-To reference the user class directly:
-
-.. code-block:: Python
-
-  from django.contrib.auth import get_user_model
-
-  user_model = get_user_model()
-
-See `Django docs <https://docs.djangoproject.com/en/2.2/topics/auth/customizing/#referencing-the-user-model>`_  for more details.
-
-Attributes
-~~~~~~~~~~
-The EmailUser model has the following attributes:
-
-email
-  The email address used as the login username.
-
-name
-    A single field for the name of the user.
-password
-  The password is hashed as set by the django settings.
-
-is_superuser
-  A boolean attribute that can only be set programatically.
-
-is_staff
-  A boolean attribute that can be set by the admin site or
-  programatically.
-
-EmailUser also subclasses ``django.contrib.auth.models.PermissionsMixin``.
+djangorestframework_emailuser
+=============================
+
+.. image:: https://github.com/simlist/django-rest-framework-emailuser/actions/workflows/testing-and-coverage.yml/badge.svg?branch=master
+    :target: https://github.com/simlist/pyluach/actions/workflows/testing-and-coverage.yml
+
+.. image:: https://coveralls.io/repos/github/simlist/django-rest-framework-emailuser/badge.svg?branch=master
+    :target: https://coveralls.io/github/simlist/django-rest-framework-emailuser?branch=master
+
+Overview
+--------
+
+A user for djangorestframework that uses an email as the username.
+
+Features
+--------
+
+* Use email as username for loging in
+* One name field instead of first name and last name
+* Endpoints for creating an account, viewing, and updating accounts
+* Django admin to work with EmailUser model.
+
+Requirements
+------------
+
+- Python 3.5+
+- Django 2.2+
+- Djangorestframework 3.10+
+
+Installation and Configuration
+------------------------------
+
+Install using ``pip``:
+
+.. code-block:: sh
+
+  $ pip install djangorestframework_emailuser
+
+Add ``'emailuser'`` to ``INSTALLED_APPS``:
+
+.. code-block:: Python
+
+  # mysite/settings.py
+  INSTALLED_APPS = [
+      ...
+      'emailuser',
+  ]
+
+Add the following line to ``settings.py`` to override django's default User
+model with the 'EmailUser' model:
+
+.. code-block:: Python
+
+  # mysite/settings.py
+  AUTH_USER_MODEL = 'emailuser.EmailUser'
+
+Add urls to url conf:
+
+.. code-block:: Python
+
+  # mysite/urls.py
+  from django.urls import path, include
+  urlpatterns = [
+    ...
+    path('accounts/', include('emailuser.urls')),
+  ]
+
+Using
+-----
+To create a user programatically:
+
+.. code-block:: Python
+
+  from django.contrib.auth import get_user_model
+
+  normal_user = get_user_model().objects.create_user(
+      email='me@example.com',
+      name='My Name',
+      password='MyPassword'
+  )
+
+  superuser = get_user_model().objects.create_superuser(
+      email='admin@example.com',
+      name='Super Name',
+      password='MySuperPassword'
+  )
+
+Using Endpoints:
+~~~~~~~~~~~~~~~~
+Assuming emailuser urls were set to ``/accounts/``:
+
+Creating user
+?????????????
+``POST`` ``{"email": email, "name": name, "password": password}``
+to ``/accounts/users/register``
+
+Updating User
+?????????????
+``PUT`` ``{"email": email, "name": name, "password": password}``
+to ``/accounts/users/<int:pk>/``
+or
+``PATCH`` the attribute you want to change
+to ``/accounts/users/<int:pk>/``
+
+Referencing User
+????????????????
+To reference user object in your code as a string (As for foreign keys):
+
+.. code-block:: Python
+
+  from django.conf import settings
+
+  user_model = settings.AUTH_USER_MODEL
+
+To reference the user class directly:
+
+.. code-block:: Python
+
+  from django.contrib.auth import get_user_model
+
+  user_model = get_user_model()
+
+See `Django docs <https://docs.djangoproject.com/en/2.2/topics/auth/customizing/#referencing-the-user-model>`_  for more details.
+
+Attributes
+~~~~~~~~~~
+The EmailUser model has the following attributes:
+
+email
+  The email address used as the login username.
+
+name
+    A single field for the name of the user.
+password
+  The password is hashed as set by the django settings.
+
+is_superuser
+  A boolean attribute that can only be set programatically.
+
+is_staff
+  A boolean attribute that can be set by the admin site or
+  programatically.
+
+EmailUser also subclasses ``django.contrib.auth.models.PermissionsMixin``.
```

### Comparing `djangorestframework_emailuser-0.2.1.dev0/emailuser/admin.py` & `djangorestframework_emailuser-0.3.0.dev0/src/emailuser/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from django.contrib import admin
-from django.contrib.auth.admin import UserAdmin
-
-from .forms import EmailUserCreationForm, EmailUserChangeForm
-from .models import EmailUser
-
-
-class EmailUserAdmin(UserAdmin):
-    add_form = EmailUserCreationForm
-    form = EmailUserChangeForm
-    model = EmailUser
-    list_display = ('email', 'name', 'is_staff', 'is_active')
-    list_filter = ('email', 'name', 'is_staff', 'is_active')
-    fieldsets = (
-        (None, {'fields': ('email', 'name', 'password')}),
-        ('Permissions', {'fields': ('is_staff', 'is_active', 'groups')}),
-    )
-    add_fieldsets = (
-        (None, {
-            'classes': ('wide',),
-            'fields': ('email', 'name', 'password1', 
-                       'password2', 'is_staff', 'is_active')
-        }),
-    )
-    search_fields = ('email', 'name')
-    ordering = ('name',)
-
-admin.site.register(EmailUser, EmailUserAdmin)
+from django.contrib import admin
+from django.contrib.auth.admin import UserAdmin
+
+from .forms import EmailUserCreationForm, EmailUserChangeForm
+from .models import EmailUser
+
+
+class EmailUserAdmin(UserAdmin):
+    add_form = EmailUserCreationForm
+    form = EmailUserChangeForm
+    list_display = ('email', 'name', 'is_staff', 'is_active')
+    list_filter = ('email', 'name', 'is_staff', 'is_active')
+    fieldsets = (
+        (None, {'fields': ('email', 'name', 'password')}),
+        ('Permissions', {'fields': ('is_staff', 'is_active', 'groups')}),
+    )
+    add_fieldsets = (
+        (None, {
+            'classes': ('wide',),
+            'fields': (
+                'email',
+                'name',
+                'password1',
+                'password2',
+                'is_staff',
+                'is_active'
+            )
+        }),
+    )
+    search_fields = ('email', 'name')
+    ordering = ('name',)
+
+
+admin.site.register(EmailUser, EmailUserAdmin)
```

### Comparing `djangorestframework_emailuser-0.2.1.dev0/emailuser/managers.py` & `djangorestframework_emailuser-0.3.0.dev0/src/emailuser/managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from django.contrib.auth.base_user import BaseUserManager
-
-
-class EmailUserManager(BaseUserManager):
-
-    def create_user(self, name, email, password=None):
-        if not name:
-            raise ValueError('Users must have a name.')
-        if not email:
-            raise ValueError('User must have an email.')
-        user = self.model(name=name, email=self.normalize_email(email.lower()))
-        user.set_password(password)
-        user.save(using=self._db)
-        return user
-    
-    def create_superuser(self, name, email, password):
-        if not password:
-            raise ValueError('Superusers must have a password.')
-        user = self.create_user(name, email, password=password)
-        user.is_superuser = True
-        user.is_staff = True
-        user.save(using=self._db)
-        return user
-    
-    def get_by_natural_key(self, username):
-        case_insensitive = '{}__iexact'.format(self.model.USERNAME_FIELD)
-        return self.get(**{case_insensitive: username})
+from django.contrib.auth.base_user import BaseUserManager
+
+
+class EmailUserManager(BaseUserManager):
+
+    def create_user(self, name, email, password=None):
+        if not name:
+            raise ValueError('Users must have a name.')
+        if not email:
+            raise ValueError('User must have an email.')
+        user = self.model(name=name, email=self.normalize_email(email.lower()))
+        user.set_password(password)
+        user.save(using=self._db)
+        return user
+
+    def create_superuser(self, name, email, password):
+        if not password:
+            raise ValueError('Superusers must have a password.')
+        user = self.create_user(name, email, password=password)
+        user.is_superuser = True
+        user.is_staff = True
+        user.save(using=self._db)
+        return user
+
+    def get_by_natural_key(self, username):
+        case_insensitive = '{}__iexact'.format(self.model.USERNAME_FIELD)
+        return self.get(**{case_insensitive: username})
```

### Comparing `djangorestframework_emailuser-0.2.1.dev0/emailuser/migrations/0001_initial.py` & `djangorestframework_emailuser-0.3.0.dev0/src/emailuser/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Generated by Django 2.2.4 on 2019-12-23 18:50
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('auth', '0011_update_proxy_permissions'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='EmailUser',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('password', models.CharField(max_length=128, verbose_name='password')),
-                ('last_login', models.DateTimeField(blank=True, null=True, verbose_name='last login')),
-                ('is_superuser', models.BooleanField(default=False, help_text='Designates that this user has all permissions without explicitly assigning them.', verbose_name='superuser status')),
-                ('email', models.EmailField(db_index=True, max_length=60, unique=True)),
-                ('name', models.CharField(max_length=40)),
-                ('is_active', models.BooleanField(default=True)),
-                ('is_staff', models.BooleanField(default=False)),
-                ('groups', models.ManyToManyField(blank=True, help_text='The groups this user belongs to. A user will get all permissions granted to each of their groups.', related_name='user_set', related_query_name='user', to='auth.Group', verbose_name='groups')),
-                ('user_permissions', models.ManyToManyField(blank=True, help_text='Specific permissions for this user.', related_name='user_set', related_query_name='user', to='auth.Permission', verbose_name='user permissions')),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 2.2.4 on 2019-12-23 18:50
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('auth', '0011_update_proxy_permissions'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='EmailUser',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('password', models.CharField(max_length=128, verbose_name='password')),
+                ('last_login', models.DateTimeField(blank=True, null=True, verbose_name='last login')),
+                ('is_superuser', models.BooleanField(default=False, help_text='Designates that this user has all permissions without explicitly assigning them.', verbose_name='superuser status')),
+                ('email', models.EmailField(db_index=True, max_length=60, unique=True)),
+                ('name', models.CharField(max_length=40)),
+                ('is_active', models.BooleanField(default=True)),
+                ('is_staff', models.BooleanField(default=False)),
+                ('groups', models.ManyToManyField(blank=True, help_text='The groups this user belongs to. A user will get all permissions granted to each of their groups.', related_name='user_set', related_query_name='user', to='auth.Group', verbose_name='groups')),
+                ('user_permissions', models.ManyToManyField(blank=True, help_text='Specific permissions for this user.', related_name='user_set', related_query_name='user', to='auth.Permission', verbose_name='user permissions')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `djangorestframework_emailuser-0.2.1.dev0/setup.py` & `djangorestframework_emailuser-0.3.0.dev0/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from setuptools import setup, find_packages
-from os import path
-from os.path import abspath
-
-with open(path.join(abspath(path.dirname(__file__)), 'README.rst')) as f:
-    long_description = f.read()
-
-setup(
-    name='djangorestframework_emailuser',
-    version='0.2.1dev0',
-    author='MS List',
-    author_email='simlist@gmail.com',
-    packages=find_packages(),
-    url='https://github.com/simlist/django-rest-framework-emailuser',
-    license='MIT',
-    description=(
-        'A user for djangorestframework that uses an email as the username.'
-    ),
-    long_description=long_description,
-    long_description_content_type='text/x-rst',
-    install_requires=[],
-    python_requires='>=3.5',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Natural Language :: English',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3 :: Only',
-        'Topic :: Internet :: WWW/HTTP',
-    ]
-)
+from setuptools import setup, find_packages
+from os import path
+from os.path import abspath
+
+with open(path.join(abspath(path.dirname(__file__)), 'README.rst')) as f:
+    long_description = f.read()
+
+setup(
+    name='djangorestframework_emailuser',
+    version='0.2.1dev0',
+    author='MS List',
+    author_email='simlist@gmail.com',
+    packages=find_packages(),
+    url='https://github.com/simlist/django-rest-framework-emailuser',
+    license='MIT',
+    description=(
+        'A user for djangorestframework that uses an email as the username.'
+    ),
+    long_description=long_description,
+    long_description_content_type='text/x-rst',
+    install_requires=[],
+    python_requires='>=3.5',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Environment :: Web Environment',
+        'Framework :: Django',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Natural Language :: English',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3 :: Only',
+        'Topic :: Internet :: WWW/HTTP',
+    ]
+)
```

