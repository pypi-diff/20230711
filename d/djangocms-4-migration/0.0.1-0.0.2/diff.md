# Comparing `tmp/djangocms-4-migration-0.0.1.tar.gz` & `tmp/djangocms-4-migration-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangocms-4-migration-0.0.1.tar", last modified: Tue Jan 12 15:29:52 2021, max compression
+gzip compressed data, was "djangocms-4-migration-0.0.2.tar", last modified: Tue Jul 11 16:52:09 2023, max compression
```

## Comparing `djangocms-4-migration-0.0.1.tar` & `djangocms-4-migration-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 aiky30     (501) staff       (20)        0 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/
-drwxr-xr-x   0 aiky30     (501) staff       (20)        0 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/
--rw-r--r--   0 aiky30     (501) staff       (20)     3610 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/PKG-INFO
--rw-r--r--   0 aiky30     (501) staff       (20)        1 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/not-zip-safe
--rw-r--r--   0 aiky30     (501) staff       (20)     1239 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/SOURCES.txt
--rw-r--r--   0 aiky30     (501) staff       (20)       22 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/top_level.txt
--rw-r--r--   0 aiky30     (501) staff       (20)        1 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/dependency_links.txt
--rw-r--r--   0 aiky30     (501) staff       (20)     3610 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/PKG-INFO
-drwxr-xr-x   0 aiky30     (501) staff       (20)        0 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/
-drwxr-xr-x   0 aiky30     (501) staff       (20)        0 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/
--rw-r--r--   0 aiky30     (501) staff       (20)     4495 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/0003_page_version_integration_data_migration.py
--rw-r--r--   0 aiky30     (501) staff       (20)        0 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/__init__.py
--rw-r--r--   0 aiky30     (501) staff       (20)     1451 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/0001_initial.py
--rw-r--r--   0 aiky30     (501) staff       (20)     1324 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/0002_collect_removed_data_data_migration.py
--rw-r--r--   0 aiky30     (501) staff       (20)     1176 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/models.py
-drwxr-xr-x   0 aiky30     (501) staff       (20)        0 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/
--rw-r--r--   0 aiky30     (501) staff       (20)        0 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/__init__.py
-drwxr-xr-x   0 aiky30     (501) staff       (20)        0 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/
--rw-r--r--   0 aiky30     (501) staff       (20)      768 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/cms4_migration.py
--rw-r--r--   0 aiky30     (501) staff       (20)        0 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/__init__.py
--rw-r--r--   0 aiky30     (501) staff       (20)     3278 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migration_cleanup.py
--rw-r--r--   0 aiky30     (501) staff       (20)     7783 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migrate_static_placeholders.py
--rw-r--r--   0 aiky30     (501) staff       (20)    11787 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migrate_alias_plugins.py
--rw-r--r--   0 aiky30     (501) staff       (20)      738 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migration_preparation.py
--rw-r--r--   0 aiky30     (501) staff       (20)     1042 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/remove_unlinked_placeholders.py
--rw-r--r--   0 aiky30     (501) staff       (20)       22 2021-01-12 15:26:22.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/__init__.py
--rw-r--r--   0 aiky30     (501) staff       (20)      115 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/apps.py
--rw-r--r--   0 aiky30     (501) staff       (20)       63 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/admin.py
--rw-r--r--   0 aiky30     (501) staff       (20)       60 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/tests.py
--rw-r--r--   0 aiky30     (501) staff       (20)      765 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/helpers.py
--rw-r--r--   0 aiky30     (501) staff       (20)       63 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/djangocms_4_migration/views.py
--rw-r--r--   0 aiky30     (501) staff       (20)     1514 2021-01-08 16:38:30.000000 djangocms-4-migration-0.0.1/LICENSE
--rw-r--r--   0 aiky30     (501) staff       (20)      141 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/MANIFEST.in
--rw-r--r--   0 aiky30     (501) staff       (20)     2621 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/README.md
--rw-r--r--   0 aiky30     (501) staff       (20)      602 2021-01-12 15:24:03.000000 djangocms-4-migration-0.0.1/setup.py
--rw-r--r--   0 aiky30     (501) staff       (20)       38 2021-01-12 15:29:52.000000 djangocms-4-migration-0.0.1/setup.cfg
+drwxrwxr-x   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:52:09.568295 djangocms-4-migration-0.0.2/
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     1514 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/LICENSE
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)      141 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/MANIFEST.in
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     3363 2023-07-11 16:52:09.568295 djangocms-4-migration-0.0.2/PKG-INFO
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     2951 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/README.md
+drwxrwxr-x   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:52:09.560295 djangocms-4-migration-0.0.2/djangocms_4_migration/
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)       22 2023-07-11 16:47:31.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/__init__.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)       63 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/admin.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)      115 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/apps.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)      765 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/helpers.py
+drwxrwxr-x   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:52:09.560295 djangocms-4-migration-0.0.2/djangocms_4_migration/management/
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/__init__.py
+drwxrwxr-x   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:52:09.564295 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/__init__.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)      768 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/cms4_migration.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)    11787 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migrate_alias_plugins.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     7783 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migrate_static_placeholders.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     3278 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migration_cleanup.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)      738 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migration_preparation.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     1042 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/remove_unlinked_placeholders.py
+drwxrwxr-x   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:52:09.568295 djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     1451 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/0001_initial.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     1324 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/0002_collect_removed_data_data_migration.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     4495 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/0003_page_version_integration_data_migration.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/__init__.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     1176 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/models.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)       60 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/tests.py
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)       63 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/djangocms_4_migration/views.py
+drwxrwxr-x   0 aiky30    (1000) aiky30    (1000)        0 2023-07-11 16:52:09.560295 djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     3363 2023-07-11 16:52:09.000000 djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/PKG-INFO
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)     1239 2023-07-11 16:52:09.000000 djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/SOURCES.txt
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)        1 2023-07-11 16:52:09.000000 djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/dependency_links.txt
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)        1 2023-07-11 16:23:43.000000 djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/not-zip-safe
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)       22 2023-07-11 16:52:09.000000 djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/top_level.txt
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)       38 2023-07-11 16:52:09.568295 djangocms-4-migration-0.0.2/setup.cfg
+-rw-rw-r--   0 aiky30    (1000) aiky30    (1000)      662 2023-07-11 16:22:29.000000 djangocms-4-migration-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/PKG-INFO` & `djangocms-4-migration-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 Metadata-Version: 2.1
 Name: djangocms-4-migration
