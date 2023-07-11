# Comparing `tmp/mizdb-tomselect-0.3.4.tar.gz` & `tmp/mizdb-tomselect-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb-tomselect-0.3.4.tar", last modified: Mon Jul  3 10:08:20 2023, max compression
+gzip compressed data, was "mizdb-tomselect-0.4.0.tar", last modified: Tue Jul 11 07:58:35 2023, max compression
```

## Comparing `mizdb-tomselect-0.3.4.tar` & `mizdb-tomselect-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/
--rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.4/LICENSE
--rw-r--r--   0 philip    (1000) philip    (1000)    10852 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)    10450 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/README.md
--rw-r--r--   0 philip    (1000) philip    (1000)     1601 2023-07-03 10:07:10.000000 mizdb-tomselect-0.3.4/pyproject.toml
--rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/setup.cfg
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.069904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/
--rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/__init__.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.070904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/css/
--rw-r--r--   0 philip    (1000) philip    (1000)      430 2023-07-03 10:03:55.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.070904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/js/
--rw-r--r--   0 philip    (1000) philip    (1000)   145719 2023-07-03 10:08:17.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.068904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.071904 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/
--rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-r--r--   0 philip    (1000) philip    (1000)     4366 2023-07-03 10:03:55.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     6229 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect/widgets.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.070904 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/
--rw-r--r--   0 philip    (1000) philip    (1000)    10852 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)      672 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/SOURCES.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/dependency_links.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/requires.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-07-03 10:08:20.000000 mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/top_level.txt
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-03 10:08:20.072904 mizdb-tomselect-0.3.4/tests/
--rw-r--r--   0 philip    (1000) philip    (1000)    14349 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/tests/test_e2e.py
--rw-r--r--   0 philip    (1000) philip    (1000)    16008 2023-07-03 10:03:55.000000 mizdb-tomselect-0.3.4/tests/test_views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     5000 2023-07-03 07:14:50.000000 mizdb-tomselect-0.3.4/tests/test_widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.865120 mizdb-tomselect-0.4.0/
+-rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.4.0/LICENSE
+-rw-r--r--   0 philip    (1000) philip    (1000)    11359 2023-07-11 07:58:35.865120 mizdb-tomselect-0.4.0/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)    10957 2023-07-11 06:57:55.000000 mizdb-tomselect-0.4.0/README.md
+-rw-r--r--   0 philip    (1000) philip    (1000)     1601 2023-07-11 07:57:19.000000 mizdb-tomselect-0.4.0/pyproject.toml
+-rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-07-11 07:58:35.865120 mizdb-tomselect-0.4.0/setup.cfg
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.860120 mizdb-tomselect-0.4.0/src/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.862120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/
+-rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/__init__.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.863120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)      647 2023-07-11 07:06:00.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.863120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/js/
+-rw-r--r--   0 philip    (1000) philip    (1000)   148177 2023-07-11 07:58:33.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.861120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.864120 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-r--r--   0 philip    (1000) philip    (1000)     4366 2023-07-04 08:10:45.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     6645 2023-07-04 09:47:30.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect/widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.863120 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/
+-rw-r--r--   0 philip    (1000) philip    (1000)    11359 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)      654 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/SOURCES.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/dependency_links.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/requires.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-07-11 07:58:35.000000 mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/top_level.txt
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 07:58:35.864120 mizdb-tomselect-0.4.0/tests/
+-rw-r--r--   0 philip    (1000) philip    (1000)    16516 2023-07-11 06:57:55.000000 mizdb-tomselect-0.4.0/tests/test_views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     5647 2023-07-11 06:57:55.000000 mizdb-tomselect-0.4.0/tests/test_widgets.py
```

### Comparing `mizdb-tomselect-0.3.4/LICENSE` & `mizdb-tomselect-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.4/PKG-INFO` & `mizdb-tomselect-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.4
+Version: 0.4.0
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -23,18 +23,18 @@
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
   * [Function & Features](#function--features)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
+    * [Inline edit link](#inline-edit-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
-
 ----
 
 ## Installation
 
 Install:
 ```bash
 pip install -U mizdb-tomselect
@@ -136,14 +136,15 @@
 | value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
 | label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
 | search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
 | create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
 | multiple       | False                                  | if True, allow selecting multiple options                                                      |
 | changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
 | add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
+| edit_url       |                                        | URL name of the edit view for this model([see below](#inline-edit-link))                       |
 | filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
 
 This widget displays the results in tabular form. A table header will be added
@@ -243,14 +244,28 @@
     path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
 widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
 
+### Inline edit link
+
+Provide a `edit_url` to attach a link to the edit/change page for each selected item.
+```python
+# urls.py
+urlpatterns = [
+    ...
+    path('city/edit/<path:object_id>/', CityChangeView.as_view(), name='city_change'),
+]
+
+# forms.py
+widget = MIZSelect(City, edit_url='city_change')
+```
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
 class Person(models.Model):
```

### Comparing `mizdb-tomselect-0.3.4/README.md` & `mizdb-tomselect-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
   * [Function & Features](#function--features)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
+    * [Inline edit link](#inline-edit-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
-
 ----
 
 ## Installation
 
 Install:
 ```bash
 pip install -U mizdb-tomselect
@@ -124,14 +124,15 @@
 | value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
 | label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
 | search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
 | create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
 | multiple       | False                                  | if True, allow selecting multiple options                                                      |
 | changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
 | add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
+| edit_url       |                                        | URL name of the edit view for this model([see below](#inline-edit-link))                       |
 | filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
 
 This widget displays the results in tabular form. A table header will be added
@@ -231,14 +232,28 @@
     path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
 widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
 
+### Inline edit link
+
+Provide a `edit_url` to attach a link to the edit/change page for each selected item.
+```python
+# urls.py
+urlpatterns = [
+    ...
+    path('city/edit/<path:object_id>/', CityChangeView.as_view(), name='city_change'),
+]
+
+# forms.py
+widget = MIZSelect(City, edit_url='city_change')
+```
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
 class Person(models.Model):
```

### Comparing `mizdb-tomselect-0.3.4/pyproject.toml` & `mizdb-tomselect-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mizdb-tomselect"
-version = "0.3.4"
+version = "0.4.0"
 authors = [
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using TomSelect"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4273,20 +4273,76 @@
                     return;
                 loading_more = true;
                 self2.load.call(self2, self2.lastValue);
             });
         });
     }
 
