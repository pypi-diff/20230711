# Comparing `tmp/xrootd-5.6.0.tar.gz` & `tmp/xrootd-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrootd-5.6.0.tar", last modified: Fri Jun 30 14:31:35 2023, max compression
+gzip compressed data, was "xrootd-5.6.1.tar", last modified: Tue Jul 11 09:20:11 2023, max compression
```

## Comparing `xrootd-5.6.0.tar` & `xrootd-5.6.1.tar`

### file list

```diff
@@ -1,1750 +1,1749 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.927901 xrootd-5.6.0/
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-30 14:28:10.000000 xrootd-5.6.0/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    35147 2023-06-30 14:28:10.000000 xrootd-5.6.0/COPYING
--rw-r--r--   0 root         (0) root         (0)     2811 2023-06-30 14:28:10.000000 xrootd-5.6.0/COPYING.BSD
--rw-r--r--   0 root         (0) root         (0)     7651 2023-06-30 14:28:10.000000 xrootd-5.6.0/COPYING.LGPL
--rw-r--r--   0 root         (0) root         (0)     1432 2023-06-30 14:28:10.000000 xrootd-5.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-30 14:28:10.000000 xrootd-5.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4632 2023-06-30 14:31:35.917901 xrootd-5.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3791 2023-06-30 14:28:10.000000 xrootd-5.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-30 14:31:31.000000 xrootd-5.6.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/bindings/
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/bindings/python/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/.gitignore
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8129 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-30 14:31:31.000000 xrootd-5.6.0/bindings/python/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/bindings/python/docs/
--rw-r--r--   0 root         (0) root         (0)     5581 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     1225 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/ReleaseNotes.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/bindings/python/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.707900 xrootd-5.6.0/bindings/python/docs/source/.static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/bindings/python/docs/source/.static/css/
--rwxr-xr-x   0 root         (0) root         (0)    15713 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/.static/css/custom.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/bindings/python/docs/source/.templates/
--rwxr-xr-x   0 root         (0) root         (0)       89 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/.templates/layout.html
--rw-r--r--   0 root         (0) root         (0)     8013 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/docs/source/examples/
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/examples/copyprocess.rst
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/examples/file.rst
--rw-r--r--   0 root         (0) root         (0)     3243 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/examples/filesystem.rst
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/examples.rst
--rw-r--r--   0 root         (0) root         (0)     4286 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/gettingstarted.rst
--rw-r--r--   0 root         (0) root         (0)      844 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/index.rst
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/install.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.707900 xrootd-5.6.0/bindings/python/docs/source/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/docs/source/modules/client/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/copyprocess.rst
--rw-r--r--   0 root         (0) root         (0)     1385 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/file.rst
--rw-r--r--   0 root         (0) root         (0)     1293 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/filesystem.rst
--rw-r--r--   0 root         (0) root         (0)     5238 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/flags.rst
--rw-r--r--   0 root         (0) root         (0)      944 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/responses.rst
--rw-r--r--   0 root         (0) root         (0)      342 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/url.rst
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/modules/client/utils.rst
--rw-r--r--   0 root         (0) root         (0)    14979 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/docs/source/xrootd-200x68.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/examples/
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/copy.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/copyprocess.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/dirlist.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/fcntl.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/fcntl_async.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/fileproperties.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/filesystemproperties.py
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/iterate.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/locate.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/mkdir.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/mv.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/query.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/read.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/readchunks.py
--rw-r--r--   0 root         (0) root         (0)      446 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/readlines.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/rm.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/rmdir.py
--rw-r--r--   0 root         (0) root         (0)      850 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/vector_read.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/visa.py
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/visa_async.py
--rw-r--r--   0 root         (0) root         (0)      356 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/examples/write.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/libs/client/
--rw-r--r--   0 root         (0) root         (0)      562 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/_version.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/copyprocess.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/env.py
--rw-r--r--   0 root         (0) root         (0)    13367 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/file.py
--rw-r--r--   0 root         (0) root         (0)    17398 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/filesystem.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/finalize.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/flags.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/glob_funcs.py
--rw-r--r--   0 root         (0) root         (0)    11449 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/responses.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/url.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/libs/client/utils.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5164 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/src/
--rw-r--r--   0 root         (0) root         (0)    12167 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/AsyncResponseHandler.hh
--rw-r--r--   0 root         (0) root         (0)     1821 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6731 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/ChunkIterator.hh
--rw-r--r--   0 root         (0) root         (0)    13695 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/Conversions.hh
--rw-r--r--   0 root         (0) root         (0)     1898 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootD.hh
--rw-r--r--   0 root         (0) root         (0)     8623 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDCopyProcess.cc
--rw-r--r--   0 root         (0) root         (0)     6663 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDCopyProcess.hh
--rw-r--r--   0 root         (0) root         (0)     4415 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDCopyProgressHandler.cc
--rw-r--r--   0 root         (0) root         (0)     3562 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDCopyProgressHandler.hh
--rw-r--r--   0 root         (0) root         (0)     5119 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDEnv.hh
--rw-r--r--   0 root         (0) root         (0)    35747 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDFile.cc
--rw-r--r--   0 root         (0) root         (0)    12239 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDFile.hh
--rw-r--r--   0 root         (0) root         (0)    37424 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDFileSystem.cc
--rw-r--r--   0 root         (0) root         (0)    10740 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDFileSystem.hh
--rw-r--r--   0 root         (0) root         (0)     2135 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDFinalize.hh
--rw-r--r--   0 root         (0) root         (0)     5199 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDModule.cc
--rw-r--r--   0 root         (0) root         (0)     7622 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDURL.cc
--rw-r--r--   0 root         (0) root         (0)     8015 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/PyXRootDURL.hh
--rw-r--r--   0 root         (0) root         (0)     6144 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/Utils.cc
--rw-r--r--   0 root         (0) root         (0)     4293 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/Utils.hh
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.727900 xrootd-5.6.0/bindings/python/tests/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/env.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/test_copy.py
--rw-r--r--   0 root         (0) root         (0)    11797 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/test_file.py
--rw-r--r--   0 root         (0) root         (0)     5387 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/test_filesystem.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/test_glob.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/test_threads.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-30 14:28:10.000000 xrootd-5.6.0/bindings/python/tests/test_url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.737900 xrootd-5.6.0/cmake/
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindAutoConf.cmake
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindAutoMake.cmake
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindCppUnit.cmake
--rw-r--r--   0 root         (0) root         (0)     1816 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindDavix.cmake
--rw-r--r--   0 root         (0) root         (0)      839 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindKerberos5.cmake
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindLibTool.cmake
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindMacaroons.cmake
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindReadline.cmake
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindSciTokensCpp.cmake
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindTinyXml.cmake
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindVOMS.cmake
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/FindYasm.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/Findfuse.cmake
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/Findisal.cmake
--rw-r--r--   0 root         (0) root         (0)     2248 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/Findlibuuid.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/Findsystemd.cmake
--rw-r--r--   0 root         (0) root         (0)     7570 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDConfig.cmake.in
--rw-r--r--   0 root         (0) root         (0)     2363 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDDefaults.cmake
--rw-r--r--   0 root         (0) root         (0)     4796 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDFindLibs.cmake
--rw-r--r--   0 root         (0) root         (0)     7174 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDOSDefs.cmake
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDSummary.cmake
--rw-r--r--   0 root         (0) root         (0)     6716 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDSystemCheck.cmake
--rw-r--r--   0 root         (0) root         (0)     2565 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDUtils.cmake
--rw-r--r--   0 root         (0) root         (0)     3053 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake/XRootDVersion.cmake
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-30 14:28:10.000000 xrootd-5.6.0/cmake_uninstall.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.737900 xrootd-5.6.0/docs/
--rw-r--r--   0 root         (0) root         (0)    11322 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     7793 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/INSTALL.md
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/PreReleaseNotes.txt
--rw-r--r--   0 root         (0) root         (0)     4415 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/README_IPV4_To_IPV6
--rw-r--r--   0 root         (0) root         (0)   174821 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/ReleaseNotes.txt
--rw-r--r--   0 root         (0) root         (0)    18648 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/TESTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.737900 xrootd-5.6.0/docs/man/
--rw-r--r--   0 root         (0) root         (0)      938 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/cmsd.8
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/frm_admin.8
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/frm_purged.8
--rw-r--r--   0 root         (0) root         (0)      929 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/frm_xfragent.8
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/frm_xfrd.8
--rw-r--r--   0 root         (0) root         (0)     4438 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/libXrdVoms.1
--rw-r--r--   0 root         (0) root         (0)     1046 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/mpxstats.8
--rw-r--r--   0 root         (0) root         (0)     1019 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdadler32.1
--rw-r--r--   0 root         (0) root         (0)    17367 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdcp.1
--rw-r--r--   0 root         (0) root         (0)     6398 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdfs.1
--rw-r--r--   0 root         (0) root         (0)     1792 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdgsiproxy.1
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdgsitest.1
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdmapc.1
--rw-r--r--   0 root         (0) root         (0)     2071 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdpfc_print.8
--rw-r--r--   0 root         (0) root         (0)      872 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdpwdadmin.8
--rw-r--r--   0 root         (0) root         (0)      850 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrdsssadmin.8
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrootd.8
--rw-r--r--   0 root         (0) root         (0)     3745 2023-06-30 14:28:10.000000 xrootd-5.6.0/docs/man/xrootdfs.1
--rwxr-xr-x   0 root         (0) root         (0)      772 2023-06-30 14:28:10.000000 xrootd-5.6.0/gen-tarball.sh
--rwxr-xr-x   0 root         (0) root         (0)     1354 2023-06-30 14:28:10.000000 xrootd-5.6.0/genversion.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.737900 xrootd-5.6.0/packaging/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.737900 xrootd-5.6.0/packaging/common/
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/client-plugin.conf.example
--rw-r--r--   0 root         (0) root         (0)     6149 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/client.conf
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/cmsd@.service
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/frm_purged@.service
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/frm_xfrd@.service
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/http.client.conf.example
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/recorder.conf
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrdhttp@.socket
--rw-r--r--   0 root         (0) root         (0)     3006 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd-clustered.cfg
--rw-r--r--   0 root         (0) root         (0)     3342 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd-filecache-clustered.cfg
--rw-r--r--   0 root         (0) root         (0)     1666 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd-filecache-standalone.cfg
--rw-r--r--   0 root         (0) root         (0)     1986 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd-http.cfg
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd-standalone.cfg
--rw-r--r--   0 root         (0) root         (0)      626 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd.logrotate
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd.te
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd@.service
--rw-r--r--   0 root         (0) root         (0)      122 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/common/xrootd@.socket
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/packaging/debian/
--rw-r--r--   0 root         (0) root         (0)        3 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/compat
--rw-r--r--   0 root         (0) root         (0)    16401 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/control
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/copyright
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdapputils1.install
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdcl2.install
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdcrypto1.install
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdcryptolite1.install
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdffs2.install
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdhttputils1.install
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdposix2.install
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdserver2.install
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdssilib1.install
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdssishmap1.install
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdutils2.install
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrdxml2.install
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrootd-client-dev.install
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrootd-dev.install
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrootd-private-dev.install
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/libxrootd-server-dev.install
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/python3-xrootd.install
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/python3-xrootd.install.new
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/rules
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/packaging/debian/source/
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/source/format
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-client-devel.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-client-libs.install
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-client-plugins.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-client.install
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-clients.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-devel.install
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-fuse.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-libs.install
--rw-r--r--   0 root         (0) root         (0)       83 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-plugins.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-private-devel.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-server-devel.install
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-server-libs.install
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-server-plugins.install
--rw-r--r--   0 root         (0) root         (0)      542 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian/xrootd-server.install
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/packaging/debian_scripts/
--rwxr-xr-x   0 root         (0) root         (0)     1738 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/debian_scripts/publish_debian_cern.sh
--rwxr-xr-x   0 root         (0) root         (0)     7960 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/makesrpm.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/packaging/rhel/
--rw-r--r--   0 root         (0) root         (0)      809 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/cmsd.init
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/frm_purged.init
--rw-r--r--   0 root         (0) root         (0)      839 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/frm_xfrd.init
--rw-r--r--   0 root         (0) root         (0)     8866 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/xrootd.functions
--rw-r--r--   0 root         (0) root         (0)     8451 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/xrootd.functions-slc4
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/xrootd.init
--rw-r--r--   0 root         (0) root         (0)    37002 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/xrootd.spec.in
--rw-r--r--   0 root         (0) root         (0)     3489 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/xrootd.sysconfig
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/rhel/xrootd.tmpfiles
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/packaging/tgz/
--rw-r--r--   0 root         (0) root         (0)     2043 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/README
--rwxr-xr-x   0 root         (0) root         (0)     4590 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StartCMS
--rwxr-xr-x   0 root         (0) root         (0)     4388 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StartFRM
--rwxr-xr-x   0 root         (0) root         (0)     5420 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StartOLB
--rw-r--r--   0 root         (0) root         (0)     2063 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StartOLB.cf.example
--rwxr-xr-x   0 root         (0) root         (0)     4767 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StartXRD
--rw-r--r--   0 root         (0) root         (0)     3842 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StartXRD.cf.example
--rwxr-xr-x   0 root         (0) root         (0)     3039 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StopCMS
--rwxr-xr-x   0 root         (0) root         (0)     3735 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StopFRM
--rwxr-xr-x   0 root         (0) root         (0)     2910 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StopOLB
--rwxr-xr-x   0 root         (0) root         (0)     2615 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/StopXRD
--rw-r--r--   0 root         (0) root         (0)     1988 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/xrootd.cf.example
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/tgz/xrootd.cf.example2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/packaging/wheel/
--rwxr-xr-x   0 root         (0) root         (0)     1169 2023-06-30 14:28:10.000000 xrootd-5.6.0/packaging/wheel/publish.sh
--rwxr-xr-x   0 root         (0) root         (0)     1169 2023-06-30 14:28:10.000000 xrootd-5.6.0/publish.sh
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-30 14:28:10.000000 xrootd-5.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 14:31:35.927901 xrootd-5.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4080 2023-06-30 14:28:10.000000 xrootd-5.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/src/
--rw-r--r--   0 root         (0) root         (0)     3848 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.747900 xrootd-5.6.0/src/XProtocol/
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XProtocol/README
--rw-r--r--   0 root         (0) root         (0)    11295 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XProtocol/XProtocol.cc
--rw-r--r--   0 root         (0) root         (0)    51065 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XProtocol/XProtocol.hh
--rw-r--r--   0 root         (0) root         (0)     5574 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XProtocol/XPtypes.hh
--rw-r--r--   0 root         (0) root         (0)    25337 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XProtocol/YProtocol.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.757900 xrootd-5.6.0/src/Xrd/
--rw-r--r--   0 root         (0) root         (0)     9005 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdBuffXL.cc
--rw-r--r--   0 root         (0) root         (0)     3279 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdBuffXL.hh
--rw-r--r--   0 root         (0) root         (0)    11819 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdBuffer.cc
--rw-r--r--   0 root         (0) root         (0)     4299 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdBuffer.hh
--rw-r--r--   0 root         (0) root         (0)    93305 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdConfig.cc
--rw-r--r--   0 root         (0) root         (0)     5661 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdConfig.hh
--rw-r--r--   0 root         (0) root         (0)     2900 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdGlobals.cc
--rw-r--r--   0 root         (0) root         (0)     9400 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdInet.cc
--rw-r--r--   0 root         (0) root         (0)     3445 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdInet.hh
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdInfo.cc
--rw-r--r--   0 root         (0) root         (0)     2489 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdInfo.hh
--rw-r--r--   0 root         (0) root         (0)     3099 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdJob.hh
--rw-r--r--   0 root         (0) root         (0)    25173 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLink.cc
--rw-r--r--   0 root         (0) root         (0)    26923 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLink.hh
--rw-r--r--   0 root         (0) root         (0)    14522 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkCtl.cc
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkCtl.hh
--rw-r--r--   0 root         (0) root         (0)     3499 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkInfo.hh
--rw-r--r--   0 root         (0) root         (0)     5054 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkMatch.cc
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkMatch.hh
--rw-r--r--   0 root         (0) root         (0)    46764 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkXeq.cc
--rw-r--r--   0 root         (0) root         (0)     7101 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdLinkXeq.hh
--rw-r--r--   0 root         (0) root         (0)     8748 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdMain.cc
--rw-r--r--   0 root         (0) root         (0)     5456 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdObject.hh
--rw-r--r--   0 root         (0) root         (0)     4407 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdObject.icc
--rw-r--r--   0 root         (0) root         (0)    12682 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPoll.cc
--rw-r--r--   0 root         (0) root         (0)     5644 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPoll.hh
--rw-r--r--   0 root         (0) root         (0)     3601 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPollE.hh
--rw-r--r--   0 root         (0) root         (0)    14457 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPollE.icc
--rw-r--r--   0 root         (0) root         (0)     3308 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPollInfo.hh
--rw-r--r--   0 root         (0) root         (0)     3207 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPollPoll.hh
--rw-r--r--   0 root         (0) root         (0)    17863 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdPollPoll.icc
--rw-r--r--   0 root         (0) root         (0)    12456 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdProtLoad.cc
--rw-r--r--   0 root         (0) root         (0)     3854 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdProtLoad.hh
--rw-r--r--   0 root         (0) root         (0)    10727 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdProtocol.hh
--rw-r--r--   0 root         (0) root         (0)    24210 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdScheduler.cc
--rw-r--r--   0 root         (0) root         (0)     5635 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdScheduler.hh
--rw-r--r--   0 root         (0) root         (0)    13605 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdSendQ.cc
--rw-r--r--   0 root         (0) root         (0)     3735 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdSendQ.hh
--rw-r--r--   0 root         (0) root         (0)    12208 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdStats.cc
--rw-r--r--   0 root         (0) root         (0)     3836 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdStats.hh
--rw-r--r--   0 root         (0) root         (0)     4914 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdTcpMonPin.hh
--rw-r--r--   0 root         (0) root         (0)     3291 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/Xrd/XrdTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.757900 xrootd-5.6.0/src/XrdAcc/
--rw-r--r--   0 root         (0) root         (0)    18177 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAccess.cc
--rw-r--r--   0 root         (0) root         (0)     8058 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAccess.hh
--rw-r--r--   0 root         (0) root         (0)     4734 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAudit.cc
--rw-r--r--   0 root         (0) root         (0)     5263 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAudit.hh
--rw-r--r--   0 root         (0) root         (0)     5258 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAuthDB.hh
--rw-r--r--   0 root         (0) root         (0)    12972 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAuthFile.cc
--rw-r--r--   0 root         (0) root         (0)     3587 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAuthFile.hh
--rw-r--r--   0 root         (0) root         (0)    12043 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccAuthorize.hh
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccCapability.cc
--rw-r--r--   0 root         (0) root         (0)     5914 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccCapability.hh
--rw-r--r--   0 root         (0) root         (0)    34347 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccConfig.cc
--rw-r--r--   0 root         (0) root         (0)     5754 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccConfig.hh
--rw-r--r--   0 root         (0) root         (0)     8327 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccEntity.cc
--rw-r--r--   0 root         (0) root         (0)     5422 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccEntity.hh
--rw-r--r--   0 root         (0) root         (0)    15542 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccGroups.cc
--rw-r--r--   0 root         (0) root         (0)     7392 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccGroups.hh
--rw-r--r--   0 root         (0) root         (0)     4791 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdAcc/XrdAccPrivs.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.757900 xrootd-5.6.0/src/XrdApps/
--rw-r--r--   0 root         (0) root         (0)    14593 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdAccTest.cc
--rw-r--r--   0 root         (0) root         (0)     7202 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdAppsCconfig.cc
--rw-r--r--   0 root         (0) root         (0)     6428 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdCks.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.757900 xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/
--rw-r--r--   0 root         (0) root         (0)     7035 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc
--rw-r--r--   0 root         (0) root         (0)    12371 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh
--rw-r--r--   0 root         (0) root         (0)     4214 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc
--rw-r--r--   0 root         (0) root         (0)     2721 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh
--rw-r--r--   0 root         (0) root         (0)     1822 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.757900 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/
--rw-r--r--   0 root         (0) root         (0)    14346 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/README.md
--rw-r--r--   0 root         (0) root         (0)    13235 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh
--rw-r--r--   0 root         (0) root         (0)     9856 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh
--rw-r--r--   0 root         (0) root         (0)    18873 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc
--rw-r--r--   0 root         (0) root         (0)     3178 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh
--rw-r--r--   0 root         (0) root         (0)    53534 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc
--rw-r--r--   0 root         (0) root         (0)     7563 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh
--rw-r--r--   0 root         (0) root         (0)    40660 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdCpConfig.cc
--rw-r--r--   0 root         (0) root         (0)    13017 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdCpConfig.hh
--rw-r--r--   0 root         (0) root         (0)     7118 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdCpFile.cc
--rw-r--r--   0 root         (0) root         (0)     3726 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdCpFile.hh
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdCrc32c.cc
--rw-r--r--   0 root         (0) root         (0)    19913 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdMapCluster.cc
--rw-r--r--   0 root         (0) root         (0)    10463 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdMpxStats.cc
--rw-r--r--   0 root         (0) root         (0)    15785 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdMpxXml.cc
--rw-r--r--   0 root         (0) root         (0)     3279 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdMpxXml.hh
--rw-r--r--   0 root         (0) root         (0)     5291 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdPinls.cc
--rw-r--r--   0 root         (0) root         (0)    10301 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdPrep.cc
--rw-r--r--   0 root         (0) root         (0)     8490 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdQStats.cc
--rw-r--r--   0 root         (0) root         (0)    10451 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/XrdWait41.cc
--rw-r--r--   0 root         (0) root         (0)     9299 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps/Xrdadler32.cc
--rw-r--r--   0 root         (0) root         (0)     6565 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdApps.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdBwm/
--rw-r--r--   0 root         (0) root         (0)    38144 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwm.cc
--rw-r--r--   0 root         (0) root         (0)    12819 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwm.hh
--rw-r--r--   0 root         (0) root         (0)    15615 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmConfig.cc
--rw-r--r--   0 root         (0) root         (0)    14111 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmHandle.cc
--rw-r--r--   0 root         (0) root         (0)     4374 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmHandle.hh
--rw-r--r--   0 root         (0) root         (0)    11034 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmLogger.cc
--rw-r--r--   0 root         (0) root         (0)     3761 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmLogger.hh
--rw-r--r--   0 root         (0) root         (0)     8624 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmPolicy.hh
--rw-r--r--   0 root         (0) root         (0)     6036 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmPolicy1.cc
--rw-r--r--   0 root         (0) root         (0)     4429 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmPolicy1.hh
--rw-r--r--   0 root         (0) root         (0)     3393 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdBwm/XrdBwmTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/.gitattributes
--rw-r--r--   0 root         (0) root         (0)     1036 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4416 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     1760 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    35147 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/COPYING
--rw-r--r--   0 root         (0) root         (0)     2811 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/COPYING.BSD
--rw-r--r--   0 root         (0) root         (0)     7651 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/COPYING.LGPL
--rw-r--r--   0 root         (0) root         (0)    11172 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/Doxyfile
--rw-r--r--   0 root         (0) root         (0)     1432 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/README
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/VERSION_INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/cmake/
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/FindCppUnit.cmake
--rw-r--r--   0 root         (0) root         (0)      840 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/FindXRootD.cmake
--rw-r--r--   0 root         (0) root         (0)      741 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/Findceph.cmake
--rw-r--r--   0 root         (0) root         (0)     7023 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/GNUInstallDirs.cmake
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/XRootDDefaults.cmake
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/XRootDFindLibs.cmake
--rw-r--r--   0 root         (0) root         (0)     1793 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/XRootDOSDefs.cmake
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/XRootDSummary.cmake
--rw-r--r--   0 root         (0) root         (0)     1417 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/cmake/XRootDUtils.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/docs/
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/docs/PreReleaseNotes.txt
--rw-r--r--   0 root         (0) root         (0)    86325 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/docs/ReleaseNotes.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/packaging/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/packaging/debian/
--rw-r--r--   0 root         (0) root         (0)        3 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/compat
--rw-r--r--   0 root         (0) root         (0)     2282 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/control
--rw-r--r--   0 root         (0) root         (0)     1432 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/copyright
--rwxr-xr-x   0 root         (0) root         (0)      538 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/rules
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/packaging/debian/source/
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/source/format
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-client-devel.install
--rw-r--r--   0 root         (0) root         (0)      253 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-client-libs.install
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-client-libs.postinst
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-client-libs.postrm
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-client.install
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-devel.install
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-libs.install
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-libs.postinst
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-libs.postrm
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-private-devel.install
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-server-devel.install
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-server-libs.install
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-server-libs.postinst
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian/xrootd-server-libs.postrm
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/packaging/debian_scripts/
--rwxr-xr-x   0 root         (0) root         (0)     1741 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/debian_scripts/publish_debian_cern.sh
--rwxr-xr-x   0 root         (0) root         (0)     8169 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/makesrpm.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/packaging/rhel/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/packaging/rhel/xrootd-ceph.spec.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/src/
--rw-r--r--   0 root         (0) root         (0)      341 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/
--rw-r--r--   0 root         (0) root         (0)     8360 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOss.cc
--rw-r--r--   0 root         (0) root         (0)     3728 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOss.hh
--rw-r--r--   0 root         (0) root         (0)     2049 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssDir.cc
--rw-r--r--   0 root         (0) root         (0)     3121 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssDir.hh
--rw-r--r--   0 root         (0) root         (0)     3209 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssFile.cc
--rw-r--r--   0 root         (0) root         (0)     3330 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssFile.hh
--rw-r--r--   0 root         (0) root         (0)    43976 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephPosix.cc
--rw-r--r--   0 root         (0) root         (0)     3885 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephPosix.hh
--rw-r--r--   0 root         (0) root         (0)     3838 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephXAttr.cc
--rw-r--r--   0 root         (0) root         (0)     7877 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephXAttr.hh
--rw-r--r--   0 root         (0) root         (0)     2369 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdCeph.cmake
--rw-r--r--   0 root         (0) root         (0)     5174 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/src/XrdVersion.hh.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/tests/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.767900 xrootd-5.6.0/src/XrdCeph/tests/XrdCephTests/
--rw-r--r--   0 root         (0) root         (0)      672 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/tests/XrdCephTests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6661 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCeph/tests/XrdCephTests/CephParsingTest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.777900 xrootd-5.6.0/src/XrdCks/
--rw-r--r--   0 root         (0) root         (0)    16444 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCks.hh
--rw-r--r--   0 root         (0) root         (0)     7765 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksAssist.cc
--rw-r--r--   0 root         (0) root         (0)     6718 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksAssist.hh
--rw-r--r--   0 root         (0) root         (0)     8525 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalc.hh
--rw-r--r--   0 root         (0) root         (0)     5687 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalcadler32.hh
--rw-r--r--   0 root         (0) root         (0)     8639 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32.cc
--rw-r--r--   0 root         (0) root         (0)     3654 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32.hh
--rw-r--r--   0 root         (0) root         (0)     1003 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32C.cc
--rw-r--r--   0 root         (0) root         (0)     2986 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32C.hh
--rw-r--r--   0 root         (0) root         (0)    12260 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalcmd5.cc
--rw-r--r--   0 root         (0) root         (0)     3564 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalcmd5.hh
--rw-r--r--   0 root         (0) root         (0)     5036 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksCalczcrc32.cc
--rw-r--r--   0 root         (0) root         (0)    10222 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksConfig.cc
--rw-r--r--   0 root         (0) root         (0)     3663 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksConfig.hh
--rw-r--r--   0 root         (0) root         (0)     5671 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksData.hh
--rw-r--r--   0 root         (0) root         (0)     7928 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksLoader.cc
--rw-r--r--   0 root         (0) root         (0)     6105 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksLoader.hh
--rw-r--r--   0 root         (0) root         (0)     9341 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksManOss.cc
--rw-r--r--   0 root         (0) root         (0)     3480 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksManOss.hh
--rw-r--r--   0 root         (0) root         (0)    21161 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksManager.cc
--rw-r--r--   0 root         (0) root         (0)     5041 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksManager.hh
--rw-r--r--   0 root         (0) root         (0)    14952 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksWrapper.hh
--rw-r--r--   0 root         (0) root         (0)     4283 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCks/XrdCksXAttr.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.787901 xrootd-5.6.0/src/XrdCl/
--rw-r--r--   0 root         (0) root         (0)     8568 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5609 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAnyObject.hh
--rw-r--r--   0 root         (0) root         (0)     3364 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClApply.hh
--rw-r--r--   0 root         (0) root         (0)    13157 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClArg.hh
--rw-r--r--   0 root         (0) root         (0)     3439 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncDiscardReader.hh
--rw-r--r--   0 root         (0) root         (0)     7661 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncHSReader.hh
--rw-r--r--   0 root         (0) root         (0)     5998 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncHSWriter.hh
--rw-r--r--   0 root         (0) root         (0)    15590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncMsgReader.hh
--rw-r--r--   0 root         (0) root         (0)    10892 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncMsgWriter.hh
--rw-r--r--   0 root         (0) root         (0)    12785 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncPageReader.hh
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncRawReader.hh
--rw-r--r--   0 root         (0) root         (0)     7097 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncRawReaderIntfc.hh
--rw-r--r--   0 root         (0) root         (0)    35077 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncSocketHandler.cc
--rw-r--r--   0 root         (0) root         (0)    13692 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncSocketHandler.hh
--rw-r--r--   0 root         (0) root         (0)    11781 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClAsyncVectorReader.hh
--rw-r--r--   0 root         (0) root         (0)     9115 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClBuffer.hh
--rw-r--r--   0 root         (0) root         (0)     9000 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClChannel.cc
--rw-r--r--   0 root         (0) root         (0)     7455 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClChannel.hh
--rw-r--r--   0 root         (0) root         (0)     2701 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClChannelHandlerList.cc
--rw-r--r--   0 root         (0) root         (0)     2547 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClChannelHandlerList.hh
--rw-r--r--   0 root         (0) root         (0)     5702 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCheckSumHelper.hh
--rw-r--r--   0 root         (0) root         (0)     5843 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCheckSumManager.cc
--rw-r--r--   0 root         (0) root         (0)     3367 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCheckSumManager.hh
--rw-r--r--   0 root         (0) root         (0)     8890 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCheckpointOperation.hh
--rw-r--r--   0 root         (0) root         (0)   109531 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClClassicCopyJob.cc
--rw-r--r--   0 root         (0) root         (0)     3921 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClClassicCopyJob.hh
--rw-r--r--   0 root         (0) root         (0)     9840 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClConstants.hh
--rw-r--r--   0 root         (0) root         (0)    33054 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCopy.cc
--rw-r--r--   0 root         (0) root         (0)     4256 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCopyJob.hh
--rw-r--r--   0 root         (0) root         (0)    21403 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCopyProcess.cc
--rw-r--r--   0 root         (0) root         (0)     9463 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCopyProcess.hh
--rw-r--r--   0 root         (0) root         (0)     4723 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClCtx.hh
--rw-r--r--   0 root         (0) root         (0)    34739 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClDefaultEnv.cc
--rw-r--r--   0 root         (0) root         (0)     8248 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClDefaultEnv.hh
--rw-r--r--   0 root         (0) root         (0)     2452 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClDlgEnv.hh
--rw-r--r--   0 root         (0) root         (0)     7058 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClEcHandler.cc
--rw-r--r--   0 root         (0) root         (0)    17884 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClEcHandler.hh
--rw-r--r--   0 root         (0) root         (0)     8264 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClEnv.cc
--rw-r--r--   0 root         (0) root         (0)     7930 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClEnv.hh
--rw-r--r--   0 root         (0) root         (0)    79044 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFS.cc
--rw-r--r--   0 root         (0) root         (0)     3598 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFSExecutor.cc
--rw-r--r--   0 root         (0) root         (0)     4052 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFSExecutor.hh
--rw-r--r--   0 root         (0) root         (0)    35374 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFile.cc
--rw-r--r--   0 root         (0) root         (0)    43555 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFile.hh
--rw-r--r--   0 root         (0) root         (0)    61991 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileOperations.hh
--rw-r--r--   0 root         (0) root         (0)   134550 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileStateHandler.cc
--rw-r--r--   0 root         (0) root         (0)    49347 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileStateHandler.hh
--rw-r--r--   0 root         (0) root         (0)    82862 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileSystem.cc
--rw-r--r--   0 root         (0) root         (0)    47082 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileSystem.hh
--rw-r--r--   0 root         (0) root         (0)    58105 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileSystemOperations.hh
--rw-r--r--   0 root         (0) root         (0)     7347 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileSystemUtils.cc
--rw-r--r--   0 root         (0) root         (0)     3917 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileSystemUtils.hh
--rw-r--r--   0 root         (0) root         (0)     1775 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileTimer.cc
--rw-r--r--   0 root         (0) root         (0)     3561 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFileTimer.hh
--rw-r--r--   0 root         (0) root         (0)     2754 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFinalOperation.hh
--rw-r--r--   0 root         (0) root         (0)     4753 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClForkHandler.cc
--rw-r--r--   0 root         (0) root         (0)     4421 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClForkHandler.hh
--rw-r--r--   0 root         (0) root         (0)     9899 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClFwd.hh
--rw-r--r--   0 root         (0) root         (0)     6373 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClInQueue.cc
--rw-r--r--   0 root         (0) root         (0)     4732 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClInQueue.hh
--rw-r--r--   0 root         (0) root         (0)     5126 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClJobManager.cc
--rw-r--r--   0 root         (0) root         (0)     4860 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClJobManager.hh
--rw-r--r--   0 root         (0) root         (0)    36455 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClLocalFileHandler.cc
--rw-r--r--   0 root         (0) root         (0)    17612 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClLocalFileHandler.hh
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClLocalFileTask.cc
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClLocalFileTask.hh
--rw-r--r--   0 root         (0) root         (0)     9775 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClLog.cc
--rw-r--r--   0 root         (0) root         (0)    10484 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClLog.hh
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClMessage.hh
--rw-r--r--   0 root         (0) root         (0)    20035 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClMessageUtils.cc
--rw-r--r--   0 root         (0) root         (0)    12633 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClMessageUtils.hh
--rw-r--r--   0 root         (0) root         (0)    18515 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClMetalinkRedirector.cc
--rw-r--r--   0 root         (0) root         (0)     8397 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClMetalinkRedirector.hh
--rw-r--r--   0 root         (0) root         (0)    10542 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClMonitor.hh
--rw-r--r--   0 root         (0) root         (0)    29362 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOperationHandlers.hh
--rw-r--r--   0 root         (0) root         (0)     1066 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOperationTimeout.hh
--rw-r--r--   0 root         (0) root         (0)     9955 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOperations.cc
--rw-r--r--   0 root         (0) root         (0)    31192 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOperations.hh
--rw-r--r--   0 root         (0) root         (0)     1295 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOptimizers.hh
--rw-r--r--   0 root         (0) root         (0)     6499 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOptional.hh
--rw-r--r--   0 root         (0) root         (0)     5396 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOutQueue.cc
--rw-r--r--   0 root         (0) root         (0)     6707 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClOutQueue.hh
--rw-r--r--   0 root         (0) root         (0)    22037 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClParallelOperation.hh
--rw-r--r--   0 root         (0) root         (0)    26771 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPlugInInterface.hh
--rw-r--r--   0 root         (0) root         (0)    18005 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPlugInManager.cc
--rw-r--r--   0 root         (0) root         (0)     7482 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPlugInManager.hh
--rw-r--r--   0 root         (0) root         (0)     7217 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPoller.hh
--rw-r--r--   0 root         (0) root         (0)    20602 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPollerBuiltIn.cc
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPollerBuiltIn.hh
--rw-r--r--   0 root         (0) root         (0)     3701 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPollerFactory.cc
--rw-r--r--   0 root         (0) root         (0)     2014 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPollerFactory.hh
--rw-r--r--   0 root         (0) root         (0)    18072 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPostMaster.cc
--rw-r--r--   0 root         (0) root         (0)     9880 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPostMaster.hh
--rw-r--r--   0 root         (0) root         (0)    24240 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPostMasterInterfaces.hh
--rw-r--r--   0 root         (0) root         (0)    11305 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClPropertyList.hh
--rw-r--r--   0 root         (0) root         (0)     4552 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClRedirectorRegistry.cc
--rw-r--r--   0 root         (0) root         (0)     8258 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClRedirectorRegistry.hh
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClRequestSync.hh
--rw-r--r--   0 root         (0) root         (0)     2659 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClResponseJob.hh
--rw-r--r--   0 root         (0) root         (0)     7628 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClSIDManager.cc
--rw-r--r--   0 root         (0) root         (0)     8555 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClSIDManager.hh
--rw-r--r--   0 root         (0) root         (0)    30690 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClSocket.cc
--rw-r--r--   0 root         (0) root         (0)    15672 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClSocket.hh
--rw-r--r--   0 root         (0) root         (0)     5694 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClStatus.cc
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClStatus.hh
--rw-r--r--   0 root         (0) root         (0)    48094 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClStream.cc
--rw-r--r--   0 root         (0) root         (0)    16875 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClStream.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClSyncQueue.hh
--rw-r--r--   0 root         (0) root         (0)     3609 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTPFallBackCopyJob.cc
--rw-r--r--   0 root         (0) root         (0)     2541 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTPFallBackCopyJob.hh
--rw-r--r--   0 root         (0) root         (0)     8986 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTaskManager.cc
--rw-r--r--   0 root         (0) root         (0)     6199 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTaskManager.hh
--rw-r--r--   0 root         (0) root         (0)    34437 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClThirdPartyCopyJob.cc
--rw-r--r--   0 root         (0) root         (0)     3740 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClThirdPartyCopyJob.hh
--rw-r--r--   0 root         (0) root         (0)    15842 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTls.cc
--rw-r--r--   0 root         (0) root         (0)     6552 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTls.hh
--rw-r--r--   0 root         (0) root         (0)     3056 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTransportManager.cc
--rw-r--r--   0 root         (0) root         (0)     2786 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClTransportManager.hh
--rw-r--r--   0 root         (0) root         (0)    17135 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClURL.cc
--rw-r--r--   0 root         (0) root         (0)    11760 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClURL.hh
--rw-r--r--   0 root         (0) root         (0)    32898 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClUtils.cc
--rw-r--r--   0 root         (0) root         (0)    18037 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClUtils.hh
--rw-r--r--   0 root         (0) root         (0)     5297 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXCpCtx.cc
--rw-r--r--   0 root         (0) root         (0)     8289 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXCpCtx.hh
--rw-r--r--   0 root         (0) root         (0)    17327 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXCpSrc.cc
--rw-r--r--   0 root         (0) root         (0)     9459 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXCpSrc.hh
--rw-r--r--   0 root         (0) root         (0)    94961 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXRootDMsgHandler.cc
--rw-r--r--   0 root         (0) root         (0)    28694 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXRootDMsgHandler.hh
--rw-r--r--   0 root         (0) root         (0)    26744 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXRootDResponses.cc
--rw-r--r--   0 root         (0) root         (0)    45771 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXRootDResponses.hh
--rw-r--r--   0 root         (0) root         (0)   130343 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXRootDTransport.cc
--rw-r--r--   0 root         (0) root         (0)    22673 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClXRootDTransport.hh
--rw-r--r--   0 root         (0) root         (0)    43178 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClZipArchive.cc
--rw-r--r--   0 root         (0) root         (0)    28344 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClZipArchive.hh
--rw-r--r--   0 root         (0) root         (0)     8602 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClZipCache.hh
--rw-r--r--   0 root         (0) root         (0)     4065 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClZipListHandler.cc
--rw-r--r--   0 root         (0) root         (0)     5224 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClZipListHandler.hh
--rw-r--r--   0 root         (0) root         (0)    27700 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCl/XrdClZipOperations.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.797901 xrootd-5.6.0/src/XrdClHttp/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    13948 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpFilePlugIn.cc
--rw-r--r--   0 root         (0) root         (0)     5602 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpFilePlugIn.hh
--rw-r--r--   0 root         (0) root         (0)     7554 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc
--rw-r--r--   0 root         (0) root         (0)     1885 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpPlugInFactory.cc
--rw-r--r--   0 root         (0) root         (0)      481 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpPlugInFactory.hh
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpPlugInUtil.cc
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpPlugInUtil.hh
--rw-r--r--   0 root         (0) root         (0)    16027 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpPosix.cc
--rw-r--r--   0 root         (0) root         (0)     2617 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdClHttp/XrdClHttpPosix.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.807901 xrootd-5.6.0/src/XrdCms/
--rw-r--r--   0 root         (0) root         (0)    29034 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsAdmin.cc
--rw-r--r--   0 root         (0) root         (0)     3908 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsAdmin.hh
--rw-r--r--   0 root         (0) root         (0)    15740 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsBaseFS.cc
--rw-r--r--   0 root         (0) root         (0)     8998 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsBaseFS.hh
--rw-r--r--   0 root         (0) root         (0)    19325 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsBlackList.cc
--rw-r--r--   0 root         (0) root         (0)     5380 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsBlackList.hh
--rw-r--r--   0 root         (0) root         (0)    21145 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsCache.cc
--rw-r--r--   0 root         (0) root         (0)     5021 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsCache.hh
--rw-r--r--   0 root         (0) root         (0)     3239 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClient.cc
--rw-r--r--   0 root         (0) root         (0)    22441 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClient.hh
--rw-r--r--   0 root         (0) root         (0)    25549 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClientConfig.cc
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClientConfig.hh
--rw-r--r--   0 root         (0) root         (0)    17324 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClientMan.cc
--rw-r--r--   0 root         (0) root         (0)     5101 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClientMan.hh
--rw-r--r--   0 root         (0) root         (0)     7117 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClientMsg.cc
--rw-r--r--   0 root         (0) root         (0)     3740 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClientMsg.hh
--rw-r--r--   0 root         (0) root         (0)     8243 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClustID.cc
--rw-r--r--   0 root         (0) root         (0)     3382 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsClustID.hh
--rw-r--r--   0 root         (0) root         (0)    77195 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsCluster.cc
--rw-r--r--   0 root         (0) root         (0)    10458 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsCluster.hh
--rw-r--r--   0 root         (0) root         (0)   109427 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsConfig.cc
--rw-r--r--   0 root         (0) root         (0)    12336 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsConfig.hh
--rw-r--r--   0 root         (0) root         (0)    49369 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsFinder.cc
--rw-r--r--   0 root         (0) root         (0)     6835 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsFinder.hh
--rw-r--r--   0 root         (0) root         (0)     5106 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsJob.cc
--rw-r--r--   0 root         (0) root         (0)     3058 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsJob.hh
--rw-r--r--   0 root         (0) root         (0)     8643 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsKey.cc
--rw-r--r--   0 root         (0) root         (0)     6829 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsKey.hh
--rw-r--r--   0 root         (0) root         (0)    10887 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsLogin.cc
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsLogin.hh
--rw-r--r--   0 root         (0) root         (0)     8263 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsManList.cc
--rw-r--r--   0 root         (0) root         (0)     3563 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsManList.hh
--rw-r--r--   0 root         (0) root         (0)     9115 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsManTree.cc
--rw-r--r--   0 root         (0) root         (0)     3708 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsManTree.hh
--rw-r--r--   0 root         (0) root         (0)    20171 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsManager.cc
--rw-r--r--   0 root         (0) root         (0)     4549 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsManager.hh
--rw-r--r--   0 root         (0) root         (0)    21971 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsMeter.cc
--rw-r--r--   0 root         (0) root         (0)     4787 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsMeter.hh
--rw-r--r--   0 root         (0) root         (0)     6578 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsNash.cc
--rw-r--r--   0 root         (0) root         (0)     3101 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsNash.hh
--rw-r--r--   0 root         (0) root         (0)    68022 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsNode.cc
--rw-r--r--   0 root         (0) root         (0)    11829 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsNode.hh
--rw-r--r--   0 root         (0) root         (0)     7875 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPList.cc
--rw-r--r--   0 root         (0) root         (0)     5436 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPList.hh
--rw-r--r--   0 root         (0) root         (0)    18983 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsParser.cc
--rw-r--r--   0 root         (0) root         (0)     4888 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsParser.hh
--rw-r--r--   0 root         (0) root         (0)     7886 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPerfMon.hh
--rw-r--r--   0 root         (0) root         (0)     6042 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPrepArgs.cc
--rw-r--r--   0 root         (0) root         (0)     3669 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPrepArgs.hh
--rw-r--r--   0 root         (0) root         (0)    18512 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPrepare.cc
--rw-r--r--   0 root         (0) root         (0)     4068 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsPrepare.hh
--rw-r--r--   0 root         (0) root         (0)    46734 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsProtocol.cc
--rw-r--r--   0 root         (0) root         (0)     5039 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsProtocol.hh
--rw-r--r--   0 root         (0) root         (0)     3945 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRRData.cc
--rw-r--r--   0 root         (0) root         (0)     4633 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRRData.hh
--rw-r--r--   0 root         (0) root         (0)    17719 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRRQ.cc
--rw-r--r--   0 root         (0) root         (0)     7590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRRQ.hh
--rw-r--r--   0 root         (0) root         (0)     5228 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRTable.cc
--rw-r--r--   0 root         (0) root         (0)     3076 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRTable.hh
--rw-r--r--   0 root         (0) root         (0)     9893 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRedirLocal.cc
--rw-r--r--   0 root         (0) root         (0)     3519 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRedirLocal.hh
--rw-r--r--   0 root         (0) root         (0)    11036 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsResp.cc
--rw-r--r--   0 root         (0) root         (0)     5382 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsResp.hh
--rw-r--r--   0 root         (0) root         (0)     5917 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRole.hh
--rw-r--r--   0 root         (0) root         (0)    11602 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRouting.cc
--rw-r--r--   0 root         (0) root         (0)     4838 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsRouting.hh
--rw-r--r--   0 root         (0) root         (0)    14804 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsSecurity.cc
--rw-r--r--   0 root         (0) root         (0)     3468 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsSecurity.hh
--rw-r--r--   0 root         (0) root         (0)     7463 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsSelect.hh
--rw-r--r--   0 root         (0) root         (0)    11542 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsState.cc
--rw-r--r--   0 root         (0) root         (0)     3997 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsState.hh
--rw-r--r--   0 root         (0) root         (0)     5187 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsSupervisor.cc
--rw-r--r--   0 root         (0) root         (0)     2750 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsSupervisor.hh
--rw-r--r--   0 root         (0) root         (0)     5637 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsTalk.cc
--rw-r--r--   0 root         (0) root         (0)     3034 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsTalk.hh
--rw-r--r--   0 root         (0) root         (0)     3426 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsTrace.hh
--rw-r--r--   0 root         (0) root         (0)     2782 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsTypes.hh
--rw-r--r--   0 root         (0) root         (0)    11723 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsUtils.cc
--rw-r--r--   0 root         (0) root         (0)     6365 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsUtils.hh
--rw-r--r--   0 root         (0) root         (0)     5656 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCms/XrdCmsVnId.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.807901 xrootd-5.6.0/src/XrdCrypto/
--rw-r--r--   0 root         (0) root         (0)     4302 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoAux.cc
--rw-r--r--   0 root         (0) root         (0)     5058 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoAux.hh
--rw-r--r--   0 root         (0) root         (0)     7678 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoBasic.cc
--rw-r--r--   0 root         (0) root         (0)     3869 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoBasic.hh
--rw-r--r--   0 root         (0) root         (0)     7405 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoCipher.cc
--rw-r--r--   0 root         (0) root         (0)     4214 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoCipher.hh
--rw-r--r--   0 root         (0) root         (0)    17653 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoFactory.cc
--rw-r--r--   0 root         (0) root         (0)     9138 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoFactory.hh
--rw-r--r--   0 root         (0) root         (0)     3500 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoLite.cc
--rw-r--r--   0 root         (0) root         (0)     5355 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoLite.hh
--rw-r--r--   0 root         (0) root         (0)     8734 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoLite_bf32.cc
--rw-r--r--   0 root         (0) root         (0)     4136 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoMsgDigest.cc
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoMsgDigest.hh
--rw-r--r--   0 root         (0) root         (0)     9058 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoRSA.cc
--rw-r--r--   0 root         (0) root         (0)     4804 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoRSA.hh
--rw-r--r--   0 root         (0) root         (0)     2994 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoTrace.hh
--rw-r--r--   0 root         (0) root         (0)    10639 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509.cc
--rw-r--r--   0 root         (0) root         (0)     5644 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509.hh
--rw-r--r--   0 root         (0) root         (0)    27273 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Chain.cc
--rw-r--r--   0 root         (0) root         (0)     7661 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Chain.hh
--rw-r--r--   0 root         (0) root         (0)     5674 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Crl.cc
--rw-r--r--   0 root         (0) root         (0)     4052 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Crl.hh
--rw-r--r--   0 root         (0) root         (0)     5256 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Req.cc
--rw-r--r--   0 root         (0) root         (0)     4177 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Req.hh
--rw-r--r--   0 root         (0) root         (0)    10162 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptogsiX509Chain.cc
--rw-r--r--   0 root         (0) root         (0)     3952 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptogsiX509Chain.hh
--rw-r--r--   0 root         (0) root         (0)    25131 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslAux.cc
--rw-r--r--   0 root         (0) root         (0)     7231 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslAux.hh
--rw-r--r--   0 root         (0) root         (0)    43961 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslCipher.cc
--rw-r--r--   0 root         (0) root         (0)     4814 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslCipher.hh
--rw-r--r--   0 root         (0) root         (0)    16817 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslFactory.cc
--rw-r--r--   0 root         (0) root         (0)     5208 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslFactory.hh
--rw-r--r--   0 root         (0) root         (0)     6084 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslMsgDigest.cc
--rw-r--r--   0 root         (0) root         (0)     3376 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslMsgDigest.hh
--rw-r--r--   0 root         (0) root         (0)    20952 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslRSA.cc
--rw-r--r--   0 root         (0) root         (0)     4241 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslRSA.hh
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslTrace.hh
--rw-r--r--   0 root         (0) root         (0)    36214 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509.cc
--rw-r--r--   0 root         (0) root         (0)     5787 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509.hh
--rw-r--r--   0 root         (0) root         (0)    20566 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Crl.cc
--rw-r--r--   0 root         (0) root         (0)     5006 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Crl.hh
--rw-r--r--   0 root         (0) root         (0)    12043 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Req.cc
--rw-r--r--   0 root         (0) root         (0)     4113 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Req.hh
--rw-r--r--   0 root         (0) root         (0)    52085 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptosslgsiAux.cc
--rw-r--r--   0 root         (0) root         (0)    18878 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto/XrdCryptotest.cc
--rw-r--r--   0 root         (0) root         (0)     4042 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdCrypto.cmake
--rw-r--r--   0 root         (0) root         (0)     2904 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDaemons.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.807901 xrootd-5.6.0/src/XrdDig/
--rw-r--r--   0 root         (0) root         (0)    14689 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDig/XrdDigAuth.cc
--rw-r--r--   0 root         (0) root         (0)     4337 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDig/XrdDigAuth.hh
--rw-r--r--   0 root         (0) root         (0)    21474 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDig/XrdDigConfig.cc
--rw-r--r--   0 root         (0) root         (0)     3831 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDig/XrdDigConfig.hh
--rw-r--r--   0 root         (0) root         (0)    28757 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDig/XrdDigFS.cc
--rw-r--r--   0 root         (0) root         (0)    11645 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdDig/XrdDigFS.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.807901 xrootd-5.6.0/src/XrdEc/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2020 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/README
--rw-r--r--   0 root         (0) root         (0)     3708 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcConfig.hh
--rw-r--r--   0 root         (0) root         (0)     3424 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcObjCfg.hh
--rw-r--r--   0 root         (0) root         (0)    47577 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcReader.cc
--rw-r--r--   0 root         (0) root         (0)     8804 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcReader.hh
--rw-r--r--   0 root         (0) root         (0)     9779 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcRedundancyProvider.cc
--rw-r--r--   0 root         (0) root         (0)     5127 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcRedundancyProvider.hh
--rw-r--r--   0 root         (0) root         (0)    17345 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcStrmWriter.cc
--rw-r--r--   0 root         (0) root         (0)    13309 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcStrmWriter.hh
--rw-r--r--   0 root         (0) root         (0)     7256 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcThreadPool.hh
--rw-r--r--   0 root         (0) root         (0)     3689 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcUtilities.cc
--rw-r--r--   0 root         (0) root         (0)     9976 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcUtilities.hh
--rw-r--r--   0 root         (0) root         (0)    12505 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdEc/XrdEcWrtBuff.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.817901 xrootd-5.6.0/src/XrdFfs/
--rw-r--r--   0 root         (0) root         (0)     6405 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/README
--rw-r--r--   0 root         (0) root         (0)    10875 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsDent.cc
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsDent.hh
--rw-r--r--   0 root         (0) root         (0)     5321 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsFsinfo.cc
--rw-r--r--   0 root         (0) root         (0)     2539 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsFsinfo.hh
--rw-r--r--   0 root         (0) root         (0)    13902 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsMisc.cc
--rw-r--r--   0 root         (0) root         (0)     3054 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsMisc.hh
--rw-r--r--   0 root         (0) root         (0)    26410 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsPosix.cc
--rw-r--r--   0 root         (0) root         (0)     4855 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsPosix.hh
--rw-r--r--   0 root         (0) root         (0)    10077 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsQueue.cc
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsQueue.hh
--rw-r--r--   0 root         (0) root         (0)    11980 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsWcache.cc
--rw-r--r--   0 root         (0) root         (0)     2664 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsWcache.hh
--rw-r--r--   0 root         (0) root         (0)    48045 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/XrdFfsXrootdfs.cc
--rwxr-xr-x   0 root         (0) root         (0)     1608 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs/xrootdfs.template
--rw-r--r--   0 root         (0) root         (0)     1905 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFfs.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.817901 xrootd-5.6.0/src/XrdFrc/
--rw-r--r--   0 root         (0) root         (0)    11084 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcCID.cc
--rw-r--r--   0 root         (0) root         (0)     3950 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcCID.hh
--rw-r--r--   0 root         (0) root         (0)    11618 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcProxy.cc
--rw-r--r--   0 root         (0) root         (0)     3742 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcProxy.hh
--rw-r--r--   0 root         (0) root         (0)     8762 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcReqAgent.cc
--rw-r--r--   0 root         (0) root         (0)     3073 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcReqAgent.hh
--rw-r--r--   0 root         (0) root         (0)    21187 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcReqFile.cc
--rw-r--r--   0 root         (0) root         (0)     4017 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcReqFile.hh
--rw-r--r--   0 root         (0) root         (0)     4547 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcRequest.hh
--rw-r--r--   0 root         (0) root         (0)     2728 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcTrace.cc
--rw-r--r--   0 root         (0) root         (0)     3411 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcTrace.hh
--rw-r--r--   0 root         (0) root         (0)    11388 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcUtils.cc
--rw-r--r--   0 root         (0) root         (0)     3289 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcUtils.hh
--rw-r--r--   0 root         (0) root         (0)     8162 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcXAttr.hh
--rw-r--r--   0 root         (0) root         (0)     2863 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrc/XrdFrcXLock.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.817901 xrootd-5.6.0/src/XrdFrm/
--rw-r--r--   0 root         (0) root         (0)    36149 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdmin.cc
--rw-r--r--   0 root         (0) root         (0)     7410 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdmin.hh
--rw-r--r--   0 root         (0) root         (0)    24369 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminAudit.cc
--rw-r--r--   0 root         (0) root         (0)    13623 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminFiles.cc
--rw-r--r--   0 root         (0) root         (0)    11144 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminFind.cc
--rw-r--r--   0 root         (0) root         (0)     6820 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminMain.cc
--rw-r--r--   0 root         (0) root         (0)    10240 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminQuery.cc
--rw-r--r--   0 root         (0) root         (0)     9903 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminReloc.cc
--rw-r--r--   0 root         (0) root         (0)     9421 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmAdminUnlink.cc
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmCns.cc
--rw-r--r--   0 root         (0) root         (0)     3675 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmCns.hh
--rw-r--r--   0 root         (0) root         (0)    71617 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmConfig.cc
--rw-r--r--   0 root         (0) root         (0)     8419 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmConfig.hh
--rw-r--r--   0 root         (0) root         (0)    17426 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmFiles.cc
--rw-r--r--   0 root         (0) root         (0)     6386 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmFiles.hh
--rw-r--r--   0 root         (0) root         (0)    11087 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmMigrate.cc
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmMigrate.hh
--rw-r--r--   0 root         (0) root         (0)    11528 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmMonitor.cc
--rw-r--r--   0 root         (0) root         (0)     3912 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmMonitor.hh
--rw-r--r--   0 root         (0) root         (0)     9482 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmPurgMain.cc
--rw-r--r--   0 root         (0) root         (0)    32604 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmPurge.cc
--rw-r--r--   0 root         (0) root         (0)     5353 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmPurge.hh
--rw-r--r--   0 root         (0) root         (0)     7763 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmReqBoss.cc
--rw-r--r--   0 root         (0) root         (0)     3059 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmReqBoss.hh
--rw-r--r--   0 root         (0) root         (0)     7051 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmTSort.cc
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmTSort.hh
--rw-r--r--   0 root         (0) root         (0)    30228 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmTransfer.cc
--rw-r--r--   0 root         (0) root         (0)     3349 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmTransfer.hh
--rw-r--r--   0 root         (0) root         (0)    10414 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrAgent.cc
--rw-r--r--   0 root         (0) root         (0)     3098 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrAgent.hh
--rw-r--r--   0 root         (0) root         (0)     7971 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrDaemon.cc
--rw-r--r--   0 root         (0) root         (0)     2782 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrDaemon.hh
--rw-r--r--   0 root         (0) root         (0)     2832 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrJob.hh
--rw-r--r--   0 root         (0) root         (0)     6343 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrMain.cc
--rw-r--r--   0 root         (0) root         (0)    17722 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrQueue.cc
--rw-r--r--   0 root         (0) root         (0)     4118 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm/XrdFrmXfrQueue.hh
--rw-r--r--   0 root         (0) root         (0)     3292 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdFrm.cmake
--rw-r--r--   0 root         (0) root         (0)     4663 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHeaders.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.817901 xrootd-5.6.0/src/XrdHttp/
--rw-r--r--   0 root         (0) root         (0)     1000 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/README-CKSUM.md
--rw-r--r--   0 root         (0) root         (0)     1909 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpChecksum.cc
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpChecksum.hh
--rw-r--r--   0 root         (0) root         (0)     5702 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpChecksumHandler.cc
--rw-r--r--   0 root         (0) root         (0)     5188 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpChecksumHandler.hh
--rw-r--r--   0 root         (0) root         (0)     3696 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpExtHandler.cc
--rw-r--r--   0 root         (0) root         (0)     6073 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpExtHandler.hh
--rw-r--r--   0 root         (0) root         (0)     2306 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpModule.cc
--rw-r--r--   0 root         (0) root         (0)    86927 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpProtocol.cc
--rw-r--r--   0 root         (0) root         (0)    14055 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpProtocol.hh
--rw-r--r--   0 root         (0) root         (0)    89263 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpReq.cc
--rw-r--r--   0 root         (0) root         (0)    14529 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpReq.hh
--rw-r--r--   0 root         (0) root         (0)     4252 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpSecXtractor.hh
--rw-r--r--   0 root         (0) root         (0)     8841 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpSecurity.cc
--rw-r--r--   0 root         (0) root         (0)     1661 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpStatic.hh
--rw-r--r--   0 root         (0) root         (0)     2175 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpTrace.hh
--rw-r--r--   0 root         (0) root         (0)     9423 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpUtils.cc
--rw-r--r--   0 root         (0) root         (0)     2321 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/XrdHttpUtils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.817901 xrootd-5.6.0/src/XrdHttp/static/
--rw-r--r--   0 root         (0) root         (0)     1400 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/static/xrdhttp.css
--rw-r--r--   0 root         (0) root         (0)     7951 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/static/xrdhttp_css.h
--rw-r--r--   0 root         (0) root         (0)     8705 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/static/xrdhttp_favicon_ico.h
--rw-r--r--   0 root         (0) root         (0)     2784 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/xrootd-http-rdr.cf
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp/xrootd-http.cf
--rw-r--r--   0 root         (0) root         (0)     2494 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdHttp.cmake
--rw-r--r--   0 root         (0) root         (0)     1578 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdIsal.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.827901 xrootd-5.6.0/src/XrdMacaroons/
--rw-r--r--   0 root         (0) root         (0)     2798 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/README.md
--rw-r--r--   0 root         (0) root         (0)     4922 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/XrdMacaroons.cc
--rw-r--r--   0 root         (0) root         (0)    18196 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsAuthz.cc
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsAuthz.hh
--rw-r--r--   0 root         (0) root         (0)     6883 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsConfigure.cc
--rw-r--r--   0 root         (0) root         (0)    21521 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsHandler.cc
--rw-r--r--   0 root         (0) root         (0)     2784 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsHandler.hh
--rw-r--r--   0 root         (0) root         (0)      122 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/export-lib-symbols
--rwxr-xr-x   0 root         (0) root         (0)     5269 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons/macaroon-init
--rw-r--r--   0 root         (0) root         (0)     1631 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdMacaroons.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.827901 xrootd-5.6.0/src/XrdNet/
--rw-r--r--   0 root         (0) root         (0)    17923 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNet.cc
--rw-r--r--   0 root         (0) root         (0)    14669 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNet.hh
--rw-r--r--   0 root         (0) root         (0)    21048 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetAddr.cc
--rw-r--r--   0 root         (0) root         (0)    15050 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetAddr.hh
--rw-r--r--   0 root         (0) root         (0)    17812 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetAddrInfo.cc
--rw-r--r--   0 root         (0) root         (0)    17695 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetAddrInfo.hh
--rw-r--r--   0 root         (0) root         (0)     5823 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetBuffer.cc
--rw-r--r--   0 root         (0) root         (0)     3948 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetBuffer.hh
--rw-r--r--   0 root         (0) root         (0)     8210 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetCache.cc
--rw-r--r--   0 root         (0) root         (0)     5934 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetCache.hh
--rw-r--r--   0 root         (0) root         (0)     5742 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetCmsNotify.cc
--rw-r--r--   0 root         (0) root         (0)     2929 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetCmsNotify.hh
--rw-r--r--   0 root         (0) root         (0)     4246 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetConnect.cc
--rw-r--r--   0 root         (0) root         (0)     3196 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetConnect.hh
--rw-r--r--   0 root         (0) root         (0)    31969 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetIF.cc
--rw-r--r--   0 root         (0) root         (0)    20067 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetIF.hh
--rw-r--r--   0 root         (0) root         (0)     6326 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetIdentity.cc
--rw-r--r--   0 root         (0) root         (0)     2701 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetIdentity.hh
--rw-r--r--   0 root         (0) root         (0)     7242 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetMsg.cc
--rw-r--r--   0 root         (0) root         (0)     7458 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetMsg.hh
--rw-r--r--   0 root         (0) root         (0)     4955 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetOpts.hh
--rw-r--r--   0 root         (0) root         (0)     3294 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPMark.cc
--rw-r--r--   0 root         (0) root         (0)     3824 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPMark.hh
--rw-r--r--   0 root         (0) root         (0)    39260 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPMarkCfg.cc
--rw-r--r--   0 root         (0) root         (0)     3755 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPMarkCfg.hh
--rw-r--r--   0 root         (0) root         (0)    13957 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPMarkFF.cc
--rw-r--r--   0 root         (0) root         (0)     3475 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPMarkFF.hh
--rw-r--r--   0 root         (0) root         (0)     2952 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetPeer.hh
--rw-r--r--   0 root         (0) root         (0)     9640 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetRegistry.cc
--rw-r--r--   0 root         (0) root         (0)     6279 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetRegistry.hh
--rw-r--r--   0 root         (0) root         (0)     9596 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetSecurity.cc
--rw-r--r--   0 root         (0) root         (0)     3339 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetSecurity.hh
--rw-r--r--   0 root         (0) root         (0)     3106 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetSockAddr.hh
--rw-r--r--   0 root         (0) root         (0)    18472 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetSocket.cc
--rw-r--r--   0 root         (0) root         (0)     7647 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetSocket.hh
--rw-r--r--   0 root         (0) root         (0)    31024 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetUtils.cc
--rw-r--r--   0 root         (0) root         (0)    24210 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdNet/XrdNetUtils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.837900 xrootd-5.6.0/src/XrdOfs/
--rw-r--r--   0 root         (0) root         (0)    99020 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfs.cc
--rw-r--r--   0 root         (0) root         (0)    21611 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfs.hh
--rw-r--r--   0 root         (0) root         (0)    19274 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsCPFile.cc
--rw-r--r--   0 root         (0) root         (0)     8379 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsCPFile.hh
--rw-r--r--   0 root         (0) root         (0)    11781 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsChkPnt.cc
--rw-r--r--   0 root         (0) root         (0)     6193 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsChkPnt.hh
--rw-r--r--   0 root         (0) root         (0)    77647 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsConfig.cc
--rw-r--r--   0 root         (0) root         (0)    10806 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsConfigCP.cc
--rw-r--r--   0 root         (0) root         (0)     3117 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsConfigCP.hh
--rw-r--r--   0 root         (0) root         (0)    33128 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsConfigPI.cc
--rw-r--r--   0 root         (0) root         (0)    14532 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsConfigPI.hh
--rw-r--r--   0 root         (0) root         (0)    12955 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsEvr.cc
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsEvr.hh
--rw-r--r--   0 root         (0) root         (0)    19534 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsEvs.cc
--rw-r--r--   0 root         (0) root         (0)     7231 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsEvs.hh
--rw-r--r--   0 root         (0) root         (0)    16520 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsFAttr.cc
--rw-r--r--   0 root         (0) root         (0)     4073 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsFS.cc
--rw-r--r--   0 root         (0) root         (0)    13054 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsFSctl.cc
--rw-r--r--   0 root         (0) root         (0)     8921 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsFSctl_PI.hh
--rw-r--r--   0 root         (0) root         (0)    30832 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsHandle.cc
--rw-r--r--   0 root         (0) root         (0)     8197 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsHandle.hh
--rw-r--r--   0 root         (0) root         (0)    13105 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsPoscq.cc
--rw-r--r--   0 root         (0) root         (0)     4134 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsPoscq.hh
--rw-r--r--   0 root         (0) root         (0)    30229 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsPrepGPI.cc
--rw-r--r--   0 root         (0) root         (0)    11518 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsPrepare.hh
--rw-r--r--   0 root         (0) root         (0)     3061 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsSecurity.hh
--rw-r--r--   0 root         (0) root         (0)     3814 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsStats.cc
--rw-r--r--   0 root         (0) root         (0)     3285 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsStats.hh
--rw-r--r--   0 root         (0) root         (0)    23543 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPC.cc
--rw-r--r--   0 root         (0) root         (0)     5117 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPC.hh
--rw-r--r--   0 root         (0) root         (0)    10359 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCAuth.cc
--rw-r--r--   0 root         (0) root         (0)     3086 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCAuth.hh
--rw-r--r--   0 root         (0) root         (0)     3108 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCConfig.hh
--rw-r--r--   0 root         (0) root         (0)     7573 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCInfo.cc
--rw-r--r--   0 root         (0) root         (0)     5241 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCInfo.hh
--rw-r--r--   0 root         (0) root         (0)     7941 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCJob.cc
--rw-r--r--   0 root         (0) root         (0)     3295 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCJob.hh
--rw-r--r--   0 root         (0) root         (0)    13429 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCProg.cc
--rw-r--r--   0 root         (0) root         (0)     3209 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTPCProg.hh
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOfs/XrdOfsTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.837900 xrootd-5.6.0/src/XrdOss/
--rw-r--r--   0 root         (0) root         (0)    11649 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOss.cc
--rw-r--r--   0 root         (0) root         (0)    46028 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOss.hh
--rw-r--r--   0 root         (0) root         (0)    18122 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssAio.cc
--rw-r--r--   0 root         (0) root         (0)    45753 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssApi.cc
--rw-r--r--   0 root         (0) root         (0)    17573 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssApi.hh
--rw-r--r--   0 root         (0) root         (0)     8491 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssAt.cc
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssAt.hh
--rw-r--r--   0 root         (0) root         (0)    31708 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssCache.cc
--rw-r--r--   0 root         (0) root         (0)    11024 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssCache.hh
--rw-r--r--   0 root         (0) root         (0)    73786 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssConfig.cc
--rw-r--r--   0 root         (0) root         (0)     3327 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssConfig.hh
--rw-r--r--   0 root         (0) root         (0)     7753 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssCopy.cc
--rw-r--r--   0 root         (0) root         (0)     2632 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssCopy.hh
--rw-r--r--   0 root         (0) root         (0)    13674 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssCreate.cc
--rw-r--r--   0 root         (0) root         (0)     3641 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssDefaultSS.hh
--rw-r--r--   0 root         (0) root         (0)     4810 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssError.hh
--rw-r--r--   0 root         (0) root         (0)    16583 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssMSS.cc
--rw-r--r--   0 root         (0) root         (0)    11917 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssMio.cc
--rw-r--r--   0 root         (0) root         (0)     3591 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssMio.hh
--rw-r--r--   0 root         (0) root         (0)     2931 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssMioFile.hh
--rw-r--r--   0 root         (0) root         (0)     2987 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssOpaque.hh
--rw-r--r--   0 root         (0) root         (0)    13731 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssPath.cc
--rw-r--r--   0 root         (0) root         (0)     3880 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssPath.hh
--rw-r--r--   0 root         (0) root         (0)     8574 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssReloc.cc
--rw-r--r--   0 root         (0) root         (0)     9890 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssRename.cc
--rw-r--r--   0 root         (0) root         (0)     9051 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssSIgpfsT.cc
--rw-r--r--   0 root         (0) root         (0)    19495 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssSpace.cc
--rw-r--r--   0 root         (0) root         (0)     4240 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssSpace.hh
--rw-r--r--   0 root         (0) root         (0)    18820 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssStage.cc
--rw-r--r--   0 root         (0) root         (0)     4090 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssStage.hh
--rw-r--r--   0 root         (0) root         (0)    21165 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssStat.cc
--rw-r--r--   0 root         (0) root         (0)    10195 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssStatInfo.hh
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssTrace.hh
--rw-r--r--   0 root         (0) root         (0)     8528 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssUnlink.cc
--rw-r--r--   0 root         (0) root         (0)     6673 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssVS.hh
--rw-r--r--   0 root         (0) root         (0)    41503 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOss/XrdOssWrapper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.837900 xrootd-5.6.0/src/XrdOssCsi/
--rw-r--r--   0 root         (0) root         (0)     3167 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/README.md
--rw-r--r--   0 root         (0) root         (0)    15159 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsi.cc
--rw-r--r--   0 root         (0) root         (0)     9618 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsi.hh
--rw-r--r--   0 root         (0) root         (0)     7059 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiConfig.cc
--rw-r--r--   0 root         (0) root         (0)     6756 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiConfig.hh
--rw-r--r--   0 root         (0) root         (0)     2527 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiCrcUtils.cc
--rw-r--r--   0 root         (0) root         (0)     4781 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiCrcUtils.hh
--rw-r--r--   0 root         (0) root         (0)    16745 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiFile.cc
--rw-r--r--   0 root         (0) root         (0)     4448 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiFileAio.cc
--rw-r--r--   0 root         (0) root         (0)    11301 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiFileAio.hh
--rw-r--r--   0 root         (0) root         (0)    29563 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiPages.cc
--rw-r--r--   0 root         (0) root         (0)     9019 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiPages.hh
--rw-r--r--   0 root         (0) root         (0)    34154 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc
--rw-r--r--   0 root         (0) root         (0)     3049 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiRanges.cc
--rw-r--r--   0 root         (0) root         (0)     6143 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiRanges.hh
--rw-r--r--   0 root         (0) root         (0)     3346 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTagstore.hh
--rw-r--r--   0 root         (0) root         (0)     8697 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc
--rw-r--r--   0 root         (0) root         (0)     6892 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh
--rw-r--r--   0 root         (0) root         (0)     3325 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTrace.hh
--rw-r--r--   0 root         (0) root         (0)    10382 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi/XrdOssHandler.hh
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOssCsi.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.857900 xrootd-5.6.0/src/XrdOuc/
--rw-r--r--   0 root         (0) root         (0)     1179 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/README.bonjour
--rw-r--r--   0 root         (0) root         (0)     8818 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucArgs.cc
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucArgs.hh
--rw-r--r--   0 root         (0) root         (0)    17677 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucBackTrace.cc
--rw-r--r--   0 root         (0) root         (0)    10560 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucBackTrace.hh
--rw-r--r--   0 root         (0) root         (0)     9481 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucBuffer.cc
--rw-r--r--   0 root         (0) root         (0)    12583 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucBuffer.hh
--rw-r--r--   0 root         (0) root         (0)    12756 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCRC.cc
--rw-r--r--   0 root         (0) root         (0)     8087 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCRC.hh
--rw-r--r--   0 root         (0) root         (0)    17087 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCRC32C.cc
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCRC32C.hh
--rw-r--r--   0 root         (0) root         (0)     5325 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCache.cc
--rw-r--r--   0 root         (0) root         (0)    37680 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCache.hh
--rw-r--r--   0 root         (0) root         (0)     5225 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCacheCM.hh
--rw-r--r--   0 root         (0) root         (0)     7071 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCacheStats.hh
--rw-r--r--   0 root         (0) root         (0)     4673 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCallBack.cc
--rw-r--r--   0 root         (0) root         (0)     5820 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCallBack.hh
--rw-r--r--   0 root         (0) root         (0)     3807 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucChain.hh
--rw-r--r--   0 root         (0) root         (0)     5655 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucChkPnt.hh
--rw-r--r--   0 root         (0) root         (0)     1514 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucCompiler.hh
--rw-r--r--   0 root         (0) root         (0)     5019 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucDLlist.hh
--rw-r--r--   0 root         (0) root         (0)     4334 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucERoute.cc
--rw-r--r--   0 root         (0) root         (0)     4301 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucERoute.hh
--rw-r--r--   0 root         (0) root         (0)     1693 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucEnum.hh
--rw-r--r--   0 root         (0) root         (0)     9097 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucEnv.cc
--rw-r--r--   0 root         (0) root         (0)     5341 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucEnv.hh
--rw-r--r--   0 root         (0) root         (0)    23619 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucErrInfo.hh
--rw-r--r--   0 root         (0) root         (0)    10829 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucExport.cc
--rw-r--r--   0 root         (0) root         (0)     5760 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucExport.hh
--rw-r--r--   0 root         (0) root         (0)     9215 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucFileInfo.cc
--rw-r--r--   0 root         (0) root         (0)     9566 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucFileInfo.hh
--rw-r--r--   0 root         (0) root         (0)    11294 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucGMap.cc
--rw-r--r--   0 root         (0) root         (0)     8302 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucGMap.hh
--rw-r--r--   0 root         (0) root         (0)     8116 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucGatherConf.cc
--rw-r--r--   0 root         (0) root         (0)     6689 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucGatherConf.hh
--rw-r--r--   0 root         (0) root         (0)     9301 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucHash.hh
--rw-r--r--   0 root         (0) root         (0)    11511 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucHash.icc
--rw-r--r--   0 root         (0) root         (0)     3214 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucHashVal.cc
--rw-r--r--   0 root         (0) root         (0)     3665 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucIOVec.hh
--rw-r--r--   0 root         (0) root         (0)   978532 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucJson.hh
--rw-r--r--   0 root         (0) root         (0)     2676 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucLock.hh
--rw-r--r--   0 root         (0) root         (0)    10867 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucLogging.cc
--rw-r--r--   0 root         (0) root         (0)     3153 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucLogging.hh
--rw-r--r--   0 root         (0) root         (0)     4695 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucMapP2X.hh
--rw-r--r--   0 root         (0) root         (0)    10179 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucMsubs.cc
--rw-r--r--   0 root         (0) root         (0)     5592 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucMsubs.hh
--rw-r--r--   0 root         (0) root         (0)     4780 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucN2NLoader.cc
--rw-r--r--   0 root         (0) root         (0)     3053 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucN2NLoader.hh
--rw-r--r--   0 root         (0) root         (0)    10498 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucN2No2p.cc
--rw-r--r--   0 root         (0) root         (0)     5458 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucNList.cc
--rw-r--r--   0 root         (0) root         (0)     5100 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucNList.hh
--rw-r--r--   0 root         (0) root         (0)    14527 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucNSWalk.cc
--rw-r--r--   0 root         (0) root         (0)     7388 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucNSWalk.hh
--rw-r--r--   0 root         (0) root         (0)     8596 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucName2Name.cc
--rw-r--r--   0 root         (0) root         (0)    12097 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucName2Name.hh
--rw-r--r--   0 root         (0) root         (0)     6417 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPList.hh
--rw-r--r--   0 root         (0) root         (0)    12474 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPgrwUtils.cc
--rw-r--r--   0 root         (0) root         (0)     7990 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPgrwUtils.hh
--rw-r--r--   0 root         (0) root         (0)     6245 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPinKing.hh
--rw-r--r--   0 root         (0) root         (0)    10383 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPinLoader.cc
--rw-r--r--   0 root         (0) root         (0)     9351 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPinLoader.hh
--rw-r--r--   0 root         (0) root         (0)     3859 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPinObject.hh
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPinPath.cc
--rw-r--r--   0 root         (0) root         (0)     3769 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPinPath.hh
--rw-r--r--   0 root         (0) root         (0)     3334 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPreload.cc
--rw-r--r--   0 root         (0) root         (0)     3993 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPreload.hh
--rw-r--r--   0 root         (0) root         (0)    12229 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucProg.cc
--rw-r--r--   0 root         (0) root         (0)     6185 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucProg.hh
--rw-r--r--   0 root         (0) root         (0)    30926 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPsx.cc
--rw-r--r--   0 root         (0) root         (0)     6045 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPsx.hh
--rw-r--r--   0 root         (0) root         (0)    13939 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPup.cc
--rw-r--r--   0 root         (0) root         (0)     8053 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucPup.hh
--rw-r--r--   0 root         (0) root         (0)     7879 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucRash.hh
--rw-r--r--   0 root         (0) root         (0)     9416 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucRash.icc
--rw-r--r--   0 root         (0) root         (0)     6087 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucReqID.cc
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucReqID.hh
--rw-r--r--   0 root         (0) root         (0)     3219 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSFVec.hh
--rw-r--r--   0 root         (0) root         (0)     9442 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSHA3.cc
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSHA3.hh
--rw-r--r--   0 root         (0) root         (0)     6346 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSid.cc
--rw-r--r--   0 root         (0) root         (0)     6332 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSid.hh
--rw-r--r--   0 root         (0) root         (0)     2968 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSiteName.cc
--rw-r--r--   0 root         (0) root         (0)     2588 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSiteName.hh
--rw-r--r--   0 root         (0) root         (0)     3074 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucStats.hh
--rw-r--r--   0 root         (0) root         (0)    47408 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucStream.cc
--rw-r--r--   0 root         (0) root         (0)    11689 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucStream.hh
--rw-r--r--   0 root         (0) root         (0)    35618 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucString.cc
--rw-r--r--   0 root         (0) root         (0)    25276 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucString.hh
--rw-r--r--   0 root         (0) root         (0)     7049 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSxeq.cc
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucSxeq.hh
--rw-r--r--   0 root         (0) root         (0)     5248 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTList.hh
--rw-r--r--   0 root         (0) root         (0)     9887 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTPC.cc
--rw-r--r--   0 root         (0) root         (0)     3801 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTPC.hh
--rw-r--r--   0 root         (0) root         (0)     3390 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTUtils.hh
--rw-r--r--   0 root         (0) root         (0)     7032 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTable.hh
--rw-r--r--   0 root         (0) root         (0)     5093 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTokenizer.cc
--rw-r--r--   0 root         (0) root         (0)     3588 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTokenizer.hh
--rw-r--r--   0 root         (0) root         (0)     3019 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTrace.cc
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucTrace.hh
--rw-r--r--   0 root         (0) root         (0)     8152 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucUri.cc
--rw-r--r--   0 root         (0) root         (0)     4397 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucUri.hh
--rw-r--r--   0 root         (0) root         (0)    44495 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucUtils.cc
--rw-r--r--   0 root         (0) root         (0)     5696 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucUtils.hh
--rw-r--r--   0 root         (0) root         (0)     5319 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucVerName.cc
--rw-r--r--   0 root         (0) root         (0)     4226 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucVerName.hh
--rw-r--r--   0 root         (0) root         (0)     7043 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOucXAttr.hh
--rw-r--r--   0 root         (0) root         (0)    15942 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOuca2x.cc
--rw-r--r--   0 root         (0) root         (0)     4130 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdOuc/XrdOuca2x.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.857900 xrootd-5.6.0/src/XrdPfc/
--rw-r--r--   0 root         (0) root         (0)     7215 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/README
--rw-r--r--   0 root         (0) root         (0)    29394 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfc.cc
--rw-r--r--   0 root         (0) root         (0)    18171 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfc.hh
--rw-r--r--   0 root         (0) root         (0)     1841 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcAllowDecision.cc
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcBlacklistDecision.cc
--rw-r--r--   0 root         (0) root         (0)    12821 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcCommand.cc
--rw-r--r--   0 root         (0) root         (0)    27813 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcConfiguration.cc
--rw-r--r--   0 root         (0) root         (0)     2444 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcDecision.hh
--rw-r--r--   0 root         (0) root         (0)     6260 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcFSctl.cc
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcFSctl.hh
--rw-r--r--   0 root         (0) root         (0)    46143 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcFile.cc
--rw-r--r--   0 root         (0) root         (0)    14635 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcFile.hh
--rw-r--r--   0 root         (0) root         (0)     1933 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcIO.cc
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcIO.hh
--rw-r--r--   0 root         (0) root         (0)    11807 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcIOFile.cc
--rw-r--r--   0 root         (0) root         (0)     3620 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcIOFile.hh
--rw-r--r--   0 root         (0) root         (0)    12359 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcIOFileBlock.cc
--rw-r--r--   0 root         (0) root         (0)     2979 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcIOFileBlock.hh
--rw-r--r--   0 root         (0) root         (0)    19051 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcInfo.cc
--rw-r--r--   0 root         (0) root         (0)    18053 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcInfo.hh
--rw-r--r--   0 root         (0) root         (0)    12636 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcPrint.cc
--rw-r--r--   0 root         (0) root         (0)     2934 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcPrint.hh
--rw-r--r--   0 root         (0) root         (0)    32423 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcPurge.cc
--rw-r--r--   0 root         (0) root         (0)     4738 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcStats.hh
--rw-r--r--   0 root         (0) root         (0)     2079 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcTrace.hh
--rw-r--r--   0 root         (0) root         (0)     1380 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc/XrdPfcTypes.hh
--rw-r--r--   0 root         (0) root         (0)     2940 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPfc.cmake
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPlugins.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.857900 xrootd-5.6.0/src/XrdPosix/
--rw-r--r--   0 root         (0) root         (0)     7201 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/README
--rw-r--r--   0 root         (0) root         (0)    34309 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosix.cc
--rw-r--r--   0 root         (0) root         (0)     4656 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosix.hh
--rw-r--r--   0 root         (0) root         (0)     7780 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixAdmin.cc
--rw-r--r--   0 root         (0) root         (0)     3383 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixAdmin.hh
--rw-r--r--   0 root         (0) root         (0)     5977 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixCache.cc
--rw-r--r--   0 root         (0) root         (0)     6942 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixCache.hh
--rw-r--r--   0 root         (0) root         (0)     2992 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixCallBack.cc
--rw-r--r--   0 root         (0) root         (0)     4732 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixCallBack.hh
--rw-r--r--   0 root         (0) root         (0)    23522 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixConfig.cc
--rw-r--r--   0 root         (0) root         (0)     3483 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixConfig.hh
--rw-r--r--   0 root         (0) root         (0)     5169 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixDir.cc
--rw-r--r--   0 root         (0) root         (0)     4117 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixDir.hh
--rw-r--r--   0 root         (0) root         (0)     8592 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixExtern.hh
--rw-r--r--   0 root         (0) root         (0)     6173 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixExtra.cc
--rw-r--r--   0 root         (0) root         (0)     5480 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixExtra.hh
--rw-r--r--   0 root         (0) root         (0)    26695 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixFile.cc
--rw-r--r--   0 root         (0) root         (0)     8437 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixFile.hh
--rw-r--r--   0 root         (0) root         (0)     7869 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixFileRH.cc
--rw-r--r--   0 root         (0) root         (0)     4377 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixFileRH.hh
--rw-r--r--   0 root         (0) root         (0)     2994 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixInfo.hh
--rw-r--r--   0 root         (0) root         (0)    14943 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixLinkage.cc
--rw-r--r--   0 root         (0) root         (0)    14590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixLinkage.hh
--rw-r--r--   0 root         (0) root         (0)     8526 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixMap.cc
--rw-r--r--   0 root         (0) root         (0)     3065 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixMap.hh
--rw-r--r--   0 root         (0) root         (0)     3041 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixObjGuard.hh
--rw-r--r--   0 root         (0) root         (0)    11702 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixObject.cc
--rw-r--r--   0 root         (0) root         (0)     4655 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixObject.hh
--rw-r--r--   0 root         (0) root         (0)     3600 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixOsDep.hh
--rw-r--r--   0 root         (0) root         (0)    24535 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixPreload.cc
--rw-r--r--   0 root         (0) root         (0)    19284 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixPreload32.cc
--rw-r--r--   0 root         (0) root         (0)     5301 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixPrepIO.cc
--rw-r--r--   0 root         (0) root         (0)     4774 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixPrepIO.hh
--rw-r--r--   0 root         (0) root         (0)     3366 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixStats.hh
--rw-r--r--   0 root         (0) root         (0)     2880 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixTrace.hh
--rw-r--r--   0 root         (0) root         (0)    53317 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixXrootd.cc
--rw-r--r--   0 root         (0) root         (0)    18316 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixXrootd.hh
--rw-r--r--   0 root         (0) root         (0)    11698 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixXrootdPath.cc
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix/XrdPosixXrootdPath.hh
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPosix.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdPss/
--rw-r--r--   0 root         (0) root         (0)    46084 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPss.cc
--rw-r--r--   0 root         (0) root         (0)     9367 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPss.hh
--rw-r--r--   0 root         (0) root         (0)     8543 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssAio.cc
--rw-r--r--   0 root         (0) root         (0)     5049 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssAioCB.cc
--rw-r--r--   0 root         (0) root         (0)     3188 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssAioCB.hh
--rw-r--r--   0 root         (0) root         (0)     8402 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssCks.cc
--rw-r--r--   0 root         (0) root         (0)     3733 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssCks.hh
--rw-r--r--   0 root         (0) root         (0)    31246 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssConfig.cc
--rw-r--r--   0 root         (0) root         (0)     2807 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssTrace.hh
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssUrlInfo.cc
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssUrlInfo.hh
--rw-r--r--   0 root         (0) root         (0)     5115 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssUtils.cc
--rw-r--r--   0 root         (0) root         (0)     3367 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdPss/XrdPssUtils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdRmc/
--rw-r--r--   0 root         (0) root         (0)     3076 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmc.cc
--rw-r--r--   0 root         (0) root         (0)     8248 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmc.hh
--rw-r--r--   0 root         (0) root         (0)    20610 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmcData.cc
--rw-r--r--   0 root         (0) root         (0)     5754 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmcData.hh
--rw-r--r--   0 root         (0) root         (0)    20813 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmcReal.cc
--rw-r--r--   0 root         (0) root         (0)     5594 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmcReal.hh
--rw-r--r--   0 root         (0) root         (0)     7041 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdRmc/XrdRmcSlot.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8455 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/README.md
--rw-r--r--   0 root         (0) root         (0)    50104 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensAccess.cc
--rw-r--r--   0 root         (0) root         (0)     2985 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1378 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensMon.cc
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensMon.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/configs/
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/configs/export-lib-symbols
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/configs/export-module-symbols
--rw-r--r--   0 root         (0) root         (0)      945 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/configs/scitokens.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/test/config/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/config/override.conf
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/config/scitokens-aud.cfg
--rw-r--r--   0 root         (0) root         (0)      115 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/config/scitokens-multi-aud.cfg
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/config/scitokens-no-aud.cfg
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/config/xrootd-http.cfg
--rw-r--r--   0 root         (0) root         (0)     1598 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/create-pubkey.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/openssl-selfsigned.conf
--rwxr-xr-x   0 root         (0) root         (0)      803 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/setup_tests.sh
--rwxr-xr-x   0 root         (0) root         (0)     5083 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/test/test_inside_docker.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/vendor/
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/README.vendor
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/.gitignore
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/.travis.yml
--rw-r--r--   0 root         (0) root         (0)    13507 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/INIReader.h
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp
--rw-r--r--   0 root         (0) root         (0)     1510 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1574 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/README.md
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/inih/test.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/.clang-format
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/.gitignore
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/.gitmodules
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/.travis.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/Changes
--rw-r--r--   0 root         (0) root         (0)     1336 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7016 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/README.mkdn
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/
--rw-r--r--   0 root         (0) root         (0)     3475 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc
--rw-r--r--   0 root         (0) root         (0)     2787 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/iostream.cc
--rw-r--r--   0 root         (0) root         (0)     2496 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/streaming.cc
--rw-r--r--   0 root         (0) root         (0)    33256 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picojson.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.867901 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picotest/
--rw-r--r--   0 root         (0) root         (0)     2452 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picotest/picotest.c
--rw-r--r--   0 root         (0) root         (0)     1519 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picotest/picotest.h
--rw-r--r--   0 root         (0) root         (0)    12611 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/test.cc
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSciTokens.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSec/
--rw-r--r--   0 root         (0) root         (0)     4540 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecAttr.hh
--rw-r--r--   0 root         (0) root         (0)     5662 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecClient.cc
--rw-r--r--   0 root         (0) root         (0)     6062 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntity.cc
--rw-r--r--   0 root         (0) root         (0)     6849 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntity.hh
--rw-r--r--   0 root         (0) root         (0)     6459 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntityAttr.cc
--rw-r--r--   0 root         (0) root         (0)     8424 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntityAttr.hh
--rw-r--r--   0 root         (0) root         (0)     4638 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntityPin.hh
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntityXtra.cc
--rw-r--r--   0 root         (0) root         (0)     2772 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecEntityXtra.hh
--rw-r--r--   0 root         (0) root         (0)    34779 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecInterface.hh
--rw-r--r--   0 root         (0) root         (0)    10669 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecLoadSecurity.cc
--rw-r--r--   0 root         (0) root         (0)     7822 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecLoadSecurity.hh
--rw-r--r--   0 root         (0) root         (0)     3233 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecMonitor.hh
--rw-r--r--   0 root         (0) root         (0)    15686 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecPManager.cc
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecPManager.hh
--rw-r--r--   0 root         (0) root         (0)    18129 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecProtect.cc
--rw-r--r--   0 root         (0) root         (0)     8540 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecProtect.hh
--rw-r--r--   0 root         (0) root         (0)    11790 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecProtector.cc
--rw-r--r--   0 root         (0) root         (0)     7608 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecProtector.hh
--rw-r--r--   0 root         (0) root         (0)     4849 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecProtocolhost.cc
--rw-r--r--   0 root         (0) root         (0)     3535 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecProtocolhost.hh
--rw-r--r--   0 root         (0) root         (0)    40467 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecServer.cc
--rw-r--r--   0 root         (0) root         (0)     5105 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecServer.hh
--rw-r--r--   0 root         (0) root         (0)    14327 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecTLayer.cc
--rw-r--r--   0 root         (0) root         (0)     7692 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecTLayer.hh
--rw-r--r--   0 root         (0) root         (0)     3076 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSecTrace.hh
--rw-r--r--   0 root         (0) root         (0)     7714 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSectestClient.cc
--rw-r--r--   0 root         (0) root         (0)    12099 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec/XrdSectestServer.cc
--rw-r--r--   0 root         (0) root         (0)     4574 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSec.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSecgsi/
--rw-r--r--   0 root         (0) root         (0)   199012 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecProtocolgsi.cc
--rw-r--r--   0 root         (0) root         (0)    25176 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecProtocolgsi.hh
--rw-r--r--   0 root         (0) root         (0)     6777 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc
--rw-r--r--   0 root         (0) root         (0)    11227 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc
--rw-r--r--   0 root         (0) root         (0)     8786 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf
--rw-r--r--   0 root         (0) root         (0)     9513 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiOpts.hh
--rw-r--r--   0 root         (0) root         (0)    26709 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiProxy.cc
--rw-r--r--   0 root         (0) root         (0)     3028 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiTrace.hh
--rw-r--r--   0 root         (0) root         (0)    17329 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi/XrdSecgsitest.cc
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecgsi.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSeckrb5/
--rw-r--r--   0 root         (0) root         (0)    38645 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSeckrb5/XrdSecProtocolkrb5.cc
--rw-r--r--   0 root         (0) root         (0)      759 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSeckrb5.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSecpwd/
--rw-r--r--   0 root         (0) root         (0)   129074 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecpwd/XrdSecProtocolpwd.cc
--rw-r--r--   0 root         (0) root         (0)    19042 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecpwd/XrdSecProtocolpwd.hh
--rw-r--r--   0 root         (0) root         (0)     2626 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecpwd/XrdSecpwdPlatform.hh
--rw-r--r--   0 root         (0) root         (0)    84590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc
--rw-r--r--   0 root         (0) root         (0)     3028 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecpwd/XrdSecpwdTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSecsss/
--rw-r--r--   0 root         (0) root         (0)    41443 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecProtocolsss.cc
--rw-r--r--   0 root         (0) root         (0)     6297 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecProtocolsss.hh
--rw-r--r--   0 root         (0) root         (0)    19394 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssAdmin.cc
--rw-r--r--   0 root         (0) root         (0)     3559 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssCon.cc
--rw-r--r--   0 root         (0) root         (0)     4329 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssCon.hh
--rw-r--r--   0 root         (0) root         (0)    11806 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssEnt.cc
--rw-r--r--   0 root         (0) root         (0)     5290 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssEnt.hh
--rw-r--r--   0 root         (0) root         (0)     9560 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssID.cc
--rw-r--r--   0 root         (0) root         (0)     8505 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssID.hh
--rw-r--r--   0 root         (0) root         (0)    25232 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssKT.cc
--rw-r--r--   0 root         (0) root         (0)     5358 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssKT.hh
--rw-r--r--   0 root         (0) root         (0)     2704 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssMap.hh
--rw-r--r--   0 root         (0) root         (0)     5765 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecsss/XrdSecsssRR.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSecunix/
--rw-r--r--   0 root         (0) root         (0)     8595 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecunix/XrdSecProtocolunix.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSecztn/
--rw-r--r--   0 root         (0) root         (0)    29163 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecztn/XrdSecProtocolztn.cc
--rw-r--r--   0 root         (0) root         (0)     6814 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecztn/XrdSecztn.cc
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSecztn.cmake
--rw-r--r--   0 root         (0) root         (0)    10685 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdServer.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.877901 xrootd-5.6.0/src/XrdSfs/
--rw-r--r--   0 root         (0) root         (0)     3999 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsAio.hh
--rw-r--r--   0 root         (0) root         (0)     5824 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsDio.hh
--rw-r--r--   0 root         (0) root         (0)     5455 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsFAttr.hh
--rw-r--r--   0 root         (0) root         (0)     5100 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsFlags.hh
--rw-r--r--   0 root         (0) root         (0)     5619 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsGPFile.hh
--rw-r--r--   0 root         (0) root         (0)    12634 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsInterface.cc
--rw-r--r--   0 root         (0) root         (0)    67321 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsInterface.hh
--rw-r--r--   0 root         (0) root         (0)    38665 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsNative.cc
--rw-r--r--   0 root         (0) root         (0)    10785 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsNative.hh
--rw-r--r--   0 root         (0) root         (0)     3537 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsXio.cc
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsXio.hh
--rw-r--r--   0 root         (0) root         (0)     4432 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSfs/XrdSfsXioImpl.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.887901 xrootd-5.6.0/src/XrdSsi/
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiAlert.cc
--rw-r--r--   0 root         (0) root         (0)     3366 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiAlert.hh
--rw-r--r--   0 root         (0) root         (0)     2661 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiAtomics.cc
--rw-r--r--   0 root         (0) root         (0)     7958 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiAtomics.hh
--rw-r--r--   0 root         (0) root         (0)     3132 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiBVec.hh
--rw-r--r--   0 root         (0) root         (0)    14419 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiClient.cc
--rw-r--r--   0 root         (0) root         (0)     7934 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiCluster.hh
--rw-r--r--   0 root         (0) root         (0)     4735 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiCms.cc
--rw-r--r--   0 root         (0) root         (0)     3752 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiCms.hh
--rw-r--r--   0 root         (0) root         (0)     7049 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiDir.cc
--rw-r--r--   0 root         (0) root         (0)     3177 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiDir.hh
--rw-r--r--   0 root         (0) root         (0)     4087 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiEntity.hh
--rw-r--r--   0 root         (0) root         (0)     2663 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiErrInfo.cc
--rw-r--r--   0 root         (0) root         (0)     6519 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiErrInfo.hh
--rw-r--r--   0 root         (0) root         (0)     7117 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiEvent.cc
--rw-r--r--   0 root         (0) root         (0)     4015 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiEvent.hh
--rw-r--r--   0 root         (0) root         (0)    18166 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFile.cc
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFile.hh
--rw-r--r--   0 root         (0) root         (0)    35655 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFileReq.cc
--rw-r--r--   0 root         (0) root         (0)     6776 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFileReq.hh
--rw-r--r--   0 root         (0) root         (0)     3711 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFileResource.cc
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFileResource.hh
--rw-r--r--   0 root         (0) root         (0)    26232 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFileSess.cc
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiFileSess.hh
--rw-r--r--   0 root         (0) root         (0)     7891 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiLogger.cc
--rw-r--r--   0 root         (0) root         (0)     8754 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiLogger.hh
--rw-r--r--   0 root         (0) root         (0)     6565 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiLogging.cc
--rw-r--r--   0 root         (0) root         (0)    17533 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiProvider.hh
--rw-r--r--   0 root         (0) root         (0)     3962 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiRRAgent.hh
--rw-r--r--   0 root         (0) root         (0)     4545 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiRRInfo.hh
--rw-r--r--   0 root         (0) root         (0)     4295 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiRRTable.hh
--rw-r--r--   0 root         (0) root         (0)     8144 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiRequest.cc
--rw-r--r--   0 root         (0) root         (0)    15740 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiRequest.hh
--rw-r--r--   0 root         (0) root         (0)     5790 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiResource.hh
--rw-r--r--   0 root         (0) root         (0)     7000 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiRespInfo.hh
--rw-r--r--   0 root         (0) root         (0)    12144 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiResponder.cc
--rw-r--r--   0 root         (0) root         (0)    13431 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiResponder.hh
--rw-r--r--   0 root         (0) root         (0)     8986 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiScale.cc
--rw-r--r--   0 root         (0) root         (0)     3515 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiScale.hh
--rw-r--r--   0 root         (0) root         (0)    12168 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiServReal.cc
--rw-r--r--   0 root         (0) root         (0)     3574 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiServReal.hh
--rw-r--r--   0 root         (0) root         (0)     3281 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiService.cc
--rw-r--r--   0 root         (0) root         (0)     9866 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiService.hh
--rw-r--r--   0 root         (0) root         (0)    17845 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiSessReal.cc
--rw-r--r--   0 root         (0) root         (0)     4784 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiSessReal.hh
--rw-r--r--   0 root         (0) root         (0)    20137 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiSfs.cc
--rw-r--r--   0 root         (0) root         (0)     7069 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiSfs.hh
--rw-r--r--   0 root         (0) root         (0)    25133 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiSfsConfig.cc
--rw-r--r--   0 root         (0) root         (0)     3556 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiSfsConfig.hh
--rw-r--r--   0 root         (0) root         (0)    45566 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiShMam.cc
--rw-r--r--   0 root         (0) root         (0)     5508 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiShMam.hh
--rw-r--r--   0 root         (0) root         (0)    22363 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiShMap.hh
--rw-r--r--   0 root         (0) root         (0)    12380 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiShMap.icc
--rw-r--r--   0 root         (0) root         (0)     3048 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiShMat.cc
--rw-r--r--   0 root         (0) root         (0)    19625 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiShMat.hh
--rw-r--r--   0 root         (0) root         (0)     6168 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiStat.cc
--rw-r--r--   0 root         (0) root         (0)     6883 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiStats.cc
--rw-r--r--   0 root         (0) root         (0)     4527 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiStats.hh
--rw-r--r--   0 root         (0) root         (0)     8580 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiStream.hh
--rw-r--r--   0 root         (0) root         (0)    24852 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiTaskReal.cc
--rw-r--r--   0 root         (0) root         (0)     4845 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiTaskReal.hh
--rw-r--r--   0 root         (0) root         (0)     2865 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiTrace.hh
--rw-r--r--   0 root         (0) root         (0)     9000 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiUtils.cc
--rw-r--r--   0 root         (0) root         (0)     3203 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi/XrdSsiUtils.hh
--rw-r--r--   0 root         (0) root         (0)     4630 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSsi.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.887901 xrootd-5.6.0/src/XrdSut/
--rw-r--r--   0 root         (0) root         (0)    22228 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutAux.cc
--rw-r--r--   0 root         (0) root         (0)    15145 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutAux.hh
--rw-r--r--   0 root         (0) root         (0)     5926 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutBuckList.cc
--rw-r--r--   0 root         (0) root         (0)     3963 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutBuckList.hh
--rw-r--r--   0 root         (0) root         (0)     8236 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutBucket.cc
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutBucket.hh
--rw-r--r--   0 root         (0) root         (0)    16296 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutBuffer.cc
--rw-r--r--   0 root         (0) root         (0)     4872 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutBuffer.hh
--rw-r--r--   0 root         (0) root         (0)     6430 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutCache.hh
--rw-r--r--   0 root         (0) root         (0)     5618 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutCacheEntry.cc
--rw-r--r--   0 root         (0) root         (0)     5456 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutCacheEntry.hh
--rw-r--r--   0 root         (0) root         (0)    21841 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutPFCache.cc
--rw-r--r--   0 root         (0) root         (0)     5757 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutPFCache.hh
--rw-r--r--   0 root         (0) root         (0)     5549 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutPFEntry.cc
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutPFEntry.hh
--rw-r--r--   0 root         (0) root         (0)    64583 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutPFile.cc
--rw-r--r--   0 root         (0) root         (0)     7738 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutPFile.hh
--rw-r--r--   0 root         (0) root         (0)     8759 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutRndm.cc
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutRndm.hh
--rw-r--r--   0 root         (0) root         (0)     2941 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSut/XrdSutTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.897901 xrootd-5.6.0/src/XrdSys/
--rw-r--r--   0 root         (0) root         (0)     5249 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysAtomics.hh
--rw-r--r--   0 root         (0) root         (0)     4979 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysDir.cc
--rw-r--r--   0 root         (0) root         (0)     3341 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysDir.hh
--rw-r--r--   0 root         (0) root         (0)     4872 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysE2T.cc
--rw-r--r--   0 root         (0) root         (0)     2750 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysE2T.hh
--rw-r--r--   0 root         (0) root         (0)     8484 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysError.cc
--rw-r--r--   0 root         (0) root         (0)     7359 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysError.hh
--rw-r--r--   0 root         (0) root         (0)     6923 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFAttr.cc
--rw-r--r--   0 root         (0) root         (0)     4996 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFAttr.hh
--rw-r--r--   0 root         (0) root         (0)     7106 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFAttrBsd.icc
--rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFAttrLnx.icc
--rw-r--r--   0 root         (0) root         (0)     6063 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFAttrMac.icc
--rw-r--r--   0 root         (0) root         (0)     7705 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFAttrSun.icc
--rw-r--r--   0 root         (0) root         (0)     7575 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFD.hh
--rw-r--r--   0 root         (0) root         (0)     4783 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFallocate.cc
--rw-r--r--   0 root         (0) root         (0)     1578 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysFallocate.hh
--rw-r--r--   0 root         (0) root         (0)     2714 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysHeaders.hh
--rw-r--r--   0 root         (0) root         (0)    43303 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysIOEvents.cc
--rw-r--r--   0 root         (0) root         (0)    26713 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysIOEvents.hh
--rw-r--r--   0 root         (0) root         (0)    16052 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollE.icc
--rw-r--r--   0 root         (0) root         (0)    17045 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollKQ.icc
--rw-r--r--   0 root         (0) root         (0)    18706 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollPoll.icc
--rw-r--r--   0 root         (0) root         (0)    14975 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollPort.icc
--rw-r--r--   0 root         (0) root         (0)    16419 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysKernelBuffer.hh
--rw-r--r--   0 root         (0) root         (0)     5437 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysLogPI.hh
--rw-r--r--   0 root         (0) root         (0)    26559 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysLogger.cc
--rw-r--r--   0 root         (0) root         (0)    11736 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysLogger.hh
--rw-r--r--   0 root         (0) root         (0)    12120 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysLogging.cc
--rw-r--r--   0 root         (0) root         (0)     5811 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysLogging.hh
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPageSize.hh
--rw-r--r--   0 root         (0) root         (0)     3233 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPlatform.cc
--rw-r--r--   0 root         (0) root         (0)     7952 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPlatform.hh
--rw-r--r--   0 root         (0) root         (0)    17849 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPlugin.cc
--rw-r--r--   0 root         (0) root         (0)    13621 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPlugin.hh
--rw-r--r--   0 root         (0) root         (0)    13000 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPriv.cc
--rw-r--r--   0 root         (0) root         (0)     4228 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPriv.hh
--rw-r--r--   0 root         (0) root         (0)    13657 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPthread.cc
--rw-r--r--   0 root         (0) root         (0)    19521 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPthread.hh
--rw-r--r--   0 root         (0) root         (0)     3245 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysPwd.hh
--rw-r--r--   0 root         (0) root         (0)    11994 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysRAtomic.hh
--rw-r--r--   0 root         (0) root         (0)     3952 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysSemWait.hh
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysShmem.hh
--rw-r--r--   0 root         (0) root         (0)     9460 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysTimer.cc
--rw-r--r--   0 root         (0) root         (0)     3814 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysTimer.hh
--rw-r--r--   0 root         (0) root         (0)    15639 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysTrace.cc
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysTrace.hh
--rw-r--r--   0 root         (0) root         (0)     8298 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysUtils.cc
--rw-r--r--   0 root         (0) root         (0)     4798 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysUtils.hh
--rw-r--r--   0 root         (0) root         (0)     4735 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysXAttr.cc
--rw-r--r--   0 root         (0) root         (0)    15063 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysXAttr.hh
--rw-r--r--   0 root         (0) root         (0)     5708 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysXSLock.cc
--rw-r--r--   0 root         (0) root         (0)     3311 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdSys/XrdSysXSLock.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.897901 xrootd-5.6.0/src/XrdThrottle/
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/README
--rw-r--r--   0 root         (0) root         (0)     7487 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottle.hh
--rw-r--r--   0 root         (0) root         (0)     6658 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottleFile.cc
--rw-r--r--   0 root         (0) root         (0)     5731 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottleFileSystem.cc
--rw-r--r--   0 root         (0) root         (0)    12897 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottleFileSystemConfig.cc
--rw-r--r--   0 root         (0) root         (0)    18594 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottleManager.cc
--rw-r--r--   0 root         (0) root         (0)     5403 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottleManager.hh
--rw-r--r--   0 root         (0) root         (0)      879 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdThrottle/XrdThrottleTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.897901 xrootd-5.6.0/src/XrdTls/
--rw-r--r--   0 root         (0) root         (0)    10417 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTls.cc
--rw-r--r--   0 root         (0) root         (0)     6921 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTls.hh
--rw-r--r--   0 root         (0) root         (0)    37752 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsContext.cc
--rw-r--r--   0 root         (0) root         (0)    14507 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsContext.hh
--rw-r--r--   0 root         (0) root         (0)     1259 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsHostcheck.hh
--rw-r--r--   0 root         (0) root         (0)     6628 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsHostcheck.icc
--rw-r--r--   0 root         (0) root         (0)     5275 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsNotary.cc
--rw-r--r--   0 root         (0) root         (0)     5222 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsNotary.hh
--rw-r--r--   0 root         (0) root         (0)     2251 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsNotaryUtils.hh
--rw-r--r--   0 root         (0) root         (0)     7142 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsNotaryUtils.icc
--rw-r--r--   0 root         (0) root         (0)     3969 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsPeerCerts.cc
--rw-r--r--   0 root         (0) root         (0)     4951 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsPeerCerts.hh
--rw-r--r--   0 root         (0) root         (0)    33590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsSocket.cc
--rw-r--r--   0 root         (0) root         (0)    11845 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsSocket.hh
--rw-r--r--   0 root         (0) root         (0)    16122 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsTempCA.cc
--rw-r--r--   0 root         (0) root         (0)     5462 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsTempCA.hh
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTls/XrdTlsTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.897901 xrootd-5.6.0/src/XrdTpc/
--rw-r--r--   0 root         (0) root         (0)     4032 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/README.md
--rw-r--r--   0 root         (0) root         (0)     5387 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcConfigure.cc
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcCurlMulti.cc
--rw-r--r--   0 root         (0) root         (0)      144 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcCurlMulti.hh
--rw-r--r--   0 root         (0) root         (0)    19456 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcMultistream.cc
--rw-r--r--   0 root         (0) root         (0)    10532 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcState.cc
--rw-r--r--   0 root         (0) root         (0)     5794 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcState.hh
--rw-r--r--   0 root         (0) root         (0)     7210 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcStream.cc
--rw-r--r--   0 root         (0) root         (0)     5499 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcStream.hh
--rw-r--r--   0 root         (0) root         (0)    44035 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcTPC.cc
--rw-r--r--   0 root         (0) root         (0)     5994 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/XrdTpcTPC.hh
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/export-lib-symbols
--rwxr-xr-x   0 root         (0) root         (0)     3709 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc/xrootd-test-tpc
--rw-r--r--   0 root         (0) root         (0)     2282 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdTpc.cmake
--rw-r--r--   0 root         (0) root         (0)    14578 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdUtils.cmake
--rw-r--r--   0 root         (0) root         (0)     5084 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVersion.hh.in
--rw-r--r--   0 root         (0) root         (0)    15666 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVersionPlugin.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.897901 xrootd-5.6.0/src/XrdVoms/
--rw-r--r--   0 root         (0) root         (0)     2917 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/README.md
--rw-r--r--   0 root         (0) root         (0)     2590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVoms.hh
--rw-r--r--   0 root         (0) root         (0)    22190 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsFun.cc
--rw-r--r--   0 root         (0) root         (0)     3835 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsFun.hh
--rw-r--r--   0 root         (0) root         (0)     6174 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsHttp.cc
--rw-r--r--   0 root         (0) root         (0)    15233 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsMapfile.cc
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsMapfile.hh
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsTrace.hh
--rw-r--r--   0 root         (0) root         (0)     4105 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms/XrdVomsgsi.cc
--rw-r--r--   0 root         (0) root         (0)     1798 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdVoms.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.907901 xrootd-5.6.0/src/XrdXml/
--rw-r--r--   0 root         (0) root         (0)    18501 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlMetaLink.cc
--rw-r--r--   0 root         (0) root         (0)     9497 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlMetaLink.hh
--rw-r--r--   0 root         (0) root         (0)    10670 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlRdrTiny.cc
--rw-r--r--   0 root         (0) root         (0)     3590 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlRdrTiny.hh
--rw-r--r--   0 root         (0) root         (0)    11751 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlRdrXml2.cc
--rw-r--r--   0 root         (0) root         (0)     3585 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlRdrXml2.hh
--rw-r--r--   0 root         (0) root         (0)     4195 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlReader.cc
--rw-r--r--   0 root         (0) root         (0)     9010 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/XrdXmlReader.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.907901 xrootd-5.6.0/src/XrdXml/tinyxml/
--rw-r--r--   0 root         (0) root         (0)     2507 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/tinyxml/tinystr.cpp
--rw-r--r--   0 root         (0) root         (0)     8197 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/tinyxml/tinystr.h
--rw-r--r--   0 root         (0) root         (0)    37588 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/tinyxml/tinyxml.cpp
--rw-r--r--   0 root         (0) root         (0)    64835 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/tinyxml/tinyxml.h
--rw-r--r--   0 root         (0) root         (0)     1791 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/tinyxml/tinyxmlerror.cpp
--rw-r--r--   0 root         (0) root         (0)    37439 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml/tinyxml/tinyxmlparser.cpp
--rw-r--r--   0 root         (0) root         (0)     2148 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXml.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/src/XrdXrootd/
--rw-r--r--   0 root         (0) root         (0)    21688 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAdmin.cc
--rw-r--r--   0 root         (0) root         (0)     3927 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAdmin.hh
--rw-r--r--   0 root         (0) root         (0)     6106 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioBuff.cc
--rw-r--r--   0 root         (0) root         (0)     3396 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioBuff.hh
--rw-r--r--   0 root         (0) root         (0)     6164 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioFob.cc
--rw-r--r--   0 root         (0) root         (0)     3140 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioFob.hh
--rw-r--r--   0 root         (0) root         (0)    10852 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioPgrw.cc
--rw-r--r--   0 root         (0) root         (0)     4017 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioPgrw.hh
--rw-r--r--   0 root         (0) root         (0)    16842 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioTask.cc
--rw-r--r--   0 root         (0) root         (0)     5932 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioTask.hh
--rw-r--r--   0 root         (0) root         (0)     3257 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdBridge.cc
--rw-r--r--   0 root         (0) root         (0)    25502 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdBridge.hh
--rw-r--r--   0 root         (0) root         (0)    17339 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdCallBack.cc
--rw-r--r--   0 root         (0) root         (0)     3955 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdCallBack.hh
--rw-r--r--   0 root         (0) root         (0)    71797 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdConfig.cc
--rw-r--r--   0 root         (0) root         (0)    25761 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdConfigMon.cc
--rw-r--r--   0 root         (0) root         (0)    14829 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdFile.cc
--rw-r--r--   0 root         (0) root         (0)     8211 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdFile.hh
--rw-r--r--   0 root         (0) root         (0)     2629 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileLock.hh
--rw-r--r--   0 root         (0) root         (0)     6072 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileLock1.cc
--rw-r--r--   0 root         (0) root         (0)     2959 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileLock1.hh
--rw-r--r--   0 root         (0) root         (0)     7522 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileStats.hh
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdGPFile.hh
--rw-r--r--   0 root         (0) root         (0)    19666 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdGSReal.cc
--rw-r--r--   0 root         (0) root         (0)     6593 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdGSReal.hh
--rw-r--r--   0 root         (0) root         (0)     5076 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdGStream.cc
--rw-r--r--   0 root         (0) root         (0)     8514 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdGStream.hh
--rw-r--r--   0 root         (0) root         (0)    26130 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdJob.cc
--rw-r--r--   0 root         (0) root         (0)     4224 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdJob.hh
--rw-r--r--   0 root         (0) root         (0)     3858 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdLoadLib.cc
--rw-r--r--   0 root         (0) root         (0)    14128 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonData.hh
--rw-r--r--   0 root         (0) root         (0)     5374 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFMap.cc
--rw-r--r--   0 root         (0) root         (0)     3118 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFMap.hh
--rw-r--r--   0 root         (0) root         (0)    18282 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFile.cc
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFile.hh
--rw-r--r--   0 root         (0) root         (0)    43427 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonitor.cc
--rw-r--r--   0 root         (0) root         (0)    12226 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonitor.hh
--rw-r--r--   0 root         (0) root         (0)    17436 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdNormAio.cc
--rw-r--r--   0 root         (0) root         (0)     3758 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdNormAio.hh
--rw-r--r--   0 root         (0) root         (0)    19524 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgrwAio.cc
--rw-r--r--   0 root         (0) root         (0)     3708 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgrwAio.hh
--rw-r--r--   0 root         (0) root         (0)     4934 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwBadCS.cc
--rw-r--r--   0 root         (0) root         (0)     2979 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwBadCS.hh
--rw-r--r--   0 root         (0) root         (0)     7262 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwCtl.cc
--rw-r--r--   0 root         (0) root         (0)     4842 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwCtl.hh
--rw-r--r--   0 root         (0) root         (0)     4520 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwFob.cc
--rw-r--r--   0 root         (0) root         (0)     4321 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwFob.hh
--rw-r--r--   0 root         (0) root         (0)     3973 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPio.cc
--rw-r--r--   0 root         (0) root         (0)     3751 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPio.hh
--rw-r--r--   0 root         (0) root         (0)     4685 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPlugin.cc
--rw-r--r--   0 root         (0) root         (0)    12615 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPrepare.cc
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdPrepare.hh
--rw-r--r--   0 root         (0) root         (0)    53955 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdProtocol.cc
--rw-r--r--   0 root         (0) root         (0)    24030 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdProtocol.hh
--rw-r--r--   0 root         (0) root         (0)     3955 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdReqID.hh
--rw-r--r--   0 root         (0) root         (0)    17733 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdResponse.cc
--rw-r--r--   0 root         (0) root         (0)     5450 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdResponse.hh
--rw-r--r--   0 root         (0) root         (0)     7898 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdStats.cc
--rw-r--r--   0 root         (0) root         (0)     4653 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdStats.hh
--rw-r--r--   0 root         (0) root         (0)     6457 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTpcMon.cc
--rw-r--r--   0 root         (0) root         (0)     4899 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTpcMon.hh
--rw-r--r--   0 root         (0) root         (0)     3605 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTrace.hh
--rw-r--r--   0 root         (0) root         (0)     4806 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransPend.cc
--rw-r--r--   0 root         (0) root         (0)     3394 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransPend.hh
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransSend.cc
--rw-r--r--   0 root         (0) root         (0)     3662 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransSend.hh
--rw-r--r--   0 root         (0) root         (0)    27246 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransit.cc
--rw-r--r--   0 root         (0) root         (0)     9705 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransit.hh
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdWVInfo.hh
--rw-r--r--   0 root         (0) root         (0)     5092 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdXPath.hh
--rw-r--r--   0 root         (0) root         (0)   148794 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeq.cc
--rw-r--r--   0 root         (0) root         (0)     3317 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeq.hh
--rw-r--r--   0 root         (0) root         (0)    12437 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeqChkPnt.cc
--rw-r--r--   0 root         (0) root         (0)    20041 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeqFAttr.cc
--rw-r--r--   0 root         (0) root         (0)    22344 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeqPgrw.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/src/XrdZip/
--rw-r--r--   0 root         (0) root         (0)    14675 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipCDFH.hh
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipDataDescriptor.hh
--rw-r--r--   0 root         (0) root         (0)     6301 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipEOCD.hh
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipExtra.hh
--rw-r--r--   0 root         (0) root         (0)     7291 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipLFH.hh
--rw-r--r--   0 root         (0) root         (0)     6734 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipUtils.hh
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipZIP64EOCD.hh
--rw-r--r--   0 root         (0) root         (0)     3227 2023-06-30 14:28:10.000000 xrootd-5.6.0/src/XrdZip/XrdZipZIP64EOCDL.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)      315 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XRootD/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XRootD/CMakeLists.txt
--rwxr-xr-x   0 root         (0) root         (0)     3065 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XRootD/smoke.sh
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XRootD/xrootd.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdCephTests/
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdCephTests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6661 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdCephTests/CephParsingTest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdCl/
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdCl/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5351 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdCl/XrdClURL.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.717900 xrootd-5.6.0/tests/XrdClHttp/cases/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/cases/000-simple-download/
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/cases/000-simple-download/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/cases/001-deep-path-download/
--rw-r--r--   0 root         (0) root         (0)     1044 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/cases/001-deep-path-download/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/cases/002-simple-upload/
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/cases/002-simple-upload/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/cases/003-deep-path-upload/
--rw-r--r--   0 root         (0) root         (0)     1157 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/cases/003-deep-path-upload/main.sh
--rw-r--r--   0 root         (0) root         (0)     1919 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/common.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/config/
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/config/caddyfile
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/config/caddyfile-webdav
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClHttp/config/client/
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/config/client/http.conf
--rwxr-xr-x   0 root         (0) root         (0)     1571 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClHttp/run_test.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClTests/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    27183 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/FileCopyTest.cc
--rw-r--r--   0 root         (0) root         (0)    22807 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/FileSystemTest.cc
--rw-r--r--   0 root         (0) root         (0)    30512 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/FileTest.cc
--rw-r--r--   0 root         (0) root         (0)    21399 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/IdentityPlugIn.cc
--rw-r--r--   0 root         (0) root         (0)     2516 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/IdentityPlugIn.hh
--rw-r--r--   0 root         (0) root         (0)    22565 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/LocalFileHandlerTest.cc
--rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/MonitorTestLib.cc
--rw-r--r--   0 root         (0) root         (0)    36161 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/OperationsWorkflowTest.cc
--rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/PollerTest.cc
--rw-r--r--   0 root         (0) root         (0)    20068 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/PostMasterTest.cc
--rw-r--r--   0 root         (0) root         (0)    11141 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/SocketTest.cc
--rw-r--r--   0 root         (0) root         (0)    12152 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/ThreadingTest.cc
--rw-r--r--   0 root         (0) root         (0)     7930 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/UtilsTest.cc
--rw-r--r--   0 root         (0) root         (0)     4848 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/XRootDProtocolHelper.cc
--rw-r--r--   0 root         (0) root         (0)     1982 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/XRootDProtocolHelper.hh
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/cppunit.supp
--rwxr-xr-x   0 root         (0) root         (0)      430 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/printenv.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClTests/tls/
--rw-r--r--   0 root         (0) root         (0)      529 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/tls/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/tls/README.md
--rw-r--r--   0 root         (0) root         (0)     1861 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/tls/xrdcl-tls.cc
--rw-r--r--   0 root         (0) root         (0)    16273 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/tls/xrdsrv-tls.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdClTests/wrt/
--rw-r--r--   0 root         (0) root         (0)    14962 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/wrt/xrdsrv-dio.cc
--rw-r--r--   0 root         (0) root         (0)    14168 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdClTests/wrt/xrdsrv-wrt.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdEcTests/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdEcTests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    19308 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdEcTests/MicroTest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdHttpTests/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdHttpTests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7081 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdHttpTests/XrdHttpTests.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/XrdSsiTests/
--rw-r--r--   0 root         (0) root         (0)      440 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdSsiTests/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    36887 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/XrdSsiTests/XrdShMap.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/tests/common/
--rw-r--r--   0 root         (0) root         (0)      901 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2485 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/CppUnitXrdHelpers.hh
--rw-r--r--   0 root         (0) root         (0)     3148 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/PathProcessor.hh
--rw-r--r--   0 root         (0) root         (0)    12734 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/Server.cc
--rw-r--r--   0 root         (0) root         (0)     7796 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/Server.hh
--rw-r--r--   0 root         (0) root         (0)     4264 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/TestEnv.cc
--rw-r--r--   0 root         (0) root         (0)     2456 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/TestEnv.hh
--rw-r--r--   0 root         (0) root         (0)     5571 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/TextRunner.cc
--rw-r--r--   0 root         (0) root         (0)     3461 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/Utils.cc
--rw-r--r--   0 root         (0) root         (0)     4485 2023-06-30 14:28:10.000000 xrootd-5.6.0/tests/common/Utils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/ups/
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-30 14:28:10.000000 xrootd-5.6.0/ups/eupspkg.cfg.sh
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-30 14:28:10.000000 xrootd-5.6.0/ups/xrootd.table
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/utils/
--rwxr-xr-x   0 root         (0) root         (0)     6678 2023-06-30 14:28:10.000000 xrootd-5.6.0/utils/XrdCmsNotify.pm
--rwxr-xr-x   0 root         (0) root         (0)     7851 2023-06-30 14:28:10.000000 xrootd-5.6.0/utils/XrdOlbMonPerf
--rwxr-xr-x   0 root         (0) root         (0)     3789 2023-06-30 14:28:10.000000 xrootd-5.6.0/utils/cms_monPerf
--rwxr-xr-x   0 root         (0) root         (0)    29321 2023-06-30 14:28:10.000000 xrootd-5.6.0/utils/hpsscp
--rwxr-xr-x   0 root         (0) root         (0)     4187 2023-06-30 14:28:10.000000 xrootd-5.6.0/utils/netchk
--rwxr-xr-x   0 root         (0) root         (0)     2181 2023-06-30 14:28:10.000000 xrootd-5.6.0/utils/xrootd-config
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:31:35.917901 xrootd-5.6.0/xrootd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4632 2023-06-30 14:31:35.000000 xrootd-5.6.0/xrootd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    48824 2023-06-30 14:31:35.000000 xrootd-5.6.0/xrootd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 14:31:35.000000 xrootd-5.6.0/xrootd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 14:28:10.000000 xrootd-5.6.0/xrootd.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-30 14:31:35.000000 xrootd-5.6.0/xrootd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/
+-rw-rw-r--   0 root         (0) root         (0)     2426 2023-07-11 08:55:00.000000 xrootd-5.6.1/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    35147 2023-07-11 08:55:00.000000 xrootd-5.6.1/COPYING
+-rw-rw-r--   0 root         (0) root         (0)     2811 2023-07-11 08:55:00.000000 xrootd-5.6.1/COPYING.BSD
+-rw-rw-r--   0 root         (0) root         (0)     7651 2023-07-11 08:55:00.000000 xrootd-5.6.1/COPYING.LGPL
+-rw-rw-r--   0 root         (0) root         (0)     1432 2023-07-11 08:55:00.000000 xrootd-5.6.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      308 2023-07-11 08:55:00.000000 xrootd-5.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-07-11 09:20:11.873076 xrootd-5.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3791 2023-07-11 08:55:00.000000 xrootd-5.6.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)        7 2023-07-11 08:55:00.000000 xrootd-5.6.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/
+-rw-rw-r--   0 root         (0) root         (0)       57 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/
+-rwxrwxr-x   0 root         (0) root         (0)       57 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)      890 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)      130 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     8129 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/README.md
+-rw-rw-r--   0 root         (0) root         (0)        7 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/docs/
+-rw-rw-r--   0 root         (0) root         (0)     5581 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/Makefile
+-rw-rw-r--   0 root         (0) root         (0)     1225 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/ReleaseNotes.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.653075 xrootd-5.6.1/bindings/python/docs/source/.static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/docs/source/.static/css/
+-rwxrwxr-x   0 root         (0) root         (0)    15713 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/.static/css/custom.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/docs/source/.templates/
+-rwxrwxr-x   0 root         (0) root         (0)       89 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/.templates/layout.html
+-rw-rw-r--   0 root         (0) root         (0)     8013 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/docs/source/examples/
+-rw-rw-r--   0 root         (0) root         (0)      307 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/examples/copyprocess.rst
+-rw-rw-r--   0 root         (0) root         (0)     2842 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/examples/file.rst
+-rw-rw-r--   0 root         (0) root         (0)     3243 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/examples/filesystem.rst
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/examples.rst
+-rw-rw-r--   0 root         (0) root         (0)     4286 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/favicon.ico
+-rw-rw-r--   0 root         (0) root         (0)     3673 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/gettingstarted.rst
+-rw-rw-r--   0 root         (0) root         (0)      844 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/index.rst
+-rw-rw-r--   0 root         (0) root         (0)      132 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/install.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.653075 xrootd-5.6.1/bindings/python/docs/source/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/docs/source/modules/client/
+-rw-rw-r--   0 root         (0) root         (0)      423 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/copyprocess.rst
+-rw-rw-r--   0 root         (0) root         (0)     1385 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/file.rst
+-rw-rw-r--   0 root         (0) root         (0)     1293 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/filesystem.rst
+-rw-rw-r--   0 root         (0) root         (0)     5238 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/flags.rst
+-rw-rw-r--   0 root         (0) root         (0)      944 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/responses.rst
+-rw-rw-r--   0 root         (0) root         (0)      342 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/url.rst
+-rw-rw-r--   0 root         (0) root         (0)      304 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/modules/client/utils.rst
+-rw-rw-r--   0 root         (0) root         (0)    14979 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/docs/source/xrootd-200x68.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/examples/
+-rw-rw-r--   0 root         (0) root         (0)      277 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/copy.py
+-rw-rw-r--   0 root         (0) root         (0)     1655 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/copyprocess.py
+-rw-rw-r--   0 root         (0) root         (0)      550 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/dirlist.py
+-rw-rw-r--   0 root         (0) root         (0)      235 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/fcntl.py
+-rw-rw-r--   0 root         (0) root         (0)      347 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/fcntl_async.py
+-rw-rw-r--   0 root         (0) root         (0)      980 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/fileproperties.py
+-rw-rw-r--   0 root         (0) root         (0)      524 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/filesystemproperties.py
+-rw-rw-r--   0 root         (0) root         (0)      323 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/iterate.py
+-rw-rw-r--   0 root         (0) root         (0)      388 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/locate.py
+-rw-rw-r--   0 root         (0) root         (0)      214 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/mkdir.py
+-rw-rw-r--   0 root         (0) root         (0)      166 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/mv.py
+-rw-rw-r--   0 root         (0) root         (0)      621 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/query.py
+-rw-rw-r--   0 root         (0) root         (0)      749 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/read.py
+-rw-rw-r--   0 root         (0) root         (0)      349 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/readchunks.py
+-rw-rw-r--   0 root         (0) root         (0)      446 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/readlines.py
+-rw-rw-r--   0 root         (0) root         (0)      143 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/rm.py
+-rw-rw-r--   0 root         (0) root         (0)      160 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/rmdir.py
+-rw-rw-r--   0 root         (0) root         (0)      850 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/vector_read.py
+-rw-rw-r--   0 root         (0) root         (0)      226 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/visa.py
+-rw-rw-r--   0 root         (0) root         (0)      338 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/visa_async.py
+-rw-rw-r--   0 root         (0) root         (0)      356 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/examples/write.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/bindings/python/libs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.673075 xrootd-5.6.1/bindings/python/libs/client/
+-rw-rw-r--   0 root         (0) root         (0)      562 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1313 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/_version.py
+-rw-rw-r--   0 root         (0) root         (0)     7054 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/copyprocess.py
+-rw-rw-r--   0 root         (0) root         (0)     2426 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/env.py
+-rw-rw-r--   0 root         (0) root         (0)    13367 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/file.py
+-rw-rw-r--   0 root         (0) root         (0)    17398 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/filesystem.py
+-rw-rw-r--   0 root         (0) root         (0)     2113 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/finalize.py
+-rw-rw-r--   0 root         (0) root         (0)     2892 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/flags.py
+-rw-rw-r--   0 root         (0) root         (0)     4357 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/glob_funcs.py
+-rw-rw-r--   0 root         (0) root         (0)    11449 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/responses.py
+-rw-rw-r--   0 root         (0) root         (0)     2842 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/url.py
+-rw-rw-r--   0 root         (0) root         (0)     3926 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/libs/client/utils.py
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     5321 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.673075 xrootd-5.6.1/bindings/python/src/
+-rw-rw-r--   0 root         (0) root         (0)    12167 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/AsyncResponseHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     1788 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     6731 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/ChunkIterator.hh
+-rw-rw-r--   0 root         (0) root         (0)    13695 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/Conversions.hh
+-rw-rw-r--   0 root         (0) root         (0)     1898 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootD.hh
+-rw-rw-r--   0 root         (0) root         (0)     8623 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDCopyProcess.cc
+-rw-rw-r--   0 root         (0) root         (0)     6663 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDCopyProcess.hh
+-rw-rw-r--   0 root         (0) root         (0)     4415 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDCopyProgressHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)     3562 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDCopyProgressHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     5119 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDEnv.hh
+-rw-rw-r--   0 root         (0) root         (0)    35747 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDFile.cc
+-rw-rw-r--   0 root         (0) root         (0)    12239 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    37424 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDFileSystem.cc
+-rw-rw-r--   0 root         (0) root         (0)    10740 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDFileSystem.hh
+-rw-rw-r--   0 root         (0) root         (0)     2135 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDFinalize.hh
+-rw-rw-r--   0 root         (0) root         (0)     5199 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDModule.cc
+-rw-rw-r--   0 root         (0) root         (0)     7622 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDURL.cc
+-rw-rw-r--   0 root         (0) root         (0)     8015 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/PyXRootDURL.hh
+-rw-rw-r--   0 root         (0) root         (0)     6144 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/Utils.cc
+-rw-rw-r--   0 root         (0) root         (0)     4293 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/Utils.hh
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.673075 xrootd-5.6.1/bindings/python/tests/
+-rw-rw-r--   0 root         (0) root         (0)      237 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/env.py
+-rw-rw-r--   0 root         (0) root         (0)     1839 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/test_copy.py
+-rw-rw-r--   0 root         (0) root         (0)    11797 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/test_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5387 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/test_filesystem.py
+-rw-rw-r--   0 root         (0) root         (0)     1728 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/test_glob.py
+-rw-rw-r--   0 root         (0) root         (0)      785 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/test_threads.py
+-rw-rw-r--   0 root         (0) root         (0)     1340 2023-07-11 08:55:00.000000 xrootd-5.6.1/bindings/python/tests/test_url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.673075 xrootd-5.6.1/cmake/
+-rw-rw-r--   0 root         (0) root         (0)      256 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindAutoConf.cmake
+-rw-rw-r--   0 root         (0) root         (0)      256 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindAutoMake.cmake
+-rw-rw-r--   0 root         (0) root         (0)      695 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindCppUnit.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1816 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindDavix.cmake
+-rw-rw-r--   0 root         (0) root         (0)      839 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindKerberos5.cmake
+-rw-rw-r--   0 root         (0) root         (0)      251 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindLibTool.cmake
+-rw-rw-r--   0 root         (0) root         (0)      393 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindMacaroons.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1699 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindReadline.cmake
+-rw-rw-r--   0 root         (0) root         (0)      434 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindSciTokensCpp.cmake
+-rw-rw-r--   0 root         (0) root         (0)      365 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindTinyXml.cmake
+-rw-rw-r--   0 root         (0) root         (0)      649 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindVOMS.cmake
+-rw-rw-r--   0 root         (0) root         (0)      236 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/FindYasm.cmake
+-rw-rw-r--   0 root         (0) root         (0)      740 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/Findfuse.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1704 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/Findisal.cmake
+-rw-rw-r--   0 root         (0) root         (0)     2931 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/Findlibuuid.cmake
+-rw-rw-r--   0 root         (0) root         (0)      683 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/Findsystemd.cmake
+-rw-rw-r--   0 root         (0) root         (0)     7570 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDConfig.cmake.in
+-rw-rw-r--   0 root         (0) root         (0)     2363 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDDefaults.cmake
+-rw-rw-r--   0 root         (0) root         (0)     4768 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDFindLibs.cmake
+-rw-rw-r--   0 root         (0) root         (0)     7219 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDOSDefs.cmake
+-rw-rw-r--   0 root         (0) root         (0)     2691 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDSummary.cmake
+-rw-rw-r--   0 root         (0) root         (0)     6716 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDSystemCheck.cmake
+-rw-rw-r--   0 root         (0) root         (0)     2565 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDUtils.cmake
+-rw-rw-r--   0 root         (0) root         (0)     3053 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake/XRootDVersion.cmake
+-rw-rw-r--   0 root         (0) root         (0)      941 2023-07-11 08:55:00.000000 xrootd-5.6.1/cmake_uninstall.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.673075 xrootd-5.6.1/docs/
+-rw-rw-r--   0 root         (0) root         (0)    11322 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/CONTRIBUTING.md
+-rw-rw-r--   0 root         (0) root         (0)     7846 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/INSTALL.md
+-rw-rw-r--   0 root         (0) root         (0)       58 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/PreReleaseNotes.txt
+-rw-rw-r--   0 root         (0) root         (0)     4415 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/README_IPV4_To_IPV6
+-rw-rw-r--   0 root         (0) root         (0)   175482 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/ReleaseNotes.txt
+-rw-rw-r--   0 root         (0) root         (0)    18648 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/TESTING.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/docs/man/
+-rw-rw-r--   0 root         (0) root         (0)      938 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/cmsd.8
+-rw-rw-r--   0 root         (0) root         (0)     1022 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/frm_admin.8
+-rw-rw-r--   0 root         (0) root         (0)     1062 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/frm_purged.8
+-rw-rw-r--   0 root         (0) root         (0)      929 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/frm_xfragent.8
+-rw-rw-r--   0 root         (0) root         (0)     1016 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/frm_xfrd.8
+-rw-rw-r--   0 root         (0) root         (0)     4438 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/libXrdVoms.1
+-rw-rw-r--   0 root         (0) root         (0)     1046 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/mpxstats.8
+-rw-rw-r--   0 root         (0) root         (0)     1019 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdadler32.1
+-rw-rw-r--   0 root         (0) root         (0)    17367 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdcp.1
+-rw-rw-r--   0 root         (0) root         (0)     6398 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdfs.1
+-rw-rw-r--   0 root         (0) root         (0)     1792 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdgsiproxy.1
+-rw-rw-r--   0 root         (0) root         (0)     6823 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdgsitest.1
+-rw-rw-r--   0 root         (0) root         (0)     1322 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdmapc.1
+-rw-rw-r--   0 root         (0) root         (0)     2071 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdpfc_print.8
+-rw-rw-r--   0 root         (0) root         (0)      872 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdpwdadmin.8
+-rw-rw-r--   0 root         (0) root         (0)      850 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrdsssadmin.8
+-rw-rw-r--   0 root         (0) root         (0)      993 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrootd.8
+-rw-rw-r--   0 root         (0) root         (0)     3745 2023-07-11 08:55:00.000000 xrootd-5.6.1/docs/man/xrootdfs.1
+-rwxrwxr-x   0 root         (0) root         (0)      772 2023-07-11 08:55:00.000000 xrootd-5.6.1/gen-tarball.sh
+-rwxrwxr-x   0 root         (0) root         (0)     1354 2023-07-11 08:55:00.000000 xrootd-5.6.1/genversion.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/common/
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/client-plugin.conf.example
+-rw-rw-r--   0 root         (0) root         (0)     6149 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/client.conf
+-rw-rw-r--   0 root         (0) root         (0)      685 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/cmsd@.service
+-rw-rw-r--   0 root         (0) root         (0)      680 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/frm_purged@.service
+-rw-rw-r--   0 root         (0) root         (0)      670 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/frm_xfrd@.service
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/http.client.conf.example
+-rw-rw-r--   0 root         (0) root         (0)       61 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/recorder.conf
+-rw-rw-r--   0 root         (0) root         (0)      121 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrdhttp@.socket
+-rw-rw-r--   0 root         (0) root         (0)     3006 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd-clustered.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3342 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd-filecache-clustered.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1666 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd-filecache-standalone.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1986 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd-http.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1590 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd-standalone.cfg
+-rw-rw-r--   0 root         (0) root         (0)      626 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd.logrotate
+-rw-rw-r--   0 root         (0) root         (0)      680 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd.te
+-rw-rw-r--   0 root         (0) root         (0)      695 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd@.service
+-rw-rw-r--   0 root         (0) root         (0)      122 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/common/xrootd@.socket
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/debian/
+-rw-rw-r--   0 root         (0) root         (0)        3 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/compat
+-rw-rw-r--   0 root         (0) root         (0)    16401 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/control
+-rw-rw-r--   0 root         (0) root         (0)     1328 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/copyright
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdapputils1.install
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdcl2.install
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdcrypto1.install
+-rw-rw-r--   0 root         (0) root         (0)       32 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdcryptolite1.install
+-rw-rw-r--   0 root         (0) root         (0)       25 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdffs2.install
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdhttputils1.install
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdposix2.install
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdserver2.install
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdssilib1.install
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdssishmap1.install
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdutils2.install
+-rw-rw-r--   0 root         (0) root         (0)       25 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrdxml2.install
+-rw-rw-r--   0 root         (0) root         (0)      175 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrootd-client-dev.install
+-rw-rw-r--   0 root         (0) root         (0)      453 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrootd-dev.install
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrootd-private-dev.install
+-rw-rw-r--   0 root         (0) root         (0)      241 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/libxrootd-server-dev.install
+-rw-rw-r--   0 root         (0) root         (0)       33 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/python3-xrootd.install
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/python3-xrootd.install.new
+-rwxrwxr-x   0 root         (0) root         (0)      932 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/rules
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/debian/source/
+-rw-rw-r--   0 root         (0) root         (0)       12 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/source/format
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-client-devel.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-client-libs.install
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-client-plugins.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-client.install
+-rw-rw-r--   0 root         (0) root         (0)      378 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-clients.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-devel.install
+-rw-rw-r--   0 root         (0) root         (0)       58 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-fuse.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-libs.install
+-rw-rw-r--   0 root         (0) root         (0)       83 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-plugins.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-private-devel.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-server-devel.install
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-server-libs.install
+-rw-rw-r--   0 root         (0) root         (0)      378 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-server-plugins.install
+-rw-rw-r--   0 root         (0) root         (0)      542 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian/xrootd-server.install
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/debian_scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     1738 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/debian_scripts/publish_debian_cern.sh
+-rwxrwxr-x   0 root         (0) root         (0)     7960 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/makesrpm.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/rhel/
+-rw-rw-r--   0 root         (0) root         (0)      809 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/cmsd.init
+-rw-rw-r--   0 root         (0) root         (0)      859 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/frm_purged.init
+-rw-rw-r--   0 root         (0) root         (0)      839 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/frm_xfrd.init
+-rw-rw-r--   0 root         (0) root         (0)     8866 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/xrootd.functions
+-rw-rw-r--   0 root         (0) root         (0)     8451 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/xrootd.functions-slc4
+-rw-rw-r--   0 root         (0) root         (0)      861 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/xrootd.init
+-rw-rw-r--   0 root         (0) root         (0)    37002 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/xrootd.spec.in
+-rw-rw-r--   0 root         (0) root         (0)     3489 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/xrootd.sysconfig
+-rw-rw-r--   0 root         (0) root         (0)       32 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/rhel/xrootd.tmpfiles
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/tgz/
+-rw-rw-r--   0 root         (0) root         (0)     2043 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/README
+-rwxrwxr-x   0 root         (0) root         (0)     4590 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StartCMS
+-rwxrwxr-x   0 root         (0) root         (0)     4388 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StartFRM
+-rwxrwxr-x   0 root         (0) root         (0)     5420 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StartOLB
+-rw-rw-r--   0 root         (0) root         (0)     2063 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StartOLB.cf.example
+-rwxrwxr-x   0 root         (0) root         (0)     4767 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StartXRD
+-rw-rw-r--   0 root         (0) root         (0)     3842 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StartXRD.cf.example
+-rwxrwxr-x   0 root         (0) root         (0)     3039 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StopCMS
+-rwxrwxr-x   0 root         (0) root         (0)     3735 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StopFRM
+-rwxrwxr-x   0 root         (0) root         (0)     2910 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StopOLB
+-rwxrwxr-x   0 root         (0) root         (0)     2615 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/StopXRD
+-rw-rw-r--   0 root         (0) root         (0)     1988 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/xrootd.cf.example
+-rw-rw-r--   0 root         (0) root         (0)     3914 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/tgz/xrootd.cf.example2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.683075 xrootd-5.6.1/packaging/wheel/
+-rwxrwxr-x   0 root         (0) root         (0)     1169 2023-07-11 08:55:00.000000 xrootd-5.6.1/packaging/wheel/publish.sh
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-11 08:55:00.000000 xrootd-5.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 09:20:11.873076 xrootd-5.6.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4228 2023-07-11 08:55:00.000000 xrootd-5.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.693075 xrootd-5.6.1/src/
+-rw-rw-r--   0 root         (0) root         (0)     3848 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.693075 xrootd-5.6.1/src/XProtocol/
+-rw-rw-r--   0 root         (0) root         (0)      947 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XProtocol/README
+-rw-rw-r--   0 root         (0) root         (0)    11295 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XProtocol/XProtocol.cc
+-rw-rw-r--   0 root         (0) root         (0)    51065 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XProtocol/XProtocol.hh
+-rw-rw-r--   0 root         (0) root         (0)     5574 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XProtocol/XPtypes.hh
+-rw-rw-r--   0 root         (0) root         (0)    25337 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XProtocol/YProtocol.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.693075 xrootd-5.6.1/src/Xrd/
+-rw-rw-r--   0 root         (0) root         (0)     9005 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdBuffXL.cc
+-rw-rw-r--   0 root         (0) root         (0)     3279 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdBuffXL.hh
+-rw-rw-r--   0 root         (0) root         (0)    11819 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdBuffer.cc
+-rw-rw-r--   0 root         (0) root         (0)     4299 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdBuffer.hh
+-rw-rw-r--   0 root         (0) root         (0)    93305 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     5661 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     2900 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdGlobals.cc
+-rw-rw-r--   0 root         (0) root         (0)     9400 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdInet.cc
+-rw-rw-r--   0 root         (0) root         (0)     3445 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdInet.hh
+-rw-rw-r--   0 root         (0) root         (0)     2840 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)     2489 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     3099 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdJob.hh
+-rw-rw-r--   0 root         (0) root         (0)    25173 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLink.cc
+-rw-rw-r--   0 root         (0) root         (0)    26923 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLink.hh
+-rw-rw-r--   0 root         (0) root         (0)    14522 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkCtl.cc
+-rw-rw-r--   0 root         (0) root         (0)     9846 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkCtl.hh
+-rw-rw-r--   0 root         (0) root         (0)     3499 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     5054 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkMatch.cc
+-rw-rw-r--   0 root         (0) root         (0)     3288 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkMatch.hh
+-rw-rw-r--   0 root         (0) root         (0)    46764 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkXeq.cc
+-rw-rw-r--   0 root         (0) root         (0)     7101 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdLinkXeq.hh
+-rw-rw-r--   0 root         (0) root         (0)     8748 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdMain.cc
+-rw-rw-r--   0 root         (0) root         (0)     5456 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdObject.hh
+-rw-rw-r--   0 root         (0) root         (0)     4407 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdObject.icc
+-rw-rw-r--   0 root         (0) root         (0)    12682 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPoll.cc
+-rw-rw-r--   0 root         (0) root         (0)     5644 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPoll.hh
+-rw-rw-r--   0 root         (0) root         (0)     3601 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPollE.hh
+-rw-rw-r--   0 root         (0) root         (0)    14457 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPollE.icc
+-rw-rw-r--   0 root         (0) root         (0)     3308 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPollInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     3207 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPollPoll.hh
+-rw-rw-r--   0 root         (0) root         (0)    17863 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdPollPoll.icc
+-rw-rw-r--   0 root         (0) root         (0)    12456 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdProtLoad.cc
+-rw-rw-r--   0 root         (0) root         (0)     3854 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdProtLoad.hh
+-rw-rw-r--   0 root         (0) root         (0)    10727 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdProtocol.hh
+-rw-rw-r--   0 root         (0) root         (0)    24210 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdScheduler.cc
+-rw-rw-r--   0 root         (0) root         (0)     5635 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdScheduler.hh
+-rw-rw-r--   0 root         (0) root         (0)    13605 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdSendQ.cc
+-rw-rw-r--   0 root         (0) root         (0)     3735 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdSendQ.hh
+-rw-rw-r--   0 root         (0) root         (0)    12208 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdStats.cc
+-rw-rw-r--   0 root         (0) root         (0)     3836 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdStats.hh
+-rw-rw-r--   0 root         (0) root         (0)     4914 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdTcpMonPin.hh
+-rw-rw-r--   0 root         (0) root         (0)     3291 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/Xrd/XrdTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.703076 xrootd-5.6.1/src/XrdAcc/
+-rw-rw-r--   0 root         (0) root         (0)    18177 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAccess.cc
+-rw-rw-r--   0 root         (0) root         (0)     8058 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAccess.hh
+-rw-rw-r--   0 root         (0) root         (0)     4734 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAudit.cc
+-rw-rw-r--   0 root         (0) root         (0)     5263 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAudit.hh
+-rw-rw-r--   0 root         (0) root         (0)     5258 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAuthDB.hh
+-rw-rw-r--   0 root         (0) root         (0)    12972 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAuthFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     3587 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAuthFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    12043 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccAuthorize.hh
+-rw-rw-r--   0 root         (0) root         (0)     7602 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccCapability.cc
+-rw-rw-r--   0 root         (0) root         (0)     5914 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccCapability.hh
+-rw-rw-r--   0 root         (0) root         (0)    34347 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     5754 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     8327 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccEntity.cc
+-rw-rw-r--   0 root         (0) root         (0)     5422 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccEntity.hh
+-rw-rw-r--   0 root         (0) root         (0)    15542 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccGroups.cc
+-rw-rw-r--   0 root         (0) root         (0)     7392 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccGroups.hh
+-rw-rw-r--   0 root         (0) root         (0)     4791 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdAcc/XrdAccPrivs.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.703076 xrootd-5.6.1/src/XrdApps/
+-rw-rw-r--   0 root         (0) root         (0)    14593 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdAccTest.cc
+-rw-rw-r--   0 root         (0) root         (0)     7202 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdAppsCconfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     6428 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdCks.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.703076 xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/
+-rw-rw-r--   0 root         (0) root         (0)     7035 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc
+-rw-rw-r--   0 root         (0) root         (0)    12371 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     4214 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc
+-rw-rw-r--   0 root         (0) root         (0)     2721 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh
+-rw-rw-r--   0 root         (0) root         (0)     1822 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.703076 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/
+-rw-rw-r--   0 root         (0) root         (0)    14346 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/README.md
+-rw-rw-r--   0 root         (0) root         (0)    13235 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh
+-rw-rw-r--   0 root         (0) root         (0)     9856 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh
+-rw-rw-r--   0 root         (0) root         (0)    18873 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh
+-rw-rw-r--   0 root         (0) root         (0)     1639 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3178 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh
+-rw-rw-r--   0 root         (0) root         (0)    53534 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc
+-rw-rw-r--   0 root         (0) root         (0)     7563 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh
+-rw-rw-r--   0 root         (0) root         (0)    40660 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdCpConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)    13017 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdCpConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     7118 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdCpFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     3726 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdCpFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     6098 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdCrc32c.cc
+-rw-rw-r--   0 root         (0) root         (0)    19913 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdMapCluster.cc
+-rw-rw-r--   0 root         (0) root         (0)    10463 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdMpxStats.cc
+-rw-rw-r--   0 root         (0) root         (0)    15785 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdMpxXml.cc
+-rw-rw-r--   0 root         (0) root         (0)     3279 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdMpxXml.hh
+-rw-rw-r--   0 root         (0) root         (0)     5291 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdPinls.cc
+-rw-rw-r--   0 root         (0) root         (0)    10301 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdPrep.cc
+-rw-rw-r--   0 root         (0) root         (0)     8490 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdQStats.cc
+-rw-rw-r--   0 root         (0) root         (0)    10451 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/XrdWait41.cc
+-rw-rw-r--   0 root         (0) root         (0)     9299 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps/Xrdadler32.cc
+-rw-rw-r--   0 root         (0) root         (0)     6565 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdApps.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.703076 xrootd-5.6.1/src/XrdBwm/
+-rw-rw-r--   0 root         (0) root         (0)    38144 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwm.cc
+-rw-rw-r--   0 root         (0) root         (0)    12819 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwm.hh
+-rw-rw-r--   0 root         (0) root         (0)    15615 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)    14111 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmHandle.cc
+-rw-rw-r--   0 root         (0) root         (0)     4374 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmHandle.hh
+-rw-rw-r--   0 root         (0) root         (0)    11034 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmLogger.cc
+-rw-rw-r--   0 root         (0) root         (0)     3761 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmLogger.hh
+-rw-rw-r--   0 root         (0) root         (0)     8624 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmPolicy.hh
+-rw-rw-r--   0 root         (0) root         (0)     6036 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmPolicy1.cc
+-rw-rw-r--   0 root         (0) root         (0)     4429 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmPolicy1.hh
+-rw-rw-r--   0 root         (0) root         (0)     3393 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdBwm/XrdBwmTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.703076 xrootd-5.6.1/src/XrdCeph/
+-rw-rw-r--   0 root         (0) root         (0)       26 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/.gitattributes
+-rw-rw-r--   0 root         (0) root         (0)     1036 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     4416 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/.gitlab-ci.yml
+-rw-rw-r--   0 root         (0) root         (0)      402 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)     1760 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    35147 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/COPYING
+-rw-rw-r--   0 root         (0) root         (0)     2811 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/COPYING.BSD
+-rw-rw-r--   0 root         (0) root         (0)     7651 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/COPYING.LGPL
+-rw-rw-r--   0 root         (0) root         (0)    11172 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/Doxyfile
+-rw-rw-r--   0 root         (0) root         (0)     1432 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1626 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/README
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/VERSION_INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/cmake/
+-rw-rw-r--   0 root         (0) root         (0)      695 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/FindCppUnit.cmake
+-rw-rw-r--   0 root         (0) root         (0)      840 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/FindXRootD.cmake
+-rw-rw-r--   0 root         (0) root         (0)      741 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/Findceph.cmake
+-rw-rw-r--   0 root         (0) root         (0)     7023 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/GNUInstallDirs.cmake
+-rw-rw-r--   0 root         (0) root         (0)      541 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/XRootDDefaults.cmake
+-rw-rw-r--   0 root         (0) root         (0)      408 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/XRootDFindLibs.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1793 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/XRootDOSDefs.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1063 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/XRootDSummary.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1417 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/cmake/XRootDUtils.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/docs/
+-rw-rw-r--   0 root         (0) root         (0)       58 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/docs/PreReleaseNotes.txt
+-rw-rw-r--   0 root         (0) root         (0)    86325 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/docs/ReleaseNotes.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/packaging/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/packaging/debian/
+-rw-rw-r--   0 root         (0) root         (0)        3 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/compat
+-rw-rw-r--   0 root         (0) root         (0)     2282 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/control
+-rw-rw-r--   0 root         (0) root         (0)     1432 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/copyright
+-rwxrwxr-x   0 root         (0) root         (0)      538 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/rules
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/packaging/debian/source/
+-rw-rw-r--   0 root         (0) root         (0)       12 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/source/format
+-rw-rw-r--   0 root         (0) root         (0)      230 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-client-devel.install
+-rw-rw-r--   0 root         (0) root         (0)      253 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-client-libs.install
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-client-libs.postinst
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-client-libs.postrm
+-rw-rw-r--   0 root         (0) root         (0)      422 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-client.install
+-rw-rw-r--   0 root         (0) root         (0)      411 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-devel.install
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-libs.install
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-libs.postinst
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-libs.postrm
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-private-devel.install
+-rw-rw-r--   0 root         (0) root         (0)      218 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-server-devel.install
+-rw-rw-r--   0 root         (0) root         (0)      403 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-server-libs.install
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-server-libs.postinst
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian/xrootd-server-libs.postrm
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/packaging/debian_scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     1741 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/debian_scripts/publish_debian_cern.sh
+-rwxrwxr-x   0 root         (0) root         (0)     8169 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/makesrpm.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/packaging/rhel/
+-rw-rw-r--   0 root         (0) root         (0)     4609 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/packaging/rhel/xrootd-ceph.spec.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/src/
+-rw-rw-r--   0 root         (0) root         (0)      341 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/
+-rw-rw-r--   0 root         (0) root         (0)     8360 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOss.cc
+-rw-rw-r--   0 root         (0) root         (0)     3728 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOss.hh
+-rw-rw-r--   0 root         (0) root         (0)     2049 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssDir.cc
+-rw-rw-r--   0 root         (0) root         (0)     3121 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssDir.hh
+-rw-rw-r--   0 root         (0) root         (0)     3209 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     3330 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    43976 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephPosix.cc
+-rw-rw-r--   0 root         (0) root         (0)     3885 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephPosix.hh
+-rw-rw-r--   0 root         (0) root         (0)     3838 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephXAttr.cc
+-rw-rw-r--   0 root         (0) root         (0)     7877 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephXAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     2369 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdCeph.cmake
+-rw-rw-r--   0 root         (0) root         (0)     5174 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/src/XrdVersion.hh.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/tests/
+-rw-rw-r--   0 root         (0) root         (0)       33 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCeph/tests/XrdCephTests/
+-rw-rw-r--   0 root         (0) root         (0)      672 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/tests/XrdCephTests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     6661 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCeph/tests/XrdCephTests/CephParsingTest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.713075 xrootd-5.6.1/src/XrdCks/
+-rw-rw-r--   0 root         (0) root         (0)    16444 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCks.hh
+-rw-rw-r--   0 root         (0) root         (0)     7765 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksAssist.cc
+-rw-rw-r--   0 root         (0) root         (0)     6718 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksAssist.hh
+-rw-rw-r--   0 root         (0) root         (0)     8525 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalc.hh
+-rw-rw-r--   0 root         (0) root         (0)     5687 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalcadler32.hh
+-rw-rw-r--   0 root         (0) root         (0)     8639 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32.cc
+-rw-rw-r--   0 root         (0) root         (0)     3654 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32.hh
+-rw-rw-r--   0 root         (0) root         (0)     1003 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32C.cc
+-rw-rw-r--   0 root         (0) root         (0)     2986 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32C.hh
+-rw-rw-r--   0 root         (0) root         (0)    12260 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalcmd5.cc
+-rw-rw-r--   0 root         (0) root         (0)     3564 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalcmd5.hh
+-rw-rw-r--   0 root         (0) root         (0)     5036 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksCalczcrc32.cc
+-rw-rw-r--   0 root         (0) root         (0)    10222 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     3663 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     5671 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksData.hh
+-rw-rw-r--   0 root         (0) root         (0)     7928 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksLoader.cc
+-rw-rw-r--   0 root         (0) root         (0)     6105 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksLoader.hh
+-rw-rw-r--   0 root         (0) root         (0)     9341 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksManOss.cc
+-rw-rw-r--   0 root         (0) root         (0)     3480 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksManOss.hh
+-rw-rw-r--   0 root         (0) root         (0)    21161 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     5041 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    14952 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksWrapper.hh
+-rw-rw-r--   0 root         (0) root         (0)     4283 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCks/XrdCksXAttr.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.733075 xrootd-5.6.1/src/XrdCl/
+-rw-rw-r--   0 root         (0) root         (0)     8568 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     5609 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAnyObject.hh
+-rw-rw-r--   0 root         (0) root         (0)     3364 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClApply.hh
+-rw-rw-r--   0 root         (0) root         (0)    13157 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClArg.hh
+-rw-rw-r--   0 root         (0) root         (0)     3439 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncDiscardReader.hh
+-rw-rw-r--   0 root         (0) root         (0)     7661 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncHSReader.hh
+-rw-rw-r--   0 root         (0) root         (0)     5998 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncHSWriter.hh
+-rw-rw-r--   0 root         (0) root         (0)    15590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncMsgReader.hh
+-rw-rw-r--   0 root         (0) root         (0)    10892 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncMsgWriter.hh
+-rw-rw-r--   0 root         (0) root         (0)    12785 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncPageReader.hh
+-rw-rw-r--   0 root         (0) root         (0)     8622 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncRawReader.hh
+-rw-rw-r--   0 root         (0) root         (0)     7097 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncRawReaderIntfc.hh
+-rw-rw-r--   0 root         (0) root         (0)    35098 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncSocketHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)    13692 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncSocketHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)    11781 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClAsyncVectorReader.hh
+-rw-rw-r--   0 root         (0) root         (0)     9115 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClBuffer.hh
+-rw-rw-r--   0 root         (0) root         (0)     9000 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClChannel.cc
+-rw-rw-r--   0 root         (0) root         (0)     7455 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClChannel.hh
+-rw-rw-r--   0 root         (0) root         (0)     2701 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClChannelHandlerList.cc
+-rw-rw-r--   0 root         (0) root         (0)     2547 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClChannelHandlerList.hh
+-rw-rw-r--   0 root         (0) root         (0)     5702 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCheckSumHelper.hh
+-rw-rw-r--   0 root         (0) root         (0)     5843 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCheckSumManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     3367 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCheckSumManager.hh
+-rw-rw-r--   0 root         (0) root         (0)     8890 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCheckpointOperation.hh
+-rw-rw-r--   0 root         (0) root         (0)   109531 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClClassicCopyJob.cc
+-rw-rw-r--   0 root         (0) root         (0)     3921 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClClassicCopyJob.hh
+-rw-rw-r--   0 root         (0) root         (0)     9840 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClConstants.hh
+-rw-rw-r--   0 root         (0) root         (0)    33054 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCopy.cc
+-rw-rw-r--   0 root         (0) root         (0)     4256 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCopyJob.hh
+-rw-rw-r--   0 root         (0) root         (0)    21403 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCopyProcess.cc
+-rw-rw-r--   0 root         (0) root         (0)     9463 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCopyProcess.hh
+-rw-rw-r--   0 root         (0) root         (0)     4723 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClCtx.hh
+-rw-rw-r--   0 root         (0) root         (0)    34739 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClDefaultEnv.cc
+-rw-rw-r--   0 root         (0) root         (0)     8248 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClDefaultEnv.hh
+-rw-rw-r--   0 root         (0) root         (0)     2452 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClDlgEnv.hh
+-rw-rw-r--   0 root         (0) root         (0)     7058 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClEcHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)    17884 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClEcHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     8264 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClEnv.cc
+-rw-rw-r--   0 root         (0) root         (0)     7930 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClEnv.hh
+-rw-rw-r--   0 root         (0) root         (0)    79044 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFS.cc
+-rw-rw-r--   0 root         (0) root         (0)     3598 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFSExecutor.cc
+-rw-rw-r--   0 root         (0) root         (0)     4052 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFSExecutor.hh
+-rw-rw-r--   0 root         (0) root         (0)    35374 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFile.cc
+-rw-rw-r--   0 root         (0) root         (0)    43555 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    61991 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileOperations.hh
+-rw-rw-r--   0 root         (0) root         (0)   134550 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileStateHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)    49347 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileStateHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)    82862 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileSystem.cc
+-rw-rw-r--   0 root         (0) root         (0)    47082 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileSystem.hh
+-rw-rw-r--   0 root         (0) root         (0)    58105 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileSystemOperations.hh
+-rw-rw-r--   0 root         (0) root         (0)     7347 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileSystemUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     3917 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileSystemUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     1775 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileTimer.cc
+-rw-rw-r--   0 root         (0) root         (0)     3561 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFileTimer.hh
+-rw-rw-r--   0 root         (0) root         (0)     2754 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFinalOperation.hh
+-rw-rw-r--   0 root         (0) root         (0)     4753 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClForkHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)     4421 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClForkHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     9899 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClFwd.hh
+-rw-rw-r--   0 root         (0) root         (0)     6373 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClInQueue.cc
+-rw-rw-r--   0 root         (0) root         (0)     4732 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClInQueue.hh
+-rw-rw-r--   0 root         (0) root         (0)     5126 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClJobManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     4860 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClJobManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    36455 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClLocalFileHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)    17612 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClLocalFileHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     1604 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClLocalFileTask.cc
+-rw-rw-r--   0 root         (0) root         (0)     1608 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClLocalFileTask.hh
+-rw-rw-r--   0 root         (0) root         (0)     9775 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClLog.cc
+-rw-rw-r--   0 root         (0) root         (0)    10484 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClLog.hh
+-rw-rw-r--   0 root         (0) root         (0)     5392 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClMessage.hh
+-rw-rw-r--   0 root         (0) root         (0)    20035 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClMessageUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)    12633 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClMessageUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)    18515 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClMetalinkRedirector.cc
+-rw-rw-r--   0 root         (0) root         (0)     8397 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClMetalinkRedirector.hh
+-rw-rw-r--   0 root         (0) root         (0)    10542 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClMonitor.hh
+-rw-rw-r--   0 root         (0) root         (0)    29362 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOperationHandlers.hh
+-rw-rw-r--   0 root         (0) root         (0)     1066 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOperationTimeout.hh
+-rw-rw-r--   0 root         (0) root         (0)     9955 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOperations.cc
+-rw-rw-r--   0 root         (0) root         (0)    31192 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOperations.hh
+-rw-rw-r--   0 root         (0) root         (0)     1295 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOptimizers.hh
+-rw-rw-r--   0 root         (0) root         (0)     6499 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOptional.hh
+-rw-rw-r--   0 root         (0) root         (0)     5396 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOutQueue.cc
+-rw-rw-r--   0 root         (0) root         (0)     6707 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClOutQueue.hh
+-rw-rw-r--   0 root         (0) root         (0)    22037 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClParallelOperation.hh
+-rw-rw-r--   0 root         (0) root         (0)    26771 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPlugInInterface.hh
+-rw-rw-r--   0 root         (0) root         (0)    18005 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPlugInManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     7482 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPlugInManager.hh
+-rw-rw-r--   0 root         (0) root         (0)     7217 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPoller.hh
+-rw-rw-r--   0 root         (0) root         (0)    20602 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPollerBuiltIn.cc
+-rw-rw-r--   0 root         (0) root         (0)     7251 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPollerBuiltIn.hh
+-rw-rw-r--   0 root         (0) root         (0)     3701 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPollerFactory.cc
+-rw-rw-r--   0 root         (0) root         (0)     2014 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPollerFactory.hh
+-rw-rw-r--   0 root         (0) root         (0)    18175 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPostMaster.cc
+-rw-rw-r--   0 root         (0) root         (0)     9880 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPostMaster.hh
+-rw-rw-r--   0 root         (0) root         (0)    24240 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPostMasterInterfaces.hh
+-rw-rw-r--   0 root         (0) root         (0)    11305 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClPropertyList.hh
+-rw-rw-r--   0 root         (0) root         (0)     4552 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClRedirectorRegistry.cc
+-rw-rw-r--   0 root         (0) root         (0)     8258 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClRedirectorRegistry.hh
+-rw-rw-r--   0 root         (0) root         (0)     4186 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClRequestSync.hh
+-rw-rw-r--   0 root         (0) root         (0)     2659 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClResponseJob.hh
+-rw-rw-r--   0 root         (0) root         (0)     7628 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClSIDManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     8555 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClSIDManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    30690 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClSocket.cc
+-rw-rw-r--   0 root         (0) root         (0)    15672 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClSocket.hh
+-rw-rw-r--   0 root         (0) root         (0)     5694 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClStatus.cc
+-rw-rw-r--   0 root         (0) root         (0)     7140 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClStatus.hh
+-rw-rw-r--   0 root         (0) root         (0)    48094 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClStream.cc
+-rw-rw-r--   0 root         (0) root         (0)    16875 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClStream.hh
+-rw-rw-r--   0 root         (0) root         (0)     3611 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClSyncQueue.hh
+-rw-rw-r--   0 root         (0) root         (0)     3609 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTPFallBackCopyJob.cc
+-rw-rw-r--   0 root         (0) root         (0)     2541 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTPFallBackCopyJob.hh
+-rw-rw-r--   0 root         (0) root         (0)     8986 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTaskManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     6199 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTaskManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    34437 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClThirdPartyCopyJob.cc
+-rw-rw-r--   0 root         (0) root         (0)     3740 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClThirdPartyCopyJob.hh
+-rw-rw-r--   0 root         (0) root         (0)    15842 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTls.cc
+-rw-rw-r--   0 root         (0) root         (0)     6552 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTls.hh
+-rw-rw-r--   0 root         (0) root         (0)     3056 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTransportManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     2786 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClTransportManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    17135 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClURL.cc
+-rw-rw-r--   0 root         (0) root         (0)    11760 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClURL.hh
+-rw-rw-r--   0 root         (0) root         (0)    32898 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)    18037 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     5297 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXCpCtx.cc
+-rw-rw-r--   0 root         (0) root         (0)     8289 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXCpCtx.hh
+-rw-rw-r--   0 root         (0) root         (0)    17327 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXCpSrc.cc
+-rw-rw-r--   0 root         (0) root         (0)     9459 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXCpSrc.hh
+-rw-rw-r--   0 root         (0) root         (0)    94961 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXRootDMsgHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)    28694 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXRootDMsgHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)    26744 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXRootDResponses.cc
+-rw-rw-r--   0 root         (0) root         (0)    45771 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXRootDResponses.hh
+-rw-rw-r--   0 root         (0) root         (0)   130343 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXRootDTransport.cc
+-rw-rw-r--   0 root         (0) root         (0)    22673 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClXRootDTransport.hh
+-rw-rw-r--   0 root         (0) root         (0)    43178 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClZipArchive.cc
+-rw-rw-r--   0 root         (0) root         (0)    28344 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClZipArchive.hh
+-rw-rw-r--   0 root         (0) root         (0)     8602 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClZipCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     4065 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClZipListHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)     5224 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClZipListHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)    27700 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCl/XrdClZipOperations.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.743075 xrootd-5.6.1/src/XrdClHttp/
+-rw-rw-r--   0 root         (0) root         (0)      415 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    13948 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpFilePlugIn.cc
+-rw-rw-r--   0 root         (0) root         (0)     5602 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpFilePlugIn.hh
+-rw-rw-r--   0 root         (0) root         (0)     7554 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc
+-rw-rw-r--   0 root         (0) root         (0)     1885 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh
+-rw-rw-r--   0 root         (0) root         (0)      692 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpPlugInFactory.cc
+-rw-rw-r--   0 root         (0) root         (0)      481 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpPlugInFactory.hh
+-rw-rw-r--   0 root         (0) root         (0)      422 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpPlugInUtil.cc
+-rw-rw-r--   0 root         (0) root         (0)      361 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpPlugInUtil.hh
+-rw-rw-r--   0 root         (0) root         (0)    16027 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpPosix.cc
+-rw-rw-r--   0 root         (0) root         (0)     2617 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdClHttp/XrdClHttpPosix.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.753075 xrootd-5.6.1/src/XrdCms/
+-rw-rw-r--   0 root         (0) root         (0)    29034 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsAdmin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3908 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsAdmin.hh
+-rw-rw-r--   0 root         (0) root         (0)    15740 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsBaseFS.cc
+-rw-rw-r--   0 root         (0) root         (0)     8998 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsBaseFS.hh
+-rw-rw-r--   0 root         (0) root         (0)    19325 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsBlackList.cc
+-rw-rw-r--   0 root         (0) root         (0)     5380 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsBlackList.hh
+-rw-rw-r--   0 root         (0) root         (0)    21145 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsCache.cc
+-rw-rw-r--   0 root         (0) root         (0)     5021 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     3239 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClient.cc
+-rw-rw-r--   0 root         (0) root         (0)    22441 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClient.hh
+-rw-rw-r--   0 root         (0) root         (0)    25549 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClientConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     5371 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClientConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)    17324 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClientMan.cc
+-rw-rw-r--   0 root         (0) root         (0)     5101 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClientMan.hh
+-rw-rw-r--   0 root         (0) root         (0)     7117 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClientMsg.cc
+-rw-rw-r--   0 root         (0) root         (0)     3740 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClientMsg.hh
+-rw-rw-r--   0 root         (0) root         (0)     8243 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClustID.cc
+-rw-rw-r--   0 root         (0) root         (0)     3382 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsClustID.hh
+-rw-rw-r--   0 root         (0) root         (0)    77195 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsCluster.cc
+-rw-rw-r--   0 root         (0) root         (0)    10458 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsCluster.hh
+-rw-rw-r--   0 root         (0) root         (0)   109427 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)    12336 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)    49369 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsFinder.cc
+-rw-rw-r--   0 root         (0) root         (0)     6835 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsFinder.hh
+-rw-rw-r--   0 root         (0) root         (0)     5106 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsJob.cc
+-rw-rw-r--   0 root         (0) root         (0)     3058 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsJob.hh
+-rw-rw-r--   0 root         (0) root         (0)     8643 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsKey.cc
+-rw-rw-r--   0 root         (0) root         (0)     6829 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsKey.hh
+-rw-rw-r--   0 root         (0) root         (0)    10887 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsLogin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3223 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsLogin.hh
+-rw-rw-r--   0 root         (0) root         (0)     8263 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsManList.cc
+-rw-rw-r--   0 root         (0) root         (0)     3563 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsManList.hh
+-rw-rw-r--   0 root         (0) root         (0)     9115 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsManTree.cc
+-rw-rw-r--   0 root         (0) root         (0)     3708 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsManTree.hh
+-rw-rw-r--   0 root         (0) root         (0)    20171 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     4549 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    21971 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsMeter.cc
+-rw-rw-r--   0 root         (0) root         (0)     4787 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsMeter.hh
+-rw-rw-r--   0 root         (0) root         (0)     6578 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsNash.cc
+-rw-rw-r--   0 root         (0) root         (0)     3101 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsNash.hh
+-rw-rw-r--   0 root         (0) root         (0)    68022 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsNode.cc
+-rw-rw-r--   0 root         (0) root         (0)    11829 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsNode.hh
+-rw-rw-r--   0 root         (0) root         (0)     7875 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPList.cc
+-rw-rw-r--   0 root         (0) root         (0)     5436 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPList.hh
+-rw-rw-r--   0 root         (0) root         (0)    18983 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsParser.cc
+-rw-rw-r--   0 root         (0) root         (0)     4888 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsParser.hh
+-rw-rw-r--   0 root         (0) root         (0)     7886 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPerfMon.hh
+-rw-rw-r--   0 root         (0) root         (0)     6042 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPrepArgs.cc
+-rw-rw-r--   0 root         (0) root         (0)     3669 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPrepArgs.hh
+-rw-rw-r--   0 root         (0) root         (0)    18512 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPrepare.cc
+-rw-rw-r--   0 root         (0) root         (0)     4068 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsPrepare.hh
+-rw-rw-r--   0 root         (0) root         (0)    46734 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsProtocol.cc
+-rw-rw-r--   0 root         (0) root         (0)     5039 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsProtocol.hh
+-rw-rw-r--   0 root         (0) root         (0)     3945 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRRData.cc
+-rw-rw-r--   0 root         (0) root         (0)     4633 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRRData.hh
+-rw-rw-r--   0 root         (0) root         (0)    17719 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRRQ.cc
+-rw-rw-r--   0 root         (0) root         (0)     7590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRRQ.hh
+-rw-rw-r--   0 root         (0) root         (0)     5228 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRTable.cc
+-rw-rw-r--   0 root         (0) root         (0)     3076 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRTable.hh
+-rw-rw-r--   0 root         (0) root         (0)     9893 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRedirLocal.cc
+-rw-rw-r--   0 root         (0) root         (0)     3519 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRedirLocal.hh
+-rw-rw-r--   0 root         (0) root         (0)    11036 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsResp.cc
+-rw-rw-r--   0 root         (0) root         (0)     5382 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsResp.hh
+-rw-rw-r--   0 root         (0) root         (0)     5917 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRole.hh
+-rw-rw-r--   0 root         (0) root         (0)    11602 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRouting.cc
+-rw-rw-r--   0 root         (0) root         (0)     4838 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsRouting.hh
+-rw-rw-r--   0 root         (0) root         (0)    14804 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsSecurity.cc
+-rw-rw-r--   0 root         (0) root         (0)     3468 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsSecurity.hh
+-rw-rw-r--   0 root         (0) root         (0)     7463 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsSelect.hh
+-rw-rw-r--   0 root         (0) root         (0)    11542 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsState.cc
+-rw-rw-r--   0 root         (0) root         (0)     3997 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsState.hh
+-rw-rw-r--   0 root         (0) root         (0)     5187 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsSupervisor.cc
+-rw-rw-r--   0 root         (0) root         (0)     2750 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsSupervisor.hh
+-rw-rw-r--   0 root         (0) root         (0)     5637 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsTalk.cc
+-rw-rw-r--   0 root         (0) root         (0)     3034 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsTalk.hh
+-rw-rw-r--   0 root         (0) root         (0)     3426 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     2782 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsTypes.hh
+-rw-rw-r--   0 root         (0) root         (0)    11723 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     6365 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     5656 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCms/XrdCmsVnId.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.753075 xrootd-5.6.1/src/XrdCrypto/
+-rw-rw-r--   0 root         (0) root         (0)     4302 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoAux.cc
+-rw-rw-r--   0 root         (0) root         (0)     5058 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoAux.hh
+-rw-rw-r--   0 root         (0) root         (0)     7678 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoBasic.cc
+-rw-rw-r--   0 root         (0) root         (0)     3869 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoBasic.hh
+-rw-rw-r--   0 root         (0) root         (0)     7405 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoCipher.cc
+-rw-rw-r--   0 root         (0) root         (0)     4214 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoCipher.hh
+-rw-rw-r--   0 root         (0) root         (0)    17888 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoFactory.cc
+-rw-rw-r--   0 root         (0) root         (0)     9138 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoFactory.hh
+-rw-rw-r--   0 root         (0) root         (0)     3500 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoLite.cc
+-rw-rw-r--   0 root         (0) root         (0)     5355 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoLite.hh
+-rw-rw-r--   0 root         (0) root         (0)     8734 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoLite_bf32.cc
+-rw-rw-r--   0 root         (0) root         (0)     4136 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoMsgDigest.cc
+-rw-rw-r--   0 root         (0) root         (0)     3452 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoMsgDigest.hh
+-rw-rw-r--   0 root         (0) root         (0)     9058 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoRSA.cc
+-rw-rw-r--   0 root         (0) root         (0)     4804 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoRSA.hh
+-rw-rw-r--   0 root         (0) root         (0)     2994 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)    10639 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509.cc
+-rw-rw-r--   0 root         (0) root         (0)     5644 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509.hh
+-rw-rw-r--   0 root         (0) root         (0)    27273 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Chain.cc
+-rw-rw-r--   0 root         (0) root         (0)     7661 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Chain.hh
+-rw-rw-r--   0 root         (0) root         (0)     5674 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Crl.cc
+-rw-rw-r--   0 root         (0) root         (0)     4052 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Crl.hh
+-rw-rw-r--   0 root         (0) root         (0)     5256 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Req.cc
+-rw-rw-r--   0 root         (0) root         (0)     4177 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Req.hh
+-rw-rw-r--   0 root         (0) root         (0)    10162 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptogsiX509Chain.cc
+-rw-rw-r--   0 root         (0) root         (0)     3952 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptogsiX509Chain.hh
+-rw-rw-r--   0 root         (0) root         (0)    25131 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslAux.cc
+-rw-rw-r--   0 root         (0) root         (0)     7231 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslAux.hh
+-rw-rw-r--   0 root         (0) root         (0)    43961 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslCipher.cc
+-rw-rw-r--   0 root         (0) root         (0)     4814 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslCipher.hh
+-rw-rw-r--   0 root         (0) root         (0)    16817 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslFactory.cc
+-rw-rw-r--   0 root         (0) root         (0)     5208 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslFactory.hh
+-rw-rw-r--   0 root         (0) root         (0)     6084 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslMsgDigest.cc
+-rw-rw-r--   0 root         (0) root         (0)     3376 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslMsgDigest.hh
+-rw-rw-r--   0 root         (0) root         (0)    20952 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslRSA.cc
+-rw-rw-r--   0 root         (0) root         (0)     4241 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslRSA.hh
+-rw-rw-r--   0 root         (0) root         (0)     2901 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)    36214 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509.cc
+-rw-rw-r--   0 root         (0) root         (0)     5787 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509.hh
+-rw-rw-r--   0 root         (0) root         (0)    20566 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Crl.cc
+-rw-rw-r--   0 root         (0) root         (0)     5006 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Crl.hh
+-rw-rw-r--   0 root         (0) root         (0)    12043 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Req.cc
+-rw-rw-r--   0 root         (0) root         (0)     4113 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Req.hh
+-rw-rw-r--   0 root         (0) root         (0)    52085 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptosslgsiAux.cc
+-rw-rw-r--   0 root         (0) root         (0)    18878 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto/XrdCryptotest.cc
+-rw-rw-r--   0 root         (0) root         (0)     4042 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdCrypto.cmake
+-rw-rw-r--   0 root         (0) root         (0)     2904 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDaemons.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.753075 xrootd-5.6.1/src/XrdDig/
+-rw-rw-r--   0 root         (0) root         (0)    14689 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDig/XrdDigAuth.cc
+-rw-rw-r--   0 root         (0) root         (0)     4337 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDig/XrdDigAuth.hh
+-rw-rw-r--   0 root         (0) root         (0)    21474 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDig/XrdDigConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     3831 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDig/XrdDigConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)    28757 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDig/XrdDigFS.cc
+-rw-rw-r--   0 root         (0) root         (0)    11645 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdDig/XrdDigFS.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.753075 xrootd-5.6.1/src/XrdEc/
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     2020 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/README
+-rw-rw-r--   0 root         (0) root         (0)     3708 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     3424 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcObjCfg.hh
+-rw-rw-r--   0 root         (0) root         (0)    47577 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcReader.cc
+-rw-rw-r--   0 root         (0) root         (0)     8804 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcReader.hh
+-rw-rw-r--   0 root         (0) root         (0)     9779 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcRedundancyProvider.cc
+-rw-rw-r--   0 root         (0) root         (0)     5127 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcRedundancyProvider.hh
+-rw-rw-r--   0 root         (0) root         (0)    17345 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcStrmWriter.cc
+-rw-rw-r--   0 root         (0) root         (0)    13309 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcStrmWriter.hh
+-rw-rw-r--   0 root         (0) root         (0)     7256 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcThreadPool.hh
+-rw-rw-r--   0 root         (0) root         (0)     3689 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcUtilities.cc
+-rw-rw-r--   0 root         (0) root         (0)     9976 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcUtilities.hh
+-rw-rw-r--   0 root         (0) root         (0)    12505 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdEc/XrdEcWrtBuff.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.763075 xrootd-5.6.1/src/XrdFfs/
+-rw-rw-r--   0 root         (0) root         (0)     6405 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/README
+-rw-rw-r--   0 root         (0) root         (0)    10875 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsDent.cc
+-rw-rw-r--   0 root         (0) root         (0)     2975 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsDent.hh
+-rw-rw-r--   0 root         (0) root         (0)     5321 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsFsinfo.cc
+-rw-rw-r--   0 root         (0) root         (0)     2539 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsFsinfo.hh
+-rw-rw-r--   0 root         (0) root         (0)    13902 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsMisc.cc
+-rw-rw-r--   0 root         (0) root         (0)     3054 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsMisc.hh
+-rw-rw-r--   0 root         (0) root         (0)    26410 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsPosix.cc
+-rw-rw-r--   0 root         (0) root         (0)     4855 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsPosix.hh
+-rw-rw-r--   0 root         (0) root         (0)    10077 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsQueue.cc
+-rw-rw-r--   0 root         (0) root         (0)     2970 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsQueue.hh
+-rw-rw-r--   0 root         (0) root         (0)    11980 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsWcache.cc
+-rw-rw-r--   0 root         (0) root         (0)     2664 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsWcache.hh
+-rw-rw-r--   0 root         (0) root         (0)    48045 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/XrdFfsXrootdfs.cc
+-rwxrwxr-x   0 root         (0) root         (0)     1608 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs/xrootdfs.template
+-rw-rw-r--   0 root         (0) root         (0)     1905 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFfs.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.763075 xrootd-5.6.1/src/XrdFrc/
+-rw-rw-r--   0 root         (0) root         (0)    11084 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcCID.cc
+-rw-rw-r--   0 root         (0) root         (0)     3950 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcCID.hh
+-rw-rw-r--   0 root         (0) root         (0)    11618 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcProxy.cc
+-rw-rw-r--   0 root         (0) root         (0)     3742 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcProxy.hh
+-rw-rw-r--   0 root         (0) root         (0)     8762 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcReqAgent.cc
+-rw-rw-r--   0 root         (0) root         (0)     3073 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcReqAgent.hh
+-rw-rw-r--   0 root         (0) root         (0)    21187 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcReqFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     4017 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcReqFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     4547 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcRequest.hh
+-rw-rw-r--   0 root         (0) root         (0)     2728 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcTrace.cc
+-rw-rw-r--   0 root         (0) root         (0)     3411 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)    11388 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     3289 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     8162 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcXAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     2863 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrc/XrdFrcXLock.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.763075 xrootd-5.6.1/src/XrdFrm/
+-rw-rw-r--   0 root         (0) root         (0)    36149 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdmin.cc
+-rw-rw-r--   0 root         (0) root         (0)     7410 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdmin.hh
+-rw-rw-r--   0 root         (0) root         (0)    24369 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminAudit.cc
+-rw-rw-r--   0 root         (0) root         (0)    13623 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminFiles.cc
+-rw-rw-r--   0 root         (0) root         (0)    11144 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminFind.cc
+-rw-rw-r--   0 root         (0) root         (0)     6820 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminMain.cc
+-rw-rw-r--   0 root         (0) root         (0)    10240 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminQuery.cc
+-rw-rw-r--   0 root         (0) root         (0)     9903 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminReloc.cc
+-rw-rw-r--   0 root         (0) root         (0)     9421 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmAdminUnlink.cc
+-rw-rw-r--   0 root         (0) root         (0)    10117 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmCns.cc
+-rw-rw-r--   0 root         (0) root         (0)     3675 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmCns.hh
+-rw-rw-r--   0 root         (0) root         (0)    71617 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     8419 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)    17426 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmFiles.cc
+-rw-rw-r--   0 root         (0) root         (0)     6386 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmFiles.hh
+-rw-rw-r--   0 root         (0) root         (0)    11087 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmMigrate.cc
+-rw-rw-r--   0 root         (0) root         (0)     3078 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmMigrate.hh
+-rw-rw-r--   0 root         (0) root         (0)    11528 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmMonitor.cc
+-rw-rw-r--   0 root         (0) root         (0)     3912 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmMonitor.hh
+-rw-rw-r--   0 root         (0) root         (0)     9482 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmPurgMain.cc
+-rw-rw-r--   0 root         (0) root         (0)    32604 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmPurge.cc
+-rw-rw-r--   0 root         (0) root         (0)     5353 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmPurge.hh
+-rw-rw-r--   0 root         (0) root         (0)     7763 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmReqBoss.cc
+-rw-rw-r--   0 root         (0) root         (0)     3059 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmReqBoss.hh
+-rw-rw-r--   0 root         (0) root         (0)     7051 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmTSort.cc
+-rw-rw-r--   0 root         (0) root         (0)     3315 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmTSort.hh
+-rw-rw-r--   0 root         (0) root         (0)    30228 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmTransfer.cc
+-rw-rw-r--   0 root         (0) root         (0)     3349 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmTransfer.hh
+-rw-rw-r--   0 root         (0) root         (0)    10414 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrAgent.cc
+-rw-rw-r--   0 root         (0) root         (0)     3098 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrAgent.hh
+-rw-rw-r--   0 root         (0) root         (0)     7971 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrDaemon.cc
+-rw-rw-r--   0 root         (0) root         (0)     2782 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrDaemon.hh
+-rw-rw-r--   0 root         (0) root         (0)     2832 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrJob.hh
+-rw-rw-r--   0 root         (0) root         (0)     6343 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrMain.cc
+-rw-rw-r--   0 root         (0) root         (0)    17722 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrQueue.cc
+-rw-rw-r--   0 root         (0) root         (0)     4118 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm/XrdFrmXfrQueue.hh
+-rw-rw-r--   0 root         (0) root         (0)     3292 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdFrm.cmake
+-rw-rw-r--   0 root         (0) root         (0)     4663 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHeaders.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.773076 xrootd-5.6.1/src/XrdHttp/
+-rw-rw-r--   0 root         (0) root         (0)     1000 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/README-CKSUM.md
+-rw-rw-r--   0 root         (0) root         (0)     1909 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpChecksum.cc
+-rw-rw-r--   0 root         (0) root         (0)     2097 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpChecksum.hh
+-rw-rw-r--   0 root         (0) root         (0)     5702 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpChecksumHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpChecksumHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     3696 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpExtHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)     6073 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpExtHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     2306 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpModule.cc
+-rw-rw-r--   0 root         (0) root         (0)    86927 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpProtocol.cc
+-rw-rw-r--   0 root         (0) root         (0)    14055 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpProtocol.hh
+-rw-rw-r--   0 root         (0) root         (0)    89263 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpReq.cc
+-rw-rw-r--   0 root         (0) root         (0)    14529 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpReq.hh
+-rw-rw-r--   0 root         (0) root         (0)     4252 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpSecXtractor.hh
+-rw-rw-r--   0 root         (0) root         (0)     8841 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpSecurity.cc
+-rw-rw-r--   0 root         (0) root         (0)     1661 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpStatic.hh
+-rw-rw-r--   0 root         (0) root         (0)     2175 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     9423 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     2321 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/XrdHttpUtils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.773076 xrootd-5.6.1/src/XrdHttp/static/
+-rw-rw-r--   0 root         (0) root         (0)     1400 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/static/favicon.ico
+-rw-rw-r--   0 root         (0) root         (0)     1274 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/static/xrdhttp.css
+-rw-rw-r--   0 root         (0) root         (0)     7951 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/static/xrdhttp_css.h
+-rw-rw-r--   0 root         (0) root         (0)     8705 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/static/xrdhttp_favicon_ico.h
+-rw-rw-r--   0 root         (0) root         (0)     2784 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/xrootd-http-rdr.cf
+-rw-rw-r--   0 root         (0) root         (0)      941 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp/xrootd-http.cf
+-rw-rw-r--   0 root         (0) root         (0)     2494 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdHttp.cmake
+-rw-rw-r--   0 root         (0) root         (0)     1578 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdIsal.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.773076 xrootd-5.6.1/src/XrdMacaroons/
+-rw-rw-r--   0 root         (0) root         (0)     2798 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/README.md
+-rw-rw-r--   0 root         (0) root         (0)     4922 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/XrdMacaroons.cc
+-rw-rw-r--   0 root         (0) root         (0)    18196 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsAuthz.cc
+-rw-rw-r--   0 root         (0) root         (0)     1789 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsAuthz.hh
+-rw-rw-r--   0 root         (0) root         (0)     6883 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsConfigure.cc
+-rw-rw-r--   0 root         (0) root         (0)    21521 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsHandler.cc
+-rw-rw-r--   0 root         (0) root         (0)     2784 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)      122 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/export-lib-symbols
+-rwxrwxr-x   0 root         (0) root         (0)     5269 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons/macaroon-init
+-rw-rw-r--   0 root         (0) root         (0)     1631 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdMacaroons.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.773076 xrootd-5.6.1/src/XrdNet/
+-rw-rw-r--   0 root         (0) root         (0)    17923 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNet.cc
+-rw-rw-r--   0 root         (0) root         (0)    14669 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNet.hh
+-rw-rw-r--   0 root         (0) root         (0)    21048 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetAddr.cc
+-rw-rw-r--   0 root         (0) root         (0)    15050 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetAddr.hh
+-rw-rw-r--   0 root         (0) root         (0)    17812 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetAddrInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)    17695 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetAddrInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     5823 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetBuffer.cc
+-rw-rw-r--   0 root         (0) root         (0)     3948 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetBuffer.hh
+-rw-rw-r--   0 root         (0) root         (0)     8210 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetCache.cc
+-rw-rw-r--   0 root         (0) root         (0)     5934 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     5742 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetCmsNotify.cc
+-rw-rw-r--   0 root         (0) root         (0)     2929 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetCmsNotify.hh
+-rw-rw-r--   0 root         (0) root         (0)     4246 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetConnect.cc
+-rw-rw-r--   0 root         (0) root         (0)     3196 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetConnect.hh
+-rw-rw-r--   0 root         (0) root         (0)    31969 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetIF.cc
+-rw-rw-r--   0 root         (0) root         (0)    20067 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetIF.hh
+-rw-rw-r--   0 root         (0) root         (0)     6326 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetIdentity.cc
+-rw-rw-r--   0 root         (0) root         (0)     2701 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetIdentity.hh
+-rw-rw-r--   0 root         (0) root         (0)     7242 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetMsg.cc
+-rw-rw-r--   0 root         (0) root         (0)     7458 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetMsg.hh
+-rw-rw-r--   0 root         (0) root         (0)     4955 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetOpts.hh
+-rw-rw-r--   0 root         (0) root         (0)     3294 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPMark.cc
+-rw-rw-r--   0 root         (0) root         (0)     3824 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPMark.hh
+-rw-rw-r--   0 root         (0) root         (0)    39260 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPMarkCfg.cc
+-rw-rw-r--   0 root         (0) root         (0)     3755 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPMarkCfg.hh
+-rw-rw-r--   0 root         (0) root         (0)    13957 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPMarkFF.cc
+-rw-rw-r--   0 root         (0) root         (0)     3475 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPMarkFF.hh
+-rw-rw-r--   0 root         (0) root         (0)     2952 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetPeer.hh
+-rw-rw-r--   0 root         (0) root         (0)     9640 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetRegistry.cc
+-rw-rw-r--   0 root         (0) root         (0)     6279 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetRegistry.hh
+-rw-rw-r--   0 root         (0) root         (0)     9596 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetSecurity.cc
+-rw-rw-r--   0 root         (0) root         (0)     3339 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetSecurity.hh
+-rw-rw-r--   0 root         (0) root         (0)     3106 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetSockAddr.hh
+-rw-rw-r--   0 root         (0) root         (0)    18472 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetSocket.cc
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetSocket.hh
+-rw-rw-r--   0 root         (0) root         (0)    31024 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)    24210 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdNet/XrdNetUtils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.783076 xrootd-5.6.1/src/XrdOfs/
+-rw-rw-r--   0 root         (0) root         (0)    99020 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfs.cc
+-rw-rw-r--   0 root         (0) root         (0)    21611 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfs.hh
+-rw-rw-r--   0 root         (0) root         (0)    19274 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsCPFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     8379 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsCPFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    11781 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsChkPnt.cc
+-rw-rw-r--   0 root         (0) root         (0)     6193 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsChkPnt.hh
+-rw-rw-r--   0 root         (0) root         (0)    77647 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)    10806 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsConfigCP.cc
+-rw-rw-r--   0 root         (0) root         (0)     3117 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsConfigCP.hh
+-rw-rw-r--   0 root         (0) root         (0)    33128 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsConfigPI.cc
+-rw-rw-r--   0 root         (0) root         (0)    14532 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsConfigPI.hh
+-rw-rw-r--   0 root         (0) root         (0)    12955 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsEvr.cc
+-rw-rw-r--   0 root         (0) root         (0)     4771 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsEvr.hh
+-rw-rw-r--   0 root         (0) root         (0)    19534 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsEvs.cc
+-rw-rw-r--   0 root         (0) root         (0)     7231 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsEvs.hh
+-rw-rw-r--   0 root         (0) root         (0)    16520 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsFAttr.cc
+-rw-rw-r--   0 root         (0) root         (0)     4073 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsFS.cc
+-rw-rw-r--   0 root         (0) root         (0)    13054 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsFSctl.cc
+-rw-rw-r--   0 root         (0) root         (0)     8921 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsFSctl_PI.hh
+-rw-rw-r--   0 root         (0) root         (0)    30832 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsHandle.cc
+-rw-rw-r--   0 root         (0) root         (0)     8197 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsHandle.hh
+-rw-rw-r--   0 root         (0) root         (0)    13105 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsPoscq.cc
+-rw-rw-r--   0 root         (0) root         (0)     4134 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsPoscq.hh
+-rw-rw-r--   0 root         (0) root         (0)    30229 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsPrepGPI.cc
+-rw-rw-r--   0 root         (0) root         (0)    11518 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsPrepare.hh
+-rw-rw-r--   0 root         (0) root         (0)     3061 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsSecurity.hh
+-rw-rw-r--   0 root         (0) root         (0)     3814 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsStats.cc
+-rw-rw-r--   0 root         (0) root         (0)     3285 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsStats.hh
+-rw-rw-r--   0 root         (0) root         (0)    23543 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPC.cc
+-rw-rw-r--   0 root         (0) root         (0)     5117 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPC.hh
+-rw-rw-r--   0 root         (0) root         (0)    10359 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCAuth.cc
+-rw-rw-r--   0 root         (0) root         (0)     3086 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCAuth.hh
+-rw-rw-r--   0 root         (0) root         (0)     3108 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     7573 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)     5241 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     7941 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCJob.cc
+-rw-rw-r--   0 root         (0) root         (0)     3295 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCJob.hh
+-rw-rw-r--   0 root         (0) root         (0)    13429 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCProg.cc
+-rw-rw-r--   0 root         (0) root         (0)     3209 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTPCProg.hh
+-rw-rw-r--   0 root         (0) root         (0)     4158 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOfs/XrdOfsTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.783076 xrootd-5.6.1/src/XrdOss/
+-rw-rw-r--   0 root         (0) root         (0)    11649 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOss.cc
+-rw-rw-r--   0 root         (0) root         (0)    46028 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOss.hh
+-rw-rw-r--   0 root         (0) root         (0)    18122 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssAio.cc
+-rw-rw-r--   0 root         (0) root         (0)    45753 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssApi.cc
+-rw-rw-r--   0 root         (0) root         (0)    17573 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssApi.hh
+-rw-rw-r--   0 root         (0) root         (0)     8491 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssAt.cc
+-rw-rw-r--   0 root         (0) root         (0)     7394 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssAt.hh
+-rw-rw-r--   0 root         (0) root         (0)    31708 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssCache.cc
+-rw-rw-r--   0 root         (0) root         (0)    11024 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssCache.hh
+-rw-rw-r--   0 root         (0) root         (0)    73786 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     3327 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     7753 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssCopy.cc
+-rw-rw-r--   0 root         (0) root         (0)     2632 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssCopy.hh
+-rw-rw-r--   0 root         (0) root         (0)    13674 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssCreate.cc
+-rw-rw-r--   0 root         (0) root         (0)     3641 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssDefaultSS.hh
+-rw-rw-r--   0 root         (0) root         (0)     4810 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssError.hh
+-rw-rw-r--   0 root         (0) root         (0)    16583 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssMSS.cc
+-rw-rw-r--   0 root         (0) root         (0)    11917 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssMio.cc
+-rw-rw-r--   0 root         (0) root         (0)     3591 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssMio.hh
+-rw-rw-r--   0 root         (0) root         (0)     2931 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssMioFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     2987 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssOpaque.hh
+-rw-rw-r--   0 root         (0) root         (0)    13731 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssPath.cc
+-rw-rw-r--   0 root         (0) root         (0)     3880 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssPath.hh
+-rw-rw-r--   0 root         (0) root         (0)     8574 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssReloc.cc
+-rw-rw-r--   0 root         (0) root         (0)     9890 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssRename.cc
+-rw-rw-r--   0 root         (0) root         (0)     9051 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssSIgpfsT.cc
+-rw-rw-r--   0 root         (0) root         (0)    19495 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssSpace.cc
+-rw-rw-r--   0 root         (0) root         (0)     4240 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssSpace.hh
+-rw-rw-r--   0 root         (0) root         (0)    18820 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssStage.cc
+-rw-rw-r--   0 root         (0) root         (0)     4090 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssStage.hh
+-rw-rw-r--   0 root         (0) root         (0)    21165 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssStat.cc
+-rw-rw-r--   0 root         (0) root         (0)    10195 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssStatInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     3186 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     8528 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssUnlink.cc
+-rw-rw-r--   0 root         (0) root         (0)     6673 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssVS.hh
+-rw-rw-r--   0 root         (0) root         (0)    41503 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOss/XrdOssWrapper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.793076 xrootd-5.6.1/src/XrdOssCsi/
+-rw-rw-r--   0 root         (0) root         (0)     3167 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/README.md
+-rw-rw-r--   0 root         (0) root         (0)    15159 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsi.cc
+-rw-rw-r--   0 root         (0) root         (0)     9618 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsi.hh
+-rw-rw-r--   0 root         (0) root         (0)     7059 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     6756 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     2527 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiCrcUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     4781 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiCrcUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)    16745 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     4448 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiFileAio.cc
+-rw-rw-r--   0 root         (0) root         (0)    11301 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiFileAio.hh
+-rw-rw-r--   0 root         (0) root         (0)    29563 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiPages.cc
+-rw-rw-r--   0 root         (0) root         (0)     9019 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiPages.hh
+-rw-rw-r--   0 root         (0) root         (0)    34154 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc
+-rw-rw-r--   0 root         (0) root         (0)     3049 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiRanges.cc
+-rw-rw-r--   0 root         (0) root         (0)     6143 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiRanges.hh
+-rw-rw-r--   0 root         (0) root         (0)     3346 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTagstore.hh
+-rw-rw-r--   0 root         (0) root         (0)     8697 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     6892 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     3325 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)    10382 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi/XrdOssHandler.hh
+-rw-rw-r--   0 root         (0) root         (0)     1825 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOssCsi.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.803076 xrootd-5.6.1/src/XrdOuc/
+-rw-rw-r--   0 root         (0) root         (0)     1179 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/README.bonjour
+-rw-rw-r--   0 root         (0) root         (0)     8818 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucArgs.cc
+-rw-rw-r--   0 root         (0) root         (0)     5805 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucArgs.hh
+-rw-rw-r--   0 root         (0) root         (0)    17677 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucBackTrace.cc
+-rw-rw-r--   0 root         (0) root         (0)    10560 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucBackTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     9481 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucBuffer.cc
+-rw-rw-r--   0 root         (0) root         (0)    12583 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucBuffer.hh
+-rw-rw-r--   0 root         (0) root         (0)    12756 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCRC.cc
+-rw-rw-r--   0 root         (0) root         (0)     8087 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCRC.hh
+-rw-rw-r--   0 root         (0) root         (0)    17087 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCRC32C.cc
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCRC32C.hh
+-rw-rw-r--   0 root         (0) root         (0)     5325 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCache.cc
+-rw-rw-r--   0 root         (0) root         (0)    37680 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     5225 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCacheCM.hh
+-rw-rw-r--   0 root         (0) root         (0)     7071 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCacheStats.hh
+-rw-rw-r--   0 root         (0) root         (0)     4673 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCallBack.cc
+-rw-rw-r--   0 root         (0) root         (0)     5820 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCallBack.hh
+-rw-rw-r--   0 root         (0) root         (0)     3807 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucChain.hh
+-rw-rw-r--   0 root         (0) root         (0)     5655 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucChkPnt.hh
+-rw-rw-r--   0 root         (0) root         (0)     1514 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucCompiler.hh
+-rw-rw-r--   0 root         (0) root         (0)     5019 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucDLlist.hh
+-rw-rw-r--   0 root         (0) root         (0)     4334 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucERoute.cc
+-rw-rw-r--   0 root         (0) root         (0)     4301 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucERoute.hh
+-rw-rw-r--   0 root         (0) root         (0)     1693 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucEnum.hh
+-rw-rw-r--   0 root         (0) root         (0)     9097 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucEnv.cc
+-rw-rw-r--   0 root         (0) root         (0)     5341 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucEnv.hh
+-rw-rw-r--   0 root         (0) root         (0)    23619 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucErrInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)    10829 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucExport.cc
+-rw-rw-r--   0 root         (0) root         (0)     5760 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucExport.hh
+-rw-rw-r--   0 root         (0) root         (0)     9215 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucFileInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)     9566 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucFileInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)    11294 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucGMap.cc
+-rw-rw-r--   0 root         (0) root         (0)     8302 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucGMap.hh
+-rw-rw-r--   0 root         (0) root         (0)     8116 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucGatherConf.cc
+-rw-rw-r--   0 root         (0) root         (0)     6689 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucGatherConf.hh
+-rw-rw-r--   0 root         (0) root         (0)     9301 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucHash.hh
+-rw-rw-r--   0 root         (0) root         (0)    11511 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucHash.icc
+-rw-rw-r--   0 root         (0) root         (0)     3214 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucHashVal.cc
+-rw-rw-r--   0 root         (0) root         (0)     3665 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucIOVec.hh
+-rw-rw-r--   0 root         (0) root         (0)   978532 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucJson.hh
+-rw-rw-r--   0 root         (0) root         (0)     2676 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucLock.hh
+-rw-rw-r--   0 root         (0) root         (0)    10867 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucLogging.cc
+-rw-rw-r--   0 root         (0) root         (0)     3153 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucLogging.hh
+-rw-rw-r--   0 root         (0) root         (0)     4695 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucMapP2X.hh
+-rw-rw-r--   0 root         (0) root         (0)    10179 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucMsubs.cc
+-rw-rw-r--   0 root         (0) root         (0)     5592 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucMsubs.hh
+-rw-rw-r--   0 root         (0) root         (0)     4780 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucN2NLoader.cc
+-rw-rw-r--   0 root         (0) root         (0)     3053 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucN2NLoader.hh
+-rw-rw-r--   0 root         (0) root         (0)    10498 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucN2No2p.cc
+-rw-rw-r--   0 root         (0) root         (0)     5458 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucNList.cc
+-rw-rw-r--   0 root         (0) root         (0)     5100 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucNList.hh
+-rw-rw-r--   0 root         (0) root         (0)    14527 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucNSWalk.cc
+-rw-rw-r--   0 root         (0) root         (0)     7388 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucNSWalk.hh
+-rw-rw-r--   0 root         (0) root         (0)     8596 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucName2Name.cc
+-rw-rw-r--   0 root         (0) root         (0)    12097 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucName2Name.hh
+-rw-rw-r--   0 root         (0) root         (0)     6417 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPList.hh
+-rw-rw-r--   0 root         (0) root         (0)    12474 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPgrwUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     7990 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPgrwUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     6245 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPinKing.hh
+-rw-rw-r--   0 root         (0) root         (0)    10383 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPinLoader.cc
+-rw-rw-r--   0 root         (0) root         (0)     9351 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPinLoader.hh
+-rw-rw-r--   0 root         (0) root         (0)     3859 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPinObject.hh
+-rw-rw-r--   0 root         (0) root         (0)     2488 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPinPath.cc
+-rw-rw-r--   0 root         (0) root         (0)     3769 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPinPath.hh
+-rw-rw-r--   0 root         (0) root         (0)     3334 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPreload.cc
+-rw-rw-r--   0 root         (0) root         (0)     3993 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPreload.hh
+-rw-rw-r--   0 root         (0) root         (0)    12229 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucProg.cc
+-rw-rw-r--   0 root         (0) root         (0)     6185 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucProg.hh
+-rw-rw-r--   0 root         (0) root         (0)    30926 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPsx.cc
+-rw-rw-r--   0 root         (0) root         (0)     6045 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPsx.hh
+-rw-rw-r--   0 root         (0) root         (0)    13939 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPup.cc
+-rw-rw-r--   0 root         (0) root         (0)     8053 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucPup.hh
+-rw-rw-r--   0 root         (0) root         (0)     7879 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucRash.hh
+-rw-rw-r--   0 root         (0) root         (0)     9416 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucRash.icc
+-rw-rw-r--   0 root         (0) root         (0)     6087 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucReqID.cc
+-rw-rw-r--   0 root         (0) root         (0)     3008 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucReqID.hh
+-rw-rw-r--   0 root         (0) root         (0)     3219 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSFVec.hh
+-rw-rw-r--   0 root         (0) root         (0)     9442 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSHA3.cc
+-rw-rw-r--   0 root         (0) root         (0)     6968 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSHA3.hh
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSid.cc
+-rw-rw-r--   0 root         (0) root         (0)     6332 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSid.hh
+-rw-rw-r--   0 root         (0) root         (0)     2968 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSiteName.cc
+-rw-rw-r--   0 root         (0) root         (0)     2588 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSiteName.hh
+-rw-rw-r--   0 root         (0) root         (0)     3074 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucStats.hh
+-rw-rw-r--   0 root         (0) root         (0)    47408 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucStream.cc
+-rw-rw-r--   0 root         (0) root         (0)    11689 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucStream.hh
+-rw-rw-r--   0 root         (0) root         (0)    35618 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucString.cc
+-rw-rw-r--   0 root         (0) root         (0)    25276 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucString.hh
+-rw-rw-r--   0 root         (0) root         (0)     7049 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSxeq.cc
+-rw-rw-r--   0 root         (0) root         (0)     3039 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucSxeq.hh
+-rw-rw-r--   0 root         (0) root         (0)     5248 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTList.hh
+-rw-rw-r--   0 root         (0) root         (0)     9887 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTPC.cc
+-rw-rw-r--   0 root         (0) root         (0)     3801 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTPC.hh
+-rw-rw-r--   0 root         (0) root         (0)     3390 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     7032 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTable.hh
+-rw-rw-r--   0 root         (0) root         (0)     5093 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTokenizer.cc
+-rw-rw-r--   0 root         (0) root         (0)     3588 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTokenizer.hh
+-rw-rw-r--   0 root         (0) root         (0)     3019 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTrace.cc
+-rw-rw-r--   0 root         (0) root         (0)     2897 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     8152 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucUri.cc
+-rw-rw-r--   0 root         (0) root         (0)     4397 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucUri.hh
+-rw-rw-r--   0 root         (0) root         (0)    44495 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     5696 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     5319 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucVerName.cc
+-rw-rw-r--   0 root         (0) root         (0)     4226 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucVerName.hh
+-rw-rw-r--   0 root         (0) root         (0)     7043 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOucXAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)    15942 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOuca2x.cc
+-rw-rw-r--   0 root         (0) root         (0)     4130 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdOuc/XrdOuca2x.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.803076 xrootd-5.6.1/src/XrdPfc/
+-rw-rw-r--   0 root         (0) root         (0)     7215 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/README
+-rw-rw-r--   0 root         (0) root         (0)    29394 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfc.cc
+-rw-rw-r--   0 root         (0) root         (0)    18171 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfc.hh
+-rw-rw-r--   0 root         (0) root         (0)     1841 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcAllowDecision.cc
+-rw-rw-r--   0 root         (0) root         (0)     3643 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcBlacklistDecision.cc
+-rw-rw-r--   0 root         (0) root         (0)    12821 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcCommand.cc
+-rw-rw-r--   0 root         (0) root         (0)    27813 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcConfiguration.cc
+-rw-rw-r--   0 root         (0) root         (0)     2444 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcDecision.hh
+-rw-rw-r--   0 root         (0) root         (0)     6260 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcFSctl.cc
+-rw-rw-r--   0 root         (0) root         (0)     4186 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcFSctl.hh
+-rw-rw-r--   0 root         (0) root         (0)    46143 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcFile.cc
+-rw-rw-r--   0 root         (0) root         (0)    14635 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     1933 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcIO.cc
+-rw-rw-r--   0 root         (0) root         (0)     2691 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcIO.hh
+-rw-rw-r--   0 root         (0) root         (0)    11807 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcIOFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     3620 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcIOFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    12359 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcIOFileBlock.cc
+-rw-rw-r--   0 root         (0) root         (0)     2979 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcIOFileBlock.hh
+-rw-rw-r--   0 root         (0) root         (0)    19051 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)    18053 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)    12636 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcPrint.cc
+-rw-rw-r--   0 root         (0) root         (0)     2934 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcPrint.hh
+-rw-rw-r--   0 root         (0) root         (0)    32423 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcPurge.cc
+-rw-rw-r--   0 root         (0) root         (0)     4738 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcStats.hh
+-rw-rw-r--   0 root         (0) root         (0)     2079 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     1380 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc/XrdPfcTypes.hh
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPfc.cmake
+-rw-rw-r--   0 root         (0) root         (0)     4821 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPlugins.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdPosix/
+-rw-rw-r--   0 root         (0) root         (0)     7201 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/README
+-rw-rw-r--   0 root         (0) root         (0)    34309 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosix.cc
+-rw-rw-r--   0 root         (0) root         (0)     4656 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosix.hh
+-rw-rw-r--   0 root         (0) root         (0)     7780 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixAdmin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3383 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixAdmin.hh
+-rw-rw-r--   0 root         (0) root         (0)     5977 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixCache.cc
+-rw-rw-r--   0 root         (0) root         (0)     6942 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     2992 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixCallBack.cc
+-rw-rw-r--   0 root         (0) root         (0)     4732 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixCallBack.hh
+-rw-rw-r--   0 root         (0) root         (0)    23522 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     3483 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)     5169 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixDir.cc
+-rw-rw-r--   0 root         (0) root         (0)     4117 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixDir.hh
+-rw-rw-r--   0 root         (0) root         (0)     8592 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixExtern.hh
+-rw-rw-r--   0 root         (0) root         (0)     6173 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixExtra.cc
+-rw-rw-r--   0 root         (0) root         (0)     5480 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixExtra.hh
+-rw-rw-r--   0 root         (0) root         (0)    26695 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     8437 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     7869 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixFileRH.cc
+-rw-rw-r--   0 root         (0) root         (0)     4377 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixFileRH.hh
+-rw-rw-r--   0 root         (0) root         (0)     2994 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)    14943 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixLinkage.cc
+-rw-rw-r--   0 root         (0) root         (0)    14590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixLinkage.hh
+-rw-rw-r--   0 root         (0) root         (0)     8526 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixMap.cc
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixMap.hh
+-rw-rw-r--   0 root         (0) root         (0)     3041 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixObjGuard.hh
+-rw-rw-r--   0 root         (0) root         (0)    11702 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixObject.cc
+-rw-rw-r--   0 root         (0) root         (0)     4655 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixObject.hh
+-rw-rw-r--   0 root         (0) root         (0)     3600 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixOsDep.hh
+-rw-rw-r--   0 root         (0) root         (0)    24535 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixPreload.cc
+-rw-rw-r--   0 root         (0) root         (0)    19284 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixPreload32.cc
+-rw-rw-r--   0 root         (0) root         (0)     5301 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixPrepIO.cc
+-rw-rw-r--   0 root         (0) root         (0)     4774 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixPrepIO.hh
+-rw-rw-r--   0 root         (0) root         (0)     3366 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixStats.hh
+-rw-rw-r--   0 root         (0) root         (0)     2880 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)    53317 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixXrootd.cc
+-rw-rw-r--   0 root         (0) root         (0)    18316 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixXrootd.hh
+-rw-rw-r--   0 root         (0) root         (0)    11698 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixXrootdPath.cc
+-rw-rw-r--   0 root         (0) root         (0)     3595 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix/XrdPosixXrootdPath.hh
+-rw-rw-r--   0 root         (0) root         (0)     3071 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPosix.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdPss/
+-rw-rw-r--   0 root         (0) root         (0)    46084 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPss.cc
+-rw-rw-r--   0 root         (0) root         (0)     9367 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPss.hh
+-rw-rw-r--   0 root         (0) root         (0)     8543 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssAio.cc
+-rw-rw-r--   0 root         (0) root         (0)     5049 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssAioCB.cc
+-rw-rw-r--   0 root         (0) root         (0)     3188 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssAioCB.hh
+-rw-rw-r--   0 root         (0) root         (0)     8402 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssCks.cc
+-rw-rw-r--   0 root         (0) root         (0)     3733 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssCks.hh
+-rw-rw-r--   0 root         (0) root         (0)    31246 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     2807 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     8758 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssUrlInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)     3611 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssUrlInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     5115 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     3367 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdPss/XrdPssUtils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdRmc/
+-rw-rw-r--   0 root         (0) root         (0)     3076 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmc.cc
+-rw-rw-r--   0 root         (0) root         (0)     8248 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmc.hh
+-rw-rw-r--   0 root         (0) root         (0)    20610 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmcData.cc
+-rw-rw-r--   0 root         (0) root         (0)     5754 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmcData.hh
+-rw-rw-r--   0 root         (0) root         (0)    20813 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmcReal.cc
+-rw-rw-r--   0 root         (0) root         (0)     5594 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmcReal.hh
+-rw-rw-r--   0 root         (0) root         (0)     7041 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdRmc/XrdRmcSlot.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdSciTokens/
+-rw-rw-r--   0 root         (0) root         (0)    11357 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     8455 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/README.md
+-rw-rw-r--   0 root         (0) root         (0)    50104 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensAccess.cc
+-rw-rw-r--   0 root         (0) root         (0)     2985 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensHelper.hh
+-rw-rw-r--   0 root         (0) root         (0)     1378 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensMon.cc
+-rw-rw-r--   0 root         (0) root         (0)      966 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensMon.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdSciTokens/configs/
+-rw-rw-r--   0 root         (0) root         (0)       78 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/configs/export-lib-symbols
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/configs/export-module-symbols
+-rw-rw-r--   0 root         (0) root         (0)      945 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/configs/scitokens.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdSciTokens/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdSciTokens/test/config/
+-rw-rw-r--   0 root         (0) root         (0)       55 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/config/override.conf
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/config/scitokens-aud.cfg
+-rw-rw-r--   0 root         (0) root         (0)      115 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/config/scitokens-multi-aud.cfg
+-rw-rw-r--   0 root         (0) root         (0)       61 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/config/scitokens-no-aud.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1879 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/config/xrootd-http.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1598 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/create-pubkey.py
+-rw-rw-r--   0 root         (0) root         (0)      594 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/openssl-selfsigned.conf
+-rwxrwxr-x   0 root         (0) root         (0)      803 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/setup_tests.sh
+-rwxrwxr-x   0 root         (0) root         (0)     5083 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/test/test_inside_docker.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdSciTokens/vendor/
+-rw-rw-r--   0 root         (0) root         (0)      181 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/README.vendor
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.813076 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/
+-rw-rw-r--   0 root         (0) root         (0)       10 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)      113 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)    13507 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/INIReader.h
+-rw-rw-r--   0 root         (0) root         (0)     1088 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp
+-rw-rw-r--   0 root         (0) root         (0)     1510 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)     1574 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/README.md
+-rw-rw-r--   0 root         (0) root         (0)      416 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/inih/test.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/
+-rw-rw-r--   0 root         (0) root         (0)       97 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/.clang-format
+-rw-rw-r--   0 root         (0) root         (0)       35 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/.gitmodules
+-rw-rw-r--   0 root         (0) root         (0)       66 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)      903 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/Changes
+-rw-rw-r--   0 root         (0) root         (0)     1336 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     7016 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/README.mkdn
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/
+-rw-rw-r--   0 root         (0) root         (0)     3475 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc
+-rw-rw-r--   0 root         (0) root         (0)     2787 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/iostream.cc
+-rw-rw-r--   0 root         (0) root         (0)     2496 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/streaming.cc
+-rw-rw-r--   0 root         (0) root         (0)    33256 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picojson.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picotest/
+-rw-rw-r--   0 root         (0) root         (0)     2452 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picotest/picotest.c
+-rw-rw-r--   0 root         (0) root         (0)     1519 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picotest/picotest.h
+-rw-rw-r--   0 root         (0) root         (0)    12611 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/test.cc
+-rw-rw-r--   0 root         (0) root         (0)     1323 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSciTokens.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSec/
+-rw-rw-r--   0 root         (0) root         (0)     4540 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     5662 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecClient.cc
+-rw-rw-r--   0 root         (0) root         (0)     6062 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntity.cc
+-rw-rw-r--   0 root         (0) root         (0)     6849 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntity.hh
+-rw-rw-r--   0 root         (0) root         (0)     6459 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntityAttr.cc
+-rw-rw-r--   0 root         (0) root         (0)     8424 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntityAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     4638 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntityPin.hh
+-rw-rw-r--   0 root         (0) root         (0)     2945 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntityXtra.cc
+-rw-rw-r--   0 root         (0) root         (0)     2772 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecEntityXtra.hh
+-rw-rw-r--   0 root         (0) root         (0)    34779 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecInterface.hh
+-rw-rw-r--   0 root         (0) root         (0)    10669 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecLoadSecurity.cc
+-rw-rw-r--   0 root         (0) root         (0)     7822 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecLoadSecurity.hh
+-rw-rw-r--   0 root         (0) root         (0)     3233 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecMonitor.hh
+-rw-rw-r--   0 root         (0) root         (0)    15686 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecPManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     5056 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecPManager.hh
+-rw-rw-r--   0 root         (0) root         (0)    18129 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecProtect.cc
+-rw-rw-r--   0 root         (0) root         (0)     8540 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecProtect.hh
+-rw-rw-r--   0 root         (0) root         (0)    11790 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecProtector.cc
+-rw-rw-r--   0 root         (0) root         (0)     7608 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecProtector.hh
+-rw-rw-r--   0 root         (0) root         (0)     4849 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecProtocolhost.cc
+-rw-rw-r--   0 root         (0) root         (0)     3535 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecProtocolhost.hh
+-rw-rw-r--   0 root         (0) root         (0)    40467 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecServer.cc
+-rw-rw-r--   0 root         (0) root         (0)     5105 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecServer.hh
+-rw-rw-r--   0 root         (0) root         (0)    14327 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecTLayer.cc
+-rw-rw-r--   0 root         (0) root         (0)     7692 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecTLayer.hh
+-rw-rw-r--   0 root         (0) root         (0)     3076 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSecTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     7714 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSectestClient.cc
+-rw-rw-r--   0 root         (0) root         (0)    12099 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec/XrdSectestServer.cc
+-rw-rw-r--   0 root         (0) root         (0)     4574 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSec.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSecgsi/
+-rw-rw-r--   0 root         (0) root         (0)   199012 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecProtocolgsi.cc
+-rw-rw-r--   0 root         (0) root         (0)    25176 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecProtocolgsi.hh
+-rw-rw-r--   0 root         (0) root         (0)     6777 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc
+-rw-rw-r--   0 root         (0) root         (0)    11227 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc
+-rw-rw-r--   0 root         (0) root         (0)     8786 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc
+-rw-rw-r--   0 root         (0) root         (0)      669 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf
+-rw-rw-r--   0 root         (0) root         (0)     9513 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiOpts.hh
+-rw-rw-r--   0 root         (0) root         (0)    26709 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiProxy.cc
+-rw-rw-r--   0 root         (0) root         (0)     3028 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)    17329 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi/XrdSecgsitest.cc
+-rw-rw-r--   0 root         (0) root         (0)     3100 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecgsi.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSeckrb5/
+-rw-rw-r--   0 root         (0) root         (0)    38645 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSeckrb5/XrdSecProtocolkrb5.cc
+-rw-rw-r--   0 root         (0) root         (0)      759 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSeckrb5.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSecpwd/
+-rw-rw-r--   0 root         (0) root         (0)   129074 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecpwd/XrdSecProtocolpwd.cc
+-rw-rw-r--   0 root         (0) root         (0)    19042 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecpwd/XrdSecProtocolpwd.hh
+-rw-rw-r--   0 root         (0) root         (0)     2626 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecpwd/XrdSecpwdPlatform.hh
+-rw-rw-r--   0 root         (0) root         (0)    84590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3028 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecpwd/XrdSecpwdTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSecsss/
+-rw-rw-r--   0 root         (0) root         (0)    41443 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecProtocolsss.cc
+-rw-rw-r--   0 root         (0) root         (0)     6297 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecProtocolsss.hh
+-rw-rw-r--   0 root         (0) root         (0)    19394 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssAdmin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3559 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssCon.cc
+-rw-rw-r--   0 root         (0) root         (0)     4329 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssCon.hh
+-rw-rw-r--   0 root         (0) root         (0)    11806 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssEnt.cc
+-rw-rw-r--   0 root         (0) root         (0)     5290 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssEnt.hh
+-rw-rw-r--   0 root         (0) root         (0)     9560 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssID.cc
+-rw-rw-r--   0 root         (0) root         (0)     8505 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssID.hh
+-rw-rw-r--   0 root         (0) root         (0)    25232 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssKT.cc
+-rw-rw-r--   0 root         (0) root         (0)     5358 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssKT.hh
+-rw-rw-r--   0 root         (0) root         (0)     2704 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssMap.hh
+-rw-rw-r--   0 root         (0) root         (0)     5765 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecsss/XrdSecsssRR.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSecunix/
+-rw-rw-r--   0 root         (0) root         (0)     8595 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecunix/XrdSecProtocolunix.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.823076 xrootd-5.6.1/src/XrdSecztn/
+-rw-rw-r--   0 root         (0) root         (0)    29163 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecztn/XrdSecProtocolztn.cc
+-rw-rw-r--   0 root         (0) root         (0)     6814 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecztn/XrdSecztn.cc
+-rw-rw-r--   0 root         (0) root         (0)      669 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSecztn.cmake
+-rw-rw-r--   0 root         (0) root         (0)    10685 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdServer.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.833076 xrootd-5.6.1/src/XrdSfs/
+-rw-rw-r--   0 root         (0) root         (0)     3999 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsAio.hh
+-rw-rw-r--   0 root         (0) root         (0)     5824 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsDio.hh
+-rw-rw-r--   0 root         (0) root         (0)     5455 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsFAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     5100 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsFlags.hh
+-rw-rw-r--   0 root         (0) root         (0)     5619 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsGPFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    12634 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsInterface.cc
+-rw-rw-r--   0 root         (0) root         (0)    67321 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsInterface.hh
+-rw-rw-r--   0 root         (0) root         (0)    38665 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsNative.cc
+-rw-rw-r--   0 root         (0) root         (0)    10785 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsNative.hh
+-rw-rw-r--   0 root         (0) root         (0)     3537 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsXio.cc
+-rw-rw-r--   0 root         (0) root         (0)     7187 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsXio.hh
+-rw-rw-r--   0 root         (0) root         (0)     4432 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSfs/XrdSfsXioImpl.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.833076 xrootd-5.6.1/src/XrdSsi/
+-rw-rw-r--   0 root         (0) root         (0)     6178 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiAlert.cc
+-rw-rw-r--   0 root         (0) root         (0)     3366 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiAlert.hh
+-rw-rw-r--   0 root         (0) root         (0)     2661 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiAtomics.cc
+-rw-rw-r--   0 root         (0) root         (0)     7958 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiAtomics.hh
+-rw-rw-r--   0 root         (0) root         (0)     3132 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiBVec.hh
+-rw-rw-r--   0 root         (0) root         (0)    14419 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiClient.cc
+-rw-rw-r--   0 root         (0) root         (0)     7934 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiCluster.hh
+-rw-rw-r--   0 root         (0) root         (0)     4735 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiCms.cc
+-rw-rw-r--   0 root         (0) root         (0)     3752 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiCms.hh
+-rw-rw-r--   0 root         (0) root         (0)     7049 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiDir.cc
+-rw-rw-r--   0 root         (0) root         (0)     3177 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiDir.hh
+-rw-rw-r--   0 root         (0) root         (0)     4087 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiEntity.hh
+-rw-rw-r--   0 root         (0) root         (0)     2663 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiErrInfo.cc
+-rw-rw-r--   0 root         (0) root         (0)     6519 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiErrInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     7117 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiEvent.cc
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiEvent.hh
+-rw-rw-r--   0 root         (0) root         (0)    18166 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     5424 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    35655 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFileReq.cc
+-rw-rw-r--   0 root         (0) root         (0)     6776 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFileReq.hh
+-rw-rw-r--   0 root         (0) root         (0)     3711 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFileResource.cc
+-rw-rw-r--   0 root         (0) root         (0)     2797 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFileResource.hh
+-rw-rw-r--   0 root         (0) root         (0)    26232 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFileSess.cc
+-rw-rw-r--   0 root         (0) root         (0)     6023 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiFileSess.hh
+-rw-rw-r--   0 root         (0) root         (0)     7891 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiLogger.cc
+-rw-rw-r--   0 root         (0) root         (0)     8754 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiLogger.hh
+-rw-rw-r--   0 root         (0) root         (0)     6565 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiLogging.cc
+-rw-rw-r--   0 root         (0) root         (0)    17533 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiProvider.hh
+-rw-rw-r--   0 root         (0) root         (0)     3962 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiRRAgent.hh
+-rw-rw-r--   0 root         (0) root         (0)     4545 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiRRInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     4295 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiRRTable.hh
+-rw-rw-r--   0 root         (0) root         (0)     8144 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiRequest.cc
+-rw-rw-r--   0 root         (0) root         (0)    15740 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiRequest.hh
+-rw-rw-r--   0 root         (0) root         (0)     5790 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiResource.hh
+-rw-rw-r--   0 root         (0) root         (0)     7000 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiRespInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)    12144 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiResponder.cc
+-rw-rw-r--   0 root         (0) root         (0)    13431 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiResponder.hh
+-rw-rw-r--   0 root         (0) root         (0)     8986 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiScale.cc
+-rw-rw-r--   0 root         (0) root         (0)     3515 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiScale.hh
+-rw-rw-r--   0 root         (0) root         (0)    12168 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiServReal.cc
+-rw-rw-r--   0 root         (0) root         (0)     3574 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiServReal.hh
+-rw-rw-r--   0 root         (0) root         (0)     3281 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiService.cc
+-rw-rw-r--   0 root         (0) root         (0)     9866 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiService.hh
+-rw-rw-r--   0 root         (0) root         (0)    17845 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiSessReal.cc
+-rw-rw-r--   0 root         (0) root         (0)     4784 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiSessReal.hh
+-rw-rw-r--   0 root         (0) root         (0)    20137 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiSfs.cc
+-rw-rw-r--   0 root         (0) root         (0)     7069 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiSfs.hh
+-rw-rw-r--   0 root         (0) root         (0)    25133 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiSfsConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)     3556 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiSfsConfig.hh
+-rw-rw-r--   0 root         (0) root         (0)    45566 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiShMam.cc
+-rw-rw-r--   0 root         (0) root         (0)     5508 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiShMam.hh
+-rw-rw-r--   0 root         (0) root         (0)    22363 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiShMap.hh
+-rw-rw-r--   0 root         (0) root         (0)    12380 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiShMap.icc
+-rw-rw-r--   0 root         (0) root         (0)     3048 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiShMat.cc
+-rw-rw-r--   0 root         (0) root         (0)    19625 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiShMat.hh
+-rw-rw-r--   0 root         (0) root         (0)     6168 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiStat.cc
+-rw-rw-r--   0 root         (0) root         (0)     6883 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiStats.cc
+-rw-rw-r--   0 root         (0) root         (0)     4527 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiStats.hh
+-rw-rw-r--   0 root         (0) root         (0)     8580 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiStream.hh
+-rw-rw-r--   0 root         (0) root         (0)    24852 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiTaskReal.cc
+-rw-rw-r--   0 root         (0) root         (0)     4845 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiTaskReal.hh
+-rw-rw-r--   0 root         (0) root         (0)     2865 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     9000 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     3203 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi/XrdSsiUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     4630 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSsi.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.843076 xrootd-5.6.1/src/XrdSut/
+-rw-rw-r--   0 root         (0) root         (0)    22228 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutAux.cc
+-rw-rw-r--   0 root         (0) root         (0)    15145 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutAux.hh
+-rw-rw-r--   0 root         (0) root         (0)     5926 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutBuckList.cc
+-rw-rw-r--   0 root         (0) root         (0)     3963 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutBuckList.hh
+-rw-rw-r--   0 root         (0) root         (0)     8236 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutBucket.cc
+-rw-rw-r--   0 root         (0) root         (0)     3458 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutBucket.hh
+-rw-rw-r--   0 root         (0) root         (0)    16296 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutBuffer.cc
+-rw-rw-r--   0 root         (0) root         (0)     4872 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutBuffer.hh
+-rw-rw-r--   0 root         (0) root         (0)     6430 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     5618 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutCacheEntry.cc
+-rw-rw-r--   0 root         (0) root         (0)     5456 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutCacheEntry.hh
+-rw-rw-r--   0 root         (0) root         (0)    21841 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutPFCache.cc
+-rw-rw-r--   0 root         (0) root         (0)     5757 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutPFCache.hh
+-rw-rw-r--   0 root         (0) root         (0)     5549 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutPFEntry.cc
+-rw-rw-r--   0 root         (0) root         (0)     4790 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutPFEntry.hh
+-rw-rw-r--   0 root         (0) root         (0)    64583 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutPFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     7738 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutPFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     8759 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutRndm.cc
+-rw-rw-r--   0 root         (0) root         (0)     3293 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutRndm.hh
+-rw-rw-r--   0 root         (0) root         (0)     2941 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSut/XrdSutTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.843076 xrootd-5.6.1/src/XrdSys/
+-rw-rw-r--   0 root         (0) root         (0)     5249 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysAtomics.hh
+-rw-rw-r--   0 root         (0) root         (0)     4979 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysDir.cc
+-rw-rw-r--   0 root         (0) root         (0)     3341 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysDir.hh
+-rw-rw-r--   0 root         (0) root         (0)     4872 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysE2T.cc
+-rw-rw-r--   0 root         (0) root         (0)     2750 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysE2T.hh
+-rw-rw-r--   0 root         (0) root         (0)     8484 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysError.cc
+-rw-rw-r--   0 root         (0) root         (0)     7359 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysError.hh
+-rw-rw-r--   0 root         (0) root         (0)     6923 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFAttr.cc
+-rw-rw-r--   0 root         (0) root         (0)     4996 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     7106 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFAttrBsd.icc
+-rw-rw-r--   0 root         (0) root         (0)     6632 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFAttrLnx.icc
+-rw-rw-r--   0 root         (0) root         (0)     6063 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFAttrMac.icc
+-rw-rw-r--   0 root         (0) root         (0)     7705 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFAttrSun.icc
+-rw-rw-r--   0 root         (0) root         (0)     7575 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFD.hh
+-rw-rw-r--   0 root         (0) root         (0)     4783 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFallocate.cc
+-rw-rw-r--   0 root         (0) root         (0)     1578 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysFallocate.hh
+-rw-rw-r--   0 root         (0) root         (0)     2714 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysHeaders.hh
+-rw-rw-r--   0 root         (0) root         (0)    43303 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysIOEvents.cc
+-rw-rw-r--   0 root         (0) root         (0)    26713 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysIOEvents.hh
+-rw-rw-r--   0 root         (0) root         (0)    16052 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollE.icc
+-rw-rw-r--   0 root         (0) root         (0)    17045 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollKQ.icc
+-rw-rw-r--   0 root         (0) root         (0)    18706 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollPoll.icc
+-rw-rw-r--   0 root         (0) root         (0)    14975 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollPort.icc
+-rw-rw-r--   0 root         (0) root         (0)    16419 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysKernelBuffer.hh
+-rw-rw-r--   0 root         (0) root         (0)     5437 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysLogPI.hh
+-rw-rw-r--   0 root         (0) root         (0)    26559 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysLogger.cc
+-rw-rw-r--   0 root         (0) root         (0)    11736 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysLogger.hh
+-rw-rw-r--   0 root         (0) root         (0)    12120 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysLogging.cc
+-rw-rw-r--   0 root         (0) root         (0)     5811 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysLogging.hh
+-rw-rw-r--   0 root         (0) root         (0)     2511 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPageSize.hh
+-rw-rw-r--   0 root         (0) root         (0)     3233 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPlatform.cc
+-rw-rw-r--   0 root         (0) root         (0)     7952 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPlatform.hh
+-rw-rw-r--   0 root         (0) root         (0)    17849 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPlugin.cc
+-rw-rw-r--   0 root         (0) root         (0)    13621 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPlugin.hh
+-rw-rw-r--   0 root         (0) root         (0)    13000 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPriv.cc
+-rw-rw-r--   0 root         (0) root         (0)     4228 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPriv.hh
+-rw-rw-r--   0 root         (0) root         (0)    13657 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPthread.cc
+-rw-rw-r--   0 root         (0) root         (0)    19521 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPthread.hh
+-rw-rw-r--   0 root         (0) root         (0)     3245 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysPwd.hh
+-rw-rw-r--   0 root         (0) root         (0)    11994 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysRAtomic.hh
+-rw-rw-r--   0 root         (0) root         (0)     3952 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysSemWait.hh
+-rw-rw-r--   0 root         (0) root         (0)     6054 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysShmem.hh
+-rw-rw-r--   0 root         (0) root         (0)     9460 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysTimer.cc
+-rw-rw-r--   0 root         (0) root         (0)     3814 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysTimer.hh
+-rw-rw-r--   0 root         (0) root         (0)    15639 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysTrace.cc
+-rw-rw-r--   0 root         (0) root         (0)     4739 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     8298 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysUtils.cc
+-rw-rw-r--   0 root         (0) root         (0)     4798 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     4735 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysXAttr.cc
+-rw-rw-r--   0 root         (0) root         (0)    15063 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysXAttr.hh
+-rw-rw-r--   0 root         (0) root         (0)     5708 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysXSLock.cc
+-rw-rw-r--   0 root         (0) root         (0)     3311 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdSys/XrdSysXSLock.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.843076 xrootd-5.6.1/src/XrdThrottle/
+-rw-rw-r--   0 root         (0) root         (0)     3577 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/README
+-rw-rw-r--   0 root         (0) root         (0)     7487 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottle.hh
+-rw-rw-r--   0 root         (0) root         (0)     6658 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottleFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     5731 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottleFileSystem.cc
+-rw-rw-r--   0 root         (0) root         (0)    12897 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottleFileSystemConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)    18594 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottleManager.cc
+-rw-rw-r--   0 root         (0) root         (0)     5403 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottleManager.hh
+-rw-rw-r--   0 root         (0) root         (0)      879 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdThrottle/XrdThrottleTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.853076 xrootd-5.6.1/src/XrdTls/
+-rw-rw-r--   0 root         (0) root         (0)    10417 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTls.cc
+-rw-rw-r--   0 root         (0) root         (0)     6921 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTls.hh
+-rw-rw-r--   0 root         (0) root         (0)    37752 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsContext.cc
+-rw-rw-r--   0 root         (0) root         (0)    14507 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsContext.hh
+-rw-rw-r--   0 root         (0) root         (0)     1259 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsHostcheck.hh
+-rw-rw-r--   0 root         (0) root         (0)     6628 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsHostcheck.icc
+-rw-rw-r--   0 root         (0) root         (0)     5275 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsNotary.cc
+-rw-rw-r--   0 root         (0) root         (0)     5222 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsNotary.hh
+-rw-rw-r--   0 root         (0) root         (0)     2251 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsNotaryUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     7142 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsNotaryUtils.icc
+-rw-rw-r--   0 root         (0) root         (0)     3969 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsPeerCerts.cc
+-rw-rw-r--   0 root         (0) root         (0)     4951 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsPeerCerts.hh
+-rw-rw-r--   0 root         (0) root         (0)    33590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsSocket.cc
+-rw-rw-r--   0 root         (0) root         (0)    11845 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsSocket.hh
+-rw-rw-r--   0 root         (0) root         (0)    16122 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsTempCA.cc
+-rw-rw-r--   0 root         (0) root         (0)     5462 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsTempCA.hh
+-rw-rw-r--   0 root         (0) root         (0)     3201 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTls/XrdTlsTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.853076 xrootd-5.6.1/src/XrdTpc/
+-rw-rw-r--   0 root         (0) root         (0)     4032 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/README.md
+-rw-rw-r--   0 root         (0) root         (0)     5387 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcConfigure.cc
+-rw-rw-r--   0 root         (0) root         (0)     1663 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcCurlMulti.cc
+-rw-rw-r--   0 root         (0) root         (0)      144 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcCurlMulti.hh
+-rw-rw-r--   0 root         (0) root         (0)    19456 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcMultistream.cc
+-rw-rw-r--   0 root         (0) root         (0)    10532 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcState.cc
+-rw-rw-r--   0 root         (0) root         (0)     5794 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcState.hh
+-rw-rw-r--   0 root         (0) root         (0)     7210 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcStream.cc
+-rw-rw-r--   0 root         (0) root         (0)     5499 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcStream.hh
+-rw-rw-r--   0 root         (0) root         (0)    44035 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcTPC.cc
+-rw-rw-r--   0 root         (0) root         (0)     5994 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/XrdTpcTPC.hh
+-rw-rw-r--   0 root         (0) root         (0)       51 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/export-lib-symbols
+-rwxrwxr-x   0 root         (0) root         (0)     3709 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc/xrootd-test-tpc
+-rw-rw-r--   0 root         (0) root         (0)     2282 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdTpc.cmake
+-rw-rw-r--   0 root         (0) root         (0)    14578 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdUtils.cmake
+-rw-rw-r--   0 root         (0) root         (0)     5084 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVersion.hh.in
+-rw-rw-r--   0 root         (0) root         (0)    15666 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVersionPlugin.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.853076 xrootd-5.6.1/src/XrdVoms/
+-rw-rw-r--   0 root         (0) root         (0)     2917 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/README.md
+-rw-rw-r--   0 root         (0) root         (0)     2590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVoms.hh
+-rw-rw-r--   0 root         (0) root         (0)    22190 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsFun.cc
+-rw-rw-r--   0 root         (0) root         (0)     3835 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsFun.hh
+-rw-rw-r--   0 root         (0) root         (0)     6174 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsHttp.cc
+-rw-rw-r--   0 root         (0) root         (0)    15233 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsMapfile.cc
+-rw-rw-r--   0 root         (0) root         (0)     4249 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsMapfile.hh
+-rw-rw-r--   0 root         (0) root         (0)     2691 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     4105 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms/XrdVomsgsi.cc
+-rw-rw-r--   0 root         (0) root         (0)     1798 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdVoms.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.853076 xrootd-5.6.1/src/XrdXml/
+-rw-rw-r--   0 root         (0) root         (0)    18501 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlMetaLink.cc
+-rw-rw-r--   0 root         (0) root         (0)     9497 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlMetaLink.hh
+-rw-rw-r--   0 root         (0) root         (0)    10670 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlRdrTiny.cc
+-rw-rw-r--   0 root         (0) root         (0)     3590 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlRdrTiny.hh
+-rw-rw-r--   0 root         (0) root         (0)    11751 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlRdrXml2.cc
+-rw-rw-r--   0 root         (0) root         (0)     3585 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlRdrXml2.hh
+-rw-rw-r--   0 root         (0) root         (0)     4195 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlReader.cc
+-rw-rw-r--   0 root         (0) root         (0)     9010 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/XrdXmlReader.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.853076 xrootd-5.6.1/src/XrdXml/tinyxml/
+-rw-rw-r--   0 root         (0) root         (0)     2507 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/tinyxml/tinystr.cpp
+-rw-rw-r--   0 root         (0) root         (0)     8197 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/tinyxml/tinystr.h
+-rw-rw-r--   0 root         (0) root         (0)    37588 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/tinyxml/tinyxml.cpp
+-rw-rw-r--   0 root         (0) root         (0)    64835 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/tinyxml/tinyxml.h
+-rw-rw-r--   0 root         (0) root         (0)     1791 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/tinyxml/tinyxmlerror.cpp
+-rw-rw-r--   0 root         (0) root         (0)    37439 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml/tinyxml/tinyxmlparser.cpp
+-rw-rw-r--   0 root         (0) root         (0)     2148 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXml.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/src/XrdXrootd/
+-rw-rw-r--   0 root         (0) root         (0)    21688 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAdmin.cc
+-rw-rw-r--   0 root         (0) root         (0)     3927 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAdmin.hh
+-rw-rw-r--   0 root         (0) root         (0)     6106 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioBuff.cc
+-rw-rw-r--   0 root         (0) root         (0)     3396 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioBuff.hh
+-rw-rw-r--   0 root         (0) root         (0)     6164 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioFob.cc
+-rw-rw-r--   0 root         (0) root         (0)     3140 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioFob.hh
+-rw-rw-r--   0 root         (0) root         (0)    10852 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioPgrw.cc
+-rw-rw-r--   0 root         (0) root         (0)     4017 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioPgrw.hh
+-rw-rw-r--   0 root         (0) root         (0)    16842 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioTask.cc
+-rw-rw-r--   0 root         (0) root         (0)     5932 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioTask.hh
+-rw-rw-r--   0 root         (0) root         (0)     3257 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdBridge.cc
+-rw-rw-r--   0 root         (0) root         (0)    25502 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdBridge.hh
+-rw-rw-r--   0 root         (0) root         (0)    17339 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdCallBack.cc
+-rw-rw-r--   0 root         (0) root         (0)     3955 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdCallBack.hh
+-rw-rw-r--   0 root         (0) root         (0)    71797 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdConfig.cc
+-rw-rw-r--   0 root         (0) root         (0)    25761 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdConfigMon.cc
+-rw-rw-r--   0 root         (0) root         (0)    14829 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     8211 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdFile.hh
+-rw-rw-r--   0 root         (0) root         (0)     2629 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileLock.hh
+-rw-rw-r--   0 root         (0) root         (0)     6072 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileLock1.cc
+-rw-rw-r--   0 root         (0) root         (0)     2959 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileLock1.hh
+-rw-rw-r--   0 root         (0) root         (0)     7522 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileStats.hh
+-rw-rw-r--   0 root         (0) root         (0)    10638 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdGPFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    19666 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdGSReal.cc
+-rw-rw-r--   0 root         (0) root         (0)     6593 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdGSReal.hh
+-rw-rw-r--   0 root         (0) root         (0)     5076 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdGStream.cc
+-rw-rw-r--   0 root         (0) root         (0)     8514 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdGStream.hh
+-rw-rw-r--   0 root         (0) root         (0)    26130 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdJob.cc
+-rw-rw-r--   0 root         (0) root         (0)     4224 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdJob.hh
+-rw-rw-r--   0 root         (0) root         (0)     3858 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdLoadLib.cc
+-rw-rw-r--   0 root         (0) root         (0)    14128 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonData.hh
+-rw-rw-r--   0 root         (0) root         (0)     5374 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFMap.cc
+-rw-rw-r--   0 root         (0) root         (0)     3118 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFMap.hh
+-rw-rw-r--   0 root         (0) root         (0)    18282 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFile.cc
+-rw-rw-r--   0 root         (0) root         (0)     4376 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFile.hh
+-rw-rw-r--   0 root         (0) root         (0)    43427 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonitor.cc
+-rw-rw-r--   0 root         (0) root         (0)    12226 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonitor.hh
+-rw-rw-r--   0 root         (0) root         (0)    17436 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdNormAio.cc
+-rw-rw-r--   0 root         (0) root         (0)     3758 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdNormAio.hh
+-rw-rw-r--   0 root         (0) root         (0)    19524 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgrwAio.cc
+-rw-rw-r--   0 root         (0) root         (0)     3708 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgrwAio.hh
+-rw-rw-r--   0 root         (0) root         (0)     4934 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwBadCS.cc
+-rw-rw-r--   0 root         (0) root         (0)     2979 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwBadCS.hh
+-rw-rw-r--   0 root         (0) root         (0)     7262 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwCtl.cc
+-rw-rw-r--   0 root         (0) root         (0)     4842 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwCtl.hh
+-rw-rw-r--   0 root         (0) root         (0)     4520 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwFob.cc
+-rw-rw-r--   0 root         (0) root         (0)     4321 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwFob.hh
+-rw-rw-r--   0 root         (0) root         (0)     3973 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPio.cc
+-rw-rw-r--   0 root         (0) root         (0)     3751 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPio.hh
+-rw-rw-r--   0 root         (0) root         (0)     4685 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPlugin.cc
+-rw-rw-r--   0 root         (0) root         (0)    12615 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPrepare.cc
+-rw-rw-r--   0 root         (0) root         (0)     4956 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdPrepare.hh
+-rw-rw-r--   0 root         (0) root         (0)    53955 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdProtocol.cc
+-rw-rw-r--   0 root         (0) root         (0)    24030 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdProtocol.hh
+-rw-rw-r--   0 root         (0) root         (0)     3955 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdReqID.hh
+-rw-rw-r--   0 root         (0) root         (0)    17733 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdResponse.cc
+-rw-rw-r--   0 root         (0) root         (0)     5450 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdResponse.hh
+-rw-rw-r--   0 root         (0) root         (0)     7898 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdStats.cc
+-rw-rw-r--   0 root         (0) root         (0)     4653 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdStats.hh
+-rw-rw-r--   0 root         (0) root         (0)     6457 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTpcMon.cc
+-rw-rw-r--   0 root         (0) root         (0)     4899 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTpcMon.hh
+-rw-rw-r--   0 root         (0) root         (0)     3605 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTrace.hh
+-rw-rw-r--   0 root         (0) root         (0)     4806 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransPend.cc
+-rw-rw-r--   0 root         (0) root         (0)     3394 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransPend.hh
+-rw-rw-r--   0 root         (0) root         (0)     3978 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransSend.cc
+-rw-rw-r--   0 root         (0) root         (0)     3662 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransSend.hh
+-rw-rw-r--   0 root         (0) root         (0)    27246 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransit.cc
+-rw-rw-r--   0 root         (0) root         (0)     9705 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransit.hh
+-rw-rw-r--   0 root         (0) root         (0)     2783 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdWVInfo.hh
+-rw-rw-r--   0 root         (0) root         (0)     5092 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdXPath.hh
+-rw-rw-r--   0 root         (0) root         (0)   148794 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeq.cc
+-rw-rw-r--   0 root         (0) root         (0)     3317 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeq.hh
+-rw-rw-r--   0 root         (0) root         (0)    12437 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeqChkPnt.cc
+-rw-rw-r--   0 root         (0) root         (0)    20041 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeqFAttr.cc
+-rw-rw-r--   0 root         (0) root         (0)    22344 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeqPgrw.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/src/XrdZip/
+-rw-rw-r--   0 root         (0) root         (0)    14675 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipCDFH.hh
+-rw-rw-r--   0 root         (0) root         (0)     1960 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipDataDescriptor.hh
+-rw-rw-r--   0 root         (0) root         (0)     6301 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipEOCD.hh
+-rw-rw-r--   0 root         (0) root         (0)     6223 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipExtra.hh
+-rw-rw-r--   0 root         (0) root         (0)     7291 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipLFH.hh
+-rw-rw-r--   0 root         (0) root         (0)     6734 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipUtils.hh
+-rw-rw-r--   0 root         (0) root         (0)     5265 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipZIP64EOCD.hh
+-rw-rw-r--   0 root         (0) root         (0)     3227 2023-07-11 08:55:00.000000 xrootd-5.6.1/src/XrdZip/XrdZipZIP64EOCDL.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)      315 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XRootD/
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XRootD/CMakeLists.txt
+-rwxrwxr-x   0 root         (0) root         (0)     3065 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XRootD/smoke.sh
+-rw-rw-r--   0 root         (0) root         (0)      310 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XRootD/xrootd.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdCephTests/
+-rw-rw-r--   0 root         (0) root         (0)      553 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdCephTests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     6661 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdCephTests/CephParsingTest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdCl/
+-rw-rw-r--   0 root         (0) root         (0)      289 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdCl/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     5351 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdCl/XrdClURL.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.663075 xrootd-5.6.1/tests/XrdClHttp/cases/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/cases/000-simple-download/
+-rw-rw-r--   0 root         (0) root         (0)      960 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/cases/000-simple-download/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/cases/001-deep-path-download/
+-rw-rw-r--   0 root         (0) root         (0)     1044 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/cases/001-deep-path-download/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/cases/002-simple-upload/
+-rw-rw-r--   0 root         (0) root         (0)     1028 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/cases/002-simple-upload/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/cases/003-deep-path-upload/
+-rw-rw-r--   0 root         (0) root         (0)     1157 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/cases/003-deep-path-upload/main.sh
+-rw-rw-r--   0 root         (0) root         (0)     1919 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/common.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/config/
+-rw-rw-r--   0 root         (0) root         (0)       58 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/config/caddyfile
+-rw-rw-r--   0 root         (0) root         (0)       21 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/config/caddyfile-webdav
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.863076 xrootd-5.6.1/tests/XrdClHttp/config/client/
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/config/client/http.conf
+-rwxrwxr-x   0 root         (0) root         (0)     1571 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClHttp/run_test.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/XrdClTests/
+-rw-rw-r--   0 root         (0) root         (0)     1540 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    27183 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/FileCopyTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    22807 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/FileSystemTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    30512 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/FileTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    21399 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/IdentityPlugIn.cc
+-rw-rw-r--   0 root         (0) root         (0)     2516 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/IdentityPlugIn.hh
+-rw-rw-r--   0 root         (0) root         (0)    22565 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/LocalFileHandlerTest.cc
+-rw-rw-r--   0 root         (0) root         (0)     9085 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/MonitorTestLib.cc
+-rw-rw-r--   0 root         (0) root         (0)    36161 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/OperationsWorkflowTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    10184 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/PollerTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    20068 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/PostMasterTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    11141 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/SocketTest.cc
+-rw-rw-r--   0 root         (0) root         (0)    12152 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/ThreadingTest.cc
+-rw-rw-r--   0 root         (0) root         (0)     7930 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/UtilsTest.cc
+-rw-rw-r--   0 root         (0) root         (0)     4848 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/XRootDProtocolHelper.cc
+-rw-rw-r--   0 root         (0) root         (0)     1982 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/XRootDProtocolHelper.hh
+-rw-rw-r--   0 root         (0) root         (0)      419 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/cppunit.supp
+-rwxrwxr-x   0 root         (0) root         (0)      430 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/printenv.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/XrdClTests/tls/
+-rw-rw-r--   0 root         (0) root         (0)      529 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/tls/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)      712 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/tls/README.md
+-rw-rw-r--   0 root         (0) root         (0)     1861 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/tls/xrdcl-tls.cc
+-rw-rw-r--   0 root         (0) root         (0)    16273 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/tls/xrdsrv-tls.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/XrdClTests/wrt/
+-rw-rw-r--   0 root         (0) root         (0)    14962 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/wrt/xrdsrv-dio.cc
+-rw-rw-r--   0 root         (0) root         (0)    14168 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdClTests/wrt/xrdsrv-wrt.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/XrdEcTests/
+-rw-rw-r--   0 root         (0) root         (0)     1059 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdEcTests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    19308 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdEcTests/MicroTest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/XrdHttpTests/
+-rw-rw-r--   0 root         (0) root         (0)      294 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdHttpTests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     7081 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdHttpTests/XrdHttpTests.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/XrdSsiTests/
+-rw-rw-r--   0 root         (0) root         (0)      440 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdSsiTests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    36887 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/XrdSsiTests/XrdShMap.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/tests/common/
+-rw-rw-r--   0 root         (0) root         (0)      901 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     2485 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/CppUnitXrdHelpers.hh
+-rw-rw-r--   0 root         (0) root         (0)     3148 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/PathProcessor.hh
+-rw-rw-r--   0 root         (0) root         (0)    12734 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/Server.cc
+-rw-rw-r--   0 root         (0) root         (0)     7796 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/Server.hh
+-rw-rw-r--   0 root         (0) root         (0)     4264 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/TestEnv.cc
+-rw-rw-r--   0 root         (0) root         (0)     2456 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/TestEnv.hh
+-rw-rw-r--   0 root         (0) root         (0)     5571 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/TextRunner.cc
+-rw-rw-r--   0 root         (0) root         (0)     3461 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/Utils.cc
+-rw-rw-r--   0 root         (0) root         (0)     4485 2023-07-11 08:55:00.000000 xrootd-5.6.1/tests/common/Utils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/ups/
+-rw-rw-r--   0 root         (0) root         (0)      721 2023-07-11 08:55:00.000000 xrootd-5.6.1/ups/eupspkg.cfg.sh
+-rw-rw-r--   0 root         (0) root         (0)      232 2023-07-11 08:55:00.000000 xrootd-5.6.1/ups/xrootd.table
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/utils/
+-rwxrwxr-x   0 root         (0) root         (0)     6678 2023-07-11 08:55:00.000000 xrootd-5.6.1/utils/XrdCmsNotify.pm
+-rwxrwxr-x   0 root         (0) root         (0)     7851 2023-07-11 08:55:00.000000 xrootd-5.6.1/utils/XrdOlbMonPerf
+-rwxrwxr-x   0 root         (0) root         (0)     3789 2023-07-11 08:55:00.000000 xrootd-5.6.1/utils/cms_monPerf
+-rwxrwxr-x   0 root         (0) root         (0)    29321 2023-07-11 08:55:00.000000 xrootd-5.6.1/utils/hpsscp
+-rwxrwxr-x   0 root         (0) root         (0)     4187 2023-07-11 08:55:00.000000 xrootd-5.6.1/utils/netchk
+-rwxrwxr-x   0 root         (0) root         (0)     2181 2023-07-11 08:55:00.000000 xrootd-5.6.1/utils/xrootd-config
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:20:11.873076 xrootd-5.6.1/xrootd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-07-11 09:20:11.000000 xrootd-5.6.1/xrootd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    48813 2023-07-11 09:20:11.000000 xrootd-5.6.1/xrootd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 09:20:11.000000 xrootd-5.6.1/xrootd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 09:20:11.000000 xrootd-5.6.1/xrootd.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 09:20:11.000000 xrootd-5.6.1/xrootd.egg-info/top_level.txt
```

### Comparing `xrootd-5.6.0/CMakeLists.txt` & `xrootd-5.6.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/COPYING` & `xrootd-5.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/COPYING.BSD` & `xrootd-5.6.1/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/COPYING.LGPL` & `xrootd-5.6.1/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/LICENSE` & `xrootd-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/PKG-INFO` & `xrootd-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xrootd
-Version: 5.6.0
+Version: 5.6.1
 Summary: eXtended ROOT daemon
 Home-page: http://xrootd.org
-Download-URL: https://github.com/xrootd/xrootd/archive/v5.6.0.tar.gz
+Download-URL: https://github.com/xrootd/xrootd/archive/v5.6.1.tar.gz
 Author: XRootD Developers
 Author-email: xrootd-dev@slac.stanford.edu
 License: LGPLv3+
 Keywords: XRootD,network filesystem
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `xrootd-5.6.0/README.md` & `xrootd-5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/CMakeLists.txt` & `xrootd-5.6.1/bindings/python/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else()
   configure_file(setup.py setup.py)
   file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/VERSION "${XRootD_VERSION_STRING}")
 
   option(INSTALL_PYTHON_BINDINGS "Install Python bindings" TRUE)
 
   if(INSTALL_PYTHON_BINDINGS)
-    set(PIP_OPTIONS "" CACHE STRING "Install options for pip")
+    set(PIP_OPTIONS "--use-pep517" CACHE STRING "Install options for pip")
 
     install(CODE "
       execute_process(COMMAND ${Python_EXECUTABLE} -m pip install ${PIP_OPTIONS}
         --prefix \$ENV{DESTDIR}${CMAKE_INSTALL_PREFIX} ${CMAKE_CURRENT_BINARY_DIR}
         RESULT_VARIABLE INSTALL_STATUS)
       if(NOT INSTALL_STATUS EQUAL 0)
         message(FATAL_ERROR \"Failed to install Python bindings\")
```

### Comparing `xrootd-5.6.0/bindings/python/README.md` & `xrootd-5.6.1/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/Makefile` & `xrootd-5.6.1/bindings/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/ReleaseNotes.txt` & `xrootd-5.6.1/bindings/python/docs/ReleaseNotes.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/.static/css/custom.css` & `xrootd-5.6.1/bindings/python/docs/source/.static/css/custom.css`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/conf.py` & `xrootd-5.6.1/bindings/python/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/examples/file.rst` & `xrootd-5.6.1/bindings/python/docs/source/examples/file.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/examples/filesystem.rst` & `xrootd-5.6.1/bindings/python/docs/source/examples/filesystem.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/favicon.ico` & `xrootd-5.6.1/bindings/python/docs/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/gettingstarted.rst` & `xrootd-5.6.1/bindings/python/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/index.rst` & `xrootd-5.6.1/bindings/python/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/modules/client/file.rst` & `xrootd-5.6.1/bindings/python/docs/source/modules/client/file.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/modules/client/filesystem.rst` & `xrootd-5.6.1/bindings/python/docs/source/modules/client/filesystem.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/modules/client/flags.rst` & `xrootd-5.6.1/bindings/python/docs/source/modules/client/flags.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/modules/client/responses.rst` & `xrootd-5.6.1/bindings/python/docs/source/modules/client/responses.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/docs/source/xrootd-200x68.png` & `xrootd-5.6.1/bindings/python/docs/source/xrootd-200x68.png`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/copyprocess.py` & `xrootd-5.6.1/bindings/python/examples/copyprocess.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/dirlist.py` & `xrootd-5.6.1/bindings/python/examples/dirlist.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/fileproperties.py` & `xrootd-5.6.1/bindings/python/examples/fileproperties.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/filesystemproperties.py` & `xrootd-5.6.1/bindings/python/examples/filesystemproperties.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/query.py` & `xrootd-5.6.1/bindings/python/examples/query.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/read.py` & `xrootd-5.6.1/bindings/python/examples/read.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/examples/vector_read.py` & `xrootd-5.6.1/bindings/python/examples/vector_read.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/__init__.py` & `xrootd-5.6.1/bindings/python/libs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/_version.py` & `xrootd-5.6.1/bindings/python/libs/client/_version.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/copyprocess.py` & `xrootd-5.6.1/bindings/python/libs/client/copyprocess.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/env.py` & `xrootd-5.6.1/bindings/python/libs/client/env.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/file.py` & `xrootd-5.6.1/bindings/python/libs/client/file.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/filesystem.py` & `xrootd-5.6.1/bindings/python/libs/client/filesystem.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/finalize.py` & `xrootd-5.6.1/bindings/python/libs/client/finalize.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/flags.py` & `xrootd-5.6.1/bindings/python/libs/client/flags.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/glob_funcs.py` & `xrootd-5.6.1/bindings/python/libs/client/glob_funcs.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/responses.py` & `xrootd-5.6.1/bindings/python/libs/client/responses.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/url.py` & `xrootd-5.6.1/bindings/python/libs/client/url.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/libs/client/utils.py` & `xrootd-5.6.1/bindings/python/libs/client/utils.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/setup.py` & `xrootd-5.6.1/bindings/python/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,19 +95,23 @@
             # path from the site-packages directory. Build with install RPATH
             # because libraries are installed by Python/pip not CMake, so CMake
             # cannot fix the install RPATH later on.
 
             cmake_args = [
                 '-DPython_EXECUTABLE={}'.format(sys.executable),
                 '-DCMAKE_BUILD_WITH_INSTALL_RPATH=TRUE',
-                '-DCMAKE_INSTALL_RPATH=$ORIGIN/../../../../$LIB',
                 '-DCMAKE_ARCHIVE_OUTPUT_DIRECTORY={}/{}'.format(self.build_temp, ext.name),
                 '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={}/{}'.format(extdir, ext.name),
             ]
 
+            if sys.platform == 'darwin':
+                cmake_args += [ '-DCMAKE_INSTALL_RPATH=@loader_path/../../..' ]
+            else:
+                cmake_args += [ '-DCMAKE_INSTALL_RPATH=$ORIGIN/../../../../$LIB' ]
+
             cmake_args += cmdline_args
 
             if not os.path.exists(self.build_temp):
                 os.makedirs(self.build_temp)
 
             check_call([cmake, ext.src, '-B', self.build_temp] + cmake_args)
             check_call([cmake, '--build', self.build_temp, '--parallel'])
```

### Comparing `xrootd-5.6.0/bindings/python/src/AsyncResponseHandler.hh` & `xrootd-5.6.1/bindings/python/src/AsyncResponseHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/CMakeLists.txt` & `xrootd-5.6.1/bindings/python/src/CMakeLists.txt`

 * *Files 17% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 )
 
 target_compile_options(client PRIVATE -w) # TODO: fix build warnings
 
 if(APPLE)
   set(CMAKE_MACOSX_RPATH TRUE)
   set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
-  set_target_properties(client PROPERTIES
-    INSTALL_NAME_DIR "@rpath" INSTALL_RPATH "@loader_path")
+  set_target_properties(client PROPERTIES INSTALL_NAME_DIR "@rpath")
 endif()
 
 # Avoid a call to find_package(XRootD) in order to be able to override
 # variables when building the module as part of a standard CMake build.
 
 if(TARGET XrdCl)
   target_link_libraries(client PRIVATE XrdCl)
```

### Comparing `xrootd-5.6.0/bindings/python/src/ChunkIterator.hh` & `xrootd-5.6.1/bindings/python/src/ChunkIterator.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/Conversions.hh` & `xrootd-5.6.1/bindings/python/src/Conversions.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootD.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDCopyProcess.cc` & `xrootd-5.6.1/bindings/python/src/PyXRootDCopyProcess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDCopyProcess.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDCopyProcess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDCopyProgressHandler.cc` & `xrootd-5.6.1/bindings/python/src/PyXRootDCopyProgressHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDCopyProgressHandler.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDCopyProgressHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDEnv.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDFile.cc` & `xrootd-5.6.1/bindings/python/src/PyXRootDFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDFile.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDFileSystem.cc` & `xrootd-5.6.1/bindings/python/src/PyXRootDFileSystem.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDFileSystem.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDFileSystem.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDFinalize.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDFinalize.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDModule.cc` & `xrootd-5.6.1/bindings/python/src/PyXRootDModule.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDURL.cc` & `xrootd-5.6.1/bindings/python/src/PyXRootDURL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/PyXRootDURL.hh` & `xrootd-5.6.1/bindings/python/src/PyXRootDURL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/Utils.cc` & `xrootd-5.6.1/bindings/python/src/Utils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/src/Utils.hh` & `xrootd-5.6.1/bindings/python/src/Utils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/tests/test_copy.py` & `xrootd-5.6.1/bindings/python/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/tests/test_file.py` & `xrootd-5.6.1/bindings/python/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/tests/test_filesystem.py` & `xrootd-5.6.1/bindings/python/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/tests/test_glob.py` & `xrootd-5.6.1/bindings/python/tests/test_glob.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/tests/test_threads.py` & `xrootd-5.6.1/bindings/python/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/bindings/python/tests/test_url.py` & `xrootd-5.6.1/bindings/python/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/FindCppUnit.cmake` & `xrootd-5.6.1/cmake/FindCppUnit.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/FindDavix.cmake` & `xrootd-5.6.1/cmake/FindDavix.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/FindKerberos5.cmake` & `xrootd-5.6.1/cmake/FindKerberos5.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/FindReadline.cmake` & `xrootd-5.6.1/cmake/FindReadline.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/FindVOMS.cmake` & `xrootd-5.6.1/cmake/FindVOMS.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/Findfuse.cmake` & `xrootd-5.6.1/cmake/Findfuse.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/Findisal.cmake` & `xrootd-5.6.1/cmake/Findisal.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/Findlibuuid.cmake` & `xrootd-5.6.1/cmake/Findlibuuid.cmake`

 * *Files 16% similar despite different names*

```diff
@@ -38,45 +38,59 @@
   unset(UUID_${var} CACHE)
 endforeach()
 
 if(NOT UUID_INCLUDE_DIR)
   find_path(UUID_INCLUDE_DIR uuid/uuid.h)
 endif()
 
-if(EXISTS UUID_INCLUDE_DIR)
+if(IS_DIRECTORY "${UUID_INCLUDE_DIR}")
+  include(CheckCXXSymbolExists)
   set(UUID_INCLUDE_DIRS ${UUID_INCLUDE_DIR})
   set(CMAKE_REQUIRED_INCLUDES ${UUID_INCLUDE_DIRS})
   check_cxx_symbol_exists("uuid_generate_random" "uuid/uuid.h" _uuid_header_only)
   unset(CMAKE_REQUIRED_INCLUDES)
 endif()
 
-if(NOT _uuid_header_only AND NOT UUID_LIBRARY)
-  find_package(PkgConfig)
-
-  if(PKG_CONFIG_FOUND)
-    if(${libuuid_FIND_REQUIRED})
-      set(libuuid_REQUIRED REQUIRED)
+if(_uuid_header_only)
+  find_package_handle_standard_args(libuuid DEFAULT_MSG UUID_INCLUDE_DIR)
+else()
+  if(NOT UUID_LIBRARY)
+    include(CheckLibraryExists)
+    check_library_exists("uuid" "uuid_generate_random" "" _have_libuuid)
+
+    if(_have_libuuid)
+      set(UUID_LIBRARY "uuid")
+      set(UUID_LIBRARIES ${UUID_LIBRARY})
+    else()
+      find_package(PkgConfig)
+      if(PKG_CONFIG_FOUND)
+        if(${libuuid_FIND_REQUIRED})
+          set(libuuid_REQUIRED REQUIRED)
+        endif()
+        pkg_check_modules(UUID ${libuuid_REQUIRED} uuid)
+        set(UUID_LIBRARIES ${UUID_LDFLAGS})
+        set(UUID_LIBRARY ${UUID_LIBRARIES})
+        set(UUID_INCLUDE_DIRS ${UUID_INCLUDE_DIRS})
+        set(UUID_INCLUDE_DIR ${UUID_INCLUDE_DIRS})
+      endif()
     endif()
-
-    pkg_check_modules(UUID ${libuuid_REQUIRED} uuid)
-
-    set(UUID_LIBRARIES ${UUID_LDFLAGS})
-    set(UUID_LIBRARY ${UUID_LIBRARIES})
-    set(UUID_INCLUDE_DIRS ${UUID_INCLUDE_DIRS})
-    set(UUID_INCLUDE_DIR ${UUID_INCLUDE_DIRS})
+    unset(_have_libuuid)
   endif()
+  find_package_handle_standard_args(libuuid DEFAULT_MSG UUID_INCLUDE_DIR UUID_LIBRARY)
 endif()
 
-if(UUID_FOUND AND NOT TARGET uuid::uuid)
+if(LIBUUID_FOUND AND NOT TARGET uuid::uuid)
   add_library(uuid::uuid INTERFACE IMPORTED)
-  set_property(TARGET uuid::uuid PROPERTY INTERFACE_INCLUDE_DIRECTORIES "${UUID_INCLUDE_DIRS}")
+  set_property(TARGET uuid::uuid PROPERTY INTERFACE_SYSTEM_INCLUDE_DIRECTORIES "${UUID_INCLUDE_DIRS}")
   set_property(TARGET uuid::uuid PROPERTY INTERFACE_LINK_LIBRARIES "${UUID_LIBRARIES}")
 endif()
 
-if(_uuid_header_only)
-  find_package_handle_standard_args(libuuid DEFAULT_MSG UUID_INCLUDE_DIR)
-else()
-  find_package_handle_standard_args(libuuid DEFAULT_MSG UUID_INCLUDE_DIR UUID_LIBRARY)
-endif()
-
-unset(_uuid_header_only)
 mark_as_advanced(UUID_INCLUDE_DIR UUID_LIBRARY)
+
+if(NOT "${libuuid_FIND_QUIET}")
+  message(DEBUG "UUID_FOUND        = ${LIBUUID_FOUND}")
+  message(DEBUG "UUID_HEADER_ONLY  = ${_uuid_header_only}")
+  message(DEBUG "UUID_INCLUDE_DIR  = ${UUID_INCLUDE_DIR}")
+  message(DEBUG "UUID_INCLUDE_DIRS = ${UUID_INCLUDE_DIRS}")
+  message(DEBUG "UUID_LIBRARY      = ${UUID_LIBRARY}")
+  message(DEBUG "UUID_LIBRARIES    = ${UUID_LIBRARIES}")
+endif()
```

### Comparing `xrootd-5.6.0/cmake/Findsystemd.cmake` & `xrootd-5.6.1/cmake/Findsystemd.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/XRootDConfig.cmake.in` & `xrootd-5.6.1/cmake/XRootDConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/XRootDDefaults.cmake` & `xrootd-5.6.1/cmake/XRootDDefaults.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/XRootDFindLibs.cmake` & `xrootd-5.6.1/cmake/XRootDFindLibs.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -169,16 +169,16 @@
       set( BUILD_XRDEC TRUE )
     else()
       set( BUILD_XRDEC FALSE )
     endif()
   endif()
 endif()
 
-if( ENABLE_PYTHON AND (LINUX OR KFREEBSD OR Hurd OR MacOSX) )
-  if( FORCE_ENABLED )
+if( ENABLE_PYTHON )
+  if( FORCE_ENABLED OR PYPI_BUILD )
     find_package( Python ${XRD_PYTHON_REQ_VERSION} COMPONENTS Interpreter Development REQUIRED )
   else()
     find_package( Python ${XRD_PYTHON_REQ_VERSION} COMPONENTS Interpreter Development )
   endif()
   if( Python_Interpreter_FOUND AND Python_Development_FOUND )
     set( BUILD_PYTHON TRUE )
   else()
```

### Comparing `xrootd-5.6.0/cmake/XRootDOSDefs.cmake` & `xrootd-5.6.1/cmake/XRootDOSDefs.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 #-------------------------------------------------------------------------------
 # MacOSX
 #-------------------------------------------------------------------------------
 if( APPLE )
   set( MacOSX TRUE )
   set( XrdClPipelines TRUE )
   
-  if( NOT DEFINED CMAKE_MACOSX_RPATH )
-    set( CMAKE_MACOSX_RPATH 1 )
-  endif()
+  set(CMAKE_MACOSX_RPATH TRUE)
+  set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
+  set(CMAKE_INSTALL_RPATH "@loader_path/../lib")
 
   # this is here because of Apple deprecating openssl and krb5
   set( CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wno-deprecated-declarations" )
 
   add_definitions( -DLT_MODULE_EXT=".dylib" )
   define_default( CMAKE_INSTALL_LIBDIR "lib" )
   define_default( CMAKE_INSTALL_BINDIR "bin" )
```

### Comparing `xrootd-5.6.0/cmake/XRootDSummary.cmake` & `xrootd-5.6.1/cmake/XRootDSummary.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/XRootDSystemCheck.cmake` & `xrootd-5.6.1/cmake/XRootDSystemCheck.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/XRootDUtils.cmake` & `xrootd-5.6.1/cmake/XRootDUtils.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake/XRootDVersion.cmake` & `xrootd-5.6.1/cmake/XRootDVersion.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/cmake_uninstall.cmake.in` & `xrootd-5.6.1/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/CONTRIBUTING.md` & `xrootd-5.6.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/INSTALL.md` & `xrootd-5.6.1/docs/INSTALL.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,23 +128,23 @@
     googletest \
     isa-l \
     krb5 \
     libxml2 \
     libxcrypt \
     make \
     openssl@1.1 \
-    ossp-uuid \
     pkg-config \
     python@3.11 \
     readline \
     zlib \
 ```
 
-Homebrew is also available on Linux. The dependency `ossp-uuid` is not required
-in this case, and `libfuse@2` can be installed to enable FUSE support.
+Homebrew is also available on Linux, where `utils-linux` is required as
+an extra dependency since uuid symbols are not provided by the kernel like
+on macOS. On Linux, `libfuse@2` may be installed to enable FUSE support.
 
 ## Building from Source Code with CMake
 
 XRootD uses [CMake](https://cmake.org) as its build generator. CMake
 is used during configuration to generate the actual build system that
 is used to build the project with a build tool like `make` or `ninja`.
 If you are new to CMake, we recommend reading the official
```

### Comparing `xrootd-5.6.0/docs/README_IPV4_To_IPV6` & `xrootd-5.6.1/docs/README_IPV4_To_IPV6`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/ReleaseNotes.txt` & `xrootd-5.6.1/docs/ReleaseNotes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,31 @@
 XRootD
 ======
 
 Release Notes
 =============
 
 -------------
+Version 5.6.1
+-------------
+
++ **Minor bug fixes**
+  **[CMake]** Fix Findlibuuid.cmake to use kernel provided uuid on macOS
+  **[XrdCl]** Avoid race in postmaster QueryTransport
+  **[XrdCl]** Add missing argument in call to debug log message.
+    This fixes sporadic crashes seen in FTS when debug logging is enabled.
+  **[XrdCrypto]** Avoid race in GetCryptoFactory
+
++ **Miscellaneous**
+  **[CMake]** Make sure Python is required in PyPI build
+  **[CMake]** Set RPATH that works for binaries and libraries on macOS
+  **[CMake,Python]** Handle RPATH for Python bindings on macOS
+  **[Python]** Use PEP517 by default when building Python bindings
+
+-------------
 Version 5.6.0
 -------------
 
 + **New Features**
   **[CMake]** Modernization of build system, now requires CMake 3.16
   **[Client]** Add xrdfs cache subcommand to allow for cache evictions
   **[Misc]** Add support for building with musl libc (issue #1645)
```

### Comparing `xrootd-5.6.0/docs/TESTING.md` & `xrootd-5.6.1/docs/TESTING.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/cmsd.8` & `xrootd-5.6.1/docs/man/cmsd.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/frm_admin.8` & `xrootd-5.6.1/docs/man/frm_admin.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/frm_purged.8` & `xrootd-5.6.1/docs/man/frm_purged.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/frm_xfragent.8` & `xrootd-5.6.1/docs/man/frm_xfragent.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/frm_xfrd.8` & `xrootd-5.6.1/docs/man/frm_xfrd.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/libXrdVoms.1` & `xrootd-5.6.1/docs/man/libXrdVoms.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/mpxstats.8` & `xrootd-5.6.1/docs/man/mpxstats.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdadler32.1` & `xrootd-5.6.1/docs/man/xrdadler32.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdcp.1` & `xrootd-5.6.1/docs/man/xrdcp.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdfs.1` & `xrootd-5.6.1/docs/man/xrdfs.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdgsiproxy.1` & `xrootd-5.6.1/docs/man/xrdgsiproxy.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdgsitest.1` & `xrootd-5.6.1/docs/man/xrdgsitest.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdmapc.1` & `xrootd-5.6.1/docs/man/xrdmapc.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdpfc_print.8` & `xrootd-5.6.1/docs/man/xrdpfc_print.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdpwdadmin.8` & `xrootd-5.6.1/docs/man/xrdpwdadmin.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrdsssadmin.8` & `xrootd-5.6.1/docs/man/xrdsssadmin.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrootd.8` & `xrootd-5.6.1/docs/man/xrootd.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/docs/man/xrootdfs.1` & `xrootd-5.6.1/docs/man/xrootdfs.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/gen-tarball.sh` & `xrootd-5.6.1/gen-tarball.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/genversion.sh` & `xrootd-5.6.1/genversion.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/client-plugin.conf.example` & `xrootd-5.6.1/packaging/common/client-plugin.conf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/client.conf` & `xrootd-5.6.1/packaging/common/client.conf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/cmsd@.service` & `xrootd-5.6.1/packaging/common/cmsd@.service`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/frm_purged@.service` & `xrootd-5.6.1/packaging/common/frm_purged@.service`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/frm_xfrd@.service` & `xrootd-5.6.1/packaging/common/frm_xfrd@.service`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd-clustered.cfg` & `xrootd-5.6.1/packaging/common/xrootd-clustered.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd-filecache-clustered.cfg` & `xrootd-5.6.1/packaging/common/xrootd-filecache-clustered.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd-filecache-standalone.cfg` & `xrootd-5.6.1/packaging/common/xrootd-filecache-standalone.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd-http.cfg` & `xrootd-5.6.1/packaging/common/xrootd-http.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd-standalone.cfg` & `xrootd-5.6.1/packaging/common/xrootd-standalone.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd.logrotate` & `xrootd-5.6.1/packaging/common/xrootd.logrotate`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd.te` & `xrootd-5.6.1/packaging/common/xrootd.te`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/common/xrootd@.service` & `xrootd-5.6.1/packaging/common/xrootd@.service`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/debian/control` & `xrootd-5.6.1/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/debian/copyright` & `xrootd-5.6.1/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/debian/rules` & `xrootd-5.6.1/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/debian/xrootd-server.install` & `xrootd-5.6.1/packaging/debian/xrootd-server.install`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/debian_scripts/publish_debian_cern.sh` & `xrootd-5.6.1/packaging/debian_scripts/publish_debian_cern.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/makesrpm.sh` & `xrootd-5.6.1/packaging/makesrpm.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/cmsd.init` & `xrootd-5.6.1/packaging/rhel/cmsd.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/frm_purged.init` & `xrootd-5.6.1/packaging/rhel/frm_purged.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/frm_xfrd.init` & `xrootd-5.6.1/packaging/rhel/frm_xfrd.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/xrootd.functions` & `xrootd-5.6.1/packaging/rhel/xrootd.functions`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/xrootd.functions-slc4` & `xrootd-5.6.1/packaging/rhel/xrootd.functions-slc4`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/xrootd.init` & `xrootd-5.6.1/packaging/rhel/xrootd.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/xrootd.spec.in` & `xrootd-5.6.1/packaging/rhel/xrootd.spec.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/rhel/xrootd.sysconfig` & `xrootd-5.6.1/packaging/rhel/xrootd.sysconfig`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/README` & `xrootd-5.6.1/packaging/tgz/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StartCMS` & `xrootd-5.6.1/packaging/tgz/StartCMS`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StartFRM` & `xrootd-5.6.1/packaging/tgz/StartFRM`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StartOLB` & `xrootd-5.6.1/packaging/tgz/StartOLB`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StartOLB.cf.example` & `xrootd-5.6.1/packaging/tgz/StartOLB.cf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StartXRD` & `xrootd-5.6.1/packaging/tgz/StartXRD`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StartXRD.cf.example` & `xrootd-5.6.1/packaging/tgz/StartXRD.cf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StopCMS` & `xrootd-5.6.1/packaging/tgz/StopCMS`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StopFRM` & `xrootd-5.6.1/packaging/tgz/StopFRM`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StopOLB` & `xrootd-5.6.1/packaging/tgz/StopOLB`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/StopXRD` & `xrootd-5.6.1/packaging/tgz/StopXRD`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/xrootd.cf.example` & `xrootd-5.6.1/packaging/tgz/xrootd.cf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/tgz/xrootd.cf.example2` & `xrootd-5.6.1/packaging/tgz/xrootd.cf.example2`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/packaging/wheel/publish.sh` & `xrootd-5.6.1/packaging/wheel/publish.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/setup.py` & `xrootd-5.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,21 +66,25 @@
             # Use $ORIGIN RPATH to ensure that the client library can load
             # libXrdCl which will be installed in the same directory. Build
             # with install RPATH because libraries are installed by Python/pip
             # not CMake, so CMake cannot fix the install RPATH later on.
 
             cmake_args = [
                 '-DPython_EXECUTABLE={}'.format(sys.executable),
-                '-DCMAKE_INSTALL_RPATH=$ORIGIN',
                 '-DCMAKE_BUILD_WITH_INSTALL_RPATH=TRUE',
                 '-DCMAKE_ARCHIVE_OUTPUT_DIRECTORY={}/{}'.format(self.build_temp, ext.name),
                 '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={}/{}'.format(extdir, ext.name),
                 '-DENABLE_PYTHON=1', '-DENABLE_XRDCL=1', '-DXRDCL_LIB_ONLY=1', '-DPYPI_BUILD=1'
             ]
 
+            if sys.platform == 'darwin':
+                cmake_args += [ '-DCMAKE_INSTALL_RPATH=@loader_path' ]
+            else:
+                cmake_args += [ '-DCMAKE_INSTALL_RPATH=$ORIGIN' ]
+
             cmake_args += cmdline_args
 
             if not os.path.exists(self.build_temp):
                 os.makedirs(self.build_temp)
 
             check_call([cmake, ext.src, '-B', self.build_temp] + cmake_args)
             check_call([cmake, '--build', self.build_temp, '--parallel'])
```

### Comparing `xrootd-5.6.0/src/CMakeLists.txt` & `xrootd-5.6.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XProtocol/README` & `xrootd-5.6.1/src/XProtocol/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XProtocol/XProtocol.cc` & `xrootd-5.6.1/src/XProtocol/XProtocol.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XProtocol/XProtocol.hh` & `xrootd-5.6.1/src/XProtocol/XProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XProtocol/XPtypes.hh` & `xrootd-5.6.1/src/XProtocol/XPtypes.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XProtocol/YProtocol.hh` & `xrootd-5.6.1/src/XProtocol/YProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdBuffXL.cc` & `xrootd-5.6.1/src/Xrd/XrdBuffXL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdBuffXL.hh` & `xrootd-5.6.1/src/Xrd/XrdBuffXL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdBuffer.cc` & `xrootd-5.6.1/src/Xrd/XrdBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdBuffer.hh` & `xrootd-5.6.1/src/Xrd/XrdBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdConfig.cc` & `xrootd-5.6.1/src/Xrd/XrdConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdConfig.hh` & `xrootd-5.6.1/src/Xrd/XrdConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdGlobals.cc` & `xrootd-5.6.1/src/Xrd/XrdGlobals.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdInet.cc` & `xrootd-5.6.1/src/Xrd/XrdInet.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdInet.hh` & `xrootd-5.6.1/src/Xrd/XrdInet.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdInfo.cc` & `xrootd-5.6.1/src/Xrd/XrdInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdInfo.hh` & `xrootd-5.6.1/src/Xrd/XrdInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdJob.hh` & `xrootd-5.6.1/src/Xrd/XrdJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLink.cc` & `xrootd-5.6.1/src/Xrd/XrdLink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLink.hh` & `xrootd-5.6.1/src/Xrd/XrdLink.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkCtl.cc` & `xrootd-5.6.1/src/Xrd/XrdLinkCtl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkCtl.hh` & `xrootd-5.6.1/src/Xrd/XrdLinkCtl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkInfo.hh` & `xrootd-5.6.1/src/Xrd/XrdLinkInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkMatch.cc` & `xrootd-5.6.1/src/Xrd/XrdLinkMatch.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkMatch.hh` & `xrootd-5.6.1/src/Xrd/XrdLinkMatch.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkXeq.cc` & `xrootd-5.6.1/src/Xrd/XrdLinkXeq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdLinkXeq.hh` & `xrootd-5.6.1/src/Xrd/XrdLinkXeq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdMain.cc` & `xrootd-5.6.1/src/Xrd/XrdMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdObject.hh` & `xrootd-5.6.1/src/Xrd/XrdObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdObject.icc` & `xrootd-5.6.1/src/Xrd/XrdObject.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPoll.cc` & `xrootd-5.6.1/src/Xrd/XrdPoll.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPoll.hh` & `xrootd-5.6.1/src/Xrd/XrdPoll.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPollE.hh` & `xrootd-5.6.1/src/Xrd/XrdPollE.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPollE.icc` & `xrootd-5.6.1/src/Xrd/XrdPollE.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPollInfo.hh` & `xrootd-5.6.1/src/Xrd/XrdPollInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPollPoll.hh` & `xrootd-5.6.1/src/Xrd/XrdPollPoll.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdPollPoll.icc` & `xrootd-5.6.1/src/Xrd/XrdPollPoll.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdProtLoad.cc` & `xrootd-5.6.1/src/Xrd/XrdProtLoad.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdProtLoad.hh` & `xrootd-5.6.1/src/Xrd/XrdProtLoad.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdProtocol.hh` & `xrootd-5.6.1/src/Xrd/XrdProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdScheduler.cc` & `xrootd-5.6.1/src/Xrd/XrdScheduler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdScheduler.hh` & `xrootd-5.6.1/src/Xrd/XrdScheduler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdSendQ.cc` & `xrootd-5.6.1/src/Xrd/XrdSendQ.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdSendQ.hh` & `xrootd-5.6.1/src/Xrd/XrdSendQ.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdStats.cc` & `xrootd-5.6.1/src/Xrd/XrdStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdStats.hh` & `xrootd-5.6.1/src/Xrd/XrdStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdTcpMonPin.hh` & `xrootd-5.6.1/src/Xrd/XrdTcpMonPin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/Xrd/XrdTrace.hh` & `xrootd-5.6.1/src/Xrd/XrdTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAccess.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccAccess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAccess.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccAccess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAudit.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccAudit.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAudit.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccAudit.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAuthDB.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccAuthDB.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAuthFile.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccAuthFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAuthFile.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccAuthFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccAuthorize.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccAuthorize.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccCapability.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccCapability.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccCapability.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccCapability.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccConfig.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccConfig.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccEntity.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccEntity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccEntity.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccEntity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccGroups.cc` & `xrootd-5.6.1/src/XrdAcc/XrdAccGroups.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccGroups.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccGroups.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdAcc/XrdAccPrivs.hh` & `xrootd-5.6.1/src/XrdAcc/XrdAccPrivs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdAccTest.cc` & `xrootd-5.6.1/src/XrdApps/XrdAccTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdAppsCconfig.cc` & `xrootd-5.6.1/src/XrdApps/XrdAppsCconfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdCks.cc` & `xrootd-5.6.1/src/XrdApps/XrdCks.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc` & `xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh` & `xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc` & `xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh` & `xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClProxyPlugin/README.md` & `xrootd-5.6.1/src/XrdApps/XrdClProxyPlugin/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/README.md` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh` & `xrootd-5.6.1/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdCpConfig.cc` & `xrootd-5.6.1/src/XrdApps/XrdCpConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdCpConfig.hh` & `xrootd-5.6.1/src/XrdApps/XrdCpConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdCpFile.cc` & `xrootd-5.6.1/src/XrdApps/XrdCpFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdCpFile.hh` & `xrootd-5.6.1/src/XrdApps/XrdCpFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdCrc32c.cc` & `xrootd-5.6.1/src/XrdApps/XrdCrc32c.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdMapCluster.cc` & `xrootd-5.6.1/src/XrdApps/XrdMapCluster.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdMpxStats.cc` & `xrootd-5.6.1/src/XrdApps/XrdMpxStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdMpxXml.cc` & `xrootd-5.6.1/src/XrdApps/XrdMpxXml.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdMpxXml.hh` & `xrootd-5.6.1/src/XrdApps/XrdMpxXml.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdPinls.cc` & `xrootd-5.6.1/src/XrdApps/XrdPinls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdPrep.cc` & `xrootd-5.6.1/src/XrdApps/XrdPrep.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdQStats.cc` & `xrootd-5.6.1/src/XrdApps/XrdQStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/XrdWait41.cc` & `xrootd-5.6.1/src/XrdApps/XrdWait41.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps/Xrdadler32.cc` & `xrootd-5.6.1/src/XrdApps/Xrdadler32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdApps.cmake` & `xrootd-5.6.1/src/XrdApps.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwm.cc` & `xrootd-5.6.1/src/XrdBwm/XrdBwm.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwm.hh` & `xrootd-5.6.1/src/XrdBwm/XrdBwm.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmConfig.cc` & `xrootd-5.6.1/src/XrdBwm/XrdBwmConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmHandle.cc` & `xrootd-5.6.1/src/XrdBwm/XrdBwmHandle.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmHandle.hh` & `xrootd-5.6.1/src/XrdBwm/XrdBwmHandle.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmLogger.cc` & `xrootd-5.6.1/src/XrdBwm/XrdBwmLogger.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmLogger.hh` & `xrootd-5.6.1/src/XrdBwm/XrdBwmLogger.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmPolicy.hh` & `xrootd-5.6.1/src/XrdBwm/XrdBwmPolicy.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmPolicy1.cc` & `xrootd-5.6.1/src/XrdBwm/XrdBwmPolicy1.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmPolicy1.hh` & `xrootd-5.6.1/src/XrdBwm/XrdBwmPolicy1.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdBwm/XrdBwmTrace.hh` & `xrootd-5.6.1/src/XrdBwm/XrdBwmTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/.gitignore` & `xrootd-5.6.1/src/XrdCeph/.gitignore`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/.gitlab-ci.yml` & `xrootd-5.6.1/src/XrdCeph/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/CMakeLists.txt` & `xrootd-5.6.1/src/XrdCeph/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/COPYING` & `xrootd-5.6.1/src/XrdCeph/COPYING`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/COPYING.BSD` & `xrootd-5.6.1/src/XrdCeph/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/COPYING.LGPL` & `xrootd-5.6.1/src/XrdCeph/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/Doxyfile` & `xrootd-5.6.1/src/XrdCeph/Doxyfile`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/LICENSE` & `xrootd-5.6.1/src/XrdCeph/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/README` & `xrootd-5.6.1/src/XrdCeph/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/FindCppUnit.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/FindCppUnit.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/FindXRootD.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/FindXRootD.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/Findceph.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/Findceph.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/GNUInstallDirs.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/GNUInstallDirs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/XRootDDefaults.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/XRootDDefaults.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/XRootDOSDefs.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/XRootDOSDefs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/XRootDSummary.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/XRootDSummary.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/cmake/XRootDUtils.cmake` & `xrootd-5.6.1/src/XrdCeph/cmake/XRootDUtils.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/docs/ReleaseNotes.txt` & `xrootd-5.6.1/src/XrdCeph/docs/ReleaseNotes.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/packaging/debian/control` & `xrootd-5.6.1/src/XrdCeph/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/packaging/debian/copyright` & `xrootd-5.6.1/src/XrdCeph/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/packaging/debian/rules` & `xrootd-5.6.1/src/XrdCeph/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/packaging/debian_scripts/publish_debian_cern.sh` & `xrootd-5.6.1/src/XrdCeph/packaging/debian_scripts/publish_debian_cern.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/packaging/makesrpm.sh` & `xrootd-5.6.1/src/XrdCeph/packaging/makesrpm.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/packaging/rhel/xrootd-ceph.spec.in` & `xrootd-5.6.1/src/XrdCeph/packaging/rhel/xrootd-ceph.spec.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOss.cc` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOss.hh` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssDir.cc` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssDir.hh` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssFile.cc` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephOssFile.hh` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephOssFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephPosix.cc` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephPosix.hh` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephXAttr.cc` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephXAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph/XrdCephXAttr.hh` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph/XrdCephXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdCeph.cmake` & `xrootd-5.6.1/src/XrdCeph/src/XrdCeph.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/src/XrdVersion.hh.in` & `xrootd-5.6.1/src/XrdCeph/src/XrdVersion.hh.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/tests/XrdCephTests/CMakeLists.txt` & `xrootd-5.6.1/src/XrdCeph/tests/XrdCephTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCeph/tests/XrdCephTests/CephParsingTest.cc` & `xrootd-5.6.1/src/XrdCeph/tests/XrdCephTests/CephParsingTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCks.hh` & `xrootd-5.6.1/src/XrdCks/XrdCks.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksAssist.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksAssist.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksAssist.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksAssist.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalc.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksCalc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalcadler32.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksCalcadler32.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32C.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32C.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalccrc32C.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksCalccrc32C.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalcmd5.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksCalcmd5.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalcmd5.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksCalcmd5.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksCalczcrc32.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksCalczcrc32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksConfig.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksConfig.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksData.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksLoader.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksLoader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksLoader.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksLoader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksManOss.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksManOss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksManOss.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksManOss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksManager.cc` & `xrootd-5.6.1/src/XrdCks/XrdCksManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksManager.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksWrapper.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksWrapper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCks/XrdCksXAttr.hh` & `xrootd-5.6.1/src/XrdCks/XrdCksXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/CMakeLists.txt` & `xrootd-5.6.1/src/XrdCl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAnyObject.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAnyObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClApply.hh` & `xrootd-5.6.1/src/XrdCl/XrdClApply.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClArg.hh` & `xrootd-5.6.1/src/XrdCl/XrdClArg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncDiscardReader.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncDiscardReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncHSReader.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncHSReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncHSWriter.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncHSWriter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncMsgReader.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncMsgReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncMsgWriter.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncMsgWriter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncPageReader.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncPageReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncRawReader.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncRawReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncRawReaderIntfc.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncRawReaderIntfc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncSocketHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncSocketHandler.cc`

 * *Files 1% similar despite different names*

```diff
@@ -620,15 +620,15 @@
         {
           //--------------------------------------------------------------------
           // We need to wait before replaying the request
           //--------------------------------------------------------------------
           Log *log = DefaultEnv::GetLog();
           log->Debug( AsyncSockMsg, "[%s] Received a wait response to endsess request, "
                       "will wait for %d seconds before replaying the endsess request",
-                      waitSeconds );
+                      pStreamName.c_str(), waitSeconds );
           pHSWaitStarted = time( 0 );
           pHSWaitSeconds = waitSeconds;
         }
         return true;
       }
       //------------------------------------------------------------------------
       // We are re-sending a protocol request
```

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncSocketHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncSocketHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClAsyncVectorReader.hh` & `xrootd-5.6.1/src/XrdCl/XrdClAsyncVectorReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClBuffer.hh` & `xrootd-5.6.1/src/XrdCl/XrdClBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClChannel.cc` & `xrootd-5.6.1/src/XrdCl/XrdClChannel.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClChannel.hh` & `xrootd-5.6.1/src/XrdCl/XrdClChannel.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClChannelHandlerList.cc` & `xrootd-5.6.1/src/XrdCl/XrdClChannelHandlerList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClChannelHandlerList.hh` & `xrootd-5.6.1/src/XrdCl/XrdClChannelHandlerList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCheckSumHelper.hh` & `xrootd-5.6.1/src/XrdCl/XrdClCheckSumHelper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCheckSumManager.cc` & `xrootd-5.6.1/src/XrdCl/XrdClCheckSumManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCheckSumManager.hh` & `xrootd-5.6.1/src/XrdCl/XrdClCheckSumManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCheckpointOperation.hh` & `xrootd-5.6.1/src/XrdCl/XrdClCheckpointOperation.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClClassicCopyJob.cc` & `xrootd-5.6.1/src/XrdCl/XrdClClassicCopyJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClClassicCopyJob.hh` & `xrootd-5.6.1/src/XrdCl/XrdClClassicCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClConstants.hh` & `xrootd-5.6.1/src/XrdCl/XrdClConstants.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCopy.cc` & `xrootd-5.6.1/src/XrdCl/XrdClCopy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCopyJob.hh` & `xrootd-5.6.1/src/XrdCl/XrdClCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCopyProcess.cc` & `xrootd-5.6.1/src/XrdCl/XrdClCopyProcess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCopyProcess.hh` & `xrootd-5.6.1/src/XrdCl/XrdClCopyProcess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClCtx.hh` & `xrootd-5.6.1/src/XrdCl/XrdClCtx.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClDefaultEnv.cc` & `xrootd-5.6.1/src/XrdCl/XrdClDefaultEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClDefaultEnv.hh` & `xrootd-5.6.1/src/XrdCl/XrdClDefaultEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClDlgEnv.hh` & `xrootd-5.6.1/src/XrdCl/XrdClDlgEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClEcHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClEcHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClEcHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClEcHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClEnv.cc` & `xrootd-5.6.1/src/XrdCl/XrdClEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClEnv.hh` & `xrootd-5.6.1/src/XrdCl/XrdClEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFS.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFSExecutor.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFSExecutor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFSExecutor.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFSExecutor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFile.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFile.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileOperations.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFileOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileStateHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFileStateHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileStateHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFileStateHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileSystem.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFileSystem.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileSystem.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFileSystem.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileSystemOperations.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFileSystemOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileSystemUtils.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFileSystemUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileSystemUtils.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFileSystemUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileTimer.cc` & `xrootd-5.6.1/src/XrdCl/XrdClFileTimer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFileTimer.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFileTimer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFinalOperation.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFinalOperation.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClForkHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClForkHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClForkHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClForkHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClFwd.hh` & `xrootd-5.6.1/src/XrdCl/XrdClFwd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClInQueue.cc` & `xrootd-5.6.1/src/XrdCl/XrdClInQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClInQueue.hh` & `xrootd-5.6.1/src/XrdCl/XrdClInQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClJobManager.cc` & `xrootd-5.6.1/src/XrdCl/XrdClJobManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClJobManager.hh` & `xrootd-5.6.1/src/XrdCl/XrdClJobManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClLocalFileHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClLocalFileHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClLocalFileHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClLocalFileHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClLocalFileTask.cc` & `xrootd-5.6.1/src/XrdCl/XrdClLocalFileTask.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClLocalFileTask.hh` & `xrootd-5.6.1/src/XrdCl/XrdClLocalFileTask.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClLog.cc` & `xrootd-5.6.1/src/XrdCl/XrdClLog.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClLog.hh` & `xrootd-5.6.1/src/XrdCl/XrdClLog.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClMessage.hh` & `xrootd-5.6.1/src/XrdCl/XrdClMessage.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClMessageUtils.cc` & `xrootd-5.6.1/src/XrdCl/XrdClMessageUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClMessageUtils.hh` & `xrootd-5.6.1/src/XrdCl/XrdClMessageUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClMetalinkRedirector.cc` & `xrootd-5.6.1/src/XrdCl/XrdClMetalinkRedirector.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClMetalinkRedirector.hh` & `xrootd-5.6.1/src/XrdCl/XrdClMetalinkRedirector.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClMonitor.hh` & `xrootd-5.6.1/src/XrdCl/XrdClMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOperationHandlers.hh` & `xrootd-5.6.1/src/XrdCl/XrdClOperationHandlers.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOperationTimeout.hh` & `xrootd-5.6.1/src/XrdCl/XrdClOperationTimeout.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOperations.cc` & `xrootd-5.6.1/src/XrdCl/XrdClOperations.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOperations.hh` & `xrootd-5.6.1/src/XrdCl/XrdClOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOptimizers.hh` & `xrootd-5.6.1/src/XrdCl/XrdClOptimizers.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOptional.hh` & `xrootd-5.6.1/src/XrdCl/XrdClOptional.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOutQueue.cc` & `xrootd-5.6.1/src/XrdCl/XrdClOutQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClOutQueue.hh` & `xrootd-5.6.1/src/XrdCl/XrdClOutQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClParallelOperation.hh` & `xrootd-5.6.1/src/XrdCl/XrdClParallelOperation.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPlugInInterface.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPlugInInterface.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPlugInManager.cc` & `xrootd-5.6.1/src/XrdCl/XrdClPlugInManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPlugInManager.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPlugInManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPoller.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPoller.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPollerBuiltIn.cc` & `xrootd-5.6.1/src/XrdCl/XrdClPollerBuiltIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPollerBuiltIn.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPollerBuiltIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPollerFactory.cc` & `xrootd-5.6.1/src/XrdCl/XrdClPollerFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPollerFactory.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPollerFactory.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPostMaster.cc` & `xrootd-5.6.1/src/XrdCl/XrdClPostMaster.cc`

 * *Files 1% similar despite different names*

```diff
@@ -241,19 +241,23 @@
   // Query the transport handler
   //----------------------------------------------------------------------------
   Status PostMaster::QueryTransport( const URL &url,
                                      uint16_t   query,
                                      AnyObject &result )
   {
     XrdSysRWLockHelper scopedLock( pImpl->pDisconnectLock );
-    PostMasterImpl::ChannelMap::iterator it =
-        pImpl->pChannelMap.find( url.GetChannelId() );
-    if( it == pImpl->pChannelMap.end() )
-      return Status( stError, errInvalidOp );
-    Channel *channel = it->second;
+    Channel *channel = 0;
+    {
+      XrdSysMutexHelper scopedLock2( pImpl->pChannelMapMutex );
+      PostMasterImpl::ChannelMap::iterator it =
+          pImpl->pChannelMap.find( url.GetChannelId() );
+      if( it == pImpl->pChannelMap.end() )
+        return Status( stError, errInvalidOp );
+      channel = it->second;
+    }
 
     if( !channel )
       return Status( stError, errNotSupported );
 
     return channel->QueryTransport( query, result );
   }
```

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPostMaster.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPostMaster.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPostMasterInterfaces.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPostMasterInterfaces.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClPropertyList.hh` & `xrootd-5.6.1/src/XrdCl/XrdClPropertyList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClRedirectorRegistry.cc` & `xrootd-5.6.1/src/XrdCl/XrdClRedirectorRegistry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClRedirectorRegistry.hh` & `xrootd-5.6.1/src/XrdCl/XrdClRedirectorRegistry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClRequestSync.hh` & `xrootd-5.6.1/src/XrdCl/XrdClRequestSync.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClResponseJob.hh` & `xrootd-5.6.1/src/XrdCl/XrdClResponseJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClSIDManager.cc` & `xrootd-5.6.1/src/XrdCl/XrdClSIDManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClSIDManager.hh` & `xrootd-5.6.1/src/XrdCl/XrdClSIDManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClSocket.cc` & `xrootd-5.6.1/src/XrdCl/XrdClSocket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClSocket.hh` & `xrootd-5.6.1/src/XrdCl/XrdClSocket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClStatus.cc` & `xrootd-5.6.1/src/XrdCl/XrdClStatus.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClStatus.hh` & `xrootd-5.6.1/src/XrdCl/XrdClStatus.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClStream.cc` & `xrootd-5.6.1/src/XrdCl/XrdClStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClStream.hh` & `xrootd-5.6.1/src/XrdCl/XrdClStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClSyncQueue.hh` & `xrootd-5.6.1/src/XrdCl/XrdClSyncQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTPFallBackCopyJob.cc` & `xrootd-5.6.1/src/XrdCl/XrdClTPFallBackCopyJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTPFallBackCopyJob.hh` & `xrootd-5.6.1/src/XrdCl/XrdClTPFallBackCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTaskManager.cc` & `xrootd-5.6.1/src/XrdCl/XrdClTaskManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTaskManager.hh` & `xrootd-5.6.1/src/XrdCl/XrdClTaskManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClThirdPartyCopyJob.cc` & `xrootd-5.6.1/src/XrdCl/XrdClThirdPartyCopyJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClThirdPartyCopyJob.hh` & `xrootd-5.6.1/src/XrdCl/XrdClThirdPartyCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTls.cc` & `xrootd-5.6.1/src/XrdCl/XrdClTls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTls.hh` & `xrootd-5.6.1/src/XrdCl/XrdClTls.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTransportManager.cc` & `xrootd-5.6.1/src/XrdCl/XrdClTransportManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClTransportManager.hh` & `xrootd-5.6.1/src/XrdCl/XrdClTransportManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClURL.cc` & `xrootd-5.6.1/src/XrdCl/XrdClURL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClURL.hh` & `xrootd-5.6.1/src/XrdCl/XrdClURL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClUtils.cc` & `xrootd-5.6.1/src/XrdCl/XrdClUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClUtils.hh` & `xrootd-5.6.1/src/XrdCl/XrdClUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXCpCtx.cc` & `xrootd-5.6.1/src/XrdCl/XrdClXCpCtx.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXCpCtx.hh` & `xrootd-5.6.1/src/XrdCl/XrdClXCpCtx.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXCpSrc.cc` & `xrootd-5.6.1/src/XrdCl/XrdClXCpSrc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXCpSrc.hh` & `xrootd-5.6.1/src/XrdCl/XrdClXCpSrc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXRootDMsgHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClXRootDMsgHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXRootDMsgHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClXRootDMsgHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXRootDResponses.cc` & `xrootd-5.6.1/src/XrdCl/XrdClXRootDResponses.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXRootDResponses.hh` & `xrootd-5.6.1/src/XrdCl/XrdClXRootDResponses.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXRootDTransport.cc` & `xrootd-5.6.1/src/XrdCl/XrdClXRootDTransport.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClXRootDTransport.hh` & `xrootd-5.6.1/src/XrdCl/XrdClXRootDTransport.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClZipArchive.cc` & `xrootd-5.6.1/src/XrdCl/XrdClZipArchive.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClZipArchive.hh` & `xrootd-5.6.1/src/XrdCl/XrdClZipArchive.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClZipCache.hh` & `xrootd-5.6.1/src/XrdCl/XrdClZipCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClZipListHandler.cc` & `xrootd-5.6.1/src/XrdCl/XrdClZipListHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClZipListHandler.hh` & `xrootd-5.6.1/src/XrdCl/XrdClZipListHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCl/XrdClZipOperations.hh` & `xrootd-5.6.1/src/XrdCl/XrdClZipOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpFilePlugIn.cc` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpFilePlugIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpFilePlugIn.hh` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpFilePlugIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpPlugInFactory.cc` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpPlugInFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpPosix.cc` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdClHttp/XrdClHttpPosix.hh` & `xrootd-5.6.1/src/XrdClHttp/XrdClHttpPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsAdmin.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsAdmin.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsBaseFS.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsBaseFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsBaseFS.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsBaseFS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsBlackList.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsBlackList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsBlackList.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsBlackList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsCache.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsCache.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClient.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClient.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsClient.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClientConfig.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsClientConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClientConfig.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsClientConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClientMan.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsClientMan.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClientMan.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsClientMan.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClientMsg.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsClientMsg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClientMsg.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsClientMsg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClustID.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsClustID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsClustID.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsClustID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsCluster.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsCluster.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsCluster.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsCluster.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsConfig.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsConfig.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsFinder.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsFinder.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsFinder.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsFinder.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsJob.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsJob.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsKey.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsKey.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsKey.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsKey.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsLogin.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsLogin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsLogin.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsLogin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsManList.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsManList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsManList.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsManList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsManTree.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsManTree.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsManTree.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsManTree.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsManager.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsManager.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsMeter.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsMeter.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsMeter.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsMeter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsNash.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsNash.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsNash.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsNash.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsNode.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsNode.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsNode.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsNode.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPList.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsPList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPList.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsPList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsParser.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsParser.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsParser.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsParser.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPerfMon.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsPerfMon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPrepArgs.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsPrepArgs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPrepArgs.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsPrepArgs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPrepare.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsPrepare.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsPrepare.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsPrepare.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsProtocol.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsProtocol.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsProtocol.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRRData.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsRRData.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRRData.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsRRData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRRQ.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsRRQ.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRRQ.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsRRQ.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRTable.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsRTable.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRTable.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsRTable.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRedirLocal.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsRedirLocal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRedirLocal.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsRedirLocal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsResp.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsResp.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsResp.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsResp.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRole.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsRole.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRouting.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsRouting.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsRouting.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsRouting.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsSecurity.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsSecurity.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsSelect.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsSelect.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsState.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsState.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsState.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsState.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsSupervisor.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsSupervisor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsSupervisor.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsSupervisor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsTalk.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsTalk.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsTalk.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsTalk.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsTrace.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsTypes.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsTypes.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsUtils.cc` & `xrootd-5.6.1/src/XrdCms/XrdCmsUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsUtils.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCms/XrdCmsVnId.hh` & `xrootd-5.6.1/src/XrdCms/XrdCmsVnId.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoAux.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoAux.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoBasic.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoBasic.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoBasic.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoBasic.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoCipher.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoCipher.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoCipher.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoCipher.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoFactory.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoFactory.cc`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 #include "XrdCrypto/XrdCryptoAux.hh"
 #include "XrdCrypto/XrdCryptoTrace.hh"
 #include "XrdCrypto/XrdCryptoFactory.hh"
 
 #include "XrdOuc/XrdOucHash.hh"
 #include "XrdOuc/XrdOucPinLoader.hh"
 #include "XrdSys/XrdSysPlatform.hh"
+#include "XrdSys/XrdSysPthread.hh"
 
 #include "XrdVersion.hh"
   
 //
 // For error logging
 static XrdSysError eDest(0,"cryptofactory_");
 
@@ -414,22 +415,27 @@
 
 //____________________________________________________________________________
 XrdCryptoFactory *XrdCryptoFactory::GetCryptoFactory(const char *factoryid)
 {
    // Static method to load/locate the crypto factory named factoryid
  
    static XrdVERSIONINFODEF(myVer,cryptoloader,XrdVNUMBER,XrdVERSION);
+   static XrdSysMutex    fMutex;
    static FactoryEntry  *factorylist = 0;
    static int            factorynum = 0;
    static XrdOucHash<XrdOucPinLoader> plugins;
    XrdCryptoFactory     *(*efact)();
    XrdCryptoFactory *factory;
    char factobjname[80], libfn[80];
    EPNAME("Factory::GetCryptoFactory");
 
+   // Factory entries are tracked in a static list.
+   // Make sure only one thread may be using or modifying the list at a time.
+   XrdSysMutexHelper mHelp(fMutex);
+
    //
    // The id must be defined
    if (!factoryid) {
       PRINT("crypto factory ID (NULL) undefined");
       return 0;
    }
    if (!strlen(factoryid)) {
```

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoFactory.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoFactory.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoLite.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoLite.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoLite.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoLite.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoLite_bf32.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoLite_bf32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoMsgDigest.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoMsgDigest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoMsgDigest.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoMsgDigest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoRSA.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoRSA.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoRSA.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoRSA.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoTrace.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Chain.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Chain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Chain.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Chain.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Crl.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Crl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Crl.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Crl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Req.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Req.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptoX509Req.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptoX509Req.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptogsiX509Chain.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptogsiX509Chain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptogsiX509Chain.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptogsiX509Chain.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslAux.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslAux.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslCipher.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslCipher.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslCipher.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslCipher.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslFactory.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslFactory.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslFactory.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslMsgDigest.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslMsgDigest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslMsgDigest.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslMsgDigest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslRSA.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslRSA.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslRSA.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslRSA.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslTrace.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Crl.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Crl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Crl.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Crl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Req.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Req.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslX509Req.hh` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslX509Req.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptosslgsiAux.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptosslgsiAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto/XrdCryptotest.cc` & `xrootd-5.6.1/src/XrdCrypto/XrdCryptotest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdCrypto.cmake` & `xrootd-5.6.1/src/XrdCrypto.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDaemons.cmake` & `xrootd-5.6.1/src/XrdDaemons.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDig/XrdDigAuth.cc` & `xrootd-5.6.1/src/XrdDig/XrdDigAuth.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDig/XrdDigAuth.hh` & `xrootd-5.6.1/src/XrdDig/XrdDigAuth.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDig/XrdDigConfig.cc` & `xrootd-5.6.1/src/XrdDig/XrdDigConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDig/XrdDigConfig.hh` & `xrootd-5.6.1/src/XrdDig/XrdDigConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDig/XrdDigFS.cc` & `xrootd-5.6.1/src/XrdDig/XrdDigFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdDig/XrdDigFS.hh` & `xrootd-5.6.1/src/XrdDig/XrdDigFS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/CMakeLists.txt` & `xrootd-5.6.1/src/XrdEc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/README` & `xrootd-5.6.1/src/XrdEc/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcConfig.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcObjCfg.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcObjCfg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcReader.cc` & `xrootd-5.6.1/src/XrdEc/XrdEcReader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcReader.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcRedundancyProvider.cc` & `xrootd-5.6.1/src/XrdEc/XrdEcRedundancyProvider.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcRedundancyProvider.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcRedundancyProvider.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcStrmWriter.cc` & `xrootd-5.6.1/src/XrdEc/XrdEcStrmWriter.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcStrmWriter.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcStrmWriter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcThreadPool.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcThreadPool.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcUtilities.cc` & `xrootd-5.6.1/src/XrdEc/XrdEcUtilities.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcUtilities.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcUtilities.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdEc/XrdEcWrtBuff.hh` & `xrootd-5.6.1/src/XrdEc/XrdEcWrtBuff.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/README` & `xrootd-5.6.1/src/XrdFfs/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsDent.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsDent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsDent.hh` & `xrootd-5.6.1/src/XrdFfs/XrdFfsDent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsFsinfo.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsFsinfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsFsinfo.hh` & `xrootd-5.6.1/src/XrdFfs/XrdFfsFsinfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsMisc.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsMisc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsMisc.hh` & `xrootd-5.6.1/src/XrdFfs/XrdFfsMisc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsPosix.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsPosix.hh` & `xrootd-5.6.1/src/XrdFfs/XrdFfsPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsQueue.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsQueue.hh` & `xrootd-5.6.1/src/XrdFfs/XrdFfsQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsWcache.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsWcache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsWcache.hh` & `xrootd-5.6.1/src/XrdFfs/XrdFfsWcache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/XrdFfsXrootdfs.cc` & `xrootd-5.6.1/src/XrdFfs/XrdFfsXrootdfs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs/xrootdfs.template` & `xrootd-5.6.1/src/XrdFfs/xrootdfs.template`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFfs.cmake` & `xrootd-5.6.1/src/XrdFfs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcCID.cc` & `xrootd-5.6.1/src/XrdFrc/XrdFrcCID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcCID.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcCID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcProxy.cc` & `xrootd-5.6.1/src/XrdFrc/XrdFrcProxy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcProxy.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcProxy.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcReqAgent.cc` & `xrootd-5.6.1/src/XrdFrc/XrdFrcReqAgent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcReqAgent.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcReqAgent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcReqFile.cc` & `xrootd-5.6.1/src/XrdFrc/XrdFrcReqFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcReqFile.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcReqFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcRequest.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcRequest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcTrace.cc` & `xrootd-5.6.1/src/XrdFrc/XrdFrcTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcTrace.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcUtils.cc` & `xrootd-5.6.1/src/XrdFrc/XrdFrcUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcUtils.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcXAttr.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrc/XrdFrcXLock.hh` & `xrootd-5.6.1/src/XrdFrc/XrdFrcXLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdmin.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdmin.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminAudit.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminAudit.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminFiles.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminFiles.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminFind.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminFind.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminMain.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminQuery.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminQuery.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminReloc.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminReloc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmAdminUnlink.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmAdminUnlink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmCns.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmCns.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmCns.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmCns.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmConfig.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmConfig.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmFiles.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmFiles.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmFiles.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmFiles.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmMigrate.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmMigrate.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmMigrate.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmMigrate.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmMonitor.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmMonitor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmMonitor.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmPurgMain.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmPurgMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmPurge.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmPurge.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmPurge.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmPurge.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmReqBoss.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmReqBoss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmReqBoss.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmReqBoss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmTSort.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmTSort.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmTSort.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmTSort.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmTransfer.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmTransfer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmTransfer.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmTransfer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrAgent.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrAgent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrAgent.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrAgent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrDaemon.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrDaemon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrDaemon.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrDaemon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrJob.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrMain.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrQueue.cc` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm/XrdFrmXfrQueue.hh` & `xrootd-5.6.1/src/XrdFrm/XrdFrmXfrQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdFrm.cmake` & `xrootd-5.6.1/src/XrdFrm.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHeaders.cmake` & `xrootd-5.6.1/src/XrdHeaders.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/README-CKSUM.md` & `xrootd-5.6.1/src/XrdHttp/README-CKSUM.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpChecksum.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpChecksum.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpChecksum.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpChecksum.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpChecksumHandler.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpChecksumHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpChecksumHandler.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpChecksumHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpExtHandler.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpExtHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpExtHandler.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpExtHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpModule.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpModule.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpProtocol.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpProtocol.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpProtocol.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpReq.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpReq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpReq.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpReq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpSecXtractor.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpSecXtractor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpSecurity.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpStatic.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpStatic.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpTrace.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpUtils.cc` & `xrootd-5.6.1/src/XrdHttp/XrdHttpUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/XrdHttpUtils.hh` & `xrootd-5.6.1/src/XrdHttp/XrdHttpUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/static/favicon.ico` & `xrootd-5.6.1/src/XrdHttp/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/static/xrdhttp.css` & `xrootd-5.6.1/src/XrdHttp/static/xrdhttp.css`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/static/xrdhttp_css.h` & `xrootd-5.6.1/src/XrdHttp/static/xrdhttp_css.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/static/xrdhttp_favicon_ico.h` & `xrootd-5.6.1/src/XrdHttp/static/xrdhttp_favicon_ico.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/xrootd-http-rdr.cf` & `xrootd-5.6.1/src/XrdHttp/xrootd-http-rdr.cf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp/xrootd-http.cf` & `xrootd-5.6.1/src/XrdHttp/xrootd-http.cf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdHttp.cmake` & `xrootd-5.6.1/src/XrdHttp.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdIsal.cmake` & `xrootd-5.6.1/src/XrdIsal.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/README.md` & `xrootd-5.6.1/src/XrdMacaroons/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/XrdMacaroons.cc` & `xrootd-5.6.1/src/XrdMacaroons/XrdMacaroons.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsAuthz.cc` & `xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsAuthz.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsAuthz.hh` & `xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsAuthz.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsConfigure.cc` & `xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsConfigure.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsHandler.cc` & `xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/XrdMacaroonsHandler.hh` & `xrootd-5.6.1/src/XrdMacaroons/XrdMacaroonsHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons/macaroon-init` & `xrootd-5.6.1/src/XrdMacaroons/macaroon-init`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdMacaroons.cmake` & `xrootd-5.6.1/src/XrdMacaroons.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNet.cc` & `xrootd-5.6.1/src/XrdNet/XrdNet.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNet.hh` & `xrootd-5.6.1/src/XrdNet/XrdNet.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetAddr.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetAddr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetAddr.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetAddr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetAddrInfo.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetAddrInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetAddrInfo.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetAddrInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetBuffer.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetBuffer.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetCache.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetCache.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetCmsNotify.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetCmsNotify.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetCmsNotify.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetCmsNotify.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetConnect.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetConnect.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetConnect.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetConnect.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetIF.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetIF.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetIF.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetIF.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetIdentity.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetIdentity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetIdentity.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetIdentity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetMsg.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetMsg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetMsg.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetMsg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetOpts.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetOpts.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPMark.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetPMark.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPMark.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetPMark.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPMarkCfg.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetPMarkCfg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPMarkCfg.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetPMarkCfg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPMarkFF.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetPMarkFF.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPMarkFF.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetPMarkFF.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetPeer.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetPeer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetRegistry.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetRegistry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetRegistry.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetRegistry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetSecurity.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetSecurity.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetSockAddr.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetSockAddr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetSocket.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetSocket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetSocket.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetSocket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetUtils.cc` & `xrootd-5.6.1/src/XrdNet/XrdNetUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdNet/XrdNetUtils.hh` & `xrootd-5.6.1/src/XrdNet/XrdNetUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfs.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfs.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsCPFile.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsCPFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsCPFile.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsCPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsChkPnt.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsChkPnt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsChkPnt.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsChkPnt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsConfig.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsConfigCP.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsConfigCP.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsConfigCP.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsConfigCP.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsConfigPI.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsConfigPI.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsConfigPI.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsConfigPI.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsEvr.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsEvr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsEvr.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsEvr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsEvs.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsEvs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsEvs.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsEvs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsFAttr.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsFAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsFS.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsFSctl.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsFSctl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsFSctl_PI.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsFSctl_PI.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsHandle.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsHandle.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsHandle.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsHandle.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsPoscq.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsPoscq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsPoscq.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsPoscq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsPrepGPI.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsPrepGPI.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsPrepare.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsPrepare.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsSecurity.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsStats.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsStats.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPC.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPC.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCAuth.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCAuth.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCAuth.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCAuth.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCConfig.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCInfo.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCInfo.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCJob.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCJob.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCProg.cc` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCProg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTPCProg.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTPCProg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOfs/XrdOfsTrace.hh` & `xrootd-5.6.1/src/XrdOfs/XrdOfsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOss.cc` & `xrootd-5.6.1/src/XrdOss/XrdOss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOss.hh` & `xrootd-5.6.1/src/XrdOss/XrdOss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssAio.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssApi.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssApi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssApi.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssApi.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssAt.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssAt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssAt.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssAt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssCache.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssCache.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssConfig.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssConfig.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssCopy.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssCopy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssCopy.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssCopy.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssCreate.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssCreate.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssDefaultSS.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssDefaultSS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssError.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssError.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssMSS.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssMSS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssMio.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssMio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssMio.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssMio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssMioFile.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssMioFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssOpaque.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssOpaque.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssPath.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssPath.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssPath.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssReloc.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssReloc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssRename.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssRename.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssSIgpfsT.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssSIgpfsT.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssSpace.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssSpace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssSpace.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssSpace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssStage.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssStage.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssStage.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssStage.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssStat.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssStat.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssStatInfo.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssStatInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssTrace.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssUnlink.cc` & `xrootd-5.6.1/src/XrdOss/XrdOssUnlink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssVS.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssVS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOss/XrdOssWrapper.hh` & `xrootd-5.6.1/src/XrdOss/XrdOssWrapper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/README.md` & `xrootd-5.6.1/src/XrdOssCsi/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsi.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsi.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsi.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiConfig.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiConfig.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiCrcUtils.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiCrcUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiCrcUtils.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiCrcUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiFile.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiFileAio.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiFileAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiFileAio.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiFileAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiPages.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiPages.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiPages.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiPages.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiRanges.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiRanges.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiRanges.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiRanges.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTagstore.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTagstore.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssCsiTrace.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssCsiTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi/XrdOssHandler.hh` & `xrootd-5.6.1/src/XrdOssCsi/XrdOssHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOssCsi.cmake` & `xrootd-5.6.1/src/XrdOssCsi.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/README.bonjour` & `xrootd-5.6.1/src/XrdOuc/README.bonjour`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucArgs.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucArgs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucArgs.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucArgs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucBackTrace.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucBackTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucBackTrace.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucBackTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucBuffer.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucBuffer.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCRC.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucCRC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCRC.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCRC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCRC32C.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucCRC32C.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCRC32C.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCRC32C.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCache.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCache.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCacheCM.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCacheCM.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCacheStats.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCacheStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCallBack.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucCallBack.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCallBack.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCallBack.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucChain.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucChain.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucChkPnt.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucChkPnt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucCompiler.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucCompiler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucDLlist.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucDLlist.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucERoute.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucERoute.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucERoute.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucERoute.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucEnum.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucEnum.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucEnv.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucEnv.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucErrInfo.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucErrInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucExport.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucExport.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucExport.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucExport.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucFileInfo.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucFileInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucFileInfo.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucFileInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucGMap.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucGMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucGMap.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucGMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucGatherConf.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucGatherConf.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucGatherConf.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucGatherConf.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucHash.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucHash.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucHash.icc` & `xrootd-5.6.1/src/XrdOuc/XrdOucHash.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucHashVal.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucHashVal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucIOVec.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucIOVec.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucJson.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucJson.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucLock.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucLogging.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucLogging.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucLogging.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucLogging.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucMapP2X.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucMapP2X.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucMsubs.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucMsubs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucMsubs.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucMsubs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucN2NLoader.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucN2NLoader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucN2NLoader.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucN2NLoader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucN2No2p.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucN2No2p.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucNList.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucNList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucNList.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucNList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucNSWalk.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucNSWalk.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucNSWalk.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucNSWalk.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucName2Name.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucName2Name.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucName2Name.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucName2Name.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPList.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPgrwUtils.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucPgrwUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPgrwUtils.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPgrwUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPinKing.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPinKing.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPinLoader.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucPinLoader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPinLoader.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPinLoader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPinObject.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPinObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPinPath.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucPinPath.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPinPath.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPinPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPreload.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucPreload.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPreload.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPreload.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucProg.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucProg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucProg.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucProg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPsx.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucPsx.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPsx.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPsx.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPup.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucPup.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucPup.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucPup.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucRash.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucRash.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucRash.icc` & `xrootd-5.6.1/src/XrdOuc/XrdOucRash.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucReqID.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucReqID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucReqID.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucReqID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSFVec.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucSFVec.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSHA3.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucSHA3.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSHA3.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucSHA3.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSid.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucSid.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSid.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucSid.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSiteName.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucSiteName.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSiteName.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucSiteName.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucStats.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucStream.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucStream.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucString.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucString.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucString.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucString.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSxeq.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucSxeq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucSxeq.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucSxeq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTList.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucTList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTPC.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucTPC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTPC.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucTPC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTUtils.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucTUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTable.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucTable.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTokenizer.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucTokenizer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTokenizer.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucTokenizer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTrace.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucTrace.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucUri.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucUri.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucUri.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucUri.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucUtils.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucUtils.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucVerName.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOucVerName.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucVerName.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucVerName.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOucXAttr.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOucXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOuca2x.cc` & `xrootd-5.6.1/src/XrdOuc/XrdOuca2x.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdOuc/XrdOuca2x.hh` & `xrootd-5.6.1/src/XrdOuc/XrdOuca2x.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/README` & `xrootd-5.6.1/src/XrdPfc/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfc.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfc.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcAllowDecision.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcAllowDecision.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcBlacklistDecision.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcBlacklistDecision.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcCommand.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcCommand.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcConfiguration.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcConfiguration.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcDecision.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcDecision.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcFSctl.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcFSctl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcFSctl.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcFSctl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcFile.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcFile.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcIO.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcIO.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcIO.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcIO.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcIOFile.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcIOFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcIOFile.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcIOFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcIOFileBlock.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcIOFileBlock.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcIOFileBlock.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcIOFileBlock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcInfo.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcInfo.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcPrint.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcPrint.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcPrint.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcPrint.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcPurge.cc` & `xrootd-5.6.1/src/XrdPfc/XrdPfcPurge.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcStats.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcTrace.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc/XrdPfcTypes.hh` & `xrootd-5.6.1/src/XrdPfc/XrdPfcTypes.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPfc.cmake` & `xrootd-5.6.1/src/XrdPfc.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPlugins.cmake` & `xrootd-5.6.1/src/XrdPlugins.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/README` & `xrootd-5.6.1/src/XrdPosix/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosix.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosix.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixAdmin.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixAdmin.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixCache.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixCache.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixCallBack.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixCallBack.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixCallBack.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixCallBack.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixConfig.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixConfig.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixDir.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixDir.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixExtern.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixExtern.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixExtra.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixExtra.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixExtra.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixExtra.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixFile.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixFile.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixFileRH.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixFileRH.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixFileRH.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixFileRH.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixInfo.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixLinkage.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixLinkage.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixLinkage.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixLinkage.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixMap.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixMap.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixObjGuard.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixObjGuard.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixObject.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixObject.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixObject.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixOsDep.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixOsDep.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixPreload.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixPreload.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixPreload32.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixPreload32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixPrepIO.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixPrepIO.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixPrepIO.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixPrepIO.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixStats.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixTrace.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixXrootd.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixXrootd.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixXrootd.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixXrootd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixXrootdPath.cc` & `xrootd-5.6.1/src/XrdPosix/XrdPosixXrootdPath.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix/XrdPosixXrootdPath.hh` & `xrootd-5.6.1/src/XrdPosix/XrdPosixXrootdPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPosix.cmake` & `xrootd-5.6.1/src/XrdPosix.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPss.cc` & `xrootd-5.6.1/src/XrdPss/XrdPss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPss.hh` & `xrootd-5.6.1/src/XrdPss/XrdPss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssAio.cc` & `xrootd-5.6.1/src/XrdPss/XrdPssAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssAioCB.cc` & `xrootd-5.6.1/src/XrdPss/XrdPssAioCB.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssAioCB.hh` & `xrootd-5.6.1/src/XrdPss/XrdPssAioCB.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssCks.cc` & `xrootd-5.6.1/src/XrdPss/XrdPssCks.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssCks.hh` & `xrootd-5.6.1/src/XrdPss/XrdPssCks.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssConfig.cc` & `xrootd-5.6.1/src/XrdPss/XrdPssConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssTrace.hh` & `xrootd-5.6.1/src/XrdPss/XrdPssTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssUrlInfo.cc` & `xrootd-5.6.1/src/XrdPss/XrdPssUrlInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssUrlInfo.hh` & `xrootd-5.6.1/src/XrdPss/XrdPssUrlInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssUtils.cc` & `xrootd-5.6.1/src/XrdPss/XrdPssUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdPss/XrdPssUtils.hh` & `xrootd-5.6.1/src/XrdPss/XrdPssUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmc.cc` & `xrootd-5.6.1/src/XrdRmc/XrdRmc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmc.hh` & `xrootd-5.6.1/src/XrdRmc/XrdRmc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmcData.cc` & `xrootd-5.6.1/src/XrdRmc/XrdRmcData.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmcData.hh` & `xrootd-5.6.1/src/XrdRmc/XrdRmcData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmcReal.cc` & `xrootd-5.6.1/src/XrdRmc/XrdRmcReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmcReal.hh` & `xrootd-5.6.1/src/XrdRmc/XrdRmcReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdRmc/XrdRmcSlot.hh` & `xrootd-5.6.1/src/XrdRmc/XrdRmcSlot.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/LICENSE` & `xrootd-5.6.1/src/XrdSciTokens/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/README.md` & `xrootd-5.6.1/src/XrdSciTokens/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensAccess.cc` & `xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensAccess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensHelper.hh` & `xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensHelper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensMon.cc` & `xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensMon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/XrdSciTokensMon.hh` & `xrootd-5.6.1/src/XrdSciTokens/XrdSciTokensMon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/configs/scitokens.cfg` & `xrootd-5.6.1/src/XrdSciTokens/configs/scitokens.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/test/config/xrootd-http.cfg` & `xrootd-5.6.1/src/XrdSciTokens/test/config/xrootd-http.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/test/create-pubkey.py` & `xrootd-5.6.1/src/XrdSciTokens/test/create-pubkey.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/test/openssl-selfsigned.conf` & `xrootd-5.6.1/src/XrdSciTokens/test/openssl-selfsigned.conf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/test/setup_tests.sh` & `xrootd-5.6.1/src/XrdSciTokens/test/setup_tests.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/test/test_inside_docker.sh` & `xrootd-5.6.1/src/XrdSciTokens/test/test_inside_docker.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/inih/INIReader.h` & `xrootd-5.6.1/src/XrdSciTokens/vendor/inih/INIReader.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp` & `xrootd-5.6.1/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/inih/LICENSE.txt` & `xrootd-5.6.1/src/XrdSciTokens/vendor/inih/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/inih/README.md` & `xrootd-5.6.1/src/XrdSciTokens/vendor/inih/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/Changes` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/Changes`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/LICENSE` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/README.mkdn` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/README.mkdn`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/iostream.cc` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/iostream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/examples/streaming.cc` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/examples/streaming.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picojson.h` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picojson.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picotest/picotest.c` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picotest/picotest.c`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/picotest/picotest.h` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/picotest/picotest.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens/vendor/picojson/test.cc` & `xrootd-5.6.1/src/XrdSciTokens/vendor/picojson/test.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSciTokens.cmake` & `xrootd-5.6.1/src/XrdSciTokens.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecAttr.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecClient.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntity.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecEntity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntity.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecEntity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntityAttr.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecEntityAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntityAttr.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecEntityAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntityPin.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecEntityPin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntityXtra.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecEntityXtra.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecEntityXtra.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecEntityXtra.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecInterface.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecInterface.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecLoadSecurity.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecLoadSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecLoadSecurity.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecLoadSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecMonitor.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecPManager.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecPManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecPManager.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecPManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecProtect.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecProtect.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecProtect.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecProtect.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecProtector.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecProtector.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecProtector.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecProtector.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecProtocolhost.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecProtocolhost.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecProtocolhost.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecProtocolhost.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecServer.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecServer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecServer.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecServer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecTLayer.cc` & `xrootd-5.6.1/src/XrdSec/XrdSecTLayer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecTLayer.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecTLayer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSecTrace.hh` & `xrootd-5.6.1/src/XrdSec/XrdSecTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSectestClient.cc` & `xrootd-5.6.1/src/XrdSec/XrdSectestClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec/XrdSectestServer.cc` & `xrootd-5.6.1/src/XrdSec/XrdSectestServer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSec.cmake` & `xrootd-5.6.1/src/XrdSec.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecProtocolgsi.cc` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecProtocolgsi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecProtocolgsi.hh` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecProtocolgsi.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiOpts.hh` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiOpts.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiProxy.cc` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiProxy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsiTrace.hh` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsiTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi/XrdSecgsitest.cc` & `xrootd-5.6.1/src/XrdSecgsi/XrdSecgsitest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecgsi.cmake` & `xrootd-5.6.1/src/XrdSecgsi.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSeckrb5/XrdSecProtocolkrb5.cc` & `xrootd-5.6.1/src/XrdSeckrb5/XrdSecProtocolkrb5.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSeckrb5.cmake` & `xrootd-5.6.1/src/XrdSeckrb5.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecpwd/XrdSecProtocolpwd.cc` & `xrootd-5.6.1/src/XrdSecpwd/XrdSecProtocolpwd.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecpwd/XrdSecProtocolpwd.hh` & `xrootd-5.6.1/src/XrdSecpwd/XrdSecProtocolpwd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecpwd/XrdSecpwdPlatform.hh` & `xrootd-5.6.1/src/XrdSecpwd/XrdSecpwdPlatform.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc` & `xrootd-5.6.1/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecpwd/XrdSecpwdTrace.hh` & `xrootd-5.6.1/src/XrdSecpwd/XrdSecpwdTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecProtocolsss.cc` & `xrootd-5.6.1/src/XrdSecsss/XrdSecProtocolsss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecProtocolsss.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecProtocolsss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssAdmin.cc` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssCon.cc` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssCon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssCon.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssCon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssEnt.cc` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssEnt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssEnt.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssEnt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssID.cc` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssID.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssKT.cc` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssKT.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssKT.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssKT.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssMap.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecsss/XrdSecsssRR.hh` & `xrootd-5.6.1/src/XrdSecsss/XrdSecsssRR.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecunix/XrdSecProtocolunix.cc` & `xrootd-5.6.1/src/XrdSecunix/XrdSecProtocolunix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecztn/XrdSecProtocolztn.cc` & `xrootd-5.6.1/src/XrdSecztn/XrdSecProtocolztn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecztn/XrdSecztn.cc` & `xrootd-5.6.1/src/XrdSecztn/XrdSecztn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSecztn.cmake` & `xrootd-5.6.1/src/XrdSecztn.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdServer.cmake` & `xrootd-5.6.1/src/XrdServer.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsAio.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsDio.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsDio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsFAttr.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsFAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsFlags.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsFlags.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsGPFile.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsGPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsInterface.cc` & `xrootd-5.6.1/src/XrdSfs/XrdSfsInterface.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsInterface.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsInterface.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsNative.cc` & `xrootd-5.6.1/src/XrdSfs/XrdSfsNative.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsNative.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsNative.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsXio.cc` & `xrootd-5.6.1/src/XrdSfs/XrdSfsXio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsXio.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsXio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSfs/XrdSfsXioImpl.hh` & `xrootd-5.6.1/src/XrdSfs/XrdSfsXioImpl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiAlert.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiAlert.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiAlert.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiAlert.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiAtomics.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiAtomics.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiAtomics.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiAtomics.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiBVec.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiBVec.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiClient.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiCluster.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiCluster.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiCms.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiCms.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiCms.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiCms.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiDir.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiDir.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiEntity.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiEntity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiErrInfo.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiErrInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiErrInfo.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiErrInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiEvent.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiEvent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiEvent.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiEvent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFile.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFile.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFileReq.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFileReq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFileReq.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFileReq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFileResource.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFileResource.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFileResource.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFileResource.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFileSess.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFileSess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiFileSess.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiFileSess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiLogger.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiLogger.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiLogger.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiLogger.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiLogging.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiLogging.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiProvider.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiProvider.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiRRAgent.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiRRAgent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiRRInfo.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiRRInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiRRTable.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiRRTable.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiRequest.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiRequest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiRequest.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiRequest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiResource.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiResource.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiRespInfo.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiRespInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiResponder.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiResponder.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiResponder.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiResponder.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiScale.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiScale.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiScale.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiScale.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiServReal.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiServReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiServReal.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiServReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiService.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiService.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiService.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiService.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiSessReal.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiSessReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiSessReal.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiSessReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiSfs.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiSfs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiSfs.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiSfs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiSfsConfig.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiSfsConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiSfsConfig.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiSfsConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiShMam.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiShMam.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiShMam.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiShMam.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiShMap.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiShMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiShMap.icc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiShMap.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiShMat.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiShMat.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiShMat.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiShMat.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiStat.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiStat.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiStats.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiStats.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiStream.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiTaskReal.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiTaskReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiTaskReal.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiTaskReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiTrace.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiUtils.cc` & `xrootd-5.6.1/src/XrdSsi/XrdSsiUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi/XrdSsiUtils.hh` & `xrootd-5.6.1/src/XrdSsi/XrdSsiUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSsi.cmake` & `xrootd-5.6.1/src/XrdSsi.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutAux.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutAux.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutBuckList.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutBuckList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutBuckList.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutBuckList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutBucket.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutBucket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutBucket.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutBucket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutBuffer.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutBuffer.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutCache.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutCacheEntry.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutCacheEntry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutCacheEntry.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutCacheEntry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutPFCache.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutPFCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutPFCache.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutPFCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutPFEntry.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutPFEntry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutPFEntry.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutPFEntry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutPFile.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutPFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutPFile.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutRndm.cc` & `xrootd-5.6.1/src/XrdSut/XrdSutRndm.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutRndm.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutRndm.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSut/XrdSutTrace.hh` & `xrootd-5.6.1/src/XrdSut/XrdSutTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysAtomics.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysAtomics.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysDir.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysDir.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysE2T.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysE2T.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysE2T.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysE2T.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysError.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysError.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysError.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysError.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFAttr.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysFAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFAttr.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysFAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFAttrBsd.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysFAttrBsd.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFAttrLnx.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysFAttrLnx.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFAttrMac.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysFAttrMac.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFAttrSun.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysFAttrSun.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFD.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysFD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFallocate.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysFallocate.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysFallocate.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysFallocate.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysHeaders.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysHeaders.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysIOEvents.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysIOEvents.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysIOEvents.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysIOEvents.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollE.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollE.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollKQ.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollKQ.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollPoll.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollPoll.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysIOEventsPollPort.icc` & `xrootd-5.6.1/src/XrdSys/XrdSysIOEventsPollPort.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysKernelBuffer.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysKernelBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysLogPI.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysLogPI.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysLogger.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysLogger.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysLogger.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysLogger.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysLogging.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysLogging.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysLogging.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysLogging.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPageSize.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysPageSize.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPlatform.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysPlatform.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPlatform.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysPlatform.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPlugin.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPlugin.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPriv.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysPriv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPriv.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysPriv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPthread.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysPthread.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPthread.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysPthread.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysPwd.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysPwd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysRAtomic.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysRAtomic.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysSemWait.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysSemWait.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysShmem.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysShmem.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysTimer.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysTimer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysTimer.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysTimer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysTrace.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysTrace.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysUtils.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysUtils.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysXAttr.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysXAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysXAttr.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysXSLock.cc` & `xrootd-5.6.1/src/XrdSys/XrdSysXSLock.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdSys/XrdSysXSLock.hh` & `xrootd-5.6.1/src/XrdSys/XrdSysXSLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/README` & `xrootd-5.6.1/src/XrdThrottle/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottle.hh` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottle.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottleFile.cc` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottleFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottleFileSystem.cc` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottleFileSystem.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottleFileSystemConfig.cc` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottleFileSystemConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottleManager.cc` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottleManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottleManager.hh` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottleManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdThrottle/XrdThrottleTrace.hh` & `xrootd-5.6.1/src/XrdThrottle/XrdThrottleTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTls.cc` & `xrootd-5.6.1/src/XrdTls/XrdTls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTls.hh` & `xrootd-5.6.1/src/XrdTls/XrdTls.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsContext.cc` & `xrootd-5.6.1/src/XrdTls/XrdTlsContext.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsContext.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsContext.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsHostcheck.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsHostcheck.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsHostcheck.icc` & `xrootd-5.6.1/src/XrdTls/XrdTlsHostcheck.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsNotary.cc` & `xrootd-5.6.1/src/XrdTls/XrdTlsNotary.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsNotary.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsNotary.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsNotaryUtils.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsNotaryUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsNotaryUtils.icc` & `xrootd-5.6.1/src/XrdTls/XrdTlsNotaryUtils.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsPeerCerts.cc` & `xrootd-5.6.1/src/XrdTls/XrdTlsPeerCerts.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsPeerCerts.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsPeerCerts.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsSocket.cc` & `xrootd-5.6.1/src/XrdTls/XrdTlsSocket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsSocket.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsSocket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsTempCA.cc` & `xrootd-5.6.1/src/XrdTls/XrdTlsTempCA.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsTempCA.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsTempCA.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTls/XrdTlsTrace.hh` & `xrootd-5.6.1/src/XrdTls/XrdTlsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/README.md` & `xrootd-5.6.1/src/XrdTpc/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcConfigure.cc` & `xrootd-5.6.1/src/XrdTpc/XrdTpcConfigure.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcCurlMulti.cc` & `xrootd-5.6.1/src/XrdTpc/XrdTpcCurlMulti.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcMultistream.cc` & `xrootd-5.6.1/src/XrdTpc/XrdTpcMultistream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcState.cc` & `xrootd-5.6.1/src/XrdTpc/XrdTpcState.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcState.hh` & `xrootd-5.6.1/src/XrdTpc/XrdTpcState.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcStream.cc` & `xrootd-5.6.1/src/XrdTpc/XrdTpcStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcStream.hh` & `xrootd-5.6.1/src/XrdTpc/XrdTpcStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcTPC.cc` & `xrootd-5.6.1/src/XrdTpc/XrdTpcTPC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/XrdTpcTPC.hh` & `xrootd-5.6.1/src/XrdTpc/XrdTpcTPC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc/xrootd-test-tpc` & `xrootd-5.6.1/src/XrdTpc/xrootd-test-tpc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdTpc.cmake` & `xrootd-5.6.1/src/XrdTpc.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdUtils.cmake` & `xrootd-5.6.1/src/XrdUtils.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVersion.hh.in` & `xrootd-5.6.1/src/XrdVersion.hh.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVersionPlugin.hh` & `xrootd-5.6.1/src/XrdVersionPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/README.md` & `xrootd-5.6.1/src/XrdVoms/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVoms.hh` & `xrootd-5.6.1/src/XrdVoms/XrdVoms.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsFun.cc` & `xrootd-5.6.1/src/XrdVoms/XrdVomsFun.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsFun.hh` & `xrootd-5.6.1/src/XrdVoms/XrdVomsFun.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsHttp.cc` & `xrootd-5.6.1/src/XrdVoms/XrdVomsHttp.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsMapfile.cc` & `xrootd-5.6.1/src/XrdVoms/XrdVomsMapfile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsMapfile.hh` & `xrootd-5.6.1/src/XrdVoms/XrdVomsMapfile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsTrace.hh` & `xrootd-5.6.1/src/XrdVoms/XrdVomsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms/XrdVomsgsi.cc` & `xrootd-5.6.1/src/XrdVoms/XrdVomsgsi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdVoms.cmake` & `xrootd-5.6.1/src/XrdVoms.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlMetaLink.cc` & `xrootd-5.6.1/src/XrdXml/XrdXmlMetaLink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlMetaLink.hh` & `xrootd-5.6.1/src/XrdXml/XrdXmlMetaLink.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlRdrTiny.cc` & `xrootd-5.6.1/src/XrdXml/XrdXmlRdrTiny.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlRdrTiny.hh` & `xrootd-5.6.1/src/XrdXml/XrdXmlRdrTiny.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlRdrXml2.cc` & `xrootd-5.6.1/src/XrdXml/XrdXmlRdrXml2.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlRdrXml2.hh` & `xrootd-5.6.1/src/XrdXml/XrdXmlRdrXml2.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlReader.cc` & `xrootd-5.6.1/src/XrdXml/XrdXmlReader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/XrdXmlReader.hh` & `xrootd-5.6.1/src/XrdXml/XrdXmlReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/tinyxml/tinystr.cpp` & `xrootd-5.6.1/src/XrdXml/tinyxml/tinystr.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/tinyxml/tinystr.h` & `xrootd-5.6.1/src/XrdXml/tinyxml/tinystr.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/tinyxml/tinyxml.cpp` & `xrootd-5.6.1/src/XrdXml/tinyxml/tinyxml.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/tinyxml/tinyxml.h` & `xrootd-5.6.1/src/XrdXml/tinyxml/tinyxml.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/tinyxml/tinyxmlerror.cpp` & `xrootd-5.6.1/src/XrdXml/tinyxml/tinyxmlerror.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml/tinyxml/tinyxmlparser.cpp` & `xrootd-5.6.1/src/XrdXml/tinyxml/tinyxmlparser.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXml.cmake` & `xrootd-5.6.1/src/XrdXml.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAdmin.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAdmin.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioBuff.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioBuff.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioBuff.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioBuff.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioFob.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioFob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioFob.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioFob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioPgrw.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioPgrw.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioPgrw.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioPgrw.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioTask.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioTask.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdAioTask.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdAioTask.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdBridge.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdBridge.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdBridge.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdBridge.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdCallBack.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdCallBack.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdCallBack.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdCallBack.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdConfig.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdConfigMon.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdConfigMon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdFile.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdFile.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileLock.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileLock1.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileLock1.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileLock1.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileLock1.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdFileStats.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdFileStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdGPFile.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdGPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdGSReal.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdGSReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdGSReal.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdGSReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdGStream.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdGStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdGStream.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdGStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdJob.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdJob.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdLoadLib.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdLoadLib.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonData.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFMap.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFMap.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFile.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonFile.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonitor.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonitor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdMonitor.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdNormAio.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdNormAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdNormAio.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdNormAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgrwAio.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgrwAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgrwAio.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgrwAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwBadCS.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwBadCS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwBadCS.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwBadCS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwCtl.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwCtl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwCtl.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwCtl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwFob.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwFob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPgwFob.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPgwFob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPio.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPio.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPlugin.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPrepare.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPrepare.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdPrepare.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdPrepare.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdProtocol.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdProtocol.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdProtocol.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdReqID.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdReqID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdResponse.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdResponse.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdResponse.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdResponse.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdStats.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdStats.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTpcMon.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTpcMon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTpcMon.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTpcMon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTrace.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransPend.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransPend.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransPend.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransPend.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransSend.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransSend.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransSend.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransSend.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransit.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransit.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdTransit.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdTransit.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdWVInfo.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdWVInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdXPath.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdXPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeq.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeq.hh` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeqChkPnt.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeqChkPnt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeqFAttr.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeqFAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdXrootd/XrdXrootdXeqPgrw.cc` & `xrootd-5.6.1/src/XrdXrootd/XrdXrootdXeqPgrw.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipCDFH.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipCDFH.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipDataDescriptor.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipDataDescriptor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipEOCD.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipEOCD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipExtra.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipExtra.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipLFH.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipLFH.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipUtils.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipZIP64EOCD.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipZIP64EOCD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/src/XrdZip/XrdZipZIP64EOCDL.hh` & `xrootd-5.6.1/src/XrdZip/XrdZipZIP64EOCDL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XRootD/CMakeLists.txt` & `xrootd-5.6.1/tests/XRootD/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XRootD/smoke.sh` & `xrootd-5.6.1/tests/XRootD/smoke.sh`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
        REF32C=$(${CRC32C} < ${TMPDIR}/${i}.ref | cut -d' '  -f1)
        NEW32C=$(${CRC32C} < ${TMPDIR}/${i}.dat | cut -d' '  -f1)
        SRV32C=$(${XRDFS} ${HOST} query checksum ${TMPDIR}/${i}.ref?cks.type=crc32c | cut -d' ' -f2)
 
        REFA32=$(${ADLER32} < ${TMPDIR}/${i}.ref | cut -d' '  -f1)
        NEWA32=$(${ADLER32} < ${TMPDIR}/${i}.dat | cut -d' '  -f1)
        SRVA32=$(${XRDFS} ${HOST} query checksum ${TMPDIR}/${i}.ref?cks.type=adler32 | cut -d' ' -f2)
-       echo "${i}:  crc32c: reference: ${REF32C}, server: ${SRV32C}, downloaded: ${REFA32}"
-       echo "${i}: adler32: reference: ${NEW32C}, server: ${SRVA32}, downloaded: ${NEWA32}"
+       echo "${i}:  crc32c: reference: ${REF32C}, server: ${SRV32C}, downloaded: ${REF32C}"
+       echo "${i}: adler32: reference: ${NEWA32}, server: ${SRVA32}, downloaded: ${NEWA32}"
 
        if [[ "${NEWA32}" != "${REFA32}" || "${SRVA32}" != "${REFA32}" ]]; then
                echo 1>&2 "$(basename $0): error: adler32 checksum check failed for file: ${i}.dat"
                exit 1
        fi
        if [[ "${NEW32C}" != "${REF32C}" || "${SRV32C}" != "${REF32C}" ]]; then
                echo 1>&2 "$(basename $0): error: crc32 checksum check failed for file: ${i}.dat"
```

### Comparing `xrootd-5.6.0/tests/XrdCephTests/CMakeLists.txt` & `xrootd-5.6.1/tests/XrdCephTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdCephTests/CephParsingTest.cc` & `xrootd-5.6.1/tests/XrdCephTests/CephParsingTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdCl/XrdClURL.cc` & `xrootd-5.6.1/tests/XrdCl/XrdClURL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClHttp/cases/000-simple-download/main.sh` & `xrootd-5.6.1/tests/XrdClHttp/cases/000-simple-download/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClHttp/cases/001-deep-path-download/main.sh` & `xrootd-5.6.1/tests/XrdClHttp/cases/001-deep-path-download/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClHttp/cases/002-simple-upload/main.sh` & `xrootd-5.6.1/tests/XrdClHttp/cases/002-simple-upload/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClHttp/cases/003-deep-path-upload/main.sh` & `xrootd-5.6.1/tests/XrdClHttp/cases/003-deep-path-upload/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClHttp/common.sh` & `xrootd-5.6.1/tests/XrdClHttp/common.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClHttp/run_test.sh` & `xrootd-5.6.1/tests/XrdClHttp/run_test.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/CMakeLists.txt` & `xrootd-5.6.1/tests/XrdClTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/FileCopyTest.cc` & `xrootd-5.6.1/tests/XrdClTests/FileCopyTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/FileSystemTest.cc` & `xrootd-5.6.1/tests/XrdClTests/FileSystemTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/FileTest.cc` & `xrootd-5.6.1/tests/XrdClTests/FileTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/IdentityPlugIn.cc` & `xrootd-5.6.1/tests/XrdClTests/IdentityPlugIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/IdentityPlugIn.hh` & `xrootd-5.6.1/tests/XrdClTests/IdentityPlugIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/LocalFileHandlerTest.cc` & `xrootd-5.6.1/tests/XrdClTests/LocalFileHandlerTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/MonitorTestLib.cc` & `xrootd-5.6.1/tests/XrdClTests/MonitorTestLib.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/OperationsWorkflowTest.cc` & `xrootd-5.6.1/tests/XrdClTests/OperationsWorkflowTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/PollerTest.cc` & `xrootd-5.6.1/tests/XrdClTests/PollerTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/PostMasterTest.cc` & `xrootd-5.6.1/tests/XrdClTests/PostMasterTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/SocketTest.cc` & `xrootd-5.6.1/tests/XrdClTests/SocketTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/ThreadingTest.cc` & `xrootd-5.6.1/tests/XrdClTests/ThreadingTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/UtilsTest.cc` & `xrootd-5.6.1/tests/XrdClTests/UtilsTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/XRootDProtocolHelper.cc` & `xrootd-5.6.1/tests/XrdClTests/XRootDProtocolHelper.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/XRootDProtocolHelper.hh` & `xrootd-5.6.1/tests/XrdClTests/XRootDProtocolHelper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/tls/CMakeLists.txt` & `xrootd-5.6.1/tests/XrdClTests/tls/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/tls/README.md` & `xrootd-5.6.1/tests/XrdClTests/tls/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/tls/xrdcl-tls.cc` & `xrootd-5.6.1/tests/XrdClTests/tls/xrdcl-tls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/tls/xrdsrv-tls.cc` & `xrootd-5.6.1/tests/XrdClTests/tls/xrdsrv-tls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/wrt/xrdsrv-dio.cc` & `xrootd-5.6.1/tests/XrdClTests/wrt/xrdsrv-dio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdClTests/wrt/xrdsrv-wrt.cc` & `xrootd-5.6.1/tests/XrdClTests/wrt/xrdsrv-wrt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdEcTests/CMakeLists.txt` & `xrootd-5.6.1/tests/XrdEcTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdEcTests/MicroTest.cc` & `xrootd-5.6.1/tests/XrdEcTests/MicroTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdHttpTests/XrdHttpTests.cc` & `xrootd-5.6.1/tests/XrdHttpTests/XrdHttpTests.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/XrdSsiTests/XrdShMap.cc` & `xrootd-5.6.1/tests/XrdSsiTests/XrdShMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/CMakeLists.txt` & `xrootd-5.6.1/tests/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/CppUnitXrdHelpers.hh` & `xrootd-5.6.1/tests/common/CppUnitXrdHelpers.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/PathProcessor.hh` & `xrootd-5.6.1/tests/common/PathProcessor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/Server.cc` & `xrootd-5.6.1/tests/common/Server.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/Server.hh` & `xrootd-5.6.1/tests/common/Server.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/TestEnv.cc` & `xrootd-5.6.1/tests/common/TestEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/TestEnv.hh` & `xrootd-5.6.1/tests/common/TestEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/TextRunner.cc` & `xrootd-5.6.1/tests/common/TextRunner.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/Utils.cc` & `xrootd-5.6.1/tests/common/Utils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/tests/common/Utils.hh` & `xrootd-5.6.1/tests/common/Utils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/ups/eupspkg.cfg.sh` & `xrootd-5.6.1/ups/eupspkg.cfg.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/utils/XrdCmsNotify.pm` & `xrootd-5.6.1/utils/XrdCmsNotify.pm`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/utils/XrdOlbMonPerf` & `xrootd-5.6.1/utils/XrdOlbMonPerf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/utils/cms_monPerf` & `xrootd-5.6.1/utils/cms_monPerf`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/utils/hpsscp` & `xrootd-5.6.1/utils/hpsscp`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/utils/netchk` & `xrootd-5.6.1/utils/netchk`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/utils/xrootd-config` & `xrootd-5.6.1/utils/xrootd-config`

 * *Files identical despite different names*

### Comparing `xrootd-5.6.0/xrootd.egg-info/PKG-INFO` & `xrootd-5.6.1/xrootd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xrootd
-Version: 5.6.0
+Version: 5.6.1
 Summary: eXtended ROOT daemon
 Home-page: http://xrootd.org
-Download-URL: https://github.com/xrootd/xrootd/archive/v5.6.0.tar.gz
+Download-URL: https://github.com/xrootd/xrootd/archive/v5.6.1.tar.gz
 Author: XRootD Developers
 Author-email: xrootd-dev@slac.stanford.edu
 License: LGPLv3+
 Keywords: XRootD,network filesystem
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `xrootd-5.6.0/xrootd.egg-info/SOURCES.txt` & `xrootd-5.6.1/xrootd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 cmake_uninstall.cmake.in
 gen-tarball.sh
 genversion.sh
-publish.sh
 pyproject.toml
 setup.py
 bindings/CMakeLists.txt
 bindings/python/.gitignore
 bindings/python/CMakeLists.txt
 bindings/python/MANIFEST.in
 bindings/python/README.md
```

