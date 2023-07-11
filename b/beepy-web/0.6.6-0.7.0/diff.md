# Comparing `tmp/beepy_web-0.6.6.tar.gz` & `tmp/beepy_web-0.7.0.tar.gz`

## Comparing `beepy_web-0.6.6.tar` & `beepy_web-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,39 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.6.6/.python-version
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy.css
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy.js
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 beepy_web-0.6.6/dev-requirements.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.6.6/requirements.txt
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/actions.py
--rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/attrs.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/children.py
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/context.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/context_menu.py
--rwxr-xr-x   0        0        0     3665 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/dev.py
--rw-r--r--   0        0        0    28176 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/framework.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/import_hooks.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/init.py
--rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/js.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/listeners.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/local_storage.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/modal.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/plot.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/router.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/style.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/table.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/tabs.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/tags.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/trackable.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/types.py
--rw-r--r--   0        0        0    11659 2020-02-02 00:00:00.000000 beepy_web-0.6.6/beepy/utils.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.6.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.6.6/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 beepy_web-0.6.6/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 beepy_web-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 beepy_web-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.7.0/.python-version
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy.css
+-rw-r--r--   0        0        0    13583 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy.js
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 beepy_web-0.7.0/dev-requirements.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/__init__.py
+-rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/attrs.py
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/children.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/context.py
+-rwxr-xr-x   0        0        0     3713 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/dev.py
+-rw-r--r--   0        0        0    28250 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/framework.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/listeners.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/router.py
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/style.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/tags.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/trackable.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/modal.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/plot.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/table.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/api.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/common.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/js.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 beepy_web-0.7.0/beepy/utils/js_py.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 beepy_web-0.7.0/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 beepy_web-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 beepy_web-0.7.0/PKG-INFO
```

### Comparing `beepy_web-0.6.6/beepy.css` & `beepy_web-0.7.0/beepy.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/beepy.js` & `beepy_web-0.7.0/beepy.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -104,25 +104,21 @@
     }
 }
 
 const DEFAULT_CONFIG = {
     // user can specify version of pyodide
     // TODO: check supporting versions of pyodide
     pyodideVersion: '0.23.4',
-    // could be useful for some internal checks
-    __loading: false,
-    // extra modules in base dir to load
-    modules: [],
     requirements: [], // also could be function
 }
 
-// could be useful in the future, i.e: get attributes of <script src="beepy" />
+// useful for getting attributes of <script src="beepy" />
 beepy.script = document.currentScript
 const _src = beepy.script.src