+    // client/plugins/edit_button.js
+    var getDom2 = (query) => {
+        if (query.jquery) {
+            return query[0];
+        }
+        if (query instanceof HTMLElement) {
+            return query;
+        }
+        if (isHtmlString2(query)) {
+            const tpl = document.createElement("template");
+            tpl.innerHTML = query.trim();
+            return tpl.content.firstChild;
+        }
+        return document.querySelector(query);
+    };
+    var isHtmlString2 = (arg) => {
+        if (typeof arg === "string" && arg.indexOf("<") > -1) {
+            return true;
+        }
+        return false;
+    };
+
+    function edit_button_default(userOptions) {
+        const options = Object.assign({
+            label: '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit-3 text-success"><path d="M12 20h9"></path><path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"></path></svg>',
+            title: "Bearbeiten",
+            className: "edit",
+            editUrl: "",
+            editUrlPlaceholder: "{pk}",
+            getEditUrl: (pluginOptions, item, value) => {
+                return pluginOptions.editUrl.replace(pluginOptions.editUrlPlaceholder, value);
+            }
+        }, userOptions);
+        if (!options.editUrl)
+            return;
+        const html = `<a class="${options.className}" title="${options.title}" target="_blank">${options.label}</a>`;
+        this.hook("after", "setupTemplates", () => {
+            const orig = this.settings.render.item;
+            this.settings.render.item = (data, escape) => {
+                const item = getDom2(orig.call(this, data, escape));
+                const editButton = getDom2(html);
+                editButton.addEventListener("click", (e) => {
+                    e.stopPropagation();
+                });
+                this.on("item_add", (value, _item) => {
+                    if (item === _item) {
+                        editButton.href = options.getEditUrl(options, item, value);
+                    }
+                });
+                item.appendChild(editButton);
+                return item;
+            };
+        });
+    }
+
     // client/mizselect.js
     TomSelect.define("clear_button", plugin_default);
     TomSelect.define("dropdown_header", plugin_default2);
     TomSelect.define("dropdown_input", plugin_default3);
     TomSelect.define("remove_button", plugin_default4);
     TomSelect.define("virtual_scroll", plugin_default5);
