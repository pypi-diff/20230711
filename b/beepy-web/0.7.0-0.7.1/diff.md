# Comparing `tmp/beepy_web-0.7.0.tar.gz` & `tmp/beepy_web-0.7.1.tar.gz`

## Comparing `beepy_web-0.7.0.tar` & `beepy_web-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.7.0/.python-version
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy.css
--rw-r--r--   0        0        0    13583 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy.js
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 beepy_web-0.7.0/dev-requirements.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.7.0/requirements.txt
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/__init__.py
--rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/attrs.py
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/children.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/context.py
--rwxr-xr-x   0        0        0     3713 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/dev.py
--rw-r--r--   0        0        0    28250 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/framework.py
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/listeners.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/router.py
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/style.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/tags.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/trackable.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/actions.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/modal.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/plot.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/table.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/tabs.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/api.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/common.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/dev.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/internal.py
--rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/js.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/js_py.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.7.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.7.0/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 beepy_web-0.7.0/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 beepy_web-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 beepy_web-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.7.1/.python-version
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy.css
+-rw-r--r--   0        0        0    13535 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy.js
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 beepy_web-0.7.1/dev-requirements.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.7.1/requirements.txt
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/__init__.py
+-rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/attrs.py
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/children.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/context.py
+-rwxr-xr-x   0        0        0     3713 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/dev.py
+-rw-r--r--   0        0        0    28250 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/framework.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/listeners.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/router.py
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/style.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/tags.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/trackable.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/modal.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/plot.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/table.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/api.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/common.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/js.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 beepy_web-0.7.1/beepy/utils/js_py.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 beepy_web-0.7.1/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 beepy_web-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 beepy_web-0.7.1/PKG-INFO
```

### Comparing `beepy_web-0.7.0/beepy.css` & `beepy_web-0.7.1/beepy.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy.js` & `beepy_web-0.7.1/beepy.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -315,32 +315,33 @@
         await _main({
             reload: true
         })
     }
 }
 
 async function _loadBeePyModule() {
-    await beepy.pip.install(`${beepy.config.path}/dist/beepy_web-0.7.0a1-py3-none-any.whl`)
-    // let version
-    // if (_src.indexOf('beepy.js') === -1) {
-    //     throw new Error('Invalid BeePy source! Cannot get version of framework')
-    // } else {
-    //     version = (new URL(_src)).searchParams.get('v')
-    //     if (version) {
-    //         if (version === 'latest') {
-    //             version = ''
-    //         } else {
-    //             version = `==${version}`
-    //         }
-    //     } else {
-    //         console.warn('No version specified in BeePy source! The latest will be used')
-    //         version = ''
-    //     }
-    // }
-    // await beepy.pip.install(`beepy_web${version}`)
+    let version
+    if (_src.indexOf('beepy.js') === -1) {
+        throw new Error('Invalid BeePy source! Cannot get version of framework')
+    } else {
+        version = (new URL(_src)).searchParams.get('v')
+        if (version) {
+            if (version === 'latest') {
+                version = ''
+            }
+        } else {
+            console.warn('No version specified in BeePy source! The latest will be used')
+            version = ''
+        }
+    }
+    try {
+        await beepy.pip.install(`beepy_web${(version ? '==' : '') + version}`)
+    } catch {
+        await beepy.pip.install(`${beepy.config.path}/dist/beepy_web-${version}-py3-none-any.whl`)
+    }
 
     beepy.globals = py(`
 import js
 from beepy import __version__
 from beepy.utils.internal import merge_configs, _BeePyGlobals
 js.console.log(f'%cBeePy version: {__version__}', 'color: lightgreen; font-size: 35px')
 merge_configs()
```

### Comparing `beepy_web-0.7.0/beepy/__init__.py` & `beepy_web-0.7.1/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/attrs.py` & `beepy_web-0.7.1/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/children.py` & `beepy_web-0.7.1/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/context.py` & `beepy_web-0.7.1/beepy/context.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/dev.py` & `beepy_web-0.7.1/beepy/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/framework.py` & `beepy_web-0.7.1/beepy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from beepy.utils import js, log, to_js, IN_BROWSER, __CONFIG__
 from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.context import OVERWRITE, SUPER, CONTENT, _SPECIAL_CHILD_STRINGS, _MetaContext, Context
 
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 __CONFIG__['version'] = __version__
 
 
 if IN_BROWSER:
     js.Element.__str__ = lambda self: f'<{self.tagName.lower()}/>'
 _current__lifecycle_method: dict[str, dict[int, 'Tag']] = {}
```

### Comparing `beepy_web-0.7.0/beepy/listeners.py` & `beepy_web-0.7.1/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/router.py` & `beepy_web-0.7.1/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/style.py` & `beepy_web-0.7.1/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/tags.py` & `beepy_web-0.7.1/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/trackable.py` & `beepy_web-0.7.1/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/types.py` & `beepy_web-0.7.1/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/modules/context_menu.py` & `beepy_web-0.7.1/beepy/modules/context_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import js
+from beepy.utils import js
 from beepy.framework import attr, state, on
 from beepy.style import Style
 from beepy.tags import div, hr, ul, li, Body
 
 
 class MenuDivider(hr):
     default_style = Style(
```

### Comparing `beepy_web-0.7.0/beepy/modules/local_storage.py` & `beepy_web-0.7.1/beepy/modules/local_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 from collections.abc import Mapping
 
-import js
+from beepy.utils import js
 
 
 class LocalStorage(Mapping):
     __slots__ = ('prefix',)
 
     def __init__(self, key: str):
         if not key.strip():
```

### Comparing `beepy_web-0.7.0/beepy/modules/modal.py` & `beepy_web-0.7.1/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/modules/table.py` & `beepy_web-0.7.1/beepy/modules/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/modules/tabs.py` & `beepy_web-0.7.1/beepy/modules/tabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
-
-import js
-
 from beepy.framework import Tag, attr, state
 from beepy.style import Style
 from beepy.attrs import html_attr
 from beepy.tags import div, ul
+from beepy.utils import js
 from beepy.utils.js_py import replace_url
 
 
 class tab(div, name='tab'):
     tab_id = state(type=str)
     visible = html_attr(False)
     title: tab_title = state()
```

### Comparing `beepy_web-0.7.0/beepy/utils/api.py` & `beepy_web-0.7.1/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/asyncio.py` & `beepy_web-0.7.1/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/common.py` & `beepy_web-0.7.1/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/dev.py` & `beepy_web-0.7.1/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/import_hooks.py` & `beepy_web-0.7.1/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/internal.py` & `beepy_web-0.7.1/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/js.py` & `beepy_web-0.7.1/beepy/utils/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/beepy/utils/js_py.py` & `beepy_web-0.7.1/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/.gitignore` & `beepy_web-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/LICENSE` & `beepy_web-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/README.md` & `beepy_web-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/pyproject.toml` & `beepy_web-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.7.0/PKG-INFO` & `beepy_web-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.7.0
+Version: 0.7.1
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

