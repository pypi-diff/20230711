# Comparing `tmp/fastchecks-0.1.0rc2.tar.gz` & `tmp/fastchecks-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0rc2.tar", max compression
+gzip compressed data, was "fastchecks-0.1.0rc3.tar", max compression
```

## Comparing `fastchecks-0.1.0rc2.tar` & `fastchecks-0.1.0rc3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1675 2023-07-10 18:11:32.675864 fastchecks-0.1.0rc2/README.md
--rw-r--r--   0        0        0      707 2023-07-09 17:17:25.642969 fastchecks-0.1.0rc2/fastchecks/__init__.py
--rw-r--r--   0        0        0     4683 2023-07-10 18:11:32.676130 fastchecks-0.1.0rc2/fastchecks/check.py
--rw-r--r--   0        0        0     9302 2023-07-10 18:11:32.676380 fastchecks-0.1.0rc2/fastchecks/cli.py
--rw-r--r--   0        0        0     3075 2023-07-10 18:11:32.676609 fastchecks-0.1.0rc2/fastchecks/conf.py
--rw-r--r--   0        0        0      311 2023-07-10 18:11:32.676793 fastchecks-0.1.0rc2/fastchecks/meta.py
--rw-r--r--   0        0        0     5661 2023-07-10 18:11:32.677045 fastchecks-0.1.0rc2/fastchecks/runner.py
--rw-r--r--   0        0        0     2328 2023-07-10 18:11:32.677294 fastchecks-0.1.0rc2/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     5114 2023-07-10 18:11:32.677569 fastchecks-0.1.0rc2/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      526 2023-07-09 17:17:25.645153 fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-10 18:11:32.677815 fastchecks-0.1.0rc2/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc2/fastchecks/util.py
--rw-r--r--   0        0        0     3530 2023-07-10 18:11:32.678274 fastchecks-0.1.0rc2/fastchecks/vutil.py
--rw-r--r--   0        0        0     1860 2023-07-10 18:11:32.724497 fastchecks-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     4826 2023-07-11 09:12:31.872679 fastchecks-0.1.0rc3/README.md
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc3/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc3/fastchecks/check.py
+-rw-r--r--   0        0        0    10504 2023-07-11 09:12:31.873206 fastchecks-0.1.0rc3/fastchecks/cli.py
+-rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc3/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc3/fastchecks/log.py
+-rw-r--r--   0        0        0      311 2023-07-10 18:11:32.676793 fastchecks-0.1.0rc3/fastchecks/meta.py
+-rw-r--r--   0        0        0     6958 2023-07-11 09:12:31.873884 fastchecks-0.1.0rc3/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc3/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc3/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc3/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc3/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc3/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1904 2023-07-11 09:12:31.920198 fastchecks-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc3/PKG-INFO
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/__init__.py` & `fastchecks-0.1.0rc3/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc2/fastchecks/check.py` & `fastchecks-0.1.0rc3/fastchecks/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
 import re2
 import aiohttp
 
 from fastchecks import conf
 from fastchecks.types import CheckResult, WebsiteCheck
 from fastchecks.util import (
     get_utcnow,
     get_utcnow_time_difference_seconds,
     is_likely_text_based_body,
     is_content_length_less_than,
 )