+    TomSelect.define("edit_button", edit_button_default);
 
     function getFormPrefix(elem) {
         const parts = elem.getAttribute("name").split("-").slice(0, -1);
         if (parts.length) {
             return parts.join("-") + "-";
         }
         return "";
@@ -4361,22 +4417,27 @@
             },
             plugins: getPlugins(elem),
             render: getRenderTemplates(elem)
         };
     }
 
     function getPlugins(elem) {
+        const removeImage = '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x text-danger"><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg>';
         const plugins = {
             dropdown_input: null,
-            virtual_scroll: null
+            virtual_scroll: null,
+            edit_button: {
+                editUrl: elem.dataset.editUrl
+            },
+            remove_button: {
+                title: "Entfernen",
+                label: removeImage
+            }
         };
         if (elem.hasAttribute("is-multiple")) {
-            plugins.remove_button = {
-                title: "Entfernen"
-            };
             plugins.clear_button = {
                 title: "Auswahl aufheben"
             };
         }
         if (elem.hasAttribute("is-tabular")) {
             plugins.dropdown_header = {
                 html: function(settings) {
```

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect/views.py` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect/views.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect/widgets.py` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect/widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from urllib.parse import unquote
 
 from django import forms
 from django.urls import reverse
 
 
 class MIZSelect(forms.Select):
     """
@@ -19,14 +20,15 @@
         value_field="",
         label_field="",
         search_lookup="",
         create_field="",
         multiple=False,
         changelist_url="",
         add_url="",
+        edit_url="",
         filter_by=(),
         **kwargs,
     ):
         """
         Instantiate a MIZSelect widget.
 
         Args:
@@ -41,16 +43,17 @@
               value of the model's `name_field` attribute. If the model has no
               `name_field` attribute, it defaults to 'name'.
             search_lookup: a Django field lookup to use with the given search
               term to filter the results
             create_field: the name of the model field used to create new
               model objects with
             multiple: if True, allow selecting multiple options
-            changelist_url: URL name of the changelist view for this model
-            add_url: URL name of the add view for this model
+            changelist_url: URL name of the 'changelist' view for this model
+            add_url: URL name of the 'add' view for this model
+            edit_url: URL name of the 'change' view for this model
             filter_by: a 2-tuple (form_field_name, field_lookup) to filter the
               results against the value of the form field using the given
               Django field lookup. For example:
                ('foo', 'bar__id') => results.filter(bar__id=data['foo'])
             kwargs: additional keyword arguments passed to forms.Select
         """
         self.model = model
@@ -58,31 +61,37 @@
         self.value_field = value_field or self.model._meta.pk.name
         self.label_field = label_field or getattr(self.model, "name_field", "name")
         self.search_lookup = search_lookup or f"{self.label_field}__icontains"
         self.create_field = create_field
         self.multiple = multiple
         self.changelist_url = changelist_url
         self.add_url = add_url
+        self.edit_url = edit_url
         self.filter_by = filter_by
         super().__init__(**kwargs)
 
     def optgroups(self, name, value, attrs=None):
         return []  # Never provide any options; let the view serve the options.
 
     def get_url(self):
         """Hook to specify the autocomplete URL."""
         return reverse(self.url)
 
     def get_add_url(self):
-        """Hook to specify the URL to the model's add page."""
+        """Hook to specify the URL to the model's 'add' page."""
         if self.add_url:
             return reverse(self.add_url)
 
+    def get_edit_url(self):
+        """Hook to specify the URL to the model's 'change' page."""
+        if self.edit_url:
+            return unquote(reverse(self.edit_url, args=["{pk}"]))
+
     def get_changelist_url(self):
-        """Hook to specify the URL the model's changelist."""
+        """Hook to specify the URL the model's 'changelist' page."""
         if self.changelist_url:
             return reverse(self.changelist_url)
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         """Build HTML attributes for the widget."""
         attrs = super().build_attrs(base_attrs, extra_attrs)
         opts = self.model._meta
@@ -94,14 +103,15 @@
                 "data-model": f"{opts.app_label}.{opts.model_name}",
                 "data-search-lookup": self.search_lookup,
                 "data-value-field": self.value_field,
                 "data-label-field": self.label_field,
                 "data-create-field": self.create_field,
                 "data-changelist-url": self.get_changelist_url() or "",
                 "data-add-url": self.get_add_url() or "",
+                "data-edit-url": self.get_edit_url() or "",
                 "data-filter-by": json.dumps(list(self.filter_by)),
             }
         )
         return attrs
 
     class Media:
         css = {
```

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/PKG-INFO` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.4
+Version: 0.4.0
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -23,18 +23,18 @@
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
   * [Function & Features](#function--features)
     * [Searching](#searching)
     * [Option creation](#option-creation)
       * [AJAX request](#ajax-request)
     * [Changelist link](#changelist-link)
+    * [Inline edit link](#inline-edit-link)
     * [Filter against values of another field](#filter-against-values-of-another-field)
   * [Development & Demo](#development--demo)
 <!-- TOC -->
-
 ----
 
 ## Installation
 
 Install:
 ```bash
 pip install -U mizdb-tomselect
@@ -136,14 +136,15 @@
 | value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
 | label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
 | search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
 | create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
 | multiple       | False                                  | if True, allow selecting multiple options                                                      |
 | changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
 | add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
+| edit_url       |                                        | URL name of the edit view for this model([see below](#inline-edit-link))                       |
 | filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
 
 This widget displays the results in tabular form. A table header will be added
@@ -243,14 +244,28 @@
     path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
 widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
 
+### Inline edit link
+
+Provide a `edit_url` to attach a link to the edit/change page for each selected item.
+```python
+# urls.py
+urlpatterns = [
+    ...
+    path('city/edit/<path:object_id>/', CityChangeView.as_view(), name='city_change'),
+]
+
+# forms.py
+widget = MIZSelect(City, edit_url='city_change')
+```
+
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
 class Person(models.Model):
```

### Comparing `mizdb-tomselect-0.3.4/src/mizdb_tomselect.egg-info/SOURCES.txt` & `mizdb-tomselect-0.4.0/src/mizdb_tomselect.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,10 +9,9 @@
 src/mizdb_tomselect.egg-info/dependency_links.txt
 src/mizdb_tomselect.egg-info/requires.txt
 src/mizdb_tomselect.egg-info/top_level.txt
 src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
 src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
 src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
 src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
-tests/test_e2e.py
 tests/test_views.py
 tests/test_widgets.py
```

### Comparing `mizdb-tomselect-0.3.4/tests/test_views.py` & `mizdb-tomselect-0.4.0/tests/test_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,130 @@
 import json
 from unittest.mock import Mock, patch
 from urllib.parse import urlencode
 
 import pytest
-from django.contrib.auth import get_permission_codename, get_user_model
-from django.contrib.auth.models import Permission
 from django.db.models.sql.where import NothingNode
-from django.http import HttpResponseBadRequest, HttpResponseForbidden, JsonResponse
+from django.http import HttpResponse, HttpResponseBadRequest, HttpResponseForbidden, JsonResponse
 from django.test import Client
-from django.urls import reverse
-from testapp.models import Ausgabe
+from django.urls import path, reverse
+from django.views.decorators.csrf import ensure_csrf_cookie
 
 from mizdb_tomselect.views import (
     FILTERBY_VAR,
-    PAGE_SIZE,
     PAGE_VAR,
     SEARCH_LOOKUP_VAR,
     SEARCH_VAR,
     VALUES_VAR,
     AutocompleteView,
 )
+from tests.testapp.models import Person
 
 
-@pytest.fixture
-def obj():
-    return Ausgabe.objects.create(name="Test", num="1", lnum="2", jahr="3")
+@ensure_csrf_cookie
+def csrf_cookie_view(request):
+    # A dummy view to make the CSRF middleware set the CSRF cookie.
+    return HttpResponse()
 
 
-@pytest.fixture(autouse=True)
-def not_found():
-    # Add a 'control' object that should never be included in the search results.
-    return Ausgabe.objects.create(name="Not Found")
+urlpatterns = [
+    path("autocomplete/", AutocompleteView.as_view(), name="autocomplete"),
+    path("csrf/", csrf_cookie_view, name="csrf"),
+]
 
 
 @pytest.fixture
-def pages():
-    # Create enough data for multiple pages.
-    return [
-        Ausgabe.objects.create(name=f"2022-{i + 1:02}", num=i + 1, lnum=100 + i, jahr="2022")
-        for i in range(PAGE_SIZE * 2)
-    ]
+def request_data():
+    """Return additional request data as set by test parametrization."""
+    return {}
+
+
+def _make_request(rf_func, request_data):
+    """Call the request factory function `rf_func` to create a request."""
+
+    def inner(data=None, user=None, **extra):
+        # Let data override the parametrized request data:
+        request = rf_func("/", data={**request_data, **(data or {})}, **extra)
+        if user:
+            request.user = user
+        return request
+
+    return inner
 
 
 @pytest.fixture
-def perms_user():
-    # Create a user that has 'add' permission for model Ausgabe
-    user = get_user_model().objects.create_user(username="perms", password="foo")
-    user.user_permissions.add(Permission.objects.get(codename=get_permission_codename("add", Ausgabe._meta)))
-    return user
+def get_request(rf, request_data):
+    """Return a GET request."""
+    return _make_request(rf.get, request_data)
 
 
 @pytest.fixture
-def noperms_user():
-    return get_user_model().objects.create_user(username="noperms", password="bar")
+def post_request(rf, request_data):
+    """Return a POST request."""
+    return _make_request(rf.post, request_data)
 
 
 @pytest.mark.django_db
+@pytest.mark.urls(__name__)
 class TestAutocompleteView:
     @pytest.fixture(autouse=True)
     def setup(self):
         self.url = reverse("autocomplete")
-        self.model_label = f"{Ausgabe._meta.app_label}.{Ausgabe._meta.model_name}"
+        self.model_label = f"{Person._meta.app_label}.{Person._meta.model_name}"
 
-    def test_get_contains_result(self, admin_client, obj):
+    def test_get_contains_result(self, admin_client, random_person):
         """The response of a search query should contain the expected result."""
-        query_string = urlencode({"model": self.model_label, SEARCH_VAR: "test", SEARCH_LOOKUP_VAR: "name__icontains"})
+        query_string = urlencode(
+            {
+                "model": self.model_label,
+                SEARCH_VAR: random_person.full_name,
+                SEARCH_LOOKUP_VAR: "full_name__icontains",
+                VALUES_VAR: json.dumps(["id", "full_name"]),
+            }
+        )
         response = admin_client.get(f"{self.url}?{query_string}")
         data = json.loads(response.content)
-        assert data["results"] == list(Ausgabe.objects.filter(pk=obj.pk).values())
+        assert data["results"] == list(Person.objects.filter(pk=random_person.pk).values("id", "full_name"))
 
-    @pytest.mark.parametrize("page_number,has_more", [(1, True), (2, False)])
-    def test_context_pagination(self, admin_client, pages, page_number, has_more):
+    @pytest.mark.parametrize("page_number,has_more", [(1, True), (2, True), (3, False)])
+    def test_context_pagination(self, admin_client, test_data, page_number, has_more):
         """
         The response of a search query should contain context items for
         pagination.
         """
         request_data = {
             "model": self.model_label,
-            SEARCH_VAR: "2022",
+            SEARCH_VAR: "Alice",
             PAGE_VAR: str(page_number),
-            SEARCH_LOOKUP_VAR: "name__icontains",
+            SEARCH_LOOKUP_VAR: "full_name__icontains",
         }
         response = admin_client.get(self.url, data=request_data)
         data = json.loads(response.content)
         assert data["page"] == page_number
         assert data["has_more"] == has_more
 
     def test_post_creates_new_object(self, admin_client):
         """A successful POST request should create a new model object."""
-        request_data = {"model": self.model_label, "name": "New Ausgabe", "create-field": "name"}
+        request_data = {"model": self.model_label, "full_name": "Bob Testman", "create-field": "full_name"}
         response = admin_client.post(self.url, data=request_data)
         assert response.status_code == 200
-        assert Ausgabe.objects.filter(name="New Ausgabe").exists()
+        assert Person.objects.filter(full_name="Bob Testman").exists()
 
     def test_post_context_contains_object_data(self, admin_client):
         """
         The context of a successful POST request should contain data about the
         created item.
         """
         request_data = {
             "model": self.model_label,
-            "name": "New Ausgabe",
-            "create-field": "name",
+            "full_name": "Bob Testman",
+            "create-field": "full_name",
         }
         response = admin_client.post(self.url, data=request_data)
-        new = Ausgabe.objects.get(name="New Ausgabe")
+        new = Person.objects.get(full_name="Bob Testman")
         data = json.loads(response.content)
         assert data["pk"] == new.pk
         assert data["text"] == str(new)
 
     def test_post_no_permission(self, client, noperms_user):
         """
         Users that do not have 'add' permission should have the POST request
@@ -143,183 +159,180 @@
         client = Client(enforce_csrf_checks=True)
         client.force_login(admin_user)
         client.get(reverse("csrf"))  # have the csrf middleware set the cookie
         token = client.cookies["csrftoken"]
 
         request_data = {
             "model": self.model_label,
-            "name": "New Ausgabe",
-            "create-field": "name",
+            "full_name": "Bob Testman",
+            "create-field": "full_name",
             "csrfmiddlewaretoken": token.coded_value if has_csrf_token else "",
         }
         response = client.post(self.url, data=request_data)
         if not has_csrf_token:
             assert response.status_code == 403
         else:
             assert response.status_code == 200
 
-    def test_get_no_search_term(self, client):
+    def test_get_no_search_term(self, client, random_person):
         """Assert that a GET request without a search term still returns results."""
-        query_string = urlencode({"model": self.model_label, SEARCH_LOOKUP_VAR: "name__icontains"})
+        query_string = urlencode({"model": self.model_label, SEARCH_LOOKUP_VAR: "full_name__icontains"})
         response = client.get(f"{self.url}?{query_string}")
         data = json.loads(response.content)
         assert data["results"]
 
-    def test_get_with_filter_by(self, client, obj):
+    def test_get_with_filter_by(self, client, random_person):
         """
         Assert that a GET request with a filterBy value returns the expected
         results.
         """
         query_string = urlencode(
-            {"model": self.model_label, SEARCH_LOOKUP_VAR: "name__icontains", FILTERBY_VAR: "lnum=2"}
+            {
+                "model": self.model_label,
+                SEARCH_LOOKUP_VAR: "full_name__icontains",
+                FILTERBY_VAR: f"city={random_person.city.pk}",
+            }
         )
         response = client.get(f"{self.url}?{query_string}")
         data = json.loads(response.content)
-        assert len(data["results"]) == 1
-        assert data["results"][0]["id"] == obj.pk
+        assert len(data["results"])
+        assert random_person.pk in [r["id"] for r in data["results"]]
 
-    def test_get_no_filter_by(self, client):
+    def test_get_no_filter_by(self, test_data, client):
         """
         Assert that a GET request returns no results when a required filterBy
         has no value.
         """
         query_string = urlencode(
-            {"model": self.model_label, SEARCH_LOOKUP_VAR: "name__icontains", FILTERBY_VAR: "lnum="}
+            {"model": self.model_label, SEARCH_LOOKUP_VAR: "full_name__icontains", FILTERBY_VAR: "city="}
         )
         response = client.get(f"{self.url}?{query_string}")
         data = json.loads(response.content)
         assert not data["results"]
 
 
 @pytest.mark.django_db
 class TestAutocompleteViewUnitTests:
     @pytest.fixture(autouse=True)
     def setup(self):
-        self.model = Ausgabe
+        self.model = Person
         self.queryset = self.model.objects.all()
         self.model_label = f"{self.model._meta.app_label}.{self.model._meta.model_name}"
 
     @pytest.fixture
-    def minimal_request_data(self):
-        # Minimal request data required for setting up the view.
-        return {"model": self.model_label}
-
-    @pytest.fixture
-    def request_data(self):
-        return {}
-
-    @pytest.fixture
-    def get_request(self, rf, minimal_request_data, request_data):
-        return rf.get("/", data={**minimal_request_data, **request_data})
-
-    @pytest.fixture
-    def post_request(self, rf, minimal_request_data, request_data):
-        print(f"{request_data=}")
-        return rf.post("/", data={**minimal_request_data, **request_data})
-
-    @pytest.fixture
     def view(self, get_request):
+        """Create an instance of AutocompleteView and assign the given request to it."""
         view = AutocompleteView()
-        view.request = get_request
+        view.request = get_request()
         return view
 
     @pytest.fixture
     def setup_view(self, view, get_request):
-        view.setup(request=get_request)
+        """Call the view's setup method with the given request."""
+        # 'model' is required by setup()
+        view.setup(request=get_request(data={"model": self.model_label}))
 
-    def test_setup_sets_model(self, view, setup_view):
+    @pytest.mark.parametrize("request_data", [{"model": f"{Person._meta.app_label}.{Person._meta.model_name}"}])
+    def test_setup_sets_model(self, view, setup_view, request_data):
         """Assert that setup() sets the `model` attribute."""
         assert view.model == self.model
 
     @pytest.mark.parametrize("request_data", [{"create-field": "create_field"}])
     def test_setup_sets_create_field(self, view, setup_view, request_data):
         """Assert that setup() sets the `create_field` attribute."""
         assert view.create_field == "create_field"
 
     @pytest.mark.parametrize("request_data", [{SEARCH_LOOKUP_VAR: "search_lookup"}])
     def test_setup_sets_search_lookup(self, view, setup_view, request_data):
         """Assert that setup() sets the `search_lookup` attribute."""
         assert view.search_lookup == "search_lookup"
 
-    @pytest.mark.parametrize("request_data", [{VALUES_VAR: json.dumps(["id", "name", "jahr", "num"])}])
+    @pytest.mark.parametrize("request_data", [{VALUES_VAR: json.dumps(["id", "full_name", "dob", "city"])}])
     def test_setup_sets_values_select(self, view, setup_view, request_data):
         """Assert that setup() sets the `values_select` attribute."""
-        assert view.values_select == ["id", "name", "jahr", "num"]
+        assert view.values_select == ["id", "full_name", "dob", "city"]
 
-    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "magazin_id=1"}])
+    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "city_id=1"}])
     def test_apply_filter_by(self, view, request_data):
         """Assert that apply_filter_by applies the expected ^filter to the queryset."""
         queryset = view.apply_filter_by(self.queryset)
         assert len(queryset.query.where.children) == 1
         lookup = queryset.query.where.children[0]
