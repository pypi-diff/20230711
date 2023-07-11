# Comparing `tmp/no-comment-0.1.0a8.tar.gz` & `tmp/no-comment-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no-comment-0.1.0a8.tar", max compression
+gzip compressed data, was "no-comment-0.1.0a9.tar", max compression
```

## Comparing `no-comment-0.1.0a8.tar` & `no-comment-0.1.0a9.tar`

### file list

```diff
@@ -1,41 +1,58 @@
--rw-r--r--   0        0        0    34523 2023-01-04 16:29:03.268951 no-comment-0.1.0a8/LICENSE
--rw-r--r--   0        0        0       47 2023-01-31 08:09:27.509432 no-comment-0.1.0a8/README.md
--rw-r--r--   0        0        0      822 2023-01-04 16:29:03.268951 no-comment-0.1.0a8/no_comment/__init__.py
--rw-r--r--   0        0        0      736 2023-01-07 13:32:42.026352 no-comment-0.1.0a8/no_comment/application/__init__.py
--rw-r--r--   0        0        0      736 2023-01-07 13:33:05.026067 no-comment-0.1.0a8/no_comment/application/use_cases/__init__.py
--rw-r--r--   0        0        0     2191 2023-02-12 13:56:08.278136 no-comment-0.1.0a8/no_comment/application/use_cases/add_comment.py
--rw-r--r--   0        0        0     1633 2023-06-16 11:42:51.386737 no-comment-0.1.0a8/no_comment/application/use_cases/view_comments.py
--rw-r--r--   0        0        0      959 2023-01-08 17:15:56.941065 no-comment-0.1.0a8/no_comment/configuration/__init__.py
--rw-r--r--   0        0        0      933 2023-01-08 17:11:40.468169 no-comment-0.1.0a8/no_comment/configuration/wsgi.py
--rw-r--r--   0        0        0      736 2023-01-07 14:02:19.276425 no-comment-0.1.0a8/no_comment/domain/__init__.py
--rw-r--r--   0        0        0      736 2023-01-07 14:02:22.416386 no-comment-0.1.0a8/no_comment/domain/commenting/__init__.py
--rw-r--r--   0        0        0      932 2023-01-22 13:20:26.155844 no-comment-0.1.0a8/no_comment/domain/commenting/entities.py
--rw-r--r--   0        0        0     1241 2023-06-16 11:57:19.584218 no-comment-0.1.0a8/no_comment/domain/commenting/repositories.py
--rw-r--r--   0        0        0     1034 2023-01-22 13:53:03.637297 no-comment-0.1.0a8/no_comment/domain/commenting/services.py
--rw-r--r--   0        0        0     2912 2023-06-16 11:55:35.681483 no-comment-0.1.0a8/no_comment/domain/commenting/value_objects.py
--rw-r--r--   0        0        0      736 2023-01-04 16:29:03.272951 no-comment-0.1.0a8/no_comment/infrastructure/__init__.py
--rw-r--r--   0        0        0      736 2023-01-08 16:21:05.908199 no-comment-0.1.0a8/no_comment/infrastructure/file_system/__init__.py
--rw-r--r--   0        0        0     2721 2023-06-16 12:26:58.490463 no-comment-0.1.0a8/no_comment/infrastructure/file_system/repositories.py
--rw-r--r--   0        0        0     2006 2023-06-16 06:00:11.287713 no-comment-0.1.0a8/no_comment/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     3325 2023-06-16 12:15:50.470651 no-comment-0.1.0a8/no_comment/infrastructure/flask/comments.py
--rw-r--r--   0        0        0     1146 2023-01-22 13:55:42.487277 no-comment-0.1.0a8/no_comment/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-16 06:00:11.291713 no-comment-0.1.0a8/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0        0 2023-06-16 06:00:11.291713 no-comment-0.1.0a8/no_comment/infrastructure/flask/static/css/no-comment.css
--rw-r--r--   0        0        0     1467 2023-06-16 07:14:41.219262 no-comment-0.1.0a8/no_comment/infrastructure/flask/static/img/favicon.svg
--rw-r--r--   0        0        0      279 2023-06-16 06:00:11.291713 no-comment-0.1.0a8/no_comment/infrastructure/flask/static/img/feed.svg
--rw-r--r--   0        0        0    42819 2023-06-16 06:00:11.291713 no-comment-0.1.0a8/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0     1281 2023-02-15 08:18:18.655114 no-comment-0.1.0a8/no_comment/infrastructure/flask/utils.py
--rw-r--r--   0        0        0      736 2023-01-07 13:36:07.955810 no-comment-0.1.0a8/no_comment/interfaces/__init__.py
--rw-r--r--   0        0        0     1426 2023-02-15 08:17:41.803550 no-comment-0.1.0a8/no_comment/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0     5657 2023-06-16 12:23:46.192822 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0      860 2023-01-25 09:27:42.239415 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/comment.pug
--rw-r--r--   0        0        0     2168 2023-06-16 07:14:41.219262 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1130 2023-01-29 14:29:41.635851 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug
--rw-r--r--   0        0        0     3549 2023-06-16 12:17:31.977408 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/stream.pug
--rw-r--r--   0        0        0      873 2023-01-25 09:27:42.239415 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/unknown_format.pug
--rw-r--r--   0        0        0     3554 2023-02-15 08:17:21.599799 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_json.py
--rw-r--r--   0        0        0     4595 2023-02-15 08:34:01.760328 no-comment-0.1.0a8/no_comment/interfaces/to_http/as_xml.py
--rw-r--r--   0        0        0     1274 2023-02-15 08:22:23.000450 no-comment-0.1.0a8/no_comment/test_factories.py
--rw-r--r--   0        0        0     1004 2023-06-16 12:38:02.170376 no-comment-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     1359 2023-06-16 12:38:43.933986 no-comment-0.1.0a8/setup.py
--rw-r--r--   0        0        0      712 2023-06-16 12:38:43.934753 no-comment-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-01-04 16:29:03.268951 no-comment-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0     1806 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/README.md
+-rw-r--r--   0        0        0      822 2023-01-04 16:29:03.268951 no-comment-0.1.0a9/no_comment/__init__.py
+-rw-r--r--   0        0        0      736 2023-01-07 13:32:42.026352 no-comment-0.1.0a9/no_comment/application/__init__.py
+-rw-r--r--   0        0        0      736 2023-01-07 13:33:05.026067 no-comment-0.1.0a9/no_comment/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-01 09:50:20.258247 no-comment-0.1.0a9/no_comment/application/use_cases/add_comment.py
+-rw-r--r--   0        0        0     2334 2023-07-01 09:49:57.074519 no-comment-0.1.0a9/no_comment/application/use_cases/create_stream.py
+-rw-r--r--   0        0        0     2347 2023-07-01 09:49:30.058835 no-comment-0.1.0a9/no_comment/application/use_cases/display_stream.py
+-rw-r--r--   0        0        0      963 2023-06-28 08:05:43.226481 no-comment-0.1.0a9/no_comment/configuration/__init__.py
+-rw-r--r--   0        0        0     1020 2023-06-28 08:25:18.860334 no-comment-0.1.0a9/no_comment/configuration/cli.py
+-rw-r--r--   0        0        0     1025 2023-06-28 08:05:47.150433 no-comment-0.1.0a9/no_comment/configuration/wsgi.py
+-rw-r--r--   0        0        0      736 2023-01-07 14:02:19.276425 no-comment-0.1.0a9/no_comment/domain/__init__.py
+-rw-r--r--   0        0        0      736 2023-01-07 14:02:22.416386 no-comment-0.1.0a9/no_comment/domain/commenting/__init__.py
+-rw-r--r--   0        0        0     1147 2023-07-01 09:34:32.001345 no-comment-0.1.0a9/no_comment/domain/commenting/entities.py
+-rw-r--r--   0        0        0      914 2023-07-01 10:00:43.526842 no-comment-0.1.0a9/no_comment/domain/commenting/exceptions.py
+-rw-r--r--   0        0        0     1482 2023-06-28 15:11:18.695494 no-comment-0.1.0a9/no_comment/domain/commenting/repositories.py
+-rw-r--r--   0        0        0      989 2023-06-28 08:05:47.162433 no-comment-0.1.0a9/no_comment/domain/commenting/services.py
+-rw-r--r--   0        0        0     1715 2023-07-01 10:03:27.048971 no-comment-0.1.0a9/no_comment/domain/commenting/value_objects.py
+-rw-r--r--   0        0        0      736 2023-01-04 16:29:03.272951 no-comment-0.1.0a9/no_comment/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2504 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/click/__init__.py
+-rw-r--r--   0        0        0     1550 2023-06-30 14:44:39.649471 no-comment-0.1.0a9/no_comment/infrastructure/click/services.py
+-rw-r--r--   0        0        0     3034 2023-07-11 07:43:46.196223 no-comment-0.1.0a9/no_comment/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-11 07:38:42.327993 no-comment-0.1.0a9/no_comment/infrastructure/flask/ip/__init__.py
+-rw-r--r--   0        0        0     2491 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-16 06:00:11.291713 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0      213 2023-07-01 10:10:02.572179 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/css/no-comment.css
+-rw-r--r--   0        0        0     1467 2023-06-16 07:14:41.219262 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/favicon.svg
+-rw-r--r--   0        0        0      551 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/feed.svg
+-rw-r--r--   0        0        0      361 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/filter-off.svg
+-rw-r--r--   0        0        0      338 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/filter.svg
+-rw-r--r--   0        0        0    42819 2023-06-16 06:00:11.291713 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-28 06:33:12.566707 no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     3512 2023-07-11 07:12:10.037688 no-comment-0.1.0a9/no_comment/infrastructure/flask/streams.py
+-rw-r--r--   0        0        0     2003 2023-07-11 07:18:44.097988 no-comment-0.1.0a9/no_comment/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1415 2023-06-30 14:40:26.308668 no-comment-0.1.0a9/no_comment/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     2374 2023-07-11 07:32:00.081972 no-comment-0.1.0a9/no_comment/infrastructure/settings.py
+-rw-r--r--   0        0        0      736 2023-06-28 08:05:43.230481 no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4621 2023-07-02 16:52:08.051300 no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2154 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/__init__.py
+-rw-r--r--   0        0        0     1426 2023-02-15 08:17:41.803550 no-comment-0.1.0a9/no_comment/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0     7432 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-11 07:44:32.735568 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     1878 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1130 2023-01-29 14:29:41.635851 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug
+-rw-r--r--   0        0        0      860 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/comment_display.pug
+-rw-r--r--   0        0        0     5333 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/display.pug
+-rw-r--r--   0        0        0      980 2023-07-11 07:12:10.041688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/root.pug
+-rw-r--r--   0        0        0      967 2023-07-11 07:12:10.045688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/unknown.pug
+-rw-r--r--   0        0        0     1772 2023-07-11 07:12:10.045688 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     3578 2023-07-01 09:36:21.732089 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_json.py
+-rw-r--r--   0        0        0     6006 2023-07-01 09:36:02.516311 no-comment-0.1.0a9/no_comment/interfaces/to_http/as_xml.py
+-rw-r--r--   0        0        0      869 2023-06-30 13:42:06.404624 no-comment-0.1.0a9/no_comment/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-30 13:42:06.404624 no-comment-0.1.0a9/no_comment/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1810 2023-06-30 13:43:27.787615 no-comment-0.1.0a9/no_comment/test_factories.py
+-rw-r--r--   0        0        0     1238 2023-07-11 07:45:30.430797 no-comment-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0     3936 2023-07-11 07:46:34.919464 no-comment-0.1.0a9/setup.py
+-rw-r--r--   0        0        0     2710 2023-07-11 07:46:34.920215 no-comment-0.1.0a9/PKG-INFO
```

### Comparing `no-comment-0.1.0a8/LICENSE` & `no-comment-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/__init__.py` & `no-comment-0.1.0a9/no_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/application/__init__.py` & `no-comment-0.1.0a9/no_comment/application/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/application/use_cases/__init__.py` & `no-comment-0.1.0a9/no_comment/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/application/use_cases/add_comment.py` & `no-comment-0.1.0a9/no_comment/application/use_cases/add_comment.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,18 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from uuid import uuid4
 
 from no_comment.domain.commenting.entities import Comment
