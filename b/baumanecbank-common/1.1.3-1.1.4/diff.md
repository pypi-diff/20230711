# Comparing `tmp/baumanecbank_common-1.1.3.tar.gz` & `tmp/baumanecbank_common-1.1.4.tar.gz`

## Comparing `baumanecbank_common-1.1.3.tar` & `baumanecbank_common-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0    15479 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.1.4/PKG-INFO
```

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/application.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class ApplicationBb(Application):
     def __init__(self, *, bot: Any, update_queue: asyncio.Queue, updater: Updater | None, job_queue: Any, update_processor: BaseUpdateProcessor, persistence: BasePersistence | None, context_types: ContextTypes, post_init: Callable[[Application], Coroutine[Any, Any, None]] | None, post_shutdown: Callable[[Application], Coroutine[Any, Any, None]] | None, post_stop: Callable[[Application], Coroutine[Any, Any, None]] | None):
         super().__init__(bot=bot, update_queue=update_queue, updater=updater, job_queue=job_queue, update_processor=update_processor, persistence=persistence, context_types=context_types, post_init=post_init, post_shutdown=post_shutdown, post_stop=post_stop)
         self.appname: str   = None
         self.pgcon:   PgCon = None
         self.i18n:    I18n  = None
+        self.update:  Callable[[ApplicationBb], Coroutine[Any, Any, None]] = None
 
         self.reply_keyboard_keys = []
         self.reply_keyboard      = ReplyKeyboardRemove()
     
     def init_keyboard(self, from_config: str = 'keyboard', attr_name: str = 'reply_keyboard') -> None:
         keyboard_keys = [
             val for _,val in self.i18n.app[from_config].items()
@@ -54,8 +55,18 @@
             return [message]
         ret = []
         while len(message) > max_len:
             index = message[:max_len].rfind(delimeter)
             ret.append(message[:index])
             message = message[index:]
         ret.append(message)
-        return ret
+        return ret
+
+    def create_update_task(self) -> None:
+        if self.update is not None:
+            self.create_task(
+                self.update(self),
+                {
+                    "action": "update task",
+                    "appname": self.appname
+                }
+            )
```

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/application_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,45 +9,51 @@
 from baumanecbank_common.postgres import PgCon
 from baumanecbank_common.i18n import I18n
 
 from baumanecbank_common.handlers import (
     ErrorHandlerFun, ChatMemberHandlerFun
 )
 
+from typing import Any, Callable, Coroutine
+
 async def default_post_init(app: ApplicationBb, my_commands: list[dict]) -> None:
     app.pgcon.write_event("Starting an application")
     bot: Bot = app.bot
     await bot.set_my_commands([
         (k, v)
         for command in my_commands
         for k,v in command.items()
     ])
 
+    if app.update is not None:
+        app.create_update_task()
+
 async def post_init_std_my_commands(app: ApplicationBb) -> None:
     await default_post_init(app, app.i18n.pure['my_commands'])
 
 async def post_init_app_my_commands(app: ApplicationBb) -> None:
     await default_post_init(app, app.i18n.app['my_commands'])
 
 async def post_shutdown(app: ApplicationBb) -> None:
     app.pgcon.write_event("Stopping an application")
 
 APP_NAME = 'APP_NAME'
 
-def ApplicationBbCreate(initialize_my_commands_from_an_app: bool = False) -> ApplicationBb:
+def ApplicationBbCreate(initialize_my_commands_from_an_app: bool = False, update_task: Callable[[ApplicationBb], Coroutine[Any, Any, None]] = None) -> ApplicationBb:
     appname = os.environ.get(APP_NAME, 'app')
     pgcon   = PgCon(appname)
     i18n    = I18n(appname)
     pgcon.connect()
     token = pgcon.get_telegram_token()
     app: ApplicationBb = ApplicationBuilder() \
         .application_class(ApplicationBb) \
         .token(token) \
         .post_init(post_init_std_my_commands if not initialize_my_commands_from_an_app else post_init_app_my_commands) \
         .post_shutdown(post_shutdown) \
         .build()
     app.appname = appname
     app.pgcon   = pgcon
     app.i18n    = i18n
+    app.update  = update_task
     app.add_error_handler(ErrorHandlerFun, block=False)
     app.add_handler(ChatMemberHandler(ChatMemberHandlerFun, chat_member_types=ChatMemberHandler.MY_CHAT_MEMBER, block=False))
     return app
```

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/handlers.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/log.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/postgres.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 PG_CONN = 'PG_CONN'
 TZ      = 'TZ'
 
 PURCHASE = 'purchase'
 SALARY   = 'salary'
 SERVICE  = 'service'
 MANUAL   = 'manual'
+DEPOSIT  = 'deposit'
+WITHDRAW = 'withdraw'
+LOAN     = 'loan'
+REPAY    = 'repay'
 
 class PgTelegramTokenManyOrMissing(Exception):
     pass
 
 class PgConAbstract(AbstractBbClass):
     def __init__(self, appname: str) -> None:
         super().__init__(appname)
@@ -389,8 +393,69 @@
             cursor.execute((
                 "SELECT * "
                 "FROM operations_clients_firms_taxes "
                 f"WHERE uuid = '{uuid}'"
             ))
             if cursor.rowcount == 0:
                 return None
-            return cursor.fetchall()
+            return cursor.fetchall()
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
+            return cursor.fetchall()
+    
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def create_deposit_transaction(self, firm_card_code_id: int|str, amount: float) -> None:
+        with self._connection.cursor() as cursor:
+            cursor.execute((
+                "INSERT INTO transactions"
+                " (source_card_code_id, amount, type)"
+                " VALUES"
+                f" ({firm_card_code_id}, {amount}, '{DEPOSIT}')"
+            ))
+            Log.info(f"INSERT transaction {DEPOSIT} {firm_card_code_id=} {amount=}")
+    
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def create_withdraw_transaction(self, firm_card_code_id: int|str, amount: float) -> None:
+        with self._connection.cursor() as cursor:
+            cursor.execute((
+                "INSERT INTO transactions"
+                " (recipient_card_code_id, amount, type)"
+                " VALUES"
+                f" ({firm_card_code_id}, {amount}, '{WITHDRAW}')"
+            ))
+            Log.info(f"INSERT transaction {WITHDRAW} {firm_card_code_id=} {amount=}")
+    
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def create_loan_transaction(self, firm_card_code_id: int|str, amount: float) -> None:
+        with self._connection.cursor() as cursor:
+            cursor.execute((
+                "INSERT INTO transactions"
+                " (recipient_card_code_id, amount, type)"
+                " VALUES"
+                f" ({firm_card_code_id}, {amount}, '{LOAN}')"
+            ))
+            Log.info(f"INSERT transaction {LOAN} {firm_card_code_id=} {amount=}")
+    
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def create_repay_transaction(self, firm_card_code_id: int|str, amount: float) -> None:
+        with self._connection.cursor() as cursor:
+            cursor.execute((
+                "INSERT INTO transactions"
+                " (source_card_code_id, amount, type)"
+                " VALUES"
+                f" ({firm_card_code_id}, {amount}, '{REPAY}')"
+            ))
+            Log.info(f"INSERT transaction {REPAY} {firm_card_code_id=} {amount=}")
```

### Comparing `baumanecbank_common-1.1.3/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.1.4/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/README.md` & `baumanecbank_common-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.1.3/pyproject.toml` & `baumanecbank_common-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `baumanecbank_common-1.1.3/PKG-INFO` & `baumanecbank_common-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.1.3
+Version: 1.1.4
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