-        assert lookup.lhs.target == self.model._meta.get_field("magazin")
+        assert lookup.lhs.target == self.model._meta.get_field("city")
         assert lookup.rhs == 1
 
     @pytest.mark.parametrize("request_data", [{}])
     def test_apply_filter_by_no_filterby_var_in_request(self, view, request_data):
         """
         Assert that apply_filter_by returns the queryset unchanged if the
         request does not contain FILTERBY_VAR.
         """
         queryset = view.apply_filter_by(self.queryset)
         assert len(queryset.query.where.children) == 0
 
-    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "magazin_id="}])
+    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "city_id="}])
     def test_apply_filter_by_no_filter_value(self, view, request_data):
         """
         Assert that apply_filter_by returns an empty queryset if no filter
         value is given.
         """
         queryset = view.apply_filter_by(self.queryset)
         assert len(queryset.query.where.children) == 1
         assert isinstance(queryset.query.where.children[0], NothingNode)
 
     def test_search(self, view):
         """Assert that search filters the queryset against the given search term."""
-        view.search_lookup = "name__icontains"
+        view.search_lookup = "full_name__icontains"
         queryset = view.search(self.queryset, "Test")
         assert len(queryset.query.where.children) == 1
         lookup = queryset.query.where.children[0]
-        assert lookup.lhs.target == self.model._meta.get_field("name")
+        assert lookup.lhs.target == self.model._meta.get_field("full_name")
         assert lookup.rhs == "Test"
 
     def test_order_queryset(self, view, setup_view):
         """Assert that order_queryset applies ordering to the queryset."""