+from fastchecks.log import MAIN_LOGGER as logging
 
 
 async def check_website(
     session: aiohttp.ClientSession, check: WebsiteCheck, timeout: float | None = None
 ) -> CheckResult:
     """
     Access (GET) website's URL and return monitoring statistics (e.g. return status, response time, etc.).
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/cli.py` & `fastchecks-0.1.0rc3/fastchecks/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 import argparse
 from argparse import Namespace as NamedArgs
 import asyncio
 import sys
 from typing import Any
 
-from fastchecks import conf, util, vutil
+from fastchecks import conf, util, vutil, log
 from fastchecks.runner import ChecksRunnerContext
 from fastchecks.types import WebsiteCheck, WebsiteCheckScheduled
 from fastchecks import meta
 
 # ---------------------------------------------------------------------------
 
 #
 # Main parser
 #
 
 PARSER = argparse.ArgumentParser(
-    prog=meta.NAME, description=meta.DESCRIPTION, epilog=f"For more help check: {meta.WEBSITE}"
+    prog=f"{meta.NAME}.cli (v{meta.VERSION})",
+    description=meta.DESCRIPTION,
+    epilog=f"For more help check: {meta.WEBSITE}",
 )
 PARSER.add_argument(
     "--pg_conninfo",
-    type=vutil.validated_postgres_conninfo,
+    type=vutil.validated_pg_conninfo,
     help=f"(Default: read from envar {conf._POSTGRES_CONNINFO_ENVAR_NAME}) PostgreSQL connection info",
     default=conf._POSTGRES_CONNINFO,
 )
+PARSER.add_argument(
+    "--pg_auto_init",
+    type=vutil.validated_parsed_bool_answer,
+    help="(Default: True) auto initialize the PostgreSQL database if the schema is not found",
+    default=True,
+)
+PARSER.add_argument(
+    "--log_console_level",
+    choices={"CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"},
+    help=f"(Default: {log.DEFAULT_LOG_CONSOLE_LEVEL}) The logging level for the console",
+)
+PARSER.add_argument(
+    "--log_root_level",
+    choices={"CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"},
+    help="The logging level for the root logger (it affects all library loggers)",
+)
 
 
 # -----------------------------------------------------------------------------
 
 #
 # Common command arguments
 #
@@ -76,18 +94,19 @@
     )
 
     cmd.add_argument("url", **_url_kwargs())
     cmd.add_argument("--regex", **_regex_kwargs())
     cmd.add_argument("--interval", **_interval_kwargs())
 
     async def fun(ctx: ChecksRunnerContext, x: NamedArgs):
-        await ctx.checks.upsert(
+        ret = await ctx.checks.upsert(
             # The args are already validated, but just in case
             WebsiteCheckScheduled.with_check(WebsiteCheck.with_validation(x.url, x.regex), interval_seconds=x.interval)
         )
+        print(ret)
 
     cmd.set_defaults(fun=fun)
 
     return (subparsers, cmd)
 
 
 _add_upsert_check(SUBPARSERS)
@@ -207,15 +226,15 @@
 
 # -----------------------------------------------------------------------------
 
 
 def _check_all_once(subparsers: argparse._SubParsersAction) -> tuple[argparse._SubParsersAction, Any]:
     cmd = subparsers.add_parser(
         "check_all_once",
-        help="Check all websites once and write the results in the data store (without scheduling; you might want to schedule this command with crontab)",
+        help="Check all websites once and write the results in the data store (without scheduling; you might want to schedule this command with cron)",
     )
 
     async def fun(ctx: ChecksRunnerContext, x: NamedArgs):
         c = 0
         async for check in ctx.check_all_once_n_write():
             c += 1
             print(f"{util.str_pad(c)}: {check}")
@@ -280,35 +299,47 @@
 # -----------------------------------------------------------------------------
 
 
 def parse_args(argv: list[str]) -> NamedArgs:
     args = PARSER.parse_args(argv)
 
     if args.command is None:
-        print("Error: you must specify a command")
+        print("(Error) you must specify a command\n")
+        PARSER.print_help()
         sys.exit(2)
 
     return args
 
 
 def parse_str_args(argv: str) -> NamedArgs:
     return parse_args(argv.split())
 
 
 async def main(args: NamedArgs) -> None:
     # args must and are assumed to be validated
 
-    async with ChecksRunnerContext.init_with_postgres(conf.get_postgres_conninfo()) as ctx:
+    if args.log_console_level is not None:
+        log.reset_main_console_logger(level=args.log_console_level)
+    elif args.command in ("check_website_only", "check_website", "check_all_once"):
+        # Increase the level for these commands by default, because they already print the results
+        log.reset_main_console_logger(level="WARNING")
+
+    if args.log_root_level is not None:
+        log.reset_root_logger(level=args.log_root_level)
+
+    async with await ChecksRunnerContext.with_single_datastore_postgres(
+        pg_conninfo=args.pg_conninfo, auto_init=args.pg_auto_init
+    ) as ctx:
         await args.fun(ctx, args)
 
 
 # -----------------------------------------------------------------------------
 
 if __name__ == "__main__":
     # ignore the first argument, which is the program name/path
     args = parse_args(sys.argv[1:])
 
     try:
         asyncio.run(main(args))
-    except (KeyboardInterrupt, SystemExit):
+    except KeyboardInterrupt:
         # ignore program-exit-like exceptions in the cli
         pass
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/conf.py` & `fastchecks-0.1.0rc3/fastchecks/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 
 
 def get_postgres_conninfo() -> str:
     """
     Return the Postgres conninfo envar value, or raise ValueError if the environment variable is not set or invalid.
     """
     ret = read_envar_value(_POSTGRES_CONNINFO_ENVAR_NAME, _POSTGRES_CONNINFO)
-    return vutil.validated_postgres_conninfo(ret)
+    return vutil.validated_pg_conninfo(ret)
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/runner.py` & `fastchecks-0.1.0rc3/fastchecks/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import asyncio
-import logging
+from fastchecks.log import MAIN_LOGGER as logging
+import sys
 from typing import AsyncIterator
 
 import aiohttp
 from apscheduler.schedulers.async_ import AsyncScheduler
 from apscheduler.triggers.interval import IntervalTrigger
 
 from fastchecks import conf, require, util, vutil
 from fastchecks.check import check_website
 from fastchecks.sockets import CheckResultSocket, WebsiteCheckSocket
-from fastchecks.sockets.postgres import CheckResultSocketPostgres, WebsiteCheckSocketPostgres
+from fastchecks.sockets.postgres import (
+    CheckResultSocketPostgres,
+    WebsiteCheckSocketPostgres,
+    common_single_pg_datastore_is_ready,
+    common_single_pg_datastore_init,
+)
 from fastchecks.types import CheckResult, WebsiteCheck, WebsiteCheckScheduled
 
 # -----------------------------------------------------------------------------
 
 
 class ChecksRunnerContext:
     """