+from no_comment.domain.commenting.exceptions import InvalidValue
 from no_comment.domain.commenting.repositories import Comments
 from no_comment.domain.commenting.services import Calendar
-from no_comment.domain.commenting.value_objects import (
-    CommentId,
-    InvalidValue,
-    StreamId,
-    Text,
-    Url,
-)
+from no_comment.domain.commenting.value_objects import CommentId, StreamId, Text, Url
 
 
 @dataclass
 class Request:
     stream_id: str
     url: str
     text: str
```

### Comparing `no-comment-0.1.0a8/no_comment/application/use_cases/view_comments.py` & `no-comment-0.1.0a9/no_comment/application/use_cases/create_stream.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,40 +12,64 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Optional
 
-from no_comment.domain.commenting.entities import Comment
-from no_comment.domain.commenting.repositories import Comments
-from no_comment.domain.commenting.value_objects import StreamId, Url
+from no_comment.domain.commenting.entities import Stream
+from no_comment.domain.commenting.exceptions import InvalidValue
+from no_comment.domain.commenting.repositories import Streams
+from no_comment.domain.commenting.services import Calendar
+from no_comment.domain.commenting.value_objects import (
+    Author,
+    Description,
+    StreamId,
+    Title,
+)
 
 
 @dataclass
 class Request:
     stream_id: str
