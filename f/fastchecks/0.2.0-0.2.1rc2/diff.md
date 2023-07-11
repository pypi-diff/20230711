# Comparing `tmp/fastchecks-0.2.0.tar.gz` & `tmp/fastchecks-0.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.2.0.tar", max compression
+gzip compressed data, was "fastchecks-0.2.1rc2.tar", max compression
```

## Comparing `fastchecks-0.2.0.tar` & `fastchecks-0.2.1rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.0/LICENSE
--rw-r--r--   0        0        0     5047 2023-07-11 10:41:01.033929 fastchecks-0.2.0/README.md
--rw-r--r--   0        0        0      569 2023-07-11 10:41:01.034019 fastchecks-0.2.0/fastchecks/NOTICE
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.0/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.0/fastchecks/check.py
--rw-r--r--   0        0        0    11388 2023-07-11 10:41:00.994591 fastchecks-0.2.0/fastchecks/cli.py
--rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.2.0/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.0/fastchecks/log.py
--rw-r--r--   0        0        0      892 2023-07-11 10:41:00.994931 fastchecks-0.2.0/fastchecks/meta.py
--rw-r--r--   0        0        0     6992 2023-07-11 10:41:00.995276 fastchecks-0.2.0/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.0/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.0/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.0/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.0/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.0/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.0/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.2.0/fastchecks/vutil.py
--rw-r--r--   0        0        0     1974 2023-07-11 10:41:01.034139 fastchecks-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5718 1970-01-01 00:00:00.000000 fastchecks-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.1rc2/LICENSE
+-rw-r--r--   0        0        0     5033 2023-07-11 11:48:52.604708 fastchecks-0.2.1rc2/README.md
+-rw-r--r--   0        0        0      569 2023-07-11 10:41:01.034019 fastchecks-0.2.1rc2/fastchecks/NOTICE
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.1rc2/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.1rc2/fastchecks/check.py
+-rw-r--r--   0        0        0    12259 2023-07-11 11:48:52.605005 fastchecks-0.2.1rc2/fastchecks/cli.py
+-rw-r--r--   0        0        0     3165 2023-07-11 11:48:52.605178 fastchecks-0.2.1rc2/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.1rc2/fastchecks/log.py
+-rw-r--r--   0        0        0      892 2023-07-11 10:41:00.994931 fastchecks-0.2.1rc2/fastchecks/meta.py
+-rw-r--r--   0        0        0     6992 2023-07-11 11:36:08.255245 fastchecks-0.2.1rc2/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.1rc2/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.1rc2/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.1rc2/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.2.1rc2/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1978 2023-07-11 11:49:32.742553 fastchecks-0.2.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     5707 1970-01-01 00:00:00.000000 fastchecks-0.2.1rc2/PKG-INFO
```

### Comparing `fastchecks-0.2.0/LICENSE` & `fastchecks-0.2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/README.md` & `fastchecks-0.2.1rc2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ## Features
 
 **🍀 Feature-rich**
 * Websites to check & their results are stored in postgres by default 🐘 (the library is ready for other data stores / sockets).
   * You can use postgres locally installed, running on docker, or with a DBaaS, e.g. Aiven.
 * Run stored all websites once, at configurable-scheduled intervals, or even with your system's cron.
 * The scheduling keeps running even if the computer goes to sleep!
+* Nice, configurable logging
 * CLI API & Python's (Python >= 3.11).
   * A [webserver](https://github.com/juanmirocks/fastchecks/issues/3) is planned.
 * ...and more!
 
 
 **🚀 Speed**
 * All operations are asynchronous. This app sits on 3 giants:
@@ -82,24 +83,24 @@
     # Then you need to pass the conninfo to the CLI,
     # * either with the explicit optional parameter `--pg_conninfo`, or
     # * by setting the envar: `FC_POSTGRES_CONNINFO`
     # For simplicity, commands below assume you've set `FC_POSTGRES_CONNINFO`, e.g.:
     export FC_POSTGRES_CONNINFO='postgres://localhost/fastchecks'
     ```
 
-2. Add some website URL checks info (to do check later)
+2. Add some website URLs to later check for:
     ```shell
     fastchecks upsert_check 'https://example.org'  # Add a simple URL check
     fastchecks upsert_check 'https://example.org' --regex 'Example D[a-z]+'  # Update the URL check to match the response body with a regex
     fastchecks upsert_check 'https://python.org' --interval 5  # Add another URL check with a specific interval (in seconds)
     ```
 
 3. Run the checks at the scheduled intervals in the foreground until stopped.
     ```shell
-    fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
+    fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable; see command help)
     ```
 
 4. That's it! You might want to explore further options:
     * For all possibilities, run: `fastchecks -h`
     * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `fastchecks check_all_once`
     * Or run a single website check once (without registering it): `fastchecks check_website 'https://www.postgresql.org/'`
```

