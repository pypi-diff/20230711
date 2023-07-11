# Comparing `tmp/yangson-1.4.8.tar.gz` & `tmp/yangson-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yangson-1.4.8.tar", last modified: Mon May 10 13:13:06 2021, max compression
+gzip compressed data, was "yangson-1.4.9.tar", last modified: Thu Jun 10 08:24:55 2021, max compression
```

## Comparing `yangson-1.4.8.tar` & `yangson-1.4.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.774342 yangson-1.4.8/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      201 2021-02-22 08:52:17.000000 yangson-1.4.8/.gitignore
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      572 2021-03-15 14:53:52.000000 yangson-1.4.8/.gitlab-ci.yml
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)        6 2021-02-22 08:52:17.000000 yangson-1.4.8/.python-version
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    35147 2020-12-09 13:53:37.000000 yangson-1.4.8/COPYING
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7650 2020-12-09 13:53:37.000000 yangson-1.4.8/COPYING.LESSER
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      247 2020-12-09 13:53:37.000000 yangson-1.4.8/MANIFEST.in
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      376 2021-05-10 13:11:41.000000 yangson-1.4.8/Makefile
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1559 2021-05-10 13:13:06.774342 yangson-1.4.8/PKG-INFO
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      733 2021-03-19 17:55:55.000000 yangson-1.4.8/README.rst
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.761009 yangson-1.4.8/docs/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7660 2021-03-23 15:58:22.000000 yangson-1.4.8/docs/Makefile
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.764342 yangson-1.4.8/docs/_templates/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      942 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/_templates/donation.html
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3985 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/_templates/donation.svg
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      113 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/_templates/layout.html
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      100 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/advanced.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      107 2020-12-09 13:53:37.000000 yangson-1.4.8/docs/basic.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     4134 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/cmdline.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7720 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/concepts-terms.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    11845 2021-03-01 09:47:59.000000 yangson-1.4.8/docs/conf.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     6205 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/constraint.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     9623 2021-03-22 13:21:43.000000 yangson-1.4.8/docs/datamodel.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    17571 2021-03-13 11:55:47.000000 yangson-1.4.8/docs/datatype.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      335 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/enumerations.rst
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.741009 yangson-1.4.8/docs/examples/
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.764342 yangson-1.4.8/docs/examples/ex1/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      175 2020-12-09 13:53:37.000000 yangson-1.4.8/docs/examples/ex1/example-1.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)       34 2021-03-21 15:55:54.000000 yangson-1.4.8/docs/examples/ex1/example-data.json
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      296 2020-12-09 13:53:37.000000 yangson-1.4.8/docs/examples/ex1/yang-library-ex1.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.764342 yangson-1.4.8/docs/examples/ex2/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      308 2021-03-13 14:55:05.000000 yangson-1.4.8/docs/examples/ex2/example-2-dev.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      728 2021-03-13 14:55:05.000000 yangson-1.4.8/docs/examples/ex2/example-2.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      451 2021-05-10 11:39:19.000000 yangson-1.4.8/docs/examples/ex2/example-data.json
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      255 2021-03-22 16:43:01.000000 yangson-1.4.8/docs/examples/ex2/example-data.yaml
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      963 2021-03-13 14:55:05.000000 yangson-1.4.8/docs/examples/ex2/yang-library-ex2.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.764342 yangson-1.4.8/docs/examples/ex3/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      465 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/examples/ex3/example-3-a@2017-08-01.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      473 2020-12-09 13:53:37.000000 yangson-1.4.8/docs/examples/ex3/example-3-b@2016-08-22.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      400 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/examples/ex3/example-3-suba@2017-08-01.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1254 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/examples/ex3/yang-library-ex3.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.764342 yangson-1.4.8/docs/examples/ex4/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      597 2021-03-13 11:55:47.000000 yangson-1.4.8/docs/examples/ex4/example-4-a.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      428 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/examples/ex4/example-4-b.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      144 2021-02-22 09:01:48.000000 yangson-1.4.8/docs/examples/ex4/example-data.json
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1237 2021-03-11 09:22:35.000000 yangson-1.4.8/docs/examples/ex4/yang-library-ex4.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.764342 yangson-1.4.8/docs/examples/ex5/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1297 2021-03-13 10:50:48.000000 yangson-1.4.8/docs/examples/ex5/example-5-a.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      197 2020-12-09 13:53:37.000000 yangson-1.4.8/docs/examples/ex5/example-5-b.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      477 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/examples/ex5/yang-library-ex5.json
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5327 2021-03-23 11:35:04.000000 yangson-1.4.8/docs/examples.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2106 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/exceptions.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7587 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/glossary.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      374 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/index.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    24690 2021-03-22 13:21:43.000000 yangson-1.4.8/docs/instance.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3734 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/instvalue.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3270 2021-03-23 15:57:34.000000 yangson-1.4.8/docs/introduction.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7577 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/parser.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     9120 2021-05-10 13:04:20.000000 yangson-1.4.8/docs/quickstart.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2259 2021-03-01 07:43:01.000000 yangson-1.4.8/docs/references.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    18245 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/schemadata.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    21266 2021-03-22 13:21:43.000000 yangson-1.4.8/docs/schemanode.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5470 2021-03-01 09:47:59.000000 yangson-1.4.8/docs/statement.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      163 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/support.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      585 2021-02-22 08:52:17.000000 yangson-1.4.8/docs/typealiases.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5152 2021-03-22 13:21:43.000000 yangson-1.4.8/docs/xpath.rst
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)       86 2021-03-22 15:26:50.000000 yangson-1.4.8/requirements.in
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)       38 2021-05-10 13:13:06.774342 yangson-1.4.8/setup.cfg
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1637 2021-02-22 08:52:17.000000 yangson-1.4.8/setup.py
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.767676 yangson-1.4.8/tests/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      575 2021-02-22 08:52:17.000000 yangson-1.4.8/tests/test_c.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1486 2021-02-22 08:52:17.000000 yangson-1.4.8/tests/test_d.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    46731 2021-03-22 13:21:43.000000 yangson-1.4.8/tests/test_model.py
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.767676 yangson-1.4.8/tools/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      623 2021-02-22 08:52:17.000000 yangson-1.4.8/tools/README.rst
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.767676 yangson-1.4.8/tools/css/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1305 2021-02-22 08:52:17.000000 yangson-1.4.8/tools/css/yang-data.css
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.767676 yangson-1.4.8/tools/python/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3545 2021-02-22 08:52:17.000000 yangson-1.4.8/tools/python/mkylib.py
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.767676 yangson-1.4.8/tools/xslt/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3209 2020-12-09 13:53:37.000000 yangson-1.4.8/tools/xslt/hello2yanglib.xsl
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.744342 yangson-1.4.8/yang-modules/
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.767676 yangson-1.4.8/yang-modules/ietf/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    15940 2020-12-09 13:53:37.000000 yangson-1.4.8/yang-modules/ietf/ietf-inet-types@2010-09-24.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    16833 2020-12-09 13:53:37.000000 yangson-1.4.8/yang-modules/ietf/ietf-inet-types@2013-07-15.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    13300 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/ietf/ietf-netconf-acm@2018-02-14.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3922 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/ietf/ietf-origin@2018-02-14.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7130 2020-12-09 13:53:37.000000 yangson-1.4.8/yang-modules/ietf/ietf-yang-library@2016-06-21.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2958 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/ietf/ietf-yang-metadata@2016-08-05.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    17939 2020-12-09 13:53:37.000000 yangson-1.4.8/yang-modules/ietf/ietf-yang-types@2013-07-15.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1443 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/ietf/yang-library.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.771009 yangson-1.4.8/yang-modules/jukebox/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5913 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/jukebox/example-jukebox@2016-08-15.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      321 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/jukebox/yang-library.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.771009 yangson-1.4.8/yang-modules/test/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      813 2021-02-28 10:22:55.000000 yangson-1.4.8/yang-modules/test/defs.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      946 2021-02-28 10:22:55.000000 yangson-1.4.8/yang-modules/test/subtest.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     4597 2021-02-28 10:22:55.000000 yangson-1.4.8/yang-modules/test/test.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1312 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/test/testb.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1522 2021-02-28 10:22:55.000000 yangson-1.4.8/yang-modules/test/yang-library.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.771009 yangson-1.4.8/yang-modules/testc/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      166 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/testc/testc@2021-01-05.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      314 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/testc/yang-library.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.771009 yangson-1.4.8/yang-modules/testd/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      236 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/testd/testd@2021-01-05.yang
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)      314 2021-02-22 08:52:17.000000 yangson-1.4.8/yang-modules/testd/yang-library.json
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.774342 yangson-1.4.8/yangson/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)       43 2021-03-17 09:04:40.000000 yangson-1.4.8/yangson/__init__.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     6496 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/__main__.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5694 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/constraint.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7792 2021-03-13 14:55:05.000000 yangson-1.4.8/yangson/datamodel.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    37037 2021-03-17 15:33:20.000000 yangson-1.4.8/yangson/datatype.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2850 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/enumerations.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    15485 2021-03-11 09:21:42.000000 yangson-1.4.8/yangson/exceptions.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    51414 2021-03-01 15:46:37.000000 yangson-1.4.8/yangson/instance.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3502 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/instvalue.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     4282 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/nodeset.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7659 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/parser.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    23028 2021-02-26 08:30:00.000000 yangson-1.4.8/yangson/schemadata.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    66244 2021-05-10 12:58:43.000000 yangson-1.4.8/yangson/schemanode.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    10529 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/schpattern.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    12894 2021-02-26 08:30:00.000000 yangson-1.4.8/yangson/statement.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2953 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/typealiases.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2241 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/xmlparser.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    27221 2021-03-24 09:40:12.000000 yangson-1.4.8/yangson/xpathast.py
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)    15202 2021-02-22 08:52:17.000000 yangson-1.4.8/yangson/xpathparser.py
-drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-05-10 13:13:06.774342 yangson-1.4.8/yangson.egg-info/
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1559 2021-05-10 13:13:06.000000 yangson-1.4.8/yangson.egg-info/PKG-INFO
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2946 2021-05-10 13:13:06.000000 yangson-1.4.8/yangson.egg-info/SOURCES.txt
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)        1 2021-05-10 13:13:06.000000 yangson-1.4.8/yangson.egg-info/dependency_links.txt
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)       51 2021-05-10 13:13:06.000000 yangson-1.4.8/yangson.egg-info/entry_points.txt
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)        5 2021-05-10 13:13:06.000000 yangson-1.4.8/yangson.egg-info/requires.txt
--rw-r--r--   0 lhotka    (1000) lhotka    (1000)        8 2021-05-10 13:13:06.000000 yangson-1.4.8/yangson.egg-info/top_level.txt
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.821555 yangson-1.4.9/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      201 2021-02-22 08:52:17.000000 yangson-1.4.9/.gitignore
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      572 2021-03-15 14:53:52.000000 yangson-1.4.9/.gitlab-ci.yml
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)        6 2021-02-22 08:52:17.000000 yangson-1.4.9/.python-version
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    35147 2020-12-09 13:53:37.000000 yangson-1.4.9/COPYING
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7650 2020-12-09 13:53:37.000000 yangson-1.4.9/COPYING.LESSER
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      247 2020-12-09 13:53:37.000000 yangson-1.4.9/MANIFEST.in
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      376 2021-06-10 08:22:19.000000 yangson-1.4.9/Makefile
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1559 2021-06-10 08:24:55.821555 yangson-1.4.9/PKG-INFO
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1098 2021-05-18 15:15:02.000000 yangson-1.4.9/README.rst
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.801555 yangson-1.4.9/docs/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7660 2021-03-23 15:58:22.000000 yangson-1.4.9/docs/Makefile
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.804889 yangson-1.4.9/docs/_templates/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      942 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/_templates/donation.html
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3985 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/_templates/donation.svg
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      113 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/_templates/layout.html
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      100 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/advanced.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      107 2020-12-09 13:53:37.000000 yangson-1.4.9/docs/basic.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     4134 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/cmdline.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7720 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/concepts-terms.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    11845 2021-03-01 09:47:59.000000 yangson-1.4.9/docs/conf.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     6205 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/constraint.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     9623 2021-03-22 13:21:43.000000 yangson-1.4.9/docs/datamodel.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    17571 2021-03-13 11:55:47.000000 yangson-1.4.9/docs/datatype.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      335 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/enumerations.rst
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.791555 yangson-1.4.9/docs/examples/
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.804889 yangson-1.4.9/docs/examples/ex1/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      175 2020-12-09 13:53:37.000000 yangson-1.4.9/docs/examples/ex1/example-1.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)       34 2021-03-21 15:55:54.000000 yangson-1.4.9/docs/examples/ex1/example-data.json
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      296 2020-12-09 13:53:37.000000 yangson-1.4.9/docs/examples/ex1/yang-library-ex1.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.804889 yangson-1.4.9/docs/examples/ex2/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      308 2021-03-13 14:55:05.000000 yangson-1.4.9/docs/examples/ex2/example-2-dev.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      728 2021-06-09 15:13:32.000000 yangson-1.4.9/docs/examples/ex2/example-2.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      451 2021-06-10 07:35:43.000000 yangson-1.4.9/docs/examples/ex2/example-data.json
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      255 2021-03-22 16:43:01.000000 yangson-1.4.9/docs/examples/ex2/example-data.yaml
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      963 2021-03-13 14:55:05.000000 yangson-1.4.9/docs/examples/ex2/yang-library-ex2.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.804889 yangson-1.4.9/docs/examples/ex3/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      465 2021-05-12 08:04:29.000000 yangson-1.4.9/docs/examples/ex3/example-3-a@2017-08-01.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      473 2020-12-09 13:53:37.000000 yangson-1.4.9/docs/examples/ex3/example-3-b@2016-08-22.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      400 2021-05-12 08:01:54.000000 yangson-1.4.9/docs/examples/ex3/example-3-suba@2017-08-01.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1254 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/examples/ex3/yang-library-ex3.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.804889 yangson-1.4.9/docs/examples/ex4/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      597 2021-03-13 11:55:47.000000 yangson-1.4.9/docs/examples/ex4/example-4-a.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      428 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/examples/ex4/example-4-b.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      144 2021-02-22 09:01:48.000000 yangson-1.4.9/docs/examples/ex4/example-data.json
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1237 2021-03-11 09:22:35.000000 yangson-1.4.9/docs/examples/ex4/yang-library-ex4.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.804889 yangson-1.4.9/docs/examples/ex5/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1297 2021-03-13 10:50:48.000000 yangson-1.4.9/docs/examples/ex5/example-5-a.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      197 2020-12-09 13:53:37.000000 yangson-1.4.9/docs/examples/ex5/example-5-b.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      477 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/examples/ex5/yang-library-ex5.json
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5327 2021-03-23 11:35:04.000000 yangson-1.4.9/docs/examples.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2106 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/exceptions.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7587 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/glossary.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      374 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/index.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    24690 2021-03-22 13:21:43.000000 yangson-1.4.9/docs/instance.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3734 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/instvalue.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3270 2021-03-23 15:57:34.000000 yangson-1.4.9/docs/introduction.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7577 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/parser.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     9120 2021-05-10 13:04:20.000000 yangson-1.4.9/docs/quickstart.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2259 2021-03-01 07:43:01.000000 yangson-1.4.9/docs/references.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    18245 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/schemadata.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    21266 2021-03-22 13:21:43.000000 yangson-1.4.9/docs/schemanode.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5470 2021-03-01 09:47:59.000000 yangson-1.4.9/docs/statement.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      163 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/support.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      585 2021-02-22 08:52:17.000000 yangson-1.4.9/docs/typealiases.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5152 2021-03-22 13:21:43.000000 yangson-1.4.9/docs/xpath.rst
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)       86 2021-03-22 15:26:50.000000 yangson-1.4.9/requirements.in
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)       38 2021-06-10 08:24:55.821555 yangson-1.4.9/setup.cfg
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1637 2021-02-22 08:52:17.000000 yangson-1.4.9/setup.py
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.808222 yangson-1.4.9/tests/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      575 2021-02-22 08:52:17.000000 yangson-1.4.9/tests/test_c.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1486 2021-02-22 08:52:17.000000 yangson-1.4.9/tests/test_d.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    46731 2021-03-22 13:21:43.000000 yangson-1.4.9/tests/test_model.py
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.808222 yangson-1.4.9/tools/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      623 2021-02-22 08:52:17.000000 yangson-1.4.9/tools/README.rst
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.808222 yangson-1.4.9/tools/css/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1305 2021-02-22 08:52:17.000000 yangson-1.4.9/tools/css/yang-data.css
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.808222 yangson-1.4.9/tools/python/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3545 2021-02-22 08:52:17.000000 yangson-1.4.9/tools/python/mkylib.py
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.808222 yangson-1.4.9/tools/xslt/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3209 2020-12-09 13:53:37.000000 yangson-1.4.9/tools/xslt/hello2yanglib.xsl
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.791555 yangson-1.4.9/yang-modules/
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.811555 yangson-1.4.9/yang-modules/ietf/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    15940 2020-12-09 13:53:37.000000 yangson-1.4.9/yang-modules/ietf/ietf-inet-types@2010-09-24.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    16833 2020-12-09 13:53:37.000000 yangson-1.4.9/yang-modules/ietf/ietf-inet-types@2013-07-15.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    13300 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/ietf/ietf-netconf-acm@2018-02-14.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3922 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/ietf/ietf-origin@2018-02-14.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7130 2020-12-09 13:53:37.000000 yangson-1.4.9/yang-modules/ietf/ietf-yang-library@2016-06-21.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2958 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/ietf/ietf-yang-metadata@2016-08-05.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    17939 2020-12-09 13:53:37.000000 yangson-1.4.9/yang-modules/ietf/ietf-yang-types@2013-07-15.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1443 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/ietf/yang-library.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.811555 yangson-1.4.9/yang-modules/jukebox/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5913 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/jukebox/example-jukebox@2016-08-15.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      321 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/jukebox/yang-library.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.811555 yangson-1.4.9/yang-modules/test/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      813 2021-02-28 10:22:55.000000 yangson-1.4.9/yang-modules/test/defs.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      946 2021-02-28 10:22:55.000000 yangson-1.4.9/yang-modules/test/subtest.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     4597 2021-02-28 10:22:55.000000 yangson-1.4.9/yang-modules/test/test.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1312 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/test/testb.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1522 2021-02-28 10:22:55.000000 yangson-1.4.9/yang-modules/test/yang-library.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.811555 yangson-1.4.9/yang-modules/testc/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      166 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/testc/testc@2021-01-05.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      314 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/testc/yang-library.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.811555 yangson-1.4.9/yang-modules/testd/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      236 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/testd/testd@2021-01-05.yang
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)      314 2021-02-22 08:52:17.000000 yangson-1.4.9/yang-modules/testd/yang-library.json
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.821555 yangson-1.4.9/yangson/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)       43 2021-03-17 09:04:40.000000 yangson-1.4.9/yangson/__init__.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     6496 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/__main__.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     5694 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/constraint.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7792 2021-03-13 14:55:05.000000 yangson-1.4.9/yangson/datamodel.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    37037 2021-03-17 15:33:20.000000 yangson-1.4.9/yangson/datatype.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2850 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/enumerations.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    15485 2021-03-11 09:21:42.000000 yangson-1.4.9/yangson/exceptions.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    51570 2021-06-10 08:19:55.000000 yangson-1.4.9/yangson/instance.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     3502 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/instvalue.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     4282 2021-05-11 08:54:25.000000 yangson-1.4.9/yangson/nodeset.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     7659 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/parser.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    23028 2021-02-26 08:30:00.000000 yangson-1.4.9/yangson/schemadata.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    66244 2021-05-10 12:58:43.000000 yangson-1.4.9/yangson/schemanode.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    10529 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/schpattern.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    12894 2021-02-26 08:30:00.000000 yangson-1.4.9/yangson/statement.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2953 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/typealiases.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2241 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/xmlparser.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    27226 2021-05-11 08:17:32.000000 yangson-1.4.9/yangson/xpathast.py
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)    15202 2021-02-22 08:52:17.000000 yangson-1.4.9/yangson/xpathparser.py
+drwxr-xr-x   0 lhotka    (1000) lhotka    (1000)        0 2021-06-10 08:24:55.821555 yangson-1.4.9/yangson.egg-info/
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     1559 2021-06-10 08:24:55.000000 yangson-1.4.9/yangson.egg-info/PKG-INFO
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)     2946 2021-06-10 08:24:55.000000 yangson-1.4.9/yangson.egg-info/SOURCES.txt
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)        1 2021-06-10 08:24:55.000000 yangson-1.4.9/yangson.egg-info/dependency_links.txt
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)       51 2021-06-10 08:24:55.000000 yangson-1.4.9/yangson.egg-info/entry_points.txt
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)        5 2021-06-10 08:24:55.000000 yangson-1.4.9/yangson.egg-info/requires.txt
+-rw-r--r--   0 lhotka    (1000) lhotka    (1000)        8 2021-06-10 08:24:55.000000 yangson-1.4.9/yangson.egg-info/top_level.txt
```

### Comparing `yangson-1.4.8/.gitlab-ci.yml` & `yangson-1.4.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/COPYING` & `yangson-1.4.9/COPYING`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/COPYING.LESSER` & `yangson-1.4.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/PKG-INFO` & `yangson-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yangson
-Version: 1.4.8
+Version: 1.4.9
 Summary: Library for working with data modelled in YANG
 Home-page: https://github.com/CZ-NIC/yangson
 Author: Ladislav Lhotka
 Author-email: lhotka@nic.cz
 License: UNKNOWN
 Description: .. |date| date::
```

