# Comparing `tmp/baumanecbank_common-1.1.4.tar.gz` & `tmp/baumanecbank_common-1.2.0.tar.gz`

## Comparing `baumanecbank_common-1.1.4.tar` & `baumanecbank_common-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/PKG-INFO
```

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/application.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from telegram.ext._basepersistence import BasePersistence
 from telegram.ext._contexttypes import ContextTypes
 from telegram.ext._updater import Updater
 from telegram.ext._baseupdateprocessor import BaseUpdateProcessor
 
 from baumanecbank_common.postgres import PgCon
 from baumanecbank_common.i18n import I18n
+from baumanecbank_common.log import Log
 
 from telegram import ReplyKeyboardMarkup, ReplyKeyboardRemove
 
 class ApplicationBb(Application):
     def __init__(self, *, bot: Any, update_queue: asyncio.Queue, updater: Updater | None, job_queue: Any, update_processor: BaseUpdateProcessor, persistence: BasePersistence | None, context_types: ContextTypes, post_init: Callable[[Application], Coroutine[Any, Any, None]] | None, post_shutdown: Callable[[Application], Coroutine[Any, Any, None]] | None, post_stop: Callable[[Application], Coroutine[Any, Any, None]] | None):
         super().__init__(bot=bot, update_queue=update_queue, updater=updater, job_queue=job_queue, update_processor=update_processor, persistence=persistence, context_types=context_types, post_init=post_init, post_shutdown=post_shutdown, post_stop=post_stop)
         self.appname: str   = None
@@ -59,14 +60,15 @@
             ret.append(message[:index])
             message = message[index:]
         ret.append(message)
         return ret
 
     def create_update_task(self) -> None:
         if self.update is not None:
+            Log.info("Creating update task")
             self.create_task(
                 self.update(self),
                 {
                     "action": "update task",
                     "appname": self.appname
                 }
             )
```

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/application_create.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/handlers.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/log.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/postgres.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,27 +397,14 @@
             ))
             if cursor.rowcount == 0:
                 return None
             return cursor.fetchall()
     
     @retry(stop=stop_after_attempt(3), wait=wait_exponential())
     @reconnect
-    def get_clients_queue_and_answer(self) -> Any|None:
-        with self._connection.cursor(cursor_factory=psycopg2.extras.NamedTupleCursor) as cursor:
-            cursor.execute((
-                "SELECT * "
-                "FROM queue_client_app "
-                f"WHERE NOT answered"
-            ))
-            if cursor.rowcount == 0:
-                return None
-            return cursor.fetchall()
-    
-    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
-    @reconnect
     def create_deposit_transaction(self, firm_card_code_id: int|str, amount: float) -> None:
         with self._connection.cursor() as cursor:
             cursor.execute((
                 "INSERT INTO transactions"
                 " (source_card_code_id, amount, type)"
                 " VALUES"
                 f" ({firm_card_code_id}, {amount}, '{DEPOSIT}')"
@@ -454,8 +441,46 @@
         with self._connection.cursor() as cursor:
             cursor.execute((
                 "INSERT INTO transactions"
                 " (source_card_code_id, amount, type)"
                 " VALUES"
                 f" ({firm_card_code_id}, {amount}, '{REPAY}')"
             ))
-            Log.info(f"INSERT transaction {REPAY} {firm_card_code_id=} {amount=}")
+            Log.info(f"INSERT transaction {REPAY} {firm_card_code_id=} {amount=}")
+    
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def get_clients_queue_and_answer(self) -> Any|None:
+        with self._connection.cursor(cursor_factory=psycopg2.extras.NamedTupleCursor) as cursor:
+            cursor.execute((
+                "SELECT * "
+                "FROM queue_client_app "
+                f"WHERE NOT answered"
+            ))
+            if cursor.rowcount == 0:
+                return None
+            ans = cursor.fetchall()
+            cursor.execute((
+                "UPDATE queue_client_app "
+                "SET answered = True "
+                f"WHERE id in ({', '.join([str(x.id) for x in ans])})"
+            ))
+            return ans
+    
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def get_firms_queue_and_answer(self) -> Any|None:
+        with self._connection.cursor(cursor_factory=psycopg2.extras.NamedTupleCursor) as cursor:
+            cursor.execute((
+                "SELECT * "
+                "FROM queue_firm_app "
+                f"WHERE NOT answered"
+            ))
+            if cursor.rowcount == 0:
+                return None
+            ans = cursor.fetchall()
+            cursor.execute((
+                "UPDATE queue_firm_app "
+                "SET answered = True "
+                f"WHERE id in ({', '.join([str(x.id) for x in ans])})"
+            ))
+            return ans
```

### Comparing `baumanecbank_common-1.1.4/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.2.0/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/README.md` & `baumanecbank_common-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.4/pyproject.toml` & `baumanecbank_common-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.1.4"
+version = "1.2.0"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `baumanecbank_common-1.1.4/PKG-INFO` & `baumanecbank_common-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.1.4
+Version: 1.2.0
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