-        assert view.order_queryset(self.queryset).query.order_by == ("magazin", "name")
+        assert view.order_queryset(self.queryset).query.order_by == ("last_name", "first_name")
 
-    @pytest.mark.parametrize("request_data", [{SEARCH_VAR: "Test", SEARCH_LOOKUP_VAR: "name__icontains"}])
+    @pytest.mark.parametrize("request_data", [{SEARCH_VAR: "Test", SEARCH_LOOKUP_VAR: "full_name__icontains"}])
     def test_get_queryset_calls_search(self, view, setup_view, request_data):
         """Assert that get_queryset calls search if a search term is given."""
         search_mock = Mock()
         with patch.object(view, "apply_filter_by", new=search_mock):
             view.get_queryset()
             search_mock.assert_called()
 
-    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "magazin_id=1", SEARCH_LOOKUP_VAR: "name__icontains"}])
+    @pytest.mark.parametrize("request_data", [{FILTERBY_VAR: "city_id=1", SEARCH_LOOKUP_VAR: "full_name__icontains"}])
     def test_get_queryset_calls_apply_filter_by(self, view, setup_view, request_data):
         """Assert that get_queryset calls apply_filter_by if FILTERBY_VAR is given."""
         apply_filter_by_mock = Mock()
         with patch.object(view, "apply_filter_by", new=apply_filter_by_mock):
             view.get_queryset()
             apply_filter_by_mock.assert_called()
 
     def test_get_queryset_calls_order_queryset(self, view, setup_view):
         """Assert that get_queryset calls order_queryset."""
         order_queryset_mock = Mock()
         with patch.object(view, "order_queryset", new=order_queryset_mock):
             view.get_queryset()
             order_queryset_mock.assert_called()
 
