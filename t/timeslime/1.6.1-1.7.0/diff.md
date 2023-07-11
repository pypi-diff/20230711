# Comparing `tmp/timeslime-1.6.1-py3-none-any.whl.zip` & `tmp/timeslime-1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 15067 bytes, number of entries: 19
--rw-r--r--  2.0 unx        0 b- defN 23-May-29 17:19 timeslime/__init__.py
--rw-r--r--  2.0 unx       52 b- defN 23-May-29 17:19 timeslime/__main__.py
--rw-r--r--  2.0 unx     7047 b- defN 23-May-29 17:19 timeslime/cli.py
--rw-r--r--  2.0 unx     1983 b- defN 23-May-29 17:19 timeslime/models.py
--rw-r--r--  2.0 unx     4429 b- defN 23-May-29 17:19 timeslime/serializer.py
--rw-r--r--  2.0 unx      489 b- defN 23-May-29 17:19 timeslime/handler/__init__.py
--rw-r--r--  2.0 unx     5997 b- defN 23-May-29 17:19 timeslime/handler/database_handler.py
--rw-r--r--  2.0 unx     1565 b- defN 23-May-29 17:19 timeslime/handler/ntp_server_handler.py
--rw-r--r--  2.0 unx     4287 b- defN 23-May-29 17:19 timeslime/handler/settings_handler.py
--rw-r--r--  2.0 unx     1092 b- defN 23-May-29 17:19 timeslime/handler/state_handler.py
--rw-r--r--  2.0 unx     8726 b- defN 23-May-29 17:19 timeslime/handler/timeslime_handler.py
--rw-r--r--  2.0 unx     5328 b- defN 23-May-29 17:19 timeslime/handler/timeslime_server_handler.py
--rw-rw-rw-  2.0 unx      534 b- defN 23-May-29 17:19 timeslime/update/1.2_to_1.3.sql
--rw-rw-rw-  2.0 unx     1072 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3073 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1617 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/RECORD
-19 files, 47447 bytes uncompressed, 12399 bytes compressed:  73.9%
+Zip file size: 15647 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 14:26 timeslime/__init__.py
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-11 14:26 timeslime/__main__.py
+-rw-r--r--  2.0 unx     8371 b- defN 23-Jul-11 14:26 timeslime/cli.py
+-rw-r--r--  2.0 unx     1983 b- defN 23-Jul-11 14:26 timeslime/models.py
+-rw-r--r--  2.0 unx     4429 b- defN 23-Jul-11 14:26 timeslime/serializer.py
+-rw-r--r--  2.0 unx      489 b- defN 23-Jul-11 14:26 timeslime/handler/__init__.py
+-rw-r--r--  2.0 unx     6366 b- defN 23-Jul-11 14:26 timeslime/handler/database_handler.py
+-rw-r--r--  2.0 unx     1565 b- defN 23-Jul-11 14:26 timeslime/handler/ntp_server_handler.py
+-rw-r--r--  2.0 unx     4287 b- defN 23-Jul-11 14:26 timeslime/handler/settings_handler.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-Jul-11 14:26 timeslime/handler/state_handler.py
+-rw-r--r--  2.0 unx     8978 b- defN 23-Jul-11 14:26 timeslime/handler/timeslime_handler.py
+-rw-r--r--  2.0 unx     5328 b- defN 23-Jul-11 14:26 timeslime/handler/timeslime_server_handler.py
+-rw-rw-rw-  2.0 unx      534 b- defN 23-Jul-11 14:26 timeslime/update/1.2_to_1.3.sql
+-rw-rw-rw-  2.0 unx     1072 b- defN 23-Jul-11 14:27 timeslime-1.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3104 b- defN 23-Jul-11 14:27 timeslime-1.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 14:27 timeslime-1.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-11 14:27 timeslime-1.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-11 14:27 timeslime-1.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1617 b- defN 23-Jul-11 14:27 timeslime-1.7.0.dist-info/RECORD
+19 files, 49423 bytes uncompressed, 12979 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: timeslime/handler/timeslime_server_handler.py
 Comment: 
 
 Filename: timeslime/update/1.2_to_1.3.sql
 Comment: 
 