### Comparing `fastchecks-0.2.0/fastchecks/NOTICE` & `fastchecks-0.2.1rc2/fastchecks/NOTICE`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/__init__.py` & `fastchecks-0.2.1rc2/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/check.py` & `fastchecks-0.2.1rc2/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/cli.py` & `fastchecks-0.2.1rc2/fastchecks/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,59 @@
 from fastchecks import conf, util, vutil, log
 from fastchecks.runner import ChecksRunnerContext
 from fastchecks.types import WebsiteCheck, WebsiteCheckScheduled
 from fastchecks import meta
 
 # ---------------------------------------------------------------------------
 
+
+#
+# Common command arguments
+#
+
+
+def _url_kwargs(**kwargs) -> dict[str, Any]:
+    return {"type": vutil.validated_web_url, "help": "The URL to check", **kwargs}
+
+
+def _regex_kwargs(**kwargs) -> dict[str, Any]:
+    return {
+        "type": vutil.validated_regex,
+        "help": "(Default: no check) The regex to match against the response body",
+        **kwargs,
+    }
+
+
+def _interval_kwargs(**kwargs) -> dict[str, Any]:
+    return {
+        "type": conf.validated_parsed_interval,
+        # Default help msg for single checks
+        "help": f"(Default: as set with '--default_interval' or envar '{conf._DEFAULT_CHECK_INTERVAL_SECONDS_ENVAR_NAME}') The interval in _seconds_ for a check when it is scheduled to be run periodically (min: {conf.MIN_INTERVAL_SECONDS}, max: {conf.MAX_INTERVAL_SECONDS})",
+        **kwargs,
+    }
+
+
+# ---------------------------------------------------------------------------
+
 #
 # Main parser
 #
 
 PARSER = argparse.ArgumentParser(
     prog=f"{meta.NAME}.cli (v{meta.VERSION})",
     description=meta.DESCRIPTION,
     epilog=f"For more help check: {meta.WEBSITE}",
 )
+
+PARSER.add_argument(
+    "--default_interval",
+    **_interval_kwargs(
+        help=f"(Default: {conf.DEFAULT_CHECK_INTERVAL_SECONDS}) The default system interval in _seconds_ for checks that don't specify it (min: {conf.MIN_INTERVAL_SECONDS}, max: {conf.MAX_INTERVAL_SECONDS}). The default value can also be overridden by the envar: {conf._DEFAULT_CHECK_INTERVAL_SECONDS_ENVAR_NAME}"
+    ),
+)
 PARSER.add_argument(
     "--pg_conninfo",
     type=vutil.validated_pg_conninfo,
     help=f"(Default: read from envar {conf._POSTGRES_CONNINFO_ENVAR_NAME}) PostgreSQL connection info in URL form (e.g. 'postgres://localhost/fastchecks')",
     default=conf._POSTGRES_CONNINFO,
 )
 PARSER.add_argument(
@@ -43,41 +79,14 @@
     help="The logging level for the root logger (it affects all library loggers)",
 )
 
 
 # -----------------------------------------------------------------------------
 
 #