@@ -42,24 +48,53 @@
             else conf.validated_interval(default_interval_seconds)
         )
         """Default interval for website checks that don't specify it"""
 
     # -----------------------------------------------------------------------------
 
     @classmethod
-    def init_with_postgres(cls, postgres_conninfo: str, **kwargs) -> "ChecksRunnerContext":
-        vutil.validated_postgres_conninfo(postgres_conninfo)
+    async def with_single_datastore_postgres(
+        cls, pg_conninfo: str, auto_init: bool, timeout_init_sec: float = 10, **kwargs
+    ) -> "ChecksRunnerContext":
+        vutil.validated_pg_conninfo(pg_conninfo)
 
-        return cls(
+        ctx = cls(
             session=aiohttp.ClientSession(),
-            checks=WebsiteCheckSocketPostgres(postgres_conninfo),
-            results=CheckResultSocketPostgres(postgres_conninfo),
+            checks=WebsiteCheckSocketPostgres(pg_conninfo),
+            results=CheckResultSocketPostgres(pg_conninfo),
             **kwargs,
         )
 
+        try:
+            # For instance, we use the socket's pool to check if the single common datastore is ready
+            is_ready = await common_single_pg_datastore_is_ready(ctx.checks._pool, timeout=timeout_init_sec)
+            logging.debug(f"Postgres datastore is ready: {is_ready}")
+
+            if not is_ready:
+                require(
+                    auto_init,
+                    "The postgres database is not initialized and auto_init==False (set to True to auto-init, i.e., create the db schema)",
+                )
+
+                inited = False
+
+                async with asyncio.timeout(delay=timeout_init_sec):
+                    inited = await common_single_pg_datastore_init(ctx.checks._pool, timeout=timeout_init_sec)
+
+                require(inited, "The postgres database could not be initialized")
+        except:
+            logging.critical(
+                f"Could not initialize the postgres database after {timeout_init_sec}s -- does the DB exist?",
+                exc_info=False,
+            )
+            await ctx.close()
+            sys.exit(2)
+
+        return ctx
+
     # -----------------------------------------------------------------------------
 
     async def __aenter__(self) -> "ChecksRunnerContext":
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await asyncio.gather(self._aiohttp_session.close(), self.checks.close(), self.results.close())
@@ -73,15 +108,15 @@
         return self.default_interval_seconds if check.interval_seconds is None else check.interval_seconds
 
     # -----------------------------------------------------------------------------
 
     async def check_only(self, check: WebsiteCheck) -> CheckResult:
         """Check website without saving into results data storage."""
         ret = await check_website(self._aiohttp_session, check)
-        logging.debug(ret)
+        logging.info(ret)
         return ret
 
     async def check_n_write(self, check: WebsiteCheck) -> CheckResult:
         """Check website and save into results data storage."""
         ret = await self.check_only(check)
         await self.results.write(ret)
         return ret
@@ -126,12 +161,12 @@
 
                 async for check in await self.checks.read_all():
                     await self._add_check_to_scheduler(scheduler, check)
                     print(f"Adding check to scheduler: {check}{'' if check.interval_seconds else default_interval_msg}")
 
                 require(len(await scheduler.get_schedules()) != 0, "No checks to run. Add some checks first.")
 
-                print("\nRunning until stopped...")
+                print("\nRunning until stopped...\n")
                 await scheduler.run_until_stopped()
 
         except (KeyboardInterrupt, SystemExit):
             pass
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.1.0rc3/fastchecks/sockets/postgres/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,72 @@
-import logging
+from fastchecks.log import MAIN_LOGGER as logging
+from importlib import resources
 from typing import AsyncIterator
+
+from psycopg import sql
+from psycopg.rows import namedtuple_row
+from psycopg_pool import AsyncConnectionPool
 from pydantic import PositiveInt
-from fastchecks.types import CheckResult, WebsiteCheckScheduled, WebsiteCheck
+
 from fastchecks.sockets import CheckResultSocket, WebsiteCheckSocket
-from psycopg_pool import AsyncConnectionPool
-from psycopg.rows import namedtuple_row
-from psycopg import sql
+from fastchecks.sockets.postgres import schema
+from fastchecks.types import CheckResult, WebsiteCheck, WebsiteCheckScheduled
+
+
+async def common_single_pg_datastore_is_ready(pool: AsyncConnectionPool, timeout: float) -> bool:
+    async with pool.connection(timeout=timeout) as aconn:
+        # We just test the WebsiteCheck (written in lowercase) for existence.
+        # Note: not 100% reliable (as no other objects are tested) but good enough for now.
+        # MAYBE: support versioning of schemas with a hidden Version/Evolutions table or similar.
+        cur = await aconn.execute(
+            """
+            SELECT
+            FROM
+                pg_tables
+            WHERE
+                schemaname = 'public'
+                AND tablename = 'websitecheck';
+                """
+        )
+
+        return cur.rowcount == 1
+
+
+async def common_single_pg_datastore_init(pool: AsyncConnectionPool, timeout: float) -> bool:
+    # WARNING: Assumed to not be initialized
+    async with pool.connection(timeout=timeout) as aconn:
+        init_sql = resources.files(schema).joinpath("up.sql").read_text()
+        await aconn.execute(init_sql)
+        return True
 
 
 class WebsiteCheckSocketPostgres(WebsiteCheckSocket):
     def __init__(self, conninfo: str) -> None:
-        self.__pool = AsyncConnectionPool(conninfo)
+        self._pool = AsyncConnectionPool(conninfo)
 
     def is_closed(self) -> bool:
-        return self.__pool.closed
+        return self._pool.closed
 
-    async def upsert(self, check: WebsiteCheckScheduled) -> None:
-        async with self.__pool.connection() as aconn:
-            await aconn.execute(
+    async def upsert(self, check: WebsiteCheckScheduled) -> int:
+        async with self._pool.connection() as aconn:
+            cur = await aconn.execute(
                 """
             INSERT INTO WebsiteCheck
             (url, regex, interval_seconds)
             VALUES (%s, %s, %s)
             ON CONFLICT (url) DO UPDATE
                 SET regex = EXCLUDED.regex,
                     interval_seconds = EXCLUDED.interval_seconds;
             """,
                 (check.url, check.regex, check.interval_seconds),
             )
+            return cur.rowcount
 
     async def read_n(self, n: PositiveInt) -> AsyncIterator[WebsiteCheckScheduled]:
-        async with self.__pool.connection() as aconn:
+        async with self._pool.connection() as aconn:
             # We format the safe query in 2 steps (also below) to avoid false positives from bandit (B608:hardcoded_sql_expressions)
             # We follow psycopg recommendations for how to escape composed SQL queries: https://www.psycopg.org/psycopg3/docs/advanced/typing.html#checking-literal-strings-in-queries
             query_raw = """
                 SELECT * FROM WebsiteCheck
                 LIMIT {};"""
             query_safe = query_raw.format(n)
 
@@ -44,49 +76,49 @@
             async for row in acur:
                 # without validation, because we trust the database -- its value were validated before
                 yield WebsiteCheckScheduled.with_check(
                     WebsiteCheck.without_validation(row.url, row.regex), row.interval_seconds
                 )
 
     async def delete(self, url: str) -> int:
-        async with self.__pool.connection() as aconn:
+        async with self._pool.connection() as aconn:
             cur = await aconn.execute(
                 """
             DELETE FROM WebsiteCheck
             WHERE url = %s;""",
                 (url,),
             )
             return cur.rowcount
 
     async def delete_all(self, confirm: bool) -> int:
         if confirm:
-            async with self.__pool.connection() as aconn:
+            async with self._pool.connection() as aconn:
                 cur = await aconn.execute(
                     """
                 TRUNCATE WebsiteCheck;"""
                 )
                 return cur.rowcount
         else:
             logging.warning("Not deleting all checks because confirm is False.")
             return 0
 
     async def close(self) -> None:
-        return await self.__pool.close()
+        return await self._pool.close()
 
 
 class CheckResultSocketPostgres(CheckResultSocket):
     def __init__(self, conninfo: str) -> None:
-        self.__pool = AsyncConnectionPool(conninfo)
+        self._pool = AsyncConnectionPool(conninfo)
 
     def is_closed(self) -> bool:
-        return self.__pool.closed
+        return self._pool.closed
 
-    async def write(self, result: CheckResult) -> None:
-        async with self.__pool.connection() as aconn:
-            await aconn.execute(
+    async def write(self, result: CheckResult) -> int:
+        async with self._pool.connection() as aconn:
+            cur = await aconn.execute(
                 """
             INSERT INTO CheckResult
             (url, regex, timestamp_start, response_time, timeout_error, host_error, other_error, response_status, regex_match)
             VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s);""",
                 (
                     result.check.url,
                     result.check.regex,
@@ -98,17 +130,18 @@
                     result.host_error,
                     result.other_error,
                     #
                     result.response_status,
                     result.regex_match_to_bool_or_none(),
                 ),
             )
+            return cur.rowcount
 
     async def read_last_n(self, n: PositiveInt) -> AsyncIterator[CheckResult]:
-        async with self.__pool.connection() as aconn:
+        async with self._pool.connection() as aconn:
             query_raw = """
                 SELECT * FROM CheckResult
                 ORDER BY timestamp_start DESC
                 LIMIT {};"""
             query_safe = query_raw.format(n)
 
             acur = await aconn.execute(sql.SQL(query_safe))
@@ -126,8 +159,8 @@
                     other_error=row.other_error,
                     #
                     response_status=row.response_status,
                     regex_match=row.regex_match,
                 )
 
     async def close(self) -> None:
-        return await self.__pool.close()
+        return await self._pool.close()
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/down.sql`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -- Drop all objects in the public schema
 -- Use for testing and experimenting only
 -- Ref: https://stackoverflow.com/questions/3327312/how-can-i-drop-all-the-tables-in-a-postgresql-database
 --
 -- Likely better alternative: just drop the database and recreate it, e.g. on the CLI (and being in the fastchecks root folder):
--- dbname="fastchecks"; dropdb "$dbname"; createdb "$dbname"; cat 'fastchecks/sockets/postgres/schema/up.sql' | psql "$dbname"; psql "$dbname" -c "\dt;"
+-- _dbname="fastchecks"; dropdb "${_dbname}"; createdb "${_dbname}"; cat 'fastchecks/sockets/postgres/schema/up.sql' | psql "${_dbname}"; psql "${_dbname}" -c "\dt;"
 
 DROP SCHEMA public CASCADE;
 CREATE SCHEMA public;
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc2/fastchecks/types.py` & `fastchecks-0.1.0rc3/fastchecks/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fastchecks import conf, require
 
 
 # We use Pydantic classes for type safety and because they could be handy in the future for de/serialization.
 # See benchmarks with other alternatives (e.g. NamedTuple): https://janhendrikewers.uk/pydantic_vs_protobuf_vs_namedtuple_vs_dataclasses.html
 # Note that Pydantic V2 (released in 2023 June) promises a 5-50x speedup over V1: https://docs.pydantic.dev/2.0/blog/pydantic-v2-alpha/#headlines
 
-_MAX_REPR_LEN: int = 500
+_MAX_REPR_LEN: int = 410
 
 
 class WebsiteCheck(BaseModel):
     url: str
     regex: str | None = None
 
     @classmethod
```

### Comparing `fastchecks-0.1.0rc2/fastchecks/util.py` & `fastchecks-0.1.0rc3/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc2/fastchecks/vutil.py` & `fastchecks-0.1.0rc3/fastchecks/vutil.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,28 @@
 from numbers import Number
 from urllib.parse import ParseResult, urlparse
 import re2
 
 from fastchecks import meta, require
 
 
+__FALSE = ["false", "f", "0", "no", "n"]
+__TRUE = ["true", "t", "1", "yes", "y"]
+
+
+def validated_parsed_bool_answer(val: str) -> bool:
+    val_low = val.lower()
+    if val_low in __TRUE:
+        return True
+    elif val_low in __FALSE:
+        return False
+    else:
+        raise ValueError(f"Could not parse boolean answer value: {val}")
+
+
 def validated_parsed_is_positive_int(val: str) -> int:
     return validated_is_positive_int(int(val))
 
 
 def validated_is_positive_int(val: int) -> int:
     require(val > 0, f"Value must be positive: {val}")
     return val
@@ -66,15 +80,15 @@
     validate_url(url, accepted_schemes=ACCEPTED_WEB_URL_SCHEMES, raise_error=True)
     return url
 
 
 ACCEPTED_PG_CONNINFO_URL_SCHEMES = {"postgres", "postgresql"}
 
 
-def validated_postgres_conninfo(conninfo: str) -> str:
+def validated_pg_conninfo(conninfo: str) -> str:
     require(
         validate_url(conninfo, accepted_schemes=ACCEPTED_PG_CONNINFO_URL_SCHEMES, raise_error=False) is not None,
         f"The Postgres conninfo must be of URL form and start with a valid scheme ({ACCEPTED_PG_CONNINFO_URL_SCHEMES}) (e.g. for a local Postgres database, 'postgresql://localhost:5432/{meta.NAME}')",
     )
     return conninfo
```

### Comparing `fastchecks-0.1.0rc2/pyproject.toml` & `fastchecks-0.1.0rc3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.1.0-rc.2"
-description = ""
+version = "0.1.0-rc.3"
+description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
 
 
 [tool.poetry.dependencies]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