-    url: Optional[str] = None
-    page: Optional[int] = None
+    title: str
+    description: str
+    author: str
 
 
 class Presenter(ABC):
     @abstractmethod
-    def comment(self, comment: Comment) -> None:
+    def bad_parameter(self, message: str) -> None:
+        ...
+
+    @abstractmethod
+    def stream_already_exists(self, stream: Stream) -> None:
+        ...
+
+    @abstractmethod
+    def stream_created(self, stream: Stream) -> None:
         ...
 
 
 @dataclass
 class Interactor:
     presenter: Presenter
-    comments: Comments
+    streams: Streams
+    calendar: Calendar
 
     def execute(self, request: Request) -> None:
-        for comment in self.comments.on_stream(
-            StreamId(request.stream_id),
-            url=Url(request.url) if request.url else None,
-            page=request.page,
-            latest_first=True,
-        ):
-            self.presenter.comment(comment)
+        try:
+            stream_id = StreamId.instanciate(request.stream_id)
+            title = Title.instanciate(request.title)
+            description = Description.instanciate(request.description)
+            author = Author.instanciate(request.author)
+        except InvalidValue as exc:
+            return self.presenter.bad_parameter(str(exc))
+
+        if stream := self.streams.by_id(stream_id):
+            return self.presenter.stream_already_exists(stream)
+
+        stream = Stream(stream_id, title, description, author, self.calendar.now())
+
+        self.streams.add(stream)
+        self.presenter.stream_created(stream)
```

### Comparing `no-comment-0.1.0a8/no_comment/configuration/__init__.py` & `no-comment-0.1.0a9/no_comment/configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import os
 
 PREFIX = "NO_COMMENT_"
 
 
-def read_wsgi_config() -> dict[str, str]:
+def read_config_from_env() -> dict[str, str]:
     result = {}
     for k, v in os.environ.items():
         if k.startswith(PREFIX):
             result[k[len(PREFIX) :]] = v
     return result
```

### Comparing `no-comment-0.1.0a8/no_comment/configuration/wsgi.py` & `no-comment-0.1.0a9/no_comment/configuration/wsgi.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from flask import Flask
 
-from no_comment.configuration import read_wsgi_config
+from no_comment.configuration import read_config_from_env
 from no_comment.infrastructure.flask import build_app
+from no_comment.infrastructure.settings import WsgiSettings
 
 
 def app() -> Flask:
-    return build_app(read_wsgi_config())
+    return build_app(WsgiSettings.from_dict(read_config_from_env()))
```

### Comparing `no-comment-0.1.0a8/no_comment/domain/__init__.py` & `no-comment-0.1.0a9/no_comment/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/domain/commenting/__init__.py` & `no-comment-0.1.0a9/no_comment/domain/commenting/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/domain/commenting/entities.py` & `no-comment-0.1.0a9/no_comment/domain/commenting/entities.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,34 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 
-from .value_objects import CommentId, DateAndTime, Text, Url
+from .value_objects import (
+    Author,
+    CommentId,
+    DateAndTime,
+    Description,
+    StreamId,
+    Text,
+    Title,
+    Url,
+)
+
+
+@dataclass
+class Stream:
+    id: StreamId
+    title: Title
+    description: Description
+    author: Author
+    created_at: DateAndTime
 
 
 @dataclass
 class Comment:
     id: CommentId
     url: Url
     text: Text
