# Comparing `tmp/shibuya-2023.6.8.tar.gz` & `tmp/shibuya-2023.7.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shibuya-2023.6.8.tar", last modified: Thu Jun  8 06:30:56 2023, max compression
+gzip compressed data, was "shibuya-2023.7.11.tar", last modified: Tue Jul 11 16:22:43 2023, max compression
```

## Comparing `shibuya-2023.6.8.tar` & `shibuya-2023.7.11.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.204380 shibuya-2023.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-08 06:30:41.000000 shibuya-2023.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 06:30:41.000000 shibuya-2023.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-08 06:30:56.204380 shibuya-2023.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-08 06:30:41.000000 shibuya-2023.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-08 06:30:41.000000 shibuya-2023.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 06:30:56.204380 shibuya-2023.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 06:30:41.000000 shibuya-2023.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.196380 shibuya-2023.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.200380 shibuya-2023.6.8/src/shibuya/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.200380 shibuya-2023.6.8/src/shibuya/css/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/css/dark.css
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/css/light.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.196380 shibuya-2023.6.8/src/shibuya/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.200380 shibuya-2023.6.8/src/shibuya/theme/shibuya/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.200380 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/nav-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/nav-versions.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/page-searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/site-foot.html
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/site-head.html
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/components/variables.html
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.204380 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/extra-head.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/opengraph.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/page-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/sidebar-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/webfonts.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.204380 shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/repo-stats.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.204380 shibuya-2023.6.8/src/shibuya/theme/shibuya/static/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/static/print.css
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    52043 2023-06-08 06:30:47.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/static/shibuya.css
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-08 06:30:45.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/static/shibuya.js
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 06:30:41.000000 shibuya-2023.6.8/src/shibuya/theme/shibuya/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:30:56.200380 shibuya-2023.6.8/src/shibuya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-08 06:30:56.000000 shibuya-2023.6.8/src/shibuya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-08 06:30:56.000000 shibuya-2023.6.8/src/shibuya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:30:56.000000 shibuya-2023.6.8/src/shibuya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 06:30:56.000000 shibuya-2023.6.8/src/shibuya.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 06:30:56.000000 shibuya-2023.6.8/src/shibuya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 06:30:56.000000 shibuya-2023.6.8/src/shibuya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.660593 shibuya-2023.7.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-11 16:22:23.000000 shibuya-2023.7.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 16:22:23.000000 shibuya-2023.7.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-11 16:22:43.660593 shibuya-2023.7.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-11 16:22:23.000000 shibuya-2023.7.11/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-11 16:22:23.000000 shibuya-2023.7.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:22:43.660593 shibuya-2023.7.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 16:22:23.000000 shibuya-2023.7.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.648593 shibuya-2023.7.11/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.652593 shibuya-2023.7.11/src/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.652593 shibuya-2023.7.11/src/shibuya/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/css/dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/css/light.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.648593 shibuya-2023.7.11/src/shibuya/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.656593 shibuya-2023.7.11/src/shibuya/theme/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.656593 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/nav-languages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/nav-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/nav-versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/site-foot.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/site-head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/components/variables.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.656593 shibuya-2023.7.11/src/shibuya/theme/shibuya/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/extensions/buysellads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.660593 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/extra-head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/globaltoc-above.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/opengraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/page-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/webfonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.660593 shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/repo-stats.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.660593 shibuya-2023.7.11/src/shibuya/theme/shibuya/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/static/print.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    66608 2023-07-11 16:22:30.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/static/shibuya.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-11 16:22:28.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/static/shibuya.js
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 16:22:23.000000 shibuya-2023.7.11/src/shibuya/theme/shibuya/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:22:43.652593 shibuya-2023.7.11/src/shibuya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-11 16:22:43.000000 shibuya-2023.7.11/src/shibuya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-11 16:22:43.000000 shibuya-2023.7.11/src/shibuya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:22:43.000000 shibuya-2023.7.11/src/shibuya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 16:22:43.000000 shibuya-2023.7.11/src/shibuya.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:22:43.000000 shibuya-2023.7.11/src/shibuya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 16:22:43.000000 shibuya-2023.7.11/src/shibuya.egg-info/top_level.txt
```

### Comparing `shibuya-2023.6.8/LICENSE` & `shibuya-2023.7.11/LICENSE`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/PKG-INFO` & `shibuya-2023.7.11/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2023.6.8
+Version: 2023.7.11
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2023.6.8/README.md` & `shibuya-2023.7.11/README.md`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/pyproject.toml` & `shibuya-2023.7.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/__init__.py` & `shibuya-2023.7.11/src/shibuya/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     create_edit_source_link,
 )
 from ._sphinx import (
     WrapperPostTransform,
     WrapLineFormatter,
 )
 
