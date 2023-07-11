# Comparing `tmp/gensaschema-0.6.7.tar.gz` & `tmp/gensaschema-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jan  9 07:50:07 2023, max compression, from Unix
+gzip compressed data, last modified: Tue Jul 11 20:32:25 2023, max compression, from Unix
```

## Comparing `gensaschema-0.6.7.tar` & `gensaschema-0.6.8.tar`

### file list

```diff
@@ -1,138 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.421237 gensaschema-0.6.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-07-31 12:25:01.000000 gensaschema-0.6.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      190 2022-07-31 12:27:14.000000 gensaschema-0.6.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2265 2023-01-09 07:50:07.421237 gensaschema-0.6.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1831 2023-01-09 07:48:10.000000 gensaschema-0.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.399237 gensaschema-0.6.7/docs/
--rw-r--r--   0 root         (0) root         (0)     2591 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/CHANGES
--rw-r--r--   0 root         (0) root         (0)      694 2022-07-31 12:28:20.000000 gensaschema-0.6.7/docs/CLASSIFIERS
--rw-r--r--   0 root         (0) root         (0)     1085 2023-01-09 07:48:10.000000 gensaschema-0.6.7/docs/DESCRIPTION
--rw-r--r--   0 root         (0) root         (0)     1032 2022-07-31 12:28:33.000000 gensaschema-0.6.7/docs/DEVELOPMENT.md
--rw-r--r--   0 root         (0) root         (0)       18 2022-07-31 12:28:38.000000 gensaschema-0.6.7/docs/PROVIDES
--rw-r--r--   0 root         (0) root         (0)       35 2022-07-31 12:28:43.000000 gensaschema-0.6.7/docs/SUMMARY
--rw-r--r--   0 root         (0) root         (0)       65 2022-07-31 12:28:49.000000 gensaschema-0.6.7/docs/TODO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.400237 gensaschema-0.6.7/docs/userdoc/
--rw-r--r--   0 root         (0) root         (0)      230 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/.buildinfo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.400237 gensaschema-0.6.7/docs/userdoc/_modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.403237 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/
--rw-r--r--   0 root         (0) root         (0)    21496 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_column.html
--rw-r--r--   0 root         (0) root         (0)    29099 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_config.html
--rw-r--r--   0 root         (0) root         (0)    42112 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_constraint.html
--rw-r--r--   0 root         (0) root         (0)     9741 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_exceptions.html
--rw-r--r--   0 root         (0) root         (0)     7812 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_meta.html
--rw-r--r--   0 root         (0) root         (0)    22003 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_schema.html
--rw-r--r--   0 root         (0) root         (0)    44089 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_symbols.html
--rw-r--r--   0 root         (0) root         (0)    58133 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_table.html
--rw-r--r--   0 root         (0) root         (0)    10789 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_template.html
--rw-r--r--   0 root         (0) root         (0)    30322 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_type.html
--rw-r--r--   0 root         (0) root         (0)     9877 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_util.html
--rw-r--r--   0 root         (0) root         (0)    10886 2023-01-09 07:49:15.000000 gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/constraints.html
--rw-r--r--   0 root         (0) root         (0)     4878 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_modules/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.403237 gensaschema-0.6.7/docs/userdoc/_sources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.406237 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/
--rw-r--r--   0 root         (0) root         (0)      137 2022-07-31 12:25:01.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/cdbx._cdb.txt
--rw-r--r--   0 root         (0) root         (0)      222 2022-07-31 12:25:01.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/cdbx.txt
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._column.txt
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._config.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._constraint.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._exceptions.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._meta.txt
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._schema.txt
--rw-r--r--   0 root         (0) root         (0)      170 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._symbols.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._table.txt
--rw-r--r--   0 root         (0) root         (0)      173 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._template.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._type.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema._util.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema.constraints.txt
--rw-r--r--   0 root         (0) root         (0)      514 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-31 12:26:03.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/index.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-01-09 07:46:41.000000 gensaschema-0.6.7/docs/userdoc/_sources/apidoc/modules.txt
--rw-r--r--   0 root         (0) root         (0)     1950 2023-01-09 07:48:10.000000 gensaschema-0.6.7/docs/userdoc/_sources/index.txt
--rw-r--r--   0 root         (0) root         (0)     1763 2023-01-09 07:48:10.000000 gensaschema-0.6.7/docs/userdoc/_sources/website_download.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.410237 gensaschema-0.6.7/docs/userdoc/_static/
--rw-r--r--   0 root         (0) root         (0)    14813 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_static/basic.css
--rw-r--r--   0 root         (0) root         (0)      206 2022-07-31 12:28:57.000000 gensaschema-0.6.7/docs/userdoc/_static/ci.css
--rw-r--r--   0 root         (0) root         (0)     6015 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/cloud.base.js
--rw-r--r--   0 root         (0) root         (0)    33560 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_static/cloud.css
--rw-r--r--   0 root         (0) root         (0)    44293 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_static/cloud.js
--rw-r--r--   0 root         (0) root         (0)     4472 2023-01-09 07:29:40.000000 gensaschema-0.6.7/docs/userdoc/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      420 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-01-09 07:29:40.000000 gensaschema-0.6.7/docs/userdoc/_static/file.png
--rw-r--r--   0 root         (0) root         (0)     1100 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-caution.png
--rw-r--r--   0 root         (0) root         (0)     1272 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-danger.png
--rw-r--r--   0 root         (0) root         (0)     1329 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-deprecated.png
--rw-r--r--   0 root         (0) root         (0)     1204 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-note.png
--rw-r--r--   0 root         (0) root         (0)      951 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-seealso.png
--rw-r--r--   0 root         (0) root         (0)     1324 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-todo.png
--rw-r--r--   0 root         (0) root         (0)      887 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/icon-warning.png
--rw-r--r--   0 root         (0) root         (0)     3121 2023-01-09 07:29:41.000000 gensaschema-0.6.7/docs/userdoc/_static/jquery.cookie.js
--rw-r--r--   0 root         (0) root         (0)     4758 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_static/language_data.js
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-09 07:29:40.000000 gensaschema-0.6.7/docs/userdoc/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-09 07:29:40.000000 gensaschema-0.6.7/docs/userdoc/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     4846 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)    18215 2023-01-09 07:29:40.000000 gensaschema-0.6.7/docs/userdoc/_static/searchtools.js
--rw-r--r--   0 root         (0) root         (0)     4712 2023-01-09 07:29:40.000000 gensaschema-0.6.7/docs/userdoc/_static/sphinx_highlight.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.414237 gensaschema-0.6.7/docs/userdoc/apidoc/
--rw-r--r--   0 root         (0) root         (0)     4211 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/cdbx._cdb.html
--rw-r--r--   0 root         (0) root         (0)     4989 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/cdbx.html
--rw-r--r--   0 root         (0) root         (0)    32789 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._column.html
--rw-r--r--   0 root         (0) root         (0)    25033 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._config.html
--rw-r--r--   0 root         (0) root         (0)    40191 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._constraint.html
--rw-r--r--   0 root         (0) root         (0)    16938 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._exceptions.html
--rw-r--r--   0 root         (0) root         (0)    13384 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._meta.html
--rw-r--r--   0 root         (0) root         (0)    22985 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._schema.html
--rw-r--r--   0 root         (0) root         (0)    49484 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._symbols.html
--rw-r--r--   0 root         (0) root         (0)    42368 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._table.html
--rw-r--r--   0 root         (0) root         (0)    16626 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._template.html
--rw-r--r--   0 root         (0) root         (0)    21053 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._type.html
--rw-r--r--   0 root         (0) root         (0)     9744 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._util.html
--rw-r--r--   0 root         (0) root         (0)    11390 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema.constraints.html
--rw-r--r--   0 root         (0) root         (0)   120409 2023-01-09 07:50:05.000000 gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema.html
--rw-r--r--   0 root         (0) root         (0)    27595 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/apidoc/index.html
--rw-r--r--   0 root         (0) root         (0)    26356 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/apidoc/modules.html
--rw-r--r--   0 root         (0) root         (0)     7916 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/index.html
--rw-r--r--   0 root         (0) root         (0)     2067 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/objects.inv
--rw-r--r--   0 root         (0) root         (0)     7327 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/py-modindex.html
--rw-r--r--   0 root         (0) root         (0)     4227 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/search.html
--rw-r--r--   0 root         (0) root         (0)    51031 2023-01-09 07:50:06.000000 gensaschema-0.6.7/docs/userdoc/searchindex.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.416237 gensaschema-0.6.7/gensaschema/
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_column.py
--rw-r--r--   0 root         (0) root         (0)     6584 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_config.py
--rw-r--r--   0 root         (0) root         (0)     8162 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_constraint.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_meta.py
--rw-r--r--   0 root         (0) root         (0)     5002 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_schema.py
--rw-r--r--   0 root         (0) root         (0)     9799 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_symbols.py
--rw-r--r--   0 root         (0) root         (0)    13596 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_table.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_template.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_type.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/_util.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-01-09 07:48:10.000000 gensaschema-0.6.7/gensaschema/constraints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.417237 gensaschema-0.6.7/gensaschema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-01-09 07:50:07.000000 gensaschema-0.6.7/gensaschema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4185 2023-01-09 07:50:07.000000 gensaschema-0.6.7/gensaschema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 07:50:07.000000 gensaschema-0.6.7/gensaschema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-31 12:34:55.000000 gensaschema-0.6.7/gensaschema.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-09 07:50:07.000000 gensaschema-0.6.7/gensaschema.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-09 07:50:07.421237 gensaschema-0.6.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3688 2023-01-09 07:48:10.000000 gensaschema-0.6.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.418237 gensaschema-0.6.7/tests/
--rw-r--r--   0 root         (0) root         (0)      771 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5153 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/_util.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-01-09 07:24:59.000000 gensaschema-0.6.7/tests/coverage.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.419237 gensaschema-0.6.7/tests/integration/
--rw-r--r--   0 root         (0) root         (0)      924 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/integration/test_schema.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/integration/test_table.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/integration/test_type.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-01-09 07:24:59.000000 gensaschema-0.6.7/tests/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.420237 gensaschema-0.6.7/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      791 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 07:50:07.421237 gensaschema-0.6.7/tests/unit/fixtures/
--rw-r--r--   0 root         (0) root         (0)      104 2022-07-31 12:25:48.000000 gensaschema-0.6.7/tests/unit/fixtures/config1.schema
--rw-r--r--   0 root         (0) root         (0)     3762 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/unit/test_column.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/unit/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/unit/test_template.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/unit/test_type.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-01-09 07:48:10.000000 gensaschema-0.6.7/tests/unit/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.009237 gensaschema-0.6.8/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-03 20:15:43.000000 gensaschema-0.6.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-03 20:15:43.000000 gensaschema-0.6.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-07-11 20:32:25.008237 gensaschema-0.6.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-03 20:15:43.000000 gensaschema-0.6.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:24.991237 gensaschema-0.6.8/docs/
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-07-11 20:31:35.000000 gensaschema-0.6.8/docs/CHANGES
+-rw-r--r--   0 root         (0) root         (0)      694 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/CLASSIFIERS
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/DESCRIPTION
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/DEVELOPMENT.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/PROVIDES
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/SUMMARY
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/TODO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:24.992237 gensaschema-0.6.8/docs/userdoc/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/.buildinfo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:24.992237 gensaschema-0.6.8/docs/userdoc/_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:24.994237 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/
+-rw-r--r--   0 root         (0) root         (0)    21525 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_column.html
+-rw-r--r--   0 root         (0) root         (0)    29101 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_config.html
+-rw-r--r--   0 root         (0) root         (0)    42676 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_constraint.html
+-rw-r--r--   0 root         (0) root         (0)     9700 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_exceptions.html
+-rw-r--r--   0 root         (0) root         (0)     7812 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_meta.html
+-rw-r--r--   0 root         (0) root         (0)    21522 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_schema.html
+-rw-r--r--   0 root         (0) root         (0)    44150 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_symbols.html
+-rw-r--r--   0 root         (0) root         (0)    58988 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_table.html
+-rw-r--r--   0 root         (0) root         (0)    10788 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_template.html
+-rw-r--r--   0 root         (0) root         (0)    34966 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_type.html
+-rw-r--r--   0 root         (0) root         (0)     9612 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_util.html
+-rw-r--r--   0 root         (0) root         (0)    11018 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/constraints.html
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_modules/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:24.994237 gensaschema-0.6.8/docs/userdoc/_sources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:24.997237 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._column.txt
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._config.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._constraint.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._exceptions.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._meta.txt
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._schema.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._symbols.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._table.txt
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._template.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._type.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema._util.txt
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema.constraints.txt
+-rw-r--r--   0 root         (0) root         (0)      514 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/index.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-11 20:27:14.000000 gensaschema-0.6.8/docs/userdoc/_sources/apidoc/modules.txt
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/userdoc/_sources/index.txt
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-11 20:31:35.000000 gensaschema-0.6.8/docs/userdoc/_sources/website_download.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.000237 gensaschema-0.6.8/docs/userdoc/_static/
+-rw-r--r--   0 root         (0) root         (0)    14813 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_static/basic.css
+-rw-r--r--   0 root         (0) root         (0)      206 2023-07-03 20:15:43.000000 gensaschema-0.6.8/docs/userdoc/_static/ci.css
+-rw-r--r--   0 root         (0) root         (0)     6015 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/cloud.base.js
+-rw-r--r--   0 root         (0) root         (0)    33560 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_static/cloud.css
+-rw-r--r--   0 root         (0) root         (0)    44293 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_static/cloud.js
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-07-11 20:09:06.000000 gensaschema-0.6.8/docs/userdoc/_static/doctools.js
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_static/documentation_options.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-11 20:09:06.000000 gensaschema-0.6.8/docs/userdoc/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-caution.png
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-danger.png
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-deprecated.png
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-note.png
+-rw-r--r--   0 root         (0) root         (0)      951 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-seealso.png
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-todo.png
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/icon-warning.png
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-07-11 20:09:08.000000 gensaschema-0.6.8/docs/userdoc/_static/jquery.cookie.js
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_static/language_data.js
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-11 20:09:06.000000 gensaschema-0.6.8/docs/userdoc/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-11 20:09:06.000000 gensaschema-0.6.8/docs/userdoc/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)     4846 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/_static/pygments.css
+-rw-r--r--   0 root         (0) root         (0)    18215 2023-07-11 20:09:06.000000 gensaschema-0.6.8/docs/userdoc/_static/searchtools.js
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-07-11 20:09:06.000000 gensaschema-0.6.8/docs/userdoc/_static/sphinx_highlight.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.003237 gensaschema-0.6.8/docs/userdoc/apidoc/
+-rw-r--r--   0 root         (0) root         (0)    32775 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._column.html
+-rw-r--r--   0 root         (0) root         (0)    25019 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._config.html
+-rw-r--r--   0 root         (0) root         (0)    40177 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._constraint.html
+-rw-r--r--   0 root         (0) root         (0)    16924 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._exceptions.html
+-rw-r--r--   0 root         (0) root         (0)    13370 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._meta.html
+-rw-r--r--   0 root         (0) root         (0)    22971 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._schema.html
+-rw-r--r--   0 root         (0) root         (0)    49470 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._symbols.html
+-rw-r--r--   0 root         (0) root         (0)    42629 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._table.html
+-rw-r--r--   0 root         (0) root         (0)    16612 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._template.html
+-rw-r--r--   0 root         (0) root         (0)    23312 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._type.html
+-rw-r--r--   0 root         (0) root         (0)     9730 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._util.html
+-rw-r--r--   0 root         (0) root         (0)    11376 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema.constraints.html
+-rw-r--r--   0 root         (0) root         (0)   120837 2023-07-11 20:32:23.000000 gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema.html
+-rw-r--r--   0 root         (0) root         (0)    28023 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/index.html
+-rw-r--r--   0 root         (0) root         (0)    26784 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/apidoc/modules.html
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/index.html
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/objects.inv
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/py-modindex.html
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/search.html
+-rw-r--r--   0 root         (0) root         (0)    50862 2023-07-11 20:32:24.000000 gensaschema-0.6.8/docs/userdoc/searchindex.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.005237 gensaschema-0.6.8/gensaschema/
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4694 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_column.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_config.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_constraint.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_meta.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_schema.py
+-rw-r--r--   0 root         (0) root         (0)     9838 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_symbols.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_table.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-03 20:15:43.000000 gensaschema-0.6.8/gensaschema/_template.py
+-rw-r--r--   0 root         (0) root         (0)     7733 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_type.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/_util.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 20:31:35.000000 gensaschema-0.6.8/gensaschema/constraints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.006237 gensaschema-0.6.8/gensaschema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-07-11 20:32:24.000000 gensaschema-0.6.8/gensaschema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4057 2023-07-11 20:32:24.000000 gensaschema-0.6.8/gensaschema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 20:32:24.000000 gensaschema-0.6.8/gensaschema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:17:00.000000 gensaschema-0.6.8/gensaschema.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 20:32:24.000000 gensaschema-0.6.8/gensaschema.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 20:32:25.009237 gensaschema-0.6.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-07-03 20:15:43.000000 gensaschema-0.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.006237 gensaschema-0.6.8/tests/
+-rw-r--r--   0 root         (0) root         (0)      771 2023-07-03 20:15:43.000000 gensaschema-0.6.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2023-07-03 20:15:43.000000 gensaschema-0.6.8/tests/_util.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-07-03 20:15:43.000000 gensaschema-0.6.8/tests/coverage.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.007237 gensaschema-0.6.8/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-03 20:15:43.000000 gensaschema-0.6.8/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/integration/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/integration/test_table.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/integration/test_type.py
+-rw-r--r--   0 root         (0) root         (0)      764 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.008237 gensaschema-0.6.8/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-03 20:15:43.000000 gensaschema-0.6.8/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:32:25.008237 gensaschema-0.6.8/tests/unit/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-03 20:15:43.000000 gensaschema-0.6.8/tests/unit/fixtures/config1.schema
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/unit/test_column.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/unit/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/unit/test_template.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/unit/test_type.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-07-11 20:31:35.000000 gensaschema-0.6.8/tests/unit/test_util.py
```

### Comparing `gensaschema-0.6.7/LICENSE` & `gensaschema-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/PKG-INFO` & `gensaschema-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensaschema
-Version: 0.6.7
+Version: 0.6.8
 Summary: Static SQLAlchemy Schema Generator
 Home-page: http://opensource.perlig.de/gensaschema/
 Author: André Malo
 Author-email: nd@perlig.de
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gensaschema-0.6.7/README.md` & `gensaschema-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/CHANGES` & `gensaschema-0.6.8/docs/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Changes with version 0.6.8
+
+ *) Emit separate PG enum objects. Thanks to happyraul and armonge for the PRs.
+
+ *) Run black formatter
+
+ *) Update project boilerplate
+
+
 Changes with version 0.6.7
 
  *) Adaptions for SA 2.0
 
  *) Update project boilerplate
```

### Comparing `gensaschema-0.6.7/docs/CLASSIFIERS` & `gensaschema-0.6.8/docs/CLASSIFIERS`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/DESCRIPTION` & `gensaschema-0.6.8/docs/DESCRIPTION`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/DEVELOPMENT.md` & `gensaschema-0.6.8/docs/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_column.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_column.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._column &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._column &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._column</a></li> 
       </ul>
     </div>
     </div>
   
@@ -125,16 +124,15 @@
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Make string representation</span>
 
 <span class="sd">        Return:</span>
 <span class="sd">          str: The string representation</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">identity</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">_sa</span><span class="p">,</span> <span class="s1">&#39;Identity&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
-        <span class="k">if</span> <span class="n">identity</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> \
-                <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_default</span><span class="p">,</span> <span class="n">identity</span><span class="p">):</span>
+        <span class="k">if</span> <span class="n">identity</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_default</span><span class="p">,</span> <span class="n">identity</span><span class="p">):</span>
             <span class="k">return</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">.</span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;sa&#39;</span><span class="p">],</span>
                 <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_default</span><span class="p">),</span>
             <span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_default</span><span class="o">.</span><span class="n">for_update</span><span class="p">:</span>
             <span class="n">for_update</span> <span class="o">=</span> <span class="s2">&quot;, for_update=</span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="kc">True</span><span class="p">,)</span>
@@ -171,16 +169,24 @@
 <span class="sd">      _server_default (Default clause):</span>
 <span class="sd">        Default clause</span>
 
 <span class="sd">      _symbols (Symbols):</span>
 <span class="sd">        Symbol table</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
-<div class="viewcode-block" id="Column.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._column.html#gensaschema._column.Column.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">ctype</span><span class="p">,</span> <span class="n">nullable</span><span class="p">,</span> <span class="n">primary_key</span><span class="p">,</span> <span class="n">autoincrement</span><span class="p">,</span>
-                 <span class="n">server_default</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
+<div class="viewcode-block" id="Column.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._column.html#gensaschema._column.Column.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span>
+        <span class="n">name</span><span class="p">,</span>
+        <span class="n">ctype</span><span class="p">,</span>
+        <span class="n">nullable</span><span class="p">,</span>
+        <span class="n">primary_key</span><span class="p">,</span>
+        <span class="n">autoincrement</span><span class="p">,</span>
+        <span class="n">server_default</span><span class="p">,</span>
+        <span class="n">symbols</span><span class="p">,</span>
+    <span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Initialization</span>
 
 <span class="sd">        Parameters:</span>
 <span class="sd">          name (unicode):</span>
 <span class="sd">            Column name</span>
 
@@ -244,20 +250,19 @@
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">params</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="nb">repr</span><span class="p">,</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">)))</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">_nullable</span><span class="p">:</span>
             <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;nullable=</span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="kc">False</span><span class="p">,))</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">_autoincrement</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_primary_key</span><span class="p">:</span>
             <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;autoincrement=</span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="kc">False</span><span class="p">,))</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_server_default</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-            <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;server_default=</span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span>
-                <span class="n">ServerDefault</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_server_default</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">),</span>
-            <span class="p">))</span>
-        <span class="k">return</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">(</span><span class="si">%s</span><span class="s2">)&quot;</span> <span class="o">%</span> <span class="p">(</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;column&#39;</span><span class="p">],</span> <span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">params</span><span class="p">)</span>
-        <span class="p">)</span></div></div>
+            <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span>
+                <span class="s1">&#39;server_default=</span><span class="si">%r</span><span class="s1">&#39;</span>
+                <span class="o">%</span> <span class="p">(</span><span class="n">ServerDefault</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_server_default</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">),)</span>
+            <span class="p">)</span>
+        <span class="k">return</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">(</span><span class="si">%s</span><span class="s2">)&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;column&#39;</span><span class="p">],</span> <span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">params</span><span class="p">))</span></div></div>
 </pre></div>
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
@@ -297,22 +302,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._column</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._column
 ****** Source code for gensaschema._column ******
 # -*- coding: ascii -*-
 u"""
 ======================================
  Column inspection and representation
@@ -78,16 +78,15 @@
         """
         Make string representation
 
         Return:
           str: The string representation
         """
         identity = getattr(_sa, 'Identity', None)
-        if identity is not None \
-                and isinstance(self._default, identity):
+        if identity is not None and isinstance(self._default, identity):
             return "%s.%s" % (
                 self._symbols['sa'],
                 _util.unicode(self._default),
             )
 
         if self._default.for_update:
             for_update = ", for_update=%r" % (True,)
@@ -125,16 +124,24 @@
       _server_default (Default clause):
         Default clause
 
       _symbols (Symbols):
         Symbol table
     """
 
-[docs]    def __init__(self, name, ctype, nullable, primary_key, autoincrement,
-                 server_default, symbols):
+[docs]    def __init__(
+        self,
+        name,
+        ctype,
+        nullable,
+        primary_key,
+        autoincrement,
+        server_default,
+        symbols,
+    ):
         """
         Initialization
 
         Parameters:
           name (unicode):
             Column name
 
@@ -200,22 +207,21 @@
         """
         params = list(map(repr, (self._name, self._ctype)))
         if not self._nullable:
             params.append('nullable=%r' % (False,))
         if not self._autoincrement and self._primary_key:
             params.append('autoincrement=%r' % (False,))
         if self._server_default is not None:
-            params.append('server_default=%r' % (
-                ServerDefault(self._server_default, self._symbols),
-            ))
-        return "%s(%s)" % (
-            self._symbols['column'], ', '.join(params)
-        )
+            params.append(
+                'server_default=%r'
+                % (ServerDefault(self._server_default, self._symbols),)
+            )
+        return "%s(%s)" % (self._symbols['column'], ', '.join(params))
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._column
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_config.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_config.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._config &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._config &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._config</a></li> 
       </ul>
     </div>
     </div>
   
@@ -90,20 +89,20 @@
 <span class="n">__author__</span> <span class="o">=</span> <span class="sa">u</span><span class="s2">&quot;Andr</span><span class="se">\xe9</span><span class="s2"> Malo&quot;</span>
 
 <span class="kn">import</span> <span class="nn">errno</span> <span class="k">as</span> <span class="nn">_errno</span>
 
 <span class="k">if</span> <span class="mi">1</span><span class="p">:</span>
     <span class="k">try</span><span class="p">:</span>
         <span class="kn">import</span> <span class="nn">ConfigParser</span> <span class="k">as</span> <span class="nn">_config_parser</span>
-    <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+    <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
         <span class="kn">import</span> <span class="nn">configparser</span> <span class="k">as</span> <span class="nn">_config_parser</span>
 
     <span class="k">try</span><span class="p">:</span>
         <span class="kn">from</span> <span class="nn">cStringIO</span> <span class="kn">import</span> <span class="n">StringIO</span> <span class="k">as</span> <span class="n">_TextIO</span>
-    <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+    <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
         <span class="kn">from</span> <span class="nn">io</span> <span class="kn">import</span> <span class="n">StringIO</span> <span class="k">as</span> <span class="n">_TextIO</span>
 
 <span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">_template</span>
 
 
 <div class="viewcode-block" id="Config"><a class="viewcode-back" href="../../apidoc/gensaschema._config.html#gensaschema.Config">[docs]</a><span class="k">class</span> <span class="nc">Config</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
@@ -119,30 +118,32 @@
 <span class="sd">      _lines (list):</span>
 <span class="sd">        Original config lines (or ``None``)</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
     <span class="c1">#: Template for empty config file</span>
     <span class="c1">#:</span>
     <span class="c1">#: :Type: `Template`</span>
-    <span class="n">_CONFIG_TPL</span> <span class="o">=</span> <span class="n">_template</span><span class="o">.</span><span class="n">Template</span><span class="p">(</span><span class="s1">&#39;&#39;&#39;</span>
-<span class="s1">        # This is a comment. I love comments.</span>
-<span class="s1">        #</span>
-<span class="s1">        # This files contains table names, one per line</span>
-<span class="s1">        # Comments and empty lines are ignored</span>
-<span class="s1">        #</span>
-<span class="s1">        # If the table name contains a dot, the first part is treated as</span>
-<span class="s1">        # schema name.</span>
-<span class="s1">        #</span>
-<span class="s1">        # If the table variable should be treated differently, use:</span>
-<span class="s1">        #</span>
-<span class="s1">        # name = table</span>
-<span class="s1">        #</span>
-<span class="s1">        # The basename of this file (modulo .schema extension) is used as</span>
-<span class="s1">        # basename for the python file.</span>
-<span class="s1">    &#39;&#39;&#39;</span><span class="p">)</span>
+    <span class="n">_CONFIG_TPL</span> <span class="o">=</span> <span class="n">_template</span><span class="o">.</span><span class="n">Template</span><span class="p">(</span>
+<span class="w">        </span><span class="sd">&#39;&#39;&#39;</span>
+<span class="sd">        # This is a comment. I love comments.</span>
+<span class="sd">        #</span>
+<span class="sd">        # This files contains table names, one per line</span>
+<span class="sd">        # Comments and empty lines are ignored</span>
+<span class="sd">        #</span>
+<span class="sd">        # If the table name contains a dot, the first part is treated as</span>
+<span class="sd">        # schema name.</span>
+<span class="sd">        #</span>
+<span class="sd">        # If the table variable should be treated differently, use:</span>
+<span class="sd">        #</span>
+<span class="sd">        # name = table</span>
+<span class="sd">        #</span>
+<span class="sd">        # The basename of this file (modulo .schema extension) is used as</span>
+<span class="sd">        # basename for the python file.</span>
+<span class="sd">    &#39;&#39;&#39;</span>
+    <span class="p">)</span>
 
 <div class="viewcode-block" id="Config.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._config.html#gensaschema.Config.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tables</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">lines</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Initialization</span>
 
 <span class="sd">        Parameters:</span>
 <span class="sd">          tables (list):</span>
@@ -265,16 +266,18 @@
         <span class="k">if</span> <span class="ow">not</span> <span class="n">lines</span><span class="p">:</span>
             <span class="n">result</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_CONFIG_TPL</span><span class="o">.</span><span class="n">expand</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="kc">False</span><span class="p">)</span>
             <span class="k">if</span> <span class="n">lines</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
                 <span class="n">tables</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;</span><span class="si">%s</span><span class="s1"> = </span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">table</span> <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">tables</span><span class="p">]</span>
                 <span class="k">if</span> <span class="n">tables</span><span class="p">:</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">tables</span><span class="p">)</span>
-                <span class="n">schemas</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;</span><span class="si">%s</span><span class="s1"> = </span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">key</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
-                           <span class="k">for</span> <span class="n">key</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">schemas</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
+                <span class="n">schemas</span> <span class="o">=</span> <span class="p">[</span>
+                    <span class="s1">&#39;</span><span class="si">%s</span><span class="s1"> = </span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">key</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
+                    <span class="k">for</span> <span class="n">key</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">schemas</span><span class="o">.</span><span class="n">items</span><span class="p">()</span>
+                <span class="p">]</span>
                 <span class="k">if</span> <span class="n">schemas</span><span class="p">:</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;[schemas]&#39;</span><span class="p">)</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">schemas</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">result</span> <span class="o">=</span> <span class="n">lines</span>
 
@@ -327,22 +330,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._config</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._config
 ****** Source code for gensaschema._config ******
 # -*- coding: ascii -*-
 u"""
 ==========================
  Schema config management
@@ -42,20 +42,20 @@
 __author__ = u"Andr\xe9 Malo"
 
 import errno as _errno
 
 if 1:
     try:
         import ConfigParser as _config_parser
-    except ImportError:  # pragma: no cover
+    except ImportError:
         import configparser as _config_parser
 
     try:
         from cStringIO import StringIO as _TextIO
-    except ImportError:  # pragma: no cover
+    except ImportError:
         from io import StringIO as _TextIO
 
 from . import _template
 
 
 [docs]class Config(object):
     """
@@ -71,30 +71,32 @@
       _lines (list):
         Original config lines (or ``None``)
     """
 
     #: Template for empty config file
     #:
     #: :Type: `Template`
-    _CONFIG_TPL = _template.Template('''
+    _CONFIG_TPL = _template.Template(
+        '''
         # This is a comment. I love comments.
         #
         # This files contains table names, one per line
         # Comments and empty lines are ignored
         #
         # If the table name contains a dot, the first part is treated as
         # schema name.
         #
         # If the table variable should be treated differently, use:
         #
         # name = table
         #
         # The basename of this file (modulo .schema extension) is used as
         # basename for the python file.
-    ''')
+    '''
+    )
 
 [docs]    def __init__(self, tables, schemas, lines=None):
         """
         Initialization
 
         Parameters:
           tables (list):
@@ -221,16 +223,18 @@
         if not lines:
             result = self._CONFIG_TPL.expand().splitlines(False)
             if lines is None:
                 tables = ['%s = %s' % table for table in self.tables]
                 if tables:
                     result.append('')
                     result.extend(tables)
-                schemas = ['%s = %s' % (key, value)
-                           for key, value in self.schemas.items()]
+                schemas = [
+                    '%s = %s' % (key, value)
+                    for key, value in self.schemas.items()
+                ]
                 if schemas:
                     result.append('')
                     result.append('[schemas]')
                     result.extend(schemas)
         else:
             result = lines
 
@@ -241,11 +245,11 @@
             content = content.encode('utf-8')
         fp.write(content)
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._config
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_constraint.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_constraint.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._constraint &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._constraint &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._constraint</a></li> 
       </ul>
     </div>
     </div>
   
@@ -100,18 +99,19 @@
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Reflected Constraint</span>
 
 <span class="sd">    Attributes:</span>
 <span class="sd">      constraint (SA Constraint):</span>
 <span class="sd">        Constraint</span>
 <span class="sd">    &quot;&quot;&quot;</span>
+
     <span class="n">_SYMBOL</span><span class="p">,</span> <span class="n">_IMPORT</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="kc">None</span>
 
 <div class="viewcode-block" id="Constraint.__new__"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.Constraint.__new__">[docs]</a>    <span class="k">def</span> <span class="fm">__new__</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">constraint</span><span class="p">,</span> <span class="n">table</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot; Constraint factory &quot;&quot;&quot;</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Constraint factory&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">cls</span> <span class="o">==</span> <span class="n">Constraint</span><span class="p">:</span>
             <span class="n">name</span> <span class="o">=</span> <span class="n">constraint</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span>
             <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="s1">&#39;CheckConstraint&#39;</span><span class="p">:</span>
                 <span class="k">return</span> <span class="kc">None</span>
             <span class="k">return</span> <span class="nb">globals</span><span class="p">()[</span><span class="n">name</span><span class="p">](</span>
                 <span class="n">constraint</span><span class="p">,</span> <span class="n">table</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="n">options</span>
             <span class="p">)</span>
@@ -137,47 +137,52 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span> <span class="o">=</span> <span class="n">constraint</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">table</span> <span class="o">=</span> <span class="n">table</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span> <span class="o">=</span> <span class="n">symbols</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="o">.</span><span class="n">imports</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_SYMBOL</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_IMPORT</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">options</span> <span class="o">=</span> <span class="n">options</span></div>
 
 <div class="viewcode-block" id="Constraint.copy"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.Constraint.copy">[docs]</a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot; Create shallow copy &quot;&quot;&quot;</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Create shallow copy&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">table</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">options</span>
         <span class="p">)</span></div>
 
 <div class="viewcode-block" id="Constraint.__cmp__"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.Constraint.__cmp__">[docs]</a>    <span class="k">def</span> <span class="nf">__cmp__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot; Compare &quot;&quot;&quot;</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Compare&quot;&quot;&quot;</span>
         <span class="n">names</span> <span class="o">=</span> <span class="p">[</span>
-            <span class="s1">&#39;PrimaryKeyConstraint&#39;</span><span class="p">,</span> <span class="s1">&#39;UniqueConstraint&#39;</span><span class="p">,</span>
-            <span class="s1">&#39;ForeignKeyConstraint&#39;</span><span class="p">,</span> <span class="s1">&#39;CheckConstraint&#39;</span>
+            <span class="s1">&#39;PrimaryKeyConstraint&#39;</span><span class="p">,</span>
+            <span class="s1">&#39;UniqueConstraint&#39;</span><span class="p">,</span>
+            <span class="s1">&#39;ForeignKeyConstraint&#39;</span><span class="p">,</span>
+            <span class="s1">&#39;CheckConstraint&#39;</span><span class="p">,</span>
         <span class="p">]</span>
 
         <span class="k">def</span> <span class="nf">bytype</span><span class="p">(</span><span class="n">const</span><span class="p">):</span>
-<span class="w">            </span><span class="sd">&quot;&quot;&quot; Sort by type &quot;&quot;&quot;</span>
+<span class="w">            </span><span class="sd">&quot;&quot;&quot;Sort by type&quot;&quot;&quot;</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="k">return</span> <span class="n">names</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">const</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">)</span>
             <span class="k">except</span> <span class="ne">IndexError</span><span class="p">:</span>
                 <span class="k">return</span> <span class="o">-</span><span class="mi">1</span>
 
-        <span class="k">return</span> <span class="n">_util</span><span class="o">.</span><span class="n">cmp</span><span class="p">((</span>
-            <span class="n">bytype</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="p">),</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">options</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">,</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">name</span><span class="p">,</span>
-            <span class="nb">repr</span><span class="p">(</span><span class="bp">self</span><span class="p">),</span>
-        <span class="p">),</span> <span class="p">(</span>
-            <span class="n">bytype</span><span class="p">(</span><span class="n">other</span><span class="o">.</span><span class="n">constraint</span><span class="p">),</span>
-            <span class="n">other</span><span class="o">.</span><span class="n">options</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">,</span>
-            <span class="n">other</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">name</span><span class="p">,</span>
-            <span class="nb">repr</span><span class="p">(</span><span class="n">other</span><span class="p">),</span>
-        <span class="p">))</span></div>
+        <span class="k">return</span> <span class="n">_util</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span>
+            <span class="p">(</span>
+                <span class="n">bytype</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="p">),</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">options</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">,</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">name</span><span class="p">,</span>
+                <span class="nb">repr</span><span class="p">(</span><span class="bp">self</span><span class="p">),</span>
+            <span class="p">),</span>
+            <span class="p">(</span>
+                <span class="n">bytype</span><span class="p">(</span><span class="n">other</span><span class="o">.</span><span class="n">constraint</span><span class="p">),</span>
+                <span class="n">other</span><span class="o">.</span><span class="n">options</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">,</span>
+                <span class="n">other</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">name</span><span class="p">,</span>
+                <span class="nb">repr</span><span class="p">(</span><span class="n">other</span><span class="p">),</span>
+            <span class="p">),</span>
+        <span class="p">)</span></div>
 
 <div class="viewcode-block" id="Constraint.__lt__"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.Constraint.__lt__">[docs]</a>    <span class="k">def</span> <span class="fm">__lt__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">,</span> <span class="n">_cmp</span><span class="o">=</span><span class="n">__cmp__</span><span class="p">):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot; Check for &#39;&lt;&#39; &quot;&quot;&quot;</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Check for &#39;&lt;&#39;&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="n">_cmp</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">)</span> <span class="o">&lt;</span> <span class="mi">0</span></div>
 
 <div class="viewcode-block" id="Constraint.repr"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.Constraint.repr">[docs]</a>    <span class="k">def</span> <span class="nf">repr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">symbol</span><span class="p">,</span> <span class="n">args</span><span class="p">,</span> <span class="n">keywords</span><span class="o">=</span><span class="p">(),</span> <span class="n">short</span><span class="o">=</span><span class="kc">False</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Base repr for all constraints</span>
 
 <span class="sd">        Parameters:</span>
@@ -204,17 +209,17 @@
             <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;name=</span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">name</span><span class="p">,))</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">deferrable</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;deferrable=</span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">deferrable</span><span class="p">,))</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">initially</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;initially=</span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">initially</span><span class="p">,))</span>
         <span class="k">for</span> <span class="n">keyword</span> <span class="ow">in</span> <span class="n">keywords</span><span class="p">:</span>
             <span class="k">if</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="p">,</span> <span class="n">keyword</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-                <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="s2">=</span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span>
-                    <span class="n">keyword</span><span class="p">,</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="p">,</span> <span class="n">keyword</span><span class="p">)</span>
-                <span class="p">))</span>
+                <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span>
+                    <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">=</span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">keyword</span><span class="p">,</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="p">,</span> <span class="n">keyword</span><span class="p">))</span>
+                <span class="p">)</span>
         <span class="k">if</span> <span class="n">short</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">params</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
             <span class="n">short</span> <span class="o">=</span> <span class="kc">False</span>
         <span class="k">if</span> <span class="n">args</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">short</span><span class="p">:</span>
                 <span class="n">args</span> <span class="o">=</span> <span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
             <span class="k">else</span><span class="p">:</span>
                 <span class="n">args</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">    &#39;</span> <span class="o">+</span> <span class="s1">&#39;,</span><span class="se">\n</span><span class="s1">    &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">args</span><span class="p">)</span> <span class="o">+</span> <span class="s1">&#39;,&#39;</span>
@@ -247,99 +252,118 @@
 <span class="sd">      str: Access string</span>
 <span class="sd">    &quot;&quot;&quot;</span>
     <span class="k">try</span><span class="p">:</span>
         <span class="n">name</span> <span class="o">=</span> <span class="n">col</span><span class="o">.</span><span class="n">name</span>
     <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
         <span class="n">name</span> <span class="o">=</span> <span class="n">col</span>
     <span class="k">try</span><span class="p">:</span>
-        <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">bytes</span><span class="p">):</span>  <span class="c1"># pragma: no cover</span>
+        <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">bytes</span><span class="p">):</span>
             <span class="n">name</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">name</span><span class="o">.</span><span class="n">encode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
     <span class="k">except</span> <span class="ne">UnicodeError</span><span class="p">:</span>
         <span class="n">is_ascii</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="k">else</span><span class="p">:</span>
         <span class="n">is_ascii</span> <span class="o">=</span> <span class="kc">True</span>
-    <span class="k">if</span> <span class="n">is_ascii</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">_keyword</span><span class="o">.</span><span class="n">iskeyword</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="ow">and</span> \
-            <span class="n">_re</span><span class="o">.</span><span class="n">match</span><span class="p">(</span><span class="n">_tokenize</span><span class="o">.</span><span class="n">Name</span> <span class="o">+</span> <span class="s1">&#39;$&#39;</span><span class="p">,</span> <span class="n">name</span><span class="p">):</span>
+    <span class="k">if</span> <span class="p">(</span>
+        <span class="n">is_ascii</span>
+        <span class="ow">and</span> <span class="ow">not</span> <span class="n">_keyword</span><span class="o">.</span><span class="n">iskeyword</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+        <span class="ow">and</span> <span class="n">_re</span><span class="o">.</span><span class="n">match</span><span class="p">(</span><span class="n">_tokenize</span><span class="o">.</span><span class="n">Name</span> <span class="o">+</span> <span class="s1">&#39;$&#39;</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span>
+    <span class="p">):</span>
         <span class="k">return</span> <span class="s2">&quot;.c.</span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="n">name</span>
     <span class="k">return</span> <span class="s2">&quot;.c[</span><span class="si">%r</span><span class="s2">]&quot;</span> <span class="o">%</span> <span class="n">name</span></div>
 
 
 <div class="viewcode-block" id="UniqueConstraint"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.UniqueConstraint">[docs]</a><span class="k">class</span> <span class="nc">UniqueConstraint</span><span class="p">(</span><span class="n">Constraint</span><span class="p">):</span>
-<span class="w">    </span><span class="sd">&quot;&quot;&quot; Unique constraint &quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;Unique constraint&quot;&quot;&quot;</span>
+
     <span class="n">_SYMBOL</span> <span class="o">=</span> <span class="s1">&#39;uk&#39;</span>
     <span class="n">_IMPORT</span> <span class="o">=</span> <span class="s1">&#39;from </span><span class="si">%(constraints)s</span><span class="s1"> import Unique as </span><span class="si">%(uk)s</span><span class="s1">&#39;</span>
 
 <div class="viewcode-block" id="UniqueConstraint.__repr__"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.UniqueConstraint.__repr__">[docs]</a>    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Make string representation</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">          str: The string representation</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">empty</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span>
         <span class="n">short</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">&lt;=</span> <span class="mi">1</span>
-        <span class="n">result</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">repr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_SYMBOL</span><span class="p">,</span> <span class="p">[</span>
-            <span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">table</span><span class="p">,</span> <span class="n">access_col</span><span class="p">(</span><span class="n">col</span><span class="p">))</span>
-            <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">columns</span>
-        <span class="p">],</span> <span class="n">short</span><span class="o">=</span><span class="n">short</span><span class="p">)</span>
+        <span class="n">result</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">repr</span><span class="p">(</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_SYMBOL</span><span class="p">,</span>
+            <span class="p">[</span>
+                <span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">table</span><span class="p">,</span> <span class="n">access_col</span><span class="p">(</span><span class="n">col</span><span class="p">))</span>
+                <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">columns</span>
+            <span class="p">],</span>
+            <span class="n">short</span><span class="o">=</span><span class="n">short</span><span class="p">,</span>
+        <span class="p">)</span>
         <span class="k">if</span> <span class="n">empty</span><span class="p">:</span>
             <span class="n">result</span> <span class="o">=</span> <span class="s2">&quot;# </span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="n">result</span>
         <span class="k">return</span> <span class="n">result</span></div></div>
 
 
 <div class="viewcode-block" id="PrimaryKeyConstraint"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.PrimaryKeyConstraint">[docs]</a><span class="k">class</span> <span class="nc">PrimaryKeyConstraint</span><span class="p">(</span><span class="n">UniqueConstraint</span><span class="p">):</span>
-<span class="w">    </span><span class="sd">&quot;&quot;&quot; Primary Key constraint &quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;Primary Key constraint&quot;&quot;&quot;</span>
+
     <span class="n">_SYMBOL</span> <span class="o">=</span> <span class="s1">&#39;pk&#39;</span>
     <span class="n">_IMPORT</span> <span class="o">=</span> <span class="s1">&#39;from </span><span class="si">%(constraints)s</span><span class="s1"> import PrimaryKey as </span><span class="si">%(pk)s</span><span class="s1">&#39;</span></div>
 
 
 <div class="viewcode-block" id="ForeignKeyConstraint"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.ForeignKeyConstraint">[docs]</a><span class="k">class</span> <span class="nc">ForeignKeyConstraint</span><span class="p">(</span><span class="n">Constraint</span><span class="p">):</span>
-<span class="w">    </span><span class="sd">&quot;&quot;&quot; ForeignKey constraint &quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;ForeignKey constraint&quot;&quot;&quot;</span>
+
     <span class="n">_SYMBOL</span> <span class="o">=</span> <span class="s1">&#39;fk&#39;</span>
     <span class="n">_IMPORT</span> <span class="o">=</span> <span class="s1">&#39;from </span><span class="si">%(constraints)s</span><span class="s1"> import ForeignKey as </span><span class="si">%(fk)s</span><span class="s1">&#39;</span>
 
 <div class="viewcode-block" id="ForeignKeyConstraint.__repr__"><a class="viewcode-back" href="../../apidoc/gensaschema._constraint.html#gensaschema._constraint.ForeignKeyConstraint.__repr__">[docs]</a>    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Make string representation</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">          str: The string representation</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">columns</span> <span class="o">=</span> <span class="s2">&quot;[</span><span class="si">%s</span><span class="s2">]&quot;</span> <span class="o">%</span> <span class="s1">&#39;,</span><span class="se">\n</span><span class="s1">    &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span>
-            <span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">table</span><span class="p">,</span> <span class="n">access_col</span><span class="p">(</span><span class="n">col</span><span class="p">))</span>
-            <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">columns</span>
-        <span class="p">])</span>
-        <span class="n">refcolumns</span> <span class="o">=</span> <span class="s2">&quot;[</span><span class="si">%s</span><span class="s2">]&quot;</span> <span class="o">%</span> <span class="s1">&#39;,</span><span class="se">\n</span><span class="s1">    &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="sa">u</span><span class="s1">&#39;table_</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">key</span><span class="o">.</span><span class="n">column</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">name</span><span class="p">],</span>
-            <span class="n">access_col</span><span class="p">(</span><span class="n">key</span><span class="o">.</span><span class="n">column</span><span class="p">),</span>
-        <span class="p">)</span> <span class="k">for</span> <span class="n">key</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">elements</span><span class="p">])</span>
+        <span class="n">columns</span> <span class="o">=</span> <span class="s2">&quot;[</span><span class="si">%s</span><span class="s2">]&quot;</span> <span class="o">%</span> <span class="s1">&#39;,</span><span class="se">\n</span><span class="s1">    &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+            <span class="p">[</span>
+                <span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">table</span><span class="p">,</span> <span class="n">access_col</span><span class="p">(</span><span class="n">col</span><span class="p">))</span>
+                <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">columns</span>
+            <span class="p">]</span>
+        <span class="p">)</span>
+        <span class="n">refcolumns</span> <span class="o">=</span> <span class="s2">&quot;[</span><span class="si">%s</span><span class="s2">]&quot;</span> <span class="o">%</span> <span class="s1">&#39;,</span><span class="se">\n</span><span class="s1">    &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+            <span class="p">[</span>
+                <span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span>
+                <span class="o">%</span> <span class="p">(</span>
+                    <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="sa">u</span><span class="s1">&#39;table_</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">key</span><span class="o">.</span><span class="n">column</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">name</span><span class="p">],</span>
+                    <span class="n">access_col</span><span class="p">(</span><span class="n">key</span><span class="o">.</span><span class="n">column</span><span class="p">),</span>
+                <span class="p">)</span>
+                <span class="k">for</span> <span class="n">key</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">elements</span>
+            <span class="p">]</span>
+        <span class="p">)</span>
         <span class="n">keywords</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;onupdate&#39;</span><span class="p">,</span> <span class="s1">&#39;ondelete&#39;</span><span class="p">]</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">use_alter</span><span class="p">:</span>
             <span class="n">keywords</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;use_alter&#39;</span><span class="p">)</span>
         <span class="n">result</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">repr</span><span class="p">(</span><span class="s1">&#39;fk&#39;</span><span class="p">,</span> <span class="p">[</span><span class="n">columns</span><span class="p">,</span> <span class="n">refcolumns</span><span class="p">],</span> <span class="n">keywords</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">options</span><span class="p">:</span>
             <span class="n">cyclic</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">use_alter</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">options</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;seen:&#39;</span><span class="p">):</span>
                 <span class="n">table</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">options</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="mi">1</span><span class="p">)[</span><span class="mi">1</span><span class="p">]</span>
                 <span class="k">if</span> <span class="n">cyclic</span><span class="p">:</span>
                     <span class="n">result</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1"># Cyclic foreign key:</span><span class="se">\n</span><span class="s1">&#39;</span> <span class="o">+</span> <span class="n">result</span>
                 <span class="k">else</span><span class="p">:</span>
                     <span class="n">result</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1"># Foreign key belongs to </span><span class="si">%r</span><span class="s1">:</span><span class="se">\n</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span>
-                        <span class="n">table</span><span class="p">,</span> <span class="n">result</span>
+                        <span class="n">table</span><span class="p">,</span>
+                        <span class="n">result</span><span class="p">,</span>
                     <span class="p">)</span>
             <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">options</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;unseen:&#39;</span><span class="p">):</span>
                 <span class="n">table</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">options</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="mi">1</span><span class="p">)[</span><span class="mi">1</span><span class="p">]</span>
                 <span class="n">result</span> <span class="o">=</span> <span class="n">result</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
                 <span class="k">if</span> <span class="n">cyclic</span><span class="p">:</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span>
                         <span class="mi">0</span><span class="p">,</span>
-                        <span class="s1">&#39;Cyclic foreign key, defined at table </span><span class="si">%r</span><span class="s1">:</span><span class="se">\n</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">table</span>
+                        <span class="s1">&#39;Cyclic foreign key, defined at table </span><span class="si">%r</span><span class="s1">:</span><span class="se">\n</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">table</span><span class="p">,</span>
                     <span class="p">)</span>
                 <span class="k">else</span><span class="p">:</span>
                     <span class="n">result</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="s1">&#39;Defined at table </span><span class="si">%r</span><span class="s1">:</span><span class="se">\n</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">table</span><span class="p">)</span>
                 <span class="n">result</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span> <span class="o">+</span> <span class="s1">&#39;&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="s1">&#39;# </span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">item</span> <span class="k">for</span> <span class="n">item</span> <span class="ow">in</span> <span class="n">result</span><span class="p">])</span>
 
         <span class="k">return</span> <span class="n">result</span></div></div>
 </pre></div>
@@ -385,22 +409,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._constraint</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._constraint
 ****** Source code for gensaschema._constraint ******
 # -*- coding: ascii -*-
 u"""
 ==========================================
  Constraint inspection and representation
@@ -52,18 +52,19 @@
     """
     Reflected Constraint
 
     Attributes:
       constraint (SA Constraint):
         Constraint
     """
+
     _SYMBOL, _IMPORT = None, None
 
 [docs]    def __new__(cls, constraint, table, symbols, options=None):
-        """ Constraint factory """
+        """Constraint factory"""
         if cls == Constraint:
             name = constraint.__class__.__name__
             if name == 'CheckConstraint':
                 return None
             return globals()[name](
                 constraint, table, symbols, options=options
             )
@@ -91,49 +92,54 @@
         self.table = table
         self._symbols = symbols
         self._symbols.imports[self._SYMBOL] = self._IMPORT
         self.options = options
 
 
 [docs]    def copy(self):
-        """ Create shallow copy """
+        """Create shallow copy"""
         return self.__class__(
             self.constraint, self.table, self._symbols, self.options
         )
 
 
 [docs]    def __cmp__(self, other):
-        """ Compare """
+        """Compare"""
         names = [
-            'PrimaryKeyConstraint', 'UniqueConstraint',
-            'ForeignKeyConstraint', 'CheckConstraint'
+            'PrimaryKeyConstraint',
+            'UniqueConstraint',
+            'ForeignKeyConstraint',
+            'CheckConstraint',
         ]
 
         def bytype(const):
-            """ Sort by type """
+            """Sort by type"""
             try:
                 return names.index(const.__class__.__name__)
             except IndexError:
                 return -1
 
-        return _util.cmp((
-            bytype(self.constraint),
-            self.options is not None,
-            self.constraint.name,
-            repr(self),
-        ), (
-            bytype(other.constraint),
-            other.options is not None,
-            other.constraint.name,
-            repr(other),
-        ))
+        return _util.cmp(
+            (
+                bytype(self.constraint),
+                self.options is not None,
+                self.constraint.name,
+                repr(self),
+            ),
+            (
+                bytype(other.constraint),
+                other.options is not None,
+                other.constraint.name,
+                repr(other),
+            ),
+        )
 
 
 [docs]    def __lt__(self, other, _cmp=__cmp__):
-        """ Check for '<' """
+        """Check for '<'"""
         return _cmp(self, other) < 0
 
 
 [docs]    def repr(self, symbol, args, keywords=(), short=False):
         """
         Base repr for all constraints
 
@@ -161,17 +167,17 @@
             params.append('name=%r' % (self.constraint.name,))
         if self.constraint.deferrable is not None:
             params.append('deferrable=%r' % (self.constraint.deferrable,))
         if self.constraint.initially is not None:
             params.append('initially=%r' % (self.constraint.initially,))
         for keyword in keywords:
             if getattr(self.constraint, keyword) is not None:
-                params.append("%s=%r" % (
-                    keyword, getattr(self.constraint, keyword)
-                ))
+                params.append(
+                    "%s=%r" % (keyword, getattr(self.constraint, keyword))
+                )
         if short and len(params) > 1:
             short = False
         if args:
             if short:
                 args = ', '.join(args)
             else:
                 args = '\n    ' + ',\n    '.join(args) + ','
@@ -205,110 +211,129 @@
       str: Access string
     """
     try:
         name = col.name
     except AttributeError:
         name = col
     try:
-        if _util.py2 and isinstance(name, _util.bytes):  # pragma: no cover
+        if _util.py2 and isinstance(name, _util.bytes):
             name.decode('ascii')
         else:
             name.encode('ascii')
     except UnicodeError:
         is_ascii = False
     else:
         is_ascii = True
-    if is_ascii and not _keyword.iskeyword(name) and \
-            _re.match(_tokenize.Name + '$', name):
+    if (
+        is_ascii
+        and not _keyword.iskeyword(name)
+        and _re.match(_tokenize.Name + '$', name)
+    ):
         return ".c.%s" % name
     return ".c[%r]" % name
 
 
 
 [docs]class UniqueConstraint(Constraint):
-    """ Unique constraint """
+    """Unique constraint"""
+
     _SYMBOL = 'uk'
     _IMPORT = 'from %(constraints)s import Unique as %(uk)s'
 
 [docs]    def __repr__(self):
         """
         Make string representation
 
         Returns:
           str: The string representation
         """
         empty = len(self.constraint.columns) == 0
         short = len(self.constraint.columns) <= 1
-        result = self.repr(self._SYMBOL, [
-            "%s%s" % (self.table, access_col(col))
-            for col in self.constraint.columns
-        ], short=short)
+        result = self.repr(
+            self._SYMBOL,
+            [
+                "%s%s" % (self.table, access_col(col))
+                for col in self.constraint.columns
+            ],
+            short=short,
+        )
         if empty:
             result = "# %s" % result
         return result
 
 
 
 [docs]class PrimaryKeyConstraint(UniqueConstraint):
-    """ Primary Key constraint """
+    """Primary Key constraint"""
+
     _SYMBOL = 'pk'
     _IMPORT = 'from %(constraints)s import PrimaryKey as %(pk)s'
 
 
 
 [docs]class ForeignKeyConstraint(Constraint):
-    """ ForeignKey constraint """
+    """ForeignKey constraint"""
+
     _SYMBOL = 'fk'
     _IMPORT = 'from %(constraints)s import ForeignKey as %(fk)s'
 
 [docs]    def __repr__(self):
         """
         Make string representation
 
         Returns:
           str: The string representation
         """
-        columns = "[%s]" % ',\n    '.join([
-            "%s%s" % (self.table, access_col(col))
-            for col in self.constraint.columns
-        ])
-        refcolumns = "[%s]" % ',\n    '.join(["%s%s" % (
-            self._symbols[u'table_%s' % key.column.table.name],
-            access_col(key.column),
-        ) for key in self.constraint.elements])
+        columns = "[%s]" % ',\n    '.join(
+            [
+                "%s%s" % (self.table, access_col(col))
+                for col in self.constraint.columns
+            ]
+        )
+        refcolumns = "[%s]" % ',\n    '.join(
+            [
+                "%s%s"
+                % (
+                    self._symbols[u'table_%s' % key.column.table.name],
+                    access_col(key.column),
+                )
+                for key in self.constraint.elements
+            ]
+        )
         keywords = ['onupdate', 'ondelete']
         if self.constraint.use_alter:
             keywords.append('use_alter')
         result = self.repr('fk', [columns, refcolumns], keywords)
 
         if self.options:
             cyclic = self.constraint.use_alter
             if self.options.startswith('seen:'):
                 table = self.options.split(None, 1)[1]
                 if cyclic:
                     result = '\n# Cyclic foreign key:\n' + result
                 else:
                     result = '\n# Foreign key belongs to %r:\n%s' % (
-                        table, result
+                        table,
+                        result,
                     )
             elif self.options.startswith('unseen:'):
                 table = self.options.split(None, 1)[1]
                 result = result.splitlines(True)
                 if cyclic:
                     result.insert(
                         0,
-                        'Cyclic foreign key, defined at table %r:\n' % table
+                        'Cyclic foreign key, defined at table %r:\n' % table,
                     )
                 else:
                     result.insert(0, 'Defined at table %r:\n' % table)
                 result = '\n' + ''.join(['# %s' % item for item in result])
 
         return result
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._constraint
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_exceptions.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_exceptions.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._exceptions &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._exceptions &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._exceptions</a></li> 
       </ul>
     </div>
     </div>
   
@@ -89,18 +88,20 @@
 <span class="sd">&quot;&quot;&quot;</span>
 <span class="n">__author__</span> <span class="o">=</span> <span class="sa">u</span><span class="s2">&quot;Andr</span><span class="se">\xe9</span><span class="s2"> Malo&quot;</span>
 
 <span class="kn">import</span> <span class="nn">warnings</span> <span class="k">as</span> <span class="nn">_warnings</span>
 
 
 <div class="viewcode-block" id="Error"><a class="viewcode-back" href="../../apidoc/gensaschema._exceptions.html#gensaschema.Error">[docs]</a><span class="k">class</span> <span class="nc">Error</span><span class="p">(</span><span class="ne">Exception</span><span class="p">):</span>
-<span class="w">    </span><span class="sd">&quot;&quot;&quot; Base exception for this package &quot;&quot;&quot;</span></div>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;Base exception for this package&quot;&quot;&quot;</span></div>
 
 
-<div class="viewcode-block" id="Warning"><a class="viewcode-back" href="../../apidoc/gensaschema._exceptions.html#gensaschema.Warning">[docs]</a><span class="k">class</span> <span class="nc">Warning</span><span class="p">(</span><span class="ne">Warning</span><span class="p">):</span>  <span class="c1"># noqa pylint: disable = redefined-builtin, undefined-variable</span>
+<div class="viewcode-block" id="Warning"><a class="viewcode-back" href="../../apidoc/gensaschema._exceptions.html#gensaschema.Warning">[docs]</a><span class="k">class</span> <span class="nc">Warning</span><span class="p">(</span>
+    <span class="ne">Warning</span>
+<span class="p">):</span>  <span class="c1"># noqa pylint: disable = redefined-builtin, undefined-variable</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Base warning for this package</span>
 
 <span class="sd">    &gt;&gt;&gt; with _warnings.catch_warnings(record=True) as record:</span>
 <span class="sd">    ...     Warning.emit(&#39;my message&#39;)</span>
 <span class="sd">    ...     assert len(record) == 1</span>
 <span class="sd">    ...     str(record[0].message)</span>
@@ -110,15 +111,15 @@
 <span class="sd">    &gt;&gt;&gt; Warning.emit(&#39;lalala&#39;)</span>
 <span class="sd">    Traceback (most recent call last):</span>
 <span class="sd">    ...</span>
 <span class="sd">    Warning: lalala</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
 <div class="viewcode-block" id="Warning.emit"><a class="viewcode-back" href="../../apidoc/gensaschema._exceptions.html#gensaschema.Warning.emit">[docs]</a>    <span class="nd">@classmethod</span>
-    <span class="k">def</span> <span class="nf">emit</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">message</span><span class="p">,</span> <span class="n">stacklevel</span><span class="o">=</span><span class="mi">1</span><span class="p">):</span>  <span class="c1"># pragma: no cover</span>
+    <span class="k">def</span> <span class="nf">emit</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">message</span><span class="p">,</span> <span class="n">stacklevel</span><span class="o">=</span><span class="mi">1</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Emit a warning of this very category</span>
 
 <span class="sd">        This method is pure convenience. It saves you the unfriendly</span>
 <span class="sd">        ``warnings.warn`` syntax (and the ``warnings`` import).</span>
 
 <span class="sd">        :Parameters:</span>
@@ -177,22 +178,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._exceptions</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._exceptions
 ****** Source code for gensaschema._exceptions ******
 # -*- coding: ascii -*-
 u"""
 :Copyright:
 
@@ -41,20 +41,21 @@
 """
 __author__ = u"Andr\xe9 Malo"
 
 import warnings as _warnings
 
 
 [docs]class Error(Exception):
-    """ Base exception for this package """
+    """Base exception for this package"""
 
 
 
-[docs]class Warning(Warning):  # noqa pylint: disable = redefined-builtin,
-undefined-variable
+[docs]class Warning(
+    Warning
+):  # noqa pylint: disable = redefined-builtin, undefined-variable
     """
     Base warning for this package
 
     >>> with _warnings.catch_warnings(record=True) as record:
     ...     Warning.emit('my message')
     ...     assert len(record) == 1
     ...     str(record[0].message)
@@ -64,15 +65,15 @@
     >>> Warning.emit('lalala')
     Traceback (most recent call last):
     ...
     Warning: lalala
     """
 
 [docs]    @classmethod
-    def emit(cls, message, stacklevel=1):  # pragma: no cover
+    def emit(cls, message, stacklevel=1):
         """
         Emit a warning of this very category
 
         This method is pure convenience. It saves you the unfriendly
         ``warnings.warn`` syntax (and the ``warnings`` import).
 
         :Parameters:
@@ -89,11 +90,11 @@
         # the stack magic.
         _warnings.warn(message, cls, max(1, stacklevel) + 1)
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._exceptions
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_meta.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_meta.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._meta &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._meta &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._meta</a></li> 
       </ul>
     </div>
     </div>
   
@@ -92,14 +91,15 @@
 <span class="kn">import</span> <span class="nn">sqlalchemy</span> <span class="k">as</span> <span class="nn">_sa</span>
 
 
 <div class="viewcode-block" id="BoundMetaData"><a class="viewcode-back" href="../../apidoc/gensaschema._meta.html#gensaschema._meta.BoundMetaData">[docs]</a><span class="k">class</span> <span class="nc">BoundMetaData</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Bound metadata proxy - SA 2.0 removed the bind, but it&#39;s part of our APIs</span>
 <span class="sd">    &quot;&quot;&quot;</span>
+
 <div class="viewcode-block" id="BoundMetaData.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._meta.html#gensaschema._meta.BoundMetaData.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">bind</span><span class="p">):</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_metadata</span> <span class="o">=</span> <span class="n">_sa</span><span class="o">.</span><span class="n">MetaData</span><span class="p">()</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">bind</span> <span class="o">=</span> <span class="n">bind</span></div>
 
 <div class="viewcode-block" id="BoundMetaData.__getattr__"><a class="viewcode-back" href="../../apidoc/gensaschema._meta.html#gensaschema._meta.BoundMetaData.__getattr__">[docs]</a>    <span class="k">def</span> <span class="fm">__getattr__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">):</span>
         <span class="k">return</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_metadata</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span></div></div>
 </pre></div>
@@ -145,22 +145,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._meta</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._meta
 ****** Source code for gensaschema._meta ******
 # -*- coding: ascii -*-
 u"""
 ==========
  Metadata
@@ -44,23 +44,24 @@
 import sqlalchemy as _sa
 
 
 [docs]class BoundMetaData(object):
     """
     Bound metadata proxy - SA 2.0 removed the bind, but it's part of our APIs
     """
+
 [docs]    def __init__(self, bind):
         self._metadata = _sa.MetaData()
         self.bind = bind
 
 
 [docs]    def __getattr__(self, name):
         return getattr(self._metadata, name)
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._meta
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_schema.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_schema.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._schema &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._schema &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._schema</a></li> 
       </ul>
     </div>
     </div>
   
@@ -114,42 +113,45 @@
 <span class="sd">      _dbname (str or None):</span>
 <span class="sd">        DB identifier</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
     <span class="c1">#: Template for the module</span>
     <span class="c1">#:</span>
     <span class="c1">#: :Type: Template</span>
-    <span class="n">_MODULE_TPL</span> <span class="o">=</span> <span class="n">_template</span><span class="o">.</span><span class="n">Template</span><span class="p">(</span><span class="s1">&#39;&#39;&#39;</span>
-<span class="s1">        # -*- coding: ascii -*-</span>
-<span class="s1">        # flake8: noqa pylint: skip-file</span>
-<span class="s1">        &quot;&quot;&quot;</span>
-<span class="s1">        ==============================</span>
-<span class="s1">         SQLAlchemy schema definition</span>
-<span class="s1">        ==============================</span>
-
-<span class="s1">        SQLAlchemy schema definition</span><span class="si">%(dbspec)s</span><span class="s1">.</span>
-
-<span class="s1">        :Warning: DO NOT EDIT, this file is generated</span>
-<span class="s1">        &quot;&quot;&quot;</span>
-
-<span class="s1">        import sqlalchemy as </span><span class="si">%(sa)s</span>
-<span class="s1">        from sqlalchemy.dialects import </span><span class="si">%(dialect)s</span><span class="s1"> as </span><span class="si">%(type)s</span>
-<span class="s1">        </span><span class="si">%(imports)s</span>
-<span class="s1">        </span><span class="si">%(meta)s</span><span class="s1"> = </span><span class="si">%(sa)s</span><span class="s1">.MetaData()</span>
-<span class="s1">        </span><span class="si">%(table)s</span><span class="s1"> = </span><span class="si">%(sa)s</span><span class="s1">.Table</span>
-<span class="s1">        </span><span class="si">%(column)s</span><span class="s1"> = </span><span class="si">%(sa)s</span><span class="s1">.Column</span>
-<span class="s1">        </span><span class="si">%(default)s</span><span class="s1"> = </span><span class="si">%(sa)s</span><span class="s1">.DefaultClause</span>
-<span class="s1">        </span><span class="si">%(lines)s</span>
-<span class="s1">        del </span><span class="si">%(sa)s</span><span class="s1">, </span><span class="si">%(table)s</span><span class="s1">, </span><span class="si">%(column)s</span><span class="s1">, </span><span class="si">%(default)s</span><span class="s1">, </span><span class="si">%(meta)s</span>
+    <span class="n">_MODULE_TPL</span> <span class="o">=</span> <span class="n">_template</span><span class="o">.</span><span class="n">Template</span><span class="p">(</span>
+<span class="w">        </span><span class="sd">&#39;&#39;&#39;</span>
+<span class="sd">        # -*- coding: ascii -*-</span>
+<span class="sd">        # flake8: noqa pylint: skip-file</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+<span class="sd">        ==============================</span>
+<span class="sd">         SQLAlchemy schema definition</span>
+<span class="sd">        ==============================</span>
+
+<span class="sd">        SQLAlchemy schema definition%(dbspec)s.</span>
 
-<span class="s1">        # vim: nowrap tw=0</span>
-<span class="s1">    &#39;&#39;&#39;</span><span class="p">)</span>
+<span class="sd">        :Warning: DO NOT EDIT, this file is generated</span>
+<span class="sd">        &quot;&quot;&quot;</span>
 
-<div class="viewcode-block" id="Schema.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._schema.html#gensaschema.Schema.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">conn</span><span class="p">,</span> <span class="n">tables</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">dbname</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-                 <span class="n">types</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+<span class="sd">        import sqlalchemy as %(sa)s</span>
+<span class="sd">        from sqlalchemy.dialects import %(dialect)s as %(type)s</span>
+<span class="sd">        %(imports)s</span>
+<span class="sd">        %(meta)s = %(sa)s.MetaData()</span>
+<span class="sd">        %(table)s = %(sa)s.Table</span>
+<span class="sd">        %(column)s = %(sa)s.Column</span>
+<span class="sd">        %(default)s = %(sa)s.DefaultClause</span>
+<span class="sd">        %(lines)s</span>
+<span class="sd">        del %(sa)s, %(table)s, %(column)s, %(default)s, %(meta)s</span>
+
+<span class="sd">        # vim: nowrap tw=0</span>
+<span class="sd">    &#39;&#39;&#39;</span>
+    <span class="p">)</span>
+
+<div class="viewcode-block" id="Schema.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._schema.html#gensaschema.Schema.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span> <span class="n">conn</span><span class="p">,</span> <span class="n">tables</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">dbname</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">types</span><span class="o">=</span><span class="kc">None</span>
+    <span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Initialization</span>
 
 <span class="sd">        Parameters:</span>
 <span class="sd">          conn (Connection or Engine):</span>
 <span class="sd">            SQLAlchemy connection or engine</span>
 
@@ -187,49 +189,53 @@
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Dump schema module to fp</span>
 
 <span class="sd">        Parameters:</span>
 <span class="sd">          fp (file):</span>
 <span class="sd">            File to write to</span>
 <span class="sd">        &quot;&quot;&quot;</span>
+        <span class="n">lines</span><span class="p">,</span> <span class="n">dlines</span> <span class="o">=</span> <span class="p">[],</span> <span class="p">[]</span>
+        <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_tables</span><span class="p">:</span>
+            <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">is_reference</span><span class="p">:</span>
+                <span class="k">continue</span>
+            <span class="n">name</span> <span class="o">=</span> <span class="n">table</span><span class="o">.</span><span class="n">sa_table</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">encode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">,</span> <span class="s1">&#39;backslashescape&#39;</span><span class="p">)</span>
+            <span class="k">if</span> <span class="nb">bytes</span> <span class="ow">is</span> <span class="ow">not</span> <span class="nb">str</span><span class="p">:</span>
+                <span class="n">name</span> <span class="o">=</span> <span class="n">name</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
+            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;# Table &quot;</span><span class="si">%s</span><span class="s1">&quot;&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">name</span><span class="p">,))</span>
+            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;</span><span class="si">%s</span><span class="s1"> = </span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">table</span><span class="o">.</span><span class="n">varname</span><span class="p">,</span> <span class="n">table</span><span class="p">))</span>
+            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
+            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
+
         <span class="n">imports</span> <span class="o">=</span> <span class="p">[</span><span class="n">item</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span> <span class="k">for</span> <span class="n">item</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="o">.</span><span class="n">imports</span><span class="p">]</span>
         <span class="k">if</span> <span class="n">imports</span><span class="p">:</span>  <span class="c1"># pragma: no branch</span>
             <span class="n">imports</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
             <span class="n">imports</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
-        <span class="n">lines</span> <span class="o">=</span> <span class="p">[]</span>
 
         <span class="n">defines</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">defines</span>
         <span class="k">if</span> <span class="n">defines</span><span class="p">:</span>
             <span class="n">defined</span> <span class="o">=</span> <span class="p">[]</span>
+            <span class="n">seen</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
             <span class="k">for</span> <span class="n">define</span> <span class="ow">in</span> <span class="n">defines</span><span class="p">:</span>
-                <span class="n">defined</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">define</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">))</span>
+                <span class="k">for</span> <span class="n">item</span> <span class="ow">in</span> <span class="n">define</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">):</span>
+                    <span class="k">if</span> <span class="n">item</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">seen</span><span class="p">:</span>
+                        <span class="n">defined</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">item</span><span class="p">)</span>
+                        <span class="n">seen</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">item</span><span class="p">)</span>
             <span class="k">if</span> <span class="n">defined</span><span class="p">:</span>
-                <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
-                <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;# Custom type definitions&#39;</span><span class="p">)</span>
-                <span class="n">lines</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">defined</span><span class="p">)</span>
-                <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
+                <span class="n">dlines</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;&#39;</span><span class="p">,</span> <span class="s1">&#39;# Custom type definitions&#39;</span><span class="p">]</span> <span class="o">+</span> <span class="n">defined</span>
 
-        <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_tables</span><span class="p">:</span>
-            <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">is_reference</span><span class="p">:</span>
-                <span class="k">continue</span>
-            <span class="k">if</span> <span class="ow">not</span> <span class="n">lines</span><span class="p">:</span>
-                <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
-            <span class="n">name</span> <span class="o">=</span> <span class="n">table</span><span class="o">.</span><span class="n">sa_table</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">encode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">,</span> <span class="s1">&#39;backslashescape&#39;</span><span class="p">)</span>
-            <span class="k">if</span> <span class="nb">bytes</span> <span class="ow">is</span> <span class="ow">not</span> <span class="nb">str</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
-                <span class="n">name</span> <span class="o">=</span> <span class="n">name</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
-            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;# Table &quot;</span><span class="si">%s</span><span class="s1">&quot;&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">name</span><span class="p">,))</span>
-            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;</span><span class="si">%s</span><span class="s1"> = </span><span class="si">%r</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">table</span><span class="o">.</span><span class="n">varname</span><span class="p">,</span> <span class="n">table</span><span class="p">))</span>
-            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
-            <span class="n">lines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">lines</span><span class="p">:</span>
+            <span class="n">dlines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
 
-        <span class="n">param</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">(((</span><span class="nb">str</span><span class="p">(</span><span class="n">key</span><span class="p">),</span> <span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">key</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">),</span>
-                     <span class="n">dbspec</span><span class="o">=</span><span class="s2">&quot; for </span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dbname</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dbname</span> <span class="k">else</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-                     <span class="n">dialect</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span>
-                     <span class="n">imports</span><span class="o">=</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">imports</span><span class="p">),</span>
-                     <span class="n">lines</span><span class="o">=</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">lines</span><span class="p">))</span>
+        <span class="n">param</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">(</span>
+            <span class="p">((</span><span class="nb">str</span><span class="p">(</span><span class="n">key</span><span class="p">),</span> <span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">key</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">),</span>
+            <span class="n">dbspec</span><span class="o">=</span><span class="s2">&quot; for </span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dbname</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dbname</span> <span class="k">else</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+            <span class="n">dialect</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span>
+            <span class="n">imports</span><span class="o">=</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">imports</span><span class="p">),</span>
+            <span class="n">lines</span><span class="o">=</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">dlines</span> <span class="o">+</span> <span class="n">lines</span><span class="p">),</span>
+        <span class="p">)</span>
         <span class="n">fp</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_MODULE_TPL</span><span class="o">.</span><span class="n">expand</span><span class="p">(</span><span class="o">**</span><span class="n">param</span><span class="p">))</span>
         <span class="n">fp</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="p">)</span></div></div>
 </pre></div>
 
             <div class="clearer"></div>
           </div>
         </div>
@@ -271,22 +277,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._schema</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._schema
 ****** Source code for gensaschema._schema ******
 # -*- coding: ascii -*-
 u"""
 ==========================
  Schema module generation
@@ -66,15 +66,16 @@
       _dbname (str or None):
         DB identifier
     """
 
     #: Template for the module
     #:
     #: :Type: Template
-    _MODULE_TPL = _template.Template('''
+    _MODULE_TPL = _template.Template(
+        '''
         # -*- coding: ascii -*-
         # flake8: noqa pylint: skip-file
         """
         ==============================
          SQLAlchemy schema definition
         ==============================
 
@@ -90,18 +91,20 @@
         %(table)s = %(sa)s.Table
         %(column)s = %(sa)s.Column
         %(default)s = %(sa)s.DefaultClause
         %(lines)s
         del %(sa)s, %(table)s, %(column)s, %(default)s, %(meta)s
 
         # vim: nowrap tw=0
-    ''')
+    '''
+    )
 
-[docs]    def __init__(self, conn, tables, schemas, symbols, dbname=None,
-                 types=None):
+[docs]    def __init__(
+        self, conn, tables, schemas, symbols, dbname=None, types=None
+    ):
         """
         Initialization
 
         Parameters:
           conn (Connection or Engine):
             SQLAlchemy connection or engine
 
@@ -140,53 +143,57 @@
         """
         Dump schema module to fp
 
         Parameters:
           fp (file):
             File to write to
         """
+        lines, dlines = [], []
+        for table in self._tables:
+            if table.is_reference:
+                continue
+            name = table.sa_table.name.encode('ascii', 'backslashescape')
+            if bytes is not str:
+                name = name.decode('ascii')
+            lines.append('# Table "%s"' % (name,))
+            lines.append('%s = %r' % (table.varname, table))
+            lines.append('')
+            lines.append('')
+
         imports = [item % self._symbols for item in self._symbols.imports]
         if imports:  # pragma: no branch
             imports.sort()
             imports.append('')
-        lines = []
 
         defines = self._symbols.types.defines
         if defines:
             defined = []
+            seen = set()
             for define in defines:
-                defined.extend(define(self._dialect, self._symbols))
+                for item in define(self._dialect, self._symbols):
+                    if item not in seen:
+                        defined.append(item)
+                        seen.add(item)
             if defined:
-                lines.append('')
-                lines.append('# Custom type definitions')
-                lines.extend(defined)
-                lines.append('')
+                dlines = ['', '# Custom type definitions'] + defined
 
-        for table in self._tables:
-            if table.is_reference:
-                continue
-            if not lines:
-                lines.append('')
-            name = table.sa_table.name.encode('ascii', 'backslashescape')
-            if bytes is not str:  # pragma: no cover
-                name = name.decode('ascii')
-            lines.append('# Table "%s"' % (name,))
-            lines.append('%s = %r' % (table.varname, table))
-            lines.append('')
-            lines.append('')
+        if lines:
+            dlines.append('')
 
-        param = dict(((str(key), value) for key, value in self._symbols),
-                     dbspec=" for %s" % self._dbname if self._dbname else "",
-                     dialect=self._dialect,
-                     imports='\n'.join(imports),
-                     lines='\n'.join(lines))
+        param = dict(
+            ((str(key), value) for key, value in self._symbols),
+            dbspec=" for %s" % self._dbname if self._dbname else "",
+            dialect=self._dialect,
+            imports='\n'.join(imports),
+            lines='\n'.join(dlines + lines),
+        )
         fp.write(self._MODULE_TPL.expand(**param))
         fp.write('\n')
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._schema
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_symbols.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_symbols.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._symbols &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._symbols &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._symbols</a></li> 
       </ul>
     </div>
     </div>
   
@@ -94,15 +93,15 @@
 <span class="kn">import</span> <span class="nn">weakref</span> <span class="k">as</span> <span class="nn">_weakref</span>
 
 <span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">_exceptions</span>
 <span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">_util</span>
 
 
 <div class="viewcode-block" id="SymbolException"><a class="viewcode-back" href="../../apidoc/gensaschema._symbols.html#gensaschema.SymbolException">[docs]</a><span class="k">class</span> <span class="nc">SymbolException</span><span class="p">(</span><span class="n">_exceptions</span><span class="o">.</span><span class="n">Error</span><span class="p">):</span>
-<span class="w">    </span><span class="sd">&quot;&quot;&quot; Symbol error &quot;&quot;&quot;</span></div>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;Symbol error&quot;&quot;&quot;</span></div>
 
 
 <div class="viewcode-block" id="Symbols"><a class="viewcode-back" href="../../apidoc/gensaschema._symbols.html#gensaschema.Symbols">[docs]</a><span class="k">class</span> <span class="nc">Symbols</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Symbol table</span>
 
 <span class="sd">    Attributes:</span>
@@ -126,24 +125,24 @@
 
 <span class="sd">          imports (iterable):</span>
 <span class="sd">            List of initial (id, import statement) tuples. If omitted or</span>
 <span class="sd">            ``None``, it&#39;s empty.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span> <span class="o">=</span> <span class="p">{}</span>
         <span class="n">defaults</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">(</span>
-            <span class="n">sa</span><span class="o">=</span><span class="s2">&quot;_sa&quot;</span><span class="p">,</span>          <span class="c1"># SQLAlchemy shortname</span>
-            <span class="n">meta</span><span class="o">=</span><span class="s2">&quot;m&quot;</span><span class="p">,</span>          <span class="c1"># MetaData shortname</span>
-            <span class="n">table</span><span class="o">=</span><span class="s2">&quot;T&quot;</span><span class="p">,</span>         <span class="c1"># Table shortname</span>
-            <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;t&quot;</span><span class="p">,</span>          <span class="c1"># Type module shortname</span>
-            <span class="n">column</span><span class="o">=</span><span class="s2">&quot;C&quot;</span><span class="p">,</span>        <span class="c1"># Column shortname</span>
-            <span class="n">default</span><span class="o">=</span><span class="s2">&quot;D&quot;</span><span class="p">,</span>       <span class="c1"># DefaultClause shortname</span>
-            <span class="n">pk</span><span class="o">=</span><span class="s2">&quot;PrimaryKey&quot;</span><span class="p">,</span>   <span class="c1"># PrimaryKey function name</span>
-            <span class="n">fk</span><span class="o">=</span><span class="s2">&quot;ForeignKey&quot;</span><span class="p">,</span>   <span class="c1"># ForeignKey function name</span>
-            <span class="n">uk</span><span class="o">=</span><span class="s2">&quot;Unique&quot;</span><span class="p">,</span>       <span class="c1"># UniqueKey function name</span>
-            <span class="n">constraints</span><span class="o">=</span><span class="p">(</span>      <span class="c1"># constraint function module</span>
+            <span class="n">sa</span><span class="o">=</span><span class="s2">&quot;_sa&quot;</span><span class="p">,</span>  <span class="c1"># SQLAlchemy shortname</span>
+            <span class="n">meta</span><span class="o">=</span><span class="s2">&quot;m&quot;</span><span class="p">,</span>  <span class="c1"># MetaData shortname</span>
+            <span class="n">table</span><span class="o">=</span><span class="s2">&quot;T&quot;</span><span class="p">,</span>  <span class="c1"># Table shortname</span>
+            <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;t&quot;</span><span class="p">,</span>  <span class="c1"># Type module shortname</span>
+            <span class="n">column</span><span class="o">=</span><span class="s2">&quot;C&quot;</span><span class="p">,</span>  <span class="c1"># Column shortname</span>
+            <span class="n">default</span><span class="o">=</span><span class="s2">&quot;D&quot;</span><span class="p">,</span>  <span class="c1"># DefaultClause shortname</span>
+            <span class="n">pk</span><span class="o">=</span><span class="s2">&quot;PrimaryKey&quot;</span><span class="p">,</span>  <span class="c1"># PrimaryKey function name</span>
+            <span class="n">fk</span><span class="o">=</span><span class="s2">&quot;ForeignKey&quot;</span><span class="p">,</span>  <span class="c1"># ForeignKey function name</span>
+            <span class="n">uk</span><span class="o">=</span><span class="s2">&quot;Unique&quot;</span><span class="p">,</span>  <span class="c1"># UniqueKey function name</span>
+            <span class="n">constraints</span><span class="o">=</span><span class="p">(</span>  <span class="c1"># constraint function module</span>
                 <span class="vm">__name__</span><span class="o">.</span><span class="n">rsplit</span><span class="p">(</span><span class="s1">&#39;.&#39;</span><span class="p">,</span> <span class="mi">1</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="s1">&#39;.constraints&#39;</span>
             <span class="p">),</span>
         <span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">imports</span> <span class="o">=</span> <span class="n">_Imports</span><span class="p">(</span><span class="n">imports</span><span class="o">=</span><span class="n">imports</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">types</span> <span class="o">=</span> <span class="n">_Types</span><span class="p">(</span><span class="n">_weakref</span><span class="o">.</span><span class="n">proxy</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
         <span class="k">if</span> <span class="n">symbols</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">symbols</span> <span class="o">=</span> <span class="p">{}</span>
@@ -177,15 +176,17 @@
 
 <span class="sd">          symbol (str):</span>
 <span class="sd">            Symbol</span>
 
 <span class="sd">        Raises:</span>
 <span class="sd">          SymbolException: Symbol could not be set because of some conflict</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span><span class="p">):</span>  <span class="c1"># pragma: no cover</span>
+        <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span>
+            <span class="n">name</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span>
+        <span class="p">):</span>  <span class="c1"># pragma: no cover</span>
             <span class="n">name</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">_keyword</span><span class="o">.</span><span class="n">iskeyword</span><span class="p">(</span><span class="n">symbol</span><span class="p">):</span>
             <span class="k">raise</span> <span class="n">SymbolException</span><span class="p">(</span>
                 <span class="s2">&quot;Cannot use keyword </span><span class="si">%r</span><span class="s2"> as symbol&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">symbol</span><span class="p">,)</span>
             <span class="p">)</span>
         <span class="k">elif</span> <span class="n">symbol</span> <span class="ow">in</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="o">.</span><span class="n">values</span><span class="p">()):</span>
             <span class="k">if</span> <span class="n">name</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="n">name</span><span class="p">]</span> <span class="o">!=</span> <span class="n">symbol</span><span class="p">:</span>
@@ -308,29 +309,29 @@
         <span class="n">mod</span> <span class="o">=</span> <span class="n">type_</span><span class="o">.</span><span class="vm">__module__</span>
         <span class="k">if</span> <span class="n">mod</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;sqlalchemy.&#39;</span><span class="p">):</span>
             <span class="n">mod</span> <span class="o">=</span> <span class="s1">&#39;.&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">mod</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;.&#39;</span><span class="p">)[:</span><span class="mi">3</span><span class="p">])</span>
             <span class="k">if</span> <span class="n">mod</span> <span class="o">==</span> <span class="s1">&#39;sqlalchemy.dialects.</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">dialect</span><span class="p">:</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;type&#39;</span><span class="p">]</span>
             <span class="k">else</span><span class="p">:</span>
                 <span class="k">try</span><span class="p">:</span>
-                    <span class="n">_load_dotted</span><span class="p">(</span><span class="s1">&#39;sqlalchemy.dialects.</span><span class="si">%s</span><span class="s1">.</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span>
-                        <span class="n">dialect</span><span class="p">,</span> <span class="n">type_</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span>
-                    <span class="p">))</span>
+                    <span class="n">_load_dotted</span><span class="p">(</span>
+                        <span class="s1">&#39;sqlalchemy.dialects.</span><span class="si">%s</span><span class="s1">.</span><span class="si">%s</span><span class="s1">&#39;</span>
+                        <span class="o">%</span> <span class="p">(</span><span class="n">dialect</span><span class="p">,</span> <span class="n">type_</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">)</span>
+                    <span class="p">)</span>
                     <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;type&#39;</span><span class="p">]</span>
                 <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
                     <span class="k">try</span><span class="p">:</span>
-                        <span class="n">_load_dotted</span><span class="p">(</span><span class="s1">&#39;sqlalchemy.types.</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span>
-                            <span class="n">type_</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span>
-                        <span class="p">))</span>
+                        <span class="n">_load_dotted</span><span class="p">(</span>
+                            <span class="s1">&#39;sqlalchemy.types.</span><span class="si">%s</span><span class="s1">&#39;</span>
+                            <span class="o">%</span> <span class="p">(</span><span class="n">type_</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,)</span>
+                        <span class="p">)</span>
                         <span class="k">return</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">.types&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;sa&#39;</span><span class="p">],)</span>
                     <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
                         <span class="k">pass</span>
-        <span class="k">raise</span> <span class="n">SymbolException</span><span class="p">(</span>
-            <span class="s2">&quot;Don&#39;t know how to address type </span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">type_</span><span class="p">,)</span>
-        <span class="p">)</span></div></div>
+        <span class="k">raise</span> <span class="n">SymbolException</span><span class="p">(</span><span class="s2">&quot;Don&#39;t know how to address type </span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">type_</span><span class="p">,))</span></div></div>
 
 
 <div class="viewcode-block" id="_Imports"><a class="viewcode-back" href="../../apidoc/gensaschema._symbols.html#gensaschema._Imports">[docs]</a><span class="k">class</span> <span class="nc">_Imports</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Import table</span>
 
 <span class="sd">    Attributes:</span>
@@ -375,22 +376,25 @@
 
 <span class="sd">          import_ (str):</span>
 <span class="sd">            Import statement</span>
 
 <span class="sd">        Raises:</span>
 <span class="sd">          SymbolException: Import conflict</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span><span class="p">):</span>  <span class="c1"># pragma: no cover</span>
+        <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span>
+            <span class="n">name</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span>
+        <span class="p">):</span>  <span class="c1"># pragma: no cover</span>
             <span class="n">name</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
         <span class="n">imports</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_imports</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">imports</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">imports</span><span class="p">[</span><span class="n">name</span><span class="p">]</span> <span class="o">!=</span> <span class="n">import_</span><span class="p">:</span>
-                <span class="k">raise</span> <span class="n">SymbolException</span><span class="p">(</span><span class="s2">&quot;Import conflict: </span><span class="si">%r</span><span class="s2">: </span><span class="si">%r</span><span class="s2"> vs. </span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span>
-                    <span class="n">name</span><span class="p">,</span> <span class="n">imports</span><span class="p">[</span><span class="n">name</span><span class="p">],</span> <span class="n">import_</span>
-                <span class="p">))</span>
+                <span class="k">raise</span> <span class="n">SymbolException</span><span class="p">(</span>
+                    <span class="s2">&quot;Import conflict: </span><span class="si">%r</span><span class="s2">: </span><span class="si">%r</span><span class="s2"> vs. </span><span class="si">%r</span><span class="s2">&quot;</span>
+                    <span class="o">%</span> <span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">imports</span><span class="p">[</span><span class="n">name</span><span class="p">],</span> <span class="n">import_</span><span class="p">)</span>
+                <span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_imports</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">name</span><span class="p">,</span> <span class="n">import_</span><span class="p">))</span></div>
 
 <div class="viewcode-block" id="_Imports.__iter__"><a class="viewcode-back" href="../../apidoc/gensaschema._symbols.html#gensaschema._Imports.__iter__">[docs]</a>    <span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Make iterator over the import statements</span>
 
@@ -479,22 +483,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._symbols</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._symbols
 ****** Source code for gensaschema._symbols ******
 # -*- coding: ascii -*-
 u"""
 ===================
  Symbol management
@@ -46,15 +46,15 @@
 import weakref as _weakref
 
 from . import _exceptions
 from . import _util
 
 
 [docs]class SymbolException(_exceptions.Error):
-    """ Symbol error """
+    """Symbol error"""
 
 
 
 [docs]class Symbols(object):
     """
     Symbol table
 
@@ -79,24 +79,24 @@
 
           imports (iterable):
             List of initial (id, import statement) tuples. If omitted or
             ``None``, it's empty.
         """
         self._symbols = {}
         defaults = dict(
-            sa="_sa",          # SQLAlchemy shortname
-            meta="m",          # MetaData shortname
-            table="T",         # Table shortname
-            type="t",          # Type module shortname
-            column="C",        # Column shortname
-            default="D",       # DefaultClause shortname
-            pk="PrimaryKey",   # PrimaryKey function name
-            fk="ForeignKey",   # ForeignKey function name
-            uk="Unique",       # UniqueKey function name
-            constraints=(      # constraint function module
+            sa="_sa",  # SQLAlchemy shortname
+            meta="m",  # MetaData shortname
+            table="T",  # Table shortname
+            type="t",  # Type module shortname
+            column="C",  # Column shortname
+            default="D",  # DefaultClause shortname
+            pk="PrimaryKey",  # PrimaryKey function name
+            fk="ForeignKey",  # ForeignKey function name
+            uk="Unique",  # UniqueKey function name
+            constraints=(  # constraint function module
                 __name__.rsplit('.', 1)[0] + '.constraints'
             ),
         )
         self.imports = _Imports(imports=imports)
         self.types = _Types(_weakref.proxy(self))
         if symbols is None:
             symbols = {}
@@ -132,16 +132,17 @@
 
           symbol (str):
             Symbol
 
         Raises:
           SymbolException: Symbol could not be set because of some conflict
         """
-        if _util.py2 and not isinstance(name, _util.unicode):  # pragma: no
-cover
+        if _util.py2 and not isinstance(
+            name, _util.unicode
+        ):  # pragma: no cover
             name = str(name).decode('ascii')
         if _keyword.iskeyword(symbol):
             raise SymbolException(
                 "Cannot use keyword %r as symbol" % (symbol,)
             )
         elif symbol in list(self._symbols.values()):
             if name in self._symbols and self._symbols[name] != symbol:
@@ -270,29 +271,29 @@
         mod = type_.__module__
         if mod.startswith('sqlalchemy.'):
             mod = '.'.join(mod.split('.')[:3])
             if mod == 'sqlalchemy.dialects.%s' % dialect:
                 return self._symbols['type']
             else:
                 try:
-                    _load_dotted('sqlalchemy.dialects.%s.%s' % (
-                        dialect, type_.__class__.__name__
-                    ))
+                    _load_dotted(
+                        'sqlalchemy.dialects.%s.%s'
+                        % (dialect, type_.__class__.__name__)
+                    )
                     return self._symbols['type']
                 except ImportError:
                     try:
-                        _load_dotted('sqlalchemy.types.%s' % (
-                            type_.__class__.__name__,
-                        ))
+                        _load_dotted(
+                            'sqlalchemy.types.%s'
+                            % (type_.__class__.__name__,)
+                        )
                         return "%s.types" % (self._symbols['sa'],)
                     except ImportError:
                         pass
-        raise SymbolException(
-            "Don't know how to address type %r" % (type_,)
-        )
+        raise SymbolException("Don't know how to address type %r" % (type_,))
 
 
 
 [docs]class _Imports(object):
     """
     Import table
 
@@ -340,23 +341,25 @@
 
           import_ (str):
             Import statement
 
         Raises:
           SymbolException: Import conflict
         """
-        if _util.py2 and not isinstance(name, _util.unicode):  # pragma: no
-cover
+        if _util.py2 and not isinstance(
+            name, _util.unicode
+        ):  # pragma: no cover
             name = str(name).decode('ascii')
         imports = dict(self._imports)
         if name in imports:
             if imports[name] != import_:
-                raise SymbolException("Import conflict: %r: %r vs. %r" % (
-                    name, imports[name], import_
-                ))
+                raise SymbolException(
+                    "Import conflict: %r: %r vs. %r"
+                    % (name, imports[name], import_)
+                )
         else:
             self._imports.append((name, import_))
 
 
 [docs]    def __iter__(self):
         """
         Make iterator over the import statements
@@ -405,11 +408,11 @@
                 raise ImportError('.'.join(path))
     return obj
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._symbols
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_table.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_table.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._table &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._table &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._table</a></li> 
       </ul>
     </div>
     </div>
   
@@ -117,14 +116,15 @@
 
 <span class="sd">      constraints (list):</span>
 <span class="sd">        Constraint list</span>
 
 <span class="sd">      _symbols (Symbols):</span>
 <span class="sd">        Symbol table</span>
 <span class="sd">    &quot;&quot;&quot;</span>
+
     <span class="c1">#: Is it a table reference (vs. a table)?</span>
     <span class="c1">#:</span>
     <span class="c1">#: :Type: bool</span>
     <span class="n">is_reference</span> <span class="o">=</span> <span class="kc">False</span>
 
 <div class="viewcode-block" id="Table.__new__"><a class="viewcode-back" href="../../apidoc/gensaschema._table.html#gensaschema._table.Table.__new__">[docs]</a>    <span class="k">def</span> <span class="fm">__new__</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">varname</span><span class="p">,</span> <span class="n">table</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
@@ -173,17 +173,27 @@
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="c1"># pylint: disable = unused-argument</span>
 
         <span class="n">symbols</span><span class="p">[</span><span class="sa">u</span><span class="s1">&#39;table_</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">table</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="n">varname</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span> <span class="o">=</span> <span class="n">symbols</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">varname</span> <span class="o">=</span> <span class="n">varname</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">sa_table</span> <span class="o">=</span> <span class="n">table</span>
-        <span class="bp">self</span><span class="o">.</span><span class="n">constraints</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">filter</span><span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="p">[</span><span class="n">_constraint</span><span class="o">.</span><span class="n">Constraint</span><span class="p">(</span>
-            <span class="n">con</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">varname</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">,</span>
-        <span class="p">)</span> <span class="k">for</span> <span class="n">con</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">constraints</span><span class="p">]))</span></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">constraints</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span>
+            <span class="nb">filter</span><span class="p">(</span>
+                <span class="kc">None</span><span class="p">,</span>
+                <span class="p">[</span>
+                    <span class="n">_constraint</span><span class="o">.</span><span class="n">Constraint</span><span class="p">(</span>
+                        <span class="n">con</span><span class="p">,</span>
+                        <span class="bp">self</span><span class="o">.</span><span class="n">varname</span><span class="p">,</span>
+                        <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">,</span>
+                    <span class="p">)</span>
+                    <span class="k">for</span> <span class="n">con</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">constraints</span>
+                <span class="p">],</span>
+            <span class="p">)</span>
+        <span class="p">)</span></div>
 
 <div class="viewcode-block" id="Table.by_name"><a class="viewcode-back" href="../../apidoc/gensaschema._table.html#gensaschema._table.Table.by_name">[docs]</a>    <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">by_name</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">varname</span><span class="p">,</span> <span class="n">metadata</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">types</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Construct by name</span>
 
 <span class="sd">        Parameters:</span>
@@ -205,68 +215,92 @@
 <span class="sd">          types (callable):</span>
 <span class="sd">            Extra type loader. If the type reflection fails, because</span>
 <span class="sd">            SQLAlchemy cannot resolve it, the type loader will be called with</span>
 <span class="sd">            the type name, (bound) metadata and the symbol table. It is</span>
 <span class="sd">            responsible for modifying the symbols and imports *and* the</span>
 <span class="sd">            dialect&#39;s ``ischema_names``. If omitted or ``None``, the reflector</span>
 <span class="sd">            will always fail on unknown types.</span>
+
+<span class="sd">        Returns:</span>
+<span class="sd">          Table: new Table instance</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">kwargs</span> <span class="o">=</span> <span class="p">{}</span>
         <span class="k">if</span> <span class="s1">&#39;.&#39;</span> <span class="ow">in</span> <span class="n">name</span><span class="p">:</span>
             <span class="n">schema</span><span class="p">,</span> <span class="n">name</span> <span class="o">=</span> <span class="n">name</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;.&#39;</span><span class="p">)</span>
             <span class="n">kwargs</span><span class="p">[</span><span class="s1">&#39;schema&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">schema</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">schema</span> <span class="o">=</span> <span class="kc">None</span>
 
         <span class="n">tmatch</span> <span class="o">=</span> <span class="n">_re</span><span class="o">.</span><span class="n">compile</span><span class="p">(</span><span class="sa">u</span><span class="s2">&quot;^Did not recognize type (.+) of column&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">match</span>
 
         <span class="k">def</span> <span class="nf">type_name</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-<span class="w">            </span><span class="sd">&quot;&quot;&quot; Extract type name from exception &quot;&quot;&quot;</span>
+<span class="w">            </span><span class="sd">&quot;&quot;&quot;Extract type name from exception&quot;&quot;&quot;</span>
             <span class="n">match</span> <span class="o">=</span> <span class="n">tmatch</span><span class="p">(</span><span class="n">e</span><span class="o">.</span><span class="n">args</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
             <span class="k">if</span> <span class="n">match</span><span class="p">:</span>
                 <span class="n">type_name</span> <span class="o">=</span> <span class="n">match</span><span class="o">.</span><span class="n">group</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
                 <span class="k">if</span> <span class="n">type_name</span><span class="o">.</span><span class="n">startswith</span><span class="p">((</span><span class="s1">&#39;&quot;&#39;</span><span class="p">,</span> <span class="s2">&quot;&#39;&quot;</span><span class="p">)):</span>
                     <span class="n">type_name</span> <span class="o">=</span> <span class="n">type_name</span><span class="p">[</span><span class="mi">1</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
                 <span class="k">return</span> <span class="n">type_name</span> <span class="ow">or</span> <span class="kc">None</span>
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">with</span> <span class="n">_warnings</span><span class="o">.</span><span class="n">catch_warnings</span><span class="p">():</span>
-            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;error&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                     <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Did not recognize type &#39;</span><span class="p">)</span>
-            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;error&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                     <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Unknown column definition &#39;</span><span class="p">)</span>
-            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;error&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                     <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Incomplete reflection of &#39;</span>
-                                             <span class="sa">r</span><span class="s1">&#39;column definition&#39;</span><span class="p">)</span>
-            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;ignore&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                     <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Could not instantiate type &#39;</span><span class="p">)</span>
-            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;ignore&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                     <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Skipped unsupported &#39;</span>
-                                             <span class="sa">r</span><span class="s1">&#39;reflection of expression-based&#39;</span>
-                                             <span class="sa">r</span><span class="s1">&#39; index &#39;</span><span class="p">)</span>
-            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;ignore&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                     <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Predicate of partial index &#39;</span><span class="p">)</span>
+            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                <span class="s1">&#39;error&#39;</span><span class="p">,</span>
+                <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Did not recognize type &#39;</span><span class="p">,</span>
+            <span class="p">)</span>
+            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                <span class="s1">&#39;error&#39;</span><span class="p">,</span>
+                <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Unknown column definition &#39;</span><span class="p">,</span>
+            <span class="p">)</span>
+            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                <span class="s1">&#39;error&#39;</span><span class="p">,</span>
+                <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Incomplete reflection of &#39;</span> <span class="sa">r</span><span class="s1">&#39;column definition&#39;</span><span class="p">,</span>
+            <span class="p">)</span>
+            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                <span class="s1">&#39;ignore&#39;</span><span class="p">,</span>
+                <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Could not instantiate type &#39;</span><span class="p">,</span>
+            <span class="p">)</span>
+            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                <span class="s1">&#39;ignore&#39;</span><span class="p">,</span>
+                <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Skipped unsupported &#39;</span>
+                <span class="sa">r</span><span class="s1">&#39;reflection of expression-based&#39;</span>
+                <span class="sa">r</span><span class="s1">&#39; index &#39;</span><span class="p">,</span>
+            <span class="p">)</span>
+            <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                <span class="s1">&#39;ignore&#39;</span><span class="p">,</span>
+                <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                <span class="n">message</span><span class="o">=</span><span class="sa">r</span><span class="s1">&#39;^Predicate of partial index &#39;</span><span class="p">,</span>
+            <span class="p">)</span>
 
             <span class="n">seen</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
             <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
                 <span class="k">try</span><span class="p">:</span>
-                    <span class="n">table</span> <span class="o">=</span> <span class="n">_sa</span><span class="o">.</span><span class="n">Table</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">metadata</span><span class="p">,</span>
-                                      <span class="n">autoload_with</span><span class="o">=</span><span class="n">metadata</span><span class="o">.</span><span class="n">bind</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+                    <span class="n">table</span> <span class="o">=</span> <span class="n">_sa</span><span class="o">.</span><span class="n">Table</span><span class="p">(</span>
+                        <span class="n">name</span><span class="p">,</span> <span class="n">metadata</span><span class="p">,</span> <span class="n">autoload_with</span><span class="o">=</span><span class="n">metadata</span><span class="o">.</span><span class="n">bind</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span>
+                    <span class="p">)</span>
                 <span class="k">except</span> <span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
                     <span class="k">if</span> <span class="n">types</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
                         <span class="n">tname</span> <span class="o">=</span> <span class="n">type_name</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
                         <span class="k">if</span> <span class="n">tname</span> <span class="ow">and</span> <span class="n">tname</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">seen</span><span class="p">:</span>
                             <span class="n">stack</span> <span class="o">=</span> <span class="p">[</span><span class="n">tname</span><span class="p">]</span>
                             <span class="k">while</span> <span class="n">stack</span><span class="p">:</span>
                                 <span class="k">try</span><span class="p">:</span>
                                     <span class="n">types</span><span class="p">(</span><span class="n">stack</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span> <span class="n">metadata</span><span class="p">,</span> <span class="n">symbols</span><span class="p">)</span>
                                 <span class="k">except</span> <span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
                                     <span class="n">tname</span> <span class="o">=</span> <span class="n">type_name</span><span class="p">(</span><span class="n">exc</span><span class="p">)</span>
-                                    <span class="k">if</span> <span class="n">tname</span> <span class="ow">and</span> <span class="n">tname</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">stack</span> <span class="ow">and</span> \
-                                            <span class="n">tname</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">seen</span><span class="p">:</span>
+                                    <span class="k">if</span> <span class="p">(</span>
+                                        <span class="n">tname</span>
+                                        <span class="ow">and</span> <span class="n">tname</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">stack</span>
+                                        <span class="ow">and</span> <span class="n">tname</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">seen</span>
+                                    <span class="p">):</span>
                                         <span class="n">stack</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">tname</span><span class="p">)</span>
                                         <span class="k">continue</span>
                                     <span class="k">raise</span>
                                 <span class="k">else</span><span class="p">:</span>
                                     <span class="n">seen</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">stack</span><span class="o">.</span><span class="n">pop</span><span class="p">())</span>
                             <span class="k">continue</span>
                     <span class="k">raise</span>
@@ -295,17 +329,17 @@
         <span class="n">result</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">(</span><span class="si">%r</span><span class="s2">, </span><span class="si">%s%s</span><span class="s2">)&quot;</span> <span class="o">%</span> <span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;table&#39;</span><span class="p">],</span>
             <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">sa_table</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">[</span><span class="s1">&#39;meta&#39;</span><span class="p">],</span>
             <span class="n">args</span><span class="p">,</span>
         <span class="p">)</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">constraints</span><span class="p">:</span>
-            <span class="n">result</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">((</span>
-                <span class="n">result</span><span class="p">,</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="nb">repr</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraints</span><span class="p">)))</span>
-            <span class="p">))</span>
+            <span class="n">result</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+                <span class="p">(</span><span class="n">result</span><span class="p">,</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="nb">repr</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">constraints</span><span class="p">))))</span>
+            <span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span></div></div>
 
 
 <div class="viewcode-block" id="TableReference"><a class="viewcode-back" href="../../apidoc/gensaschema._table.html#gensaschema._table.TableReference">[docs]</a><span class="k">class</span> <span class="nc">TableReference</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Referenced table</span>
 
@@ -315,14 +349,15 @@
 
 <span class="sd">      sa_table (sqlalchemy.Table):</span>
 <span class="sd">        Table</span>
 
 <span class="sd">      constraints (list):</span>
 <span class="sd">        Constraint list</span>
 <span class="sd">    &quot;&quot;&quot;</span>
+
     <span class="c1">#: Is it a table reference (vs. a table)?</span>
     <span class="c1">#:</span>
     <span class="c1">#: :Type: bool</span>
     <span class="n">is_reference</span> <span class="o">=</span> <span class="kc">True</span>
 
 <div class="viewcode-block" id="TableReference.__init__"><a class="viewcode-back" href="../../apidoc/gensaschema._table.html#gensaschema._table.TableReference.__init__">[docs]</a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">varname</span><span class="p">,</span> <span class="n">table</span><span class="p">,</span> <span class="n">schema</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
@@ -341,24 +376,26 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">varname</span> <span class="o">=</span> <span class="n">varname</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">sa_table</span> <span class="o">=</span> <span class="n">table</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">constraints</span> <span class="o">=</span> <span class="p">[]</span>
         <span class="n">pkg</span><span class="p">,</span> <span class="n">mod</span> <span class="o">=</span> <span class="n">schema</span><span class="o">.</span><span class="n">rsplit</span><span class="p">(</span><span class="s1">&#39;.&#39;</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">mod</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;_&#39;</span><span class="p">):</span>
             <span class="n">modas</span> <span class="o">=</span> <span class="s1">&#39;_&#39;</span> <span class="o">+</span> <span class="n">mod</span>
             <span class="n">symbols</span><span class="o">.</span><span class="n">imports</span><span class="p">[</span><span class="n">schema</span><span class="p">]</span> <span class="o">=</span> <span class="s1">&#39;from </span><span class="si">%s</span><span class="s1"> import </span><span class="si">%s</span><span class="s1"> as </span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span>
-                <span class="n">pkg</span><span class="p">,</span> <span class="n">mod</span><span class="p">,</span> <span class="n">modas</span>
+                <span class="n">pkg</span><span class="p">,</span>
+                <span class="n">mod</span><span class="p">,</span>
+                <span class="n">modas</span><span class="p">,</span>
             <span class="p">)</span>
             <span class="n">mod</span> <span class="o">=</span> <span class="n">modas</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">symbols</span><span class="o">.</span><span class="n">imports</span><span class="p">[</span><span class="n">schema</span><span class="p">]</span> <span class="o">=</span> <span class="s1">&#39;from </span><span class="si">%s</span><span class="s1"> import </span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">pkg</span><span class="p">,</span> <span class="n">mod</span><span class="p">)</span>
         <span class="n">symbols</span><span class="p">[</span><span class="sa">u</span><span class="s1">&#39;table_</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="n">table</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">.</span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">mod</span><span class="p">,</span> <span class="n">varname</span><span class="p">)</span></div></div>
 
 
 <div class="viewcode-block" id="TableCollection"><a class="viewcode-back" href="../../apidoc/gensaschema._table.html#gensaschema._table.TableCollection">[docs]</a><span class="k">class</span> <span class="nc">TableCollection</span><span class="p">(</span><span class="nb">tuple</span><span class="p">):</span>
-<span class="w">    </span><span class="sd">&quot;&quot;&quot; Table collection &quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;Table collection&quot;&quot;&quot;</span>
 
 <div class="viewcode-block" id="TableCollection.by_names"><a class="viewcode-back" href="../../apidoc/gensaschema._table.html#gensaschema._table.TableCollection.by_names">[docs]</a>    <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">by_names</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">metadata</span><span class="p">,</span> <span class="n">names</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">types</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Construct by table names</span>
 
 <span class="sd">        Parameters:</span>
@@ -378,27 +415,29 @@
 <span class="sd">            responsible for modifying the symbols and imports *and* the</span>
 <span class="sd">            dialect&#39;s ``ischema_names``. If omitted or ``None``, the reflector</span>
 <span class="sd">            will always fail on unknown types.</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">          TableCollection: New table collection instance</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">objects</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">((</span><span class="n">table</span><span class="o">.</span><span class="n">sa_table</span><span class="o">.</span><span class="n">key</span><span class="p">,</span> <span class="n">table</span><span class="p">)</span> <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="p">[</span>
-            <span class="n">Table</span><span class="o">.</span><span class="n">by_name</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">varname</span><span class="p">,</span> <span class="n">metadata</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span>
-                          <span class="n">types</span><span class="o">=</span><span class="n">types</span><span class="p">)</span>
-            <span class="k">for</span> <span class="n">varname</span><span class="p">,</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span>
-        <span class="p">])</span>
+        <span class="n">objects</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">(</span>
+            <span class="p">(</span><span class="n">table</span><span class="o">.</span><span class="n">sa_table</span><span class="o">.</span><span class="n">key</span><span class="p">,</span> <span class="n">table</span><span class="p">)</span>
+            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="p">[</span>
+                <span class="n">Table</span><span class="o">.</span><span class="n">by_name</span><span class="p">(</span>
+                    <span class="n">name</span><span class="p">,</span> <span class="n">varname</span><span class="p">,</span> <span class="n">metadata</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span><span class="p">,</span> <span class="n">types</span><span class="o">=</span><span class="n">types</span>
+                <span class="p">)</span>
+                <span class="k">for</span> <span class="n">varname</span><span class="p">,</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span>
+            <span class="p">]</span>
+        <span class="p">)</span>
 
         <span class="k">def</span> <span class="nf">map_table</span><span class="p">(</span><span class="n">sa_table</span><span class="p">):</span>
-<span class="w">            </span><span class="sd">&quot;&quot;&quot; Map SA table to table object &quot;&quot;&quot;</span>
+<span class="w">            </span><span class="sd">&quot;&quot;&quot;Map SA table to table object&quot;&quot;&quot;</span>
             <span class="k">if</span> <span class="n">sa_table</span><span class="o">.</span><span class="n">key</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">objects</span><span class="p">:</span>
                 <span class="n">varname</span> <span class="o">=</span> <span class="n">sa_table</span><span class="o">.</span><span class="n">name</span>
-                <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> \
-                        <span class="nb">isinstance</span><span class="p">(</span><span class="n">varname</span><span class="p">,</span>
-                                   <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span><span class="p">):</span>  <span class="c1"># pragma: no cover</span>
+                <span class="k">if</span> <span class="n">_util</span><span class="o">.</span><span class="n">py2</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">varname</span><span class="p">,</span> <span class="n">_util</span><span class="o">.</span><span class="n">unicode</span><span class="p">):</span>
                     <span class="n">varname</span> <span class="o">=</span> <span class="n">varname</span><span class="o">.</span><span class="n">encode</span><span class="p">(</span><span class="s1">&#39;ascii&#39;</span><span class="p">)</span>
                 <span class="n">objects</span><span class="p">[</span><span class="n">sa_table</span><span class="o">.</span><span class="n">key</span><span class="p">]</span> <span class="o">=</span> <span class="n">Table</span><span class="p">(</span>
                     <span class="n">varname</span><span class="p">,</span> <span class="n">sa_table</span><span class="p">,</span> <span class="n">schemas</span><span class="p">,</span> <span class="n">symbols</span>
                 <span class="p">)</span>
             <span class="k">return</span> <span class="n">objects</span><span class="p">[</span><span class="n">sa_table</span><span class="o">.</span><span class="n">key</span><span class="p">]</span>
 
         <span class="n">tables</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="n">map_table</span><span class="p">,</span> <span class="n">metadata</span><span class="o">.</span><span class="n">tables</span><span class="o">.</span><span class="n">values</span><span class="p">()))</span>
@@ -431,16 +470,17 @@
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Find foreign key cycles and break them apart</span>
 
 <span class="sd">    Parameters:</span>
 <span class="sd">      metadata (sqlalchemy.MetaData):</span>
 <span class="sd">        Metadata</span>
 <span class="sd">    &quot;&quot;&quot;</span>
+
     <span class="k">def</span> <span class="nf">break_cycle</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot; Break foreign key cycle &quot;&quot;&quot;</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Break foreign key cycle&quot;&quot;&quot;</span>
         <span class="n">cycle_keys</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="n">_op</span><span class="o">.</span><span class="n">attrgetter</span><span class="p">(</span><span class="s1">&#39;key&#39;</span><span class="p">),</span> <span class="n">e</span><span class="o">.</span><span class="n">cycles</span><span class="p">))</span>
         <span class="n">cycle_path</span> <span class="o">=</span> <span class="p">[</span>
             <span class="p">(</span><span class="n">parent</span><span class="p">,</span> <span class="n">child</span><span class="p">)</span>
             <span class="k">for</span> <span class="n">parent</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="n">e</span><span class="o">.</span><span class="n">edges</span>
             <span class="k">if</span> <span class="n">parent</span><span class="o">.</span><span class="n">key</span> <span class="ow">in</span> <span class="n">cycle_keys</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">key</span> <span class="ow">in</span> <span class="n">cycle_keys</span>
         <span class="p">]</span>
         <span class="n">deps</span> <span class="o">=</span> <span class="p">[</span><span class="n">cycle_path</span><span class="o">.</span><span class="n">pop</span><span class="p">()]</span>
@@ -458,34 +498,41 @@
             <span class="k">raise</span> <span class="ne">AssertionError</span><span class="p">(</span><span class="s2">&quot;Could not construct sorted cycle path&quot;</span><span class="p">)</span>
 
         <span class="n">deps</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="n">_op</span><span class="o">.</span><span class="n">itemgetter</span><span class="p">(</span><span class="mi">0</span><span class="p">),</span> <span class="n">deps</span><span class="p">))</span>
         <span class="n">first_dep</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">sorted</span><span class="p">(</span><span class="n">deps</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">_op</span><span class="o">.</span><span class="n">attrgetter</span><span class="p">(</span><span class="s1">&#39;name&#39;</span><span class="p">)))[</span><span class="mi">0</span><span class="p">]</span>
         <span class="k">while</span> <span class="n">first_dep</span> <span class="o">!=</span> <span class="n">deps</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
             <span class="n">deps</span> <span class="o">=</span> <span class="p">[</span><span class="n">deps</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]]</span> <span class="o">+</span> <span class="n">deps</span><span class="p">[:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">deps</span><span class="o">.</span><span class="n">reverse</span><span class="p">()</span>
-        <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="s2">&quot;Found foreign key cycle: </span><span class="si">%s</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot; -&gt; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span>
-            <span class="nb">repr</span><span class="p">(</span><span class="n">table</span><span class="o">.</span><span class="n">name</span><span class="p">)</span> <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">deps</span> <span class="o">+</span> <span class="p">[</span><span class="n">deps</span><span class="p">[</span><span class="mi">0</span><span class="p">]]</span>
-        <span class="p">]))</span>
+        <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
+            <span class="s2">&quot;Found foreign key cycle: </span><span class="si">%s</span><span class="s2">&quot;</span><span class="p">,</span>
+            <span class="s2">&quot; -&gt; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">repr</span><span class="p">(</span><span class="n">table</span><span class="o">.</span><span class="n">name</span><span class="p">)</span> <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">deps</span> <span class="o">+</span> <span class="p">[</span><span class="n">deps</span><span class="p">[</span><span class="mi">0</span><span class="p">]]]),</span>
+        <span class="p">)</span>
 
         <span class="k">def</span> <span class="nf">visit_foreign_key</span><span class="p">(</span><span class="n">fkey</span><span class="p">):</span>
-<span class="w">            </span><span class="sd">&quot;&quot;&quot; Visit foreign key &quot;&quot;&quot;</span>
+<span class="w">            </span><span class="sd">&quot;&quot;&quot;Visit foreign key&quot;&quot;&quot;</span>
             <span class="k">if</span> <span class="n">fkey</span><span class="o">.</span><span class="n">column</span><span class="o">.</span><span class="n">table</span> <span class="o">==</span> <span class="n">deps</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
                 <span class="n">fkey</span><span class="o">.</span><span class="n">use_alter</span> <span class="o">=</span> <span class="kc">True</span>
                 <span class="n">fkey</span><span class="o">.</span><span class="n">constraint</span><span class="o">.</span><span class="n">use_alter</span> <span class="o">=</span> <span class="kc">True</span>
 
-        <span class="n">_sa</span><span class="o">.</span><span class="n">sql</span><span class="o">.</span><span class="n">visitors</span><span class="o">.</span><span class="n">traverse</span><span class="p">(</span><span class="n">deps</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="nb">dict</span><span class="p">(</span><span class="n">schema_visitor</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="nb">dict</span><span class="p">(</span>
-            <span class="n">foreign_key</span><span class="o">=</span><span class="n">visit_foreign_key</span><span class="p">,</span>
-        <span class="p">))</span>
+        <span class="n">_sa</span><span class="o">.</span><span class="n">sql</span><span class="o">.</span><span class="n">visitors</span><span class="o">.</span><span class="n">traverse</span><span class="p">(</span>
+            <span class="n">deps</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span>
+            <span class="nb">dict</span><span class="p">(</span><span class="n">schema_visitor</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span>
+            <span class="nb">dict</span><span class="p">(</span>
+                <span class="n">foreign_key</span><span class="o">=</span><span class="n">visit_foreign_key</span><span class="p">,</span>
+            <span class="p">),</span>
+        <span class="p">)</span>
 
     <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="k">with</span> <span class="n">_warnings</span><span class="o">.</span><span class="n">catch_warnings</span><span class="p">():</span>
-                <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s1">&#39;ignore&#39;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
-                                         <span class="n">message</span><span class="o">=</span><span class="p">(</span><span class="sa">r</span><span class="s1">&#39;^Cannot correctly sort &#39;</span>
-                                                  <span class="sa">r</span><span class="s1">&#39;tables&#39;</span><span class="p">))</span>
+                <span class="n">_warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span>
+                    <span class="s1">&#39;ignore&#39;</span><span class="p">,</span>
+                    <span class="n">category</span><span class="o">=</span><span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">SAWarning</span><span class="p">,</span>
+                    <span class="n">message</span><span class="o">=</span><span class="p">(</span><span class="sa">r</span><span class="s1">&#39;^Cannot correctly sort &#39;</span> <span class="sa">r</span><span class="s1">&#39;tables&#39;</span><span class="p">),</span>
+                <span class="p">)</span>
 
                 <span class="n">metadata</span><span class="o">.</span><span class="n">sorted_tables</span>  <span class="c1"># pylint: disable = pointless-statement</span>
         <span class="k">except</span> <span class="n">_sa</span><span class="o">.</span><span class="n">exc</span><span class="o">.</span><span class="n">CircularDependencyError</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
             <span class="n">break_cycle</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="k">break</span></div>
 </pre></div>
@@ -531,22 +578,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._table</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._table
 ****** Source code for gensaschema._table ******
 # -*- coding: ascii -*-
 u"""
 =====================================
  Table inspection and representation
@@ -69,14 +69,15 @@
 
       constraints (list):
         Constraint list
 
       _symbols (Symbols):
         Symbol table
     """
+
     #: Is it a table reference (vs. a table)?
     #:
     #: :Type: bool
     is_reference = False
 
 [docs]    def __new__(cls, varname, table, schemas, symbols):
         """
@@ -126,17 +127,27 @@
         """
         # pylint: disable = unused-argument
 
         symbols[u'table_%s' % table.name] = varname
         self._symbols = symbols
         self.varname = varname
         self.sa_table = table
-        self.constraints = list(filter(None, [_constraint.Constraint(
-            con, self.varname, self._symbols,
-        ) for con in table.constraints]))
+        self.constraints = list(
+            filter(
+                None,
+                [
+                    _constraint.Constraint(
+                        con,
+                        self.varname,
+                        self._symbols,
+                    )
+                    for con in table.constraints
+                ],
+            )
+        )
 
 
 [docs]    @classmethod
     def by_name(cls, name, varname, metadata, schemas, symbols, types=None):
         """
         Construct by name
 
@@ -159,68 +170,92 @@
           types (callable):
             Extra type loader. If the type reflection fails, because
             SQLAlchemy cannot resolve it, the type loader will be called with
             the type name, (bound) metadata and the symbol table. It is
             responsible for modifying the symbols and imports *and* the
             dialect's ``ischema_names``. If omitted or ``None``, the reflector
             will always fail on unknown types.
+
+        Returns:
+          Table: new Table instance
         """
         kwargs = {}
         if '.' in name:
             schema, name = name.split('.')
             kwargs['schema'] = schema
         else:
             schema = None
 
         tmatch = _re.compile(u"^Did not recognize type (.+) of column").match
 
         def type_name(e):
-            """ Extract type name from exception """
+            """Extract type name from exception"""
             match = tmatch(e.args[0])
             if match:
                 type_name = match.group(1).strip()
                 if type_name.startswith(('"', "'")):
                     type_name = type_name[1:-1]
                 return type_name or None
             return None
 
         with _warnings.catch_warnings():
-            _warnings.filterwarnings('error', category=_sa.exc.SAWarning,
-                                     message=r'^Did not recognize type ')
-            _warnings.filterwarnings('error', category=_sa.exc.SAWarning,
-                                     message=r'^Unknown column definition ')
-            _warnings.filterwarnings('error', category=_sa.exc.SAWarning,
-                                     message=r'^Incomplete reflection of '
-                                             r'column definition')
-            _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                     message=r'^Could not instantiate type ')
-            _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                     message=r'^Skipped unsupported '
-                                             r'reflection of expression-based'
-                                             r' index ')
-            _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                     message=r'^Predicate of partial index ')
+            _warnings.filterwarnings(
+                'error',
+                category=_sa.exc.SAWarning,
+                message=r'^Did not recognize type ',
+            )
+            _warnings.filterwarnings(
+                'error',
+                category=_sa.exc.SAWarning,
+                message=r'^Unknown column definition ',
+            )
+            _warnings.filterwarnings(
+                'error',
+                category=_sa.exc.SAWarning,
+                message=r'^Incomplete reflection of ' r'column definition',
+            )
+            _warnings.filterwarnings(
+                'ignore',
+                category=_sa.exc.SAWarning,
+                message=r'^Could not instantiate type ',
+            )
+            _warnings.filterwarnings(
+                'ignore',
+                category=_sa.exc.SAWarning,
+                message=r'^Skipped unsupported '
+                r'reflection of expression-based'
+                r' index ',
+            )
+            _warnings.filterwarnings(
+                'ignore',
+                category=_sa.exc.SAWarning,
+                message=r'^Predicate of partial index ',
+            )
 
             seen = set()
             while True:
                 try:
-                    table = _sa.Table(name, metadata,
-                                      autoload_with=metadata.bind, **kwargs)
+                    table = _sa.Table(
+                        name, metadata, autoload_with=metadata.bind, **kwargs
+                    )
                 except _sa.exc.SAWarning as e:
                     if types is not None:
                         tname = type_name(e)
                         if tname and tname not in seen:
                             stack = [tname]
                             while stack:
                                 try:
                                     types(stack[-1], metadata, symbols)
                                 except _sa.exc.SAWarning as exc:
                                     tname = type_name(exc)
-                                    if tname and tname not in stack and \
-                                            tname not in seen:
+                                    if (
+                                        tname
+                                        and tname not in stack
+                                        and tname not in seen
+                                    ):
                                         stack.append(tname)
                                         continue
                                     raise
                                 else:
                                     seen.add(stack.pop())
                             continue
                     raise
@@ -250,17 +285,17 @@
         result = "%s(%r, %s%s)" % (
             self._symbols['table'],
             _util.unicode(self.sa_table.name),
             self._symbols['meta'],
             args,
         )
         if self.constraints:
-            result = "\n".join((
-                result, '\n'.join(map(repr, sorted(self.constraints)))
-            ))
+            result = "\n".join(
+                (result, '\n'.join(map(repr, sorted(self.constraints))))
+            )
         return result
 
 
 
 [docs]class TableReference(object):
     """
     Referenced table
@@ -271,14 +306,15 @@
 
       sa_table (sqlalchemy.Table):
         Table
 
       constraints (list):
         Constraint list
     """
+
     #: Is it a table reference (vs. a table)?
     #:
     #: :Type: bool
     is_reference = True
 
 [docs]    def __init__(self, varname, table, schema, symbols):
         """
@@ -297,25 +333,27 @@
         self.varname = varname
         self.sa_table = table
         self.constraints = []
         pkg, mod = schema.rsplit('.', 1)
         if not mod.startswith('_'):
             modas = '_' + mod
             symbols.imports[schema] = 'from %s import %s as %s' % (
-                pkg, mod, modas
+                pkg,
+                mod,
+                modas,
             )
             mod = modas
         else:
             symbols.imports[schema] = 'from %s import %s' % (pkg, mod)
         symbols[u'table_%s' % table.name] = "%s.%s" % (mod, varname)
 
 
 
 [docs]class TableCollection(tuple):
-    """ Table collection """
+    """Table collection"""
 
 [docs]    @classmethod
     def by_names(cls, metadata, names, schemas, symbols, types=None):
         """
         Construct by table names
 
         Parameters:
@@ -335,27 +373,29 @@
             responsible for modifying the symbols and imports *and* the
             dialect's ``ischema_names``. If omitted or ``None``, the reflector
             will always fail on unknown types.
 
         Returns:
           TableCollection: New table collection instance
         """
-        objects = dict((table.sa_table.key, table) for table in [
-            Table.by_name(name, varname, metadata, schemas, symbols,
-                          types=types)
-            for varname, name in names
-        ])
+        objects = dict(
+            (table.sa_table.key, table)
+            for table in [
+                Table.by_name(
+                    name, varname, metadata, schemas, symbols, types=types
+                )
+                for varname, name in names
+            ]
+        )
 
         def map_table(sa_table):
-            """ Map SA table to table object """
+            """Map SA table to table object"""
             if sa_table.key not in objects:
                 varname = sa_table.name
-                if _util.py2 and \
-                        isinstance(varname,
-                                   _util.unicode):  # pragma: no cover
+                if _util.py2 and isinstance(varname, _util.unicode):
                     varname = varname.encode('ascii')
                 objects[sa_table.key] = Table(
                     varname, sa_table, schemas, symbols
                 )
             return objects[sa_table.key]
 
         tables = list(map(map_table, metadata.tables.values()))
@@ -389,16 +429,17 @@
     """
     Find foreign key cycles and break them apart
 
     Parameters:
       metadata (sqlalchemy.MetaData):
         Metadata
     """
+
     def break_cycle(e):
-        """ Break foreign key cycle """
+        """Break foreign key cycle"""
         cycle_keys = set(map(_op.attrgetter('key'), e.cycles))
         cycle_path = [
             (parent, child)
             for parent, child in e.edges
             if parent.key in cycle_keys and child.key in cycle_keys
         ]
         deps = [cycle_path.pop()]
@@ -416,42 +457,49 @@
             raise AssertionError("Could not construct sorted cycle path")
 
         deps = list(map(_op.itemgetter(0), deps))
         first_dep = list(sorted(deps, key=_op.attrgetter('name')))[0]
         while first_dep != deps[-1]:
             deps = [deps[-1]] + deps[:-1]
         deps.reverse()
-        logger.debug("Found foreign key cycle: %s", " -> ".join([
-            repr(table.name) for table in deps + [deps[0]]
-        ]))
+        logger.debug(
+            "Found foreign key cycle: %s",
+            " -> ".join([repr(table.name) for table in deps + [deps[0]]]),
+        )
 
         def visit_foreign_key(fkey):
-            """ Visit foreign key """
+            """Visit foreign key"""
             if fkey.column.table == deps[1]:
                 fkey.use_alter = True
                 fkey.constraint.use_alter = True
 
-        _sa.sql.visitors.traverse(deps[0], dict(schema_visitor=True), dict(
-            foreign_key=visit_foreign_key,
-        ))
+        _sa.sql.visitors.traverse(
+            deps[0],
+            dict(schema_visitor=True),
+            dict(
+                foreign_key=visit_foreign_key,
+            ),
+        )
 
     while True:
         try:
             with _warnings.catch_warnings():
-                _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                         message=(r'^Cannot correctly sort '
-                                                  r'tables'))
+                _warnings.filterwarnings(
+                    'ignore',
+                    category=_sa.exc.SAWarning,
+                    message=(r'^Cannot correctly sort ' r'tables'),
+                )
 
                 metadata.sorted_tables  # pylint: disable = pointless-statement
         except _sa.exc.CircularDependencyError as e:
             break_cycle(e)
         else:
             break
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._table
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_template.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_template.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._template &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._template &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._template</a></li> 
       </ul>
     </div>
     </div>
   
@@ -191,22 +190,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._template</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._template
 ****** Source code for gensaschema._template ******
 # -*- coding: ascii -*-
 u"""
 =============================
  Simple template abstraction
@@ -102,11 +102,11 @@
             return self._template % kwargs
         return self._template
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._template
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_type.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_type.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._type &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._type &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._type</a></li> 
       </ul>
     </div>
     </div>
   
@@ -121,15 +120,15 @@
 
 <span class="sd">          dialect_name (str):</span>
 <span class="sd">            Dialect name</span>
 
 <span class="sd">          symbols (Symbols):</span>
 <span class="sd">            Symbol table</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span> <span class="o">=</span> <span class="n">ctype</span>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span> <span class="o">=</span> <span class="n">_finalize_type</span><span class="p">(</span><span class="n">ctype</span><span class="p">,</span> <span class="n">dialect_name</span><span class="p">,</span> <span class="n">symbols</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span> <span class="o">=</span> <span class="n">dialect_name</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span> <span class="o">=</span> <span class="n">symbols</span></div>
 
 <div class="viewcode-block" id="Type.by_column"><a class="viewcode-back" href="../../apidoc/gensaschema._type.html#gensaschema.Type.by_column">[docs]</a>    <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">by_column</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Construct by SA column</span>
@@ -174,15 +173,15 @@
             <span class="k">pass</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="k">return</span> <span class="n">custom_repr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">)</span>
 
         <span class="n">mod</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">resolve</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">)</span>
         <span class="n">params</span> <span class="o">=</span> <span class="p">[]</span>
 
-        <span class="k">if</span> <span class="n">_have_signature</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+        <span class="k">if</span> <span class="n">_have_signature</span><span class="p">:</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="c1"># pylint: disable = no-member</span>
                 <span class="n">sign</span> <span class="o">=</span> <span class="n">_inspect</span><span class="o">.</span><span class="n">signature</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="o">.</span><span class="fm">__init__</span><span class="p">)</span>
             <span class="k">except</span> <span class="p">(</span><span class="ne">TypeError</span><span class="p">,</span> <span class="ne">ValueError</span><span class="p">):</span>
                 <span class="k">pass</span>
             <span class="k">else</span><span class="p">:</span>
                 <span class="n">varargs</span><span class="p">,</span> <span class="n">kwds</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="kc">False</span>
@@ -197,33 +196,44 @@
                     <span class="k">if</span> <span class="n">value</span> <span class="ow">is</span> <span class="n">unset</span><span class="p">:</span>
                         <span class="k">continue</span>
 
                     <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">default</span> <span class="ow">is</span> <span class="ow">not</span> <span class="n">arg</span><span class="o">.</span><span class="n">empty</span> <span class="ow">and</span> <span class="n">arg</span><span class="o">.</span><span class="n">default</span> <span class="o">==</span> <span class="n">value</span><span class="p">:</span>
                         <span class="n">kwds</span> <span class="o">=</span> <span class="n">arg</span><span class="o">.</span><span class="n">kind</span> <span class="o">!=</span> <span class="n">arg</span><span class="o">.</span><span class="n">POSITIONAL_ONLY</span>
                         <span class="k">continue</span>
                     <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">_sa</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">TypeEngine</span><span class="p">):</span>
-                        <span class="n">rvalue</span> <span class="o">=</span> <span class="nb">repr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span>
-                                                     <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">))</span>
+                        <span class="n">rvalue</span> <span class="o">=</span> <span class="nb">repr</span><span class="p">(</span>
+                            <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="p">(</span>
+                                <span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span>
+                            <span class="p">)</span>
+                        <span class="p">)</span>
                     <span class="k">else</span><span class="p">:</span>
                         <span class="n">rvalue</span> <span class="o">=</span> <span class="nb">repr</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
 
                     <span class="k">if</span> <span class="n">kwds</span><span class="p">:</span>
                         <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;</span><span class="si">%s</span><span class="s1">=</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">rvalue</span><span class="p">))</span>
                     <span class="k">else</span><span class="p">:</span>
                         <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">rvalue</span><span class="p">)</span>
                 <span class="k">if</span> <span class="ow">not</span> <span class="n">kwds</span> <span class="ow">and</span> <span class="n">varargs</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-                    <span class="k">if</span> <span class="n">_find_class</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="s1">&#39;__init__&#39;</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> \
-                            <span class="n">_sa</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">TypeEngine</span><span class="p">:</span>
-                        <span class="n">params</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span>
-                            <span class="nb">map</span><span class="p">(</span><span class="nb">repr</span><span class="p">,</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="n">varargs</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="p">()))</span>
-                        <span class="p">))</span>
+                    <span class="k">if</span> <span class="p">(</span>
+                        <span class="n">_find_class</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="s1">&#39;__init__&#39;</span><span class="p">)</span>
+                        <span class="ow">is</span> <span class="ow">not</span> <span class="n">_sa</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">TypeEngine</span>
+                    <span class="p">):</span>
+                        <span class="n">params</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+                            <span class="nb">list</span><span class="p">(</span>
+                                <span class="nb">map</span><span class="p">(</span>
+                                    <span class="nb">repr</span><span class="p">,</span>
+                                    <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="n">varargs</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="p">()),</span>
+                                <span class="p">)</span>
+                            <span class="p">)</span>
+                        <span class="p">)</span>
 
-        <span class="k">else</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+        <span class="k">else</span><span class="p">:</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="c1"># pylint: disable = deprecated-method</span>
+                <span class="c1"># pylint: disable = no-member</span>
                 <span class="n">spec</span> <span class="o">=</span> <span class="n">_inspect</span><span class="o">.</span><span class="n">getargspec</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="o">.</span><span class="fm">__init__</span><span class="p">)</span>
             <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
                 <span class="k">pass</span>
             <span class="k">else</span><span class="p">:</span>
                 <span class="n">defaults</span> <span class="o">=</span> <span class="nb">dict</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="n">spec</span><span class="p">[</span><span class="mi">0</span><span class="p">][::</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span> <span class="p">(</span><span class="n">spec</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span> <span class="ow">or</span> <span class="p">())[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]))</span>
                 <span class="n">kwds</span> <span class="o">=</span> <span class="kc">False</span>
                 <span class="k">for</span> <span class="n">arg</span> <span class="ow">in</span> <span class="n">spec</span><span class="p">[</span><span class="mi">0</span><span class="p">][</span><span class="mi">1</span><span class="p">:]:</span>
@@ -231,35 +241,71 @@
                     <span class="k">if</span> <span class="n">value</span> <span class="ow">is</span> <span class="n">unset</span><span class="p">:</span>
                         <span class="k">continue</span>
 
                     <span class="k">if</span> <span class="n">arg</span> <span class="ow">in</span> <span class="n">defaults</span> <span class="ow">and</span> <span class="n">defaults</span><span class="p">[</span><span class="n">arg</span><span class="p">]</span> <span class="o">==</span> <span class="n">value</span><span class="p">:</span>
                         <span class="n">kwds</span> <span class="o">=</span> <span class="kc">True</span>
                         <span class="k">continue</span>
                     <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">_sa</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">TypeEngine</span><span class="p">):</span>
-                        <span class="n">rvalue</span> <span class="o">=</span> <span class="nb">repr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span>
-                                                     <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span><span class="p">))</span>
+                        <span class="n">rvalue</span> <span class="o">=</span> <span class="nb">repr</span><span class="p">(</span>
+                            <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="p">(</span>
+                                <span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dialect</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_symbols</span>
+                            <span class="p">)</span>
+                        <span class="p">)</span>
                     <span class="k">else</span><span class="p">:</span>
                         <span class="n">rvalue</span> <span class="o">=</span> <span class="nb">repr</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
                     <span class="k">if</span> <span class="n">kwds</span><span class="p">:</span>
                         <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;</span><span class="si">%s</span><span class="s1">=</span><span class="si">%s</span><span class="s1">&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,</span> <span class="n">rvalue</span><span class="p">))</span>
                     <span class="k">else</span><span class="p">:</span>
                         <span class="n">params</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">rvalue</span><span class="p">)</span>
                 <span class="k">if</span> <span class="ow">not</span> <span class="n">kwds</span> <span class="ow">and</span> <span class="n">spec</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-                    <span class="k">if</span> <span class="n">_find_class</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="s1">&#39;__init__&#39;</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> \
-                            <span class="n">_sa</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">TypeEngine</span><span class="p">:</span>
-                        <span class="n">params</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span>
-                            <span class="nb">map</span><span class="p">(</span><span class="nb">repr</span><span class="p">,</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="n">spec</span><span class="p">[</span><span class="mi">1</span><span class="p">]))</span>
-                        <span class="p">))</span>
+                    <span class="k">if</span> <span class="p">(</span>
+                        <span class="n">_find_class</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="s1">&#39;__init__&#39;</span><span class="p">)</span>
+                        <span class="ow">is</span> <span class="ow">not</span> <span class="n">_sa</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">TypeEngine</span>
+                    <span class="p">):</span>
+                        <span class="n">params</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+                            <span class="nb">list</span><span class="p">(</span><span class="nb">map</span><span class="p">(</span><span class="nb">repr</span><span class="p">,</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="p">,</span> <span class="n">spec</span><span class="p">[</span><span class="mi">1</span><span class="p">])))</span>
+                        <span class="p">)</span>
 
         <span class="n">params</span> <span class="o">=</span> <span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">params</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">params</span><span class="p">:</span>
             <span class="n">params</span> <span class="o">=</span> <span class="s2">&quot;(</span><span class="si">%s</span><span class="s2">)&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">params</span><span class="p">,)</span>
         <span class="k">return</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">.</span><span class="si">%s%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">mod</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctype</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="n">params</span><span class="p">)</span></div></div>
 
 
+<div class="viewcode-block" id="_finalize_type"><a class="viewcode-back" href="../../apidoc/gensaschema._type.html#gensaschema._finalize_type">[docs]</a><span class="k">def</span> <span class="nf">_finalize_type</span><span class="p">(</span><span class="n">ctype</span><span class="p">,</span> <span class="n">dialect</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">    Finalize type definitions and modifications</span>
+
+<span class="sd">    :TODO: should be generalized at some point in the future.</span>
+<span class="sd">    &quot;&quot;&quot;</span>
+
+    <span class="k">if</span> <span class="n">dialect</span> <span class="o">==</span> <span class="s1">&#39;postgresql&#39;</span><span class="p">:</span>
+        <span class="k">if</span> <span class="n">ctype</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span> <span class="o">==</span> <span class="s1">&#39;ENUM&#39;</span><span class="p">:</span>
+            <span class="n">_add_postgres_enum</span><span class="p">(</span><span class="n">ctype</span><span class="p">,</span> <span class="n">symbols</span><span class="p">)</span>
+
+    <span class="k">return</span> <span class="n">ctype</span></div>
+
+
+<div class="viewcode-block" id="_add_postgres_enum"><a class="viewcode-back" href="../../apidoc/gensaschema._type.html#gensaschema._add_postgres_enum">[docs]</a><span class="k">def</span> <span class="nf">_add_postgres_enum</span><span class="p">(</span><span class="n">ctype</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;Add postgres enum&quot;&quot;&quot;</span>
+    <span class="k">if</span> <span class="n">ctype</span> <span class="ow">in</span> <span class="n">symbols</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">instance_repr</span><span class="p">:</span>
+        <span class="k">return</span>
+
+    <span class="n">esymbol</span> <span class="o">=</span> <span class="s2">&quot;enum_</span><span class="si">%s</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">ctype</span><span class="o">.</span><span class="n">name</span><span class="p">,)</span>
+
+    <span class="k">def</span> <span class="nf">define</span><span class="p">(</span><span class="n">_</span><span class="p">,</span> <span class="n">symbols</span><span class="p">):</span>
+        <span class="k">return</span> <span class="p">[</span><span class="s2">&quot;</span><span class="si">%s</span><span class="s2"> = </span><span class="si">%s</span><span class="s2">.</span><span class="si">%r</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="n">esymbol</span><span class="p">,</span> <span class="n">symbols</span><span class="p">[</span><span class="s2">&quot;type&quot;</span><span class="p">],</span> <span class="n">ctype</span><span class="p">)]</span>
+
+    <span class="k">def</span> <span class="nf">custom_repr</span><span class="p">(</span><span class="o">*</span><span class="n">_</span><span class="p">):</span>
+        <span class="k">return</span> <span class="n">esymbol</span>
+
+    <span class="n">symbols</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">defines</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">define</span><span class="p">)</span>
+    <span class="n">symbols</span><span class="o">.</span><span class="n">types</span><span class="o">.</span><span class="n">instance_repr</span><span class="p">[</span><span class="n">ctype</span><span class="p">]</span> <span class="o">=</span> <span class="n">custom_repr</span></div>
+
+
 <div class="viewcode-block" id="_find_class"><a class="viewcode-back" href="../../apidoc/gensaschema._type.html#gensaschema._find_class">[docs]</a><span class="k">def</span> <span class="nf">_find_class</span><span class="p">(</span><span class="n">first_cls</span><span class="p">,</span> <span class="n">name</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Find class where a method is defined</span>
 
 <span class="sd">    Parameters:</span>
 <span class="sd">      first_cls (type):</span>
 <span class="sd">        Class to start with</span>
@@ -320,22 +366,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._type</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._type
 ****** Source code for gensaschema._type ******
 # -*- coding: ascii -*-
 u"""
 ====================================
  Type inspection and representation
@@ -73,15 +73,15 @@
 
           dialect_name (str):
             Dialect name
 
           symbols (Symbols):
             Symbol table
         """
-        self._ctype = ctype
+        self._ctype = _finalize_type(ctype, dialect_name, symbols)
         self._dialect = dialect_name
         self._symbols = symbols
 
 
 [docs]    @classmethod
     def by_column(cls, column, symbols):
         """
@@ -128,15 +128,15 @@
             pass
         else:
             return custom_repr(self._ctype, self._dialect, self._symbols)
 
         mod = self._symbols.types.resolve(self._ctype, self._dialect)
         params = []
 
-        if _have_signature:  # pragma: no cover
+        if _have_signature:
             try:
                 # pylint: disable = no-member
                 sign = _inspect.signature(self._ctype.__init__)
             except (TypeError, ValueError):
                 pass
             else:
                 varargs, kwds = None, False
@@ -151,33 +151,44 @@
                     if value is unset:
                         continue
 
                     if arg.default is not arg.empty and arg.default == value:
                         kwds = arg.kind != arg.POSITIONAL_ONLY
                         continue
                     if isinstance(value, _sa.types.TypeEngine):
-                        rvalue = repr(self.__class__(value, self._dialect,
-                                                     self._symbols))
+                        rvalue = repr(
+                            self.__class__(
+                                value, self._dialect, self._symbols
+                            )
+                        )
                     else:
                         rvalue = repr(value)
 
                     if kwds:
                         params.append('%s=%s' % (arg.name, rvalue))
                     else:
                         params.append(rvalue)
                 if not kwds and varargs is not None:
-                    if _find_class(self._ctype, '__init__') is not \
-                            _sa.types.TypeEngine:
-                        params.extend(list(
-                            map(repr, getattr(self._ctype, varargs.name, ()))
-                        ))
+                    if (
+                        _find_class(self._ctype, '__init__')
+                        is not _sa.types.TypeEngine
+                    ):
+                        params.extend(
+                            list(
+                                map(
+                                    repr,
+                                    getattr(self._ctype, varargs.name, ()),
+                                )
+                            )
+                        )
 
-        else:  # pragma: no cover
+        else:
             try:
                 # pylint: disable = deprecated-method
+                # pylint: disable = no-member
                 spec = _inspect.getargspec(self._ctype.__init__)
             except TypeError:
                 pass
             else:
                 defaults = dict(zip(spec[0][::-1], (spec[3] or ())[::-1]))
                 kwds = False
                 for arg in spec[0][1:]:
@@ -185,36 +196,74 @@
                     if value is unset:
                         continue
 
                     if arg in defaults and defaults[arg] == value:
                         kwds = True
                         continue
                     if isinstance(value, _sa.types.TypeEngine):
-                        rvalue = repr(self.__class__(value, self._dialect,
-                                                     self._symbols))
+                        rvalue = repr(
+                            self.__class__(
+                                value, self._dialect, self._symbols
+                            )
+                        )
                     else:
                         rvalue = repr(value)
                     if kwds:
                         params.append('%s=%s' % (arg, rvalue))
                     else:
                         params.append(rvalue)
                 if not kwds and spec[1] is not None:
-                    if _find_class(self._ctype, '__init__') is not \
-                            _sa.types.TypeEngine:
-                        params.extend(list(
-                            map(repr, getattr(self._ctype, spec[1]))
-                        ))
+                    if (
+                        _find_class(self._ctype, '__init__')
+                        is not _sa.types.TypeEngine
+                    ):
+                        params.extend(
+                            list(map(repr, getattr(self._ctype, spec[1])))
+                        )
 
         params = ', '.join(params)
         if params:
             params = "(%s)" % (params,)
         return "%s.%s%s" % (mod, self._ctype.__class__.__name__, params)
 
 
 
+[docs]def _finalize_type(ctype, dialect, symbols):
+    """
+    Finalize type definitions and modifications
+
+    :TODO: should be generalized at some point in the future.
+    """
+
+    if dialect == 'postgresql':
+        if ctype.__class__.__name__ == 'ENUM':
+            _add_postgres_enum(ctype, symbols)
+
+    return ctype
+
+
+
+[docs]def _add_postgres_enum(ctype, symbols):
+    """Add postgres enum"""
+    if ctype in symbols.types.instance_repr:
+        return
+
+    esymbol = "enum_%s" % (ctype.name,)
+
+    def define(_, symbols):
+        return ["%s = %s.%r" % (esymbol, symbols["type"], ctype)]
+
+    def custom_repr(*_):
+        return esymbol
+
+    symbols.types.defines.append(define)
+    symbols.types.instance_repr[ctype] = custom_repr
+
+
+
 [docs]def _find_class(first_cls, name):
     """
     Find class where a method is defined
 
     Parameters:
       first_cls (type):
         Class to start with
@@ -233,11 +282,11 @@
             return cls
     return None
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._type
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/_util.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/_util.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema._util &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._util &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._util</a></li> 
       </ul>
     </div>
     </div>
   
@@ -88,33 +87,33 @@
 <span class="sd">&quot;&quot;&quot;</span>
 <span class="n">__author__</span> <span class="o">=</span> <span class="sa">u</span><span class="s2">&quot;Andr</span><span class="se">\xe9</span><span class="s2"> Malo&quot;</span>
 
 
 <span class="c1"># pylint: disable = redefined-builtin, invalid-name, self-assigning-variable</span>
 <span class="k">try</span><span class="p">:</span>
     <span class="n">unicode</span>  <span class="c1"># pylint: disable = used-before-assignment</span>
-<span class="k">except</span> <span class="ne">NameError</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+<span class="k">except</span> <span class="ne">NameError</span><span class="p">:</span>
     <span class="n">unicode</span> <span class="o">=</span> <span class="nb">str</span>
-<span class="k">else</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+<span class="k">else</span><span class="p">:</span>
     <span class="n">unicode</span> <span class="o">=</span> <span class="n">unicode</span>
 
 <span class="k">try</span><span class="p">:</span>
     <span class="nb">bytes</span>  <span class="c1"># pylint: disable = used-before-assignment</span>
-<span class="k">except</span> <span class="ne">NameError</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+<span class="k">except</span> <span class="ne">NameError</span><span class="p">:</span>
     <span class="nb">bytes</span> <span class="o">=</span> <span class="nb">str</span>
-<span class="k">else</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+<span class="k">else</span><span class="p">:</span>
     <span class="nb">bytes</span> <span class="o">=</span> <span class="nb">bytes</span>
 
 <span class="n">py2</span> <span class="o">=</span> <span class="nb">bytes</span> <span class="ow">is</span> <span class="nb">str</span>
 
 <span class="k">try</span><span class="p">:</span>
     <span class="n">cmp</span>  <span class="c1"># pylint: disable = used-before-assignment</span>
-<span class="k">except</span> <span class="ne">NameError</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+<span class="k">except</span> <span class="ne">NameError</span><span class="p">:</span>
     <span class="n">cmp</span> <span class="o">=</span> <span class="k">lambda</span> <span class="n">a</span><span class="p">,</span> <span class="n">b</span><span class="p">:</span> <span class="p">(</span><span class="n">a</span> <span class="o">&gt;</span> <span class="n">b</span><span class="p">)</span> <span class="o">-</span> <span class="p">(</span><span class="n">a</span> <span class="o">&lt;</span> <span class="n">b</span><span class="p">)</span>
-<span class="k">else</span><span class="p">:</span>  <span class="c1"># pragma: no cover</span>
+<span class="k">else</span><span class="p">:</span>
     <span class="n">cmp</span> <span class="o">=</span> <span class="n">cmp</span>
 
 
 <div class="viewcode-block" id="find_public"><a class="viewcode-back" href="../../apidoc/gensaschema._util.html#gensaschema._util.find_public">[docs]</a><span class="k">def</span> <span class="nf">find_public</span><span class="p">(</span><span class="n">space</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Determine all public names in space</span>
 
@@ -175,22 +174,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._util</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._util
 ****** Source code for gensaschema._util ******
 # -*- coding: ascii -*-
 r"""
 :Copyright:
 
@@ -40,33 +40,33 @@
 """
 __author__ = u"Andr\xe9 Malo"
 
 
 # pylint: disable = redefined-builtin, invalid-name, self-assigning-variable
 try:
     unicode  # pylint: disable = used-before-assignment
-except NameError:  # pragma: no cover
+except NameError:
     unicode = str
-else:  # pragma: no cover
+else:
     unicode = unicode
 
 try:
     bytes  # pylint: disable = used-before-assignment
-except NameError:  # pragma: no cover
+except NameError:
     bytes = str
-else:  # pragma: no cover
+else:
     bytes = bytes
 
 py2 = bytes is str
 
 try:
     cmp  # pylint: disable = used-before-assignment
-except NameError:  # pragma: no cover
+except NameError:
     cmp = lambda a, b: (a > b) - (a < b)
-else:  # pragma: no cover
+else:
     cmp = cmp
 
 
 [docs]def find_public(space):
     """
     Determine all public names in space
 
@@ -85,11 +85,11 @@
         return list(space['__all__'])
     return [key for key in space.keys() if not key.startswith('_')]
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema._util
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/gensaschema/constraints.html` & `gensaschema-0.6.8/docs/userdoc/_modules/gensaschema/constraints.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>gensaschema.constraints &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema.constraints &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" accesskey="U">Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema.constraints</a></li> 
       </ul>
     </div>
     </div>
   
@@ -101,52 +100,59 @@
 <span class="sd">    Parameters:</span>
 <span class="sd">      *columns:</span>
 <span class="sd">        Constraint columns</span>
 
 <span class="sd">      \*\*kwargs:</span>
 <span class="sd">        Additional arguments</span>
 <span class="sd">    &quot;&quot;&quot;</span>
-    <span class="n">columns</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">append_constraint</span><span class="p">(</span><span class="n">_sa</span><span class="o">.</span><span class="n">UniqueConstraint</span><span class="p">(</span>
-        <span class="o">*</span><span class="n">columns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span>
-    <span class="p">))</span></div>
+    <span class="n">columns</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">append_constraint</span><span class="p">(</span>
+        <span class="n">_sa</span><span class="o">.</span><span class="n">UniqueConstraint</span><span class="p">(</span><span class="o">*</span><span class="n">columns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+    <span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="PrimaryKey"><a class="viewcode-back" href="../../apidoc/gensaschema.constraints.html#gensaschema.constraints.PrimaryKey">[docs]</a><span class="k">def</span> <span class="nf">PrimaryKey</span><span class="p">(</span><span class="o">*</span><span class="n">columns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>  <span class="c1"># pylint: disable = invalid-name</span>
 <span class="w">    </span><span class="sa">r</span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Append primary key</span>
 
 <span class="sd">    Parameters:</span>
 <span class="sd">      \*columns:</span>
 <span class="sd">        Constraint columns</span>
 
 <span class="sd">      \*\*kwargs:</span>
 <span class="sd">        Additional parameters</span>
 <span class="sd">    &quot;&quot;&quot;</span>
-    <span class="n">columns</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">append_constraint</span><span class="p">(</span><span class="n">_sa</span><span class="o">.</span><span class="n">PrimaryKeyConstraint</span><span class="p">(</span>
-        <span class="o">*</span><span class="n">columns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span>
-    <span class="p">))</span></div>
+    <span class="n">columns</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">append_constraint</span><span class="p">(</span>
+        <span class="n">_sa</span><span class="o">.</span><span class="n">PrimaryKeyConstraint</span><span class="p">(</span><span class="o">*</span><span class="n">columns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+    <span class="p">)</span></div>
 
 
-<div class="viewcode-block" id="ForeignKey"><a class="viewcode-back" href="../../apidoc/gensaschema.constraints.html#gensaschema.constraints.ForeignKey">[docs]</a><span class="k">def</span> <span class="nf">ForeignKey</span><span class="p">(</span><span class="n">columns</span><span class="p">,</span> <span class="n">refcolumns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>  <span class="c1"># noqa pylint: disable = invalid-name</span>
+<div class="viewcode-block" id="ForeignKey"><a class="viewcode-back" href="../../apidoc/gensaschema.constraints.html#gensaschema.constraints.ForeignKey">[docs]</a><span class="k">def</span> <span class="nf">ForeignKey</span><span class="p">(</span>
+    <span class="n">columns</span><span class="p">,</span> <span class="n">refcolumns</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span>
+<span class="p">):</span>  <span class="c1"># noqa pylint: disable = invalid-name</span>
 <span class="w">    </span><span class="sa">r</span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Append foreign key</span>
 
 <span class="sd">    Parameters:</span>
 <span class="sd">      columns (sequence):</span>
 <span class="sd">        Source columns</span>
 
 <span class="sd">      refcolumns (sequence):</span>
 <span class="sd">        Referred columns</span>
 
 <span class="sd">      \*\*kwargs:</span>
 <span class="sd">        Additional parameters</span>
 <span class="sd">    &quot;&quot;&quot;</span>
-    <span class="n">columns</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">append_constraint</span><span class="p">(</span><span class="n">_sa</span><span class="o">.</span><span class="n">ForeignKeyConstraint</span><span class="p">(</span>
-        <span class="p">[</span><span class="n">col</span><span class="o">.</span><span class="n">name</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">],</span> <span class="n">refcolumns</span><span class="p">,</span> <span class="n">link_to_name</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span>
-    <span class="p">))</span></div>
+    <span class="n">columns</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">table</span><span class="o">.</span><span class="n">append_constraint</span><span class="p">(</span>
+        <span class="n">_sa</span><span class="o">.</span><span class="n">ForeignKeyConstraint</span><span class="p">(</span>
+            <span class="p">[</span><span class="n">col</span><span class="o">.</span><span class="n">name</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">],</span>
+            <span class="n">refcolumns</span><span class="p">,</span>
+            <span class="n">link_to_name</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+            <span class="o">**</span><span class="n">kwargs</span>
+        <span class="p">)</span>
+    <span class="p">)</span></div>
 </pre></div>
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
@@ -186,22 +192,22 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="../index.html" >Module code</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema.constraints</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema.constraints
 ****** Source code for gensaschema.constraints ******
 # -*- coding: ascii -*-
 """
 ========================
  Constraint Declarators
@@ -53,57 +53,63 @@
     Parameters:
       *columns:
         Constraint columns
 
       \*\*kwargs:
         Additional arguments
     """
-    columns[0].table.append_constraint(_sa.UniqueConstraint(
-        *columns, **kwargs
-    ))
+    columns[0].table.append_constraint(
+        _sa.UniqueConstraint(*columns, **kwargs)
+    )
 
 
 
 [docs]def PrimaryKey(*columns, **kwargs):  # pylint: disable = invalid-name
     r"""
     Append primary key
 
     Parameters:
       \*columns:
         Constraint columns
 
       \*\*kwargs:
         Additional parameters
     """
-    columns[0].table.append_constraint(_sa.PrimaryKeyConstraint(
-        *columns, **kwargs
-    ))
+    columns[0].table.append_constraint(
+        _sa.PrimaryKeyConstraint(*columns, **kwargs)
+    )
 
 
 
-[docs]def ForeignKey(columns, refcolumns, **kwargs):  # noqa pylint: disable =
-invalid-name
+[docs]def ForeignKey(
+    columns, refcolumns, **kwargs
+):  # noqa pylint: disable = invalid-name
     r"""
     Append foreign key
 
     Parameters:
       columns (sequence):
         Source columns
 
       refcolumns (sequence):
         Referred columns
 
       \*\*kwargs:
         Additional parameters
     """
-    columns[0].table.append_constraint(_sa.ForeignKeyConstraint(
-        [col.name for col in columns], refcolumns, link_to_name=True, **kwargs
-    ))
+    columns[0].table.append_constraint(
+        _sa.ForeignKeyConstraint(
+            [col.name for col in columns],
+            refcolumns,
+            link_to_name=True,
+            **kwargs
+        )
+    )
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Module_code »
     * gensaschema.constraints
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_modules/index.html` & `gensaschema-0.6.8/docs/userdoc/_modules/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Overview: module code &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>Overview: module code &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -40,15 +39,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">Overview: module code</a></li> 
       </ul>
     </div>
     </div>
   
 
@@ -113,21 +112,21 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">Overview: module code</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Overview: module code
 ****** All modules for which code is available ******
     * gensaschema._column
     * gensaschema._config
     * gensaschema._constraint
     * gensaschema._exceptions
     * gensaschema._meta
@@ -23,10 +23,10 @@
     * gensaschema._util
     * gensaschema.constraints
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Overview: module code
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_sources/apidoc/gensaschema.txt` & `gensaschema-0.6.8/docs/userdoc/_sources/apidoc/gensaschema.txt`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_sources/index.txt` & `gensaschema-0.6.8/docs/userdoc/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_sources/website_download.txt` & `gensaschema-0.6.8/docs/userdoc/_sources/website_download.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Download
 ~~~~~~~~
 
 Change Log
 ----------
 
-- `CHANGES file <http://storage.perlig.de/gensaschema/CHANGES-0.6.7>`_
+- `CHANGES file <http://storage.perlig.de/gensaschema/CHANGES-0.6.8>`_
 
 
 Source Packages
 ---------------
 
 .. begin stable
 
 Current Stable Version
 ''''''''''''''''''''''
 
-- `CHANGES file <http://storage.perlig.de/gensaschema/CHANGES-0.6.7>`_
-- `gensaschema-0.6.7.tar.xz <http://storage.perlig.de/gensaschema/gensaschema-0.6.7.tar.xz>`_
-- `gensaschema-0.6.7.tar.bz2 <http://storage.perlig.de/gensaschema/gensaschema-0.6.7.tar.bz2>`_
-- `gensaschema-0.6.7.tar.gz <http://storage.perlig.de/gensaschema/gensaschema-0.6.7.tar.gz>`_
-- `gensaschema-0.6.7.zip <http://storage.perlig.de/gensaschema/gensaschema-0.6.7.zip>`_
-- `gensaschema-0.6.7.digests <http://storage.perlig.de/gensaschema/gensaschema-0.6.7.digests>`_
+- `CHANGES file <http://storage.perlig.de/gensaschema/CHANGES-0.6.8>`_
+- `gensaschema-0.6.8.tar.xz <http://storage.perlig.de/gensaschema/gensaschema-0.6.8.tar.xz>`_
+- `gensaschema-0.6.8.tar.bz2 <http://storage.perlig.de/gensaschema/gensaschema-0.6.8.tar.bz2>`_
+- `gensaschema-0.6.8.tar.gz <http://storage.perlig.de/gensaschema/gensaschema-0.6.8.tar.gz>`_
+- `gensaschema-0.6.8.zip <http://storage.perlig.de/gensaschema/gensaschema-0.6.8.zip>`_
+- `gensaschema-0.6.8.digests <http://storage.perlig.de/gensaschema/gensaschema-0.6.8.digests>`_
 
 .. end stable
 
 
 .. begin dev
 .. end dev
 
 
 Integrity Check
 ---------------
 
 There are hashes (MD5, SHA1 and SHA256) of the download packages stored
 in the `digests file
-<http://storage.perlig.de/gensaschema/gensaschema-0.6.7.digests>`_\.
+<http://storage.perlig.de/gensaschema/gensaschema-0.6.8.digests>`_\.
 In order to check the integrity of the downloaded file, use a tool like
 md5sum (or sha1sum, sha256sum accordingly), e.g.:
 
 .. sourcecode:: console
 
-    $ md5sum -c gensaschema-0.6.7.digests
-    gensaschema-0.6.7.tar.bz2: OK
-    gensaschema-0.6.7.tar.gz: OK
-    gensaschema-0.6.7.tar.xz: OK
-    gensaschema-0.6.7.zip: OK
+    $ md5sum -c gensaschema-0.6.8.digests
+    gensaschema-0.6.8.tar.bz2: OK
+    gensaschema-0.6.8.tar.gz: OK
+    gensaschema-0.6.8.tar.xz: OK
+    gensaschema-0.6.8.zip: OK
 
 In order to check the integrity of the digest file itself, you can check
 the PGP signature of that file. The file is signed by André Malo, Key-ID
 0x029C942244325167:
 
 .. sourcecode:: console
 
-    $ gpg --verify gensaschema-0.6.7.digests
+    $ gpg --verify gensaschema-0.6.8.digests
     gpg: Signature made Fri May 20 10:03:36 2022 CEST
     gpg:                using RSA key 21B65583FF640D34E8662B6B3DED446369F2EE1A
     gpg: Good signature from "André Malo <nd@perlig.de>"
 
 
 .. vim: ft=rest tw=72
```

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/basic.css` & `gensaschema-0.6.8/docs/userdoc/_static/basic.css`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/cloud.base.js` & `gensaschema-0.6.8/docs/userdoc/_static/cloud.base.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/cloud.css` & `gensaschema-0.6.8/docs/userdoc/_static/cloud.css`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/cloud.js` & `gensaschema-0.6.8/docs/userdoc/_static/cloud.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/doctools.js` & `gensaschema-0.6.8/docs/userdoc/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-caution.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-caution.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-danger.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-danger.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-deprecated.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-deprecated.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-note.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-note.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-seealso.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-seealso.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-todo.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-todo.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/icon-warning.png` & `gensaschema-0.6.8/docs/userdoc/_static/icon-warning.png`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/jquery.cookie.js` & `gensaschema-0.6.8/docs/userdoc/_static/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/language_data.js` & `gensaschema-0.6.8/docs/userdoc/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/pygments.css` & `gensaschema-0.6.8/docs/userdoc/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/searchtools.js` & `gensaschema-0.6.8/docs/userdoc/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/_static/sphinx_highlight.js` & `gensaschema-0.6.8/docs/userdoc/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/cdbx._cdb.html` & `gensaschema-0.6.8/docs/userdoc/search.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,108 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-    <title>cdbx._cdb module &#8212; GenSASchema 0.6.7 documentation</title>
-    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+    <title>Search &#8212; GenSASchema 0.6.8 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="_static/cloud.css" />
+    <link rel="stylesheet" type="text/css" href="_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
-    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
-    <script src="../_static/doctools.js"></script>
-    <script src="../_static/sphinx_highlight.js"></script>
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
 
     
     
      
-        <script src="../_static/jquery.cookie.js"></script>
+        <script src="_static/jquery.cookie.js"></script>
     
 
     
      
-        <script src="../_static/cloud.base.js"></script>
+        <script src="_static/cloud.base.js"></script>
     
 
     
      
-        <script src="../_static/cloud.js"></script>
+        <script src="_static/cloud.js"></script>
     
 
-    <link rel="search" title="Search" href="../search.html" /> 
+    <script src="_static/searchtools.js"></script>
+    <script src="_static/language_data.js"></script>
+    <link rel="search" title="Search" href="#" />
+  <script src="searchindex.js" defer></script>
+   
         <meta name="viewport" content="width=device-width, initial-scale=1">
+
   </head><body>
     <div class="relbar-top">
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
-          <a href="../py-modindex.html" title="Python Module Index"
+          <a href="py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
-        <li class="nav-item nav-item-this"><a href="">cdbx._cdb module</a></li> 
+        <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     </div>
   
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
-  <section id="cdbx-cdb-module">
-<h1>cdbx._cdb module<a class="headerlink" href="#cdbx-cdb-module" title="Permalink to this heading">¶</a></h1>
-</section>
-
+  <h1 id="search-documentation">Search</h1>
+  
+  <noscript>
+  <div class="admonition warning">
+  <p>
+    Please activate JavaScript to enable the search
+    functionality.
+  </p>
+  </div>
+  </noscript>
+  
+  
+  <p>
+    Searching for multiple words only shows matches that contain
+    all words.
+  </p>
+  
+  
+  <form action="" method="get">
+    <input type="text" name="q" aria-labelledby="search-documentation" value="" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+    <input type="submit" value="search" />
+    <span id="search-progress" style="padding-left: 10px"></span>
+  </form>
+  
+  
+  
+  <div id="search-results">
+  
+  </div>
+  
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="../search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
     
     
         <div class="sidebar-toggle-group no-js">
             
             <button class="sidebar-toggle" id="sidebar-hide" title="Hide the sidebar menu">
@@ -102,23 +122,23 @@
     </div>
     <div class="relbar-bottom">
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
-          <a href="../py-modindex.html" title="Python Module Index"
+          <a href="py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
-        <li class="nav-item nav-item-this"><a href="">cdbx._cdb module</a></li> 
+        <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,18 +3,19 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
-    * cdbx._cdb module
-****** cdbx._cdb moduleÂ¶ ******
-**** Quick search ****
-[q                   ] [Go]
+    * GenSASchema_0.6.8_documentation »
+    * Search
+****** Search ******
+Please activate JavaScript to enable the search functionality.
+Searching for multiple words only shows matches that contain all words.
+[q                   ] [search]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
-    * cdbx._cdb module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+    * GenSASchema_0.6.8_documentation »
+    * Search
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._column.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._column.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._column module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._column module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._config.html" title="gensaschema._config module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema.html" title="gensaschema package"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._column module</a></li> 
       </ul>
     </div>
     </div>
@@ -414,23 +413,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._config.html" title="gensaschema._config module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema.html" title="gensaschema package"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._column module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._column module
 ****** gensaschema._column moduleÂ¶ ******
 ***** Column inspection and representationÂ¶ *****
 Column inspection and generation.
   Copyright:
@@ -168,12 +168,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._column module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._config.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._config.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._config module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._config module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._constraint.html" title="gensaschema._constraint module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._column.html" title="gensaschema._column module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._config module</a></li> 
       </ul>
     </div>
     </div>
@@ -334,23 +333,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._constraint.html" title="gensaschema._constraint module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._column.html" title="gensaschema._column module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._config module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._config module
 ****** gensaschema._config moduleÂ¶ ******
 ***** Schema config managementÂ¶ *****
 Schema config management.
   Copyright:
@@ -128,12 +128,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._config module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._constraint.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._constraint.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._constraint module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._constraint module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._exceptions.html" title="gensaschema._exceptions module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._config.html" title="gensaschema._config module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._constraint module</a></li> 
       </ul>
     </div>
     </div>
@@ -430,23 +429,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._exceptions.html" title="gensaschema._exceptions module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._config.html" title="gensaschema._config module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._constraint module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._constraint module
 ****** gensaschema._constraint moduleÂ¶ ******
 ***** Constraint inspection and representationÂ¶ *****
 Constraint inspection and representation.
   Copyright:
@@ -161,12 +161,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._constraint module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._exceptions.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._exceptions.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._exceptions module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._exceptions module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._meta.html" title="gensaschema._meta module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._constraint.html" title="gensaschema._constraint module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._exceptions module</a></li> 
       </ul>
     </div>
     </div>
@@ -255,23 +254,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._meta.html" title="gensaschema._meta module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._constraint.html" title="gensaschema._constraint module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._exceptions module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._exceptions module
 ****** gensaschema._exceptions moduleÂ¶ ******
   Copyright:
       Copyright 2014 - 2023 AndrÃ© Malo or his licensors, as applicable
   License:
@@ -84,12 +84,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._exceptions module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._meta.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._meta.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._meta module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._meta module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._schema.html" title="gensaschema._schema module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._exceptions.html" title="gensaschema._exceptions module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._meta module</a></li> 
       </ul>
     </div>
     </div>
@@ -202,23 +201,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._schema.html" title="gensaschema._schema module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._exceptions.html" title="gensaschema._exceptions module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._meta module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._meta module
 ****** gensaschema._meta moduleÂ¶ ******
 ***** MetadataÂ¶ *****
 Schema module generation code.
   Copyright:
@@ -61,12 +61,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._meta module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._schema.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._schema.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._schema module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._schema module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._symbols.html" title="gensaschema._symbols module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._meta.html" title="gensaschema._meta module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._schema module</a></li> 
       </ul>
     </div>
     </div>
@@ -305,23 +304,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._symbols.html" title="gensaschema._symbols module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._meta.html" title="gensaschema._meta module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._schema module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._schema module
 ****** gensaschema._schema moduleÂ¶ ******
 ***** Schema module generationÂ¶ *****
 Schema module generation code.
   Copyright:
@@ -118,12 +118,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._schema module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._symbols.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._symbols.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._symbols module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._symbols module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._table.html" title="gensaschema._table module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._schema.html" title="gensaschema._schema module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._symbols module</a></li> 
       </ul>
     </div>
     </div>
@@ -588,23 +587,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._table.html" title="gensaschema._table module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._schema.html" title="gensaschema._schema module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._symbols module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._symbols module
 ****** gensaschema._symbols moduleÂ¶ ******
 ***** Symbol managementÂ¶ *****
 Symbol management.
   Copyright:
@@ -251,12 +251,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._symbols module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._table.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._table.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._table module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._table module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._template.html" title="gensaschema._template module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._symbols.html" title="gensaschema._symbols module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._table module</a></li> 
       </ul>
     </div>
     </div>
@@ -226,14 +225,20 @@
 SQLAlchemy cannot resolve it, the type loader will be called with
 the type name, (bound) metadata and the symbol table. It is
 responsible for modifying the symbols and imports <em>and</em> the
 dialect’s <code class="docutils literal notranslate"><span class="pre">ischema_names</span></code>. If omitted or <code class="docutils literal notranslate"><span class="pre">None</span></code>, the reflector
 will always fail on unknown types.</p></li>
 </ul>
 </dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>new Table instance</p>
+</dd>
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p><a class="reference internal" href="#gensaschema._table.Table" title="gensaschema._table.Table">Table</a></p>
+</dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="gensaschema._table.Table.is_reference">
 <span class="sig-name descname"><span class="pre">is_reference</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">False</span></em><a class="headerlink" href="#gensaschema._table.Table.is_reference" title="Permalink to this definition">¶</a></dt>
 <dd><p>Is it a table reference (vs. a table)?</p>
@@ -248,15 +253,15 @@
 
 <dl class="py class">
 <dt class="sig sig-object py" id="gensaschema._table.TableCollection">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">gensaschema._table.</span></span><span class="sig-name descname"><span class="pre">TableCollection</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">iterable</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">/</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="../_modules/gensaschema/_table.html#TableCollection"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#gensaschema._table.TableCollection" title="Permalink to this definition">¶</a></dt>
 <dd><p>Table collection</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="gensaschema._table.TableCollection.__dict__">
-<span class="sig-name descname"><span class="pre">__dict__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">mappingproxy({'__module__':</span> <span class="pre">'gensaschema._table',</span> <span class="pre">'__doc__':</span> <span class="pre">'</span> <span class="pre">Table</span> <span class="pre">collection</span> <span class="pre">',</span> <span class="pre">'by_names':</span> <span class="pre">&lt;classmethod(&lt;function</span> <span class="pre">TableCollection.by_names&gt;)&gt;,</span> <span class="pre">'__dict__':</span> <span class="pre">&lt;attribute</span> <span class="pre">'__dict__'</span> <span class="pre">of</span> <span class="pre">'TableCollection'</span> <span class="pre">objects&gt;,</span> <span class="pre">'__annotations__':</span> <span class="pre">{}})</span></em><a class="headerlink" href="#gensaschema._table.TableCollection.__dict__" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">__dict__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">mappingproxy({'__module__':</span> <span class="pre">'gensaschema._table',</span> <span class="pre">'__doc__':</span> <span class="pre">'Table</span> <span class="pre">collection',</span> <span class="pre">'by_names':</span> <span class="pre">&lt;classmethod(&lt;function</span> <span class="pre">TableCollection.by_names&gt;)&gt;,</span> <span class="pre">'__dict__':</span> <span class="pre">&lt;attribute</span> <span class="pre">'__dict__'</span> <span class="pre">of</span> <span class="pre">'TableCollection'</span> <span class="pre">objects&gt;,</span> <span class="pre">'__annotations__':</span> <span class="pre">{}})</span></em><a class="headerlink" href="#gensaschema._table.TableCollection.__dict__" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="gensaschema._table.TableCollection.__module__">
 <span class="sig-name descname"><span class="pre">__module__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'gensaschema._table'</span></em><a class="headerlink" href="#gensaschema._table.TableCollection.__module__" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
@@ -483,23 +488,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._template.html" title="gensaschema._template module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._symbols.html" title="gensaschema._symbols module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._table module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._table module
 ****** gensaschema._table moduleÂ¶ ******
 ***** Table inspection and representationÂ¶ *****
 Table inspection and representation
   Copyright:
@@ -98,22 +98,26 @@
                       * types (callable) â Extra type loader. If the type
                         reflection fails, because SQLAlchemy cannot resolve it,
                         the type loader will be called with the type name,
                         (bound) metadata and the symbol table. It is
                         responsible for modifying the symbols and imports and
                         the dialectâs ischema_names. If omitted or None, the
                         reflector will always fail on unknown types.
+              Returns:
+                  new Table instance
+              Return type:
+                  Table
         is_reference= FalseÂ¶
             Is it a table reference (vs. a table)?
               Type:
                   bool
   classgensaschema._table.TableCollection(iterable=(), /)[source]Â¶
       Table collection
         __dict__= mappingproxy({'__module__': 'gensaschema._table', '__doc__':
-        ' Table collection ', 'by_names': <classmethod(<function
+        'Table collection', 'by_names': <classmethod(<function
         TableCollection.by_names>)>, '__dict__': <attribute '__dict__' of
         'TableCollection' objects>, '__annotations__': {}})Â¶
         __module__= 'gensaschema._table'Â¶
         classmethodby_names(metadata, names, schemas, symbols, types=None)
         [source]Â¶
             Construct by table names
               Parameters:
@@ -209,12 +213,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._table module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._template.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._template.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._template module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._template module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._type.html" title="gensaschema._type module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._table.html" title="gensaschema._table module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._template module</a></li> 
       </ul>
     </div>
     </div>
@@ -244,23 +243,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._type.html" title="gensaschema._type module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._table.html" title="gensaschema._table module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._template module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._template module
 ****** gensaschema._template moduleÂ¶ ******
 ***** Simple template abstractionÂ¶ *****
 Simple template abstraction.
   Copyright:
@@ -82,12 +82,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._template module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._type.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._type.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._type module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._type module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._util.html" title="gensaschema._util module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._template.html" title="gensaschema._template module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._type module</a></li> 
       </ul>
     </div>
     </div>
@@ -196,14 +195,31 @@
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
+<dt class="sig sig-object py" id="gensaschema._type._add_postgres_enum">
+<span class="sig-prename descclassname"><span class="pre">gensaschema._type.</span></span><span class="sig-name descname"><span class="pre">_add_postgres_enum</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ctype</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">symbols</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="../_modules/gensaschema/_type.html#_add_postgres_enum"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#gensaschema._type._add_postgres_enum" title="Permalink to this definition">¶</a></dt>
+<dd><p>Add postgres enum</p>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="gensaschema._type._finalize_type">
+<span class="sig-prename descclassname"><span class="pre">gensaschema._type.</span></span><span class="sig-name descname"><span class="pre">_finalize_type</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ctype</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dialect</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">symbols</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="../_modules/gensaschema/_type.html#_finalize_type"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#gensaschema._type._finalize_type" title="Permalink to this definition">¶</a></dt>
+<dd><p>Finalize type definitions and modifications</p>
+<dl class="field-list simple">
+<dt class="field-odd">TODO<span class="colon">:</span></dt>
+<dd class="field-odd"><p>should be generalized at some point in the future.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py function">
 <dt class="sig sig-object py" id="gensaschema._type._find_class">
 <span class="sig-prename descclassname"><span class="pre">gensaschema._type.</span></span><span class="sig-name descname"><span class="pre">_find_class</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">first_cls</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="../_modules/gensaschema/_type.html#_find_class"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#gensaschema._type._find_class" title="Permalink to this definition">¶</a></dt>
 <dd><p>Find class where a method is defined</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>first_cls</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">type</span></code>) – Class to start with</p></li>
@@ -241,14 +257,16 @@
 <li><a class="reference internal" href="#gensaschema._type.Type.__init__"><code class="docutils literal notranslate"><span class="pre">Type.__init__()</span></code></a></li>
 <li><a class="reference internal" href="#gensaschema._type.Type.__module__"><code class="docutils literal notranslate"><span class="pre">Type.__module__</span></code></a></li>
 <li><a class="reference internal" href="#gensaschema._type.Type.__repr__"><code class="docutils literal notranslate"><span class="pre">Type.__repr__()</span></code></a></li>
 <li><a class="reference internal" href="#gensaschema._type.Type.__weakref__"><code class="docutils literal notranslate"><span class="pre">Type.__weakref__</span></code></a></li>
 <li><a class="reference internal" href="#gensaschema._type.Type.by_column"><code class="docutils literal notranslate"><span class="pre">Type.by_column()</span></code></a></li>
 </ul>
 </li>
+<li><a class="reference internal" href="#gensaschema._type._add_postgres_enum"><code class="docutils literal notranslate"><span class="pre">_add_postgres_enum()</span></code></a></li>
+<li><a class="reference internal" href="#gensaschema._type._finalize_type"><code class="docutils literal notranslate"><span class="pre">_finalize_type()</span></code></a></li>
 <li><a class="reference internal" href="#gensaschema._type._find_class"><code class="docutils literal notranslate"><span class="pre">_find_class()</span></code></a></li>
 </ul>
 </li>
 </ul>
 
   </div>
   <div class="sphinxprev">
@@ -302,23 +320,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._util.html" title="gensaschema._util module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._template.html" title="gensaschema._template module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._type module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._type module
 ****** gensaschema._type moduleÂ¶ ******
 ***** Type inspection and representationÂ¶ *****
 Type inspection and representation.
   Copyright:
@@ -72,14 +72,20 @@
             Construct by SA column
               Parameters:
                   column (SA column) â SA column
               Returns:
                   New Type instance
               Return type:
                   Type
+  gensaschema._type._add_postgres_enum(ctype, symbols)[source]Â¶
+      Add postgres enum
+  gensaschema._type._finalize_type(ctype, dialect, symbols)[source]Â¶
+      Finalize type definitions and modifications
+        TODO:
+            should be generalized at some point in the future.
   gensaschema._type._find_class(first_cls, name)[source]Â¶
       Find class where a method is defined
         Parameters:
                 * first_cls (type) â Class to start with
                 * name (str) â Method name
         Returns:
             class or None
@@ -95,24 +101,26 @@
                 # Type.__annotations__
                 # Type.__dict__
                 # Type.__init__()
                 # Type.__module__
                 # Type.__repr__()
                 # Type.__weakref__
                 # Type.by_column()
+          o _add_postgres_enum()
+          o _finalize_type()
           o _find_class()
 *** Previous page ***
 ←_gensaschema._template_module
 *** Next page ***
 →_gensaschema._util_module
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._type module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema._util.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema._util.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema._util module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema._util module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema.constraints.html" title="gensaschema.constraints module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._type.html" title="gensaschema._type module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._util module</a></li> 
       </ul>
     </div>
     </div>
@@ -189,23 +188,23 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema.constraints.html" title="gensaschema.constraints module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="gensaschema._type.html" title="gensaschema._type module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema._util module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._util module
 ****** gensaschema._util moduleÂ¶ ******
   Copyright:
       Copyright 2014 - 2023 Andrxe9 Malo or his licensors, as applicable
   License:
@@ -54,12 +54,12 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema._util module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema.constraints.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema.constraints.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema.constraints module &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema.constraints module &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -45,15 +44,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._util.html" title="gensaschema._util module"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" accesskey="U">gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema.constraints module</a></li> 
       </ul>
     </div>
     </div>
@@ -198,23 +197,23 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._util.html" title="gensaschema._util module"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="gensaschema.html" >gensaschema package</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema.constraints module</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 **** Navigation ****
     * modules
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema.constraints module
 ****** gensaschema.constraints moduleÂ¶ ******
 ***** Constraint DeclaratorsÂ¶ *****
 Helper functions to define constraints. These will be part of the generated
 schema modules. Copy or the reference the module where needed. The location is
@@ -56,12 +56,12 @@
 ←_gensaschema._util_module
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema_package »
     * gensaschema.constraints module
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/gensaschema.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/gensaschema.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema package &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema package &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._column.html" title="gensaschema._column module"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="index.html" title="gensaschema"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">gensaschema</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema package</a></li> 
       </ul>
     </div>
     </div>
   
@@ -323,14 +322,16 @@
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type.__init__"><code class="docutils literal notranslate"><span class="pre">Type.__init__()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type.__module__"><code class="docutils literal notranslate"><span class="pre">Type.__module__</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type.__repr__"><code class="docutils literal notranslate"><span class="pre">Type.__repr__()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type.__weakref__"><code class="docutils literal notranslate"><span class="pre">Type.__weakref__</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type.by_column"><code class="docutils literal notranslate"><span class="pre">Type.by_column()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._add_postgres_enum"><code class="docutils literal notranslate"><span class="pre">_add_postgres_enum()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._finalize_type"><code class="docutils literal notranslate"><span class="pre">_finalize_type()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._find_class"><code class="docutils literal notranslate"><span class="pre">_find_class()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="gensaschema._util.html">gensaschema._util module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="gensaschema._util.html#misc-utilities">Misc Utilities</a></li>
 <li class="toctree-l2"><a class="reference internal" href="gensaschema._util.html#gensaschema._util.cmp"><code class="docutils literal notranslate"><span class="pre">cmp()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="gensaschema._util.html#gensaschema._util.find_public"><code class="docutils literal notranslate"><span class="pre">find_public()</span></code></a></li>
@@ -1127,22 +1128,22 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema._column.html" title="gensaschema._column module"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="index.html" title="gensaschema"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
           <li class="nav-item nav-item-1"><a href="index.html" >gensaschema</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">gensaschema package</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema package
 ****** gensaschema packageÂ¶ ******
 ***** SubmodulesÂ¶ *****
     * gensaschema._column_module
           o Column_inspection_and_representation
           o Column
@@ -208,14 +208,16 @@
                 # Type.__annotations__
                 # Type.__dict__
                 # Type.__init__()
                 # Type.__module__
                 # Type.__repr__()
                 # Type.__weakref__
                 # Type.by_column()
+          o _add_postgres_enum()
+          o _finalize_type()
           o _find_class()
     * gensaschema._util_module
           o Misc_Utilities
           o cmp()
           o find_public()
     * gensaschema.constraints_module
           o Constraint_Declarators
@@ -598,11 +600,11 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema »
     * gensaschema package
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/index.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -49,15 +48,15 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema.html" title="gensaschema package"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="../index.html" title="GenSASchema - Static SQLAlchemy Schema Generator"
              accesskey="P">previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">gensaschema</a></li> 
       </ul>
     </div>
     </div>
   
 
@@ -129,14 +128,16 @@
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._template.html#simple-template-abstraction">Simple template abstraction</a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._template.html#gensaschema._template.Template"><code class="docutils literal notranslate"><span class="pre">Template</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html">gensaschema._type module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#type-inspection-and-representation">Type inspection and representation</a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._add_postgres_enum"><code class="docutils literal notranslate"><span class="pre">_add_postgres_enum()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._finalize_type"><code class="docutils literal notranslate"><span class="pre">_finalize_type()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._find_class"><code class="docutils literal notranslate"><span class="pre">_find_class()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._util.html">gensaschema._util module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._util.html#misc-utilities">Misc Utilities</a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._util.html#gensaschema._util.cmp"><code class="docutils literal notranslate"><span class="pre">cmp()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._util.html#gensaschema._util.find_public"><code class="docutils literal notranslate"><span class="pre">find_public()</span></code></a></li>
@@ -291,21 +292,21 @@
              >modules</a></li>
         <li class="right" >
           <a href="gensaschema.html" title="gensaschema package"
              >next</a> &nbsp; &nbsp;</li>
         <li class="right" >
           <a href="../index.html" title="GenSASchema - Static SQLAlchemy Schema Generator"
              >previous</a> &nbsp; &nbsp;</li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">gensaschema</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema
 ****** gensaschemaÂ¶ ******
     * gensaschema_package
           o Submodules
                 # gensaschema._column_module
                       # Column_inspection_and_representation
                       # Column
@@ -55,14 +55,16 @@
                       # _break_cycles()
                 # gensaschema._template_module
                       # Simple_template_abstraction
                       # Template
                 # gensaschema._type_module
                       # Type_inspection_and_representation
                       # Type
+                      # _add_postgres_enum()
+                      # _finalize_type()
                       # _find_class()
                 # gensaschema._util_module
                       # Misc_Utilities
                       # cmp()
                       # find_public()
                 # gensaschema.constraints_module
                       # Constraint_Declarators
@@ -136,10 +138,10 @@
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
     * previous    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/apidoc/modules.html` & `gensaschema-0.6.8/docs/userdoc/apidoc/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>gensaschema &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>gensaschema &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="../_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -41,15 +40,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">gensaschema</a></li> 
       </ul>
     </div>
     </div>
   
 
@@ -121,14 +120,16 @@
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._template.html#simple-template-abstraction">Simple template abstraction</a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._template.html#gensaschema._template.Template"><code class="docutils literal notranslate"><span class="pre">Template</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._type.html">gensaschema._type module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#type-inspection-and-representation">Type inspection and representation</a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._add_postgres_enum"><code class="docutils literal notranslate"><span class="pre">_add_postgres_enum()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._finalize_type"><code class="docutils literal notranslate"><span class="pre">_finalize_type()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._type.html#gensaschema._type._find_class"><code class="docutils literal notranslate"><span class="pre">_find_class()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="gensaschema._util.html">gensaschema._util module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._util.html#misc-utilities">Misc Utilities</a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._util.html#gensaschema._util.cmp"><code class="docutils literal notranslate"><span class="pre">cmp()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="gensaschema._util.html#gensaschema._util.find_public"><code class="docutils literal notranslate"><span class="pre">find_public()</span></code></a></li>
@@ -267,21 +268,21 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a></li>
-    <li><a href="../index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="../index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">gensaschema</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema
 ****** gensaschemaÂ¶ ******
     * gensaschema_package
           o Submodules
                 # gensaschema._column_module
                       # Column_inspection_and_representation
                       # Column
@@ -51,14 +51,16 @@
                       # _break_cycles()
                 # gensaschema._template_module
                       # Simple_template_abstraction
                       # Template
                 # gensaschema._type_module
                       # Type_inspection_and_representation
                       # Type
+                      # _add_postgres_enum()
+                      # _finalize_type()
                       # _find_class()
                 # gensaschema._util_module
                       # Misc_Utilities
                       # cmp()
                       # find_public()
                 # gensaschema.constraints_module
                       # Constraint_Declarators
@@ -126,10 +128,10 @@
                       # Warning.__weakref__
                       # Warning.emit()
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * gensaschema
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/index.html` & `gensaschema-0.6.8/docs/userdoc/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>GenSASchema - Static SQLAlchemy Schema Generator &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>GenSASchema - Static SQLAlchemy Schema Generator &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -45,15 +44,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a></li>
         <li class="right" >
           <a href="apidoc/index.html" title="gensaschema"
              accesskey="N">next</a> &nbsp; &nbsp;</li>
-    <li><a href="#">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="#">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">GenSASchema - Static SQLAlchemy Schema Generator</a></li> 
       </ul>
     </div>
     </div>
   
 
@@ -167,21 +166,21 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a></li>
         <li class="right" >
           <a href="apidoc/index.html" title="gensaschema"
              >next</a> &nbsp; &nbsp;</li>
-    <li><a href="#">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="#">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">GenSASchema - Static SQLAlchemy Schema Generator</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 **** Navigation ****
     * modules
     * next    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * GenSASchema - Static SQLAlchemy Schema Generator
 ****** GenSASchema - Static SQLAlchemy Schema GeneratorÂ¶ ******
 GenSASchema is a static SQLAlchemy Schema Generator.
 Supported python versions are Python 2.7 and Python 3.6 and above.
 ***** DocumentationÂ¶ *****
     * Documentation_Search (needs javascript)
     * API_Documentation (generated)
@@ -50,10 +50,10 @@
 →_gensaschema
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
     * next    
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * GenSASchema - Static SQLAlchemy Schema Generator
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/py-modindex.html` & `gensaschema-0.6.8/docs/userdoc/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; GenSASchema 0.6.7 documentation</title>
+    <title>Python Module Index &#8212; GenSASchema 0.6.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/cloud.css" />
     <link rel="stylesheet" type="text/css" href="_static/ci.css" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Noticia+Text:400,i,b,bi|Open+Sans:400,i,b,bi|Roboto+Mono:400,i,b,bi&amp;display=swap" type="text/css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -43,15 +42,15 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="Python Module Index"
              >modules</a></li>
-    <li><a href="index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     </div>
   
 
@@ -181,21 +180,21 @@
         
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="Python Module Index"
              >modules</a></li>
-    <li><a href="index.html">GenSASchema 0.6.7 documentation</a> &#187;</li>
+    <li><a href="index.html">GenSASchema 0.6.8 documentation</a> &#187;</li>
 
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     </div>
 
     <div class="footer" role="contentinfo">
         &#169; Copyright 2015 - 2023 André Malo.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
     <!-- cloud_sptheme 1.4 -->
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Python Module Index
 ****** Python Module Index ******
 g
      
     g
 [-] gensaschema
         gensaschema._column
@@ -27,10 +27,10 @@
         gensaschema._util
         gensaschema.constraints
 **** Quick search ****
 [q                   ] [Go]
  Â« hide menu   menu sidebar Â»
 **** Navigation ****
     * modules
-    * GenSASchema_0.6.7_documentation »
+    * GenSASchema_0.6.8_documentation »
     * Python Module Index
-© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 6.1.2.
+© Copyright 2015 - 2023 AndrÃ© Malo. Created using Sphinx 7.0.1.
```

### Comparing `gensaschema-0.6.7/docs/userdoc/searchindex.js` & `gensaschema-0.6.8/docs/userdoc/searchindex.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,825 +1,838 @@
 Search.setIndex({
-    "docnames": ["apidoc/cdbx", "apidoc/cdbx._cdb", "apidoc/gensaschema", "apidoc/gensaschema._column", "apidoc/gensaschema._config", "apidoc/gensaschema._constraint", "apidoc/gensaschema._exceptions", "apidoc/gensaschema._meta", "apidoc/gensaschema._schema", "apidoc/gensaschema._symbols", "apidoc/gensaschema._table", "apidoc/gensaschema._template", "apidoc/gensaschema._type", "apidoc/gensaschema._util", "apidoc/gensaschema.constraints", "apidoc/index", "apidoc/modules", "index", "website_download"],
-    "filenames": ["apidoc/cdbx.txt", "apidoc/cdbx._cdb.txt", "apidoc/gensaschema.txt", "apidoc/gensaschema._column.txt", "apidoc/gensaschema._config.txt", "apidoc/gensaschema._constraint.txt", "apidoc/gensaschema._exceptions.txt", "apidoc/gensaschema._meta.txt", "apidoc/gensaschema._schema.txt", "apidoc/gensaschema._symbols.txt", "apidoc/gensaschema._table.txt", "apidoc/gensaschema._template.txt", "apidoc/gensaschema._type.txt", "apidoc/gensaschema._util.txt", "apidoc/gensaschema.constraints.txt", "apidoc/index.txt", "apidoc/modules.txt", "index.txt", "website_download.txt"],
-    "titles": ["cdbx package", "cdbx._cdb module", "gensaschema package", "gensaschema._column module", "gensaschema._config module", "gensaschema._constraint module", "gensaschema._exceptions module", "gensaschema._meta module", "gensaschema._schema module", "gensaschema._symbols module", "gensaschema._table module", "gensaschema._template module", "gensaschema._type module", "gensaschema._util module", "gensaschema.constraints module", "gensaschema", "gensaschema", "GenSASchema - Static SQLAlchemy Schema Generator", "Download"],
+    "docnames": ["apidoc/gensaschema", "apidoc/gensaschema._column", "apidoc/gensaschema._config", "apidoc/gensaschema._constraint", "apidoc/gensaschema._exceptions", "apidoc/gensaschema._meta", "apidoc/gensaschema._schema", "apidoc/gensaschema._symbols", "apidoc/gensaschema._table", "apidoc/gensaschema._template", "apidoc/gensaschema._type", "apidoc/gensaschema._util", "apidoc/gensaschema.constraints", "apidoc/index", "apidoc/modules", "index", "website_download"],
+    "filenames": ["apidoc/gensaschema.txt", "apidoc/gensaschema._column.txt", "apidoc/gensaschema._config.txt", "apidoc/gensaschema._constraint.txt", "apidoc/gensaschema._exceptions.txt", "apidoc/gensaschema._meta.txt", "apidoc/gensaschema._schema.txt", "apidoc/gensaschema._symbols.txt", "apidoc/gensaschema._table.txt", "apidoc/gensaschema._template.txt", "apidoc/gensaschema._type.txt", "apidoc/gensaschema._util.txt", "apidoc/gensaschema.constraints.txt", "apidoc/index.txt", "apidoc/modules.txt", "index.txt", "website_download.txt"],
+    "titles": ["gensaschema package", "gensaschema._column module", "gensaschema._config module", "gensaschema._constraint module", "gensaschema._exceptions module", "gensaschema._meta module", "gensaschema._schema module", "gensaschema._symbols module", "gensaschema._table module", "gensaschema._template module", "gensaschema._type module", "gensaschema._util module", "gensaschema.constraints module", "gensaschema", "gensaschema", "GenSASchema - Static SQLAlchemy Schema Generator", "Download"],
     "terms": {
-        "gensaschema": [0, 1, 18],
-        "_cdb": 0,
-        "_column": [2, 15, 16],
-        "column": [2, 5, 12, 14, 15, 16],
-        "inspect": [2, 13, 15, 16],
-        "represent": [2, 15, 16],
-        "_name": [2, 3],
-        "_ctype": [2, 3, 12, 15, 16],
-        "_nullabl": [2, 3],
-        "_primary_kei": [2, 3],
-        "_autoincr": [2, 3],
-        "_server_default": [2, 3],
-        "_symbol": [2, 3, 5, 8, 10, 12, 15, 16],
-        "__dict__": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12, 15, 16],
-        "__init__": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12, 15, 16],
-        "__module__": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
-        "__repr__": [2, 3, 5, 10, 12, 15, 16],
-        "__weakref__": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
-        "from_sa": [2, 3],
-        "serverdefault": [2, 3, 15, 16],
-        "_default": [2, 3],
-        "_config": [2, 15, 16],
-        "config": [2, 15, 16],
-        "manag": [2, 15, 16],
-        "tabl": [2, 3, 4, 5, 8, 9, 12, 15, 16],
-        "_line": [2, 4, 15, 16],
-        "_config_tpl": [2, 4, 15, 16],
-        "__annotations__": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
-        "dump": [2, 4, 8, 15, 16],
-        "from_fil": [2, 4, 15, 16],
-        "from_lin": [2, 4, 15, 16],
-        "from_pars": [2, 4, 15, 16],
-        "_constraint": [2, 15, 16],
-        "constraint": [2, 10, 15, 16],
-        "_import": [2, 5, 9, 15, 16],
-        "__cmp__": [2, 5],
-        "__lt__": [2, 5],
-        "__new__": [2, 5, 10],
-        "copi": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "repr": [2, 5],
-        "foreignkeyconstraint": [2, 5, 15, 16],
-        "primarykeyconstraint": [2, 5, 15, 16],
-        "uniqueconstraint": [2, 5, 15, 16],
-        "access_col": [2, 5, 15, 16],
-        "_except": [2, 15, 16],
-        "except": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16],
-        "error": [2, 4, 6, 9, 15, 16],
-        "warn": [2, 6, 15, 16],
-        "emit": [2, 6, 8, 15, 16],
-        "_meta": [2, 15, 16],
-        "metadata": [2, 8, 10, 15, 16],
-        "boundmetadata": [2, 7, 15, 16],
-        "__getattr__": [2, 7],
-        "_schema": [2, 15, 16],
-        "_dialect": [2, 8, 12, 15, 16],
-        "_tabl": [2, 8, 15, 16],
-        "_dbname": [2, 8, 15, 16],
-        "_module_tpl": [2, 8, 15, 16],
-        "symbol": [2, 3, 5, 8, 10, 12, 13, 15, 16],
-        "symbolexcept": [2, 9, 15, 16],
-        "import": [2, 5, 6, 8, 9, 10, 15, 16],
-        "type": [2, 3, 4, 5, 8, 9, 10, 11, 13, 15, 16],
-        "__contains__": [2, 9, 15, 16],
-        "__delitem__": [2, 9, 15, 16],
-        "__getitem__": [2, 9, 15, 16],
-        "__iter__": [2, 9, 15, 16],
-        "__setitem__": [2, 9, 15, 16],
-        "_type": [2, 9, 15, 16],
-        "resolv": [2, 8, 9, 10],
-        "_load_dot": [2, 9, 15, 16],
-        "varnam": [2, 5, 10],
-        "sa_tabl": [2, 10],
-        "by_nam": [2, 10],
-        "is_refer": [2, 10],
-        "tablecollect": [2, 8, 10, 15, 16],
-        "tablerefer": [2, 10, 15, 16],
-        "_break_cycl": [2, 10, 15, 16],
-        "_templat": [2, 4, 8, 15, 16],
-        "simpl": [2, 15, 16],
-        "templat": [2, 4, 8, 15, 16],
-        "abstract": [2, 15, 16],
-        "expand": [2, 11],
-        "by_column": [2, 12, 15, 16],
-        "_find_class": [2, 12, 15, 16],
-        "_util": [2, 15, 16],
-        "misc": [2, 15, 16],
-        "util": [2, 15, 16],
-        "cmp": [2, 13, 15, 16],
-        "find_publ": [2, 13, 15, 16],
-        "declar": [2, 15, 16],
-        "foreignkei": [2, 5, 14, 15, 16],
-        "primarykei": [2, 5, 14, 15, 16],
-        "uniqu": [2, 5, 9, 14, 15, 16],
-        "copyright": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "2014": [2, 6, 13],
-        "2023": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "andr\u00e9": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 17, 18],
-        "malo": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17, 18],
-        "hi": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "licensor": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "applic": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "licens": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "under": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "apach": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "version": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "2": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "0": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17, 18],
-        "you": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17, 18],
-        "mai": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 18],
-        "us": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 18],
-        "thi": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "file": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 18],
-        "complianc": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "obtain": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "http": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "www": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "org": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "unless": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "requir": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "law": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "agre": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "write": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "softwar": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "distribut": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "i": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17, 18],
-        "an": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "AS": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "basi": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "without": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "warranti": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "OR": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "condit": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "OF": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "ani": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "kind": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "either": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "express": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "impli": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "see": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "specif": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "languag": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "govern": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "permiss": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "limit": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "definit": 2,
-        "": [2, 5, 7, 8, 9, 10],
-        "capabl": 2,
-        "class": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12],
-        "line": [2, 4, 5],
-        "none": [2, 4, 5, 8, 9, 10, 12],
-        "sourc": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 17],
-        "contain": [2, 3, 4, 8, 9, 10, 11, 12, 13],
-        "list": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13],
-        "alien": [2, 4],
-        "map": [2, 4, 8, 9, 10],
-        "dict": [2, 4, 5, 8, 9, 10, 11, 13],
-        "origin": [2, 4],
-        "object": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
-        "empti": [2, 4, 9],
-        "mappingproxi": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12],
-        "__doc__": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12],
-        "n": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12],
-        "attribut": [2, 3, 4, 5, 7, 8, 9, 10, 11, 12],
-        "function": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14],
-        "classmethod": [2, 3, 4, 6, 10, 12],
-        "initi": [2, 3, 4, 5, 8, 9, 10, 11, 12],
-        "paramet": [2, 3, 4, 5, 6, 8, 9, 10, 11, 12, 13, 14],
-        "iter": [2, 4, 5, 9, 10],
-        "If": [2, 4, 8, 9, 10, 11, 13],
-        "omit": [2, 4, 8, 9, 10],
-        "ar": [2, 4, 5, 13, 17, 18],
-        "avail": [2, 4, 9, 17],
-        "weak": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
-        "refer": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14],
-        "defin": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14],
-        "fp": [2, 4, 8],
-        "stream": [2, 4],
-        "name_or_fil": [2, 4],
-        "construct": [2, 3, 4, 10, 12],
-        "from": [2, 3, 4, 5, 9, 18],
-        "str": [2, 3, 4, 5, 6, 8, 9, 10, 11, 12],
-        "filenam": [2, 4],
-        "pointer": [2, 4],
-        "return": [2, 3, 4, 5, 9, 10, 11, 12, 13],
-        "new": [2, 3, 4, 10, 12],
-        "instanc": [2, 3, 4, 10, 12],
-        "rais": [2, 4, 9, 11],
-        "ioerror": [2, 4],
-        "read": [2, 4],
-        "enoent": [2, 4],
-        "which": [2, 4, 9],
-        "treat": [2, 4],
-        "creat": [2, 4, 5],
-        "parser": [2, 4],
-        "configpars": [2, 4],
-        "rawconfigpars": [2, 4],
-        "base": [2, 5, 6],
-        "conn": [2, 8],
-        "dbname": [2, 8],
-        "dialect": [2, 8, 9, 10, 12],
-        "name": [2, 3, 5, 7, 8, 9, 10, 12, 13],
-        "collect": [2, 8, 10],
-        "db": [2, 8],
-        "identifi": [2, 8, 9],
-        "connect": [2, 8],
-        "engin": [2, 8],
-        "reflect": [2, 5, 8, 10],
-        "local": [2, 8],
-        "pair": [2, 8],
-        "option": [2, 5, 8],
-        "inform": [2, 8],
-        "purpos": [2, 8],
-        "just": [2, 8],
-        "won": [2, 8],
-        "t": [2, 8],
-        "callabl": [2, 8, 10],
-        "extra": [2, 8, 10],
-        "loader": [2, 8, 10],
-        "fail": [2, 8, 10],
-        "becaus": [2, 8, 9, 10],
-        "cannot": [2, 8, 10],
-        "call": [2, 6, 8, 10],
-        "bound": [2, 7, 8, 10],
-        "It": [2, 6, 8, 10],
-        "respons": [2, 8, 10],
-        "modifi": [2, 8, 10],
-        "ischema_nam": [2, 8, 10],
-        "reflector": [2, 8, 10],
-        "alwai": [2, 8, 10],
-        "unknown": [2, 8, 10],
-        "check": [2, 5, 9],
-        "entri": [2, 9],
-        "doe": [2, 9],
-        "exist": [2, 9],
-        "bool": [2, 3, 5, 9, 10, 11],
-        "remov": [2, 7, 9],
-        "get": [2, 9],
-        "The": [2, 3, 5, 6, 9, 10, 11, 12, 14, 18],
-        "keyerror": [2, 9],
-        "found": [2, 9, 17],
-        "id": [2, 9, 18],
-        "statement": [2, 9],
-        "tupl": [2, 9, 10, 11],
-        "make": [2, 3, 5, 9, 10, 12],
-        "item": [2, 9],
-        "valu": [2, 9],
-        "set": [2, 9],
-        "could": [2, 9],
-        "some": [2, 9],
-        "conflict": [2, 9],
-        "ctype": [2, 3, 12],
-        "dialect_nam": [2, 12],
-        "sa": [2, 3, 5, 7, 10, 12],
-        "string": [2, 3, 5, 10, 11, 12],
-        "_warn": [2, 6],
-        "catch_warn": [2, 6],
-        "record": [2, 6],
-        "true": [2, 6, 10, 11],
-        "my": [2, 6],
-        "messag": [2, 6],
-        "assert": [2, 6],
-        "len": [2, 6],
-        "1": [2, 6],
-        "simplefilt": [2, 6],
-        "lalala": [2, 6],
-        "traceback": [2, 6],
-        "most": [2, 6],
-        "recent": [2, 6],
-        "last": [2, 6],
-        "stacklevel": [2, 6],
-        "veri": [2, 6],
-        "categori": [2, 6],
-        "method": [2, 6, 12],
-        "pure": [2, 6],
-        "conveni": [2, 6],
-        "save": [2, 6],
-        "unfriendli": [2, 6],
-        "syntax": [2, 6],
-        "int": [2, 6],
-        "number": [2, 6],
-        "stackfram": [2, 6],
-        "go": [2, 6],
-        "up": [2, 6],
-        "order": [2, 6, 18],
-        "place": [2, 6],
-        "helper": [2, 6, 14],
-        "alreadi": [2, 6],
-        "taken": [2, 6],
-        "account": [2, 6],
-        "gener": [3, 5, 6, 7, 14, 15, 16],
-        "2010": [3, 4, 5, 8, 9, 10, 11, 12, 14],
-        "nullabl": 3,
-        "primary_kei": 3,
-        "autoincr": 3,
-        "server_default": 3,
-        "unicod": 3,
-        "part": [3, 7, 14],
-        "primari": [3, 5, 14],
-        "kei": [3, 5, 10, 14, 18],
-        "possibl": 3,
-        "default": 3,
-        "claus": 3,
-        "other": 5,
-        "compar": 5,
-        "staticmethod": [5, 10],
-        "_cmp": 5,
-        "static": [5, 10, 15, 16],
-        "cl": [5, 10],
-        "factori": 5,
-        "shallow": 5,
-        "arg": [5, 11],
-        "keyword": [5, 11],
-        "short": 5,
-        "fals": [5, 10],
-        "all": [5, 6, 13],
-        "posit": [5, 11],
-        "argument": [5, 11, 14],
-        "specifi": 5,
-        "e": [5, 9, 18],
-        "one": [5, 17],
-        "onli": 5,
-        "appli": 5,
-        "too": 5,
-        "mani": 5,
-        "fk": 5,
-        "pk": 5,
-        "uk": 5,
-        "col": 5,
-        "access": 5,
-        "via": 5,
-        "provid": 6,
-        "throughout": 6,
-        "packag": [6, 15, 16, 17],
-        "schema": [7, 10, 14, 15, 16],
-        "code": [7, 8],
-        "bind": 7,
-        "proxi": 7,
-        "our": 7,
-        "api": [7, 17],
-        "sqlalchemi": [8, 10, 15, 16],
-        "over": 9,
-        "import_": 9,
-        "support": [9, 17],
-        "class_": 9,
-        "match": 9,
-        "type_": 9,
-        "load": 9,
-        "dot": 9,
-        "stolen": 9,
-        "wtf": 9,
-        "server": 9,
-        "can": [9, 18],
-        "anyth": 9,
-        "passiv": 9,
-        "invoc": 9,
-        "like": [9, 18],
-        "importerror": 9,
-        "A": 9,
-        "path": 9,
-        "variabl": 10,
-        "might": 10,
-        "actual": 10,
-        "possibli": 10,
-        "qualifi": 10,
-        "v": 10,
-        "referenc": 10,
-        "find": [10, 12, 17],
-        "foreign": [10, 14],
-        "cycl": 10,
-        "break": 10,
-        "them": 10,
-        "apart": 10,
-        "dedent": 11,
-        "rstrip": 11,
-        "automat": 11,
-        "kwarg": [11, 14],
-        "given": 11,
-        "both": 11,
-        "noth": 11,
-        "typeerror": 11,
-        "first_cl": 12,
-        "where": [12, 14],
-        "start": [12, 13],
-        "andrxe9": 13,
-        "b": 13,
-        "space": 13,
-        "determin": 13,
-        "public": 13,
-        "__all__": 13,
-        "sequenc": [13, 14],
-        "otherwis": 13,
-        "underscor": 13,
-        "These": 14,
-        "need": [14, 17],
-        "locat": 14,
-        "configur": 14,
-        "refcolumn": 14,
-        "append": 14,
-        "addit": 14,
-        "submodul": [15, 16],
-        "modul": [15, 16],
-        "content": [15, 16],
-        "python": 17,
-        "7": [17, 18],
-        "3": 17,
-        "6": [17, 18],
-        "abov": 17,
-        "search": 17,
-        "javascript": 17,
-        "writem": 17,
-        "beta": 17,
-        "term": 17,
-        "ll": 17,
-        "detail": 17,
-        "root": 17,
-        "directori": 17,
-        "onlin": 17,
-        "No": 17,
-        "cours": 17,
-        "But": 17,
-        "ve": 17,
-        "have": 17,
-        "idea": 17,
-        "how": 17,
-        "improv": 17,
-        "feel": 17,
-        "free": 17,
-        "send": 17,
-        "pull": 17,
-        "request": 17,
-        "github": 17,
-        "mail": 17,
-        "perlig": [17, 18],
-        "de": [17, 18],
-        "wa": 17,
-        "written": 17,
-        "maintain": 17,
-        "tar": 18,
-        "xz": 18,
-        "bz2": 18,
-        "gz": 18,
-        "zip": 18,
-        "digest": 18,
-        "There": 18,
-        "hash": 18,
-        "md5": 18,
-        "sha1": 18,
-        "sha256": 18,
-        "store": 18,
-        "In": 18,
-        "tool": 18,
-        "md5sum": 18,
-        "sha1sum": 18,
-        "sha256sum": 18,
-        "accordingli": 18,
-        "g": 18,
-        "c": 18,
-        "ok": 18,
-        "itself": 18,
-        "pgp": 18,
-        "signatur": 18,
-        "sign": 18,
-        "0x029c942244325167": 18,
-        "gpg": 18,
-        "verifi": 18,
-        "made": 18,
-        "fri": 18,
-        "20": 18,
-        "10": 18,
-        "03": 18,
-        "36": 18,
-        "2022": 18,
-        "cest": 18,
-        "rsa": 18,
-        "21b65583ff640d34e8662b6b3ded446369f2ee1a": 18,
-        "good": 18,
-        "nd": 18
+        "_column": [0, 13, 14],
+        "column": [0, 3, 10, 12, 13, 14],
+        "inspect": [0, 11, 13, 14],
+        "represent": [0, 13, 14],
+        "_name": [0, 1],
+        "_ctype": [0, 1, 10, 13, 14],
+        "_nullabl": [0, 1],
+        "_primary_kei": [0, 1],
+        "_autoincr": [0, 1],
+        "_server_default": [0, 1],
+        "_symbol": [0, 1, 3, 6, 8, 10, 13, 14],
+        "__dict__": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10, 13, 14],
+        "__init__": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10, 13, 14],
+        "__module__": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 13, 14],
+        "__repr__": [0, 1, 3, 8, 10, 13, 14],
+        "__weakref__": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 13, 14],
+        "from_sa": [0, 1],
+        "serverdefault": [0, 1, 13, 14],
+        "_default": [0, 1],
+        "_config": [0, 13, 14],
+        "config": [0, 13, 14],
+        "manag": [0, 13, 14],
+        "tabl": [0, 1, 2, 3, 6, 7, 10, 13, 14],
+        "_line": [0, 2, 13, 14],
+        "_config_tpl": [0, 2, 13, 14],
+        "__annotations__": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 13, 14],
+        "dump": [0, 2, 6, 13, 14],
+        "from_fil": [0, 2, 13, 14],
+        "from_lin": [0, 2, 13, 14],
+        "from_pars": [0, 2, 13, 14],
+        "_constraint": [0, 13, 14],
+        "constraint": [0, 8, 13, 14],
+        "_import": [0, 3, 7, 13, 14],
+        "__cmp__": [0, 3],
+        "__lt__": [0, 3],
+        "__new__": [0, 3, 8],
+        "copi": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "repr": [0, 3],
+        "foreignkeyconstraint": [0, 3, 13, 14],
+        "primarykeyconstraint": [0, 3, 13, 14],
+        "uniqueconstraint": [0, 3, 13, 14],
+        "access_col": [0, 3, 13, 14],
+        "_except": [0, 13, 14],
+        "except": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
+        "error": [0, 2, 4, 7, 13, 14],
+        "warn": [0, 4, 13, 14],
+        "emit": [0, 4, 6, 13, 14],
+        "_meta": [0, 13, 14],
+        "metadata": [0, 6, 8, 13, 14],
+        "boundmetadata": [0, 5, 13, 14],
+        "__getattr__": [0, 5],
+        "_schema": [0, 13, 14],
+        "_dialect": [0, 6, 10, 13, 14],
+        "_tabl": [0, 6, 13, 14],
+        "_dbname": [0, 6, 13, 14],
+        "_module_tpl": [0, 6, 13, 14],
+        "symbol": [0, 1, 3, 6, 8, 10, 11, 13, 14],
+        "symbolexcept": [0, 7, 13, 14],
+        "import": [0, 3, 4, 6, 7, 8, 13, 14],
+        "type": [0, 1, 2, 3, 6, 7, 8, 9, 11, 13, 14],
+        "__contains__": [0, 7, 13, 14],
+        "__delitem__": [0, 7, 13, 14],
+        "__getitem__": [0, 7, 13, 14],
+        "__iter__": [0, 7, 13, 14],
+        "__setitem__": [0, 7, 13, 14],
+        "_type": [0, 7, 13, 14],
+        "resolv": [0, 6, 7, 8],
+        "_load_dot": [0, 7, 13, 14],
+        "varnam": [0, 3, 8],
+        "sa_tabl": [0, 8],
+        "by_nam": [0, 8],
+        "is_refer": [0, 8],
+        "tablecollect": [0, 6, 8, 13, 14],
+        "tablerefer": [0, 8, 13, 14],
+        "_break_cycl": [0, 8, 13, 14],
+        "_templat": [0, 2, 6, 13, 14],
+        "simpl": [0, 13, 14],
+        "templat": [0, 2, 6, 13, 14],
+        "abstract": [0, 13, 14],
+        "expand": [0, 9],
+        "by_column": [0, 10, 13, 14],
+        "_add_postgres_enum": [0, 10, 13, 14],
+        "_finalize_typ": [0, 10, 13, 14],
+        "_find_class": [0, 10, 13, 14],
+        "_util": [0, 13, 14],
+        "misc": [0, 13, 14],
+        "util": [0, 13, 14],
+        "cmp": [0, 11, 13, 14],
+        "find_publ": [0, 11, 13, 14],
+        "declar": [0, 13, 14],
+        "foreignkei": [0, 3, 12, 13, 14],
+        "primarykei": [0, 3, 12, 13, 14],
+        "uniqu": [0, 3, 7, 12, 13, 14],
+        "copyright": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "2014": [0, 4, 11],
+        "2023": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "andr\u00e9": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 15, 16],
+        "malo": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
+        "hi": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "licensor": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "applic": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "licens": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "under": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "apach": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "version": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "2": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "0": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
+        "you": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
+        "mai": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 16],
+        "us": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 16],
+        "thi": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "file": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 16],
+        "complianc": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "obtain": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "http": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "www": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "org": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "unless": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "requir": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "law": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "agre": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "write": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "softwar": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "distribut": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "i": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16],
+        "an": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "AS": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "basi": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "without": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "warranti": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "OR": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "condit": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "OF": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "ani": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "kind": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "either": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "express": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "impli": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "see": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "specif": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "languag": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "govern": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "permiss": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "limit": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "definit": [0, 10],
+        "": [0, 3, 5, 6, 7, 8],
+        "capabl": 0,
+        "class": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10],
+        "line": [0, 2, 3],
+        "none": [0, 2, 3, 6, 7, 8, 10],
+        "sourc": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15],
+        "contain": [0, 1, 2, 6, 7, 8, 9, 10, 11],
+        "list": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+        "alien": [0, 2],
+        "map": [0, 2, 6, 7, 8],
+        "dict": [0, 2, 3, 6, 7, 8, 9, 11],
+        "origin": [0, 2],
+        "object": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+        "empti": [0, 2, 7],
+        "mappingproxi": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10],
+        "__doc__": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10],
+        "n": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10],
+        "attribut": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10],
+        "function": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12],
+        "classmethod": [0, 1, 2, 4, 8, 10],
+        "initi": [0, 1, 2, 3, 6, 7, 8, 9, 10],
+        "paramet": [0, 1, 2, 3, 4, 6, 7, 8, 9, 10, 11, 12],
+        "iter": [0, 2, 3, 7, 8],
+        "If": [0, 2, 6, 7, 8, 9, 11],
+        "omit": [0, 2, 6, 7, 8],
+        "ar": [0, 2, 3, 11, 15, 16],
+        "avail": [0, 2, 7, 15],
+        "weak": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+        "refer": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12],
+        "defin": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12],
+        "fp": [0, 2, 6],
+        "stream": [0, 2],
+        "name_or_fil": [0, 2],
+        "construct": [0, 1, 2, 8, 10],
+        "from": [0, 1, 2, 3, 7, 16],
+        "str": [0, 1, 2, 3, 4, 6, 7, 8, 9, 10],
+        "filenam": [0, 2],
+        "pointer": [0, 2],
+        "return": [0, 1, 2, 3, 7, 8, 9, 10, 11],
+        "new": [0, 1, 2, 8, 10],
+        "instanc": [0, 1, 2, 8, 10],
+        "rais": [0, 2, 7, 9],
+        "ioerror": [0, 2],
+        "read": [0, 2],
+        "enoent": [0, 2],
+        "which": [0, 2, 7],
+        "treat": [0, 2],
+        "creat": [0, 2, 3],
+        "parser": [0, 2],
+        "configpars": [0, 2],
+        "rawconfigpars": [0, 2],
+        "base": [0, 3, 4],
+        "conn": [0, 6],
+        "dbname": [0, 6],
+        "dialect": [0, 6, 7, 8, 10],
+        "name": [0, 1, 3, 5, 6, 7, 8, 10, 11],
+        "collect": [0, 6, 8],
+        "db": [0, 6],
+        "identifi": [0, 6, 7],
+        "connect": [0, 6],
+        "engin": [0, 6],
+        "reflect": [0, 3, 6, 8],
+        "local": [0, 6],
+        "pair": [0, 6],
+        "option": [0, 3, 6],
+        "inform": [0, 6],
+        "purpos": [0, 6],
+        "just": [0, 6],
+        "won": [0, 6],
+        "t": [0, 6],
+        "callabl": [0, 6, 8],
+        "extra": [0, 6, 8],
+        "loader": [0, 6, 8],
+        "fail": [0, 6, 8],
+        "becaus": [0, 6, 7, 8],
+        "cannot": [0, 6, 8],
+        "call": [0, 4, 6, 8],
+        "bound": [0, 5, 6, 8],
+        "It": [0, 4, 6, 8],
+        "respons": [0, 6, 8],
+        "modifi": [0, 6, 8],
+        "ischema_nam": [0, 6, 8],
+        "reflector": [0, 6, 8],
+        "alwai": [0, 6, 8],
+        "unknown": [0, 6, 8],
+        "check": [0, 3, 7],
+        "entri": [0, 7],
+        "doe": [0, 7],
+        "exist": [0, 7],
+        "bool": [0, 1, 3, 7, 8, 9],
+        "remov": [0, 5, 7],
+        "get": [0, 7],
+        "The": [0, 1, 3, 4, 7, 8, 9, 10, 12, 16],
+        "keyerror": [0, 7],
+        "found": [0, 7, 15],
+        "id": [0, 7, 16],
+        "statement": [0, 7],
+        "tupl": [0, 7, 8, 9],
+        "make": [0, 1, 3, 7, 8, 10],
+        "item": [0, 7],
+        "valu": [0, 7],
+        "set": [0, 7],
+        "could": [0, 7],
+        "some": [0, 7, 10],
+        "conflict": [0, 7],
+        "ctype": [0, 1, 10],
+        "dialect_nam": [0, 10],
+        "sa": [0, 1, 3, 5, 8, 10],
+        "string": [0, 1, 3, 8, 9, 10],
+        "_warn": [0, 4],
+        "catch_warn": [0, 4],
+        "record": [0, 4],
+        "true": [0, 4, 8, 9],
+        "my": [0, 4],
+        "messag": [0, 4],
+        "assert": [0, 4],
+        "len": [0, 4],
+        "1": [0, 4],
+        "simplefilt": [0, 4],
+        "lalala": [0, 4],
+        "traceback": [0, 4],
+        "most": [0, 4],
+        "recent": [0, 4],
+        "last": [0, 4],
+        "stacklevel": [0, 4],
+        "veri": [0, 4],
+        "categori": [0, 4],
+        "method": [0, 4, 10],
+        "pure": [0, 4],
+        "conveni": [0, 4],
+        "save": [0, 4],
+        "unfriendli": [0, 4],
+        "syntax": [0, 4],
+        "int": [0, 4],
+        "number": [0, 4],
+        "stackfram": [0, 4],
+        "go": [0, 4],
+        "up": [0, 4],
+        "order": [0, 4, 16],
+        "place": [0, 4],
+        "helper": [0, 4, 12],
+        "alreadi": [0, 4],
+        "taken": [0, 4],
+        "account": [0, 4],
+        "gener": [1, 3, 4, 5, 10, 12, 13, 14],
+        "2010": [1, 2, 3, 6, 7, 8, 9, 10, 12],
+        "nullabl": 1,
+        "primary_kei": 1,
+        "autoincr": 1,
+        "server_default": 1,
+        "unicod": 1,
+        "part": [1, 5, 12],
+        "primari": [1, 3, 12],
+        "kei": [1, 3, 8, 12, 16],
+        "possibl": 1,
+        "default": 1,
+        "claus": 1,
+        "other": 3,
+        "compar": 3,
+        "staticmethod": [3, 8],
+        "_cmp": 3,
+        "static": [3, 8, 13, 14],
+        "cl": [3, 8],
+        "factori": 3,
+        "shallow": 3,
+        "arg": [3, 9],
+        "keyword": [3, 9],
+        "short": 3,
+        "fals": [3, 8],
+        "all": [3, 4, 11],
+        "posit": [3, 9],
+        "argument": [3, 9, 12],
+        "specifi": 3,
+        "e": [3, 7, 16],
+        "one": [3, 15],
+        "onli": 3,
+        "appli": 3,
+        "too": 3,
+        "mani": 3,
+        "fk": 3,
+        "pk": 3,
+        "uk": 3,
+        "col": 3,
+        "access": 3,
+        "via": 3,
+        "provid": 4,
+        "throughout": 4,
+        "packag": [4, 13, 14, 15],
+        "schema": [5, 8, 12, 13, 14],
+        "code": [5, 6],
+        "bind": 5,
+        "proxi": 5,
+        "our": 5,
+        "api": [5, 15],
+        "sqlalchemi": [6, 8, 13, 14],
+        "over": 7,
+        "import_": 7,
+        "support": [7, 15],
+        "class_": 7,
+        "match": 7,
+        "type_": 7,
+        "load": 7,
+        "dot": 7,
+        "stolen": 7,
+        "wtf": 7,
+        "server": 7,
+        "can": [7, 16],
+        "anyth": 7,
+        "passiv": 7,
+        "invoc": 7,
+        "like": [7, 16],
+        "importerror": 7,
+        "A": 7,
+        "path": 7,
+        "variabl": 8,
+        "might": 8,
+        "actual": 8,
+        "possibli": 8,
+        "qualifi": 8,
+        "v": 8,
+        "referenc": 8,
+        "find": [8, 10, 15],
+        "foreign": [8, 12],
+        "cycl": 8,
+        "break": 8,
+        "them": 8,
+        "apart": 8,
+        "dedent": 9,
+        "rstrip": 9,
+        "automat": 9,
+        "kwarg": [9, 12],
+        "given": 9,
+        "both": 9,
+        "noth": 9,
+        "typeerror": 9,
+        "add": 10,
+        "postgr": 10,
+        "enum": 10,
+        "final": 10,
+        "modif": 10,
+        "todo": 10,
+        "should": 10,
+        "point": 10,
+        "futur": 10,
+        "first_cl": 10,
+        "where": [10, 12],
+        "start": [10, 11],
+        "andrxe9": 11,
+        "b": 11,
+        "space": 11,
+        "determin": 11,
+        "public": 11,
+        "__all__": 11,
+        "sequenc": [11, 12],
+        "otherwis": 11,
+        "underscor": 11,
+        "These": 12,
+        "need": [12, 15],
+        "locat": 12,
+        "configur": 12,
+        "refcolumn": 12,
+        "append": 12,
+        "addit": 12,
+        "submodul": [13, 14],
+        "modul": [13, 14],
+        "content": [13, 14],
+        "python": 15,
+        "7": 15,
+        "3": 15,
+        "6": [15, 16],
+        "abov": 15,
+        "search": 15,
+        "javascript": 15,
+        "writem": 15,
+        "beta": 15,
+        "term": 15,
+        "ll": 15,
+        "detail": 15,
+        "root": 15,
+        "directori": 15,
+        "onlin": 15,
+        "No": 15,
+        "cours": 15,
+        "But": 15,
+        "ve": 15,
+        "have": 15,
+        "idea": 15,
+        "how": 15,
+        "improv": 15,
+        "feel": 15,
+        "free": 15,
+        "send": 15,
+        "pull": 15,
+        "request": 15,
+        "github": 15,
+        "mail": 15,
+        "perlig": [15, 16],
+        "de": [15, 16],
+        "wa": 15,
+        "written": 15,
+        "maintain": 15,
+        "gensaschema": 16,
+        "8": 16,
+        "tar": 16,
+        "xz": 16,
+        "bz2": 16,
+        "gz": 16,
+        "zip": 16,
+        "digest": 16,
+        "There": 16,
+        "hash": 16,
+        "md5": 16,
+        "sha1": 16,
+        "sha256": 16,
+        "store": 16,
+        "In": 16,
+        "tool": 16,
+        "md5sum": 16,
+        "sha1sum": 16,
+        "sha256sum": 16,
+        "accordingli": 16,
+        "g": 16,
+        "c": 16,
+        "ok": 16,
+        "itself": 16,
+        "pgp": 16,
+        "signatur": 16,
+        "sign": 16,
+        "0x029c942244325167": 16,
+        "gpg": 16,
+        "verifi": 16,
+        "made": 16,
+        "fri": 16,
+        "20": 16,
+        "10": 16,
+        "03": 16,
+        "36": 16,
+        "2022": 16,
+        "cest": 16,
+        "rsa": 16,
+        "21b65583ff640d34e8662b6b3ded446369f2ee1a": 16,
+        "good": 16,
+        "nd": 16
     },
     "objects": {
         "": [
-            [2, 0, 0, "-", "gensaschema"]
+            [0, 0, 0, "-", "gensaschema"]
         ],
         "gensaschema": [
-            [2, 1, 1, "", "Config"],
-            [2, 4, 1, "", "Error"],
-            [2, 1, 1, "", "Schema"],
-            [2, 4, 1, "", "SymbolException"],
-            [2, 1, 1, "", "Symbols"],
-            [2, 1, 1, "", "Type"],
-            [2, 4, 1, "", "Warning"],
-            [3, 0, 0, "-", "_column"],
-            [4, 0, 0, "-", "_config"],
-            [5, 0, 0, "-", "_constraint"],
-            [6, 0, 0, "-", "_exceptions"],
-            [7, 0, 0, "-", "_meta"],
-            [8, 0, 0, "-", "_schema"],
-            [9, 0, 0, "-", "_symbols"],
-            [10, 0, 0, "-", "_table"],
-            [11, 0, 0, "-", "_template"],
-            [12, 0, 0, "-", "_type"],
-            [13, 0, 0, "-", "_util"],
-            [14, 0, 0, "-", "constraints"]
+            [0, 1, 1, "", "Config"],
+            [0, 4, 1, "", "Error"],
+            [0, 1, 1, "", "Schema"],
+            [0, 4, 1, "", "SymbolException"],
+            [0, 1, 1, "", "Symbols"],
+            [0, 1, 1, "", "Type"],
+            [0, 4, 1, "", "Warning"],
+            [1, 0, 0, "-", "_column"],
+            [2, 0, 0, "-", "_config"],
+            [3, 0, 0, "-", "_constraint"],
+            [4, 0, 0, "-", "_exceptions"],
+            [5, 0, 0, "-", "_meta"],
+            [6, 0, 0, "-", "_schema"],
+            [7, 0, 0, "-", "_symbols"],
+            [8, 0, 0, "-", "_table"],
+            [9, 0, 0, "-", "_template"],
+            [10, 0, 0, "-", "_type"],
+            [11, 0, 0, "-", "_util"],
+            [12, 0, 0, "-", "constraints"]
         ],
         "gensaschema.Config": [
-            [2, 2, 1, "", "_CONFIG_TPL"],
-            [2, 2, 1, "", "__dict__"],
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "__module__"],
-            [2, 2, 1, "", "__weakref__"],
-            [2, 2, 1, "", "_lines"],
-            [2, 3, 1, "", "dump"],
-            [2, 3, 1, "", "from_file"],
-            [2, 3, 1, "", "from_lines"],
-            [2, 3, 1, "", "from_parser"],
-            [2, 2, 1, "", "schemas"],
-            [2, 2, 1, "", "tables"]
+            [0, 2, 1, "", "_CONFIG_TPL"],
+            [0, 2, 1, "", "__dict__"],
+            [0, 3, 1, "", "__init__"],
+            [0, 2, 1, "", "__module__"],
+            [0, 2, 1, "", "__weakref__"],
+            [0, 2, 1, "", "_lines"],
+            [0, 3, 1, "", "dump"],
+            [0, 3, 1, "", "from_file"],
+            [0, 3, 1, "", "from_lines"],
+            [0, 3, 1, "", "from_parser"],
+            [0, 2, 1, "", "schemas"],
+            [0, 2, 1, "", "tables"]
         ],
         "gensaschema.Error": [
-            [2, 2, 1, "", "__module__"],
-            [2, 2, 1, "", "__weakref__"]
+            [0, 2, 1, "", "__module__"],
+            [0, 2, 1, "", "__weakref__"]
         ],
         "gensaschema.Schema": [
-            [2, 2, 1, "", "_MODULE_TPL"],
-            [2, 2, 1, "", "__dict__"],
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "__module__"],
-            [2, 2, 1, "", "__weakref__"],
-            [2, 2, 1, "", "_dbname"],
-            [2, 2, 1, "", "_dialect"],
-            [2, 2, 1, "", "_schemas"],
-            [2, 2, 1, "", "_symbols"],
-            [2, 2, 1, "", "_tables"],
-            [2, 3, 1, "", "dump"]
+            [0, 2, 1, "", "_MODULE_TPL"],
+            [0, 2, 1, "", "__dict__"],
+            [0, 3, 1, "", "__init__"],
+            [0, 2, 1, "", "__module__"],
+            [0, 2, 1, "", "__weakref__"],
+            [0, 2, 1, "", "_dbname"],
+            [0, 2, 1, "", "_dialect"],
+            [0, 2, 1, "", "_schemas"],
+            [0, 2, 1, "", "_symbols"],
+            [0, 2, 1, "", "_tables"],
+            [0, 3, 1, "", "dump"]
         ],
         "gensaschema.SymbolException": [
-            [2, 2, 1, "", "__annotations__"],
-            [2, 2, 1, "", "__module__"]
+            [0, 2, 1, "", "__annotations__"],
+            [0, 2, 1, "", "__module__"]
         ],
         "gensaschema.Symbols": [
-            [2, 3, 1, "", "__contains__"],
-            [2, 3, 1, "", "__delitem__"],
-            [2, 2, 1, "", "__dict__"],
-            [2, 3, 1, "", "__getitem__"],
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "__iter__"],
-            [2, 2, 1, "", "__module__"],
-            [2, 3, 1, "", "__setitem__"],
-            [2, 2, 1, "", "__weakref__"],
-            [2, 2, 1, "", "_symbols"],
-            [2, 2, 1, "", "imports"],
-            [2, 2, 1, "", "types"]
+            [0, 3, 1, "", "__contains__"],
+            [0, 3, 1, "", "__delitem__"],
+            [0, 2, 1, "", "__dict__"],
+            [0, 3, 1, "", "__getitem__"],
+            [0, 3, 1, "", "__init__"],
+            [0, 3, 1, "", "__iter__"],
+            [0, 2, 1, "", "__module__"],
+            [0, 3, 1, "", "__setitem__"],
+            [0, 2, 1, "", "__weakref__"],
+            [0, 2, 1, "", "_symbols"],
+            [0, 2, 1, "", "imports"],
+            [0, 2, 1, "", "types"]
         ],
         "gensaschema.Type": [
-            [2, 2, 1, "", "__dict__"],
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "__module__"],
-            [2, 3, 1, "", "__repr__"],
-            [2, 2, 1, "", "__weakref__"],
-            [2, 2, 1, "", "_ctype"],
-            [2, 2, 1, "", "_dialect"],
-            [2, 2, 1, "", "_symbols"],
-            [2, 3, 1, "", "by_column"]
+            [0, 2, 1, "", "__dict__"],
+            [0, 3, 1, "", "__init__"],
+            [0, 2, 1, "", "__module__"],
+            [0, 3, 1, "", "__repr__"],
+            [0, 2, 1, "", "__weakref__"],
+            [0, 2, 1, "", "_ctype"],
+            [0, 2, 1, "", "_dialect"],
+            [0, 2, 1, "", "_symbols"],
+            [0, 3, 1, "", "by_column"]
         ],
         "gensaschema.Warning": [
-            [2, 2, 1, "", "__module__"],
-            [2, 2, 1, "", "__weakref__"],
-            [2, 3, 1, "", "emit"]
+            [0, 2, 1, "", "__module__"],
+            [0, 2, 1, "", "__weakref__"],
+            [0, 3, 1, "", "emit"]
         ],
         "gensaschema._column": [
-            [3, 1, 1, "", "Column"],
-            [3, 1, 1, "", "ServerDefault"]
+            [1, 1, 1, "", "Column"],
+            [1, 1, 1, "", "ServerDefault"]
         ],
         "gensaschema._column.Column": [
-            [3, 2, 1, "", "__dict__"],
-            [3, 3, 1, "", "__init__"],
-            [3, 2, 1, "", "__module__"],
-            [3, 3, 1, "", "__repr__"],
-            [3, 2, 1, "", "__weakref__"],
-            [3, 2, 1, "", "_autoincrement"],
-            [3, 2, 1, "", "_ctype"],
-            [3, 2, 1, "", "_name"],
-            [3, 2, 1, "", "_nullable"],
-            [3, 2, 1, "", "_primary_key"],
-            [3, 2, 1, "", "_server_default"],
-            [3, 2, 1, "", "_symbols"],
-            [3, 3, 1, "", "from_sa"]
+            [1, 2, 1, "", "__dict__"],
+            [1, 3, 1, "", "__init__"],
+            [1, 2, 1, "", "__module__"],
+            [1, 3, 1, "", "__repr__"],
+            [1, 2, 1, "", "__weakref__"],
+            [1, 2, 1, "", "_autoincrement"],
+            [1, 2, 1, "", "_ctype"],
+            [1, 2, 1, "", "_name"],
+            [1, 2, 1, "", "_nullable"],
+            [1, 2, 1, "", "_primary_key"],
+            [1, 2, 1, "", "_server_default"],
+            [1, 2, 1, "", "_symbols"],
+            [1, 3, 1, "", "from_sa"]
         ],
         "gensaschema._column.ServerDefault": [
-            [3, 2, 1, "", "__dict__"],
-            [3, 3, 1, "", "__init__"],
-            [3, 2, 1, "", "__module__"],
-            [3, 3, 1, "", "__repr__"],
-            [3, 2, 1, "", "__weakref__"],
-            [3, 2, 1, "", "_default"],
-            [3, 2, 1, "", "_symbols"]
+            [1, 2, 1, "", "__dict__"],
+            [1, 3, 1, "", "__init__"],
+            [1, 2, 1, "", "__module__"],
+            [1, 3, 1, "", "__repr__"],
+            [1, 2, 1, "", "__weakref__"],
+            [1, 2, 1, "", "_default"],
+            [1, 2, 1, "", "_symbols"]
         ],
         "gensaschema._config": [
-            [4, 1, 1, "", "Config"]
+            [2, 1, 1, "", "Config"]
         ],
         "gensaschema._config.Config": [
-            [4, 2, 1, "", "_CONFIG_TPL"],
-            [4, 2, 1, "", "__annotations__"],
-            [4, 2, 1, "", "__dict__"],
-            [4, 3, 1, "", "__init__"],
-            [4, 2, 1, "", "__module__"],
-            [4, 2, 1, "", "__weakref__"],
-            [4, 2, 1, "", "_lines"],
-            [4, 3, 1, "", "dump"],
-            [4, 3, 1, "", "from_file"],
-            [4, 3, 1, "", "from_lines"],
-            [4, 3, 1, "", "from_parser"],
-            [4, 2, 1, "", "schemas"],
-            [4, 2, 1, "", "tables"]
+            [2, 2, 1, "", "_CONFIG_TPL"],
+            [2, 2, 1, "", "__annotations__"],
+            [2, 2, 1, "", "__dict__"],
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "__module__"],
+            [2, 2, 1, "", "__weakref__"],
+            [2, 2, 1, "", "_lines"],
+            [2, 3, 1, "", "dump"],
+            [2, 3, 1, "", "from_file"],
+            [2, 3, 1, "", "from_lines"],
+            [2, 3, 1, "", "from_parser"],
+            [2, 2, 1, "", "schemas"],
+            [2, 2, 1, "", "tables"]
         ],
         "gensaschema._constraint": [
-            [5, 1, 1, "", "Constraint"],
-            [5, 1, 1, "", "ForeignKeyConstraint"],
-            [5, 1, 1, "", "PrimaryKeyConstraint"],
-            [5, 1, 1, "", "UniqueConstraint"],
-            [5, 5, 1, "", "access_col"]
+            [3, 1, 1, "", "Constraint"],
+            [3, 1, 1, "", "ForeignKeyConstraint"],
+            [3, 1, 1, "", "PrimaryKeyConstraint"],
+            [3, 1, 1, "", "UniqueConstraint"],
+            [3, 5, 1, "", "access_col"]
         ],
         "gensaschema._constraint.Constraint": [
-            [5, 2, 1, "", "_IMPORT"],
-            [5, 2, 1, "", "_SYMBOL"],
-            [5, 3, 1, "", "__cmp__"],
-            [5, 2, 1, "", "__dict__"],
-            [5, 3, 1, "", "__init__"],
-            [5, 3, 1, "", "__lt__"],
-            [5, 2, 1, "", "__module__"],
-            [5, 3, 1, "", "__new__"],
-            [5, 2, 1, "", "__weakref__"],
-            [5, 2, 1, "", "constraint"],
-            [5, 3, 1, "", "copy"],
-            [5, 3, 1, "", "repr"]
+            [3, 2, 1, "", "_IMPORT"],
+            [3, 2, 1, "", "_SYMBOL"],
+            [3, 3, 1, "", "__cmp__"],
+            [3, 2, 1, "", "__dict__"],
+            [3, 3, 1, "", "__init__"],
+            [3, 3, 1, "", "__lt__"],
+            [3, 2, 1, "", "__module__"],
+            [3, 3, 1, "", "__new__"],
+            [3, 2, 1, "", "__weakref__"],
+            [3, 2, 1, "", "constraint"],
+            [3, 3, 1, "", "copy"],
+            [3, 3, 1, "", "repr"]
         ],
         "gensaschema._constraint.ForeignKeyConstraint": [
-            [5, 2, 1, "", "_IMPORT"],
-            [5, 2, 1, "", "_SYMBOL"],
-            [5, 2, 1, "", "__annotations__"],
-            [5, 2, 1, "", "__module__"],
-            [5, 3, 1, "", "__repr__"]
+            [3, 2, 1, "", "_IMPORT"],
+            [3, 2, 1, "", "_SYMBOL"],
+            [3, 2, 1, "", "__annotations__"],
+            [3, 2, 1, "", "__module__"],
+            [3, 3, 1, "", "__repr__"]
         ],
         "gensaschema._constraint.PrimaryKeyConstraint": [
-            [5, 2, 1, "", "_IMPORT"],
-            [5, 2, 1, "", "_SYMBOL"],
-            [5, 2, 1, "", "__annotations__"],
-            [5, 2, 1, "", "__module__"]
+            [3, 2, 1, "", "_IMPORT"],
+            [3, 2, 1, "", "_SYMBOL"],
+            [3, 2, 1, "", "__annotations__"],
+            [3, 2, 1, "", "__module__"]
         ],
         "gensaschema._constraint.UniqueConstraint": [
-            [5, 2, 1, "", "_IMPORT"],
-            [5, 2, 1, "", "_SYMBOL"],
-            [5, 2, 1, "", "__annotations__"],
-            [5, 2, 1, "", "__module__"],
-            [5, 3, 1, "", "__repr__"]
+            [3, 2, 1, "", "_IMPORT"],
+            [3, 2, 1, "", "_SYMBOL"],
+            [3, 2, 1, "", "__annotations__"],
+            [3, 2, 1, "", "__module__"],
+            [3, 3, 1, "", "__repr__"]
         ],
         "gensaschema._exceptions": [
-            [6, 4, 1, "", "Error"],
-            [6, 4, 1, "", "Warning"]
+            [4, 4, 1, "", "Error"],
+            [4, 4, 1, "", "Warning"]
         ],
         "gensaschema._exceptions.Error": [
-            [6, 2, 1, "", "__annotations__"],
-            [6, 2, 1, "", "__module__"],
-            [6, 2, 1, "", "__weakref__"]
+            [4, 2, 1, "", "__annotations__"],
+            [4, 2, 1, "", "__module__"],
+            [4, 2, 1, "", "__weakref__"]
         ],
         "gensaschema._exceptions.Warning": [
-            [6, 2, 1, "", "__annotations__"],
-            [6, 2, 1, "", "__module__"],
-            [6, 2, 1, "", "__weakref__"],
-            [6, 3, 1, "", "emit"]
+            [4, 2, 1, "", "__annotations__"],
+            [4, 2, 1, "", "__module__"],
+            [4, 2, 1, "", "__weakref__"],
+            [4, 3, 1, "", "emit"]
         ],
         "gensaschema._meta": [
-            [7, 1, 1, "", "BoundMetaData"]
+            [5, 1, 1, "", "BoundMetaData"]
         ],
         "gensaschema._meta.BoundMetaData": [
-            [7, 2, 1, "", "__dict__"],
-            [7, 3, 1, "", "__getattr__"],
-            [7, 3, 1, "", "__init__"],
-            [7, 2, 1, "", "__module__"],
-            [7, 2, 1, "", "__weakref__"]
+            [5, 2, 1, "", "__dict__"],
+            [5, 3, 1, "", "__getattr__"],
+            [5, 3, 1, "", "__init__"],
+            [5, 2, 1, "", "__module__"],
+            [5, 2, 1, "", "__weakref__"]
         ],
         "gensaschema._schema": [
-            [8, 1, 1, "", "Schema"]
+            [6, 1, 1, "", "Schema"]
         ],
         "gensaschema._schema.Schema": [
-            [8, 2, 1, "", "_MODULE_TPL"],
-            [8, 2, 1, "", "__annotations__"],
-            [8, 2, 1, "", "__dict__"],
-            [8, 3, 1, "", "__init__"],
-            [8, 2, 1, "", "__module__"],
-            [8, 2, 1, "", "__weakref__"],
-            [8, 2, 1, "", "_dbname"],
-            [8, 2, 1, "", "_dialect"],
-            [8, 2, 1, "", "_schemas"],
-            [8, 2, 1, "", "_symbols"],
-            [8, 2, 1, "", "_tables"],
-            [8, 3, 1, "", "dump"]
+            [6, 2, 1, "", "_MODULE_TPL"],
+            [6, 2, 1, "", "__annotations__"],
+            [6, 2, 1, "", "__dict__"],
+            [6, 3, 1, "", "__init__"],
+            [6, 2, 1, "", "__module__"],
+            [6, 2, 1, "", "__weakref__"],
+            [6, 2, 1, "", "_dbname"],
+            [6, 2, 1, "", "_dialect"],
+            [6, 2, 1, "", "_schemas"],
+            [6, 2, 1, "", "_symbols"],
+            [6, 2, 1, "", "_tables"],
+            [6, 3, 1, "", "dump"]
         ],
         "gensaschema._symbols": [
-            [9, 4, 1, "", "SymbolException"],
-            [9, 1, 1, "", "Symbols"],
-            [9, 1, 1, "", "_Imports"],
-            [9, 1, 1, "", "_Types"],
-            [9, 5, 1, "", "_load_dotted"]
+            [7, 4, 1, "", "SymbolException"],
+            [7, 1, 1, "", "Symbols"],
+            [7, 1, 1, "", "_Imports"],
+            [7, 1, 1, "", "_Types"],
+            [7, 5, 1, "", "_load_dotted"]
         ],
         "gensaschema._symbols.SymbolException": [
-            [9, 2, 1, "", "__annotations__"],
-            [9, 2, 1, "", "__module__"]
+            [7, 2, 1, "", "__annotations__"],
+            [7, 2, 1, "", "__module__"]
         ],
         "gensaschema._symbols.Symbols": [
-            [9, 2, 1, "", "__annotations__"],
-            [9, 3, 1, "", "__contains__"],
-            [9, 3, 1, "", "__delitem__"],
-            [9, 2, 1, "", "__dict__"],
-            [9, 3, 1, "", "__getitem__"],
-            [9, 3, 1, "", "__init__"],
-            [9, 3, 1, "", "__iter__"],
-            [9, 2, 1, "", "__module__"],
-            [9, 3, 1, "", "__setitem__"],
-            [9, 2, 1, "", "__weakref__"],
-            [9, 2, 1, "", "_symbols"],
-            [9, 2, 1, "", "imports"],
-            [9, 2, 1, "", "types"]
+            [7, 2, 1, "", "__annotations__"],
+            [7, 3, 1, "", "__contains__"],
+            [7, 3, 1, "", "__delitem__"],
+            [7, 2, 1, "", "__dict__"],
+            [7, 3, 1, "", "__getitem__"],
+            [7, 3, 1, "", "__init__"],
+            [7, 3, 1, "", "__iter__"],
+            [7, 2, 1, "", "__module__"],
+            [7, 3, 1, "", "__setitem__"],
+            [7, 2, 1, "", "__weakref__"],
+            [7, 2, 1, "", "_symbols"],
+            [7, 2, 1, "", "imports"],
+            [7, 2, 1, "", "types"]
         ],
         "gensaschema._symbols._Imports": [
-            [9, 3, 1, "", "__contains__"],
-            [9, 2, 1, "", "__dict__"],
-            [9, 3, 1, "", "__init__"],
-            [9, 3, 1, "", "__iter__"],
-            [9, 2, 1, "", "__module__"],
-            [9, 3, 1, "", "__setitem__"],
-            [9, 2, 1, "", "__weakref__"],
-            [9, 2, 1, "", "_imports"]
+            [7, 3, 1, "", "__contains__"],
+            [7, 2, 1, "", "__dict__"],
+            [7, 3, 1, "", "__init__"],
+            [7, 3, 1, "", "__iter__"],
+            [7, 2, 1, "", "__module__"],
+            [7, 3, 1, "", "__setitem__"],
+            [7, 2, 1, "", "__weakref__"],
+            [7, 2, 1, "", "_imports"]
         ],
         "gensaschema._symbols._Types": [
-            [9, 2, 1, "", "__dict__"],
-            [9, 3, 1, "", "__init__"],
-            [9, 2, 1, "", "__module__"],
-            [9, 3, 1, "", "__setitem__"],
-            [9, 2, 1, "", "__weakref__"],
-            [9, 2, 1, "", "_symbols"],
-            [9, 2, 1, "", "_types"],
-            [9, 3, 1, "", "resolve"]
+            [7, 2, 1, "", "__dict__"],
+            [7, 3, 1, "", "__init__"],
+            [7, 2, 1, "", "__module__"],
+            [7, 3, 1, "", "__setitem__"],
+            [7, 2, 1, "", "__weakref__"],
+            [7, 2, 1, "", "_symbols"],
+            [7, 2, 1, "", "_types"],
+            [7, 3, 1, "", "resolve"]
         ],
         "gensaschema._table": [
-            [10, 1, 1, "", "Table"],
-            [10, 1, 1, "", "TableCollection"],
-            [10, 1, 1, "", "TableReference"],
-            [10, 5, 1, "", "_break_cycles"]
+            [8, 1, 1, "", "Table"],
+            [8, 1, 1, "", "TableCollection"],
+            [8, 1, 1, "", "TableReference"],
+            [8, 5, 1, "", "_break_cycles"]
         ],
         "gensaschema._table.Table": [
-            [10, 2, 1, "", "__dict__"],
-            [10, 3, 1, "", "__init__"],
-            [10, 2, 1, "", "__module__"],
-            [10, 3, 1, "", "__new__"],
-            [10, 3, 1, "", "__repr__"],
-            [10, 2, 1, "", "__weakref__"],
-            [10, 2, 1, "", "_symbols"],
-            [10, 3, 1, "", "by_name"],
-            [10, 2, 1, "", "constraints"],
-            [10, 2, 1, "", "is_reference"],
-            [10, 2, 1, "", "sa_table"],
-            [10, 2, 1, "", "varname"]
+            [8, 2, 1, "", "__dict__"],
+            [8, 3, 1, "", "__init__"],
+            [8, 2, 1, "", "__module__"],
+            [8, 3, 1, "", "__new__"],
+            [8, 3, 1, "", "__repr__"],
+            [8, 2, 1, "", "__weakref__"],
+            [8, 2, 1, "", "_symbols"],
+            [8, 3, 1, "", "by_name"],
+            [8, 2, 1, "", "constraints"],
+            [8, 2, 1, "", "is_reference"],
+            [8, 2, 1, "", "sa_table"],
+            [8, 2, 1, "", "varname"]
         ],
         "gensaschema._table.TableCollection": [
-            [10, 2, 1, "", "__dict__"],
-            [10, 2, 1, "", "__module__"],
-            [10, 3, 1, "", "by_names"]
+            [8, 2, 1, "", "__dict__"],
+            [8, 2, 1, "", "__module__"],
+            [8, 3, 1, "", "by_names"]
         ],
         "gensaschema._table.TableReference": [
-            [10, 2, 1, "", "__dict__"],
-            [10, 3, 1, "", "__init__"],
-            [10, 2, 1, "", "__module__"],
-            [10, 2, 1, "", "__weakref__"],
-            [10, 2, 1, "", "constraints"],
-            [10, 2, 1, "", "is_reference"],
-            [10, 2, 1, "", "sa_table"],
-            [10, 2, 1, "", "varname"]
+            [8, 2, 1, "", "__dict__"],
+            [8, 3, 1, "", "__init__"],
+            [8, 2, 1, "", "__module__"],
+            [8, 2, 1, "", "__weakref__"],
+            [8, 2, 1, "", "constraints"],
+            [8, 2, 1, "", "is_reference"],
+            [8, 2, 1, "", "sa_table"],
+            [8, 2, 1, "", "varname"]
         ],
         "gensaschema._template": [
-            [11, 1, 1, "", "Template"]
+            [9, 1, 1, "", "Template"]
         ],
         "gensaschema._template.Template": [
-            [11, 2, 1, "", "__dict__"],
-            [11, 3, 1, "", "__init__"],
-            [11, 2, 1, "", "__module__"],
-            [11, 2, 1, "", "__weakref__"],
-            [11, 2, 1, "", "_template"],
-            [11, 3, 1, "", "expand"]
+            [9, 2, 1, "", "__dict__"],
+            [9, 3, 1, "", "__init__"],
+            [9, 2, 1, "", "__module__"],
+            [9, 2, 1, "", "__weakref__"],
+            [9, 2, 1, "", "_template"],
+            [9, 3, 1, "", "expand"]
         ],
         "gensaschema._type": [
-            [12, 1, 1, "", "Type"],
-            [12, 5, 1, "", "_find_class"]
+            [10, 1, 1, "", "Type"],
+            [10, 5, 1, "", "_add_postgres_enum"],
+            [10, 5, 1, "", "_finalize_type"],
+            [10, 5, 1, "", "_find_class"]
         ],
         "gensaschema._type.Type": [
-            [12, 2, 1, "", "__annotations__"],
-            [12, 2, 1, "", "__dict__"],
-            [12, 3, 1, "", "__init__"],
-            [12, 2, 1, "", "__module__"],
-            [12, 3, 1, "", "__repr__"],
-            [12, 2, 1, "", "__weakref__"],
-            [12, 2, 1, "", "_ctype"],
-            [12, 2, 1, "", "_dialect"],
-            [12, 2, 1, "", "_symbols"],
-            [12, 3, 1, "", "by_column"]
+            [10, 2, 1, "", "__annotations__"],
+            [10, 2, 1, "", "__dict__"],
+            [10, 3, 1, "", "__init__"],
+            [10, 2, 1, "", "__module__"],
+            [10, 3, 1, "", "__repr__"],
+            [10, 2, 1, "", "__weakref__"],
+            [10, 2, 1, "", "_ctype"],
+            [10, 2, 1, "", "_dialect"],
+            [10, 2, 1, "", "_symbols"],
+            [10, 3, 1, "", "by_column"]
         ],
         "gensaschema._util": [
-            [13, 5, 1, "", "cmp"],
-            [13, 5, 1, "", "find_public"]
+            [11, 5, 1, "", "cmp"],
+            [11, 5, 1, "", "find_public"]
         ],
         "gensaschema.constraints": [
-            [14, 5, 1, "", "ForeignKey"],
-            [14, 5, 1, "", "PrimaryKey"],
-            [14, 5, 1, "", "Unique"]
+            [12, 5, 1, "", "ForeignKey"],
+            [12, 5, 1, "", "PrimaryKey"],
+            [12, 5, 1, "", "Unique"]
         ]
     },
     "objtypes": {
         "0": "py:module",
         "1": "py:class",
         "2": "py:attribute",
         "3": "py:method",
@@ -831,73 +844,71 @@
         "1": ["py", "class", "Python class"],
         "2": ["py", "attribute", "Python attribute"],
         "3": ["py", "method", "Python method"],
         "4": ["py", "exception", "Python exception"],
         "5": ["py", "function", "Python function"]
     },
     "titleterms": {
-        "cdbx": [0, 1],
-        "packag": [0, 2, 18],
-        "submodul": [0, 2],
-        "modul": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
-        "content": [0, 2],
-        "_cdb": 1,
-        "gensaschema": [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17],
-        "static": [2, 17],
-        "sqlalchemi": [2, 17],
-        "schema": [2, 4, 8, 17],
-        "gener": [2, 8, 17],
-        "_column": 3,
-        "column": 3,
-        "inspect": [3, 5, 10, 12],
-        "represent": [3, 5, 10, 12],
-        "_config": 4,
-        "config": 4,
-        "manag": [4, 9],
-        "_constraint": 5,
-        "constraint": [5, 14],
-        "_except": 6,
-        "except": 6,
-        "_meta": 7,
-        "metadata": 7,
-        "_schema": 8,
-        "_symbol": 9,
-        "symbol": 9,
-        "_tabl": 10,
-        "tabl": 10,
-        "_templat": 11,
-        "simpl": 11,
-        "templat": 11,
-        "abstract": 11,
-        "_type": 12,
-        "type": 12,
-        "_util": 13,
-        "misc": 13,
-        "util": 13,
-        "declar": 14,
-        "document": 17,
-        "rational": 17,
-        "advocaci": 17,
-        "kei": 17,
-        "featur": 17,
-        "develop": 17,
-        "statu": 17,
-        "licens": 17,
-        "bug": 17,
-        "author": 17,
-        "inform": 17,
-        "download": 18,
-        "chang": 18,
-        "log": 18,
-        "sourc": 18,
-        "current": 18,
-        "stabl": 18,
-        "version": 18,
-        "integr": 18,
-        "check": 18
+        "gensaschema": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15],
+        "packag": [0, 16],
+        "submodul": 0,
+        "modul": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+        "content": 0,
+        "static": [0, 15],
+        "sqlalchemi": [0, 15],
+        "schema": [0, 2, 6, 15],
+        "gener": [0, 6, 15],
+        "_column": 1,
+        "column": 1,
+        "inspect": [1, 3, 8, 10],
+        "represent": [1, 3, 8, 10],
+        "_config": 2,
+        "config": 2,
+        "manag": [2, 7],
+        "_constraint": 3,
+        "constraint": [3, 12],
+        "_except": 4,
+        "except": 4,
+        "_meta": 5,
+        "metadata": 5,
+        "_schema": 6,
+        "_symbol": 7,
+        "symbol": 7,
+        "_tabl": 8,
+        "tabl": 8,
+        "_templat": 9,
+        "simpl": 9,
+        "templat": 9,
+        "abstract": 9,
+        "_type": 10,
+        "type": 10,
+        "_util": 11,
+        "misc": 11,
+        "util": 11,
+        "declar": 12,
+        "document": 15,
+        "rational": 15,
+        "advocaci": 15,
+        "kei": 15,
+        "featur": 15,
+        "develop": 15,
+        "statu": 15,
+        "licens": 15,
+        "bug": 15,
+        "author": 15,
+        "inform": 15,
+        "download": 16,
+        "chang": 16,
+        "log": 16,
+        "sourc": 16,
+        "current": 16,
+        "stabl": 16,
+        "version": 16,
+        "integr": 16,
+        "check": 16
     },
     "envversion": {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 8,
         "sphinx.domains.index": 1,
@@ -907,908 +918,906 @@
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx.ext.viewcode": 1,
         "sphinx": 57
     },
     "alltitles": {
         "gensaschema package": [
-            [2, "gensaschema-package"]
+            [0, "gensaschema-package"]
         ],
         "Submodules": [
-            [2, "submodules"],
             [0, "submodules"]
         ],
         "Module contents": [
-            [2, "module-gensaschema"],
-            [0, "module-contents"]
+            [0, "module-gensaschema"]
         ],
         "GenSASchema - Static SQLAlchemy Schema Generator": [
-            [2, "gensaschema-static-sqlalchemy-schema-generator"],
-            [17, "gensaschema-static-sqlalchemy-schema-generator"]
+            [0, "gensaschema-static-sqlalchemy-schema-generator"],
+            [15, "gensaschema-static-sqlalchemy-schema-generator"]
         ],
         "gensaschema._column module": [
-            [3, "module-gensaschema._column"]
+            [1, "module-gensaschema._column"]
         ],
         "Column inspection and representation": [
-            [3, "column-inspection-and-representation"]
+            [1, "column-inspection-and-representation"]
         ],
         "gensaschema._config module": [
-            [4, "module-gensaschema._config"]
+            [2, "module-gensaschema._config"]
         ],
         "Schema config management": [
-            [4, "schema-config-management"]
+            [2, "schema-config-management"]
         ],
         "gensaschema._constraint module": [
-            [5, "module-gensaschema._constraint"]
+            [3, "module-gensaschema._constraint"]
         ],
         "Constraint inspection and representation": [
-            [5, "constraint-inspection-and-representation"]
+            [3, "constraint-inspection-and-representation"]
         ],
         "gensaschema._exceptions module": [
-            [6, "module-gensaschema._exceptions"]
+            [4, "module-gensaschema._exceptions"]
         ],
         "GenSASchema Exceptions": [
-            [6, "gensaschema-exceptions"]
+            [4, "gensaschema-exceptions"]
         ],
         "gensaschema._meta module": [
-            [7, "module-gensaschema._meta"]
+            [5, "module-gensaschema._meta"]
         ],
         "Metadata": [
-            [7, "metadata"]
+            [5, "metadata"]
         ],
         "gensaschema._schema module": [
-            [8, "module-gensaschema._schema"]
+            [6, "module-gensaschema._schema"]
         ],
         "Schema module generation": [
-            [8, "schema-module-generation"]
+            [6, "schema-module-generation"]
         ],
         "gensaschema._symbols module": [
-            [9, "module-gensaschema._symbols"]
+            [7, "module-gensaschema._symbols"]
         ],
         "Symbol management": [
-            [9, "symbol-management"]
+            [7, "symbol-management"]
         ],
         "gensaschema._table module": [
-            [10, "module-gensaschema._table"]
+            [8, "module-gensaschema._table"]
         ],
         "Table inspection and representation": [
-            [10, "table-inspection-and-representation"]
+            [8, "table-inspection-and-representation"]
         ],
         "gensaschema._template module": [
-            [11, "module-gensaschema._template"]
+            [9, "module-gensaschema._template"]
         ],
         "Simple template abstraction": [
-            [11, "simple-template-abstraction"]
+            [9, "simple-template-abstraction"]
         ],
         "gensaschema._type module": [
-            [12, "module-gensaschema._type"]
+            [10, "module-gensaschema._type"]
         ],
         "Type inspection and representation": [
-            [12, "type-inspection-and-representation"]
+            [10, "type-inspection-and-representation"]
         ],
         "gensaschema._util module": [
-            [13, "module-gensaschema._util"]
+            [11, "module-gensaschema._util"]
         ],
         "Misc Utilities": [
-            [13, "misc-utilities"]
+            [11, "misc-utilities"]
         ],
         "gensaschema.constraints module": [
-            [14, "module-gensaschema.constraints"]
+            [12, "module-gensaschema.constraints"]
         ],
         "Constraint Declarators": [
-            [14, "constraint-declarators"]
+            [12, "constraint-declarators"]
         ],
         "gensaschema": [
-            [15, "gensaschema"],
-            [16, "gensaschema"]
+            [13, "gensaschema"],
+            [14, "gensaschema"]
         ],
         "Documentation": [
-            [17, "documentation"]
+            [15, "documentation"]
         ],
         "Rationale, Advocacy, Key Features": [
-            [17, "rationale-advocacy-key-features"]
+            [15, "rationale-advocacy-key-features"]
         ],
         "Development Status": [
-            [17, "development-status"]
+            [15, "development-status"]
         ],
         "License": [
-            [17, "license"]
+            [15, "license"]
         ],
         "Bugs": [
-            [17, "bugs"]
+            [15, "bugs"]
         ],
         "Author Information": [
-            [17, "author-information"]
+            [15, "author-information"]
         ],
         "Download": [
-            [18, "download"]
+            [16, "download"]
         ],
         "Change Log": [
-            [18, "change-log"]
+            [16, "change-log"]
         ],
         "Source Packages": [
-            [18, "source-packages"]
+            [16, "source-packages"]
         ],
         "Current Stable Version": [
-            [18, "current-stable-version"]
+            [16, "current-stable-version"]
         ],
         "Integrity Check": [
-            [18, "integrity-check"]
-        ],
-        "cdbx package": [
-            [0, "cdbx-package"]
-        ],
-        "cdbx._cdb module": [
-            [1, "cdbx-cdb-module"]
+            [16, "integrity-check"]
         ]
     },
     "indexentries": {
         "config (class in gensaschema)": [
-            [2, "gensaschema.Config"]
+            [0, "gensaschema.Config"]
         ],
         "error": [
-            [2, "gensaschema.Error"],
-            [6, "gensaschema._exceptions.Error"]
+            [0, "gensaschema.Error"],
+            [4, "gensaschema._exceptions.Error"]
         ],
         "schema (class in gensaschema)": [
-            [2, "gensaschema.Schema"]
+            [0, "gensaschema.Schema"]
         ],
         "symbolexception": [
-            [2, "gensaschema.SymbolException"],
-            [9, "gensaschema._symbols.SymbolException"]
+            [0, "gensaschema.SymbolException"],
+            [7, "gensaschema._symbols.SymbolException"]
         ],
         "symbols (class in gensaschema)": [
-            [2, "gensaschema.Symbols"]
+            [0, "gensaschema.Symbols"]
         ],
         "type (class in gensaschema)": [
-            [2, "gensaschema.Type"]
+            [0, "gensaschema.Type"]
         ],
         "warning": [
-            [2, "gensaschema.Warning"],
-            [6, "gensaschema._exceptions.Warning"]
+            [0, "gensaschema.Warning"],
+            [4, "gensaschema._exceptions.Warning"]
         ],
         "_config_tpl (gensaschema.config attribute)": [
-            [2, "gensaschema.Config._CONFIG_TPL"]
+            [0, "gensaschema.Config._CONFIG_TPL"]
         ],
         "_module_tpl (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema._MODULE_TPL"]
+            [0, "gensaschema.Schema._MODULE_TPL"]
         ],
         "__annotations__ (gensaschema.symbolexception attribute)": [
-            [2, "gensaschema.SymbolException.__annotations__"]
+            [0, "gensaschema.SymbolException.__annotations__"]
         ],
         "__contains__() (gensaschema.symbols method)": [
-            [2, "gensaschema.Symbols.__contains__"]
+            [0, "gensaschema.Symbols.__contains__"]
         ],
         "__delitem__() (gensaschema.symbols method)": [
-            [2, "gensaschema.Symbols.__delitem__"]
+            [0, "gensaschema.Symbols.__delitem__"]
         ],
         "__dict__ (gensaschema.config attribute)": [
-            [2, "gensaschema.Config.__dict__"]
+            [0, "gensaschema.Config.__dict__"]
         ],
         "__dict__ (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema.__dict__"]
+            [0, "gensaschema.Schema.__dict__"]
         ],
         "__dict__ (gensaschema.symbols attribute)": [
-            [2, "gensaschema.Symbols.__dict__"]
+            [0, "gensaschema.Symbols.__dict__"]
         ],
         "__dict__ (gensaschema.type attribute)": [
-            [2, "gensaschema.Type.__dict__"]
+            [0, "gensaschema.Type.__dict__"]
         ],
         "__getitem__() (gensaschema.symbols method)": [
-            [2, "gensaschema.Symbols.__getitem__"]
+            [0, "gensaschema.Symbols.__getitem__"]
         ],
         "__init__() (gensaschema.config method)": [
-            [2, "gensaschema.Config.__init__"]
+            [0, "gensaschema.Config.__init__"]
         ],
         "__init__() (gensaschema.schema method)": [
-            [2, "gensaschema.Schema.__init__"]
+            [0, "gensaschema.Schema.__init__"]
         ],
         "__init__() (gensaschema.symbols method)": [
-            [2, "gensaschema.Symbols.__init__"]
+            [0, "gensaschema.Symbols.__init__"]
         ],
         "__init__() (gensaschema.type method)": [
-            [2, "gensaschema.Type.__init__"]
+            [0, "gensaschema.Type.__init__"]
         ],
         "__iter__() (gensaschema.symbols method)": [
-            [2, "gensaschema.Symbols.__iter__"]
+            [0, "gensaschema.Symbols.__iter__"]
         ],
         "__module__ (gensaschema.config attribute)": [
-            [2, "gensaschema.Config.__module__"]
+            [0, "gensaschema.Config.__module__"]
         ],
         "__module__ (gensaschema.error attribute)": [
-            [2, "gensaschema.Error.__module__"]
+            [0, "gensaschema.Error.__module__"]
         ],
         "__module__ (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema.__module__"]
+            [0, "gensaschema.Schema.__module__"]
         ],
         "__module__ (gensaschema.symbolexception attribute)": [
-            [2, "gensaschema.SymbolException.__module__"]
+            [0, "gensaschema.SymbolException.__module__"]
         ],
         "__module__ (gensaschema.symbols attribute)": [
-            [2, "gensaschema.Symbols.__module__"]
+            [0, "gensaschema.Symbols.__module__"]
         ],
         "__module__ (gensaschema.type attribute)": [
-            [2, "gensaschema.Type.__module__"]
+            [0, "gensaschema.Type.__module__"]
         ],
         "__module__ (gensaschema.warning attribute)": [
-            [2, "gensaschema.Warning.__module__"]
+            [0, "gensaschema.Warning.__module__"]
         ],
         "__repr__() (gensaschema.type method)": [
-            [2, "gensaschema.Type.__repr__"]
+            [0, "gensaschema.Type.__repr__"]
         ],
         "__setitem__() (gensaschema.symbols method)": [
-            [2, "gensaschema.Symbols.__setitem__"]
+            [0, "gensaschema.Symbols.__setitem__"]
         ],
         "__weakref__ (gensaschema.config attribute)": [
-            [2, "gensaschema.Config.__weakref__"]
+            [0, "gensaschema.Config.__weakref__"]
         ],
         "__weakref__ (gensaschema.error attribute)": [
-            [2, "gensaschema.Error.__weakref__"]
+            [0, "gensaschema.Error.__weakref__"]
         ],
         "__weakref__ (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema.__weakref__"]
+            [0, "gensaschema.Schema.__weakref__"]
         ],
         "__weakref__ (gensaschema.symbols attribute)": [
-            [2, "gensaschema.Symbols.__weakref__"]
+            [0, "gensaschema.Symbols.__weakref__"]
         ],
         "__weakref__ (gensaschema.type attribute)": [
-            [2, "gensaschema.Type.__weakref__"]
+            [0, "gensaschema.Type.__weakref__"]
         ],
         "__weakref__ (gensaschema.warning attribute)": [
-            [2, "gensaschema.Warning.__weakref__"]
+            [0, "gensaschema.Warning.__weakref__"]
         ],
         "_ctype (gensaschema.type attribute)": [
-            [2, "gensaschema.Type._ctype"]
+            [0, "gensaschema.Type._ctype"]
         ],
         "_dbname (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema._dbname"]
+            [0, "gensaschema.Schema._dbname"]
         ],
         "_dialect (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema._dialect"]
+            [0, "gensaschema.Schema._dialect"]
         ],
         "_dialect (gensaschema.type attribute)": [
-            [2, "gensaschema.Type._dialect"]
+            [0, "gensaschema.Type._dialect"]
         ],
         "_lines (gensaschema.config attribute)": [
-            [2, "gensaschema.Config._lines"]
+            [0, "gensaschema.Config._lines"]
         ],
         "_schemas (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema._schemas"]
+            [0, "gensaschema.Schema._schemas"]
         ],
         "_symbols (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema._symbols"]
+            [0, "gensaschema.Schema._symbols"]
         ],
         "_symbols (gensaschema.symbols attribute)": [
-            [2, "gensaschema.Symbols._symbols"]
+            [0, "gensaschema.Symbols._symbols"]
         ],
         "_symbols (gensaschema.type attribute)": [
-            [2, "gensaschema.Type._symbols"]
+            [0, "gensaschema.Type._symbols"]
         ],
         "_tables (gensaschema.schema attribute)": [
-            [2, "gensaschema.Schema._tables"]
+            [0, "gensaschema.Schema._tables"]
         ],
         "by_column() (gensaschema.type class method)": [
-            [2, "gensaschema.Type.by_column"]
+            [0, "gensaschema.Type.by_column"]
         ],
         "dump() (gensaschema.config method)": [
-            [2, "gensaschema.Config.dump"]
+            [0, "gensaschema.Config.dump"]
         ],
         "dump() (gensaschema.schema method)": [
-            [2, "gensaschema.Schema.dump"]
+            [0, "gensaschema.Schema.dump"]
         ],
         "emit() (gensaschema.warning class method)": [
-            [2, "gensaschema.Warning.emit"]
+            [0, "gensaschema.Warning.emit"]
         ],
         "from_file() (gensaschema.config class method)": [
-            [2, "gensaschema.Config.from_file"]
+            [0, "gensaschema.Config.from_file"]
         ],
         "from_lines() (gensaschema.config class method)": [
-            [2, "gensaschema.Config.from_lines"]
+            [0, "gensaschema.Config.from_lines"]
         ],
         "from_parser() (gensaschema.config class method)": [
-            [2, "gensaschema.Config.from_parser"]
+            [0, "gensaschema.Config.from_parser"]
         ],
         "gensaschema": [
-            [2, "module-gensaschema"]
+            [0, "module-gensaschema"]
         ],
         "imports (gensaschema.symbols attribute)": [
-            [2, "gensaschema.Symbols.imports"]
+            [0, "gensaschema.Symbols.imports"]
         ],
         "module": [
-            [2, "module-gensaschema"],
-            [3, "module-gensaschema._column"],
-            [4, "module-gensaschema._config"],
-            [5, "module-gensaschema._constraint"],
-            [6, "module-gensaschema._exceptions"],
-            [7, "module-gensaschema._meta"],
-            [8, "module-gensaschema._schema"],
-            [9, "module-gensaschema._symbols"],
-            [10, "module-gensaschema._table"],
-            [11, "module-gensaschema._template"],
-            [12, "module-gensaschema._type"],
-            [13, "module-gensaschema._util"],
-            [14, "module-gensaschema.constraints"]
+            [0, "module-gensaschema"],
+            [1, "module-gensaschema._column"],
+            [2, "module-gensaschema._config"],
+            [3, "module-gensaschema._constraint"],
+            [4, "module-gensaschema._exceptions"],
+            [5, "module-gensaschema._meta"],
+            [6, "module-gensaschema._schema"],
+            [7, "module-gensaschema._symbols"],
+            [8, "module-gensaschema._table"],
+            [9, "module-gensaschema._template"],
+            [10, "module-gensaschema._type"],
+            [11, "module-gensaschema._util"],
+            [12, "module-gensaschema.constraints"]
         ],
         "schemas (gensaschema.config attribute)": [
-            [2, "gensaschema.Config.schemas"]
+            [0, "gensaschema.Config.schemas"]
         ],
         "tables (gensaschema.config attribute)": [
-            [2, "gensaschema.Config.tables"]
+            [0, "gensaschema.Config.tables"]
         ],
         "types (gensaschema.symbols attribute)": [
-            [2, "gensaschema.Symbols.types"]
+            [0, "gensaschema.Symbols.types"]
         ],
         "column (class in gensaschema._column)": [
-            [3, "gensaschema._column.Column"]
+            [1, "gensaschema._column.Column"]
         ],
         "serverdefault (class in gensaschema._column)": [
-            [3, "gensaschema._column.ServerDefault"]
+            [1, "gensaschema._column.ServerDefault"]
         ],
         "__dict__ (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column.__dict__"]
+            [1, "gensaschema._column.Column.__dict__"]
         ],
         "__dict__ (gensaschema._column.serverdefault attribute)": [
-            [3, "gensaschema._column.ServerDefault.__dict__"]
+            [1, "gensaschema._column.ServerDefault.__dict__"]
         ],
         "__init__() (gensaschema._column.column method)": [
-            [3, "gensaschema._column.Column.__init__"]
+            [1, "gensaschema._column.Column.__init__"]
         ],
         "__init__() (gensaschema._column.serverdefault method)": [
-            [3, "gensaschema._column.ServerDefault.__init__"]
+            [1, "gensaschema._column.ServerDefault.__init__"]
         ],
         "__module__ (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column.__module__"]
+            [1, "gensaschema._column.Column.__module__"]
         ],
         "__module__ (gensaschema._column.serverdefault attribute)": [
-            [3, "gensaschema._column.ServerDefault.__module__"]
+            [1, "gensaschema._column.ServerDefault.__module__"]
         ],
         "__repr__() (gensaschema._column.column method)": [
-            [3, "gensaschema._column.Column.__repr__"]
+            [1, "gensaschema._column.Column.__repr__"]
         ],
         "__repr__() (gensaschema._column.serverdefault method)": [
-            [3, "gensaschema._column.ServerDefault.__repr__"]
+            [1, "gensaschema._column.ServerDefault.__repr__"]
         ],
         "__weakref__ (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column.__weakref__"]
+            [1, "gensaschema._column.Column.__weakref__"]
         ],
         "__weakref__ (gensaschema._column.serverdefault attribute)": [
-            [3, "gensaschema._column.ServerDefault.__weakref__"]
+            [1, "gensaschema._column.ServerDefault.__weakref__"]
         ],
         "_autoincrement (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._autoincrement"]
+            [1, "gensaschema._column.Column._autoincrement"]
         ],
         "_ctype (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._ctype"]
+            [1, "gensaschema._column.Column._ctype"]
         ],
         "_default (gensaschema._column.serverdefault attribute)": [
-            [3, "gensaschema._column.ServerDefault._default"]
+            [1, "gensaschema._column.ServerDefault._default"]
         ],
         "_name (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._name"]
+            [1, "gensaschema._column.Column._name"]
         ],
         "_nullable (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._nullable"]
+            [1, "gensaschema._column.Column._nullable"]
         ],
         "_primary_key (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._primary_key"]
+            [1, "gensaschema._column.Column._primary_key"]
         ],
         "_server_default (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._server_default"]
+            [1, "gensaschema._column.Column._server_default"]
         ],
         "_symbols (gensaschema._column.column attribute)": [
-            [3, "gensaschema._column.Column._symbols"]
+            [1, "gensaschema._column.Column._symbols"]
         ],
         "_symbols (gensaschema._column.serverdefault attribute)": [
-            [3, "gensaschema._column.ServerDefault._symbols"]
+            [1, "gensaschema._column.ServerDefault._symbols"]
         ],
         "from_sa() (gensaschema._column.column class method)": [
-            [3, "gensaschema._column.Column.from_sa"]
+            [1, "gensaschema._column.Column.from_sa"]
         ],
         "gensaschema._column": [
-            [3, "module-gensaschema._column"]
+            [1, "module-gensaschema._column"]
         ],
         "config (class in gensaschema._config)": [
-            [4, "gensaschema._config.Config"]
+            [2, "gensaschema._config.Config"]
         ],
         "_config_tpl (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config._CONFIG_TPL"]
+            [2, "gensaschema._config.Config._CONFIG_TPL"]
         ],
         "__annotations__ (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config.__annotations__"]
+            [2, "gensaschema._config.Config.__annotations__"]
         ],
         "__dict__ (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config.__dict__"]
+            [2, "gensaschema._config.Config.__dict__"]
         ],
         "__init__() (gensaschema._config.config method)": [
-            [4, "gensaschema._config.Config.__init__"]
+            [2, "gensaschema._config.Config.__init__"]
         ],
         "__module__ (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config.__module__"]
+            [2, "gensaschema._config.Config.__module__"]
         ],
         "__weakref__ (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config.__weakref__"]
+            [2, "gensaschema._config.Config.__weakref__"]
         ],
         "_lines (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config._lines"]
+            [2, "gensaschema._config.Config._lines"]
         ],
         "dump() (gensaschema._config.config method)": [
-            [4, "gensaschema._config.Config.dump"]
+            [2, "gensaschema._config.Config.dump"]
         ],
         "from_file() (gensaschema._config.config class method)": [
-            [4, "gensaschema._config.Config.from_file"]
+            [2, "gensaschema._config.Config.from_file"]
         ],
         "from_lines() (gensaschema._config.config class method)": [
-            [4, "gensaschema._config.Config.from_lines"]
+            [2, "gensaschema._config.Config.from_lines"]
         ],
         "from_parser() (gensaschema._config.config class method)": [
-            [4, "gensaschema._config.Config.from_parser"]
+            [2, "gensaschema._config.Config.from_parser"]
         ],
         "gensaschema._config": [
-            [4, "module-gensaschema._config"]
+            [2, "module-gensaschema._config"]
         ],
         "schemas (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config.schemas"]
+            [2, "gensaschema._config.Config.schemas"]
         ],
         "tables (gensaschema._config.config attribute)": [
-            [4, "gensaschema._config.Config.tables"]
+            [2, "gensaschema._config.Config.tables"]
         ],
         "constraint (class in gensaschema._constraint)": [
-            [5, "gensaschema._constraint.Constraint"]
+            [3, "gensaschema._constraint.Constraint"]
         ],
         "foreignkeyconstraint (class in gensaschema._constraint)": [
-            [5, "gensaschema._constraint.ForeignKeyConstraint"]
+            [3, "gensaschema._constraint.ForeignKeyConstraint"]
         ],
         "primarykeyconstraint (class in gensaschema._constraint)": [
-            [5, "gensaschema._constraint.PrimaryKeyConstraint"]
+            [3, "gensaschema._constraint.PrimaryKeyConstraint"]
         ],
         "uniqueconstraint (class in gensaschema._constraint)": [
-            [5, "gensaschema._constraint.UniqueConstraint"]
+            [3, "gensaschema._constraint.UniqueConstraint"]
         ],
         "_import (gensaschema._constraint.constraint attribute)": [
-            [5, "gensaschema._constraint.Constraint._IMPORT"]
+            [3, "gensaschema._constraint.Constraint._IMPORT"]
         ],
         "_import (gensaschema._constraint.foreignkeyconstraint attribute)": [
-            [5, "gensaschema._constraint.ForeignKeyConstraint._IMPORT"]
+            [3, "gensaschema._constraint.ForeignKeyConstraint._IMPORT"]
         ],
         "_import (gensaschema._constraint.primarykeyconstraint attribute)": [
-            [5, "gensaschema._constraint.PrimaryKeyConstraint._IMPORT"]
+            [3, "gensaschema._constraint.PrimaryKeyConstraint._IMPORT"]
         ],
         "_import (gensaschema._constraint.uniqueconstraint attribute)": [
-            [5, "gensaschema._constraint.UniqueConstraint._IMPORT"]
+            [3, "gensaschema._constraint.UniqueConstraint._IMPORT"]
         ],
         "_symbol (gensaschema._constraint.constraint attribute)": [
-            [5, "gensaschema._constraint.Constraint._SYMBOL"]
+            [3, "gensaschema._constraint.Constraint._SYMBOL"]
         ],
         "_symbol (gensaschema._constraint.foreignkeyconstraint attribute)": [
-            [5, "gensaschema._constraint.ForeignKeyConstraint._SYMBOL"]
+            [3, "gensaschema._constraint.ForeignKeyConstraint._SYMBOL"]
         ],
         "_symbol (gensaschema._constraint.primarykeyconstraint attribute)": [
-            [5, "gensaschema._constraint.PrimaryKeyConstraint._SYMBOL"]
+            [3, "gensaschema._constraint.PrimaryKeyConstraint._SYMBOL"]
         ],
         "_symbol (gensaschema._constraint.uniqueconstraint attribute)": [
-            [5, "gensaschema._constraint.UniqueConstraint._SYMBOL"]
+            [3, "gensaschema._constraint.UniqueConstraint._SYMBOL"]
         ],
         "__annotations__ (gensaschema._constraint.foreignkeyconstraint attribute)": [
-            [5, "gensaschema._constraint.ForeignKeyConstraint.__annotations__"]
+            [3, "gensaschema._constraint.ForeignKeyConstraint.__annotations__"]
         ],
         "__annotations__ (gensaschema._constraint.primarykeyconstraint attribute)": [
-            [5, "gensaschema._constraint.PrimaryKeyConstraint.__annotations__"]
+            [3, "gensaschema._constraint.PrimaryKeyConstraint.__annotations__"]
         ],
         "__annotations__ (gensaschema._constraint.uniqueconstraint attribute)": [
-            [5, "gensaschema._constraint.UniqueConstraint.__annotations__"]
+            [3, "gensaschema._constraint.UniqueConstraint.__annotations__"]
         ],
         "__cmp__() (gensaschema._constraint.constraint method)": [
-            [5, "gensaschema._constraint.Constraint.__cmp__"]
+            [3, "gensaschema._constraint.Constraint.__cmp__"]
         ],
         "__dict__ (gensaschema._constraint.constraint attribute)": [
-            [5, "gensaschema._constraint.Constraint.__dict__"]
+            [3, "gensaschema._constraint.Constraint.__dict__"]
         ],
         "__init__() (gensaschema._constraint.constraint method)": [
-            [5, "gensaschema._constraint.Constraint.__init__"]
+            [3, "gensaschema._constraint.Constraint.__init__"]
         ],
         "__lt__() (gensaschema._constraint.constraint method)": [
-            [5, "gensaschema._constraint.Constraint.__lt__"]
+            [3, "gensaschema._constraint.Constraint.__lt__"]
         ],
         "__module__ (gensaschema._constraint.constraint attribute)": [
-            [5, "gensaschema._constraint.Constraint.__module__"]
+            [3, "gensaschema._constraint.Constraint.__module__"]
         ],
         "__module__ (gensaschema._constraint.foreignkeyconstraint attribute)": [
-            [5, "gensaschema._constraint.ForeignKeyConstraint.__module__"]
+            [3, "gensaschema._constraint.ForeignKeyConstraint.__module__"]
         ],
         "__module__ (gensaschema._constraint.primarykeyconstraint attribute)": [
-            [5, "gensaschema._constraint.PrimaryKeyConstraint.__module__"]
+            [3, "gensaschema._constraint.PrimaryKeyConstraint.__module__"]
         ],
         "__module__ (gensaschema._constraint.uniqueconstraint attribute)": [
-            [5, "gensaschema._constraint.UniqueConstraint.__module__"]
+            [3, "gensaschema._constraint.UniqueConstraint.__module__"]
         ],
         "__new__() (gensaschema._constraint.constraint static method)": [
-            [5, "gensaschema._constraint.Constraint.__new__"]
+            [3, "gensaschema._constraint.Constraint.__new__"]
         ],
         "__repr__() (gensaschema._constraint.foreignkeyconstraint method)": [
-            [5, "gensaschema._constraint.ForeignKeyConstraint.__repr__"]
+            [3, "gensaschema._constraint.ForeignKeyConstraint.__repr__"]
         ],
         "__repr__() (gensaschema._constraint.uniqueconstraint method)": [
-            [5, "gensaschema._constraint.UniqueConstraint.__repr__"]
+            [3, "gensaschema._constraint.UniqueConstraint.__repr__"]
         ],
         "__weakref__ (gensaschema._constraint.constraint attribute)": [
-            [5, "gensaschema._constraint.Constraint.__weakref__"]
+            [3, "gensaschema._constraint.Constraint.__weakref__"]
         ],
         "access_col() (in module gensaschema._constraint)": [
-            [5, "gensaschema._constraint.access_col"]
+            [3, "gensaschema._constraint.access_col"]
         ],
         "constraint (gensaschema._constraint.constraint attribute)": [
-            [5, "gensaschema._constraint.Constraint.constraint"]
+            [3, "gensaschema._constraint.Constraint.constraint"]
         ],
         "copy() (gensaschema._constraint.constraint method)": [
-            [5, "gensaschema._constraint.Constraint.copy"]
+            [3, "gensaschema._constraint.Constraint.copy"]
         ],
         "gensaschema._constraint": [
-            [5, "module-gensaschema._constraint"]
+            [3, "module-gensaschema._constraint"]
         ],
         "repr() (gensaschema._constraint.constraint method)": [
-            [5, "gensaschema._constraint.Constraint.repr"]
+            [3, "gensaschema._constraint.Constraint.repr"]
         ],
         "__annotations__ (gensaschema._exceptions.error attribute)": [
-            [6, "gensaschema._exceptions.Error.__annotations__"]
+            [4, "gensaschema._exceptions.Error.__annotations__"]
         ],
         "__annotations__ (gensaschema._exceptions.warning attribute)": [
-            [6, "gensaschema._exceptions.Warning.__annotations__"]
+            [4, "gensaschema._exceptions.Warning.__annotations__"]
         ],
         "__module__ (gensaschema._exceptions.error attribute)": [
-            [6, "gensaschema._exceptions.Error.__module__"]
+            [4, "gensaschema._exceptions.Error.__module__"]
         ],
         "__module__ (gensaschema._exceptions.warning attribute)": [
-            [6, "gensaschema._exceptions.Warning.__module__"]
+            [4, "gensaschema._exceptions.Warning.__module__"]
         ],
         "__weakref__ (gensaschema._exceptions.error attribute)": [
-            [6, "gensaschema._exceptions.Error.__weakref__"]
+            [4, "gensaschema._exceptions.Error.__weakref__"]
         ],
         "__weakref__ (gensaschema._exceptions.warning attribute)": [
-            [6, "gensaschema._exceptions.Warning.__weakref__"]
+            [4, "gensaschema._exceptions.Warning.__weakref__"]
         ],
         "emit() (gensaschema._exceptions.warning class method)": [
-            [6, "gensaschema._exceptions.Warning.emit"]
+            [4, "gensaschema._exceptions.Warning.emit"]
         ],
         "gensaschema._exceptions": [
-            [6, "module-gensaschema._exceptions"]
+            [4, "module-gensaschema._exceptions"]
         ],
         "boundmetadata (class in gensaschema._meta)": [
-            [7, "gensaschema._meta.BoundMetaData"]
+            [5, "gensaschema._meta.BoundMetaData"]
         ],
         "__dict__ (gensaschema._meta.boundmetadata attribute)": [
-            [7, "gensaschema._meta.BoundMetaData.__dict__"]
+            [5, "gensaschema._meta.BoundMetaData.__dict__"]
         ],
         "__getattr__() (gensaschema._meta.boundmetadata method)": [
-            [7, "gensaschema._meta.BoundMetaData.__getattr__"]
+            [5, "gensaschema._meta.BoundMetaData.__getattr__"]
         ],
         "__init__() (gensaschema._meta.boundmetadata method)": [
-            [7, "gensaschema._meta.BoundMetaData.__init__"]
+            [5, "gensaschema._meta.BoundMetaData.__init__"]
         ],
         "__module__ (gensaschema._meta.boundmetadata attribute)": [
-            [7, "gensaschema._meta.BoundMetaData.__module__"]
+            [5, "gensaschema._meta.BoundMetaData.__module__"]
         ],
         "__weakref__ (gensaschema._meta.boundmetadata attribute)": [
-            [7, "gensaschema._meta.BoundMetaData.__weakref__"]
+            [5, "gensaschema._meta.BoundMetaData.__weakref__"]
         ],
         "gensaschema._meta": [
-            [7, "module-gensaschema._meta"]
+            [5, "module-gensaschema._meta"]
         ],
         "schema (class in gensaschema._schema)": [
-            [8, "gensaschema._schema.Schema"]
+            [6, "gensaschema._schema.Schema"]
         ],
         "_module_tpl (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema._MODULE_TPL"]
+            [6, "gensaschema._schema.Schema._MODULE_TPL"]
         ],
         "__annotations__ (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema.__annotations__"]
+            [6, "gensaschema._schema.Schema.__annotations__"]
         ],
         "__dict__ (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema.__dict__"]
+            [6, "gensaschema._schema.Schema.__dict__"]
         ],
         "__init__() (gensaschema._schema.schema method)": [
-            [8, "gensaschema._schema.Schema.__init__"]
+            [6, "gensaschema._schema.Schema.__init__"]
         ],
         "__module__ (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema.__module__"]
+            [6, "gensaschema._schema.Schema.__module__"]
         ],
         "__weakref__ (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema.__weakref__"]
+            [6, "gensaschema._schema.Schema.__weakref__"]
         ],
         "_dbname (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema._dbname"]
+            [6, "gensaschema._schema.Schema._dbname"]
         ],
         "_dialect (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema._dialect"]
+            [6, "gensaschema._schema.Schema._dialect"]
         ],
         "_schemas (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema._schemas"]
+            [6, "gensaschema._schema.Schema._schemas"]
         ],
         "_symbols (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema._symbols"]
+            [6, "gensaschema._schema.Schema._symbols"]
         ],
         "_tables (gensaschema._schema.schema attribute)": [
-            [8, "gensaschema._schema.Schema._tables"]
+            [6, "gensaschema._schema.Schema._tables"]
         ],
         "dump() (gensaschema._schema.schema method)": [
-            [8, "gensaschema._schema.Schema.dump"]
+            [6, "gensaschema._schema.Schema.dump"]
         ],
         "gensaschema._schema": [
-            [8, "module-gensaschema._schema"]
+            [6, "module-gensaschema._schema"]
         ],
         "symbols (class in gensaschema._symbols)": [
-            [9, "gensaschema._symbols.Symbols"]
+            [7, "gensaschema._symbols.Symbols"]
         ],
         "_imports (class in gensaschema._symbols)": [
-            [9, "gensaschema._symbols._Imports"]
+            [7, "gensaschema._symbols._Imports"]
         ],
         "_types (class in gensaschema._symbols)": [
-            [9, "gensaschema._symbols._Types"]
+            [7, "gensaschema._symbols._Types"]
         ],
         "__annotations__ (gensaschema._symbols.symbolexception attribute)": [
-            [9, "gensaschema._symbols.SymbolException.__annotations__"]
+            [7, "gensaschema._symbols.SymbolException.__annotations__"]
         ],
         "__annotations__ (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols.__annotations__"]
+            [7, "gensaschema._symbols.Symbols.__annotations__"]
         ],
         "__contains__() (gensaschema._symbols.symbols method)": [
-            [9, "gensaschema._symbols.Symbols.__contains__"]
+            [7, "gensaschema._symbols.Symbols.__contains__"]
         ],
         "__contains__() (gensaschema._symbols._imports method)": [
-            [9, "gensaschema._symbols._Imports.__contains__"]
+            [7, "gensaschema._symbols._Imports.__contains__"]
         ],
         "__delitem__() (gensaschema._symbols.symbols method)": [
-            [9, "gensaschema._symbols.Symbols.__delitem__"]
+            [7, "gensaschema._symbols.Symbols.__delitem__"]
         ],
         "__dict__ (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols.__dict__"]
+            [7, "gensaschema._symbols.Symbols.__dict__"]
         ],
         "__dict__ (gensaschema._symbols._imports attribute)": [
-            [9, "gensaschema._symbols._Imports.__dict__"]
+            [7, "gensaschema._symbols._Imports.__dict__"]
         ],
         "__dict__ (gensaschema._symbols._types attribute)": [
-            [9, "gensaschema._symbols._Types.__dict__"]
+            [7, "gensaschema._symbols._Types.__dict__"]
         ],
         "__getitem__() (gensaschema._symbols.symbols method)": [
-            [9, "gensaschema._symbols.Symbols.__getitem__"]
+            [7, "gensaschema._symbols.Symbols.__getitem__"]
         ],
         "__init__() (gensaschema._symbols.symbols method)": [
-            [9, "gensaschema._symbols.Symbols.__init__"]
+            [7, "gensaschema._symbols.Symbols.__init__"]
         ],
         "__init__() (gensaschema._symbols._imports method)": [
-            [9, "gensaschema._symbols._Imports.__init__"]
+            [7, "gensaschema._symbols._Imports.__init__"]
         ],
         "__init__() (gensaschema._symbols._types method)": [
-            [9, "gensaschema._symbols._Types.__init__"]
+            [7, "gensaschema._symbols._Types.__init__"]
         ],
         "__iter__() (gensaschema._symbols.symbols method)": [
-            [9, "gensaschema._symbols.Symbols.__iter__"]
+            [7, "gensaschema._symbols.Symbols.__iter__"]
         ],
         "__iter__() (gensaschema._symbols._imports method)": [
-            [9, "gensaschema._symbols._Imports.__iter__"]
+            [7, "gensaschema._symbols._Imports.__iter__"]
         ],
         "__module__ (gensaschema._symbols.symbolexception attribute)": [
-            [9, "gensaschema._symbols.SymbolException.__module__"]
+            [7, "gensaschema._symbols.SymbolException.__module__"]
         ],
         "__module__ (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols.__module__"]
+            [7, "gensaschema._symbols.Symbols.__module__"]
         ],
         "__module__ (gensaschema._symbols._imports attribute)": [
-            [9, "gensaschema._symbols._Imports.__module__"]
+            [7, "gensaschema._symbols._Imports.__module__"]
         ],
         "__module__ (gensaschema._symbols._types attribute)": [
-            [9, "gensaschema._symbols._Types.__module__"]
+            [7, "gensaschema._symbols._Types.__module__"]
         ],
         "__setitem__() (gensaschema._symbols.symbols method)": [
-            [9, "gensaschema._symbols.Symbols.__setitem__"]
+            [7, "gensaschema._symbols.Symbols.__setitem__"]
         ],
         "__setitem__() (gensaschema._symbols._imports method)": [
-            [9, "gensaschema._symbols._Imports.__setitem__"]
+            [7, "gensaschema._symbols._Imports.__setitem__"]
         ],
         "__setitem__() (gensaschema._symbols._types method)": [
-            [9, "gensaschema._symbols._Types.__setitem__"]
+            [7, "gensaschema._symbols._Types.__setitem__"]
         ],
         "__weakref__ (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols.__weakref__"]
+            [7, "gensaschema._symbols.Symbols.__weakref__"]
         ],
         "__weakref__ (gensaschema._symbols._imports attribute)": [
-            [9, "gensaschema._symbols._Imports.__weakref__"]
+            [7, "gensaschema._symbols._Imports.__weakref__"]
         ],
         "__weakref__ (gensaschema._symbols._types attribute)": [
-            [9, "gensaschema._symbols._Types.__weakref__"]
+            [7, "gensaschema._symbols._Types.__weakref__"]
         ],
         "_imports (gensaschema._symbols._imports attribute)": [
-            [9, "gensaschema._symbols._Imports._imports"]
+            [7, "gensaschema._symbols._Imports._imports"]
         ],
         "_load_dotted() (in module gensaschema._symbols)": [
-            [9, "gensaschema._symbols._load_dotted"]
+            [7, "gensaschema._symbols._load_dotted"]
         ],
         "_symbols (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols._symbols"]
+            [7, "gensaschema._symbols.Symbols._symbols"]
         ],
         "_symbols (gensaschema._symbols._types attribute)": [
-            [9, "gensaschema._symbols._Types._symbols"]
+            [7, "gensaschema._symbols._Types._symbols"]
         ],
         "_types (gensaschema._symbols._types attribute)": [
-            [9, "gensaschema._symbols._Types._types"]
+            [7, "gensaschema._symbols._Types._types"]
         ],
         "gensaschema._symbols": [
-            [9, "module-gensaschema._symbols"]
+            [7, "module-gensaschema._symbols"]
         ],
         "imports (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols.imports"]
+            [7, "gensaschema._symbols.Symbols.imports"]
         ],
         "resolve() (gensaschema._symbols._types method)": [
-            [9, "gensaschema._symbols._Types.resolve"]
+            [7, "gensaschema._symbols._Types.resolve"]
         ],
         "types (gensaschema._symbols.symbols attribute)": [
-            [9, "gensaschema._symbols.Symbols.types"]
+            [7, "gensaschema._symbols.Symbols.types"]
         ],
         "table (class in gensaschema._table)": [
-            [10, "gensaschema._table.Table"]
+            [8, "gensaschema._table.Table"]
         ],
         "tablecollection (class in gensaschema._table)": [
-            [10, "gensaschema._table.TableCollection"]
+            [8, "gensaschema._table.TableCollection"]
         ],
         "tablereference (class in gensaschema._table)": [
-            [10, "gensaschema._table.TableReference"]
+            [8, "gensaschema._table.TableReference"]
         ],
         "__dict__ (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.__dict__"]
+            [8, "gensaschema._table.Table.__dict__"]
         ],
         "__dict__ (gensaschema._table.tablecollection attribute)": [
-            [10, "gensaschema._table.TableCollection.__dict__"]
+            [8, "gensaschema._table.TableCollection.__dict__"]
         ],
         "__dict__ (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.__dict__"]
+            [8, "gensaschema._table.TableReference.__dict__"]
         ],
         "__init__() (gensaschema._table.table method)": [
-            [10, "gensaschema._table.Table.__init__"]
+            [8, "gensaschema._table.Table.__init__"]
         ],
         "__init__() (gensaschema._table.tablereference method)": [
-            [10, "gensaschema._table.TableReference.__init__"]
+            [8, "gensaschema._table.TableReference.__init__"]
         ],
         "__module__ (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.__module__"]
+            [8, "gensaschema._table.Table.__module__"]
         ],
         "__module__ (gensaschema._table.tablecollection attribute)": [
-            [10, "gensaschema._table.TableCollection.__module__"]
+            [8, "gensaschema._table.TableCollection.__module__"]
         ],
         "__module__ (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.__module__"]
+            [8, "gensaschema._table.TableReference.__module__"]
         ],
         "__new__() (gensaschema._table.table static method)": [
-            [10, "gensaschema._table.Table.__new__"]
+            [8, "gensaschema._table.Table.__new__"]
         ],
         "__repr__() (gensaschema._table.table method)": [
-            [10, "gensaschema._table.Table.__repr__"]
+            [8, "gensaschema._table.Table.__repr__"]
         ],
         "__weakref__ (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.__weakref__"]
+            [8, "gensaschema._table.Table.__weakref__"]
         ],
         "__weakref__ (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.__weakref__"]
+            [8, "gensaschema._table.TableReference.__weakref__"]
         ],
         "_break_cycles() (in module gensaschema._table)": [
-            [10, "gensaschema._table._break_cycles"]
+            [8, "gensaschema._table._break_cycles"]
         ],
         "_symbols (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table._symbols"]
+            [8, "gensaschema._table.Table._symbols"]
         ],
         "by_name() (gensaschema._table.table class method)": [
-            [10, "gensaschema._table.Table.by_name"]
+            [8, "gensaschema._table.Table.by_name"]
         ],
         "by_names() (gensaschema._table.tablecollection class method)": [
-            [10, "gensaschema._table.TableCollection.by_names"]
+            [8, "gensaschema._table.TableCollection.by_names"]
         ],
         "constraints (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.constraints"]
+            [8, "gensaschema._table.Table.constraints"]
         ],
         "constraints (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.constraints"]
+            [8, "gensaschema._table.TableReference.constraints"]
         ],
         "gensaschema._table": [
-            [10, "module-gensaschema._table"]
+            [8, "module-gensaschema._table"]
         ],
         "is_reference (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.is_reference"]
+            [8, "gensaschema._table.Table.is_reference"]
         ],
         "is_reference (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.is_reference"]
+            [8, "gensaschema._table.TableReference.is_reference"]
         ],
         "sa_table (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.sa_table"]
+            [8, "gensaschema._table.Table.sa_table"]
         ],
         "sa_table (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.sa_table"]
+            [8, "gensaschema._table.TableReference.sa_table"]
         ],
         "varname (gensaschema._table.table attribute)": [
-            [10, "gensaschema._table.Table.varname"]
+            [8, "gensaschema._table.Table.varname"]
         ],
         "varname (gensaschema._table.tablereference attribute)": [
-            [10, "gensaschema._table.TableReference.varname"]
+            [8, "gensaschema._table.TableReference.varname"]
         ],
         "template (class in gensaschema._template)": [
-            [11, "gensaschema._template.Template"]
+            [9, "gensaschema._template.Template"]
         ],
         "__dict__ (gensaschema._template.template attribute)": [
-            [11, "gensaschema._template.Template.__dict__"]
+            [9, "gensaschema._template.Template.__dict__"]
         ],
         "__init__() (gensaschema._template.template method)": [
-            [11, "gensaschema._template.Template.__init__"]
+            [9, "gensaschema._template.Template.__init__"]
         ],
         "__module__ (gensaschema._template.template attribute)": [
-            [11, "gensaschema._template.Template.__module__"]
+            [9, "gensaschema._template.Template.__module__"]
         ],
         "__weakref__ (gensaschema._template.template attribute)": [
-            [11, "gensaschema._template.Template.__weakref__"]
+            [9, "gensaschema._template.Template.__weakref__"]
         ],
         "_template (gensaschema._template.template attribute)": [
-            [11, "gensaschema._template.Template._template"]
+            [9, "gensaschema._template.Template._template"]
         ],
         "expand() (gensaschema._template.template method)": [
-            [11, "gensaschema._template.Template.expand"]
+            [9, "gensaschema._template.Template.expand"]
         ],
         "gensaschema._template": [
-            [11, "module-gensaschema._template"]
+            [9, "module-gensaschema._template"]
         ],
         "type (class in gensaschema._type)": [
-            [12, "gensaschema._type.Type"]
+            [10, "gensaschema._type.Type"]
         ],
         "__annotations__ (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type.__annotations__"]
+            [10, "gensaschema._type.Type.__annotations__"]
         ],
         "__dict__ (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type.__dict__"]
+            [10, "gensaschema._type.Type.__dict__"]
         ],
         "__init__() (gensaschema._type.type method)": [
-            [12, "gensaschema._type.Type.__init__"]
+            [10, "gensaschema._type.Type.__init__"]
         ],
         "__module__ (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type.__module__"]
+            [10, "gensaschema._type.Type.__module__"]
         ],
         "__repr__() (gensaschema._type.type method)": [
-            [12, "gensaschema._type.Type.__repr__"]
+            [10, "gensaschema._type.Type.__repr__"]
         ],
         "__weakref__ (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type.__weakref__"]
+            [10, "gensaschema._type.Type.__weakref__"]
+        ],
+        "_add_postgres_enum() (in module gensaschema._type)": [
+            [10, "gensaschema._type._add_postgres_enum"]
         ],
         "_ctype (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type._ctype"]
+            [10, "gensaschema._type.Type._ctype"]
         ],
         "_dialect (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type._dialect"]
+            [10, "gensaschema._type.Type._dialect"]
+        ],
+        "_finalize_type() (in module gensaschema._type)": [
+            [10, "gensaschema._type._finalize_type"]
         ],
         "_find_class() (in module gensaschema._type)": [
-            [12, "gensaschema._type._find_class"]
+            [10, "gensaschema._type._find_class"]
         ],
         "_symbols (gensaschema._type.type attribute)": [
-            [12, "gensaschema._type.Type._symbols"]
+            [10, "gensaschema._type.Type._symbols"]
         ],
         "by_column() (gensaschema._type.type class method)": [
-            [12, "gensaschema._type.Type.by_column"]
+            [10, "gensaschema._type.Type.by_column"]
         ],
         "gensaschema._type": [
-            [12, "module-gensaschema._type"]
+            [10, "module-gensaschema._type"]
         ],
         "cmp() (in module gensaschema._util)": [
-            [13, "gensaschema._util.cmp"]
+            [11, "gensaschema._util.cmp"]
         ],
         "find_public() (in module gensaschema._util)": [
-            [13, "gensaschema._util.find_public"]
+            [11, "gensaschema._util.find_public"]
         ],
         "gensaschema._util": [
-            [13, "module-gensaschema._util"]
+            [11, "module-gensaschema._util"]
         ],
         "foreignkey() (in module gensaschema.constraints)": [
-            [14, "gensaschema.constraints.ForeignKey"]
+            [12, "gensaschema.constraints.ForeignKey"]
         ],
         "primarykey() (in module gensaschema.constraints)": [
-            [14, "gensaschema.constraints.PrimaryKey"]
+            [12, "gensaschema.constraints.PrimaryKey"]
         ],
         "unique() (in module gensaschema.constraints)": [
-            [14, "gensaschema.constraints.Unique"]
+            [12, "gensaschema.constraints.Unique"]
         ],
         "gensaschema.constraints": [
-            [14, "module-gensaschema.constraints"]
+            [12, "module-gensaschema.constraints"]
         ]
     }
 })
```

### Comparing `gensaschema-0.6.7/gensaschema/__init__.py` & `gensaschema-0.6.8/gensaschema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ==================================================
 
 GenSASchema generates static schema definitions using SQLAlchemy's
 inspection capabilities.
 """
 __author__ = u"Andr\xe9 Malo"
 __license__ = "Apache License, Version 2.0"
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 
 from gensaschema import _util
 from gensaschema._exceptions import *  # noqa pylint: disable = redefined-builtin, wildcard-import
 
 from gensaschema._config import Config  # noqa
 from gensaschema._schema import Schema  # noqa
 from gensaschema._symbols import Symbols, SymbolException  # noqa
```

### Comparing `gensaschema-0.6.7/gensaschema/_column.py` & `gensaschema-0.6.8/gensaschema/_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,15 @@
         """
         Make string representation
 
         Return:
           str: The string representation
         """
         identity = getattr(_sa, 'Identity', None)
-        if identity is not None \
-                and isinstance(self._default, identity):
+        if identity is not None and isinstance(self._default, identity):
             return "%s.%s" % (
                 self._symbols['sa'],
                 _util.unicode(self._default),
             )
 
         if self._default.for_update:
             for_update = ", for_update=%r" % (True,)
@@ -110,16 +109,24 @@
       _server_default (Default clause):
         Default clause
 
       _symbols (Symbols):
         Symbol table
     """
 
-    def __init__(self, name, ctype, nullable, primary_key, autoincrement,
-                 server_default, symbols):
+    def __init__(
+        self,
+        name,
+        ctype,
+        nullable,
+        primary_key,
+        autoincrement,
+        server_default,
+        symbols,
+    ):
         """
         Initialization
 
         Parameters:
           name (unicode):
             Column name
 
@@ -183,13 +190,12 @@
         """
         params = list(map(repr, (self._name, self._ctype)))
         if not self._nullable:
             params.append('nullable=%r' % (False,))
         if not self._autoincrement and self._primary_key:
             params.append('autoincrement=%r' % (False,))
         if self._server_default is not None:
-            params.append('server_default=%r' % (
-                ServerDefault(self._server_default, self._symbols),
-            ))
-        return "%s(%s)" % (
-            self._symbols['column'], ', '.join(params)
-        )
+            params.append(
+                'server_default=%r'
+                % (ServerDefault(self._server_default, self._symbols),)
+            )
+        return "%s(%s)" % (self._symbols['column'], ', '.join(params))
```

### Comparing `gensaschema-0.6.7/gensaschema/_config.py` & `gensaschema-0.6.8/gensaschema/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 __author__ = u"Andr\xe9 Malo"
 
 import errno as _errno
 
 if 1:
     try:
         import ConfigParser as _config_parser
-    except ImportError:  # pragma: no cover
+    except ImportError:
         import configparser as _config_parser
 
     try:
         from cStringIO import StringIO as _TextIO
-    except ImportError:  # pragma: no cover
+    except ImportError:
         from io import StringIO as _TextIO
 
 from . import _template
 
 
 class Config(object):
     """
@@ -58,30 +58,32 @@
       _lines (list):
         Original config lines (or ``None``)
     """
 
     #: Template for empty config file
     #:
     #: :Type: `Template`
-    _CONFIG_TPL = _template.Template('''
+    _CONFIG_TPL = _template.Template(
+        '''
         # This is a comment. I love comments.
         #
         # This files contains table names, one per line
         # Comments and empty lines are ignored
         #
         # If the table name contains a dot, the first part is treated as
         # schema name.
         #
         # If the table variable should be treated differently, use:
         #
         # name = table
         #
         # The basename of this file (modulo .schema extension) is used as
         # basename for the python file.
-    ''')
+    '''
+    )
 
     def __init__(self, tables, schemas, lines=None):
         """
         Initialization
 
         Parameters:
           tables (list):
@@ -204,16 +206,18 @@
         if not lines:
             result = self._CONFIG_TPL.expand().splitlines(False)
             if lines is None:
                 tables = ['%s = %s' % table for table in self.tables]
                 if tables:
                     result.append('')
                     result.extend(tables)
-                schemas = ['%s = %s' % (key, value)
-                           for key, value in self.schemas.items()]
+                schemas = [
+                    '%s = %s' % (key, value)
+                    for key, value in self.schemas.items()
+                ]
                 if schemas:
                     result.append('')
                     result.append('[schemas]')
                     result.extend(schemas)
         else:
             result = lines
```

### Comparing `gensaschema-0.6.7/gensaschema/_constraint.py` & `gensaschema-0.6.8/gensaschema/_constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,19 @@
     """
     Reflected Constraint
 
     Attributes:
       constraint (SA Constraint):
         Constraint
     """
+
     _SYMBOL, _IMPORT = None, None
 
     def __new__(cls, constraint, table, symbols, options=None):
-        """ Constraint factory """
+        """Constraint factory"""
         if cls == Constraint:
             name = constraint.__class__.__name__
             if name == 'CheckConstraint':
                 return None
             return globals()[name](
                 constraint, table, symbols, options=options
             )
@@ -76,47 +77,52 @@
         self.constraint = constraint
         self.table = table
         self._symbols = symbols
         self._symbols.imports[self._SYMBOL] = self._IMPORT
         self.options = options
 
     def copy(self):
-        """ Create shallow copy """
+        """Create shallow copy"""
         return self.__class__(
             self.constraint, self.table, self._symbols, self.options
         )
 
     def __cmp__(self, other):
-        """ Compare """
+        """Compare"""
         names = [
-            'PrimaryKeyConstraint', 'UniqueConstraint',
-            'ForeignKeyConstraint', 'CheckConstraint'
+            'PrimaryKeyConstraint',
+            'UniqueConstraint',
+            'ForeignKeyConstraint',
+            'CheckConstraint',
         ]
 
         def bytype(const):
-            """ Sort by type """
+            """Sort by type"""
             try:
                 return names.index(const.__class__.__name__)
             except IndexError:
                 return -1
 
-        return _util.cmp((
-            bytype(self.constraint),
-            self.options is not None,
-            self.constraint.name,
-            repr(self),
-        ), (
-            bytype(other.constraint),
-            other.options is not None,
-            other.constraint.name,
-            repr(other),
-        ))
+        return _util.cmp(
+            (
+                bytype(self.constraint),
+                self.options is not None,
+                self.constraint.name,
+                repr(self),
+            ),
+            (
+                bytype(other.constraint),
+                other.options is not None,
+                other.constraint.name,
+                repr(other),
+            ),
+        )
 
     def __lt__(self, other, _cmp=__cmp__):
-        """ Check for '<' """
+        """Check for '<'"""
         return _cmp(self, other) < 0
 
     def repr(self, symbol, args, keywords=(), short=False):
         """
         Base repr for all constraints
 
         Parameters:
@@ -143,17 +149,17 @@
             params.append('name=%r' % (self.constraint.name,))
         if self.constraint.deferrable is not None:
             params.append('deferrable=%r' % (self.constraint.deferrable,))
         if self.constraint.initially is not None:
             params.append('initially=%r' % (self.constraint.initially,))
         for keyword in keywords:
             if getattr(self.constraint, keyword) is not None:
-                params.append("%s=%r" % (
-                    keyword, getattr(self.constraint, keyword)
-                ))
+                params.append(
+                    "%s=%r" % (keyword, getattr(self.constraint, keyword))
+                )
         if short and len(params) > 1:
             short = False
         if args:
             if short:
                 args = ', '.join(args)
             else:
                 args = '\n    ' + ',\n    '.join(args) + ','
@@ -186,98 +192,117 @@
       str: Access string
     """
     try:
         name = col.name
     except AttributeError:
         name = col
     try:
-        if _util.py2 and isinstance(name, _util.bytes):  # pragma: no cover
+        if _util.py2 and isinstance(name, _util.bytes):
             name.decode('ascii')
         else:
             name.encode('ascii')
     except UnicodeError:
         is_ascii = False
     else:
         is_ascii = True
-    if is_ascii and not _keyword.iskeyword(name) and \
-            _re.match(_tokenize.Name + '$', name):
+    if (
+        is_ascii
+        and not _keyword.iskeyword(name)
+        and _re.match(_tokenize.Name + '$', name)
+    ):
         return ".c.%s" % name
     return ".c[%r]" % name
 
 
 class UniqueConstraint(Constraint):
-    """ Unique constraint """
+    """Unique constraint"""
+
     _SYMBOL = 'uk'
     _IMPORT = 'from %(constraints)s import Unique as %(uk)s'
 
     def __repr__(self):
         """
         Make string representation
 
         Returns:
           str: The string representation
         """
         empty = len(self.constraint.columns) == 0
         short = len(self.constraint.columns) <= 1
-        result = self.repr(self._SYMBOL, [
-            "%s%s" % (self.table, access_col(col))
-            for col in self.constraint.columns
-        ], short=short)
+        result = self.repr(
+            self._SYMBOL,
+            [
+                "%s%s" % (self.table, access_col(col))
+                for col in self.constraint.columns
+            ],
+            short=short,
+        )
         if empty:
             result = "# %s" % result
         return result
 
 
 class PrimaryKeyConstraint(UniqueConstraint):
-    """ Primary Key constraint """
+    """Primary Key constraint"""
+
     _SYMBOL = 'pk'
     _IMPORT = 'from %(constraints)s import PrimaryKey as %(pk)s'
 
 
 class ForeignKeyConstraint(Constraint):
-    """ ForeignKey constraint """
+    """ForeignKey constraint"""
+
     _SYMBOL = 'fk'
     _IMPORT = 'from %(constraints)s import ForeignKey as %(fk)s'
 
     def __repr__(self):
         """
         Make string representation
 
         Returns:
           str: The string representation
         """
-        columns = "[%s]" % ',\n    '.join([
-            "%s%s" % (self.table, access_col(col))
-            for col in self.constraint.columns
-        ])
-        refcolumns = "[%s]" % ',\n    '.join(["%s%s" % (
-            self._symbols[u'table_%s' % key.column.table.name],
-            access_col(key.column),
-        ) for key in self.constraint.elements])
+        columns = "[%s]" % ',\n    '.join(
+            [
+                "%s%s" % (self.table, access_col(col))
+                for col in self.constraint.columns
+            ]
+        )
+        refcolumns = "[%s]" % ',\n    '.join(
+            [
+                "%s%s"
+                % (
+                    self._symbols[u'table_%s' % key.column.table.name],
+                    access_col(key.column),
+                )
+                for key in self.constraint.elements
+            ]
+        )
         keywords = ['onupdate', 'ondelete']
         if self.constraint.use_alter:
             keywords.append('use_alter')
         result = self.repr('fk', [columns, refcolumns], keywords)
 
         if self.options:
             cyclic = self.constraint.use_alter
             if self.options.startswith('seen:'):
                 table = self.options.split(None, 1)[1]
                 if cyclic:
                     result = '\n# Cyclic foreign key:\n' + result
                 else:
                     result = '\n# Foreign key belongs to %r:\n%s' % (
-                        table, result
+                        table,
+                        result,
                     )
             elif self.options.startswith('unseen:'):
                 table = self.options.split(None, 1)[1]
                 result = result.splitlines(True)
                 if cyclic:
                     result.insert(
                         0,
-                        'Cyclic foreign key, defined at table %r:\n' % table
+                        'Cyclic foreign key, defined at table %r:\n' % table,
                     )
                 else:
                     result.insert(0, 'Defined at table %r:\n' % table)
                 result = '\n' + ''.join(['# %s' % item for item in result])
 
         return result
```

### Comparing `gensaschema-0.6.7/gensaschema/_exceptions.py` & `gensaschema-0.6.8/gensaschema/_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 """
 __author__ = u"Andr\xe9 Malo"
 
 import warnings as _warnings
 
 
 class Error(Exception):
-    """ Base exception for this package """
+    """Base exception for this package"""
 
 
-class Warning(Warning):  # noqa pylint: disable = redefined-builtin, undefined-variable
+class Warning(
+    Warning
+):  # noqa pylint: disable = redefined-builtin, undefined-variable
     """
     Base warning for this package
 
     >>> with _warnings.catch_warnings(record=True) as record:
     ...     Warning.emit('my message')
     ...     assert len(record) == 1
     ...     str(record[0].message)
@@ -49,15 +51,15 @@
     >>> Warning.emit('lalala')
     Traceback (most recent call last):
     ...
     Warning: lalala
     """
 
     @classmethod
-    def emit(cls, message, stacklevel=1):  # pragma: no cover
+    def emit(cls, message, stacklevel=1):
         """
         Emit a warning of this very category
 
         This method is pure convenience. It saves you the unfriendly
         ``warnings.warn`` syntax (and the ``warnings`` import).
 
         :Parameters:
```

### Comparing `gensaschema-0.6.7/gensaschema/_meta.py` & `gensaschema-0.6.8/gensaschema/_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,13 +31,14 @@
 import sqlalchemy as _sa
 
 
 class BoundMetaData(object):
     """
     Bound metadata proxy - SA 2.0 removed the bind, but it's part of our APIs
     """
+
     def __init__(self, bind):
         self._metadata = _sa.MetaData()
         self.bind = bind
 
     def __getattr__(self, name):
         return getattr(self._metadata, name)
```

### Comparing `gensaschema-0.6.7/gensaschema/_schema.py` & `gensaschema-0.6.8/gensaschema/_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,16 @@
       _dbname (str or None):
         DB identifier
     """
 
     #: Template for the module
     #:
     #: :Type: Template
-    _MODULE_TPL = _template.Template('''
+    _MODULE_TPL = _template.Template(
+        '''
         # -*- coding: ascii -*-
         # flake8: noqa pylint: skip-file
         """
         ==============================
          SQLAlchemy schema definition
         ==============================
 
@@ -77,18 +78,20 @@
         %(table)s = %(sa)s.Table
         %(column)s = %(sa)s.Column
         %(default)s = %(sa)s.DefaultClause
         %(lines)s
         del %(sa)s, %(table)s, %(column)s, %(default)s, %(meta)s
 
         # vim: nowrap tw=0
-    ''')
+    '''
+    )
 
-    def __init__(self, conn, tables, schemas, symbols, dbname=None,
-                 types=None):
+    def __init__(
+        self, conn, tables, schemas, symbols, dbname=None, types=None
+    ):
         """
         Initialization
 
         Parameters:
           conn (Connection or Engine):
             SQLAlchemy connection or engine
 
@@ -126,44 +129,48 @@
         """
         Dump schema module to fp
 
         Parameters:
           fp (file):
             File to write to
         """
+        lines, dlines = [], []
+        for table in self._tables:
+            if table.is_reference:
+                continue
+            name = table.sa_table.name.encode('ascii', 'backslashescape')
+            if bytes is not str:
+                name = name.decode('ascii')
+            lines.append('# Table "%s"' % (name,))
+            lines.append('%s = %r' % (table.varname, table))
+            lines.append('')
+            lines.append('')
+
         imports = [item % self._symbols for item in self._symbols.imports]
         if imports:  # pragma: no branch
             imports.sort()
             imports.append('')
-        lines = []
 
         defines = self._symbols.types.defines
         if defines:
             defined = []
+            seen = set()
             for define in defines:
-                defined.extend(define(self._dialect, self._symbols))
+                for item in define(self._dialect, self._symbols):
+                    if item not in seen:
+                        defined.append(item)
+                        seen.add(item)
             if defined:
-                lines.append('')
-                lines.append('# Custom type definitions')
-                lines.extend(defined)
-                lines.append('')
+                dlines = ['', '# Custom type definitions'] + defined
 
-        for table in self._tables:
-            if table.is_reference:
-                continue
-            if not lines:
-                lines.append('')
-            name = table.sa_table.name.encode('ascii', 'backslashescape')
-            if bytes is not str:  # pragma: no cover
-                name = name.decode('ascii')
-            lines.append('# Table "%s"' % (name,))
-            lines.append('%s = %r' % (table.varname, table))
-            lines.append('')
-            lines.append('')
+        if lines:
+            dlines.append('')
 
-        param = dict(((str(key), value) for key, value in self._symbols),
-                     dbspec=" for %s" % self._dbname if self._dbname else "",
-                     dialect=self._dialect,
-                     imports='\n'.join(imports),
-                     lines='\n'.join(lines))
+        param = dict(
+            ((str(key), value) for key, value in self._symbols),
+            dbspec=" for %s" % self._dbname if self._dbname else "",
+            dialect=self._dialect,
+            imports='\n'.join(imports),
+            lines='\n'.join(dlines + lines),
+        )
         fp.write(self._MODULE_TPL.expand(**param))
         fp.write('\n')
```

### Comparing `gensaschema-0.6.7/gensaschema/_symbols.py` & `gensaschema-0.6.8/gensaschema/_symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import weakref as _weakref
 
 from . import _exceptions
 from . import _util
 
 
 class SymbolException(_exceptions.Error):
-    """ Symbol error """
+    """Symbol error"""
 
 
 class Symbols(object):
     """
     Symbol table
 
     Attributes:
@@ -65,24 +65,24 @@
 
           imports (iterable):
             List of initial (id, import statement) tuples. If omitted or
             ``None``, it's empty.
         """
         self._symbols = {}
         defaults = dict(
-            sa="_sa",          # SQLAlchemy shortname
-            meta="m",          # MetaData shortname
-            table="T",         # Table shortname
-            type="t",          # Type module shortname
-            column="C",        # Column shortname
-            default="D",       # DefaultClause shortname
-            pk="PrimaryKey",   # PrimaryKey function name
-            fk="ForeignKey",   # ForeignKey function name
-            uk="Unique",       # UniqueKey function name
-            constraints=(      # constraint function module
+            sa="_sa",  # SQLAlchemy shortname
+            meta="m",  # MetaData shortname
+            table="T",  # Table shortname
+            type="t",  # Type module shortname
+            column="C",  # Column shortname
+            default="D",  # DefaultClause shortname
+            pk="PrimaryKey",  # PrimaryKey function name
+            fk="ForeignKey",  # ForeignKey function name
+            uk="Unique",  # UniqueKey function name
+            constraints=(  # constraint function module
                 __name__.rsplit('.', 1)[0] + '.constraints'
             ),
         )
         self.imports = _Imports(imports=imports)
         self.types = _Types(_weakref.proxy(self))
         if symbols is None:
             symbols = {}
@@ -116,15 +116,17 @@
 
           symbol (str):
             Symbol
 
         Raises:
           SymbolException: Symbol could not be set because of some conflict
         """
-        if _util.py2 and not isinstance(name, _util.unicode):  # pragma: no cover
+        if _util.py2 and not isinstance(
+            name, _util.unicode
+        ):  # pragma: no cover
             name = str(name).decode('ascii')
         if _keyword.iskeyword(symbol):
             raise SymbolException(
                 "Cannot use keyword %r as symbol" % (symbol,)
             )
         elif symbol in list(self._symbols.values()):
             if name in self._symbols and self._symbols[name] != symbol:
@@ -247,29 +249,29 @@
         mod = type_.__module__
         if mod.startswith('sqlalchemy.'):
             mod = '.'.join(mod.split('.')[:3])
             if mod == 'sqlalchemy.dialects.%s' % dialect:
                 return self._symbols['type']
             else:
                 try:
-                    _load_dotted('sqlalchemy.dialects.%s.%s' % (
-                        dialect, type_.__class__.__name__
-                    ))
+                    _load_dotted(
+                        'sqlalchemy.dialects.%s.%s'
+                        % (dialect, type_.__class__.__name__)
+                    )
                     return self._symbols['type']
                 except ImportError:
                     try:
-                        _load_dotted('sqlalchemy.types.%s' % (
-                            type_.__class__.__name__,
-                        ))
+                        _load_dotted(
+                            'sqlalchemy.types.%s'
+                            % (type_.__class__.__name__,)
+                        )
                         return "%s.types" % (self._symbols['sa'],)
                     except ImportError:
                         pass
-        raise SymbolException(
-            "Don't know how to address type %r" % (type_,)
-        )
+        raise SymbolException("Don't know how to address type %r" % (type_,))
 
 
 class _Imports(object):
     """
     Import table
 
     Attributes:
@@ -314,22 +316,25 @@
 
           import_ (str):
             Import statement
 
         Raises:
           SymbolException: Import conflict
         """
-        if _util.py2 and not isinstance(name, _util.unicode):  # pragma: no cover
+        if _util.py2 and not isinstance(
+            name, _util.unicode
+        ):  # pragma: no cover
             name = str(name).decode('ascii')
         imports = dict(self._imports)
         if name in imports:
             if imports[name] != import_:
-                raise SymbolException("Import conflict: %r: %r vs. %r" % (
-                    name, imports[name], import_
-                ))
+                raise SymbolException(
+                    "Import conflict: %r: %r vs. %r"
+                    % (name, imports[name], import_)
+                )
         else:
             self._imports.append((name, import_))
 
     def __iter__(self):
         """
         Make iterator over the import statements
```

### Comparing `gensaschema-0.6.7/gensaschema/_table.py` & `gensaschema-0.6.8/gensaschema/_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
       constraints (list):
         Constraint list
 
       _symbols (Symbols):
         Symbol table
     """
+
     #: Is it a table reference (vs. a table)?
     #:
     #: :Type: bool
     is_reference = False
 
     def __new__(cls, varname, table, schemas, symbols):
         """
@@ -112,17 +113,27 @@
         """
         # pylint: disable = unused-argument
 
         symbols[u'table_%s' % table.name] = varname
         self._symbols = symbols
         self.varname = varname
         self.sa_table = table
-        self.constraints = list(filter(None, [_constraint.Constraint(
-            con, self.varname, self._symbols,
-        ) for con in table.constraints]))
+        self.constraints = list(
+            filter(
+                None,
+                [
+                    _constraint.Constraint(
+                        con,
+                        self.varname,
+                        self._symbols,
+                    )
+                    for con in table.constraints
+                ],
+            )
+        )
 
     @classmethod
     def by_name(cls, name, varname, metadata, schemas, symbols, types=None):
         """
         Construct by name
 
         Parameters:
@@ -144,68 +155,92 @@
           types (callable):
             Extra type loader. If the type reflection fails, because
             SQLAlchemy cannot resolve it, the type loader will be called with
             the type name, (bound) metadata and the symbol table. It is
             responsible for modifying the symbols and imports *and* the
             dialect's ``ischema_names``. If omitted or ``None``, the reflector
             will always fail on unknown types.
+
+        Returns:
+          Table: new Table instance
         """
         kwargs = {}
         if '.' in name:
             schema, name = name.split('.')
             kwargs['schema'] = schema
         else:
             schema = None
 
         tmatch = _re.compile(u"^Did not recognize type (.+) of column").match
 
         def type_name(e):
-            """ Extract type name from exception """
+            """Extract type name from exception"""
             match = tmatch(e.args[0])
             if match:
                 type_name = match.group(1).strip()
                 if type_name.startswith(('"', "'")):
                     type_name = type_name[1:-1]
                 return type_name or None
             return None
 
         with _warnings.catch_warnings():
-            _warnings.filterwarnings('error', category=_sa.exc.SAWarning,
-                                     message=r'^Did not recognize type ')
-            _warnings.filterwarnings('error', category=_sa.exc.SAWarning,
-                                     message=r'^Unknown column definition ')
-            _warnings.filterwarnings('error', category=_sa.exc.SAWarning,
-                                     message=r'^Incomplete reflection of '
-                                             r'column definition')
-            _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                     message=r'^Could not instantiate type ')
-            _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                     message=r'^Skipped unsupported '
-                                             r'reflection of expression-based'
-                                             r' index ')
-            _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                     message=r'^Predicate of partial index ')
+            _warnings.filterwarnings(
+                'error',
+                category=_sa.exc.SAWarning,
+                message=r'^Did not recognize type ',
+            )
+            _warnings.filterwarnings(
+                'error',
+                category=_sa.exc.SAWarning,
+                message=r'^Unknown column definition ',
+            )
+            _warnings.filterwarnings(
+                'error',
+                category=_sa.exc.SAWarning,
+                message=r'^Incomplete reflection of ' r'column definition',
+            )
+            _warnings.filterwarnings(
+                'ignore',
+                category=_sa.exc.SAWarning,
+                message=r'^Could not instantiate type ',
+            )
+            _warnings.filterwarnings(
+                'ignore',
+                category=_sa.exc.SAWarning,
+                message=r'^Skipped unsupported '
+                r'reflection of expression-based'
+                r' index ',
+            )
+            _warnings.filterwarnings(
+                'ignore',
+                category=_sa.exc.SAWarning,
+                message=r'^Predicate of partial index ',
+            )
 
             seen = set()
             while True:
                 try:
-                    table = _sa.Table(name, metadata,
-                                      autoload_with=metadata.bind, **kwargs)
+                    table = _sa.Table(
+                        name, metadata, autoload_with=metadata.bind, **kwargs
+                    )
                 except _sa.exc.SAWarning as e:
                     if types is not None:
                         tname = type_name(e)
                         if tname and tname not in seen:
                             stack = [tname]
                             while stack:
                                 try:
                                     types(stack[-1], metadata, symbols)
                                 except _sa.exc.SAWarning as exc:
                                     tname = type_name(exc)
-                                    if tname and tname not in stack and \
-                                            tname not in seen:
+                                    if (
+                                        tname
+                                        and tname not in stack
+                                        and tname not in seen
+                                    ):
                                         stack.append(tname)
                                         continue
                                     raise
                                 else:
                                     seen.add(stack.pop())
                             continue
                     raise
@@ -234,17 +269,17 @@
         result = "%s(%r, %s%s)" % (
             self._symbols['table'],
             _util.unicode(self.sa_table.name),
             self._symbols['meta'],
             args,
         )
         if self.constraints:
-            result = "\n".join((
-                result, '\n'.join(map(repr, sorted(self.constraints)))
-            ))
+            result = "\n".join(
+                (result, '\n'.join(map(repr, sorted(self.constraints))))
+            )
         return result
 
 
 class TableReference(object):
     """
     Referenced table
 
@@ -254,14 +289,15 @@
 
       sa_table (sqlalchemy.Table):
         Table
 
       constraints (list):
         Constraint list
     """
+
     #: Is it a table reference (vs. a table)?
     #:
     #: :Type: bool
     is_reference = True
 
     def __init__(self, varname, table, schema, symbols):
         """
@@ -280,24 +316,26 @@
         self.varname = varname
         self.sa_table = table
         self.constraints = []
         pkg, mod = schema.rsplit('.', 1)
         if not mod.startswith('_'):
             modas = '_' + mod
             symbols.imports[schema] = 'from %s import %s as %s' % (
-                pkg, mod, modas
+                pkg,
+                mod,
+                modas,
             )
             mod = modas
         else:
             symbols.imports[schema] = 'from %s import %s' % (pkg, mod)
         symbols[u'table_%s' % table.name] = "%s.%s" % (mod, varname)
 
 
 class TableCollection(tuple):
-    """ Table collection """
+    """Table collection"""
 
     @classmethod
     def by_names(cls, metadata, names, schemas, symbols, types=None):
         """
         Construct by table names
 
         Parameters:
@@ -317,27 +355,29 @@
             responsible for modifying the symbols and imports *and* the
             dialect's ``ischema_names``. If omitted or ``None``, the reflector
             will always fail on unknown types.
 
         Returns:
           TableCollection: New table collection instance
         """
-        objects = dict((table.sa_table.key, table) for table in [
-            Table.by_name(name, varname, metadata, schemas, symbols,
-                          types=types)
-            for varname, name in names
-        ])
+        objects = dict(
+            (table.sa_table.key, table)
+            for table in [
+                Table.by_name(
+                    name, varname, metadata, schemas, symbols, types=types
+                )
+                for varname, name in names
+            ]
+        )
 
         def map_table(sa_table):
-            """ Map SA table to table object """
+            """Map SA table to table object"""
             if sa_table.key not in objects:
                 varname = sa_table.name
-                if _util.py2 and \
-                        isinstance(varname,
-                                   _util.unicode):  # pragma: no cover
+                if _util.py2 and isinstance(varname, _util.unicode):
                     varname = varname.encode('ascii')
                 objects[sa_table.key] = Table(
                     varname, sa_table, schemas, symbols
                 )
             return objects[sa_table.key]
 
         tables = list(map(map_table, metadata.tables.values()))
@@ -370,16 +410,17 @@
     """
     Find foreign key cycles and break them apart
 
     Parameters:
       metadata (sqlalchemy.MetaData):
         Metadata
     """
+
     def break_cycle(e):
-        """ Break foreign key cycle """
+        """Break foreign key cycle"""
         cycle_keys = set(map(_op.attrgetter('key'), e.cycles))
         cycle_path = [
             (parent, child)
             for parent, child in e.edges
             if parent.key in cycle_keys and child.key in cycle_keys
         ]
         deps = [cycle_path.pop()]
@@ -397,33 +438,40 @@
             raise AssertionError("Could not construct sorted cycle path")
 
         deps = list(map(_op.itemgetter(0), deps))
         first_dep = list(sorted(deps, key=_op.attrgetter('name')))[0]
         while first_dep != deps[-1]:
             deps = [deps[-1]] + deps[:-1]
         deps.reverse()
-        logger.debug("Found foreign key cycle: %s", " -> ".join([
-            repr(table.name) for table in deps + [deps[0]]
-        ]))
+        logger.debug(
+            "Found foreign key cycle: %s",
+            " -> ".join([repr(table.name) for table in deps + [deps[0]]]),
+        )
 
         def visit_foreign_key(fkey):
-            """ Visit foreign key """
+            """Visit foreign key"""
             if fkey.column.table == deps[1]:
                 fkey.use_alter = True
                 fkey.constraint.use_alter = True
 
-        _sa.sql.visitors.traverse(deps[0], dict(schema_visitor=True), dict(
-            foreign_key=visit_foreign_key,
-        ))
+        _sa.sql.visitors.traverse(
+            deps[0],
+            dict(schema_visitor=True),
+            dict(
+                foreign_key=visit_foreign_key,
+            ),
+        )
 
     while True:
         try:
             with _warnings.catch_warnings():
-                _warnings.filterwarnings('ignore', category=_sa.exc.SAWarning,
-                                         message=(r'^Cannot correctly sort '
-                                                  r'tables'))
+                _warnings.filterwarnings(
+                    'ignore',
+                    category=_sa.exc.SAWarning,
+                    message=(r'^Cannot correctly sort ' r'tables'),
+                )
 
                 metadata.sorted_tables  # pylint: disable = pointless-statement
         except _sa.exc.CircularDependencyError as e:
             break_cycle(e)
         else:
             break
```

### Comparing `gensaschema-0.6.7/gensaschema/_template.py` & `gensaschema-0.6.8/gensaschema/_template.py`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/gensaschema/_type.py` & `gensaschema-0.6.8/gensaschema/_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
           dialect_name (str):
             Dialect name
 
           symbols (Symbols):
             Symbol table
         """
-        self._ctype = ctype
+        self._ctype = _finalize_type(ctype, dialect_name, symbols)
         self._dialect = dialect_name
         self._symbols = symbols
 
     @classmethod
     def by_column(cls, column, symbols):
         """
         Construct by SA column
@@ -113,15 +113,15 @@
             pass
         else:
             return custom_repr(self._ctype, self._dialect, self._symbols)
 
         mod = self._symbols.types.resolve(self._ctype, self._dialect)
         params = []
 
-        if _have_signature:  # pragma: no cover
+        if _have_signature:
             try:
                 # pylint: disable = no-member
                 sign = _inspect.signature(self._ctype.__init__)
             except (TypeError, ValueError):
                 pass
             else:
                 varargs, kwds = None, False
@@ -136,33 +136,44 @@
                     if value is unset:
                         continue
 
                     if arg.default is not arg.empty and arg.default == value:
                         kwds = arg.kind != arg.POSITIONAL_ONLY
                         continue
                     if isinstance(value, _sa.types.TypeEngine):
-                        rvalue = repr(self.__class__(value, self._dialect,
-                                                     self._symbols))
+                        rvalue = repr(
+                            self.__class__(
+                                value, self._dialect, self._symbols
+                            )
+                        )
                     else:
                         rvalue = repr(value)
 
                     if kwds:
                         params.append('%s=%s' % (arg.name, rvalue))
                     else:
                         params.append(rvalue)
                 if not kwds and varargs is not None:
-                    if _find_class(self._ctype, '__init__') is not \
-                            _sa.types.TypeEngine:
-                        params.extend(list(
-                            map(repr, getattr(self._ctype, varargs.name, ()))
-                        ))
+                    if (
+                        _find_class(self._ctype, '__init__')
+                        is not _sa.types.TypeEngine
+                    ):
+                        params.extend(
+                            list(
+                                map(
+                                    repr,
+                                    getattr(self._ctype, varargs.name, ()),
+                                )
+                            )
+                        )
 
-        else:  # pragma: no cover
+        else:
             try:
                 # pylint: disable = deprecated-method
+                # pylint: disable = no-member
                 spec = _inspect.getargspec(self._ctype.__init__)
             except TypeError:
                 pass
             else:
                 defaults = dict(zip(spec[0][::-1], (spec[3] or ())[::-1]))
                 kwds = False
                 for arg in spec[0][1:]:
@@ -170,35 +181,71 @@
                     if value is unset:
                         continue
 
                     if arg in defaults and defaults[arg] == value:
                         kwds = True
                         continue
                     if isinstance(value, _sa.types.TypeEngine):
-                        rvalue = repr(self.__class__(value, self._dialect,
-                                                     self._symbols))
+                        rvalue = repr(
+                            self.__class__(
+                                value, self._dialect, self._symbols
+                            )
+                        )
                     else:
                         rvalue = repr(value)
                     if kwds:
                         params.append('%s=%s' % (arg, rvalue))
                     else:
                         params.append(rvalue)
                 if not kwds and spec[1] is not None:
-                    if _find_class(self._ctype, '__init__') is not \
-                            _sa.types.TypeEngine:
-                        params.extend(list(
-                            map(repr, getattr(self._ctype, spec[1]))
-                        ))
+                    if (
+                        _find_class(self._ctype, '__init__')
+                        is not _sa.types.TypeEngine
+                    ):
+                        params.extend(
+                            list(map(repr, getattr(self._ctype, spec[1])))
+                        )
 
         params = ', '.join(params)
         if params:
             params = "(%s)" % (params,)
         return "%s.%s%s" % (mod, self._ctype.__class__.__name__, params)
 
 
+def _finalize_type(ctype, dialect, symbols):
+    """
+    Finalize type definitions and modifications
+
+    :TODO: should be generalized at some point in the future.
+    """
+
+    if dialect == 'postgresql':
+        if ctype.__class__.__name__ == 'ENUM':
+            _add_postgres_enum(ctype, symbols)
+
+    return ctype
+
+
+def _add_postgres_enum(ctype, symbols):
+    """Add postgres enum"""
+    if ctype in symbols.types.instance_repr:
+        return
+
+    esymbol = "enum_%s" % (ctype.name,)
+
+    def define(_, symbols):
+        return ["%s = %s.%r" % (esymbol, symbols["type"], ctype)]
+
+    def custom_repr(*_):
+        return esymbol
+
+    symbols.types.defines.append(define)
+    symbols.types.instance_repr[ctype] = custom_repr
+
+
 def _find_class(first_cls, name):
     """
     Find class where a method is defined
 
     Parameters:
       first_cls (type):
         Class to start with
```

### Comparing `gensaschema-0.6.7/gensaschema/_util.py` & `gensaschema-0.6.8/gensaschema/_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,33 +27,33 @@
 """
 __author__ = u"Andr\xe9 Malo"
 
 
 # pylint: disable = redefined-builtin, invalid-name, self-assigning-variable
 try:
     unicode  # pylint: disable = used-before-assignment
-except NameError:  # pragma: no cover
+except NameError:
     unicode = str
-else:  # pragma: no cover
+else:
     unicode = unicode
 
 try:
     bytes  # pylint: disable = used-before-assignment
-except NameError:  # pragma: no cover
+except NameError:
     bytes = str
-else:  # pragma: no cover
+else:
     bytes = bytes
 
 py2 = bytes is str
 
 try:
     cmp  # pylint: disable = used-before-assignment
-except NameError:  # pragma: no cover
+except NameError:
     cmp = lambda a, b: (a > b) - (a < b)
-else:  # pragma: no cover
+else:
     cmp = cmp
 
 
 def find_public(space):
     """
     Determine all public names in space
```

### Comparing `gensaschema-0.6.7/gensaschema/constraints.py` & `gensaschema-0.6.8/gensaschema/constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,45 +40,52 @@
     Parameters:
       *columns:
         Constraint columns
 
       \*\*kwargs:
         Additional arguments
     """
-    columns[0].table.append_constraint(_sa.UniqueConstraint(
-        *columns, **kwargs
-    ))
+    columns[0].table.append_constraint(
+        _sa.UniqueConstraint(*columns, **kwargs)
+    )
 
 
 def PrimaryKey(*columns, **kwargs):  # pylint: disable = invalid-name
     r"""
     Append primary key
 
     Parameters:
       \*columns:
         Constraint columns
 
       \*\*kwargs:
         Additional parameters
     """
-    columns[0].table.append_constraint(_sa.PrimaryKeyConstraint(
-        *columns, **kwargs
-    ))
+    columns[0].table.append_constraint(
+        _sa.PrimaryKeyConstraint(*columns, **kwargs)
+    )
 
 
-def ForeignKey(columns, refcolumns, **kwargs):  # noqa pylint: disable = invalid-name
+def ForeignKey(
+    columns, refcolumns, **kwargs
+):  # noqa pylint: disable = invalid-name
     r"""
     Append foreign key
 
     Parameters:
       columns (sequence):
         Source columns
 
       refcolumns (sequence):
         Referred columns
 
       \*\*kwargs:
         Additional parameters
     """
-    columns[0].table.append_constraint(_sa.ForeignKeyConstraint(
-        [col.name for col in columns], refcolumns, link_to_name=True, **kwargs
-    ))
+    columns[0].table.append_constraint(
+        _sa.ForeignKeyConstraint(
+            [col.name for col in columns],
+            refcolumns,
+            link_to_name=True,
+            **kwargs
+        )
+    )
```

### Comparing `gensaschema-0.6.7/gensaschema.egg-info/PKG-INFO` & `gensaschema-0.6.8/gensaschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensaschema
-Version: 0.6.7
+Version: 0.6.8
 Summary: Static SQLAlchemy Schema Generator
 Home-page: http://opensource.perlig.de/gensaschema/
 Author: André Malo
 Author-email: nd@perlig.de
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gensaschema-0.6.7/gensaschema.egg-info/SOURCES.txt` & `gensaschema-0.6.8/gensaschema.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 docs/userdoc/_modules/gensaschema/_table.html
 docs/userdoc/_modules/gensaschema/_template.html
 docs/userdoc/_modules/gensaschema/_type.html
 docs/userdoc/_modules/gensaschema/_util.html
 docs/userdoc/_modules/gensaschema/constraints.html
 docs/userdoc/_sources/index.txt
 docs/userdoc/_sources/website_download.txt
-docs/userdoc/_sources/apidoc/cdbx._cdb.txt
-docs/userdoc/_sources/apidoc/cdbx.txt
 docs/userdoc/_sources/apidoc/gensaschema._column.txt
 docs/userdoc/_sources/apidoc/gensaschema._config.txt
 docs/userdoc/_sources/apidoc/gensaschema._constraint.txt
 docs/userdoc/_sources/apidoc/gensaschema._exceptions.txt
 docs/userdoc/_sources/apidoc/gensaschema._meta.txt
 docs/userdoc/_sources/apidoc/gensaschema._schema.txt
 docs/userdoc/_sources/apidoc/gensaschema._symbols.txt
@@ -65,16 +63,14 @@
 docs/userdoc/_static/jquery.cookie.js
 docs/userdoc/_static/language_data.js
 docs/userdoc/_static/minus.png
 docs/userdoc/_static/plus.png
 docs/userdoc/_static/pygments.css
 docs/userdoc/_static/searchtools.js
 docs/userdoc/_static/sphinx_highlight.js
-docs/userdoc/apidoc/cdbx._cdb.html
-docs/userdoc/apidoc/cdbx.html
 docs/userdoc/apidoc/gensaschema._column.html
 docs/userdoc/apidoc/gensaschema._config.html
 docs/userdoc/apidoc/gensaschema._constraint.html
 docs/userdoc/apidoc/gensaschema._exceptions.html
 docs/userdoc/apidoc/gensaschema._meta.html
 docs/userdoc/apidoc/gensaschema._schema.html
 docs/userdoc/apidoc/gensaschema._symbols.html
@@ -102,14 +98,15 @@
 gensaschema.egg-info/PKG-INFO
 gensaschema.egg-info/SOURCES.txt
 gensaschema.egg-info/dependency_links.txt
 gensaschema.egg-info/not-zip-safe
 gensaschema.egg-info/top_level.txt
 tests/__init__.py
 tests/_util.py
+tests/conftest.py
 tests/coverage.txt
 tests/requirements.txt
 tests/integration/__init__.py
 tests/integration/test_schema.py
 tests/integration/test_table.py
 tests/integration/test_type.py
 tests/unit/__init__.py
```

### Comparing `gensaschema-0.6.7/setup.py` & `gensaschema-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/tests/__init__.py` & `gensaschema-0.6.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/tests/_util.py` & `gensaschema-0.6.8/tests/_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,106 +30,121 @@
 import contextlib as _contextlib
 import sys as _sys
 import types as _types
 
 from pytest import skip  # noqa pylint: disable = unused-import
 
 try:
-    from unittest import mock  # pylint: disable = unused-import
+    import mock
 except ImportError:
-    import mock  # noqa
+    from unittest import mock
 
 try:
-    reload
+    reload  # pylint: disable = used-before-assignment
 except NameError:
     # pylint: disable = redefined-builtin
     try:
         from importlib import reload
     except ImportError:
         from imp import reload  # noqa pylint: disable = deprecated-module
 
-unset = object()
+_unset = type("_unset", (object,), {})()  # pylint: disable=invalid-name
+
+
+# pylint: disable = useless-object-inheritance
 
 
 class Bunch(object):
-    """ Bunch object - represent all init kwargs as attributes """
+    """Bunch object"""
 
-    def __init__(self, **kw):
-        """ Initialization """
-        self.__dict__.update(kw)
+    def __init__(self, **kwargs):
+        self.__dict__.update(kwargs)
 
 
 @_contextlib.contextmanager
-def patched_import(what, how=unset):
+def patched_import(what, how=_unset):
     """
     Context manager to mock an import statement temporarily
 
     :Parameters:
       `what` : ``str``
         Name of the module to mock
 
       `how` : any
         How should it be replaced? If omitted or `unset`, a new MagicMock
         instance is created. The result is yielded as context.
     """
+    # basically stolen from opensource.perlig.de/tdi/
+
     class_types = (type,)
     if str is bytes:
         # pylint: disable = no-member
         class_types += (_types.ClassType,)
 
+    # pylint: disable = unnecessary-lambda-assignment
     _is_exc = lambda obj: isinstance(obj, BaseException) or (
         isinstance(obj, (type, class_types))
         and issubclass(obj, BaseException)
     )
 
     class FinderLoader(object):
-        """ Finder / Loader for meta path """
+        """Finder / Loader for meta path"""
 
         def __init__(self, fullname, module):
             self.module = module
             self.name = fullname
-            extra = '%s.' % fullname
+            extra = "%s." % fullname
             for key in list(_sys.modules):
                 if key.startswith(extra):
                     del _sys.modules[key]
             if fullname in _sys.modules:
                 del _sys.modules[fullname]
 
+        def find_spec(self, name, path=None, target=None):
+            """Find spec (Python 3.10+)"""
+            # pylint: disable = unused-argument
+            if name != self.name:
+                return None
+
+            from importlib import util
+
+            return util.spec_from_loader(name, self)
+
         def find_module(self, fullname, path=None):
-            """ Find the module """
+            """Find the module"""
             # pylint: disable = unused-argument
             if fullname == self.name:
                 return self
             return None
 
         def load_module(self, fullname):
-            """ Load the module """
+            """Load the module"""
             if _is_exc(self.module):
                 raise self.module
             _sys.modules[fullname] = self.module
             return self.module
 
     realmodules = _sys.modules.copy()
     try:
-        obj = FinderLoader(what, mock.MagicMock() if how is unset else how)
+        obj = FinderLoader(what, mock.MagicMock() if how is _unset else how)
         realpath = _sys.meta_path[:]
         try:
             _sys.meta_path[:] = [obj] + realpath
-            old, parts = unset, what.rsplit('.', 1)
+            old, parts = _unset, what.rsplit(".", 1)
             if len(parts) == 2:
                 parent, base = parts[0], parts[1]
                 if parent in _sys.modules:
                     parent = _sys.modules[parent]
                     if hasattr(parent, base):
                         old = getattr(parent, base)
                         setattr(parent, base, obj.module)
             try:
                 yield obj.module
             finally:
-                if old is not unset:
+                if old is not _unset:
                     setattr(parent, base, old)
         finally:
             _sys.meta_path[:] = realpath
     finally:
         _sys.modules.clear()
         _sys.modules.update(realmodules)
 
@@ -145,45 +160,58 @@
     :Return: The decoded string
     :Rtype: ``unicode``
     """
     return value.encode('ascii').decode('unicode_escape')
 
 
 class badstr(object):  # pylint: disable = invalid-name
-    """ bad string """
+    """bad string"""
+
     def __str__(self):
         raise RuntimeError("yo")
+
+
 badstr = badstr()
 
 
 class badbytes(object):  # pylint: disable = invalid-name
-    """ bad bytes """
+    """bad bytes"""
+
     def __bytes__(self):
         raise RuntimeError("yoyo")
+
     if str is bytes:
         __str__ = __bytes__
+
+
 badbytes = badbytes()
 
 
 class badbool(object):  # pylint: disable = invalid-name
-    """ bad bool """
+    """bad bool"""
+
     def __bool__(self):
         raise RuntimeError("yoyo")
+
     if str is bytes:
         __nonzero__ = __bool__
+
+
 badbool = badbool()
 
 
 class baditer(object):  # pylint: disable = invalid-name
-    """ bad iter """
+    """bad iter"""
+
     def __init__(self, *what):
         self._what = iter(what)
 
     def __iter__(self):
         return self
 
     def __next__(self):
         for item in self._what:
             if isinstance(item, Exception):
                 raise item
             return item
+
     next = __next__
```

### Comparing `gensaschema-0.6.7/tests/integration/__init__.py` & `gensaschema-0.6.8/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `gensaschema-0.6.7/tests/integration/test_table.py` & `gensaschema-0.6.8/tests/integration/test_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,28 +37,33 @@
 
 # pylint: disable = invalid-name
 
 sa_version = tuple(map(int, _sa.__version__.split('.')[:3]))
 
 
 def test_table(tmpdir):
-    """ _table.Table() works as expected """
+    """_table.Table() works as expected"""
     tmpdir = str(tmpdir)
     filename = _os.path.join(tmpdir, 'tabletest.db')
 
     db = _sa.create_engine('sqlite:///%s' % (filename,)).connect()
     meta = _meta.BoundMetaData(db)
     with db.begin():
-        db.execute(_sa.text("""
+        db.execute(
+            _sa.text(
+                """
             CREATE TABLE stocks
             (date DATE, trans text, symbol varchar(12), qty real, price real,
             primary key (date))
-        """))
-    table = _table.Table.by_name('main.stocks', 'STOCKS', meta, {},
-                                 _symbols.Symbols())
+        """
+            )
+        )
+    table = _table.Table.by_name(
+        'main.stocks', 'STOCKS', meta, {}, _symbols.Symbols()
+    )
 
     expected = (
         "T(u'stocks', m,\n"
         "    C('date', t.DATE%(nullable)s),\n"
         "    C('trans', t.TEXT),\n"
         "    C('symbol', t.VARCHAR(12)),\n"
         "    C('qty', t.REAL),\n"
```

### Comparing `gensaschema-0.6.7/tests/integration/test_type.py` & `gensaschema-0.6.8/tests/integration/test_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from gensaschema import _type
 
 # pylint: disable = protected-access
 
 
 def test_find_class():
-    """ _find_class() works as expected """
+    """_find_class() works as expected"""
     if _sa is None or _mysql is None:
         skip("SA not installed")
 
     assert _type._find_class(_sa.Unicode, '__init__')
     assert _type._find_class(_sa.Unicode(255), '__init__')
     assert _type._find_class(_mysql.DATE, '__init__')
     assert _type._find_class(_mysql.ENUM('a', 'b'), '__init__')
```

### Comparing `gensaschema-0.6.7/tests/requirements.txt` & `gensaschema-0.6.8/tests/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # Requirements file for tests
 
-pytest == 7.2.0; python_version >= '3.7'
+pytest == 7.4.0; python_version >= '3.7'
 pytest == 7.0.1; python_version == '3.6'
-pytest < 6.2.0; python_version == '3.5'
-pytest < 5.0.0; python_version < '3.5'
+pytest < 5.0.0; python_version < '3.6'
 
-pytest-cov == 4.0.0; python_version >= '3.6'
+pytest-cov == 4.1.0; python_version >= '3.7'
+pytest-cov == 4.0.0; python_version == '3.6'
 pytest-cov == 2.12.1; python_version < '3.6'
 
-coverage == 7.0.4; python_version >= '3.7'
+coverage == 7.2.7; python_version >= '3.7'
 coverage == 6.2.0; python_version == '3.6'
 coverage == 5.5; python_version < '3.6'
 
-pytest-mock == 3.10.0; python_version >= '3.7'
+pytest-mock == 3.11.1; python_version >= '3.7'
 pytest-mock == 3.6.1; python_version == '3.6'
-pytest-mock == 1.12.1; python_version < '3.5'
+pytest-mock == 1.12.1; python_version < '3.6'
+
+psycopg2 ~= 2.9.6; python_version >= '3.6'
+psycopg2 ~= 2.8.6; python_version < '3.6'
+
+docker ~= 6.1.3; python_version >= '3.7'
+docker ~= 5.0.3; python_version == '3.6'
+docker ~= 4.4.4; python_version < '3.6'
```

### Comparing `gensaschema-0.6.7/tests/unit/__init__.py` & `gensaschema-0.6.8/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: ascii -*-
-r"""
+u"""
 :Copyright:
 
  Copyright 2014 - 2023
  Andr\xe9 Malo or his licensors, as applicable
 
 :License:
```

### Comparing `gensaschema-0.6.7/tests/unit/test_column.py` & `gensaschema-0.6.8/tests/unit/test_column.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from .. import _util as _test
 
 # pylint: disable = invalid-name
 
 
 def test_ServerDefault():
-    """ _column.ServerDefault() works as expected """
+    """_column.ServerDefault() works as expected"""
     default = _test.Bunch(for_update=None, arg=12)
     symbols = dict(default='DEF')
 
     if bytes is str:
         inst = _column.ServerDefault(default, symbols)
         assert repr(inst) == "DEF(u'12')"
 
@@ -56,60 +56,73 @@
         assert repr(inst) == "DEF('12')"
 
         default.for_update = u'lalala'
         assert repr(inst) == "DEF('12', for_update=True)"
 
 
 def test_Column():
-    """ _column.Column() works as expected """
+    """_column.Column() works as expected"""
     meta = _sa.MetaData()
     table = _sa.Table(
-        u'mytable', meta,
-        _sa.Column(u'Lala', _mysql.VARCHAR(255), nullable=True,
-                   server_default='""'),
-        _sa.Column(u'lolo', _mysql.INTEGER, primary_key=True,
-                   autoincrement=False),
+        u'mytable',
+        meta,
+        _sa.Column(
+            u'Lala', _mysql.VARCHAR(255), nullable=True, server_default='""'
+        ),
+        _sa.Column(
+            u'lolo', _mysql.INTEGER, primary_key=True, autoincrement=False
+        ),
     )
     meta.bind = _test.Bunch(dialect=_test.Bunch(name='mysql'))
     symbols = _symbols.Symbols(symbols=dict(type="TT"))
 
     inst = _column.Column.from_sa(table.c.Lala, symbols)
     if bytes is str:
-        assert repr(inst) == ('C(\'Lala\', TT.VARCHAR(255), '
-                              'server_default=D(u\'""\'))')
+        assert repr(inst) == (
+            'C(\'Lala\', TT.VARCHAR(255), ' 'server_default=D(u\'""\'))'
+        )
     else:
-        assert repr(inst) == ('C(\'Lala\', TT.VARCHAR(255), '
-                              'server_default=D(\'""\'))')
+        assert repr(inst) == (
+            'C(\'Lala\', TT.VARCHAR(255), ' 'server_default=D(\'""\'))'
+        )
 
     inst = _column.Column.from_sa(table.c.lolo, symbols)
-    assert repr(inst) == ("C('lolo', TT.INTEGER, nullable=False, "
-                          "autoincrement=False)")
+    assert repr(inst) == (
+        "C('lolo', TT.INTEGER, nullable=False, " "autoincrement=False)"
+    )
 
 
 def test_Column_identity():
-    """ _column.Column() works ith identity """
+    """_column.Column() works ith identity"""
     if not getattr(_sa, 'Identity', None):
         skip("Identity not defined")
 
     meta = _sa.MetaData()
     table = _sa.Table(
-        u'mytable', meta,
+        u'mytable',
+        meta,
         _sa.Column(u'Lala', _mysql.VARCHAR(255), _sa.Identity()),
-        _sa.Column(u'lolo', _mysql.INTEGER, primary_key=True,
-                   autoincrement=False),
+        _sa.Column(
+            u'lolo', _mysql.INTEGER, primary_key=True, autoincrement=False
+        ),
     )
     meta.bind = _test.Bunch(dialect=_test.Bunch(name='mysql'))
     symbols = _symbols.Symbols(symbols=dict(type="TT"))
 
     inst = _column.Column.from_sa(table.c.Lala, symbols)
     if bytes is str:
-        assert repr(inst) == ('C(\'Lala\', TT.VARCHAR(255), '
-                              'nullable=False, '
-                              'server_default=_sa.Identity())')
+        assert repr(inst) == (
+            'C(\'Lala\', TT.VARCHAR(255), '
+            'nullable=False, '
+            'server_default=_sa.Identity())'
+        )
     else:
-        assert repr(inst) == ('C(\'Lala\', TT.VARCHAR(255), '
-                              'nullable=False, '
-                              'server_default=_sa.Identity())')
+        assert repr(inst) == (
+            'C(\'Lala\', TT.VARCHAR(255), '
+            'nullable=False, '
+            'server_default=_sa.Identity())'
+        )
 
     inst = _column.Column.from_sa(table.c.lolo, symbols)
-    assert repr(inst) == ("C('lolo', TT.INTEGER, nullable=False, "
-                          "autoincrement=False)")
+    assert repr(inst) == (
+        "C('lolo', TT.INTEGER, nullable=False, " "autoincrement=False)"
+    )
```

### Comparing `gensaschema-0.6.7/tests/unit/test_config.py` & `gensaschema-0.6.8/tests/unit/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,55 +32,68 @@
 
 from gensaschema import _config
 
 # pylint: disable = protected-access
 
 
 def fixture(name):
-    """ Find fixture """
+    """Find fixture"""
     return _os.path.join(
         _os.path.dirname(_os.path.normpath(_os.path.abspath(__file__))),
         'fixtures',
         name,
     )
 
 
 def test_init():
-    """ Config initialization works as expected """
+    """Config initialization works as expected"""
     inst = _config.Config.from_file(fixture('config1.schema'))
     assert inst.tables == [
         ('Yo', 'Yo'),
         ('some', 'table'),
         ('somethingElse', 'somethingElse'),
         ('y', 'x.y'),
         ('a', 'b.c'),
     ]
     assert inst.schemas == {'foo': 'bar'}
     assert inst._lines == [
-        '# This is a comment. I love comments.\n', '#\n', '\n', 'Yo\n',
-        'some = table\n', 'somethingElse\n', 'x.y\n', 'a = b.c\n', '\n',
-        '[schemas]\n', 'foo = bar\n',
+        '# This is a comment. I love comments.\n',
+        '#\n',
+        '\n',
+        'Yo\n',
+        'some = table\n',
+        'somethingElse\n',
+        'x.y\n',
+        'a = b.c\n',
+        '\n',
+        '[schemas]\n',
+        'foo = bar\n',
     ]
 
 
 def test_dump():
-    """ Config dumps properly """
-    inst = _config.Config(tables=[
-        ('Yo', 'Yo'),
-        ('some', 'table'),
-        ('somethingElse', 'somethingElse'),
-        ('y', 'x.y'),
-        ('a', 'b.c'),
-    ], schemas={'foo': 'bar'})
+    """Config dumps properly"""
+    inst = _config.Config(
+        tables=[
+            ('Yo', 'Yo'),
+            ('some', 'table'),
+            ('somethingElse', 'somethingElse'),
+            ('y', 'x.y'),
+            ('a', 'b.c'),
+        ],
+        schemas={'foo': 'bar'},
+    )
 
     fp = _tempfile.TemporaryFile(mode="w+")
     inst.dump(fp)
     fp.seek(0, 0)
 
-    assert fp.read() == """
+    assert (
+        fp.read()
+        == """
 # This is a comment. I love comments.
 #
 # This files contains table names, one per line
 # Comments and empty lines are ignored
 #
 # If the table name contains a dot, the first part is treated as
 # schema name.
@@ -96,9 +109,11 @@
 some = table
 somethingElse = somethingElse
 y = x.y
 a = b.c
 
 [schemas]
 foo = bar
-    """.strip() + '\n'
+    """.strip()
+        + '\n'
+    )
     fp.close()
```

### Comparing `gensaschema-0.6.7/tests/unit/test_template.py` & `gensaschema-0.6.8/tests/unit/test_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,39 +31,48 @@
 
 from gensaschema import _template
 
 # pylint: disable = invalid-name, protected-access
 
 
 def test_Template_init():
-    """ _template.Template initializes properly """
-    inst = _template.Template("""
+    """_template.Template initializes properly"""
+    inst = _template.Template(
+        """
         lalala
 
          lolo
-    """)
+    """
+    )
     assert inst._template == 'lalala\n\n lolo'
 
-    inst = _template.Template("""
+    inst = _template.Template(
+        """
         lalala
 
          lolo
-    """, dedent=False)
+    """,
+        dedent=False,
+    )
     assert inst._template == '\n        lalala\n\n         lolo'
 
-    inst = _template.Template("""
+    inst = _template.Template(
+        """
         lalala
 
          lolo
-    """, dedent=False, rstrip=False)
+    """,
+        dedent=False,
+        rstrip=False,
+    )
     assert inst._template == '\n        lalala\n\n         lolo\n    '
 
 
 def test_Template_expand():
-    """ _template.Template().expand() works as expected """
+    """_template.Template().expand() works as expected"""
     inst = _template.Template("""%s xxx %d""")
     assert inst.expand() == '%s xxx %d'
     assert inst.expand('blah', 12) == 'blah xxx 12'
     with raises(TypeError):
         inst.expand(foo='blah', bar=12)
 
     inst = _template.Template("""%(foo)s xxx %(bar)d""")
```

### Comparing `gensaschema-0.6.7/tests/unit/test_type.py` & `gensaschema-0.6.8/tests/unit/test_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,20 @@
 
 from gensaschema import _type
 
 # pylint: disable = protected-access
 
 
 def test_find_class():
-    """ _find_class() works as expected """
+    """_find_class() works as expected"""
+
     class Sub(_type.Type):
-        """ Subtype """
+        """Subtype"""
+
         def __repr__(self):
-            """ repr"""
+            """repr"""
             return "Sub"
 
     assert _type._find_class(_type.Type, '__init__') is _type.Type
     assert _type._find_class(_type.Type, '__repr__') is _type.Type
     assert _type._find_class(Sub, '__init__') is _type.Type
     assert _type._find_class(Sub, '__repr__') is Sub
```

### Comparing `gensaschema-0.6.7/tests/unit/test_util.py` & `gensaschema-0.6.8/tests/unit/test_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 from gensaschema import _util
 
 # pylint: disable = protected-access
 
 
 def test_find_public_symbols():
-    """ find_public finds all non underscored symbols """
+    """find_public finds all non underscored symbols"""
     mod = _types.ModuleType('lala')
     mod.a = 1
     mod._b = 2
 
     assert _util.find_public(vars(mod)) == ['a']
 
 
 def test_find_public_all():
-    """ find_public passes __all__ """
+    """find_public passes __all__"""
     mod = _types.ModuleType('lala')
     mod.__all__ = ['_b', 'c']
 
     assert _util.find_public(vars(mod)) == ['_b', 'c']
```