-    created: DateAndTime
+    created_at: DateAndTime
```

### Comparing `no-comment-0.1.0a8/no_comment/domain/commenting/repositories.py` & `no-comment-0.1.0a9/no_comment/domain/commenting/repositories.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,27 +13,38 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from typing import Optional
 
-from .entities import Comment
+from .entities import Comment, Stream
 from .value_objects import StreamId, Url
 
 
+class Streams(ABC):
+    @abstractmethod
+    def by_id(self, stream_id: StreamId) -> Optional[Stream]:
+        ...
+
+    @abstractmethod
+    def add(self, stream: Stream) -> None:
+        ...
+
+
 class Comments(ABC):
     @abstractmethod
     def on_stream(
         self,
         stream_id: StreamId,
         /,
         *,
         latest_first: bool = True,
         page: Optional[int] = None,
+        page_size: Optional[int] = None,
         url: Optional[Url] = None,
     ) -> list[Comment]:
         ...
 
     @abstractmethod
     def add(self, stream_id: StreamId, comment: Comment) -> None:
         ...
```

### Comparing `no-comment-0.1.0a8/no_comment/domain/commenting/services.py` & `no-comment-0.1.0a9/no_comment/interfaces/to_terminal/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from datetime import datetime, timezone
+from abc import ABC, abstractmethod
 
-from .value_objects import DateAndTime
 
-
-class Calendar:
-    def __init__(self, tzinfo: timezone = timezone.utc) -> None:
-        self.__tzinfo = tzinfo
-
-    def now(self) -> DateAndTime:
-        return DateAndTime.instanciate(datetime.now(self.__tzinfo))
+class TerminalPresenter(ABC):
+    @abstractmethod
+    def exit_code(self) -> int:
+        ...
```

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/__init__.py` & `no-comment-0.1.0a9/no_comment/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/file_system/__init__.py` & `no-comment-0.1.0a9/no_comment/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/file_system/repositories.py` & `no-comment-0.1.0a9/no_comment/application/use_cases/display_stream.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,72 +10,68 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import json
-from pathlib import Path
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from typing import Optional
 
-from no_comment.domain.commenting.entities import Comment
-from no_comment.domain.commenting.repositories import Comments as InterfaceComments
-from no_comment.domain.commenting.value_objects import (
-    CommentId,
-    DateAndTime,
-    StreamId,
-    Text,
-    Url,
-)
-
-
-class Comments(InterfaceComments):
-    PAGE_SIZE: int = 10
-
-    def __init__(self, data_dir: Path) -> None:
-        self.__data_dir = data_dir
-
-    def on_stream(
-        self,
-        stream_id: StreamId,
-        /,
-        *,
-        latest_first: bool = True,
-        page: Optional[int] = None,
-        url: Optional[Url] = None,
-    ) -> list[Comment]:
-        path = self.__path_for(stream_id)
-        if not path.exists():
-            return []
-        comments = [
-            # TODO: decide what to do with bad data.
-            Comment(
-                CommentId(data.get("id", "")),
-                Url(data.get("url", "")),
-                Text(data.get("text", "")),
-                DateAndTime.from_isoformat(
-                    data.get("created", "1971-01-01T00:00:00+00:00")
-                ),
-            )
-            for data in [json.loads(line) for line in path.read_text().splitlines()]
-        ]
-        comments = sorted(comments, key=lambda c: c.created, reverse=latest_first)
-
-        first = ((page or 1) - 1) * Comments.PAGE_SIZE
-        number = Comments.PAGE_SIZE
-        return comments[first:][:number]
-
-    def __path_for(self, stream_id: StreamId) -> Path:
-        return self.__data_dir / f"{stream_id}.jsons"
-
-    def add(self, stream_id: StreamId, comment: Comment) -> None:
-        data = {
-            "id": str(comment.id),
-            "url": str(comment.url),
-            "text": str(comment.text),
-            "created": comment.created.to_isoformat(),
-        }
-        path = self.__path_for(stream_id)
-        with path.open("a") as fh:
-            fh.write(json.dumps(data))
-            fh.write("\n")
+from no_comment.domain.commenting.entities import Comment, Stream
+from no_comment.domain.commenting.exceptions import InvalidValue
+from no_comment.domain.commenting.repositories import Comments, Streams
+from no_comment.domain.commenting.value_objects import StreamId, Url
+
+
+@dataclass
+class Request:
+    stream_id: str
+    url: Optional[str] = None
+    page: Optional[int] = None
+    page_size: Optional[int] = None
+
+
+class Presenter(ABC):
+    @abstractmethod
+    def bad_request(self) -> None:
+        ...
+
+    @abstractmethod
+    def unknown_stream(self, stream_id: StreamId) -> None:
+        ...
+
+    @abstractmethod
+    def stream(self, stream: Stream) -> None:
+        ...
+
+    @abstractmethod
+    def comment(self, comment: Comment) -> None:
+        ...
+
+
+@dataclass
+class Interactor:
+    presenter: Presenter
+    streams: Streams
+    comments: Comments
+
+    def execute(self, request: Request) -> None:
+        try:
+            stream_id = StreamId.instanciate(request.stream_id)
+        except InvalidValue:
+            return self.presenter.bad_request()
+
+        if not (stream := self.streams.by_id(stream_id)):
+            return self.presenter.unknown_stream(stream_id)
+
+        self.presenter.stream(stream)
+
+        for comment in self.comments.on_stream(
+            stream.id,
+            url=Url(request.url) if request.url else None,
+            page=request.page,
+            page_size=request.page_size,
+            latest_first=True,
+        ):
+            self.presenter.comment(comment)
```

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/__init__.py` & `no-comment-0.1.0a9/no_comment/infrastructure/flask/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,47 +15,74 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from flask import Flask, get_flashed_messages, url_for
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 import no_comment.interfaces.to_http.as_html as html_presenters
 from no_comment import __version__
