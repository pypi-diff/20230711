# Comparing `tmp/fastchecks-0.1.0rc3.tar.gz` & `tmp/fastchecks-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0rc3.tar", max compression
+gzip compressed data, was "fastchecks-0.1.0rc4.tar", max compression
```

## Comparing `fastchecks-0.1.0rc3.tar` & `fastchecks-0.1.0rc4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4826 2023-07-11 09:12:31.872679 fastchecks-0.1.0rc3/README.md
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc3/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc3/fastchecks/check.py
--rw-r--r--   0        0        0    10504 2023-07-11 09:12:31.873206 fastchecks-0.1.0rc3/fastchecks/cli.py
--rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc3/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc3/fastchecks/log.py
--rw-r--r--   0        0        0      311 2023-07-10 18:11:32.676793 fastchecks-0.1.0rc3/fastchecks/meta.py
--rw-r--r--   0        0        0     6958 2023-07-11 09:12:31.873884 fastchecks-0.1.0rc3/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc3/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc3/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc3/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc3/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc3/fastchecks/vutil.py
--rw-r--r--   0        0        0     1904 2023-07-11 09:12:31.920198 fastchecks-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     4826 2023-07-11 09:12:31.872679 fastchecks-0.1.0rc4/README.md
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc4/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc4/fastchecks/check.py
+-rw-r--r--   0        0        0    11178 2023-07-11 09:32:40.251963 fastchecks-0.1.0rc4/fastchecks/cli.py
+-rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc4/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc4/fastchecks/log.py
+-rw-r--r--   0        0        0      311 2023-07-10 18:11:32.676793 fastchecks-0.1.0rc4/fastchecks/meta.py
+-rw-r--r--   0        0        0     6958 2023-07-11 09:12:31.873884 fastchecks-0.1.0rc4/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc4/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc4/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc4/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc4/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc4/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc4/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc4/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1963 2023-07-11 09:34:25.793919 fastchecks-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc4/PKG-INFO
```

### Comparing `fastchecks-0.1.0rc3/README.md` & `fastchecks-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/__init__.py` & `fastchecks-0.1.0rc4/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/check.py` & `fastchecks-0.1.0rc4/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/cli.py` & `fastchecks-0.1.0rc4/fastchecks/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from argparse import Namespace as NamedArgs
 import asyncio
 import sys
-from typing import Any
+from typing import Any, Sequence
 
 from fastchecks import conf, util, vutil, log
 from fastchecks.runner import ChecksRunnerContext
 from fastchecks.types import WebsiteCheck, WebsiteCheckScheduled
 from fastchecks import meta
 
 # ---------------------------------------------------------------------------
@@ -293,33 +293,43 @@
     return (subparsers, cmd)
 
 
 _add_read_last_results(SUBPARSERS)
 
 
 # -----------------------------------------------------------------------------
+# ---------------------------------------------------------------------------
+# ---------------------------------------------------------------------------
 
 
-def parse_args(argv: list[str]) -> NamedArgs:
+def parse_validate_seq_args(argv: Sequence[str]) -> NamedArgs:
     args = PARSER.parse_args(argv)
 
     if args.command is None:
         print("(Error) you must specify a command\n")
         PARSER.print_help()
         sys.exit(2)
 
     return args
 
 
+def parse_sys_args() -> NamedArgs:
+    # ignore the first argument, which is the program name/path
+    return parse_validate_seq_args(sys.argv[1:])
+
+
 def parse_str_args(argv: str) -> NamedArgs:
-    return parse_args(argv.split())
+    return parse_validate_seq_args(argv.split())
 
 
-async def main(args: NamedArgs) -> None:
-    # args must and are assumed to be validated
+# ---------------------------------------------------------------------------
+
+
+async def _run_with_namespace(args: NamedArgs) -> None:
+    """Given args must and are ASSUMED to be validated"""
 
     if args.log_console_level is not None:
         log.reset_main_console_logger(level=args.log_console_level)
     elif args.command in ("check_website_only", "check_website", "check_all_once"):
         # Increase the level for these commands by default, because they already print the results
         log.reset_main_console_logger(level="WARNING")
 
@@ -328,18 +338,30 @@
 
     async with await ChecksRunnerContext.with_single_datastore_postgres(
         pg_conninfo=args.pg_conninfo, auto_init=args.pg_auto_init
     ) as ctx:
         await args.fun(ctx, args)
 
 
-# -----------------------------------------------------------------------------
+async def run_str(command: str) -> None:
+    """Convenience method to run a string command"""
+    args = parse_str_args(command)
+    await _run_with_namespace(args)
 
-if __name__ == "__main__":
-    # ignore the first argument, which is the program name/path
-    args = parse_args(sys.argv[1:])
+
+# ---------------------------------------------------------------------------
+
+
+def main() -> None:
+    args = parse_sys_args()
 
     try:
-        asyncio.run(main(args))
+        asyncio.run(_run_with_namespace(args))
     except KeyboardInterrupt:
         # ignore program-exit-like exceptions in the cli
         pass
+
+
+# -----------------------------------------------------------------------------
+
+if __name__ == "__main__":
+    main()
```

### Comparing `fastchecks-0.1.0rc3/fastchecks/conf.py` & `fastchecks-0.1.0rc4/fastchecks/conf.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/log.py` & `fastchecks-0.1.0rc4/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/runner.py` & `fastchecks-0.1.0rc4/fastchecks/runner.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/sockets/__init__.py` & `fastchecks-0.1.0rc4/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.1.0rc4/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.1.0rc4/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.1.0rc4/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/types.py` & `fastchecks-0.1.0rc4/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/util.py` & `fastchecks-0.1.0rc4/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/fastchecks/vutil.py` & `fastchecks-0.1.0rc4/fastchecks/vutil.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc3/pyproject.toml` & `fastchecks-0.1.0rc4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.1.0-rc.3"
+version = "0.1.0-rc.4"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
 
 
+[tool.poetry.scripts]
+fastchecks = 'fastchecks.cli:main'
+
+
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.8.4"
 psycopg = { extras = ["binary", "pool"], version = "^3.1.9" }
 pydantic = "^2.0.1"
 apscheduler = "4.0.0a2"
 google-re2 = "^1.0"
```

### Comparing `fastchecks-0.1.0rc3/PKG-INFO` & `fastchecks-0.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: 🚥 Fast website monitoring backend service
 Home-page: https://github.com/juanmirocks/fastchecks
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