-__version__ = "2023.6.8"
+__version__ = "2023.7.11"
 
 shibuya_version = __version__
 
 THEME_PATH = (Path(__file__).parent / "theme" / "shibuya").resolve()
 
 
 def _add_version(name: str):
```

### Comparing `shibuya-2023.6.8/src/shibuya/_sphinx.py` & `shibuya-2023.7.11/src/shibuya/_sphinx.py`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/context.py` & `shibuya-2023.7.11/src/shibuya/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import Dict, Any
 from pathlib import Path
+import xml.etree.ElementTree as ET
+
 
 CSS_PATH = Path(__file__).parent / "css"
 
 
 def css_to_dict(filename: str):
     filepath = (CSS_PATH / filename).resolve()
     rv = {}
@@ -24,42 +26,50 @@
         return re.sub(r'index\.html$', '', pageurl)
     if builder == 'dirhtml' and pageurl.endswith('.html'):
         return re.sub(r'\.html$', '/', pageurl)
     return pageurl
 
 
 def normalize_toc(toc: str):
-    toc = re.sub(r'^<ul>\n<li>.*?</a>', '', toc)
-    toc = re.sub(r'</li>\n</ul>$', '', toc)
+    if not toc:
+        return toc
+
+    root = ET.fromstring(toc)
+    if len(root) != 1:
+        return toc
+
+    child = root[0]
+    if len(child) == 2 and child[1].tag == "ul":
+        return ET.tostring(child[1]).decode("utf-8")
     return toc
 
 
 def create_edit_source_link(context: Dict[str, Any]):
     source_type = context.get("source_type")
     if not source_type:
         source_type = _normalize_readthedocs_context(context)
 
     source_user = context.get("source_user")
     source_repo = context.get("source_repo")
-    source_docs_path = context.get("source_docs_path", "docs")
+    source_docs_path = context.get("source_docs_path", "/docs/")
     source_edit_template = context.get("source_edit_template")
 
     def edit_source_link(filename: str) -> str:
         if source_edit_template:
             return source_edit_template.format(filename)
 
         if not source_user or not source_repo:
             return
 
         if source_type == "github":
-            return f"https://github.com/{source_user}/{source_repo}/blob/master/{source_docs_path}/{filename}"
+            return f"https://github.com/{source_user}/{source_repo}/blob/master{source_docs_path}{filename}"
         elif source_type == "gitlab":
-            return f"https://gitlab.com/{source_user}/{source_repo}/-/blob/master/{source_docs_path}/{filename}"
+            return f"https://gitlab.com/{source_user}/{source_repo}/-/blob/master{source_docs_path}{filename}"
         elif source_type == "bitbucket":
-            return  f"https://bitbucket.org/{source_user}/{source_repo}/src/master/{source_docs_path}/{filename}"
+            return  f"https://bitbucket.org/{source_user}/{source_repo}/src/master{source_docs_path}{filename}"
 
     return edit_source_link
 
 
 def _normalize_readthedocs_context(context: Dict[str, Any]):
     if context.get("display_github"):
         source_type = "github"
```

### Comparing `shibuya-2023.6.8/src/shibuya/css/base.css` & `shibuya-2023.7.11/src/shibuya/css/base.css`

 * *Files 15% similar despite different names*