-Version: 0.0.1
+Version: 0.0.2
 Summary: A django CMS 3 to 4 migration package
-Home-page: UNKNOWN
+Home-page: https://github.com/Aiky30/djangocms-4-migration/
 Author: Andrew Aikman (Aiky30)
-License: UNKNOWN
-Description: # django CMS 4 Migration
-        
-        ## When do I need this package?
-        This package is designed to migrate a django CMS 3.5+ project to django CMS 4.0.
-        
-        ## What does this package do?
-        - Keeps any draft and published content, ensuring that any new draft changes are kept as a new draft version in djangocms_versioning. 
-        
-        ## Limitations
-        Due to the nature of the changes between django CMS 3.5+ and 4.0 the package will fail to function if an incompatible package is installed. 
-        
-        This may require you to:
-         - Fork or copy and modify this package to work with any bespoke requirements your project has (we may accept these changes back for popular packages as a configurable option)
-         - Ensure that all installed packages for your project are 
-        
-        ## Prerequisites 
-        Require knowledge of the changes and new features in 4.0:
-        - New cms app configuration
-        - Revised Page, Title (Now named PageContent) and Placeholder relationships
-        
-        Requires knowledge of django CMS Versioning
-        - Grouper and content model terms
-        - Understanding how versioning selects published content
-        
-        ### Install the following packages
-        The following packages are not yet officially released, they need to be installed directly from the repository. We need your help to make packages v4.0 compatible and to provide documentation for the wider community!
-        
-        django CMS 4.0
-        ```
-        pip install http://github.com/divio/django-cms/tarball/release/4.0.x#egg=django-cms
-        ```
-        
-        djangocms-text-ckeditor
-        ```
-        pip install https://github.com/divio/djangocms-text-ckeditor/tarball/support/4.0.x#egg=djangocms-text-ckeditor
-        ```
-        
-        djangocms-versioning
-        ```
-        pip install https://github.com/divio/djangocms-versioning/tarball/master#egg=djangocms-versioning
-        ```
-        
-        djangocms-alias
-        ```
-        pip install https://github.com/divio/djangocms-alias/tarball/master#egg=djangocms-alias
-        ```
-        
-        ## Installation
-        **Warning**: This package can leave your DB in a corrupted state if used incorrectly, be sure to backup any databases prior to running any commands listed here!
-        
-        First install this package in your project
-        ```
-        pip install djangocms-4-migration
-        ```
-        
-        ## Running
-        Simply run the following command to run the data migration. 
-        **Note:** This command calls the django migrate command, this is because it has to run commands that save information that would have been lost by running the cms migrations directly.
-        ```
-        python manage.py cms4_migration
-        ```
-        
-        ## Common solutions for django CMS 4.0 compatibility
-        
-        Import PageContent in a backwards compatible way (Title).
-        ```python
-        
-        # django CMS v4
-        try:
-            from cms.models import PageContent
-        # django CMS 3.x
-        except ImportError:
-            from cms.models import Title as PageContent
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django CMS 4 Migration
+
+**Warning:** If the migration process fails to complete you will not be able to undo the changes without reloading a database backup. We cannot be held accountable for any data loss sustained when running the commands provided in this project. Please keep a database backup before running any commands provided by this package. 
+
+## When do I need this package?
+This package is designed to migrate a django CMS 3.5+ project to django CMS 4.0.
+
+## What does this package do?
+- Keeps any draft and published content, ensuring that any new draft changes are kept as a new draft version in djangocms_versioning. 
+
+## Limitations
+Due to the nature of the changes between django CMS 3.5+ and 4.0 the package will fail to function if an incompatible package is installed. 
+
+This may require you to:
+ - Fork or copy and modify this package to work with any bespoke requirements your project has (we may accept these changes back for popular packages as a configurable option)
+ - Ensure that all installed packages for your project are 
+
+## Prerequisites 
+Require knowledge of the changes and new features in 4.0:
+- New cms app configuration
+- Revised Page, Title (Now named PageContent) and Placeholder relationships
+
+Requires knowledge of django CMS Versioning
+- Grouper and content model terms
+- Understanding how versioning selects published content
+
+### Install the following packages
+The following packages are not yet officially released, they need to be installed directly from the repository. We need your help to make packages v4.0 compatible and to provide documentation for the wider community!
+
+django CMS 4.0
+```
+pip install http://github.com/divio/django-cms/tarball/release/4.0.x#egg=django-cms
+```
+
+djangocms-text-ckeditor
+```
+pip install https://github.com/divio/djangocms-text-ckeditor/tarball/support/4.0.x#egg=djangocms-text-ckeditor
+```
+
+djangocms-versioning
+```
+pip install https://github.com/divio/djangocms-versioning/tarball/master#egg=djangocms-versioning
+```
+
+djangocms-alias
+```
+pip install https://github.com/divio/djangocms-alias/tarball/master#egg=djangocms-alias
+```
+
+## Installation
+**Warning**: This package can leave your DB in a corrupted state if used incorrectly, be sure to backup any databases prior to running any commands listed here!
+
+First install this package in your project
+```
+pip install djangocms-4-migration
+```
+
+## Running
+Simply run the following command to run the data migration. 
+**Note:** This command calls the django migrate command, this is because it has to run commands that save information that would have been lost by running the cms migrations directly.
+```
+python manage.py cms4_migration
+```
+
+## Common solutions for django CMS 4.0 compatibility
+
+Import PageContent in a backwards compatible way (Title).
+```python
+
+# django CMS v4
+try:
+    from cms.models import PageContent
+# django CMS 3.x
+except ImportError:
+    from cms.models import Title as PageContent
+```
```

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration.egg-info/SOURCES.txt` & `djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/PKG-INFO` & `djangocms-4-migration-0.0.2/djangocms_4_migration.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 Metadata-Version: 2.1
 Name: djangocms-4-migration