-    @pytest.mark.parametrize("request_data", [{VALUES_VAR: json.dumps(["id", "name", "jahr", "num"])}])
-    def test_get_result_values(self, view, setup_view, request_data, obj):
+    @pytest.mark.parametrize("request_data", [{VALUES_VAR: json.dumps(["id", "full_name", "dob", "city__name"])}])
+    def test_get_result_values(self, view, setup_view, request_data, random_person):
         """Assert that get_result_values returns a list of queryset values."""
-        results = view.get_result_values(self.queryset.filter(pk=obj.pk))
-        assert results == [{"id": obj.pk, "name": "Test", "jahr": "3", "num": "1"}]
+        results = view.get_result_values(self.queryset.filter(pk=random_person.pk))
+        assert results == [
+            {
+                "id": random_person.pk,
+                "full_name": random_person.full_name,
+                "dob": random_person.dob,
+                "city__name": random_person.city.name,
+            }
+        ]
 
-    def test_get(self, view, setup_view, admin_user, obj):
+    def test_get(self, view, setup_view, admin_user):
         """Assert that get returns the expected response."""
         view.request.user = admin_user
         response = view.get(view.request)
         assert isinstance(response, JsonResponse)
         data = json.loads(response.content)
         assert "results" in data
         assert "page" in data