```diff
@@ -4,11 +4,11 @@
   --sy-f-heading: var(--sy-f-sys), var(--sy-f-cjk), sans-serif;
   --sy-f-text: var(--sy-f-sys), var(--sy-f-cjk), sans-serif;
   --sy-f-mono: Menlo, Monaco, Consolas, "Courier New", monospace;
   --sy-c-divider: rgba(var(--sy-rc-text), 0.1);
   --sy-c-divider-weak: rgba(var(--sy-rc-text), 0.05);
   --sy-c-border: rgba(var(--sy-rc-text), 0.14);
   --sy-s-banner-height: 0rem;
-  --sy-s-navbar-height: 4rem;
+  --sy-s-navbar-height: 56px;
   --sy-s-offset-top: calc(var(--sy-s-navbar-height) + var(--sy-s-banner-height));
   --sy-c-link: rgb(var(--sy-rc-theme));
 }
```

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/base.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/base.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/components/navigation.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/components/navigation.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/components/site-foot.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/components/site-foot.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/components/site-head.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/components/site-head.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-{%- from "components/nav-links.html" import renderNavLinks with context -%}
-
 {%- macro render_logo(src, classname) -%}
   {%- if src and src.startswith(('https://', 'http://')) -%}
     <img class="{{ classname }}" src="{{ src }}" alt="{{ project }}" height="28" />
   {%- elif src -%}
     <img class="{{ classname }}" src="{{ pathto(src, 1) }}" alt="{{ project }}" height="28" />
   {%- elif logo_url -%}
     <img class="{{ classname }}" src="{{ logo_url }}" alt="{{ project }}" height="28" />
   {%- endif -%}
 {%- endmacro -%}
 
 <div class="sy-head">
   <div class="sy-head-blur"></div>
   <div class="sy-head-inner sy-container mx-auto">
-    <div class="sy-head-links flex items-center">
-      <div class="md:hidden flex items-center">
-        <button class="hamburger js-menu mr-3" aria-label="Menu" type="button" aria-controls="lside" aria-expanded="false">
-          <span class="hamburger_1"></span>
-          <span class="hamburger_2 -translate-x-2"></span>
-          <span class="hamburger_3 -translate-x-1"></span>
-        </button>
-      </div>
-      <a class="sy-head-brand" href="{% if theme_logo_target %}{{ theme_logo_target }}{% else %}{{ pathto(root_doc) }}{% endif %}">
-        {{ render_logo(theme_light_logo, 'light-logo') }}
-        {{ render_logo(theme_dark_logo, 'dark-logo') }}
-        <strong>{{ project }}</strong>
-      </a>
-      {%- if theme_nav_links -%}
-      <nav class="sy-head-nav ml-4 hidden md:block">
-        {{ renderNavLinks(theme_nav_links, True) }}
+    <a class="sy-head-brand mr-4" href="{% if theme_logo_target %}{{ theme_logo_target }}{% else %}{{ pathto(root_doc) }}{% endif %}">
+      {{ render_logo(theme_light_logo, 'light-logo') }}
+      {{ render_logo(theme_dark_logo, 'dark-logo') }}
+      <strong>{{ project }}</strong>
+    </a>
+    <div class="sy-head-links" id="_sy_links">
+      <nav class="sy-head-nav">
+        {%- if theme_nav_links -%}
+          {% include "components/nav-links.html" %}
+        {%- endif -%}
       </nav>
-      {%- endif -%}
-    </div>
-    <div class="sy-head-actions flex gap-2 items-center print:hidden">
-      {% include "components/nav-versions.html" %}
-      <div class="hidden md:block">
+      <div class="sy-head-extra flex gap-2 items-center print:hidden">
+        {% include "components/nav-versions.html" %}
         {%- include "components/searchbox.html" %}
+        {% include "components/nav-languages.html" %}
+        <div class="flex gap-2 items-center">
+          {%- if theme_github_url %}
+            <a class="flex items-center ml-1" href="{{ theme_github_url }}" aria-label="GitHub">
+              <i class="i-icon github"></i>
+            </a>
+          {%- endif %}
+          {%- if theme_discord_url %}
+            <a class="flex items-center ml-1" href="{{ theme_discord_url }}" aria-label="Discord">
+              <i class="i-icon discord"></i>
+            </a>
+          {%- endif %}
+        </div>
       </div>
-      {%- if theme_github_url %}
-        <a class="flex items-center ml-1" href="{{ theme_github_url }}" aria-label="GitHub">
-          <i class="i-icon github"></i>
-        </a>
-      {%- endif %}
-      <button class="js-theme theme-switch flex items-center ml-1" data-aria-light="{{ _('Switch to dark mode') }}" data-aria-dark="{{ _('Switch to light mode') }}">
+    </div>
+    <div class="sy-head-actions flex items-center ml-3 shrink-0 print:hidden">
+      <button class="js-theme theme-switch flex items-center" data-aria-light="{{ _('Switch to dark mode') }}" data-aria-dark="{{ _('Switch to light mode') }}">
         <i class="i-icon theme-icon"></i>
       </button>