+from no_comment.infrastructure.settings import WsgiSettings
 
-from .comments import blueprint as comments
+from . import services
+from .auth import blueprint as auth
+from .streams import blueprint as streams
 
 
-def build_app(config: dict[str, str]) -> Flask:
+def build_app(settings: WsgiSettings) -> Flask:
+    services.define_settings(settings)
+
     app = Flask(
         __name__,
         static_url_path="/resources",
         static_folder="./static/",
     )
 
-    configure(app, config)
-    register_blueprints(app)
-    register_globals()
+    configure(app, settings)
+    register_blueprints(app, settings)
+    register_globals(settings)
+
+    app.teardown_appcontext(services.teardown_connection)
 
     return app
 
 
-def configure(app: Flask, config: dict[str, str]) -> None:
-    if config.get("PROXIED", ""):
+def configure(app: Flask, settings: WsgiSettings) -> None:
+    if settings.PROXIED:
         app.wsgi_app = ProxyFix(  # type: ignore[assignment]
             app.wsgi_app, x_for=1, x_proto=1, x_host=1, x_prefix=1
         )
 
     app.config.update(
-        # SESSION_COOKIE_SECURE=True,
+        SECRET_KEY=settings.SECRET_KEY,
+        SESSION_COOKIE_SECURE=True,
         SESSION_COOKIE_HTTPONLY=True,
         SESSION_COOKIE_SAMESITE="Lax",
     )
-    app.config.update(config)
 
 
-def register_blueprints(app: Flask) -> None:
-    app.register_blueprint(comments, url_prefix="/")
+def register_blueprints(app: Flask, settings: WsgiSettings) -> None:
+    app.register_blueprint(streams, url_prefix="/")
+
+    app.auth_links = []  # type: ignore[attr-defined]
+    app.register_blueprint(auth, url_prefix="/auth")
+
+    if settings.TOTP:
+        from no_comment.infrastructure.flask.totp import blueprint as totp
+
+        app.register_blueprint(totp, url_prefix="/auth/totp")
+        app.auth_links.append(  # type: ignore[attr-defined]
+            {"route": "totp.login", "label": "TOTP"}
+        )
+
+    if settings.AUTHORIZED_IP:
+        from no_comment.infrastructure.flask.ip import blueprint as ip
+
+        app.register_blueprint(ip, url_prefix="/auth/ip")
+        app.auth_links.append(  # type: ignore[attr-defined]
+            {"route": "ip.login", "label": "IP"}
+        )
 
 
-def register_globals() -> None:
+def register_globals(settings: WsgiSettings) -> None:
     html_presenters.register_jinja_global("version", __version__)
     html_presenters.register_jinja_global("url_for", url_for)
     html_presenters.register_jinja_global("get_flashed_messages", get_flashed_messages)