-if (!beepy.config.path && _src.indexOf('beepy.js')) {
+if (!beepy.config.path && _src.indexOf('beepy.js') !== -1) {
     beepy.config.path = _src.substring(0, _src.indexOf('beepy.js') - 1).replace(/\/+$/, '')
 }
 
 const config = mergeDeep(DEFAULT_CONFIG, beepy.config)
 beepy.__CONFIG__ = config
 beepy.addElement = function addElement(mountPoint, elementName, options = {}) {
     const element = document.createElement(elementName, {
@@ -156,72 +152,46 @@
 
 
 // defining tools for running python
 
 const rootFolder = '__beepy_root__'
 
 beepy.loadFile = async function loadFile(filePath, {
-    _internal = false,
     checkPathExists = false
 } = {}, _method_head = false) {
-    if (!_internal) beepy.__CURRENT_LOADING_FILE__ = filePath
+    beepy.__CURRENT_LOADING_FILE__ = filePath
     if (!filePath.includes('http')) filePath = `${window.location.origin}/${filePath}`
-    if (checkPathExists && !(await beepy.loadFile(filePath, {
-            _internal
-        }, true)).ok) return '<'
+    if (checkPathExists && !(await beepy.loadFile(filePath, {}, true)).ok) return '<'
 
     const r = await fetch(filePath, {
         method: _method_head ? 'HEAD' : 'GET'
     })
     return _method_head ? r : await r.text()
 }
 
 beepy.loadFileSync = function loadFileSync(filePath, {
-    _internal = false,
     checkPathExists = false
 } = {}, _method_head = false) {
-    if (!_internal) beepy.__CURRENT_LOADING_FILE__ = filePath
+    beepy.__CURRENT_LOADING_FILE__ = filePath
     if (!filePath.includes('http')) filePath = `${window.location.origin}/${filePath}`
-    if (checkPathExists && beepy.loadFileSync(filePath, {
-            _internal
-        }, true).status !== 200) return '<'
+    if (checkPathExists && beepy.loadFileSync(filePath, {}, true).status !== 200) return '<'
 
     const req = new XMLHttpRequest()
     req.open(_method_head ? 'HEAD' : 'GET', filePath, false)
     req.send(null)
     return _method_head ? req : req.response
 }
 
-beepy._writeInternalFile = async function _writeInternalFile(file, content) {
-    if (!content) content = await beepy.loadFile(`${config.path}/beepy/${file}`, {
-        _internal: true
-    })
-    pyodide.FS.writeFile(`beepy/${file}`, content)
-}
-
-beepy._writeInternalFileSync = function _writeInternalFileSync(file, content) {
-    if (!content) content = beepy.loadFileSync(`${config.path}/beepy/${file}`, {
-        _internal: true
-    })
-    pyodide.FS.writeFile(`beepy/${file}`, content)
-}
-
 beepy._writeLocalFile = async function _writeLocalFile(file, content) {
-    if (file.substring(0, 6) === 'beepy/') return await beepy._writeInternalFile(file.substring(6), content)
-    if (!content) content = await beepy.loadFile(_lstrip(file), {
-        _internal: true
-    })
+    if (!content) content = await beepy.loadFile(_lstrip(file))
     pyodide.FS.writeFile(`${rootFolder}/${file}`, content)
 }
 
 beepy._writeLocalFileSync = function _writeLocalFileSync(file, content) {
-    if (file.substring(0, 6) === 'beepy/') return beepy._writeInternalFileSync(file.substring(6), content)
-    if (!content) content = beepy.loadFileSync(_lstrip(file), {
-        _internal: true
-    })
+    if (!content) content = beepy.loadFileSync(_lstrip(file))
     pyodide.FS.writeFile(`${rootFolder}/${file}`, content)
 }
 
 function _getGlobalsDict(options) {
     if (isObject(options)) {
         return {
             globals: options.globals || beepy.globals
@@ -296,100 +266,94 @@
 beepy.stopLoading = function stopLoading() {
     const loadingEl = document.getElementById('beepy-loading')
     if (!!loadingEl) loadingEl.remove()
 }
 
 window.__beepy_load = async () => {
     beepy.startLoading()
-    await Promise.all([systemLoad(), beepyLoad()])
-    window.removeEventListener('load', window.__beepy_load)
-}
-window.addEventListener('load', window.__beepy_load)
 
-async function systemLoad() {
     window.pyodide = await window.loadPyodide({
         indexURL
     })
+
+    pyodide.FS.mkdir(rootFolder)
+
     beepy.globals = pyodide.globals
     await pyodide.loadPackage('micropip')
+    beepy.pip = pyodide.pyimport('micropip')
+    console.log(pyodide._api.sys.version)
+
     let requirements = beepy.__CONFIG__.requirements
     if (!Array.isArray(requirements)) requirements = requirements()
-    await Promise.all(requirements.map(requirement => pyodide.loadPackage(requirement)))
-    beepy.__CONFIG__.__loading = true
 
+    await Promise.all([...requirements.map(beepy.pip.install), _loadDevServer(), _loadBeePyModule()])
+
+    window.removeEventListener('load', window.__beepy_load)
+}
+window.addEventListener('load', window.__beepy_load)
+
+beepy.DEV__hot_reload = false
+async function _loadDevServer() {
     try { // TODO: add flag parameter for this
         beepy.DEV__hot_reload_ws = new WebSocket('ws://localhost:8998/')
     } catch (e) {} // Dev Hot Reload server is not started
     beepy.DEV__hot_reload = !!beepy.DEV__hot_reload_ws
-    if (beepy.DEV__hot_reload) {
-        await apy('import importlib as _dev_importlib; import sys as _dev_sys')
-        beepy.DEV__hot_reload_ws.onmessage = async ({
-            data: file
-        }) => {
-            const data = beepy._filePathToModuleAndRealFileCache[file]
-            if (data) {
-                const [fileToWrite, module] = data
-                if (module) {
-                    await beepy._writeLocalFile(fileToWrite, await beepy.loadFile(file))
-                    await apy(`_dev_importlib.reload(_dev_sys.modules['${module}'])`)
-                }
+    if (!beepy.DEV__hot_reload) return
+
+    await apy('import importlib as _dev_importlib; import sys as _dev_sys')
+    beepy.DEV__hot_reload_ws.onmessage = async ({
+        data: file
+    }) => {
+        const data = beepy._filePathToModuleAndRealFileCache[file]
+        if (data) {
+            const [fileToWrite, module] = data
+            if (module) {
+                await beepy._writeLocalFile(fileToWrite, await beepy.loadFile(file))
+                await apy(`_dev_importlib.reload(_dev_sys.modules['${module}'])`)
             }
-            await apy(`_dev_importlib.reload(_dev_sys.modules['${rootFolder}'])`)
-            await _main({
-                reload: true
-            })
         }
+        await apy(`_dev_importlib.reload(_dev_sys.modules['${rootFolder}'])`)
+        await _main({
+            reload: true
+        })
     }
-
-    console.log(pyodide._api.sys.version)
 }
 
-async function beepyLoad() {
-    // load relative modules from beepy/__init__.py
-    const _init = await beepy.loadFile(`${config.path}/beepy/init.py`, {
-        _internal: true
-    })
-    const beepyModules = []
-    for (const match of _init.matchAll(/from beepy import (?<modules>.+)/g)) {
-        for (const module of match.groups.modules.split(/, ?/g)) {
-            beepyModules.push(`${module}.py`)
-        }
-    }
-    config.modules.unshift('__init__.py', ...beepyModules)
-
-    // TODO: create wheel and load beepy modules via pip
-    const contents = await Promise.all(
-        config.modules.map(file => beepy.loadFile(`${config.path}/beepy/${file === '__init__.py' ? 'init.py' : file}`, {
-            _internal: true
-        }))
-    )
-
-    while (beepy.__CONFIG__.__loading === false) {
-        await delay(100)
-    }
-    // pyodide loaded in systemLoad()
-
-    pyodide.FS.mkdir(rootFolder)
-    pyodide.FS.mkdir('beepy')
-    await Promise.all(config.modules.map((file, i) => beepy._writeInternalFile(file, contents[i])))
+async function _loadBeePyModule() {
+    await beepy.pip.install(`${beepy.config.path}/dist/beepy_web-0.7.0a1-py3-none-any.whl`)
+    // let version
+    // if (_src.indexOf('beepy.js') === -1) {
+    //     throw new Error('Invalid BeePy source! Cannot get version of framework')
+    // } else {
+    //     version = (new URL(_src)).searchParams.get('v')
+    //     if (version) {
+    //         if (version === 'latest') {
+    //             version = ''
+    //         } else {
+    //             version = `==${version}`
+    //         }
+    //     } else {
+    //         console.warn('No version specified in BeePy source! The latest will be used')
+    //         version = ''
+    //     }
+    // }
+    // await beepy.pip.install(`beepy_web${version}`)
 
     beepy.globals = py(`
 import js
 from beepy import __version__
-from beepy.utils import merge_configs, _BeePyGlobals
+from beepy.utils.internal import merge_configs, _BeePyGlobals
 js.console.log(f'%cBeePy version: {__version__}', 'color: lightgreen; font-size: 35px')
 merge_configs()
 
 del js, merge_configs
 _globals = _BeePyGlobals(globals())
 del _BeePyGlobals
 _globals # last evaluated value is returned from 'py' function
 `)
-
-    delete beepy.__CONFIG__.__loading
     await _main()
 }
 
 async function _main(options = {
     reload: false
 }) {
     beepy.__CURRENT_LOADING_FILE__ = ''
@@ -411,17 +375,16 @@
 
 
 function mkDirPath(path, removeFileName = false) {
     const pathParts = path.split('/')
     let maxLength = pathParts.length
     if (removeFileName) maxLength -= 1
 
-    for (let length = 0; length < maxLength; length++) {
-        let pathToCreate = pathParts.slice(0, length + 1).join('/')
-        if (!pathParts.includes('beepy')) pathToCreate = rootFolder + '/' + pathToCreate
+    for (let length = 1; length <= maxLength; length++) {
+        let pathToCreate = rootFolder + '/' + pathParts.slice(0, length).join('/')
         if (!pyodide.FS.analyzePath(pathToCreate).exists) pyodide.FS.mkdir(pathToCreate)
     }
 }
 
 
 function _parseAndMkDirFile(filePath, addCurrentPath = false, separator = '/') {
     let path = ''
```

### Comparing `beepy_web-0.6.6/beepy/__init__.py` & `beepy_web-0.7.0/beepy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-# This file is actually not imported in Frontend (due to some restrictions)
-
 try:
     from pyodide.ffi import IN_BROWSER
 except ImportError:
     try:
         from pyodide import IN_BROWSER
     except ImportError:
         print('Did you forget to install optional requirements with `pip install -U beepy-web[dev]`?')
         exit(1)
 
 if not IN_BROWSER:
     import sys
-    from . import js
+    from beepy.utils import js
 
     sys.modules['js'] = js
     del sys
 
-from beepy import local_storage, trackable, utils, types
-from beepy import listeners, attrs, children
-from beepy import context, framework, style, tags, actions, router, import_hooks
+import beepy.children  # must be loaded before .framework due to circular import
+import beepy.utils.import_hooks  # allows to use `import` for local files
 from beepy.tags import Head, Body
 from beepy.style import Style
 from beepy.context import *
 from beepy.context import __all__ as __context_all__
 from beepy.framework import *
 from beepy.framework import __version__, __all__ as __framework_all__
 
 __all__ = [
-    'local_storage', 'trackable', 'utils', 'types',
-    'listeners', 'attrs', 'children',
-    'context', 'framework', 'style', 'tags', 'actions', 'router', 'import_hooks',
-    'Head', 'Body', 'Style',
+    'Head',
+    'Body',
+    'Style',
     *__context_all__,
     *__framework_all__,
 ]
```

### Comparing `beepy_web-0.6.6/beepy/attrs.py` & `beepy_web-0.7.0/beepy/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import builtins
 import keyword
 from typing import Optional, Callable, Union, Sequence, Type, get_type_hints, ForwardRef, TypeVar, Any
 from collections import defaultdict
 
 from beepy.types import AttrType, AttrValue
-from beepy.utils import log, NONE_TYPE, wraps_with_name, to_kebab_case
+from beepy.utils.common import NONE_TYPE, wraps_with_name, to_kebab_case
+from beepy.utils import log
 
 
 Context = ForwardRef('Context')
 T = TypeVar('T')
 
 SPECIAL_CONVERT_ATTRIBUTES = {
     'contenteditable': lambda tag, val: (
```

### Comparing `beepy_web-0.6.6/beepy/children.py` & `beepy_web-0.7.0/beepy/children.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Optional, Callable, Union, Type, TypeVar, Generic, Iterable
 
-import js
-
 import beepy
 from beepy.types import Tag, Renderer, WebBase, Children, ContentType
 from beepy.context import Context
-from beepy.utils import log, _PY_TAG_ATTRIBUTE
+from beepy.utils import js, log
+from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 
 
 class CustomWrapper(WebBase):
     pass
 
 
 class StringWrapper(CustomWrapper):
```

### Comparing `beepy_web-0.6.6/beepy/context.py` & `beepy_web-0.7.0/beepy/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 from abc import ABCMeta
 from typing import Union, Type, TypeVar
 
-import js
 import beepy
 
 from beepy.attrs import attr
 from beepy.types import AttrType
-from beepy.utils import log10_ceil, get_random_name, const_attribute, Interval, to_kebab_case, create_once_callable
+from beepy.utils import js
+from beepy.utils.dev import const_attribute
+from beepy.utils.common import log10_ceil, get_random_name, to_kebab_case
+from beepy.utils.js_py import create_once_callable, Interval
 
 
 __obj = object()
 _base_obj_dir = tuple(dir(__obj)) + ('__abstractmethods__',)
 
 
 Self = TypeVar('Self', bound='Context')
```

### Comparing `beepy_web-0.6.6/beepy/context_menu.py` & `beepy_web-0.7.0/beepy/modules/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/beepy/dev.py` & `beepy_web-0.7.0/beepy/dev.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         for ws in self.websockets[:]:
             try:
                 await ws.send(message)
             except ConnectionClosedOK:
                 self.websockets.remove(ws)
 
         if not self.websockets:
-            print('No clients connected! Please, restart your page to connect to the dev server')
+            print('[BeePy] No clients connected! Please, restart your page to connect to the dev server')
 
     def handle_file_event(self, event):
         path = event.src_path
         if (
             event.is_directory
             or event.src_path.endswith(('~', '.tmp'))
             or '/__pycache__/' in path
@@ -52,23 +52,23 @@
             return
 
         if path.startswith(self.root_path):
             path = path[len(self.root_path): ]
         if path.startswith('/'):
             path = path[1:]
 
-        print(f'Found file change: {path}')
+        print(f'[BeePy] Found file change: {path}')
         asyncio.run(self.ws_send(path))
 
     def _watcher_start(self):
 
         event_handler = MonitorFolder(self)
         observer = Observer()
         observer.schedule(event_handler, path=self.root_path, recursive=True)
-        print(f'Monitoring started for {self.root_path}')
+        print(f'[BeePy] Monitoring started for {self.root_path}')
         observer.start()
         self.observer = observer
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt:
             observer.stop()
@@ -77,31 +77,31 @@
     async def _ws_echo(self, websocket):
         self.websockets.append(websocket)
 
         async for message in websocket:
             print(f'{websocket=} {message=}')  # We really don't receive messages
 
     async def _ws_main(self):
-        print('WebSockets started')
+        print('[BeePy] WebSockets started')
         async with serve(self._ws_echo, 'localhost', 8998):
             await asyncio.Future()  # run forever
 
     def _ws_start(self):
         asyncio.run(self._ws_main())
 
     def _simple_http_start(self, port=8888):
         with socketserver.TCPServer(
             ('', port), functools.partial(http.server.SimpleHTTPRequestHandler, directory=self.root_path)
         ) as httpd:
-            print(f'Serving at port {port}\nOpen server: http://localhost:{port}')
+            print(f'[BeePy] Serving at port {port}\nOpen server: http://localhost:{port}')
             httpd.serve_forever()
 
     def start(self, start_http=None, root_path=None, wait=False):
         if self.observer is not None:
-            print('Server is already started')
+            print('[BeePy] Server is already started')
             return
 
         if root_path is None:
             root_path = sys.argv[1] if len(sys.argv) > 1 else os.getcwd()
 
         self.root_path = root_path
```

### Comparing `beepy_web-0.6.6/beepy/framework.py` & `beepy_web-0.7.0/beepy/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 import traceback
 from collections import defaultdict
 from typing import Union, Callable, Type, Any, Iterable, Optional
 from types import MethodType
 from functools import wraps, partial, cache
 from copy import deepcopy
 
-import js
-
 from beepy.attrs import attr, set_html_attribute, state, html_attr
 from beepy.children import CustomWrapper, StringWrapper, ContentWrapper, ChildRef, TagRef, Children
 from beepy.listeners import on
 from beepy.types import safe_html, Renderer, Mounter, WebBase, AttrType, ContentType
-from beepy.utils import (
-    log, NONE_TYPE, _PY_TAG_ATTRIBUTE, __CONFIG__, _debugger, get_random_name, to_kebab_case, IN_BROWSER, to_js
-)
+from beepy.utils import js, log, to_js, IN_BROWSER, __CONFIG__
+from beepy.utils.internal import _PY_TAG_ATTRIBUTE
+from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
+from beepy.utils.dev import _debugger
 from beepy.context import OVERWRITE, SUPER, CONTENT, _SPECIAL_CHILD_STRINGS, _MetaContext, Context
 
 
-__version__ = '0.6.6'
+__version__ = '0.7.0'
 __CONFIG__['version'] = __version__
 
 
 if IN_BROWSER:
     js.Element.__str__ = lambda self: f'<{self.tagName.lower()}/>'
 _current__lifecycle_method: dict[str, dict[int, 'Tag']] = {}
```

### Comparing `beepy_web-0.6.6/beepy/import_hooks.py` & `beepy_web-0.7.0/beepy/utils/import_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import sys
 
 from importlib.abc import MetaPathFinder
 from importlib.util import spec_from_file_location
 
-import js
-from beepy.utils import IN_BROWSER, __CONFIG__, _debugger
+from beepy.utils.js_py import js, IN_BROWSER
+from beepy.utils.internal import __CONFIG__
+from beepy.utils.dev import _debugger
 
 
 BEEPY_ROOT_PACKAGE = '__beepy_root__'
 requirements = __CONFIG__['requirements']
 MODULES_NOT_EXISTING_ON_SERVER = [
     BEEPY_ROOT_PACKAGE,
     *(requirements() if callable(requirements) else requirements),
     '_hashlib',
     '_strptime',
     'unicodedata',
     'pprint',
 ]
 # some modules must be ignored to prevent load it from local server, when importing modules like micropip or datetime
-# TODO: move this hook higher to support importing `beepy/__init__.py` natively
 
 
 class ServerFinder(MetaPathFinder):
     def find_spec(self, fullname, path, target=None):
         if path and any(p.startswith('/lib') for p in path):
             return
```

### Comparing `beepy_web-0.6.6/beepy/js.py` & `beepy_web-0.7.0/beepy/utils/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/beepy/listeners.py` & `beepy_web-0.7.0/beepy/listeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import inspect
 from typing import Optional, Any, Callable
 from types import MethodType
 from functools import partial, wraps
 from copy import deepcopy
 
-import js
-
 from beepy.types import Tag
-from beepy.utils import _PY_TAG_ATTRIBUTE, create_proxy, to_js
+from beepy.utils import js, to_js
+from beepy.utils.js_py import create_proxy
+from beepy.utils.internal import _PY_TAG_ATTRIBUTE
+
 
 GLOBAL_EVENTS_LIST = ('keyup', 'keypress', 'keydown')
 _key_codes = {
     'esc': (27,),
     'tab': (9,),
     'enter': (13,),
     'space': (32,),
```

### Comparing `beepy_web-0.6.6/beepy/local_storage.py` & `beepy_web-0.7.0/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/beepy/modal.py` & `beepy_web-0.7.0/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/beepy/router.py` & `beepy_web-0.7.0/beepy/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import re
 from re import Match
 from typing import Union, Type
 from dataclasses import dataclass
 
-import js
-
 from beepy.framework import Tag, state, on
 from beepy.tags import a
 from beepy.types import Children
-from beepy.utils import lazy_import_cls, _debugger, push_url, reload_requirements, add_event_listener, force_sync
+from beepy.utils import js, force_sync
+from beepy.utils.js_py import add_event_listener, push_url
+from beepy.utils.dev import _debugger
+from beepy.utils.internal import lazy_import_cls, reload_requirements
 
 
 class WithRouter:
     match: Match = state(move_on=True)
     router: Router = state(move_on=True)
```

### Comparing `beepy_web-0.6.6/beepy/style.py` & `beepy_web-0.7.0/beepy/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 from typing import Any, Optional, Type
 
-import js
-
 from beepy.framework import __CONFIG__, Tag, attr, state
-from beepy.utils import log10_ceil, get_random_name, to_kebab_case, safe_issubclass
+from beepy.utils import js
+from beepy.utils.common import log10_ceil, get_random_name, to_kebab_case, safe_issubclass
 from beepy.tags import Head
 from beepy.types import safe_html
 
 
 def dict_of_properties_to_css(properties):
     for prop, value in properties.items():
         if not prop:
```

### Comparing `beepy_web-0.6.6/beepy/table.py` & `beepy_web-0.7.0/beepy/modules/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TypeVar, Type, Literal, Union
 
 from beepy.attrs import state
 from beepy.children import Children
 from beepy.tags import table, thead, tbody, tr, th, td
 from beepy.style import Style
 from beepy.listeners import on
-from beepy.actions import Action
+from beepy.modules.actions import Action
 
 
 T = TypeVar('T')
 
 
 class TableCellAction(Action, _root=True):
     components: dict[str, Type[TableCellAction]] = {}
```

### Comparing `beepy_web-0.6.6/beepy/tabs.py` & `beepy_web-0.7.0/beepy/modules/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import js
 
 from beepy.framework import Tag, attr, state
 from beepy.style import Style
 from beepy.attrs import html_attr
 from beepy.tags import div, ul
-from beepy.utils import replace_url
+from beepy.utils.js_py import replace_url
 
 
 class tab(div, name='tab'):
     tab_id = state(type=str)
     visible = html_attr(False)
     title: tab_title = state()
 
@@ -149,10 +149,11 @@
             url.href = url.href[:-1]
         if url.searchParams.get(self.name) == selected_tab.tab_id:
             return
 
         url.searchParams.set(self.name, selected_tab.tab_id)  # modifies url.href
 
         replace_url(url, name=selected_tab.id, title=''.join(getattr(self.tabs_titles, selected_tab.tab_id).content()))
+        print(f'URL replaced to {url} for {selected_tab} [3]')
 
 
 __all__ = ['tab', 'tab_title', 'tabs']
```

### Comparing `beepy_web-0.6.6/beepy/tags.py` & `beepy_web-0.7.0/beepy/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Optional
 
-import js
-
 from beepy.framework import Tag
 from beepy.attrs import attr, state, html_attr
 from beepy.children import Children
-from beepy.utils import get_random_name, __CONFIG__, AnyOfType
+from beepy.utils import js, __CONFIG__
+from beepy.utils.common import get_random_name, AnyOfType
 
 
 AUTO_ID = object()
 
 
 class html_tag(Tag, _root=True, content_tag=None):
     contenteditable = html_attr(type=bool)
```

### Comparing `beepy_web-0.6.6/beepy/trackable.py` & `beepy_web-0.7.0/beepy/trackable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Union, SupportsIndex, Callable
 
-from beepy.utils import Locker
+from beepy.utils.common import Locker
 
 
 class Trackable(ABC):
     __slots__ = ()
 
     onchange_triggers: list[Callable]
```

### Comparing `beepy_web-0.6.6/beepy/types.py` & `beepy_web-0.7.0/beepy/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
-import js
-
 from abc import ABC, abstractmethod
 from typing import Optional, Union, Iterable, ForwardRef
 from functools import wraps
 
 import beepy
 from beepy.trackable import TrackableList
-from beepy.utils import __CONFIG__, escape_html
-
+from beepy.utils import js, __CONFIG__
+from beepy.utils.common import escape_html
 
 attr = ForwardRef('attr')
 Tag = ForwardRef('Tag')
 ChildrenRef = ForwardRef('ChildrenRef')
 
 
 class AttrValue:
```

### Comparing `beepy_web-0.6.6/.gitignore` & `beepy_web-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/LICENSE` & `beepy_web-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/README.md` & `beepy_web-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/pyproject.toml` & `beepy_web-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.6/PKG-INFO` & `beepy_web-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.6.6
+Version: 0.7.0
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