-Filename: timeslime-1.6.1.dist-info/LICENSE
+Filename: timeslime-1.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: timeslime-1.6.1.dist-info/METADATA
+Filename: timeslime-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: timeslime-1.6.1.dist-info/WHEEL
+Filename: timeslime-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: timeslime-1.6.1.dist-info/entry_points.txt
+Filename: timeslime-1.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: timeslime-1.6.1.dist-info/top_level.txt
+Filename: timeslime-1.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: timeslime-1.6.1.dist-info/RECORD
+Filename: timeslime-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## timeslime/cli.py

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 import sys
-from datetime import timedelta
+from datetime import datetime, timedelta
 from os.path import expanduser, join
 
 import click
 from peewee import OperationalError
+from rich.console import Console
+from rich.table import Table
 
 from timeslime.handler import (
     DatabaseHandler,
     NtpServerHandler,
     SettingsHandler,
     StateHandler,
     TimeslimeHandler,
@@ -60,19 +62,51 @@
 @click.pass_context
 def stop(ctx, time):
     """stop time"""
     timeslime_handler = boot(ctx.obj)
     timeslime_handler.stop_time(time)
 
 @main.command('display', short_help='Display your time')
+@click.argument("date", required=False)
 @click.pass_context
-def display(ctx):
+def display(ctx, date):
+    """display elapsed time"""
     timeslime_handler = boot(ctx.obj)
-    elapsed_time = str(abs(timeslime_handler.get_elapsed_time()))
-    print(elapsed_time)
+    if date:
+        try:
+            requested_date = datetime.strptime(date, "%Y-%m-%d")
+        except ValueError as value_error:
+            raise ValueError(
+                "Date must be in the format %Y-%m-%d (eg. 2023-07-11)!"
+            ) from value_error
+    else:
+        requested_date = datetime.now().replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+    date_str = requested_date.strftime("%Y-%m-%d")
+    table = Table(
+        title=f"Timeslime - {date_str}", show_footer=True, footer_style="green"
+    )
+
+    table.add_column("Start Time", footer="Total")
+    table.add_column("Stop Time")
+    elapsed_time = str(abs(timeslime_handler.get_elapsed_time(requested_date)))
+    table.add_column("Difference", footer=elapsed_time, justify="right", style="green")
+    for timespan in timeslime_handler.get_all(start_time=requested_date):
+        if timespan.stop_time:
+            table.add_row(
+                timespan.start_time.strftime("%H:%M:%S"),
+                timespan.stop_time.strftime("%H:%M:%S"),
+                str(timespan.stop_time - timespan.start_time),
+            )
+        else:
+            table.add_row(timespan.start_time.strftime("%H:%M:%S"), "-", "-")
+
+    console = Console()
+    console.print(table)
 
 @main.command('settings', short_help='Get or set a setting')
 @click.pass_context
 @click.option('--key', required=True, help='defines setting key')
 @click.option('--value', help='defines setting value')
 @click.option('--delete', is_flag=True, help='delete a setting')
 def settings(ctx, key, value, delete):
```

## timeslime/handler/database_handler.py

```diff
@@ -1,12 +1,12 @@
 """database handler class"""
 from datetime import datetime, timedelta, timezone
 from os import mkdir
 from os.path import dirname, exists, join, realpath
-from typing import Union
+from typing import Optional, Union
 
 from peewee import SqliteDatabase
 
 from timeslime.models import Setting, State, Timespan
 
 
 class DatabaseHandler():
@@ -99,18 +99,26 @@
         """read timespan from database
         :param guid: defines id"""
         if not id:
             return None
 
         return Timespan.get_by_id(guid)
 
-    def read_timespans(self, date: datetime = None) -> list:
+    def read_timespans(
+        self,
+        start_time: Optional[datetime] = None,
+        update_at: Optional[datetime] = None,
+    ) -> list[Timespan]:
         """read all timespans from database"""
-        if date:
-            return Timespan.select().where(Timespan.updated_at > date)
+        if update_at and not start_time:
+            return Timespan.select().where(Timespan.updated_at > update_at)
+        if start_time and not update_at:
+            return Timespan.select().where(Timespan.start_time > start_time)
+        if start_time and update_at:
+            raise NotImplementedError("Set either `start_time` or `update_at`")
 
         return Timespan.select()
 
     def save_setting(self, setting: Setting) -> Setting:
         """save setting to database
         :param setting: define setting"""
         if not isinstance(setting, Setting):
```

## timeslime/handler/timeslime_handler.py

```diff
@@ -137,20 +137,23 @@
                 "Wait a few seconds to get an accurate time tracking."
             )
         else:
             time = datetime.now(tz=timezone.utc)
 
         return time
 