+    html_presenters.register_jinja_global("timezone", settings.TIMEZONE)
```

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/comments.py` & `no-comment-0.1.0a9/no_comment/infrastructure/flask/streams.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,75 +12,84 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from flask import Blueprint, Response, request, url_for
 
-from no_comment.application.use_cases import add_comment, view_comments
-from no_comment.infrastructure.flask.utils import presenter_to_response
+from no_comment.application.use_cases import add_comment, display_stream
+from no_comment.infrastructure.flask.utils import htmx, presenter_to_response
+from no_comment.interfaces import Pager
 from no_comment.interfaces.to_http import as_html as html_presenters
 from no_comment.interfaces.to_http import as_json as json_presenters
 from no_comment.interfaces.to_http import as_xml as xml_presenters
 
 from . import services
 
-blueprint = Blueprint("comments", __name__)
+blueprint = Blueprint("streams", __name__)
+
+
+@blueprint.get("/")
+@presenter_to_response
+def root() -> Response:
+    return html_presenters.PugPresenter("streams/root")
 
 
 @blueprint.get("/<string:stream_id>")
 @blueprint.get("/<string:stream_id>.<string:format>")
 @presenter_to_response
-def index(stream_id: str, format: str = "html") -> Response:
-    presenter = select_presenter_for_view_comments(
+def display(stream_id: str, format: str = "html") -> Response:
+    presenter = select_presenter_for_display_stream(
+        stream_id, format, request.args.get("url", "")
+    )
+    interactor = display_stream.Interactor(
+        presenter, services.get_streams(), services.get_comments()
+    )
+    rq = display_stream.Request(
         stream_id,
-        format,
-        page=int(request.args.get("page", "1")),
-        fragment=request.headers.get("Hx-Target", ""),
-    )
-    interactor = view_comments.Interactor(presenter, services.comments())
-    rq = view_comments.Request(
-        stream_id, request.args.get("url"), int(request.args.get("page", "1"))
+        request.args.get("url"),
+        int(request.args.get("page", "1")),
+        Pager.PAGE_SIZE,
     )
     interactor.execute(rq)
     return presenter
 
 
-def select_presenter_for_view_comments(
-    stream_id: str, format: str, page: int = 1, fragment: str = ""
-) -> view_comments.Presenter:
-    url_comments = url_for("comments.index", stream_id=stream_id, _external=True)
-    url_feed = url_for(
-        "comments.index", stream_id=stream_id, format=format, _external=True
+def select_presenter_for_display_stream(
+    stream_id: str, format: str, filter: str
+) -> display_stream.Presenter:
+    url_self = url_for(
+        "streams.display", stream_id=stream_id, format=format, _external=True
     )
-    description = "Description"
-    author = "Author"
+    url_alternate = url_for("streams.display", stream_id=stream_id, _external=True)
+
     PRESENTERS = {
-        "html": html_presenters.Stream(stream_id, page=page, fragment=fragment),
-        "atom": xml_presenters.StreamAsAtom(url_comments, stream_id, url_feed, author),
-        "rss": xml_presenters.StreamAsRss(stream_id, description, url_comments),
-        "json": json_presenters.StreamAsJsonFeed(),
+        "html": html_presenters.DisplayStream(
+            request.url, user=services.get_user(), fragment=htmx.target, filter=filter
+        ),
+        "atom": xml_presenters.DisplayStreamAsAtom(url_self, url_alternate),
+        "rss": xml_presenters.DisplayStreamAsRss(url_self, url_alternate),
+        "json": json_presenters.DisplayStreamAsJsonFeed(url_self, url_alternate),
     }
-    return PRESENTERS.get(format, html_presenters.UnknownFormat())
+    return PRESENTERS.get(format, html_presenters.UnknownFormat(url_alternate))
 
 
 @blueprint.post("/<string:stream_id>")
 @presenter_to_response
-def index_POST(stream_id: str) -> Response:
+def comment_add(stream_id: str) -> Response:
     presenter = html_presenters.AddComment(
-        lambda: url_for("comments.index", stream_id=stream_id),
-        fragment=request.headers.get("Hx-Target", ""),
+        lambda: url_for("streams.display", stream_id=stream_id), fragment=htmx.target
     )
     interactor = add_comment.Interactor(
-        presenter, services.comments(), services.calendar()
+        presenter, services.get_comments(), services.get_calendar()
     )
     rq = add_comment.Request(
         stream_id, request.form.get("url", ""), request.form.get("text", "")
     )
     interactor.execute(rq)
     return presenter
 
 
 @blueprint.get("/<string:stream_id>/<string:comment_id>")
 @presenter_to_response
-def comment(stream_id: str, comment_id: str) -> Response:
-    return html_presenters.Comment()
+def comment_display(stream_id: str, comment_id: str) -> Response:
+    return html_presenters.DisplayComment()
```

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/services.py` & `no-comment-0.1.0a9/no_comment/configuration/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,22 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from pathlib import Path
+from typing import Any
 
-from flask import current_app
+from no_comment.configuration import read_config_from_env
+from no_comment.infrastructure.click import build_cli
+from no_comment.infrastructure.settings import CliSettings
 
-from no_comment.domain.commenting.services import Calendar
-from no_comment.infrastructure.file_system.repositories import Comments
 
-
-def comments() -> Comments:
-    return Comments(Path(current_app.config.get("DATA_DIR", "")))
-
-
-def calendar() -> Calendar:
-    # TODO: read timezone info from service and/or server configuration.
-    return Calendar()
+def cli() -> Any:
+    return build_cli(CliSettings.from_dict(read_config_from_env()))
```

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/static/img/favicon.svg` & `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `no-comment-0.1.0a9/no_comment/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/infrastructure/flask/utils.py` & `no-comment-0.1.0a9/no_comment/infrastructure/flask/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,32 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from functools import wraps
 from typing import Any, Callable
 
-from flask import Response
+from flask import Response, request
 
 from no_comment.interfaces.to_http import HttpPresenter
 
 
+class Htmx:
+    @property
+    def target(self) -> str:
+        return request.headers.get("Hx-Target", "")
+
+
 def presenter_to_response(f: Callable[..., HttpPresenter]) -> Callable[[], Response]:
     @wraps(f)
     def decorated_function(*args: Any, **kwargs: Any) -> Response:
         presenter = f(*args, **kwargs)
         return Response(
             status=presenter.status_code(),
             headers=presenter.headers(),
             response=presenter.data(),
         )
 
     return decorated_function
+
+
+htmx = Htmx()
```

### Comparing `no-comment-0.1.0a8/no_comment/interfaces/__init__.py` & `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/comment_display.pug`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-# No Comment --- Comment any resource on the web!
-# Copyright © 2023 Bioneland
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
+//- No Comment --- Comment any resource on the web!
+//- Copyright © 2023 Bioneland
+//-
+//- This program is free software: you can redistribute it and/or modify
+//- it under the terms of the GNU Affero General Public License as
+//- published by the Free Software Foundation, either version 3 of the
+//- License, or (at your option) any later version.
+//-
+//- This program is distributed in the hope that it will be useful,
+//- but WITHOUT ANY WARRANTY; without even the implied warranty of
+//- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+//- GNU Affero General Public License for more details.
+//-
+//- You should have received a copy of the GNU Affero General Public License
+//- along with this program. If not, see <http://www.gnu.org/licenses/>.
+
+extends layout
+
+block content
+  section.section
+    .container
+      h1.title.is-1 A comment
```

### Comparing `no-comment-0.1.0a8/no_comment/interfaces/to_http/__init__.py` & `no-comment-0.1.0a9/no_comment/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/__init__.py` & `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,70 +10,85 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+from datetime import datetime
 from http import HTTPStatus as HTTP
 from pathlib import Path