-      {% if display_toc %}
-        <button class="js-menu xl:hidden flex items-center ml-1" aria-label="Show table of contents" type="button" aria-controls="rside" aria-expanded="false">
-          <i class="i-icon outdent"></i>
+      <div class="md:hidden flex items-center ml-3">
+        <button class="hamburger js-menu" aria-label="Menu" type="button" aria-controls="_sy_links" aria-expanded="false">
+          <span class="hamburger_1"></span>
+          <span class="hamburger_2 -translate-x-2"></span>
+          <span class="hamburger_3 -translate-x-1"></span>
         </button>
-      {%- endif %}
+      </div>
     </div>
   </div>
 </div>
```

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/components/variables.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/components/variables.html`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 @media (prefers-color-scheme: light) {
   :root {
     {{ declare_css_vars(shibuya_light_css_variables, theme_light_css_variables) }}
   }
 }
 @media (prefers-color-scheme: dark) {
   :root {
-    {{ declare_css_vars(shibuya_dark_css_variables, theme_light_css_variables) }}
+    {{ declare_css_vars(shibuya_dark_css_variables, theme_dark_css_variables) }}
   }
 }
 html.light {
   {{ declare_css_vars(shibuya_light_css_variables, theme_light_css_variables) }}
 }
 html.dark {
-  {{ declare_css_vars(shibuya_dark_css_variables, theme_light_css_variables) }}
+  {{ declare_css_vars(shibuya_dark_css_variables, theme_dark_css_variables) }}
 }
 </style>
```

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/layout.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/layout.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,16 @@
 {%- extends "base.html" -%}
-{%- from "components/nav-links.html" import renderNavLinks with context -%}
 
 {%- block document -%}
 <div class="document">
   {%- include "partials/banner.html" -%}
   {%- block header -%}
     {% include "components/site-head.html" with context %}
   {%- endblock -%}
 
-  <aside id="lside" class="sy-lside md:hidden">
-    {%- block mobile_navbar -%}
-    <div class="sy-lside-inner md:sticky">
-      <div class="sy-lside-top pt-3 pb-3 px-6">
-        <div class="pt-3">
-          {%- include "components/page-searchbox.html" %}
-        </div>
-        {%- if theme_nav_links -%}
-        <div class="pt-3">
-          {{ renderNavLinks(theme_nav_links) }}
-        </div>
-        {%- endif -%}
-      </div>
-    </div>
-    {%- endblock %}
-  </aside>
-
   <div class="sy-container mx-auto body">
     <main class="sy-content mx-auto pt-12 px-6 xl:px-12 break-words">
       <article class="yue" role="main">
         {% block body %}{% endblock %}
       </article>
     </main>
   </div>
```

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/page.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/page.html`

 * *Files 17% similar despite different names*

```diff
@@ -13,48 +13,43 @@
   {% set dark_code = False %}
 {%- endif -%}
 
 {% block body %}
 <div class="sy-page sy-container flex mx-auto">
   <aside id="lside" class="sy-lside md:w-64 md:shrink-0 print:hidden">
     <div class="sy-lside-inner md:sticky">
-      <div class="sy-lside-top md:hidden pt-3 pb-3 px-6">
-        <div class="pt-3">
-          {%- include "components/page-searchbox.html" %}
-        </div>
-        {%- if theme_nav_links -%}
-        <div class="pt-3">
-          {{ renderNavLinks(theme_nav_links) }}
-        </div>
-        {%- endif -%}
-      </div>
       <div class="sy-scrollbar p-6">
-        {%- include "partials/sidebar-links.html" %}
+        {%- include "partials/globaltoc-above.html" %}
         <div class="globaltoc">
           {{ toctree(collapse=False, titles_only=True, includehidden=True) }}
         </div>
       </div>
+      {% if READTHEDOCS %}
+      <div class="sy-lside-bottom px-6" id="readthedocs-embed-flyout"></div>
+      {% endif %}
     </div>
   </aside>