### Comparing `yangson-1.4.8/README.rst` & `yangson-1.4.9/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 .. |date| date::
 
+.. |v6| image:: https://img.shields.io/badge/python-3.6-blue.svg
+   :alt: Python 3.6
+
+.. |v7| image:: https://img.shields.io/badge/python-3.7-blue.svg
+   :alt: Python 3.7
+
+.. |v8| image:: https://img.shields.io/badge/python-3.8-blue.svg
+   :alt: Python 3.8
+
+.. |v9| image:: https://img.shields.io/badge/python-3.9-blue.svg
+   :alt: Python 3.9
+
+|v6| |v7| |v8| |v9|
+
 ******************
 Welcome to Yangson
 ******************
 
 :Author: Ladislav Lhotka <lhotka@nic.cz>
 :Date: |date|
```

### Comparing `yangson-1.4.8/docs/Makefile` & `yangson-1.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/_templates/donation.html` & `yangson-1.4.9/docs/_templates/donation.html`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/_templates/donation.svg` & `yangson-1.4.9/docs/_templates/donation.svg`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/cmdline.rst` & `yangson-1.4.9/docs/cmdline.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/concepts-terms.rst` & `yangson-1.4.9/docs/concepts-terms.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/conf.py` & `yangson-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/constraint.rst` & `yangson-1.4.9/docs/constraint.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/datamodel.rst` & `yangson-1.4.9/docs/datamodel.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/datatype.rst` & `yangson-1.4.9/docs/datatype.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples/ex2/example-2.yang` & `yangson-1.4.9/docs/examples/ex2/example-2.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples/ex2/yang-library-ex2.json` & `yangson-1.4.9/docs/examples/ex2/yang-library-ex2.json`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples/ex3/yang-library-ex3.json` & `yangson-1.4.9/docs/examples/ex3/yang-library-ex3.json`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples/ex4/example-4-a.yang` & `yangson-1.4.9/docs/examples/ex4/example-4-a.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples/ex4/yang-library-ex4.json` & `yangson-1.4.9/docs/examples/ex4/yang-library-ex4.json`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples/ex5/example-5-a.yang` & `yangson-1.4.9/docs/examples/ex5/example-5-a.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/examples.rst` & `yangson-1.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/exceptions.rst` & `yangson-1.4.9/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/glossary.rst` & `yangson-1.4.9/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/instance.rst` & `yangson-1.4.9/docs/instance.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/instvalue.rst` & `yangson-1.4.9/docs/instvalue.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/introduction.rst` & `yangson-1.4.9/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/parser.rst` & `yangson-1.4.9/docs/parser.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/quickstart.rst` & `yangson-1.4.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/references.rst` & `yangson-1.4.9/docs/references.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/schemadata.rst` & `yangson-1.4.9/docs/schemadata.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/schemanode.rst` & `yangson-1.4.9/docs/schemanode.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/statement.rst` & `yangson-1.4.9/docs/statement.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/typealiases.rst` & `yangson-1.4.9/docs/typealiases.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/docs/xpath.rst` & `yangson-1.4.9/docs/xpath.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/setup.py` & `yangson-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tests/test_c.py` & `yangson-1.4.9/tests/test_c.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tests/test_d.py` & `yangson-1.4.9/tests/test_d.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tests/test_model.py` & `yangson-1.4.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tools/README.rst` & `yangson-1.4.9/tools/README.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tools/css/yang-data.css` & `yangson-1.4.9/tools/css/yang-data.css`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tools/python/mkylib.py` & `yangson-1.4.9/tools/python/mkylib.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/tools/xslt/hello2yanglib.xsl` & `yangson-1.4.9/tools/xslt/hello2yanglib.xsl`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-inet-types@2010-09-24.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-inet-types@2010-09-24.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-inet-types@2013-07-15.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-inet-types@2013-07-15.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-netconf-acm@2018-02-14.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-netconf-acm@2018-02-14.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-origin@2018-02-14.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-origin@2018-02-14.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-yang-library@2016-06-21.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-yang-library@2016-06-21.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-yang-metadata@2016-08-05.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-yang-metadata@2016-08-05.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/ietf-yang-types@2013-07-15.yang` & `yangson-1.4.9/yang-modules/ietf/ietf-yang-types@2013-07-15.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/ietf/yang-library.json` & `yangson-1.4.9/yang-modules/ietf/yang-library.json`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/jukebox/example-jukebox@2016-08-15.yang` & `yangson-1.4.9/yang-modules/jukebox/example-jukebox@2016-08-15.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/test/defs.yang` & `yangson-1.4.9/yang-modules/test/defs.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/test/subtest.yang` & `yangson-1.4.9/yang-modules/test/subtest.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/test/test.yang` & `yangson-1.4.9/yang-modules/test/test.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/test/testb.yang` & `yangson-1.4.9/yang-modules/test/testb.yang`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yang-modules/test/yang-library.json` & `yangson-1.4.9/yang-modules/test/yang-library.json`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/__main__.py` & `yangson-1.4.9/yangson/__main__.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/constraint.py` & `yangson-1.4.9/yangson/constraint.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/datamodel.py` & `yangson-1.4.9/yangson/datamodel.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/datatype.py` & `yangson-1.4.9/yangson/datatype.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/enumerations.py` & `yangson-1.4.9/yangson/enumerations.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/exceptions.py` & `yangson-1.4.9/yangson/exceptions.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/instance.py` & `yangson-1.4.9/yangson/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,17 @@
 
     @property
     def path(self: "InstanceNode") -> Tuple[InstanceKey]:
         """Return the list of keys on the path from root to the receiver."""
         res = []
         inst: InstanceNode = self
         while inst.parinst:
-            res.insert(0, inst._key)
+            res.append(inst._key)
             inst = inst.parinst
+        res.reverse()
         return tuple(res)
 
     def __str__(self: "InstanceNode") -> str:
         """Return string representation of the receiver's value."""
         sn = self.schema_node
         return (str(self.value) if isinstance(self.value, StructuredValue) else
                 sn.type.canonical_string(self.value))
@@ -226,16 +227,17 @@
         return "/" + "/".join([str(c) for c in self.path])
 
     def instance_route(self: "InstanceNode") -> "InstanceRoute":
         """Return :class:`InstanceRoute` of the receiver."""
         res = InstanceRoute()
         inst = self
         while inst.parinst:
-            res.insert(0, inst._instance_route_entry())
+            res.append(inst._instance_route_entry())
             inst = inst.parinst
+        res.reverse()
         return res
 
     def is_internal(self: "InstanceNode") -> bool:
         """Return ``True`` if the receiver is an instance of an internal node.
         """
         return isinstance(self.schema_node, InternalNode)
 
@@ -947,18 +949,21 @@
         sn = self.schema_node
         if isinstance(sn, LeafListNode):
             return EntryValue(sn.type.canonical_string(self.value))
         if not sn.keys:
             return EntryIndex(self._key)
         kdict = {}
         for k in sn.keys:
-            if k[1] == sn.ns:
-                kdict[(k[0], None)] = str(self[k[0]])
-            else:
-                kdict[k] = str(self[f"{k[1]}:{k[0]}"])
+            try:
+                if k[1] == sn.ns:
+                    kdict[(k[0], None)] = str(self[k[0]])
+                else:
+                    kdict[k] = str(self[f"{k[1]}:{k[0]}"])
+            except NonexistentInstance:
+                return EntryIndex(self._key)
         return EntryKeys(kdict)
 
     def _ancestors_or_self(
             self: "ArrayEntry",
             qname: Union[QualName, bool] = None) -> List[InstanceNode]:
         """XPath - return the list of receiver's ancestors including itself."""
         res = [] if qname and self.qual_name != qname else [self]
```

### Comparing `yangson-1.4.8/yangson/instvalue.py` & `yangson-1.4.9/yangson/instvalue.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/nodeset.py` & `yangson-1.4.9/yangson/nodeset.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/parser.py` & `yangson-1.4.9/yangson/parser.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/schemadata.py` & `yangson-1.4.9/yangson/schemadata.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/schemanode.py` & `yangson-1.4.9/yangson/schemanode.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/schpattern.py` & `yangson-1.4.9/yangson/schpattern.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/statement.py` & `yangson-1.4.9/yangson/statement.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/typealiases.py` & `yangson-1.4.9/yangson/typealiases.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/xmlparser.py` & `yangson-1.4.9/yangson/xmlparser.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson/xpathast.py` & `yangson-1.4.9/yangson/xpathast.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,15 +687,15 @@
             ns = self.expr._eval(xctx)
             try:
                 node = ns[0]
             except TypeError:
                 raise XPathTypeError(str(ns))
             except IndexError:
                 return ""
-        if node.path == ():
+        if node.parinst is None:
             return ""
         if self.local:
             p, s, loc = node.name.partition(":")
             return loc if s else p
         return node.name
```

### Comparing `yangson-1.4.8/yangson/xpathparser.py` & `yangson-1.4.9/yangson/xpathparser.py`

 * *Files identical despite different names*

### Comparing `yangson-1.4.8/yangson.egg-info/PKG-INFO` & `yangson-1.4.9/yangson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yangson
-Version: 1.4.8
+Version: 1.4.9
 Summary: Library for working with data modelled in YANG
 Home-page: https://github.com/CZ-NIC/yangson
 Author: Ladislav Lhotka
 Author-email: lhotka@nic.cz
 License: UNKNOWN
 Description: .. |date| date::
```

### Comparing `yangson-1.4.8/yangson.egg-info/SOURCES.txt` & `yangson-1.4.9/yangson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