-from typing import Any, Callable
+from typing import Any, Callable, Optional
+from zoneinfo import ZoneInfo
 
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 from jinja2_fragments import render_block
 
-from no_comment.application.use_cases import add_comment, view_comments
-from no_comment.domain.commenting import entities
-from no_comment.domain.commenting import entities as e
+from no_comment.application.use_cases import add_comment, display_stream
+from no_comment.domain.commenting import entities, value_objects
+from no_comment.interfaces import Pager, User
 from no_comment.interfaces.to_http import HttpPresenter
 
 ENVIRONMENT = Environment(
     loader=FileSystemLoader([Path(__file__).parent / "templates"]),
     autoescape=select_autoescape(),
     extensions=["pypugjs.ext.jinja.PyPugJSExtension"],
 )
+ENVIRONMENT.globals["timezone"] = "Europe/Paris"
 
 
 def register_jinja_global(key: str, value: Any) -> None:
     ENVIRONMENT.globals[key] = value
 
 
+def format_datetime(dt: datetime) -> str:
+    z = ZoneInfo(str(ENVIRONMENT.globals["timezone"]))
+    return dt.astimezone(z).strftime("%Y-%m-%d %H:%M:%S")
+
+
 class JinjaPresenter(HttpPresenter):
     def __init__(self, template: str, /, *, fragment: str = "", **context: Any) -> None:
         self.__status_code = HTTP.OK
         self.__headers = {"Content-Type": "text/html; charset=UTF-8"}
         self.__template = template
         self.__fragment = fragment
         self.__context = context
         self.__error = ""
 
+    def set_status_code(self, status_code: HTTP) -> None:
+        self.__status_code = status_code
+
     def status_code(self) -> int:
         return int(self.__status_code)
 
+    def set_header(self, name: str, value: str) -> None:
+        self.__headers[name] = value
+
     def headers(self) -> dict[str, str]:
         return self.__headers
 
     def data(self) -> str:
         return self.render()
 
-    def set_status_code(self, status_code: HTTP) -> None:
-        self.__status_code = status_code
-
     def error(self, message: str, status_code: HTTP) -> None:
         self.__error = message
         self.__status_code = status_code
 
     def access_not_allowed(self, login: str) -> None:
         if login:
             self.__status_code = HTTP.FORBIDDEN
             self.__error = "You cannot access this page!"
         else:
             self.__status_code = HTTP.UNAUTHORIZED
             self.__error = "You must be logged in to access this page!"
 
+    def set_template(self, template: str, fragment: str = "") -> None:
+        self.__template = template
+        self.__fragment = fragment
+
     def render(self, **context: Any) -> str:
         if self.__error:
             return ENVIRONMENT.get_template("error.pug").render(
                 **self.__context,
                 **context,
                 message=self.__error,
             )
@@ -90,57 +105,105 @@
         )
 
 
 class PugPresenter(JinjaPresenter):
     def __init__(self, template: str, **context: Any) -> None:
         super().__init__(template + ".pug", **context)
 
+    def set_template(self, template: str, fragment: str = "") -> None:
+        super().set_template(template + ".pug", fragment)
 
-class UnknownFormat(view_comments.Presenter, PugPresenter):
-    def __init__(self) -> None:
-        super().__init__("unknown_format")
-        self.set_status_code(HTTP.NOT_FOUND)
+
+class UnknownFormat(display_stream.Presenter, HttpPresenter):
+    def __init__(self, url: str) -> None:
+        self.__url = url
+
+    def status_code(self) -> int:
+        return HTTP.SEE_OTHER
+
+    def headers(self) -> dict[str, str]:
+        return {"Location": self.__url}
+
+    def data(self) -> str:
+        return ""
+
+    def bad_request(self) -> None:
+        pass
+
+    def unknown_stream(self, stream_id: value_objects.StreamId) -> None:
+        pass
+
+    def stream(self, stream: entities.Stream) -> None:
+        pass
 
     def comment(self, comment: entities.Comment) -> None:
         pass
 
 
-class Stream(view_comments.Presenter, PugPresenter):
-    def __init__(self, stream_id: str, /, *, page: int = 1, fragment: str = "") -> None:
-        super().__init__("stream", fragment=fragment)
-        self.__context: dict[str, Any] = {"stream_id": stream_id, "comments": []}
-        self.__set_page_urls(page)
-
-    def __set_page_urls(self, page: int) -> None:
-        if page > 1:
-            self.__context["previous_page_url"] = f"?page={page - 1}"
-        # FIXME how to know it's the last page?!
-        self.__context["next_page_url"] = f"?page={page + 1}"
+class DisplayStream(display_stream.Presenter, PugPresenter):
+    def __init__(
+        self,
+        url: str,
+        /,
+        *,
+        fragment: str = "",
+        filter: str = "",
+        user: Optional[User] = None,
+    ) -> None:
+        super().__init__("streams/display", fragment=fragment, user=user)
+        self.__context: dict[str, Any] = {
+            "stream": {"title": "?", "description": "?", "author": "?"},
+            "comments": [],
+            "url": filter,
+            "pager": Pager(url),
+            "error": "",
+        }
+
+    def bad_request(self) -> None:
+        self.__context["error"] = "bad request"
+        self.set_status_code(HTTP.BAD_REQUEST)
+
+    def unknown_stream(self, stream_id: value_objects.StreamId) -> None:
+        self.set_status_code(HTTP.NOT_FOUND)
+        self.set_template("streams/unknown")
+
+    def stream(self, stream: entities.Stream) -> None:
+        self.__context["stream"] = {
+            "id": str(stream.id),
+            "title": str(stream.title),
+            "description": str(stream.description),
+            "author": str(stream.author),
+        }
 
     def comment(self, comment: entities.Comment) -> None:
         self.__context["comments"].append(
             {
                 "url": str(comment.url),
                 "text": str(comment.text),
-                "created": comment.created.format("%Y-%m-%d"),
+                "created_at": format_datetime(comment.created_at.to_datetime()),
             },
         )
 
     def render(self, **context: Any) -> str:
+        self.__context["comments"] = sorted(
+            self.__context["comments"],
+            key=lambda c: str(c["created_at"]),
+            reverse=True,
+        )
         return super().render(**self.__context, **context)
 
 
-class Comment(PugPresenter):
+class DisplayComment(PugPresenter):
     def __init__(self) -> None:
-        super().__init__("comment")
+        super().__init__("streams/comment_display")
 
 
 class AddComment(PugPresenter, add_comment.Presenter):
     def __init__(self, next_url: Callable[[], str], /, *, fragment: str = "") -> None:
-        super().__init__("stream", fragment=fragment)
+        super().__init__("streams/display", fragment=fragment)
         self.__next_url = next_url
         self.__fragment = fragment
         self.__comment_id = ""
         self.__error = ""
 
     def status_code(self) -> int:
         if self.__fragment:
@@ -156,9 +219,9 @@
         if self.__fragment:
             return super().render(comment_id=self.__comment_id, error=self.__error)
         return ""
 
     def bad_parameter(self, name: str, value: str) -> None:
         self.__error = f"Missing {name}!"
 
-    def comment_added(self, comment: e.Comment) -> None:
+    def comment_added(self, comment: entities.Comment) -> None:
         self.__comment_id = str(comment.id)
```

### Comparing `no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/comment.pug` & `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/unknown.pug`

 * *Files 12% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 extends layout
 
 block content
   section.section
     .container
-      h1.title.is-1 A comment
+      h1.title.is-1 Unknown stream
+
+      article.message.is-danger
+        .message-body The stream you are looking for does not exist!
```

### Comparing `no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug` & `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/mixins/flash_messages.pug`

 * *Files identical despite different names*

### Comparing `no-comment-0.1.0a8/no_comment/interfaces/to_http/as_html/templates/unknown_format.pug` & `no-comment-0.1.0a9/no_comment/interfaces/to_http/as_html/templates/streams/root.pug`

 * *Files 19% similar despite different names*

```diff
@@ -15,9 +15,11 @@
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 extends layout
 
 block content
   section.section
     .container
-      h1.title.is-1 Unknown stream format
+      h1.title.is-1 Root
 
+      article.message.is-info
+        .message-body This is the root of all streams! Please append a stream ID to your URL.
```

### Comparing `no-comment-0.1.0a8/no_comment/test_factories.py` & `no-comment-0.1.0a9/no_comment/test_factories.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,19 +12,43 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime, timezone
 
-from no_comment.domain.commenting.entities import Comment
-from no_comment.domain.commenting.value_objects import CommentId, DateAndTime, Text, Url
+from no_comment.domain.commenting.entities import Comment, Stream
+from no_comment.domain.commenting.services import Calendar
+from no_comment.domain.commenting.value_objects import (
+    Author,
+    CommentId,
+    DateAndTime,
+    Description,
+    StreamId,
+    Text,
+    Title,
+    Url,
+)
 
 
 # FIXME `comment` is also defined as a fixture in `conftest.py`.
-def comment() -> Comment:
+def make_comment() -> Comment:
     return Comment(
         CommentId.instanciate("00000000-0000-0000-0000-000000000000"),
         Url.instanciate("https://s.d.t/p"),
         Text.instanciate("The text of the comment."),
         DateAndTime.instanciate(datetime.now(timezone.utc)),
     )
+
+
+def make_stream_id(id: str = "00000000-0000-0000-0000-000000000000") -> StreamId:
+    return StreamId.instanciate(id)
+
+
+def make_stream(id: str = str(make_stream_id())) -> Stream:
+    return Stream(
+        StreamId.instanciate(id),
+        Title.instanciate("title"),
+        Description.instanciate("description"),
+        Author.instanciate("author"),
+        Calendar().now(),
+    )
```

### Comparing `no-comment-0.1.0a8/pyproject.toml` & `no-comment-0.1.0a9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 [tool.poetry]
 name = "no-comment"
-version = "0.1.0-alpha.8"
+version = "0.1.0-alpha.9"
 description = "Comment any resource on the web!"
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
     "**/*_test.py",
     "**/conftest.py",
 ]
 
+[tool.poetry.scripts]
+no-comment = "no_comment.configuration.cli:cli"
+
 [tool.poetry.dependencies]
 python = "^3.9"
 Flask = "^2.2.2"
 pypugjs = "^5.9.12"
-bl3d = "^0.3.0"
+bl3d = "^0.4.1"
 jinja2-fragments = "^0.3.0"
+SQLAlchemy = "^2.0.17"
+bl-seth = "^0.2.0"
+click = "^8.1.3"
+tzdata = "^2023.3"
+pyotp = {version = "^2.8.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 flake8 = "^6.0.0"
 invoke = "^1.7.3"
 isort = "^5.11.4"
 mamba = "^0.11.2"
@@ -29,14 +37,17 @@
 pytest = "^7.2.0"
 robber = "^1.1.5"
 termcolor = "^2.2.0"
 types-setuptools = "^65.6.0"
 beautifulsoup4 = "^4.11.1"
 libsass = "^0.22.0"
 
+[tool.poetry.extras]
+totp = ["pyotp"]
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 line-length = 89
```