@@ -332,53 +345,52 @@
         Assert that has_add_permission returns whether the user has 'add'
         permission for the given model.
         """
         _request = get_request
         _request.user = request.getfixturevalue(user_name)
         assert view.has_add_permission(_request) == has_perm
 
-    @pytest.mark.parametrize("request_data", [{"create-field": "name"}])
+    @pytest.mark.parametrize("request_data", [{"create-field": "full_name"}])
     def test_create_object(self, view, setup_view, request_data):
         """Assert that create_object creates an object."""
-        obj = view.create_object({"name": "Test"})
+        obj = view.create_object({"full_name": "Bob Testman"})
         assert isinstance(obj, self.model)
-        assert obj.name == "Test"
+        assert obj.full_name == "Bob Testman"
 
     @pytest.mark.parametrize("request_data", [{"create-field": "name", "name": "__anything__"}])
-    def test_post(self, view, setup_view, post_request, request_data, obj):
+    def test_post(self, view, setup_view, post_request, request_data):
         """Assert that post returns the expected response."""
 
         class DummyObject:
             pk = 42
             name = "foo"
 
             def __str__(self):
                 return f"{self.name}"
 
         create_object_mock = Mock(return_value=DummyObject())
 
         with patch.object(view, "has_add_permission", new=Mock(return_value=True)):
             with patch.object(view, "create_object", new=create_object_mock):
-                response = view.post(post_request)
+                response = view.post(post_request())
                 assert isinstance(response, JsonResponse)
                 create_object_mock.assert_called()
                 data = json.loads(response.content)
                 assert data["pk"] == 42
                 assert data["text"] == "foo"
 
     def test_post_no_permission(self, view, setup_view, noperms_user, post_request):
         """
         Assert that post returns a HttpResponseForbidden response when the user
         does not have permission to add objects.
         """
-        request = post_request
-        request.user = noperms_user
-        assert isinstance(view.post(post_request), HttpResponseForbidden)
+        # request = post_request
+        # request.user = noperms_user
+        assert isinstance(view.post(post_request(user=noperms_user)), HttpResponseForbidden)
 
-    @pytest.mark.parametrize("request_data", [{"create-field": "name"}])
-    def test_post_no_create_field_data(self, view, setup_view, post_request, request_data):
+    def test_post_no_create_field_data(self, view, setup_view, post_request):
         """
         Assert that post returns a HttpResponseBadRequest response when the
         request did not contain data for the create_field.
         """
         with patch.object(view, "has_add_permission", new=Mock(return_value=True)):
-            assert isinstance(view.post(post_request), HttpResponseBadRequest)
+            assert isinstance(view.post(post_request(data={"create-field": "name"})), HttpResponseBadRequest)
```

### Comparing `mizdb-tomselect-0.3.4/tests/test_widgets.py` & `mizdb-tomselect-0.4.0/tests/test_widgets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,161 @@
 import pytest
 from django.db import models
-from testapp.models import Ausgabe
+from django.urls import path
 
 from mizdb_tomselect.widgets import MIZSelect, MIZSelectTabular
+from tests.testapp.models import Person
 
+urlpatterns = [
+    path("test/autocomplete/", lambda r: None, name="autocomplete"),
+    path("test/add/", lambda r: None, name="add_page"),
+    path("test/edit/<path:object_id>/", lambda r: None, name="edit_page"),
+    path("test/changelist/", lambda r: None, name="changelist_page"),
+]
 
-class WidgetTestCase:
-    widget_class = None
+pytestmark = pytest.mark.urls(__name__)
 
-    @pytest.fixture(autouse=True)
-    def make_widget(self):
-        def _make_widget(model=Ausgabe, **kwargs):
-            return self.widget_class(model, **kwargs)
 
-        self.make_widget = _make_widget
+@pytest.fixture
+def make_widget(widget_class):
+    """Return factory function that creates widgets of the given widget_class."""
 
+    def inner(model=None, **kwargs):
+        return widget_class(model=model, **kwargs)
 
-class TestMIZSelect(WidgetTestCase):
+    return inner
+
+
+@pytest.fixture
+def widget(make_widget, model=Person, **widget_kwargs):
+    """Create a widget for the given model with the given kwargs."""
+    return make_widget(model=model, **widget_kwargs)
+
+
+@pytest.mark.parametrize("widget_class", [MIZSelect])
+class TestMIZSelect:
     widget_class = MIZSelect
 
-    def test_init_sets_default_value_field(self):
+    def test_init_sets_default_value_field(self, make_widget):
         """
         Assert that init sets the default for `value_field` to the model's
         primary key.
         """
 
         class CustomPrimaryKeyModel(models.Model):
             my_primary_key = models.PositiveIntegerField(primary_key=True)
 
             class Meta:
                 app_label = "testapp"
 
-        widget = self.widget_class(CustomPrimaryKeyModel)
+        widget = make_widget(model=CustomPrimaryKeyModel)
         assert widget.value_field == "my_primary_key"
 
-    def test_init_sets_default_label_field_to_name(self):
+    def test_init_sets_default_label_field_to_name(self, make_widget):
         """
         Assert that init sets the default for `label_field` to 'name' if the
         model has no `name_field`.
         """
 
         class NoNameFieldModel(models.Model):
             foo = models.CharField(max_length=1)
 
             class Meta:
                 app_label = "testapp"
 
-        widget = self.widget_class(NoNameFieldModel)
+        widget = make_widget(model=NoNameFieldModel)
         assert widget.label_field == "name"
 
-    def test_init_sets_default_label_field_to_name_field(self):
+    def test_init_sets_default_label_field_to_name_field(self, make_widget):
         """
         Assert that init sets the default for `label_field` to the model's
         `name_field`.
         """
 
         class NameFieldModel(models.Model):
             foo = models.CharField(max_length=1)
 
             name_field = "foo"
 
             class Meta:
                 app_label = "testapp"
 
-        widget = self.widget_class(NameFieldModel)
+        widget = make_widget(model=NameFieldModel)
         assert widget.label_field == "foo"
 
-    def test_init_sets_default_search_lookup_from_label_field(self):
+    def test_init_sets_default_search_lookup_from_label_field(self, make_widget):
         """
         Assert that init sets the default for `search_lookup` to the value of
         label_field + icontains.
         """
-        widget = MIZSelect(Ausgabe, label_field="foo")
+        widget = make_widget(model=Person, label_field="foo")
         assert widget.search_lookup == "foo__icontains"
 
-    def test_optgroups_no_initial_choices(self):
+    def test_optgroups_no_initial_choices(self, widget):
         """Assert that the widget is rendered without any options."""
-        context = self.make_widget().get_context("ausgabe", None, {})
+        context = widget.get_context("ausgabe", None, {})
         assert not context["widget"]["optgroups"]
 
-    def test_build_attrs(self):
+    def test_build_attrs(self, make_widget):
         """Assert that the required HTML attributes are added."""
-        widget = self.make_widget(
-            model=Ausgabe,
-            url="dummy_url",
+        widget = make_widget(
+            model=Person,
+            url="autocomplete",
             value_field="pk",
-            label_field="num",
+            label_field="name",
             create_field="the_create_field",
             multiple=True,
             changelist_url="changelist_page",
             add_url="add_page",
+            edit_url="edit_page",
         )
         attrs = widget.build_attrs({})
         assert attrs["is-tomselect"]
         assert attrs["is-multiple"]
-        assert attrs["data-autocomplete-url"] == "/dummy/url/"
-        assert attrs["data-model"] == f"{Ausgabe._meta.app_label}.{Ausgabe._meta.model_name}"
+        assert attrs["data-autocomplete-url"] == "/test/autocomplete/"
+        assert attrs["data-model"] == f"{Person._meta.app_label}.{Person._meta.model_name}"
         assert attrs["data-value-field"] == "pk"
-        assert attrs["data-label-field"] == "num"
+        assert attrs["data-label-field"] == "name"
         assert attrs["data-create-field"] == "the_create_field"
-        assert attrs["data-changelist-url"] == "/testapp/changelist/"
-        assert attrs["data-add-url"] == "/testapp/add/"
+        assert attrs["data-changelist-url"] == "/test/changelist/"
+        assert attrs["data-add-url"] == "/test/add/"
+        assert attrs["data-edit-url"] == "/test/edit/{pk}/"
 
     @pytest.mark.parametrize(
         "static_file",
         ("mizselect.css", "tom-select.bootstrap5.css", "mizselect.js"),
     )
-    def test_media(self, static_file):
+    def test_media(self, widget, static_file):
         """Assert that the necessary static files are included."""
-        assert static_file in str(self.make_widget().media)
-
+        assert static_file in str(widget.media)
 
-class TestTabularMIZSelect(WidgetTestCase):
-    widget_class = MIZSelectTabular
 
-    def test_init_sets_label_field_label(self):
+@pytest.mark.parametrize("widget_class", [MIZSelectTabular])
+class TestTabularMIZSelect:
+    def test_init_sets_label_field_label(self, widget):
         """
         Assert that init sets the default for `label_field_label` to the
         verbose_name of the model.
         """
-        widget = self.widget_class(Ausgabe)
-        assert widget.label_field_label == "Ausgabe"
+        assert widget.label_field_label == "Person"
 
-    def test_init_sets_value_field_label(self):
+    def test_init_sets_value_field_label(self, widget):
         """
         Assert that init sets the default for `value_field_label` to
         value_field.title().
         """
-        widget = self.widget_class(Ausgabe)
         assert widget.value_field_label == "Id"
 
-    def test_build_attrs(self):
+    def test_build_attrs(self, make_widget):
         """Assert that the required HTML attributes are added."""
-        widget = self.make_widget(
-            model=Ausgabe,
-            extra_columns={"jahr": "Jahr", "num": "Nummer", "lnum": "lfd.Nummer"},
+        widget = make_widget(
+            model=Person,
+            extra_columns={"dob": "Date of Birth", "city": "City"},
             value_field_label="Primary Key",
-            label_field_label="Ausgabe",
+            label_field_label="Person",
         )
         attrs = widget.build_attrs({})
         assert attrs["is-tabular"]
         assert attrs["data-value-field-label"] == "Primary Key"
-        assert attrs["data-label-field-label"] == "Ausgabe"
-        assert attrs["data-extra-headers"] == '["Jahr", "Nummer", "lfd.Nummer"]'
-        assert attrs["data-extra-columns"] == '["jahr", "num", "lnum"]'
+        assert attrs["data-label-field-label"] == "Person"
+        assert attrs["data-extra-headers"] == '["Date of Birth", "City"]'
+        assert attrs["data-extra-columns"] == '["dob", "city"]'
```

