# Comparing `tmp/baumanecbank_common-1.0.6.tar.gz` & `tmp/baumanecbank_common-1.1.0.tar.gz`

## Comparing `baumanecbank_common-1.0.6.tar` & `baumanecbank_common-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0    12581 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.0/PKG-INFO
```

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/application.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/application.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/application_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
 APP_NAME = 'APP_NAME'
 
 def ApplicationBbCreate(initialize_my_commands_from_an_app: bool = False) -> ApplicationBb:
     appname = os.environ.get(APP_NAME, 'app')
     pgcon   = PgCon(appname)
     i18n    = I18n(appname)
-    token   = pgcon.get_telegram_token()
+    pgcon.connect()
+    token = pgcon.get_telegram_token()
     app: ApplicationBb = ApplicationBuilder() \
         .application_class(ApplicationBb) \
         .token(token) \
         .post_init(post_init_std_my_commands if not initialize_my_commands_from_an_app else post_init_app_my_commands) \
         .post_shutdown(post_shutdown) \
         .build()
     app.appname = appname
```

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/handlers.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/log.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.1.0/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/README.md` & `baumanecbank_common-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.6/pyproject.toml` & `baumanecbank_common-1.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.0.6"
+version = "1.1.0"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -18,13 +18,14 @@
 ]
 dependencies = [
   'python-telegram-bot==20.4',
   'psycopg2-binary',
   'python-dotenv',
   'pyzbar',
   'Pillow',
-  'pyyaml'
+  'pyyaml',
+  'tenacity'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/twobrowin-study/baumanec-bank"
 "Bug Tracker" = "https://github.com/twobrowin-study/baumanec-bank/issues"
```

### Comparing `baumanecbank_common-1.0.6/PKG-INFO` & `baumanecbank_common-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.0.6
+Version: 1.1.0
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: pillow
 Requires-Dist: psycopg2-binary
 Requires-Dist: python-dotenv
 Requires-Dist: python-telegram-bot==20.4
 Requires-Dist: pyyaml
 Requires-Dist: pyzbar
+Requires-Dist: tenacity
 Description-Content-Type: text/markdown
 
 # Пакет основных функций для ботов БауБанка
 
 Для работы требуются пременные окружения:
 
 * `PG_HOST` - значение по-умолчанию `localhost`
```