-    def get_elapsed_time(self) -> bool:
+    def get_elapsed_time(self, datetime_now: Optional[datetime] = None) -> bool:
         if not self.ntp_server_handler.ntp_server_is_synchronized:
             print('NTP server is not synchronized yet. Wait a few seconds to get an accurate time tracking.')
             return
+        if not datetime_now:
+            datetime_now = datetime.now()
+
         daily_sum_in_seconds = self.database_handler.get_tracked_time_in_seconds(
-            datetime.now()
+            datetime_now
         )
         current_timedelta = timedelta(seconds=0)
         if self.timespan is not None and self.timespan.stop_time is None:
             current_timedelta = datetime.now(tz=timezone.utc) - self.timespan.start_time
         return self._daily_working_time - daily_sum_in_seconds - current_timedelta
 
     def is_running(self):
@@ -160,18 +163,24 @@
             return False
 
     def get(self, guid: str) -> Timespan:
         """get a timespan
         : param guid: defines guid"""
         return self.database_handler.read_timespan(guid)
 
-    def get_all(self, filter_date: datetime = None) -> list:
+    def get_all(
+        self,
+        start_time: Optional[datetime] = None,
+        update_at: Optional[datetime] = None,
+    ) -> list[Timespan]:
         """get all timespans
         :param filter_date: defines date"""
-        return self.database_handler.read_timespans(filter_date)
+        return self.database_handler.read_timespans(
+            start_time=start_time, update_at=update_at
+        )
 
     def contains(self, guid: str) -> bool:
         """check if list contains defined id
         :param guid: defines guid"""
         try:
             self.database_handler.read_timespan(guid)
             return True
```

## Comparing `timeslime-1.6.1.dist-info/LICENSE` & `timeslime-1.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `timeslime-1.6.1.dist-info/METADATA` & `timeslime-1.7.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: timeslime
-Version: 1.6.1
+Version: 1.7.0
 Author: Christian Decker
 Author-email: christian.decker@lookslikematrix.de
 License: MIT
 Project-URL: Donate, https://www.buymeacoffee.com/lookslikematrix
 Project-URL: Source Code, https://gitlab.com/lookslikematrix/timeslime
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (==2.30.0)
-Requires-Dist: click (==8.1.3)
+Requires-Dist: click (==8.1.4)
 Requires-Dist: peewee (==3.16.2)
+Requires-Dist: rich (==13.4.2)
 Requires-Dist: dbus-python (==1.3.2) ; platform_system == "Linux"
 
 # timeslime
 
 It's a tool to track your time.
 
 ## Install
```

