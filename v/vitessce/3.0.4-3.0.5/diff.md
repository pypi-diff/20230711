# Comparing `tmp/vitessce-3.0.4.tar.gz` & `tmp/vitessce-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitessce-3.0.4.tar", last modified: Mon Mar 27 17:18:50 2023, max compression
+gzip compressed data, was "vitessce-3.0.5.tar", last modified: Tue Jul 11 20:49:38 2023, max compression
```

## Comparing `vitessce-3.0.4.tar` & `vitessce-3.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 17:18:50.392510 vitessce-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-03-27 17:17:20.000000 vitessce-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      295 2023-03-27 17:17:20.000000 vitessce-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7874 2023-03-27 17:18:50.392510 vitessce-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5649 2023-03-27 17:17:20.000000 vitessce-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2023-03-27 17:17:20.000000 vitessce-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      558 2023-03-27 17:18:50.392510 vitessce-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-27 17:17:20.000000 vitessce-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 17:18:50.388510 vitessce-3.0.4/vitessce/
--rw-r--r--   0 runner    (1001) docker     (116)     1298 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    50062 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    13522 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 17:18:50.392510 vitessce-3.0.4/vitessce/data_utils/
--rw-r--r--   0 runner    (1001) docker     (116)      333 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10258 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/data_utils/anndata.py
--rw-r--r--   0 runner    (1001) docker     (116)    11665 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/data_utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (116)     9687 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/data_utils/multivec.py
--rw-r--r--   0 runner    (1001) docker     (116)     4904 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/data_utils/ome.py
--rw-r--r--   0 runner    (1001) docker     (116)     3842 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/export.py
--rw-r--r--   0 runner    (1001) docker     (116)     2287 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/repr.py
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/routes.py
--rw-r--r--   0 runner    (1001) docker     (116)    13961 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/widget.py
--rw-r--r--   0 runner    (1001) docker     (116)    31757 2023-03-27 17:17:20.000000 vitessce-3.0.4/vitessce/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 17:18:50.388510 vitessce-3.0.4/vitessce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7874 2023-03-27 17:18:50.000000 vitessce-3.0.4/vitessce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      533 2023-03-27 17:18:50.000000 vitessce-3.0.4/vitessce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-27 17:18:50.000000 vitessce-3.0.4/vitessce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      551 2023-03-27 17:18:50.000000 vitessce-3.0.4/vitessce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2023-03-27 17:18:50.000000 vitessce-3.0.4/vitessce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.423904 vitessce-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 20:47:35.000000 vitessce-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 20:47:35.000000 vitessce-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-11 20:49:38.423904 vitessce-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-11 20:47:35.000000 vitessce-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-11 20:47:35.000000 vitessce-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-11 20:49:38.423904 vitessce-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:47:35.000000 vitessce-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.419904 vitessce-3.0.5/vitessce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50062 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.423904 vitessce-3.0.5/vitessce/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/multivec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/ome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.419904 vitessce-3.0.5/vitessce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/top_level.txt
```

### Comparing `vitessce-3.0.4/LICENSE` & `vitessce-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/PKG-INFO` & `vitessce-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.0.4
+Version: 3.0.5
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vitessce-3.0.4/README.md` & `vitessce-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/pyproject.toml` & `vitessce-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel>=0.38.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vitessce"
-version = "3.0.4"
+version = "3.0.5"
 authors = [
   { name="Mark Keller", email="mark_keller@hms.harvard.edu" },
 ]
 description = "Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -56,15 +56,15 @@
   # nbconvert and jinja2 versions need to be pinned.
   # Reference: https://github.com/vitessce/vitessce-python/issues/152
   'nbconvert==5.6.1',
   'jinja2==3.0.3',
 ]
 all = [
   'jupyter-server-proxy>=1.5.2',
-  'anywidget==0.2.0',
+  'anywidget==0.4.2',
   'uvicorn>=0.17.0',
   'ujson>=4.0.1',
   'starlette==0.14.0',
   'generate-tiff-offsets>=0.1.7',
 
   # aiofiles is not explicitly referenced in our code,
   # but it is an implicit dependency of starlette==0.14.0.
```

### Comparing `vitessce-3.0.4/setup.cfg` & `vitessce-3.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/__init__.py` & `vitessce-3.0.5/vitessce/__init__.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/config.py` & `vitessce-3.0.5/vitessce/config.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/constants.py` & `vitessce-3.0.5/vitessce/constants.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/data_utils/anndata.py` & `vitessce-3.0.5/vitessce/data_utils/anndata.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,16 @@
             # uses the CSC sparse format.
             if not to_dense_X and not to_sparse_X:
                 # In the future, we can use sparse matrices with equal performance:
                 # https://github.com/theislab/anndata/issues/524
                 # Vitessce can use csc matrices somewhat efficiently.
                 if issparse(new_X):
                     new_X = new_X.tocsc()
+        else:
+            new_X = None
     else:
         new_X = None
     # Only keep the subset of columns required.
     if obs_cols is not None:
         new_obs = adata.obs[obs_cols]
     else:
         new_obs = adata.obs
```

### Comparing `vitessce-3.0.4/vitessce/data_utils/entities.py` & `vitessce-3.0.5/vitessce/data_utils/entities.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/data_utils/multivec.py` & `vitessce-3.0.5/vitessce/data_utils/multivec.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/data_utils/ome.py` & `vitessce-3.0.5/vitessce/data_utils/ome.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/export.py` & `vitessce-3.0.5/vitessce/export.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/repr.py` & `vitessce-3.0.5/vitessce/repr.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/routes.py` & `vitessce-3.0.5/vitessce/routes.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce/widget.py` & `vitessce-3.0.5/vitessce/widget.py`

 * *Files 21% similar despite different names*

```diff
@@ -144,17 +144,25 @@
         uid_str = str(uuid.uuid4())[:4]
     else:
         uid_str = uid
     return uid_str
 
 
 ESM = """
-import * as d3 from 'https://esm.sh/d3-require@1.3.0';
-import React from 'https://esm.sh/react@18.2.0';
-import ReactDOM from 'https://esm.sh/react-dom@18.2.0';
+import { importWithMap } from 'https://unpkg.com/dynamic-importmap@0.0.1';
+const importMap = {
+  imports: {
+    "react": "https://esm.sh/react@18.2.0?dev",
+    "react-dom": "https://esm.sh/react-dom@18.2.0?dev",
+    "react-dom/client": "https://esm.sh/react-dom@18.2.0/client?dev",
+  },
+};
+
+const React = await importWithMap("react", importMap);
+const { createRoot } = await importWithMap("react-dom/client", importMap);
 
 function asEsModule(component) {
   return {
     __esModule: true,
     default: component,
   };
 }
@@ -189,43 +197,34 @@
         ...f,
         url: `${origin}${baseUrl}${f.url}`,
       })),
     })),
   };
 }
 
-export function render(view) {
+export async function render(view) {
     const cssUid = view.model.get('uid');
+    const jsDevMode = view.model.get('js_dev_mode');
     const jsPackageVersion = view.model.get('js_package_version');
-    let customRequire = d3.require;
     const customJsUrl = view.model.get('custom_js_url');
-    if(customJsUrl.length > 0) {
-        customRequire = d3.requireFrom(async () => {
-            return customJsUrl;
-        });
-    }
 
-    const aliasedRequire = customRequire.alias({
-        "react": React,
-        "react-dom": ReactDOM
-    });
-
-    const Vitessce = React.lazy(() => {
-        // Workaround for preventing side effects due to loading the Vitessce UMD bundle twice
-        // running createGenerateClassNames twice.
-        // Alternate solution should be possible in JS release v2.0.3.
-        // Reference: https://github.com/vitessce/vitessce/pull/1391
-        return aliasedRequire(`vitessce@${jsPackageVersion}`)
-            .then(vitessce => asEsModule(vitessce.Vitessce));
-    });
+    const pkgName = (jsDevMode ? "@vitessce/dev" : "vitessce");
+
+    importMap.imports["vitessce"] = (customJsUrl.length > 0
+        ? customJsUrl
+        : `https://unpkg.com/${pkgName}@${jsPackageVersion}`
+    );
+
+    const { Vitessce } = await importWithMap("vitessce", importMap);
 
     function VitessceWidget(props) {
         const { model } = props;
 
-        const config = prependBaseUrl(model.get('config'), model.get('proxy'), model.get('has_host_name'));
+        const [config, setConfig] = React.useState(prependBaseUrl(model.get('config'), model.get('proxy'), model.get('has_host_name')));
+        const [validateConfig, setValidateConfig] = React.useState(true);
         const height = model.get('height');
         const theme = model.get('theme') === 'auto' ? (prefersDark ? 'dark' : 'light') : model.get('theme');
 
         const divRef = React.useRef();
 
         React.useEffect(() => {
             if(!divRef.current) {
@@ -252,29 +251,63 @@
                 if(divRef.current) {
                     divRef.current.removeEventListener("mouseenter", handleMouseEnter);
                     divRef.current.removeEventListener("mouseleave", handleMouseLeave);
                 }
             };
         }, [divRef]);
 
+        // Config changed on JS side (from within <Vitessce/>),
+        // send updated config to Python side.
         const onConfigChange = React.useCallback((config) => {
             model.set('config', config);
+            setValidateConfig(false);
             model.save_changes();
         }, [model]);
 
-        const vitessceProps = { height, theme, config, onConfigChange, uid: cssUid };
+        // Config changed on Python side,
+        // pass to <Vitessce/> component to it is updated on JS side.
+        React.useEffect(() => {
+            model.on('change:config', () => {
+                const newConfig = prependBaseUrl(model.get('config'), model.get('proxy'), model.get('has_host_name'));
+
+                // Force a re-render and re-validation by setting a new config.uid value.
+                // TODO: make this conditional on a parameter from Python.
+                //newConfig.uid = `random-${Math.random()}`;
+                //console.log('newConfig', newConfig);
+                setConfig(newConfig);
+            });
+        }, []);
+
+        const vitessceProps = { height, theme, config, onConfigChange, validateConfig };
 
         return e('div', { ref: divRef, style: { height: height + 'px' } },
             e(React.Suspense, { fallback: e('div', {}, 'Loading...') },
-                e(Vitessce, vitessceProps)
-            )
+                e(React.StrictMode, {},
+                    e(Vitessce, vitessceProps)
+                ),
+            ),
         );
     }
 
-    ReactDOM.render(e(VitessceWidget, { model: view.model }), view.el);
+    const root = createRoot(view.el);
+    root.render(e(VitessceWidget, { model: view.model }));
+
+    return () => {
+        // Re-enable scrolling.
+        const jpn = view.el.closest('.jp-Notebook');
+        if(jpn) {
+            jpn.style.overflow = "auto";
+        }
+
+        // Clean up React and DOM state.
+        root.unmount();
+        if(view._isFromDisplay) {
+            view.el.remove();
+        }
+    };
 }
 """
 
 
 class VitessceWidget(anywidget.AnyWidget):
     """
     A class to represent a Jupyter widget for Vitessce.
@@ -290,18 +323,19 @@
     theme = Unicode('auto').tag(sync=True)
     proxy = Bool(False).tag(sync=True)
     uid = Unicode('').tag(sync=True)
     has_host_name = Bool(False).tag(sync=True)
 
     next_port = DEFAULT_PORT
 
-    js_package_version = Unicode('2.0.3').tag(sync=True)
+    js_package_version = Unicode('3.0.1').tag(sync=True)
+    js_dev_mode = Bool(False).tag(sync=True)
     custom_js_url = Unicode('').tag(sync=True)
 
-    def __init__(self, config, height=600, theme='auto', uid=None, port=None, proxy=False, js_package_version='2.0.3', custom_js_url=''):
+    def __init__(self, config, height=600, theme='auto', uid=None, port=None, proxy=False, js_package_version='3.0.1', js_dev_mode=False, custom_js_url=''):
         """
         Construct a new Vitessce widget.
 
         :param config: A view config instance.
         :type config: VitessceConfig
         :param str theme: The theme name, either "light" or "dark". By default, "auto", which selects light or dark based on operating system preferences.
         :param int height: The height of the widget, in pixels. By default, 600.
@@ -325,15 +359,15 @@
         config_dict = config.to_dict(base_url=base_url)
         routes = config.get_routes()
 
         uid_str = get_uid_str(uid)
 
         super(VitessceWidget, self).__init__(
             config=config_dict, height=height, theme=theme, proxy=proxy,
-            js_package_version=js_package_version, custom_js_url=custom_js_url,
+            js_package_version=js_package_version, js_dev_mode=js_dev_mode, custom_js_url=custom_js_url,
             uid=uid_str,
         )
 
         serve_routes(config, routes, use_port)
 
     def _get_coordination_value(self, coordination_type, coordination_scope):
         obj = self.config['coordinationSpace'][coordination_type]
@@ -361,49 +395,109 @@
     def close(self):
         self.config_obj.stop_server(self.port)
         super().close()
 
 # Launch Vitessce using plain HTML representation (no ipywidgets)
 
 
-def ipython_display(config, height=600, theme='auto', base_url=None, host_name=None, uid=None, port=None, proxy=False, js_package_version='2.0.3', custom_js_url=''):
+def ipython_display(config, height=600, theme='auto', base_url=None, host_name=None, uid=None, port=None, proxy=False, js_package_version='3.0.1', js_dev_mode=False, custom_js_url=''):
     from IPython.display import display, HTML
     uid_str = "vitessce" + get_uid_str(uid)
 
     base_url, use_port, _ = get_base_url_and_port(
         port, DEFAULT_PORT, proxy=proxy, base_url=base_url, host_name=host_name)
     config_dict = config.to_dict(base_url=base_url)
     routes = config.get_routes()
     serve_routes(config, routes, use_port)
 
     model_vals = {
         "uid": uid_str,
         "js_package_version": js_package_version,
+        "js_dev_mode": js_dev_mode,
         "custom_js_url": custom_js_url,
         "proxy": proxy,
         "has_host_name": host_name is not None,
         "height": height,
         "theme": theme,
         "config": config_dict,
     }
 
+    # We need to clean up the React and DOM state in any case in which
+    # .display() is being run in the same cell as a previous .display().
+    # Otherwise, React tries to diff the virtual DOM,
+    # causing the browser to become unresponsive.
+
+    # In the .widget() case, we return a cleanup function that anywidget runs for us.
+    # However, in the .display() case, we need to run do cleanup ourselves.
+    # However, using IPython.display, there is not bidirectional communication,
+    # so we cannot simply sent "events" or "messages" to previously rendered widgets
+    # to tell them to clean up. Instead, we need to store a reference to the wrapper
+    # div element on the window, scoped to the cell, for cleanup.
+
+    # There are two edge cases in which the user runs .display(), then .widget()
+    # or vice-versa, in the same cell -- we do not currently handle those,
+    # as this would require using the hack-y cleanup over the AnyWidget cleanup
+    # in all cases.
+
+    CLEANUP_STR = """
+        // Initialize the global Map if not yet defined.
+        if (!window.__VITESSCE_DISPLAY_CELLS__) {
+            window.__VITESSCE_DISPLAY_CELLS__ = new Map();
+        }
+
+        // Rename for readability.
+        const CELL_MAP = window.__VITESSCE_DISPLAY_CELLS__;
+
+        // Need cases for getting parent in plain notebook, colab, etc.
+        const potentialParents = [
+            nextWidgetEl.closest('.jp-Notebook-cell'), // JupyterLab
+            nextWidgetEl.closest('.cell'), // JupyterLab Classic Notebook
+        ];
+
+        // Get the cell's parent element.
+        const parentEl = potentialParents.find(potentialEl => potentialEl !== null);
+
+        if (parentEl) {
+            const prevCleanupFunctionPromise = CELL_MAP.get(parentEl);
+
+            if (prevCleanupFunctionPromise) {
+                const prevCleanupFunction = await prevCleanupFunctionPromise;
+                prevCleanupFunction();
+                CELL_MAP.set(parentEl, null);
+            }
+        }
+    """
+
     HTML_STR = f"""
         <div id="{uid_str}"></div>
 
         <script type="module">
 
+            const nextWidgetEl = document.getElementById("{uid_str}");
+
             """ + ESM + """
 
-            render({
+            """ + CLEANUP_STR + """
+
+            const nextCleanupFunction = render({
                 model: {
                     get: (key) => {
                         const vals = """ + json.dumps(model_vals) + """;
                         return vals[key];
                     },
                     set: () => {},
-                    save_changes: () => {}
+                    save_changes: () => {},
+                    on: () => {},
                 },
-                el: """ + f"""document.getElementById("{uid_str}")""" + """,
+                el: nextWidgetEl,
+                _isFromDisplay: true,
             });
+
+            // Store a reference to the widget div element on the window, scoped to the cell,
+            // for future cleanups to use.
+            if (parentEl) {
+                CELL_MAP.set(parentEl, nextCleanupFunction);
+            }
         </script>
     """
+
     display(HTML(HTML_STR))
```

### Comparing `vitessce-3.0.4/vitessce/wrappers.py` & `vitessce-3.0.5/vitessce/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -430,25 +430,27 @@
     Wrap an OME-NGFF Zarr store by creating an instance of the ``OmeZarrWrapper`` class.
 
     :param str img_path: A local filepath to an OME-NGFF Zarr store.
     :param str img_url: A remote URL of an OME-NGFF Zarr store.
     :param \\*\\*kwargs: Keyword arguments inherited from :class:`~vitessce.wrappers.AbstractWrapper`
     """
 
-    def __init__(self, img_path=None, img_url=None, **kwargs):
+    def __init__(self, img_path=None, img_url=None, name="", is_bitmask=False, **kwargs):
         super().__init__(**kwargs)
         self._repr = make_repr(locals())
         if img_url is not None and img_path is not None:
             raise ValueError(
                 "Did not expect img_path to be provided with img_url")
         if img_url is None and img_path is None:
             raise ValueError(
                 "Expected either img_url or img_path to be provided")
         self._img_path = img_path
         self._img_url = img_url
+        self.name = name
+        self.is_bitmask = is_bitmask
         if self._img_path is not None:
             self.is_remote = False
         else:
             self.is_remote = True
         self.local_dir_uid = str(uuid4())
 
     def convert_and_save(self, dataset_uid, obj_i, base_dir=None):
@@ -478,17 +480,37 @@
         def image_file_def_creator(base_url):
             return {
                 "fileType": "image.ome-zarr",
                 "url": self.get_img_url(base_url, dataset_uid, obj_i)
             }
         return image_file_def_creator
 
+    # The following two functions will be used when OmeZarrWrapper
+    # is used within MultiImageWrapper.
+    def make_image_def(self, dataset_uid, obj_i, base_url):
+        img_url = self.get_img_url(base_url, dataset_uid, obj_i)
+        return self.create_image_json(img_url)
+
+    def create_image_json(self, img_url):
+        metadata = {}
+        image = {
+            "name": self.name,
+            "type": "ome-zarr",
+            "url": img_url,
+        }
+        if self.is_bitmask:
+            metadata["isBitmask"] = self.is_bitmask
+        # Only attach metadata if there is some - otherwise schema validation fails.
+        if len(metadata.keys()) > 0:
+            image["metadata"] = metadata
+        return image
+
 
 class AnnDataWrapper(AbstractWrapper):
-    def __init__(self, adata_path=None, adata_url=None, obs_feature_matrix_path=None, feature_filter_path=None, initial_feature_filter_path=None, obs_set_paths=None, obs_set_names=None, obs_locations_path=None, obs_segmentations_path=None, obs_embedding_paths=None, obs_embedding_names=None, obs_embedding_dims=None, request_init=None, feature_labels_path=None, convert_to_dense=True, coordination_values=None, **kwargs):
+    def __init__(self, adata_path=None, adata_url=None, obs_feature_matrix_path=None, feature_filter_path=None, initial_feature_filter_path=None, obs_set_paths=None, obs_set_names=None, obs_locations_path=None, obs_segmentations_path=None, obs_embedding_paths=None, obs_embedding_names=None, obs_embedding_dims=None, request_init=None, feature_labels_path=None, obs_labels_path=None, convert_to_dense=True, coordination_values=None, **kwargs):
         """
         Wrap an AnnData object by creating an instance of the ``AnnDataWrapper`` class.
 
         :param str adata_path: A path to an AnnData object written to a Zarr store containing single-cell experiment data.
         :param str adata_url: A remote url pointing to a zarr-backed AnnData store.
         :param str obs_feature_matrix_path: Location of the expression (cell x gene) matrix, like `X` or `obsm/highly_variable_genes_subset`
         :param str feature_filter_path: A string like `var/highly_variable` used in conjunction with `obs_feature_matrix_path` if obs_feature_matrix_path points to a subset of `X` of the full `var` list.
@@ -497,15 +519,16 @@
         :param list[str] obs_set_names: Names to display in place of those in `obs_set_paths`, like `['Louvain', 'Cell Type']
         :param str obs_locations_path: Column name in `obsm` that contains centroid coordinates for displaying centroids in the spatial viewer
         :param str obs_segmentations_path: Column name in `obsm` that contains polygonal coordinates for displaying outlines in the spatial viewer
         :param list[str] obs_embedding_paths: Column names like `['obsm/X_umap', 'obsm/X_pca']` for showing scatterplots
         :param list[str] obs_embedding_names: Overriding names like `['UMAP', 'PCA'] for displaying above scatterplots
         :param list[str] obs_embedding_dims: Dimensions along which to get data for the scatterplot, like [[0, 1], [4, 5]] where [0, 1] is just the normal x and y but [4, 5] could be comparing the third and fourth principal components, for example.
         :param dict request_init: options to be passed along with every fetch request from the browser, like { "header": { "Authorization": "Bearer dsfjalsdfa1431" } }
-        :param str feature_labels_path: The name of a column containing gene names, instead of the default index in `var` of the AnnData store.
+        :param str feature_labels_path: The name of a column containing feature labels (e.g., alternate gene symbols), instead of the default index in `var` of the AnnData store.
+        :param str obs_labels_path: The name of a column containing observation labels (e.g., alternate cell IDs), instead of the default index in `obs` of the AnnData store.
         :param bool convert_to_dense: Whether or not to convert `X` to dense the zarr store (dense is faster but takes more disk space).
         :param coordination_values: Coordination values for the file definition.
         :type coordination_values: dict or None
         :param \\*\\*kwargs: Keyword arguments inherited from :class:`~vitessce.wrappers.AbstractWrapper`
         """
         super().__init__(**kwargs)
         self._repr = make_repr(locals())
@@ -532,14 +555,15 @@
         self._cell_set_obs = obs_set_paths
         self._spatial_centroid_obsm = obs_locations_path
         self._spatial_polygon_obsm = obs_segmentations_path
         self._mappings_obsm = obs_embedding_paths
         self._mappings_obsm_dims = obs_embedding_dims
         self._request_init = request_init
         self._gene_alias = feature_labels_path
+        self._obs_labels_path = obs_labels_path
         self._convert_to_dense = convert_to_dense
         self._coordination_values = coordination_values
 
     def convert_and_save(self, dataset_uid, obj_i, base_dir=None):
         # Only create out-directory if needed
         if not self.is_remote:
             super().convert_and_save(dataset_uid, obj_i, base_dir=base_dir)
@@ -610,18 +634,22 @@
                 options["obsFeatureMatrix"] = {
                     "path": self._expression_matrix
                 }
                 if self._gene_var_filter is not None:
                     options["obsFeatureMatrix"]["featureFilterPath"] = self._gene_var_filter
                 if self._matrix_gene_var_filter is not None:
                     options["obsFeatureMatrix"]["initialFeatureFilterPath"] = self._matrix_gene_var_filter
-                if self._gene_alias is not None:
-                    options["featureLabels"] = {
-                        "path": self._gene_alias
-                    }
+            if self._gene_alias is not None:
+                options["featureLabels"] = {
+                    "path": self._gene_alias
+                }
+            if self._obs_labels_path is not None:
+                options["obsLabels"] = {
+                    "path": self._obs_labels_path
+                }
             if len(options.keys()) > 0:
                 obj_file_def = {
                     "fileType": ft.ANNDATA_ZARR.value,
                     "url": self.get_zarr_url(base_url, dataset_uid, obj_i),
                     "options": options
                 }
                 if self._request_init is not None:
```

### Comparing `vitessce-3.0.4/vitessce.egg-info/PKG-INFO` & `vitessce-3.0.5/vitessce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.0.4
+Version: 3.0.5
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vitessce-3.0.4/vitessce.egg-info/SOURCES.txt` & `vitessce-3.0.5/vitessce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.4/vitessce.egg-info/requires.txt` & `vitessce-3.0.5/vitessce.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 numpy>=1.21.2
 anndata<0.9,>=0.7.8
 ome-zarr==0.2.1
 tifffile>=2020.10.1
 
 [all]
 jupyter-server-proxy>=1.5.2
-anywidget==0.2.0
+anywidget==0.4.2
 uvicorn>=0.17.0
 ujson>=4.0.1
 starlette==0.14.0
 generate-tiff-offsets>=0.1.7
 aiofiles>=0.6.0
 
 [building]
```