+  <div class="lside-overlay js-menu" role="button" aria-label="Close left sidebar" aria-controls="lside" aria-expanded="false"></div>
   <aside id="rside" class="sy-rside pb-3 w-64 shrink-0 order-last">
     <button class="rside-close js-menu xl:hidden" aria-label="Close Table of Contents" type="button" aria-controls="rside" aria-expanded="false">
       <i class="i-icon close"></i>
     </button>
     <div class="sy-scrollbar px-6 xl:top-16 xl:sticky xl:pl-0 pt-6 pb-4">
       {%- if sidebars %}
         {%- for sidebartemplate in sidebars %}
           {%- include sidebartemplate %}
         {%- endfor %}
       {%- endif %}
     </div>
   </aside>
   <div class="rside-overlay js-menu" role="button" aria-label="Close Table of Contents" aria-controls="rside" aria-expanded="false"></div>
   <main class="sy-main w-full max-sm:max-w-full print:pt-6">
+    {% include "components/breadcrumbs.html" %}
     <div class="flex flex-col break-words justify-between">
-      <div class="min-w-0 max-w-6xl px-6 pb-6 pt-6 xl:px-12">
+      <div class="min-w-0 max-w-6xl px-6 pb-6 pt-8 xl:px-12">
         <article class="yue{% if dark_code %} dark-code{% endif %}" role="main">
           {% block content %}{{ body }}{% endblock %}
         </article>
         {% include "partials/article-bottom.html" %}
       </div>
       <div class="min-w-0 max-w-6xl px-6 pb-6 xl:pt-6 xl:px-12">
         {% include "components/navigation.html" %}
```

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/partials/opengraph.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/partials/opengraph.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/sidebars/repo-stats.html` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/sidebars/repo-stats.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/static/pygments.css` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/static/pygments.css`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/static/shibuya.js` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/static/shibuya.js`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya/theme/shibuya/theme.conf` & `shibuya-2023.7.11/src/shibuya/theme/shibuya/theme.conf`

 * *Files identical despite different names*

### Comparing `shibuya-2023.6.8/src/shibuya.egg-info/PKG-INFO` & `shibuya-2023.7.11/src/shibuya.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2023.6.8
+Version: 2023.7.11
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2023.6.8/src/shibuya.egg-info/SOURCES.txt` & `shibuya-2023.7.11/src/shibuya.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 src/shibuya/css/light.css
 src/shibuya/theme/shibuya/base.html
 src/shibuya/theme/shibuya/layout.html
 src/shibuya/theme/shibuya/page.html
 src/shibuya/theme/shibuya/search.html
 src/shibuya/theme/shibuya/searchbox.html
 src/shibuya/theme/shibuya/theme.conf
+src/shibuya/theme/shibuya/components/breadcrumbs.html
+src/shibuya/theme/shibuya/components/nav-languages.html
 src/shibuya/theme/shibuya/components/nav-links.html
 src/shibuya/theme/shibuya/components/nav-versions.html
 src/shibuya/theme/shibuya/components/navigation.html
-src/shibuya/theme/shibuya/components/page-searchbox.html
 src/shibuya/theme/shibuya/components/searchbox.html
 src/shibuya/theme/shibuya/components/site-foot.html
 src/shibuya/theme/shibuya/components/site-head.html
 src/shibuya/theme/shibuya/components/variables.html
+src/shibuya/theme/shibuya/extensions/buysellads.html
 src/shibuya/theme/shibuya/partials/article-bottom.html
 src/shibuya/theme/shibuya/partials/banner.html
 src/shibuya/theme/shibuya/partials/extra-head.html
 src/shibuya/theme/shibuya/partials/footer.html
+src/shibuya/theme/shibuya/partials/globaltoc-above.html
 src/shibuya/theme/shibuya/partials/opengraph.html
 src/shibuya/theme/shibuya/partials/page-bottom.html
-src/shibuya/theme/shibuya/partials/sidebar-links.html
 src/shibuya/theme/shibuya/partials/webfonts.html
 src/shibuya/theme/shibuya/sidebars/carbon-ads.html
 src/shibuya/theme/shibuya/sidebars/edit-this-page.html
 src/shibuya/theme/shibuya/sidebars/ethical-ads.html
 src/shibuya/theme/shibuya/sidebars/localtoc.html
 src/shibuya/theme/shibuya/sidebars/repo-stats.html
 src/shibuya/theme/shibuya/static/print.css
```