-Version: 0.0.1
+Version: 0.0.2
 Summary: A django CMS 3 to 4 migration package
-Home-page: UNKNOWN
+Home-page: https://github.com/Aiky30/djangocms-4-migration/
 Author: Andrew Aikman (Aiky30)
-License: UNKNOWN
-Description: # django CMS 4 Migration
-        
-        ## When do I need this package?
-        This package is designed to migrate a django CMS 3.5+ project to django CMS 4.0.
-        
-        ## What does this package do?
-        - Keeps any draft and published content, ensuring that any new draft changes are kept as a new draft version in djangocms_versioning. 
-        
-        ## Limitations
-        Due to the nature of the changes between django CMS 3.5+ and 4.0 the package will fail to function if an incompatible package is installed. 
-        
-        This may require you to:
-         - Fork or copy and modify this package to work with any bespoke requirements your project has (we may accept these changes back for popular packages as a configurable option)
-         - Ensure that all installed packages for your project are 
-        
-        ## Prerequisites 
-        Require knowledge of the changes and new features in 4.0:
-        - New cms app configuration
-        - Revised Page, Title (Now named PageContent) and Placeholder relationships
-        
-        Requires knowledge of django CMS Versioning
-        - Grouper and content model terms
-        - Understanding how versioning selects published content
-        
-        ### Install the following packages
-        The following packages are not yet officially released, they need to be installed directly from the repository. We need your help to make packages v4.0 compatible and to provide documentation for the wider community!
-        
-        django CMS 4.0
-        ```
-        pip install http://github.com/divio/django-cms/tarball/release/4.0.x#egg=django-cms
-        ```
-        
-        djangocms-text-ckeditor
-        ```
-        pip install https://github.com/divio/djangocms-text-ckeditor/tarball/support/4.0.x#egg=djangocms-text-ckeditor
-        ```
-        
-        djangocms-versioning
-        ```
-        pip install https://github.com/divio/djangocms-versioning/tarball/master#egg=djangocms-versioning
-        ```
-        
-        djangocms-alias
-        ```
-        pip install https://github.com/divio/djangocms-alias/tarball/master#egg=djangocms-alias
-        ```
-        
-        ## Installation
-        **Warning**: This package can leave your DB in a corrupted state if used incorrectly, be sure to backup any databases prior to running any commands listed here!
-        
-        First install this package in your project
-        ```
-        pip install djangocms-4-migration
-        ```
-        
-        ## Running
-        Simply run the following command to run the data migration. 
-        **Note:** This command calls the django migrate command, this is because it has to run commands that save information that would have been lost by running the cms migrations directly.
-        ```
-        python manage.py cms4_migration
-        ```
-        
-        ## Common solutions for django CMS 4.0 compatibility
-        
-        Import PageContent in a backwards compatible way (Title).
-        ```python
-        
-        # django CMS v4
-        try:
-            from cms.models import PageContent
-        # django CMS 3.x
-        except ImportError:
-            from cms.models import Title as PageContent
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django CMS 4 Migration
+
+**Warning:** If the migration process fails to complete you will not be able to undo the changes without reloading a database backup. We cannot be held accountable for any data loss sustained when running the commands provided in this project. Please keep a database backup before running any commands provided by this package. 
+
+## When do I need this package?
+This package is designed to migrate a django CMS 3.5+ project to django CMS 4.0.
+
+## What does this package do?
+- Keeps any draft and published content, ensuring that any new draft changes are kept as a new draft version in djangocms_versioning. 
+
+## Limitations
+Due to the nature of the changes between django CMS 3.5+ and 4.0 the package will fail to function if an incompatible package is installed. 
+
+This may require you to:
+ - Fork or copy and modify this package to work with any bespoke requirements your project has (we may accept these changes back for popular packages as a configurable option)
+ - Ensure that all installed packages for your project are 
+
+## Prerequisites 
+Require knowledge of the changes and new features in 4.0:
+- New cms app configuration
+- Revised Page, Title (Now named PageContent) and Placeholder relationships
+
+Requires knowledge of django CMS Versioning
+- Grouper and content model terms
+- Understanding how versioning selects published content
+
+### Install the following packages
+The following packages are not yet officially released, they need to be installed directly from the repository. We need your help to make packages v4.0 compatible and to provide documentation for the wider community!
+
+django CMS 4.0
+```
+pip install http://github.com/divio/django-cms/tarball/release/4.0.x#egg=django-cms
+```
+
+djangocms-text-ckeditor
+```
+pip install https://github.com/divio/djangocms-text-ckeditor/tarball/support/4.0.x#egg=djangocms-text-ckeditor
+```
+
+djangocms-versioning
+```
+pip install https://github.com/divio/djangocms-versioning/tarball/master#egg=djangocms-versioning
+```
+
+djangocms-alias
+```
+pip install https://github.com/divio/djangocms-alias/tarball/master#egg=djangocms-alias
+```
+
+## Installation
+**Warning**: This package can leave your DB in a corrupted state if used incorrectly, be sure to backup any databases prior to running any commands listed here!
+
+First install this package in your project
+```
+pip install djangocms-4-migration
+```
+
+## Running
+Simply run the following command to run the data migration. 
+**Note:** This command calls the django migrate command, this is because it has to run commands that save information that would have been lost by running the cms migrations directly.
+```
+python manage.py cms4_migration
+```
+
+## Common solutions for django CMS 4.0 compatibility
+
+Import PageContent in a backwards compatible way (Title).
+```python
+
+# django CMS v4
+try:
+    from cms.models import PageContent
+# django CMS 3.x
+except ImportError:
+    from cms.models import Title as PageContent
+```
```

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/0003_page_version_integration_data_migration.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/0003_page_version_integration_data_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/0001_initial.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/migrations/0002_collect_removed_data_data_migration.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/migrations/0002_collect_removed_data_data_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/models.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/cms4_migration.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/cms4_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migration_cleanup.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migration_cleanup.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migrate_static_placeholders.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migrate_static_placeholders.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migrate_alias_plugins.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migrate_alias_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/migration_preparation.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/migration_preparation.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/management/commands/remove_unlinked_placeholders.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/management/commands/remove_unlinked_placeholders.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/djangocms_4_migration/helpers.py` & `djangocms-4-migration-0.0.2/djangocms_4_migration/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/LICENSE` & `djangocms-4-migration-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-4-migration-0.0.1/README.md` & `djangocms-4-migration-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # django CMS 4 Migration
 
+**Warning:** If the migration process fails to complete you will not be able to undo the changes without reloading a database backup. We cannot be held accountable for any data loss sustained when running the commands provided in this project. Please keep a database backup before running any commands provided by this package. 
+
 ## When do I need this package?
 This package is designed to migrate a django CMS 3.5+ project to django CMS 4.0.
 
 ## What does this package do?
 - Keeps any draft and published content, ensuring that any new draft changes are kept as a new draft version in djangocms_versioning. 
 
 ## Limitations
```

### Comparing `djangocms-4-migration-0.0.1/setup.py` & `djangocms-4-migration-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from djangocms_4_migration import __version__
 
 
 setup(
     name='djangocms-4-migration',
     version=__version__,
     author="Andrew Aikman (Aiky30)",
+    url='https://github.com/Aiky30/djangocms-4-migration/',
     description="A django CMS 3 to 4 migration package",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
```