-# Common command arguments
-#
-
-
-def _url_kwargs(**kwargs) -> dict[str, Any]:
-    return {"type": vutil.validated_web_url, "help": "The URL to check", **kwargs}
-
-
-def _regex_kwargs(**kwargs) -> dict[str, Any]:
-    return {
-        "type": vutil.validated_regex,
-        "help": "(Default: no check) The regex to match against the response body",
-        **kwargs,
-    }
-
-
-def _interval_kwargs(**kwargs) -> dict[str, Any]:
-    return {
-        "type": conf.validated_parsed_interval,
-        "help": f"(Default: {conf.DEFAULT_CHECK_INTERVAL_SECONDS}) The interval in _seconds_ for a check when it is scheduled to be run periodically (min: {conf.MIN_INTERVAL_SECONDS}, max: {conf.MAX_INTERVAL_SECONDS})",
-        **kwargs,
-    }
-
-
-# -----------------------------------------------------------------------------
-
-#
 # Following subparsers (commands)
 #
 
 SUBPARSERS = PARSER.add_subparsers(
     title="Commands",
     dest="command",
     description=" ",
@@ -338,25 +347,31 @@
         # Increase the level for these commands by default, because they already print the results
         log.reset_main_console_logger(level="WARNING")
 
     if args.log_root_level is not None:
         log.reset_root_logger(level=args.log_root_level)
 
     async with await ChecksRunnerContext.with_single_datastore_postgres(
-        pg_conninfo=args.pg_conninfo, auto_init=args.pg_auto_init
+        pg_conninfo=args.pg_conninfo, auto_init=args.pg_auto_init, default_interval_seconds=args.default_interval
     ) as ctx:
         await args.fun(ctx, args)
 
 
 async def run_str(command: str) -> None:
-    """Convenience method to run a string command"""
+    """Convenience method to run a string command. However, within-string spaces must be escaped with a backslash, e.g.:"""
     args = parse_str_args(command)
     await _run_with_namespace(args)
 
 
+async def run_seq(command: Sequence[str]) -> None:
+    """Convenience method to run a string command. However, within-string spaces must be escaped with a backslash, e.g.:"""
+    args = parse_validate_seq_args(command)
+    await _run_with_namespace(args)
+
+
 # ---------------------------------------------------------------------------
 
 
 def main() -> None:
     args = parse_sys_args()
 
     try:
```

### Comparing `fastchecks-0.2.0/fastchecks/conf.py` & `fastchecks-0.2.1rc2/fastchecks/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,19 @@
 def validated_interval_accepting_none(interval_seconds: int | None, name: str = "interval") -> int | None:
     if interval_seconds is None:
         return None
     else:
         return vutil.validated_in_range(name, interval_seconds, MIN_INTERVAL_SECONDS, MAX_INTERVAL_SECONDS)
 
 
+_DEFAULT_CHECK_INTERVAL_SECONDS_ENVAR_NAME = "FC_DEFAULT_CHECK_INTERVAL_SECONDS"
+
 DEFAULT_CHECK_INTERVAL_SECONDS: int = validated_interval(
-    get_typed_envar("FC_DEFAULT_CHECK_INTERVAL_SECONDS", default=180, conversion=lambda x: int(x)),
-    name="FC_DEFAULT_CHECK_INTERVAL_SECONDS",
+    get_typed_envar(_DEFAULT_CHECK_INTERVAL_SECONDS_ENVAR_NAME, default=180, conversion=lambda x: int(x)),
+    name=_DEFAULT_CHECK_INTERVAL_SECONDS_ENVAR_NAME,
 )
 
 
 # -----------------------------------------------------------------------------
 
 TOO_BIG_CONTENT_LENGTH_KB = get_typed_envar("FC_TOO_BIG_CONTENT_LENGTH_KB", default=100000, conversion=lambda x: int(x))
 """
```

### Comparing `fastchecks-0.2.0/fastchecks/log.py` & `fastchecks-0.2.1rc2/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/meta.py` & `fastchecks-0.2.1rc2/fastchecks/meta.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/runner.py` & `fastchecks-0.2.1rc2/fastchecks/runner.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/sockets/__init__.py` & `fastchecks-0.2.1rc2/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/types.py` & `fastchecks-0.2.1rc2/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/util.py` & `fastchecks-0.2.1rc2/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/fastchecks/vutil.py` & `fastchecks-0.2.1rc2/fastchecks/vutil.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.0/pyproject.toml` & `fastchecks-0.2.1rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.2.0"
+version = "0.2.1-rc2"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
```

### Comparing `fastchecks-0.2.0/PKG-INFO` & `fastchecks-0.2.1rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.2.0
+Version: 0.2.1rc2
 Summary: 🚥 Fast website monitoring backend service
 Home-page: https://github.com/juanmirocks/fastchecks
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -28,14 +28,15 @@
 ## Features
 
 **🍀 Feature-rich**
 * Websites to check & their results are stored in postgres by default 🐘 (the library is ready for other data stores / sockets).
   * You can use postgres locally installed, running on docker, or with a DBaaS, e.g. Aiven.
 * Run stored all websites once, at configurable-scheduled intervals, or even with your system's cron.
 * The scheduling keeps running even if the computer goes to sleep!
+* Nice, configurable logging
 * CLI API & Python's (Python >= 3.11).
   * A [webserver](https://github.com/juanmirocks/fastchecks/issues/3) is planned.
 * ...and more!
 
 
 **🚀 Speed**
 * All operations are asynchronous. This app sits on 3 giants:
@@ -100,24 +101,24 @@
     # Then you need to pass the conninfo to the CLI,
     # * either with the explicit optional parameter `--pg_conninfo`, or
     # * by setting the envar: `FC_POSTGRES_CONNINFO`
     # For simplicity, commands below assume you've set `FC_POSTGRES_CONNINFO`, e.g.:
     export FC_POSTGRES_CONNINFO='postgres://localhost/fastchecks'
     ```
 
-2. Add some website URL checks info (to do check later)
+2. Add some website URLs to later check for:
     ```shell
     fastchecks upsert_check 'https://example.org'  # Add a simple URL check
     fastchecks upsert_check 'https://example.org' --regex 'Example D[a-z]+'  # Update the URL check to match the response body with a regex
     fastchecks upsert_check 'https://python.org' --interval 5  # Add another URL check with a specific interval (in seconds)
     ```
 
 3. Run the checks at the scheduled intervals in the foreground until stopped.
     ```shell
-    fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
+    fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable; see command help)
     ```
 
 4. That's it! You might want to explore further options:
     * For all possibilities, run: `fastchecks -h`
     * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `fastchecks check_all_once`
     * Or run a single website check once (without registering it): `fastchecks check_website 'https://www.postgresql.org/'`
```

