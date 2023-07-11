# Comparing `tmp/blastpipe-0.4.26.tar.gz` & `tmp/blastpipe-0.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-0.4.26.tar", last modified: Thu Jul  6 02:06:59 2023, max compression
+gzip compressed data, was "blastpipe-0.4.27.tar", last modified: Tue Jul 11 11:02:30 2023, max compression
```

## Comparing `blastpipe-0.4.26.tar` & `blastpipe-0.4.27.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.674680 blastpipe-0.4.26/
--rw-rw-r--   0 ross      (1000) ross      (1000)     3723 2023-07-06 02:06:59.000000 blastpipe-0.4.26/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)       56 2023-07-06 02:06:59.000000 blastpipe-0.4.26/.markdownlint.json
--rw-rw-r--   0 ross      (1000) ross      (1000)    13270 2023-07-06 02:06:59.000000 blastpipe-0.4.26/CHANGELOG.md
--rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-07-06 02:06:59.000000 blastpipe-0.4.26/LICENSE.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)     4612 2023-07-06 02:06:59.000000 blastpipe-0.4.26/NOTICE.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     6925 2023-07-06 02:06:59.000000 blastpipe-0.4.26/PKG-INFO
--rw-rw-r--   0 ross      (1000) ross      (1000)     6032 2023-07-06 02:06:59.000000 blastpipe-0.4.26/README.rst
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/
--rw-rw-r--   0 ross      (1000) ross      (1000)     1629 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3234 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/backports.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1811 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/buffer.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1666 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/loop.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2867 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/malloc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      971 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     1351 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/mixin.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1808 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/sequence.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1408 2023-07-06 02:06:59.000000 blastpipe-0.4.26/blastpipe/tailcall.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2987 2023-07-06 02:06:59.000000 blastpipe-0.4.26/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     5543 2023-07-06 02:06:59.000000 blastpipe-0.4.26/meson.options
--rw-rw-r--   0 ross      (1000) ross      (1000)    13364 2023-07-06 02:06:59.000000 blastpipe-0.4.26/pyproject.toml
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/
--rw-rw-r--   0 ross      (1000) ross      (1000)      739 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/dev.wrap
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/
--rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/css/
--rw-rw-r--   0 ross      (1000) ross      (1000)      767 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 ross      (1000) ross      (1000)      693 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)      633 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_templates/
--rw-rw-r--   0 ross      (1000) ross      (1000)     1033 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 ross      (1000) ross      (1000)      694 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)      860 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/conf.cfg
--rw-rw-r--   0 ross      (1000) ross      (1000)     1751 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/index.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)     2680 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     2058 2023-07-06 02:06:59.000000 blastpipe-0.4.26/subprojects/docs/meson.options
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/
--rw-rw-r--   0 ross      (1000) ross      (1000)     2350 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     1173 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/test_backports.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2503 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/test_fuzz.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1689 2023-07-06 02:06:59.000000 blastpipe-0.4.26/tests/test_tailcall.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.553930 blastpipe-0.4.27/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3723 2023-07-11 11:02:30.000000 blastpipe-0.4.27/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)       56 2023-07-11 11:02:30.000000 blastpipe-0.4.27/.markdownlint.json
+-rw-rw-r--   0 ross      (1000) ross      (1000)    13941 2023-07-11 11:02:30.000000 blastpipe-0.4.27/CHANGELOG.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-07-11 11:02:30.000000 blastpipe-0.4.27/LICENSE.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4612 2023-07-11 11:02:30.000000 blastpipe-0.4.27/NOTICE.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     6925 2023-07-11 11:02:30.000000 blastpipe-0.4.27/PKG-INFO
+-rw-rw-r--   0 ross      (1000) ross      (1000)     6032 2023-07-11 11:02:30.000000 blastpipe-0.4.27/README.rst
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1739 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3001 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/backports.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1979 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/buffer.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1677 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/loop.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3070 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/malloc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      971 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1423 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/mixin.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      617 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/py.typed
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1828 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/sequence.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1531 2023-07-11 11:02:30.000000 blastpipe-0.4.27/blastpipe/tailcall.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2987 2023-07-11 11:02:30.000000 blastpipe-0.4.27/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     5549 2023-07-11 11:02:30.000000 blastpipe-0.4.27/meson.options
+-rw-rw-r--   0 ross      (1000) ross      (1000)    13363 2023-07-11 11:02:30.000000 blastpipe-0.4.27/pyproject.toml
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/
+-rw-rw-r--   0 ross      (1000) ross      (1000)      739 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/dev.wrap
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_static/
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_static/css/
+-rw-rw-r--   0 ross      (1000) ross      (1000)      767 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 ross      (1000) ross      (1000)      693 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)      633 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_templates/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1033 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 ross      (1000) ross      (1000)      694 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)      860 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/conf.cfg
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1751 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/index.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2680 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2058 2023-07-11 11:02:30.000000 blastpipe-0.4.27/subprojects/docs/meson.options
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-07-11 11:02:30.000000 blastpipe-0.4.27/tests/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2350 2023-07-11 11:02:30.000000 blastpipe-0.4.27/tests/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1219 2023-07-11 11:02:30.000000 blastpipe-0.4.27/tests/test_backports.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2583 2023-07-11 11:02:30.000000 blastpipe-0.4.27/tests/test_fuzz.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1858 2023-07-11 11:02:30.000000 blastpipe-0.4.27/tests/test_tailcall.py
```

### Comparing `blastpipe-0.4.26/.gitignore` & `blastpipe-0.4.27/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/CHANGELOG.md` & `blastpipe-0.4.27/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,24 @@
    specific language governing permissions and limitations
    under the License. -->
 
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.26 (2023-07-05)
+
+### Other
+
+* 🔨 changelog ([`34ff55a`](https://github.com/rjdbcm/blastpipe/commit/34ff55a9d7d4567065d9da1f82f616bc08a28edf))
+* PKG-INFO Updated ([`4046a0b`](https://github.com/rjdbcm/blastpipe/commit/4046a0bfc7ca7e9ec39badb68691f25023d1c1da))
+* 🔨(meson.options): disable doc8 run for now. ([`16e3219`](https://github.com/rjdbcm/blastpipe/commit/16e3219ac85e11a7b744a708a4909309c6212755))
+* Merge ([`d17ef64`](https://github.com/rjdbcm/blastpipe/commit/d17ef64e2e3f3b6b005eb6130dfbc2aee67d92f6))
+* 🔨(meson.build): disable subprojects/docs ([`22f48fb`](https://github.com/rjdbcm/blastpipe/commit/22f48fb1c9e3dc0c127ad993256e9a16d1e8549c))
+
 ## v0.4.25 (2023-07-05)
 
 ### Fix
 
 * :pencil2:(pyproject.toml): defer sphinxawesome-theme to ozi. ([`b1e144d`](https://github.com/rjdbcm/blastpipe/commit/b1e144d050f04f3887b1d64ac6a4f7454585792a))
 * :pencil2:(README.rst): use blastpipe badge not OZI. ([`7a71e70`](https://github.com/rjdbcm/blastpipe/commit/7a71e70618441555406c574633e49b5e842309c8))
```

### Comparing `blastpipe-0.4.26/LICENSE.txt` & `blastpipe-0.4.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/NOTICE.md` & `blastpipe-0.4.27/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/PKG-INFO` & `blastpipe-0.4.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 0.4.26
+Version: 0.4.27
 Summary: Packaged with OZI.
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blastpipe-0.4.26/README.rst` & `blastpipe-0.4.27/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/blastpipe/__init__.py` & `blastpipe-0.4.27/blastpipe/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import platform
 import sys
-from datetime import date
+from datetime import date, datetime, timezone
 from importlib.metadata import PackageNotFoundError, version
+from typing import Annotated, Any
 
 try:
-    __version__ = version("blastpipe")
-except PackageNotFoundError:
-    # package is not installed
+    __version__ = version('blastpipe')
+except PackageNotFoundError:  # pragma: no cover
     pass
 
 PYMAJOR, PYMINOR, PYPATCH = map(int, platform.python_version_tuple())
 minor_deprecation = {
     9: date(2025, 10, 1),
     10: date(2026, 10, 1),
     11: date(2027, 10, 1),
     12: date(2028, 10, 1),
 }
 python3_eol = minor_deprecation.get(PYMINOR, date(2008, 12, 3))
 
-if date.today() > python3_eol:  # pragma: no cover
+if datetime.now(tz=timezone.utc).date() > python3_eol:  # pragma: no cover
     raise RuntimeError(
-        f"Python {PYMAJOR}.{PYMINOR}.{PYPATCH} is not supported" f"as of {python3_eol}."
+        f'Python {PYMAJOR}.{PYMINOR}.{PYPATCH} is not supported as of {python3_eol}.'
     )
 
 
-def public(obj):
+def public(obj: Any) -> Annotated[Any, '__name__ in __all__']:
     """Declares an object as public."""
     mod = sys.modules[obj.__module__]
     # pylint: disable=unnecessary-dunder-call
-    if hasattr(mod, "__all__"):
+    if hasattr(mod, '__all__'):
         mod.__all__.append(obj.__name__)
     else:
-        mod.__setattr__("__all__", [obj.__name__])
+        mod.__setattr__('__all__', [obj.__name__])
     return obj
```

### Comparing `blastpipe-0.4.26/blastpipe/backports.py` & `blastpipe-0.4.27/blastpipe/backports.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,85 +11,79 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import re
 import string
-from typing import List, Optional, Protocol, TypeVar
+from typing import Any, List, Optional, Protocol, TypeVar
 
+# pylint: disable=import-error
 from . import PYMAJOR, PYMINOR, public
 from .mixin import Mixin, mixin
 
 
-# pylint: disable=missing-function-docstring
 class IsTemplatePre311(Protocol):
     """Protocol to check if a Template is pre-3.11"""
 
     delimiter: str
-    # r'[a-z]' matches to non-ASCII letters when used with IGNORECASE, but
-    # without the ASCII flag.  We can't add re.ASCII to flags because of
-    # backward compatibility.  So we use the ?a local flag and [a-z] pattern.
-    # See https://bugs.python.org/issue31672
-    idpattern: r"str"
-    braceidpattern: r"Optional[str]"
+    idpattern: r'str'
+    braceidpattern: r'Optional[str]'
     flags: int
     pattern: re.Pattern
     template: str
 
-    def safe_substitute(self):
-        ...
+    def safe_substitute(self: Any) -> Optional[str]:
+        """Abstract method to be implemented by base"""
 
-    def substitute(self):
-        ...
+    def substitute(self: Any) -> Optional[str]:
+        """Abstract method to be implemented by base"""
 
 
-T = TypeVar("T", bound="string.Template")
+T = TypeVar('T', bound='string.Template')
 
 
 class TemplateGetIdentifiersMixin(Mixin):
     """Example Template mixin with preferred way of typing and using mixins"""
 
     delimiter: str
-    idpattern: r"str"
-    braceidpattern: r"Optional[str]"
+    idpattern: r'str'
+    braceidpattern: r'Optional[str]'
     flags: int
     pattern: re.Pattern
     template: str
 
-    def safe_substitute(self):
+    def safe_substitute(self: object) -> Optional[str]:
         """Abstract method to be implemented by base"""
 
-    def substitute(self):
+    def substitute(self: object) -> Optional[str]:
         """Abstract method to be implemented by base"""
 
     def get_identifiers(self: IsTemplatePre311) -> List[str]:  # pragma: defer to string
         """Mixin method get_identifiers for older Template pre-3.11"""
         ids = []
         for i in self.pattern.finditer(self.template):
-            named = i.group("named") or i.group("braced")
+            named = i.group('named') or i.group('braced')
             if named is not None and named not in ids:
-                # add a named group only the first time it appears
                 ids.append(named)
-            elif named is None and i.group("invalid") is None and i.group("escaped") is None:
-                # If all the groups are None, there must be
-                # another group we're not expecting
-                raise ValueError("Unrecognized named group in pattern", self.pattern)
+            elif named is None and i.group('invalid') is None and i.group('escaped') is None:
+                raise ValueError('Unrecognized named group in pattern', self.pattern)
         return ids
 
     @classmethod
     def extend_with(cls: type[IsTemplatePre311], instance: T) -> T:
+        """Extend the class with the mixin instance."""
         instance.__class__ = type(
-            f"{instance.__class__.__name__}With{cls.__name__}",
+            f'{instance.__class__.__name__}With{cls.__name__}',
             (instance.__class__, cls),
             {},
         )
         return instance
 
 
 # pylint: disable=line-too-long
 if PYMAJOR >= 3 and PYMINOR < 11:  # pragma: defer to python
     Template = public(
         mixin(TemplateGetIdentifiersMixin, string.Template)
-    )  # noqa: E501; pragma: defer to string
+    )  # pragma: defer to string
 else:
     Template = public(string.Template)  # pragma: defer to string
```

### Comparing `blastpipe-0.4.26/blastpipe/buffer.py` & `blastpipe-0.4.27/blastpipe/buffer.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,29 @@
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-import asyncio  # pragma: defer to asyncio
+from typing import TYPE_CHECKING  # pragma: no cover
 
+# pylint: disable=import-error
 from . import public  # pragma: no cover
 
+if TYPE_CHECKING:  # pragma: no cover
+    import asyncio  # pragma: defer to asyncio
 
+
+# pylint: disable=used-before-assignment
 @public  # pragma: defer to python
 async def prefixed_send(stream: asyncio.StreamWriter, buffer: bytes) -> None:
     """Write a length-prefixed buffer to the stream"""
     # Encode the message length as a 4 byte big-endian integer.
-    prefix = len(buffer).to_bytes(4, "big")
+    prefix = len(buffer).to_bytes(4, 'big')
 
     # Write the prefix and buffer to the stream.
     stream.write(prefix)
     await stream.drain()
 
     stream.write(buffer)
     await stream.drain()
@@ -39,11 +44,11 @@
 async def prefixed_recv(stream: asyncio.StreamReader) -> bytes:
     """Read a length-prefixed buffer from the stream"""
     # Read the next 4 byte prefix
     prefix = await stream.readexactly(4)
 
     # Convert the prefix back into an integer for the next message length
     # pylint: disable=invalid-name
-    n = int.from_bytes(prefix, "big")
+    n = int.from_bytes(prefix, 'big')
 
     # Read in the full message buffer
     return await stream.readexactly(n)
```

### Comparing `blastpipe-0.4.26/blastpipe/loop.py` & `blastpipe-0.4.27/blastpipe/loop.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,39 +9,39 @@
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
-# pyright: reportGeneralTypeIssues=false
 from contextlib import suppress
-from typing import Any, Callable, Optional, Tuple, Type
+from typing import Any, Callable, NoReturn, Optional, Tuple, Type, Union
 
+# pylint: disable=import-error
 from . import public
 
 
-# pylint: disable=inconsistent-return-statements
 @public
 def while_raised(
     exc_types: Tuple[Type[Exception]],
     target: Callable,
-    *args,
-    implicit_break=True,
-) -> Optional[Any]:
+    /,
+    *args: Any,
+    implicit_break: bool = True,
+) -> Union[Optional[Any], NoReturn]:
     """Repeats a target function while suppressing exceptions provided.
     This is a convenience wrapper around :py:func:`contextlib.suppress`.
     :param exc_types: The exception types to suppress.
     :type  exc_types: Tuple[Type[Exception]]
     :param target: The function to repeat.
     :type  target: Callable
     :param implicit_break: Whether to implicitly break out of the loop.
     :type  implicit_break: bool, defaults to True
     :return: The return value of the target function.
     """
     while True:
-        with suppress(exc_types):
+        with suppress(*exc_types):
             if implicit_break:
                 return target(*args)
             target(*args)
             break
+    return None
```

### Comparing `blastpipe-0.4.26/blastpipe/malloc.py` & `blastpipe-0.4.27/blastpipe/malloc.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,31 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from collections import deque
 from itertools import chain
 from sys import getsizeof, stderr
+from typing import Any, Callable, Dict, Hashable, Optional, Sized, Union
 
 try:
     from reprlib import repr  # pylint: disable=redefined-builtin
 except ImportError:  # pragma: defer to python
     pass
 
+# pylint: disable=import-error
 from . import public
 
 
 @public
-def total_size(obj, handlers=None, verbose=False):  # noqa: C901
+def total_size(  # noqa: C901
+    obj: Hashable,
+    handlers: Optional[Dict[Any, Callable]] = None,
+    verbose: bool = False,
+) -> int:
     """Returns the approximate memory footprint an object and all of its contents.
 
     See `recipe <https://code.activestate.com/recipes/577504/>`__ for original.
 
     :param obj: object to measure size of
     :type  obj: object
     :param handlers: handlers to iterate over contents of containers, defaults to None
@@ -46,38 +52,40 @@
 
         handlers = {SomeContainerClass: iter,
                     OtherContainerClass: OtherContainerClass.get_elements}
     """
     if handlers is None:
         handlers = {}
 
-    def dict_handler(_dict):  # pragma: defer to python
+    def dict_handler(_dict: dict) -> chain:  # pragma: defer to python
+        """Default handler for dict objects"""
         return chain.from_iterable(_dict.items())
 
     all_handlers = {
         tuple: iter,
         list: iter,
         deque: iter,
         dict: dict_handler,
         set: iter,
         frozenset: iter,
     }
-    all_handlers.update(handlers)  # user handlers take precedence
-    seen = set()  # track which object id's have already been seen
-    default_size = getsizeof(0)  # estimate sizeof object without __sizeof__
+    all_handlers.update(handlers)
+    seen = set()
+    default_size = getsizeof(0)
 
-    def sizeof(obj):
+    def sizeof(obj: Union[Sized, Hashable]) -> int:
+        """return size of object in bytes"""
         if id(obj) in seen:  # pragma: defer to python
             return 0
         seen.add(id(obj))
         size_total = getsizeof(obj, default_size)
 
         if verbose:
             print(size_total, type(obj), repr(obj), file=stderr)
 
         for typ, handler in all_handlers.items():
             if isinstance(obj, typ):
-                size_total += sum(map(sizeof, handler(obj)))
+                size_total += sum(map(sizeof, handler(obj)))  # type: ignore
                 break
         return size_total
 
     return sizeof(obj)
```

### Comparing `blastpipe-0.4.26/blastpipe/meson.build` & `blastpipe-0.4.27/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/blastpipe/mixin.py` & `blastpipe-0.4.27/blastpipe/mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,37 +12,39 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from abc import ABC, abstractmethod
 from typing import Any, Generic, TypeVar
 
+# pylint: disable=import-error
 from . import public
 
 
 # pylint: disable=too-few-public-methods
 @public
 class BaseMixin(ABC):
     """Abstract mixin class"""
 
     @classmethod
     @abstractmethod
     def extend_with(cls: Any, instance: Any) -> Any:
         """extend the instance with the mixin cls"""
 
 
-_T = TypeVar("_T", bound="BaseMixin")
+_T = TypeVar('_T', bound='BaseMixin')
 
 
 @public
 class Mixin(Generic[_T], BaseMixin):
     """Generic mixin class"""
 
 
 @public
 def mixin(cls: Any, base: Any) -> Any:
     """Helper function to extend the class with the base"""
 
-    def __wrapper(*args, **kwargs):
+    def __wrapper(*args: Any, **kwargs: Any) -> Any:
+        """decorator"""
         return cls.extend_with(base(*args, **kwargs))
 
     return __wrapper
```

### Comparing `blastpipe-0.4.26/blastpipe/sequence.py` & `blastpipe-0.4.27/blastpipe/sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,37 +12,38 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import asyncio
 from typing import Set
 
+# pylint: disable=import-error
 from . import public
 from .tailcall import async_tail_call
 
 
-async def _chr_union(*args) -> Set[str]:
+async def _chr_union(*args: int) -> Set[str]:
     """creates a set of all characters in the union of the given chars"""
     chars = set()
     if len(args) == 2 and all(map(isinstance, args, (int,) * len(args))):
         start, stop = args
         chars |= {chr(i) for i in range(start, stop)}
         return chars
     for i in args:
         if isinstance(i, int):
             chars |= {chr(i)}
         elif len(i) == 2 and all(map(isinstance, i, (int,) * len(i))):
-            return i  # async_tail_call(chr_union, i)
+            return i
         else:
-            raise TypeError(f"Expected Sequence or int, got {type(i)}")
+            raise TypeError(f'Expected Sequence or int, got {type(i)}')
     return chars
 
 
 @public
-def chr_union(*args):
+def chr_union(*args: int) -> Set[str]:
     """Wraps an asynchronous sequence of int ranges or ints into a set of str
     :return: a set of chr()
        # 1. range(start=args[0], stop=args[1])
           * OR
        # 2. chr(arg[n] if type(arg[n])==int) | chr_union(arg[:2])
     :raises: TypeError
         if not a sequence of start,stop pairs and ints, an int, or a start, stop pair
```

### Comparing `blastpipe-0.4.26/blastpipe/tailcall.py` & `blastpipe-0.4.27/blastpipe/tailcall.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import functools
-from typing import Annotated, Callable, Optional, Tuple
+from typing import Annotated, Any, Callable, Mapping, Optional, Tuple
 
+# pylint: disable=import-error
 from . import public
 
-__all__ = []
-
-TAIL_CALL: Tuple[()] = tuple()  # PEP 484 Empty Tuple
+TAIL_CALL: Tuple[()] = ()
 
 
 @public
 def async_tail_call(
-    active=True,
-) -> Annotated[Callable, Annotated[Optional[Tuple[()]], "@tail_call()"]]:
+    active: bool = True,
+) -> Annotated[Callable, Annotated[Optional[Tuple[()]], '@tail_call()']]:
     """Async tail_call decorator.
     :param active: Whether to activate async tail call optimization.
     """
 
-    def __wrapper(func):
-        async def __trampoline(*args, **_):
+    def __wrapper(func: Callable) -> Optional[Callable]:
+        """decorator"""
+
+        async def __trampoline(*args: Tuple, **_: Mapping[Any, Any]) -> Tuple:
             """Tail call optimization."""
             while args.__class__ is tuple:
                 args = await func(*args)
             return args
 
         if active:
             functools.update_wrapper(__trampoline, func)
             return __trampoline
+        return None
 
     return __wrapper
```

### Comparing `blastpipe-0.4.26/meson.build` & `blastpipe-0.4.27/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/meson.options` & `blastpipe-0.4.27/meson.options`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             'pytest-tcpclient',
             'pytest-xdist'])
 option('args-bandit',
     description: 'application', type: 'array',
     value: ['--configfile', 'pyproject.toml', '--ignore-nosec', '-r', '@project_name@'])
 option('args-black',
     description: 'application', type: 'array', 
-    value: ['--verbose', '--check', '--diff', '--no-color', '--exclude', '.gitignore', '@project_name@'])
+    value: ['-S', '--verbose', '--check', '--diff', '--no-color', '--exclude', '.gitignore', '@project_name@'])
 option('args-isort',
     description: 'application', type: 'array', 
     value: ['-c', '@project_name@'])
 option('args-pylint',
     description: 'application', type: 'array', 
     value: ['@project_name@'])
 option('args-restructuredtext-lint',
```

### Comparing `blastpipe-0.4.26/pyproject.toml` & `blastpipe-0.4.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 git clean -dfX && \
                 tox && \
                 git stash -- PKG-INFO && \
                 git stash drop"""
 remove_dist                    = false
 repository                     = "pypi"
 tag_format                     = "{version}"
-upload_to_release              = false
+upload_to_release              = true
 upload_to_repository           = true
 use_textual_changelog_sections = true
 version_source                 = "tag_only"
 version_variable               = "PKG-INFO:Version: {version}"
 
 [tool.setuptools_scm]
 write_to_template = """
```

### Comparing `blastpipe-0.4.26/subprojects/dev.wrap` & `blastpipe-0.4.27/subprojects/dev.wrap`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/LICENSE.txt` & `blastpipe-0.4.27/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/_static/css/custom.css` & `blastpipe-0.4.27/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/_static/css/meson.build` & `blastpipe-0.4.27/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/_static/meson.build` & `blastpipe-0.4.27/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/_templates/layout.html` & `blastpipe-0.4.27/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/_templates/meson.build` & `blastpipe-0.4.27/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/conf.cfg` & `blastpipe-0.4.27/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/index.rst` & `blastpipe-0.4.27/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/meson.build` & `blastpipe-0.4.27/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/subprojects/docs/meson.options` & `blastpipe-0.4.27/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/tests/meson.build` & `blastpipe-0.4.27/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.26/tests/test_backports.py` & `blastpipe-0.4.27/tests/test_backports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: INP001
 """Tests for backported code."""
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
@@ -14,14 +15,15 @@
 # specific language governing permissions and limitations
 # under the License.
 import string
 
 from hypothesis import given
 from hypothesis import strategies as st
 
+# pylint: disable=import-error
 import blastpipe.backports
 
 
 # pylint: disable=invalid-name
 @given(instance=st.builds(string.Template, st.text()))
 def test_fuzz_TemplateGetIdentifiersMixin_extend_with(instance: string.Template) -> None:
     """Test extension of arbitrary :py:class:`string.Template` text.
```

### Comparing `blastpipe-0.4.26/tests/test_fuzz.py` & `blastpipe-0.4.27/tests/test_fuzz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: INP001
 """Mixin module tests."""
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
@@ -14,21 +15,24 @@
 # specific language governing permissions and limitations
 # under the License.
 import typing
 
 from hypothesis import given
 from hypothesis import strategies as st
 
+# pylint: disable=import-error
 import blastpipe.mixin
 import blastpipe.malloc
 import blastpipe.loop
 
 
 @st.composite
-def sized_objects(draw) -> typing.Tuple[st.SearchStrategy, ...]:
+def sized_objects(
+    draw: typing.Any,
+) -> typing.Tuple[st.SearchStrategy, ...]:
     """sized object strategy"""
     return (
         draw(st.binary()),
         draw(st.booleans()),
         draw(st.complex_numbers()),
         draw(st.datetimes()),
         draw(st.floats()),
@@ -58,19 +62,19 @@
     exc_types=st.tuples(st.just(Exception)),
     target=st.functions(),
     implicit_break=st.booleans(),
 )
 def test_fuzz_while_raised(
     exc_types: typing.Tuple[typing.Type[Exception]],
     target: typing.Callable,
-    implicit_break,
+    implicit_break: bool,
 ) -> None:
     """This test code was written by the `hypothesis.extra.ghostwriter` module"""
     blastpipe.loop.while_raised(
-        exc_types=exc_types, target=target, implicit_break=implicit_break
+        exc_types, target, implicit_break=implicit_break
     )
 
 
 @given(obj=sized_objects(), verbose=st.booleans())
-def test_fuzz_total_size(obj, verbose):
+def test_fuzz_total_size(obj: typing.Any, verbose: bool) -> None:
     """This test code was written by the `hypothesis.extra.ghostwriter` module"""
     blastpipe.malloc.total_size(obj=obj, handlers=None, verbose=verbose)
```

### Comparing `blastpipe-0.4.26/tests/test_tailcall.py` & `blastpipe-0.4.27/tests/test_tailcall.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: INP001
 """Tail call optimization tests"""
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
@@ -9,47 +10,50 @@
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+import typing
+
 import pytest
 from hypothesis import given
 from hypothesis import strategies as st
 
+# pylint: disable=import-error
 import blastpipe.sequence
 from blastpipe.sequence import chr_union
 
 
 @given(active=st.booleans())
-def test_fuzz_async_tail_call(active):
+def test_fuzz_async_tail_call(active: bool) -> None:
     """This test code was written by the `hypothesis.extra.ghostwriter` module"""
     blastpipe.sequence.async_tail_call(active=active)
 
 
-def test_chr_union_range():
+def test_chr_union_range() -> None:
     """Test chr_union with a range"""
-    assert chr_union((32, 35)) == {" ", "!", '"'}
-    assert chr_union(32) == {" "}
+    assert chr_union((32, 35)) == {' ', '!', '"'}
+    assert chr_union(32) == {' '}
 
 
 @st.composite
-def bad_input(draw):
+def bad_input(draw: typing.Any) -> typing.Tuple[st.SearchStrategy, ...]:
     """Test bad input for chr_union"""
     return (
         draw(st.lists(st.floats())),
         draw(st.lists(st.text())),
         draw(st.lists(st.functions())),
         draw(st.lists(st.booleans())),
         draw(st.floats()),
         draw(st.text()),
         draw(st.functions()),
         draw(st.booleans()),
     )
 
 
 @given(args=bad_input())
-def test_fuzz_bad_input_chr_union(args):
+def test_fuzz_bad_input_chr_union(args: typing.Tuple[typing.Any]) -> None:
     """Test bad input for chr_union"""
     with pytest.raises(TypeError):
         _ = chr_union(args)
```