## Comparing `timeslime-1.6.1.dist-info/RECORD` & `timeslime-1.7.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 timeslime/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 timeslime/__main__.py,sha256=D-c9Wts6p0sR6ES-shgtXLmF1nVCS_53ixj0OJ9IsMU,52
-timeslime/cli.py,sha256=HUsg4bAztn5QW56h_Fj86YS7q1nAPT9xm-D9FdjKei4,7047
+timeslime/cli.py,sha256=4vZ02eO37TMUSEcOaCrR_QCq1To7YwAKOwEHtNSwwqQ,8371
 timeslime/models.py,sha256=maP58Mclu1aQgtEBAgdcf6U3iOAY4JxvRQoooJiDDLk,1983
 timeslime/serializer.py,sha256=M9V3jR722miV7IoXkxcjKVUfP1UOKIkQXzqwHZJqbhg,4429
 timeslime/handler/__init__.py,sha256=DgB8v_mx-6g0vIT5HBIO0GYCRbmBviytzDoT_eib4AI,489
-timeslime/handler/database_handler.py,sha256=f1hucZy8FUYMmR096TREf-dOgw5qES82pI8W4BHiKj8,5997
+timeslime/handler/database_handler.py,sha256=MA8PG5KgTxmrPnLyM3YczIVBopAaSflDJM1gHdAOX7Y,6366
 timeslime/handler/ntp_server_handler.py,sha256=da6K6OX10MxvZaFDe5uHpjMGaEKpq0T7ew3x2SP8naQ,1565
 timeslime/handler/settings_handler.py,sha256=e59rOUrmBKnP7D8JbKXIAf0QI7QUXh_mkYtZyJCuObU,4287
 timeslime/handler/state_handler.py,sha256=4NbHzLnddWpPBqKZiQeMbJiF9DTc-2gDyB1gO7J6xx8,1092
-timeslime/handler/timeslime_handler.py,sha256=FhfpHGIqAcYNZLfhCjI_11CO3R-GcLqKCDps3Nhejoo,8726
+timeslime/handler/timeslime_handler.py,sha256=_XtSl90uM1a7U_amGrBDG1P3wKmPjn7LCOSEutYzSxI,8978
 timeslime/handler/timeslime_server_handler.py,sha256=4pmMifFKQHYGI9u-MQ-0jg7oninHzBY9Kv_vRugAAAI,5328
 timeslime/update/1.2_to_1.3.sql,sha256=LLuT0LCA9W4J-5kGuiqxJ9rEgq8cSr94v1GLC-oIRBA,534
-timeslime-1.6.1.dist-info/LICENSE,sha256=LiRYlunBxa9UIPdfV7F9IRSRSISLC7bCz-DubILGtgs,1072
-timeslime-1.6.1.dist-info/METADATA,sha256=KKMysfH16H0u1367m3HHL8TWf0h9iDw9d5bSkhIc9-k,3073
-timeslime-1.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-timeslime-1.6.1.dist-info/entry_points.txt,sha256=MT9_31puJx5fzANMynwiNIhyhYsl0KWKYNkzK8PZB-g,54
-timeslime-1.6.1.dist-info/top_level.txt,sha256=kToBlgsTKvfE41ILjN4v6ZIQYLxFlROmu21LJPKmz8M,10
-timeslime-1.6.1.dist-info/RECORD,,
+timeslime-1.7.0.dist-info/LICENSE,sha256=LiRYlunBxa9UIPdfV7F9IRSRSISLC7bCz-DubILGtgs,1072
+timeslime-1.7.0.dist-info/METADATA,sha256=hgNJ0pKm6Dm5SvJIbB8YYqhVvqpuqO-oe4OfB4mgZ2o,3104
+timeslime-1.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+timeslime-1.7.0.dist-info/entry_points.txt,sha256=MT9_31puJx5fzANMynwiNIhyhYsl0KWKYNkzK8PZB-g,54
+timeslime-1.7.0.dist-info/top_level.txt,sha256=kToBlgsTKvfE41ILjN4v6ZIQYLxFlROmu21LJPKmz8M,10
+timeslime-1.7.0.dist-info/RECORD,,
```

