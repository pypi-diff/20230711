# Comparing `tmp/mariadb-1.1.6.tar.gz` & `tmp/mariadb-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mariadb-1.1.6.tar", last modified: Sun Feb 19 09:08:35 2023, from Unix
+gzip compressed data, was "mariadb-1.1.7.tar", last modified: Mon Jul  3 08:14:45 2023, max compression
```

## Comparing `mariadb-1.1.6.tar` & `mariadb-1.1.7.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 georg     (1000) georg     (1000)        0 2023-02-19 09:08:35.737502 mariadb-1.1.6/
--rw-rw-r--   0 georg     (1000) georg     (1000)    26526 2022-11-01 07:50:04.000000 mariadb-1.1.6/LICENSE
--rw-rw-r--   0 georg     (1000) georg     (1000)      198 2022-11-01 07:50:04.000000 mariadb-1.1.6/MANIFEST.in
--rw-rw-r--   0 georg     (1000) georg     (1000)     2978 2023-02-19 09:08:35.737502 mariadb-1.1.6/PKG-INFO
--rw-rw-r--   0 georg     (1000) georg     (1000)     1592 2023-01-11 19:13:26.000000 mariadb-1.1.6/README.md
-drwxrwxr-x   0 georg     (1000) georg     (1000)        0 2023-02-19 09:08:35.729502 mariadb-1.1.6/include/
-drwxrwxr-x   0 georg     (1000) georg     (1000)        0 2023-02-19 09:08:35.729502 mariadb-1.1.6/include/docs/
--rw-rw-r--   0 georg     (1000) georg     (1000)     3462 2022-11-01 07:50:04.000000 mariadb-1.1.6/include/docs/common.h
--rw-rw-r--   0 georg     (1000) georg     (1000)     4347 2022-11-01 07:50:04.000000 mariadb-1.1.6/include/docs/connection.h
--rw-rw-r--   0 georg     (1000) georg     (1000)     3607 2022-11-01 07:50:04.000000 mariadb-1.1.6/include/docs/cursor.h
--rw-rw-r--   0 georg     (1000) georg     (1000)     2601 2022-11-01 07:50:04.000000 mariadb-1.1.6/include/docs/exception.h
--rw-rw-r--   0 georg     (1000) georg     (1000)     1067 2022-11-01 07:50:04.000000 mariadb-1.1.6/include/docs/module.h
--rwxrwxr-x   0 georg     (1000) georg     (1000)    24887 2023-02-02 15:34:06.000000 mariadb-1.1.6/include/mariadb_python.h
-drwxrwxr-x   0 georg     (1000) georg     (1000)        0 2023-02-19 09:08:35.733502 mariadb-1.1.6/mariadb/
--rw-rw-r--   0 georg     (1000) georg     (1000)     6310 2023-02-03 06:16:27.000000 mariadb-1.1.6/mariadb/__init__.py
--rw-rw-r--   0 georg     (1000) georg     (1000)    11334 2023-02-08 15:14:22.000000 mariadb-1.1.6/mariadb/connectionpool.py
--rw-rw-r--   0 georg     (1000) georg     (1000)    22830 2023-02-06 14:21:30.000000 mariadb-1.1.6/mariadb/connections.py
-drwxrwxr-x   0 georg     (1000) georg     (1000)        0 2023-02-19 09:08:35.737502 mariadb-1.1.6/mariadb/constants/
--rw-rw-r--   0 georg     (1000) georg     (1000)      831 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/CAPABILITY.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      828 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/CLIENT.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      209 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/CURSOR.py
--rw-rw-r--   0 georg     (1000) georg     (1000)    41779 2022-11-01 07:50:04.000000 mariadb-1.1.6/mariadb/constants/ERR.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      609 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/FIELD_FLAG.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      630 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/FIELD_TYPE.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      354 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/INDICATOR.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      696 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/INFO.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      426 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/STATUS.py
--rw-rw-r--   0 georg     (1000) georg     (1000)       29 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/TPC_STATE.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      114 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/constants/__init__.py
--rw-rw-r--   0 georg     (1000) georg     (1000)    19243 2023-02-12 07:17:39.000000 mariadb-1.1.6/mariadb/cursors.py
--rw-rw-r--   0 georg     (1000) georg     (1000)     3311 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/dbapi20.py
--rw-rw-r--   0 georg     (1000) georg     (1000)     2363 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb/field.py
--rw-rw-r--   0 georg     (1000) georg     (1000)     6306 2023-02-03 06:16:27.000000 mariadb-1.1.6/mariadb/mariadb.c
--rw-rw-r--   0 georg     (1000) georg     (1000)    45303 2023-02-02 15:34:18.000000 mariadb-1.1.6/mariadb/mariadb_codecs.c
--rw-rw-r--   0 georg     (1000) georg     (1000)    27118 2023-02-02 15:34:18.000000 mariadb-1.1.6/mariadb/mariadb_connection.c
--rw-rw-r--   0 georg     (1000) georg     (1000)    35344 2023-02-12 07:19:43.000000 mariadb-1.1.6/mariadb/mariadb_cursor.c
--rw-rw-r--   0 georg     (1000) georg     (1000)     7503 2023-02-02 15:34:18.000000 mariadb-1.1.6/mariadb/mariadb_exception.c
--rwxrwxr-x   0 georg     (1000) georg     (1000)    12070 2023-02-02 15:34:18.000000 mariadb-1.1.6/mariadb/mariadb_parser.c
--rw-rw-r--   0 georg     (1000) georg     (1000)       80 2023-02-19 09:08:35.000000 mariadb-1.1.6/mariadb/release_info.py
-drwxrwxr-x   0 georg     (1000) georg     (1000)        0 2023-02-19 09:08:35.733502 mariadb-1.1.6/mariadb.egg-info/
--rw-rw-r--   0 georg     (1000) georg     (1000)     2978 2023-02-19 09:08:35.000000 mariadb-1.1.6/mariadb.egg-info/PKG-INFO
--rw-rw-r--   0 georg     (1000) georg     (1000)     1015 2023-02-19 09:08:35.000000 mariadb-1.1.6/mariadb.egg-info/SOURCES.txt
--rw-rw-r--   0 georg     (1000) georg     (1000)        1 2023-02-19 09:08:35.000000 mariadb-1.1.6/mariadb.egg-info/dependency_links.txt
--rw-rw-r--   0 georg     (1000) georg     (1000)       10 2023-02-19 09:08:35.000000 mariadb-1.1.6/mariadb.egg-info/requires.txt
--rw-rw-r--   0 georg     (1000) georg     (1000)        8 2023-02-19 09:08:35.000000 mariadb-1.1.6/mariadb.egg-info/top_level.txt
--rw-rw-r--   0 georg     (1000) georg     (1000)     2811 2023-01-16 13:12:03.000000 mariadb-1.1.6/mariadb_posix.py
--rwxrwxr-x   0 georg     (1000) georg     (1000)     3129 2023-01-11 19:13:26.000000 mariadb-1.1.6/mariadb_windows.py
--rw-rw-r--   0 georg     (1000) georg     (1000)       72 2023-01-11 19:13:26.000000 mariadb-1.1.6/pyproject.toml
--rw-rw-r--   0 georg     (1000) georg     (1000)       38 2023-02-19 09:08:35.741502 mariadb-1.1.6/setup.cfg
--rw-rw-r--   0 georg     (1000) georg     (1000)     6089 2023-01-11 19:13:26.000000 mariadb-1.1.6/setup.py
--rw-rw-r--   0 georg     (1000) georg     (1000)      396 2022-11-01 07:50:04.000000 mariadb-1.1.6/site.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 08:14:45.688677 mariadb-1.1.7/
+-rw-rw-rw-   0        0        0    27030 2023-07-02 06:23:10.000000 mariadb-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-07-02 09:50:17.000000 mariadb-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3051 2023-07-03 08:14:45.688677 mariadb-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1632 2023-07-02 09:50:17.000000 mariadb-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 08:14:45.610170 mariadb-1.1.7/include/
+-rw-rw-rw-   0        0        0      100 2023-07-03 08:14:45.000000 mariadb-1.1.7/include/config_win.h
+drwxrwxrwx   0        0        0        0 2023-07-03 08:14:45.625781 mariadb-1.1.7/include/docs/
+-rw-rw-rw-   0        0        0     3538 2023-07-02 09:50:17.000000 mariadb-1.1.7/include/docs/common.h
+-rw-rw-rw-   0        0        0     4474 2023-07-02 09:50:17.000000 mariadb-1.1.7/include/docs/connection.h
+-rw-rw-rw-   0        0        0     3732 2023-07-02 09:50:17.000000 mariadb-1.1.7/include/docs/cursor.h
+-rw-rw-rw-   0        0        0     2677 2023-07-02 09:50:17.000000 mariadb-1.1.7/include/docs/exception.h
+-rw-rw-rw-   0        0        0     1089 2023-07-02 09:50:17.000000 mariadb-1.1.7/include/docs/module.h
+-rw-rw-rw-   0        0        0    25725 2023-07-02 09:50:17.000000 mariadb-1.1.7/include/mariadb_python.h
+drwxrwxrwx   0        0        0        0 2023-07-03 08:14:45.679168 mariadb-1.1.7/mariadb/
+-rw-rw-rw-   0        0        0     6667 2023-07-03 08:13:35.000000 mariadb-1.1.7/mariadb/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/connectionpool.py
+-rw-rw-rw-   0        0        0    23504 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/connections.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:14:45.688677 mariadb-1.1.7/mariadb/constants/
+-rw-rw-rw-   0        0        0      869 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/CAPABILITY.py
+-rw-rw-rw-   0        0        0      866 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/CLIENT.py
+-rw-rw-rw-   0        0        0      218 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/CURSOR.py
+-rw-rw-rw-   0        0        0    43033 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/ERR.py
+-rw-rw-rw-   0        0        0      638 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/FIELD_FLAG.py
+-rw-rw-rw-   0        0        0      670 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/FIELD_TYPE.py
+-rw-rw-rw-   0        0        0      373 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/INDICATOR.py
+-rw-rw-rw-   0        0        0      736 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/INFO.py
+-rw-rw-rw-   0        0        0      447 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/STATUS.py
+-rw-rw-rw-   0        0        0       32 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/TPC_STATE.py
+-rw-rw-rw-   0        0        0      116 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/constants/__init__.py
+-rw-rw-rw-   0        0        0    19783 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/cursors.py
+-rw-rw-rw-   0        0        0     3422 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/dbapi20.py
+-rw-rw-rw-   0        0        0     2422 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/field.py
+-rw-rw-rw-   0        0        0     6498 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/mariadb.c
+-rw-rw-rw-   0        0        0    47009 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/mariadb_codecs.c
+-rw-rw-rw-   0        0        0    28265 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/mariadb_connection.c
+-rw-rw-rw-   0        0        0    37471 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/mariadb_cursor.c
+-rw-rw-rw-   0        0        0     7723 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/mariadb_exception.c
+-rw-rw-rw-   0        0        0    12480 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb/mariadb_parser.c
+-rw-rw-rw-   0        0        0       83 2023-07-03 08:14:45.000000 mariadb-1.1.7/mariadb/release_info.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:14:45.688677 mariadb-1.1.7/mariadb.egg-info/
+-rw-rw-rw-   0        0        0     3051 2023-07-03 08:14:45.000000 mariadb-1.1.7/mariadb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2023-07-03 08:14:45.000000 mariadb-1.1.7/mariadb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:14:45.000000 mariadb-1.1.7/mariadb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 08:14:45.000000 mariadb-1.1.7/mariadb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 08:14:45.000000 mariadb-1.1.7/mariadb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2898 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb_posix.py
+-rw-rw-rw-   0        0        0     3212 2023-07-02 09:50:17.000000 mariadb-1.1.7/mariadb_windows.py
+-rw-rw-rw-   0        0        0       78 2023-07-02 09:50:17.000000 mariadb-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:14:45.688677 mariadb-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     6240 2023-07-03 08:13:35.000000 mariadb-1.1.7/setup.py
+-rw-rw-rw-   0        0        0      405 2023-07-02 09:50:17.000000 mariadb-1.1.7/site.cfg
```

### Comparing `mariadb-1.1.6/LICENSE` & `mariadb-1.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,504 +1,504 @@
-                  GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 2.1, February 1999
-
- Copyright (C) 1991, 1999 Free Software Foundation, Inc.
- 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-[This is the first released version of the Lesser GPL.  It also counts
- as the successor of the GNU Library Public License, version 2, hence
- the version number 2.1.]
-
-                            Preamble
-
-  The licenses for most software are designed to take away your
-freedom to share and change it.  By contrast, the GNU General Public
-Licenses are intended to guarantee your freedom to share and change
-free software--to make sure the software is free for all its users.
-
-  This license, the Lesser General Public License, applies to some
-specially designated software packages--typically libraries--of the
-Free Software Foundation and other authors who decide to use it.  You
-can use it too, but we suggest you first think carefully about whether
-this license or the ordinary General Public License is the better
-strategy to use in any particular case, based on the explanations below.
-
-  When we speak of free software, we are referring to freedom of use,
-not price.  Our General Public Licenses are designed to make sure that
-you have the freedom to distribute copies of free software (and charge
-for this service if you wish); that you receive source code or can get
-it if you want it; that you can change the software and use pieces of
-it in new free programs; and that you are informed that you can do
-these things.
-
-  To protect your rights, we need to make restrictions that forbid
-distributors to deny you these rights or to ask you to surrender these
-rights.  These restrictions translate to certain responsibilities for
-you if you distribute copies of the library or if you modify it.
-
-  For example, if you distribute copies of the library, whether gratis
-or for a fee, you must give the recipients all the rights that we gave
-you.  You must make sure that they, too, receive or can get the source
-code.  If you link other code with the library, you must provide
-complete object files to the recipients, so that they can relink them
-with the library after making changes to the library and recompiling
-it.  And you must show them these terms so they know their rights.
-
-  We protect your rights with a two-step method: (1) we copyright the
-library, and (2) we offer you this license, which gives you legal
-permission to copy, distribute and/or modify the library.
-
-  To protect each distributor, we want to make it very clear that
-there is no warranty for the free library.  Also, if the library is
-modified by someone else and passed on, the recipients should know
-that what they have is not the original version, so that the original
-author's reputation will not be affected by problems that might be
-introduced by others.
-
-  Finally, software patents pose a constant threat to the existence of
-any free program.  We wish to make sure that a company cannot
-effectively restrict the users of a free program by obtaining a
-restrictive license from a patent holder.  Therefore, we insist that
-any patent license obtained for a version of the library must be
-consistent with the full freedom of use specified in this license.
-
-  Most GNU software, including some libraries, is covered by the
-ordinary GNU General Public License.  This license, the GNU Lesser
-General Public License, applies to certain designated libraries, and
-is quite different from the ordinary General Public License.  We use
-this license for certain libraries in order to permit linking those
-libraries into non-free programs.
-
-  When a program is linked with a library, whether statically or using
-a shared library, the combination of the two is legally speaking a
-combined work, a derivative of the original library.  The ordinary
-General Public License therefore permits such linking only if the
-entire combination fits its criteria of freedom.  The Lesser General
-Public License permits more lax criteria for linking other code with
-the library.
-
-  We call this license the "Lesser" General Public License because it
-does Less to protect the user's freedom than the ordinary General
-Public License.  It also provides other free software developers Less
-of an advantage over competing non-free programs.  These disadvantages
-are the reason we use the ordinary General Public License for many
-libraries.  However, the Lesser license provides advantages in certain
-special circumstances.
-
-  For example, on rare occasions, there may be a special need to
-encourage the widest possible use of a certain library, so that it becomes
-a de-facto standard.  To achieve this, non-free programs must be
-allowed to use the library.  A more frequent case is that a free
-library does the same job as widely used non-free libraries.  In this
-case, there is little to gain by limiting the free library to free
-software only, so we use the Lesser General Public License.
-
-  In other cases, permission to use a particular library in non-free
-programs enables a greater number of people to use a large body of
-free software.  For example, permission to use the GNU C Library in
-non-free programs enables many more people to use the whole GNU
-operating system, as well as its variant, the GNU/Linux operating
-system.
-
-  Although the Lesser General Public License is Less protective of the
-users' freedom, it does ensure that the user of a program that is
-linked with the Library has the freedom and the wherewithal to run
-that program using a modified version of the Library.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.  Pay close attention to the difference between a
-"work based on the library" and a "work that uses the library".  The
-former contains code derived from the library, whereas the latter must
-be combined with the library in order to run.
-
-                  GNU LESSER GENERAL PUBLIC LICENSE
-   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-  0. This License Agreement applies to any software library or other
-program which contains a notice placed by the copyright holder or
-other authorized party saying it may be distributed under the terms of
-this Lesser General Public License (also called "this License").
-Each licensee is addressed as "you".
-
-  A "library" means a collection of software functions and/or data
-prepared so as to be conveniently linked with application programs
-(which use some of those functions and data) to form executables.
-
-  The "Library", below, refers to any such software library or work
-which has been distributed under these terms.  A "work based on the
-Library" means either the Library or any derivative work under
-copyright law: that is to say, a work containing the Library or a
-portion of it, either verbatim or with modifications and/or translated
-straightforwardly into another language.  (Hereinafter, translation is
-included without limitation in the term "modification".)
-
-  "Source code" for a work means the preferred form of the work for
-making modifications to it.  For a library, complete source code means
-all the source code for all modules it contains, plus any associated
-interface definition files, plus the scripts used to control compilation
-and installation of the library.
-
-  Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope.  The act of
-running a program using the Library is not restricted, and output from
-such a program is covered only if its contents constitute a work based
-on the Library (independent of the use of the Library in a tool for
-writing it).  Whether that is true depends on what the Library does
-and what the program that uses the Library does.
-
-  1. You may copy and distribute verbatim copies of the Library's
-complete source code as you receive it, in any medium, provided that
-you conspicuously and appropriately publish on each copy an
-appropriate copyright notice and disclaimer of warranty; keep intact
-all the notices that refer to this License and to the absence of any
-warranty; and distribute a copy of this License along with the
-Library.
-
-  You may charge a fee for the physical act of transferring a copy,
-and you may at your option offer warranty protection in exchange for a
-fee.
-
-  2. You may modify your copy or copies of the Library or any portion
-of it, thus forming a work based on the Library, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
-    a) The modified work must itself be a software library.
-
-    b) You must cause the files modified to carry prominent notices
-    stating that you changed the files and the date of any change.
-
-    c) You must cause the whole of the work to be licensed at no
-    charge to all third parties under the terms of this License.
-
-    d) If a facility in the modified Library refers to a function or a
-    table of data to be supplied by an application program that uses
-    the facility, other than as an argument passed when the facility
-    is invoked, then you must make a good faith effort to ensure that,
-    in the event an application does not supply such function or
-    table, the facility still operates, and performs whatever part of
-    its purpose remains meaningful.
-
-    (For example, a function in a library to compute square roots has
-    a purpose that is entirely well-defined independent of the
-    application.  Therefore, Subsection 2d requires that any
-    application-supplied function or table used by this function must
-    be optional: if the application does not supply it, the square
-    root function must still compute square roots.)
-
-These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Library,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works.  But when you
-distribute the same sections as part of a whole which is a work based
-on the Library, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote
-it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Library.
-
-In addition, mere aggregation of another work not based on the Library
-with the Library (or with a work based on the Library) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-  3. You may opt to apply the terms of the ordinary GNU General Public
-License instead of this License to a given copy of the Library.  To do
-this, you must alter all the notices that refer to this License, so
-that they refer to the ordinary GNU General Public License, version 2,
-instead of to this License.  (If a newer version than version 2 of the
-ordinary GNU General Public License has appeared, then you can specify
-that version instead if you wish.)  Do not make any other change in
-these notices.
-
-  Once this change is made in a given copy, it is irreversible for
-that copy, so the ordinary GNU General Public License applies to all
-subsequent copies and derivative works made from that copy.
-
-  This option is useful when you wish to copy part of the code of
-the Library into a program that is not a library.
-
-  4. You may copy and distribute the Library (or a portion or
-derivative of it, under Section 2) in object code or executable form
-under the terms of Sections 1 and 2 above provided that you accompany
-it with the complete corresponding machine-readable source code, which
-must be distributed under the terms of Sections 1 and 2 above on a
-medium customarily used for software interchange.
-
-  If distribution of object code is made by offering access to copy
-from a designated place, then offering equivalent access to copy the
-source code from the same place satisfies the requirement to
-distribute the source code, even though third parties are not
-compelled to copy the source along with the object code.
-
-  5. A program that contains no derivative of any portion of the
-Library, but is designed to work with the Library by being compiled or
-linked with it, is called a "work that uses the Library".  Such a
-work, in isolation, is not a derivative work of the Library, and
-therefore falls outside the scope of this License.
-
-  However, linking a "work that uses the Library" with the Library
-creates an executable that is a derivative of the Library (because it
-contains portions of the Library), rather than a "work that uses the
-library".  The executable is therefore covered by this License.
-Section 6 states terms for distribution of such executables.
-
-  When a "work that uses the Library" uses material from a header file
-that is part of the Library, the object code for the work may be a
-derivative work of the Library even though the source code is not.
-Whether this is true is especially significant if the work can be
-linked without the Library, or if the work is itself a library.  The
-threshold for this to be true is not precisely defined by law.
-
-  If such an object file uses only numerical parameters, data
-structure layouts and accessors, and small macros and small inline
-functions (ten lines or less in length), then the use of the object
-file is unrestricted, regardless of whether it is legally a derivative
-work.  (Executables containing this object code plus portions of the
-Library will still fall under Section 6.)
-
-  Otherwise, if the work is a derivative of the Library, you may
-distribute the object code for the work under the terms of Section 6.
-Any executables containing that work also fall under Section 6,
-whether or not they are linked directly with the Library itself.
-
-  6. As an exception to the Sections above, you may also combine or
-link a "work that uses the Library" with the Library to produce a
-work containing portions of the Library, and distribute that work
-under terms of your choice, provided that the terms permit
-modification of the work for the customer's own use and reverse
-engineering for debugging such modifications.
-
-  You must give prominent notice with each copy of the work that the
-Library is used in it and that the Library and its use are covered by
-this License.  You must supply a copy of this License.  If the work
-during execution displays copyright notices, you must include the
-copyright notice for the Library among them, as well as a reference
-directing the user to the copy of this License.  Also, you must do one
-of these things:
-
-    a) Accompany the work with the complete corresponding
-    machine-readable source code for the Library including whatever
-    changes were used in the work (which must be distributed under
-    Sections 1 and 2 above); and, if the work is an executable linked
-    with the Library, with the complete machine-readable "work that
-    uses the Library", as object code and/or source code, so that the
-    user can modify the Library and then relink to produce a modified
-    executable containing the modified Library.  (It is understood
-    that the user who changes the contents of definitions files in the
-    Library will not necessarily be able to recompile the application
-    to use the modified definitions.)
-
-    b) Use a suitable shared library mechanism for linking with the
-    Library.  A suitable mechanism is one that (1) uses at run time a
-    copy of the library already present on the user's computer system,
-    rather than copying library functions into the executable, and (2)
-    will operate properly with a modified version of the library, if
-    the user installs one, as long as the modified version is
-    interface-compatible with the version that the work was made with.
-
-    c) Accompany the work with a written offer, valid for at
-    least three years, to give the same user the materials
-    specified in Subsection 6a, above, for a charge no more
-    than the cost of performing this distribution.
-
-    d) If distribution of the work is made by offering access to copy
-    from a designated place, offer equivalent access to copy the above
-    specified materials from the same place.
-
-    e) Verify that the user has already received a copy of these
-    materials or that you have already sent this user a copy.
-
-  For an executable, the required form of the "work that uses the
-Library" must include any data and utility programs needed for
-reproducing the executable from it.  However, as a special exception,
-the materials to be distributed need not include anything that is
-normally distributed (in either source or binary form) with the major
-components (compiler, kernel, and so on) of the operating system on
-which the executable runs, unless that component itself accompanies
-the executable.
-
-  It may happen that this requirement contradicts the license
-restrictions of other proprietary libraries that do not normally
-accompany the operating system.  Such a contradiction means you cannot
-use both them and the Library together in an executable that you
-distribute.
-
-  7. You may place library facilities that are a work based on the
-Library side-by-side in a single library together with other library
-facilities not covered by this License, and distribute such a combined
-library, provided that the separate distribution of the work based on
-the Library and of the other library facilities is otherwise
-permitted, and provided that you do these two things:
-
-    a) Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other library
-    facilities.  This must be distributed under the terms of the
-    Sections above.
-
-    b) Give prominent notice with the combined library of the fact
-    that part of it is a work based on the Library, and explaining
-    where to find the accompanying uncombined form of the same work.
-
-  8. You may not copy, modify, sublicense, link with, or distribute
-the Library except as expressly provided under this License.  Any
-attempt otherwise to copy, modify, sublicense, link with, or
-distribute the Library is void, and will automatically terminate your
-rights under this License.  However, parties who have received copies,
-or rights, from you under this License will not have their licenses
-terminated so long as such parties remain in full compliance.
-
-  9. You are not required to accept this License, since you have not
-signed it.  However, nothing else grants you permission to modify or
-distribute the Library or its derivative works.  These actions are
-prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Library (or any work based on the
-Library), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Library or works based on it.
-
-  10. Each time you redistribute the Library (or any work based on the
-Library), the recipient automatically receives a license from the
-original licensor to copy, distribute, link with or modify the Library
-subject to these terms and conditions.  You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties with
-this License.
-
-  11. If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues),
-conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot
-distribute so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not distribute the Library at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Library by
-all those who receive copies directly or indirectly through you, then
-the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Library.
-
-If any portion of this section is held invalid or unenforceable under any
-particular circumstance, the balance of the section is intended to apply,
-and the section as a whole is intended to apply in other circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system which is
-implemented by public license practices.  Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-  12. If the distribution and/or use of the Library is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Library under this License may add
-an explicit geographical distribution limitation excluding those countries,
-so that distribution is permitted only in or among countries not thus
-excluded.  In such case, this License incorporates the limitation as if
-written in the body of this License.
-
-  13. The Free Software Foundation may publish revised and/or new
-versions of the Lesser General Public License from time to time.
-Such new versions will be similar in spirit to the present version,
-but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Library
-specifies a version number of this License which applies to it and
-"any later version", you have the option of following the terms and
-conditions either of that version or of any later version published by
-the Free Software Foundation.  If the Library does not specify a
-license version number, you may choose any version ever published by
-the Free Software Foundation.
-
-  14. If you wish to incorporate parts of the Library into other free
-programs whose distribution conditions are incompatible with these,
-write to the author to ask for permission.  For software which is
-copyrighted by the Free Software Foundation, write to the Free
-Software Foundation; we sometimes make exceptions for this.  Our
-decision will be guided by the two goals of preserving the free status
-of all derivatives of our free software and of promoting the sharing
-and reuse of software generally.
-
-                            NO WARRANTY
-
-  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
-WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
-EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
-OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
-KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
-LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
-THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
-WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
-AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
-FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
-CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
-LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
-RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
-FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
-SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGES.
-
-                     END OF TERMS AND CONDITIONS
-
-           How to Apply These Terms to Your New Libraries
-
-  If you develop a new library, and you want it to be of the greatest
-possible use to the public, we recommend making it free software that
-everyone can redistribute and change.  You can do so by permitting
-redistribution under these terms (or, alternatively, under the terms of the
-ordinary General Public License).
-
-  To apply these terms, attach the following notices to the library.  It is
-safest to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the library's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This library is free software; you can redistribute it and/or
-    modify it under the terms of the GNU Lesser General Public
-    License as published by the Free Software Foundation; either
-    version 2.1 of the License, or (at your option) any later version.
-
-    This library is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    Lesser General Public License for more details.
-
-    You should have received a copy of the GNU Lesser General Public
-    License along with this library; if not, write to the Free Software
-    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
-    USA
-
-Also add information on how to contact you by electronic and paper mail.
-
-You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the library, if
-necessary.  Here is a sample; alter the names:
-
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the
-  library `Frob' (a library for tweaking knobs) written by James Random
-  Hacker.
-
-  <signature of Ty Coon>, 1 April 1990
-  Ty Coon, President of Vice
-
-That's all there is to it!
+                  GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 2.1, February 1999
+
+ Copyright (C) 1991, 1999 Free Software Foundation, Inc.
+ 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+[This is the first released version of the Lesser GPL.  It also counts
+ as the successor of the GNU Library Public License, version 2, hence
+ the version number 2.1.]
+
+                            Preamble
+
+  The licenses for most software are designed to take away your
+freedom to share and change it.  By contrast, the GNU General Public
+Licenses are intended to guarantee your freedom to share and change
+free software--to make sure the software is free for all its users.
+
+  This license, the Lesser General Public License, applies to some
+specially designated software packages--typically libraries--of the
+Free Software Foundation and other authors who decide to use it.  You
+can use it too, but we suggest you first think carefully about whether
+this license or the ordinary General Public License is the better
+strategy to use in any particular case, based on the explanations below.
+
+  When we speak of free software, we are referring to freedom of use,
+not price.  Our General Public Licenses are designed to make sure that
+you have the freedom to distribute copies of free software (and charge
+for this service if you wish); that you receive source code or can get
+it if you want it; that you can change the software and use pieces of
+it in new free programs; and that you are informed that you can do
+these things.
+
+  To protect your rights, we need to make restrictions that forbid
+distributors to deny you these rights or to ask you to surrender these
+rights.  These restrictions translate to certain responsibilities for
+you if you distribute copies of the library or if you modify it.
+
+  For example, if you distribute copies of the library, whether gratis
+or for a fee, you must give the recipients all the rights that we gave
+you.  You must make sure that they, too, receive or can get the source
+code.  If you link other code with the library, you must provide
+complete object files to the recipients, so that they can relink them
+with the library after making changes to the library and recompiling
+it.  And you must show them these terms so they know their rights.
+
+  We protect your rights with a two-step method: (1) we copyright the
+library, and (2) we offer you this license, which gives you legal
+permission to copy, distribute and/or modify the library.
+
+  To protect each distributor, we want to make it very clear that
+there is no warranty for the free library.  Also, if the library is
+modified by someone else and passed on, the recipients should know
+that what they have is not the original version, so that the original
+author's reputation will not be affected by problems that might be
+introduced by others.
+
+  Finally, software patents pose a constant threat to the existence of
+any free program.  We wish to make sure that a company cannot
+effectively restrict the users of a free program by obtaining a
+restrictive license from a patent holder.  Therefore, we insist that
+any patent license obtained for a version of the library must be
+consistent with the full freedom of use specified in this license.
+
+  Most GNU software, including some libraries, is covered by the
+ordinary GNU General Public License.  This license, the GNU Lesser
+General Public License, applies to certain designated libraries, and
+is quite different from the ordinary General Public License.  We use
+this license for certain libraries in order to permit linking those
+libraries into non-free programs.
+
+  When a program is linked with a library, whether statically or using
+a shared library, the combination of the two is legally speaking a
+combined work, a derivative of the original library.  The ordinary
+General Public License therefore permits such linking only if the
+entire combination fits its criteria of freedom.  The Lesser General
+Public License permits more lax criteria for linking other code with
+the library.
+
+  We call this license the "Lesser" General Public License because it
+does Less to protect the user's freedom than the ordinary General
+Public License.  It also provides other free software developers Less
+of an advantage over competing non-free programs.  These disadvantages
+are the reason we use the ordinary General Public License for many
+libraries.  However, the Lesser license provides advantages in certain
+special circumstances.
+
+  For example, on rare occasions, there may be a special need to
+encourage the widest possible use of a certain library, so that it becomes
+a de-facto standard.  To achieve this, non-free programs must be
+allowed to use the library.  A more frequent case is that a free
+library does the same job as widely used non-free libraries.  In this
+case, there is little to gain by limiting the free library to free
+software only, so we use the Lesser General Public License.
+
+  In other cases, permission to use a particular library in non-free
+programs enables a greater number of people to use a large body of
+free software.  For example, permission to use the GNU C Library in
+non-free programs enables many more people to use the whole GNU
+operating system, as well as its variant, the GNU/Linux operating
+system.
+
+  Although the Lesser General Public License is Less protective of the
+users' freedom, it does ensure that the user of a program that is
+linked with the Library has the freedom and the wherewithal to run
+that program using a modified version of the Library.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.  Pay close attention to the difference between a
+"work based on the library" and a "work that uses the library".  The
+former contains code derived from the library, whereas the latter must
+be combined with the library in order to run.
+
+                  GNU LESSER GENERAL PUBLIC LICENSE
+   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+  0. This License Agreement applies to any software library or other
+program which contains a notice placed by the copyright holder or
+other authorized party saying it may be distributed under the terms of
+this Lesser General Public License (also called "this License").
+Each licensee is addressed as "you".
+
+  A "library" means a collection of software functions and/or data
+prepared so as to be conveniently linked with application programs
+(which use some of those functions and data) to form executables.
+
+  The "Library", below, refers to any such software library or work
+which has been distributed under these terms.  A "work based on the
+Library" means either the Library or any derivative work under
+copyright law: that is to say, a work containing the Library or a
+portion of it, either verbatim or with modifications and/or translated
+straightforwardly into another language.  (Hereinafter, translation is
+included without limitation in the term "modification".)
+
+  "Source code" for a work means the preferred form of the work for
+making modifications to it.  For a library, complete source code means
+all the source code for all modules it contains, plus any associated
+interface definition files, plus the scripts used to control compilation
+and installation of the library.
+
+  Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope.  The act of
+running a program using the Library is not restricted, and output from
+such a program is covered only if its contents constitute a work based
+on the Library (independent of the use of the Library in a tool for
+writing it).  Whether that is true depends on what the Library does
+and what the program that uses the Library does.
+
+  1. You may copy and distribute verbatim copies of the Library's
+complete source code as you receive it, in any medium, provided that
+you conspicuously and appropriately publish on each copy an
+appropriate copyright notice and disclaimer of warranty; keep intact
+all the notices that refer to this License and to the absence of any
+warranty; and distribute a copy of this License along with the
+Library.
+
+  You may charge a fee for the physical act of transferring a copy,
+and you may at your option offer warranty protection in exchange for a
+fee.
+
+  2. You may modify your copy or copies of the Library or any portion
+of it, thus forming a work based on the Library, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+    a) The modified work must itself be a software library.
+
+    b) You must cause the files modified to carry prominent notices
+    stating that you changed the files and the date of any change.
+
+    c) You must cause the whole of the work to be licensed at no
+    charge to all third parties under the terms of this License.
+
+    d) If a facility in the modified Library refers to a function or a
+    table of data to be supplied by an application program that uses
+    the facility, other than as an argument passed when the facility
+    is invoked, then you must make a good faith effort to ensure that,
+    in the event an application does not supply such function or
+    table, the facility still operates, and performs whatever part of
+    its purpose remains meaningful.
+
+    (For example, a function in a library to compute square roots has
+    a purpose that is entirely well-defined independent of the
+    application.  Therefore, Subsection 2d requires that any
+    application-supplied function or table used by this function must
+    be optional: if the application does not supply it, the square
+    root function must still compute square roots.)
+
+These requirements apply to the modified work as a whole.  If
+identifiable sections of that work are not derived from the Library,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works.  But when you
+distribute the same sections as part of a whole which is a work based
+on the Library, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote
+it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Library.
+
+In addition, mere aggregation of another work not based on the Library
+with the Library (or with a work based on the Library) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+  3. You may opt to apply the terms of the ordinary GNU General Public
+License instead of this License to a given copy of the Library.  To do
+this, you must alter all the notices that refer to this License, so
+that they refer to the ordinary GNU General Public License, version 2,
+instead of to this License.  (If a newer version than version 2 of the
+ordinary GNU General Public License has appeared, then you can specify
+that version instead if you wish.)  Do not make any other change in
+these notices.
+
+  Once this change is made in a given copy, it is irreversible for
+that copy, so the ordinary GNU General Public License applies to all
+subsequent copies and derivative works made from that copy.
+
+  This option is useful when you wish to copy part of the code of
+the Library into a program that is not a library.
+
+  4. You may copy and distribute the Library (or a portion or
+derivative of it, under Section 2) in object code or executable form
+under the terms of Sections 1 and 2 above provided that you accompany
+it with the complete corresponding machine-readable source code, which
+must be distributed under the terms of Sections 1 and 2 above on a
+medium customarily used for software interchange.
+
+  If distribution of object code is made by offering access to copy
+from a designated place, then offering equivalent access to copy the
+source code from the same place satisfies the requirement to
+distribute the source code, even though third parties are not
+compelled to copy the source along with the object code.
+
+  5. A program that contains no derivative of any portion of the
+Library, but is designed to work with the Library by being compiled or
+linked with it, is called a "work that uses the Library".  Such a
+work, in isolation, is not a derivative work of the Library, and
+therefore falls outside the scope of this License.
+
+  However, linking a "work that uses the Library" with the Library
+creates an executable that is a derivative of the Library (because it
+contains portions of the Library), rather than a "work that uses the
+library".  The executable is therefore covered by this License.
+Section 6 states terms for distribution of such executables.
+
+  When a "work that uses the Library" uses material from a header file
+that is part of the Library, the object code for the work may be a
+derivative work of the Library even though the source code is not.
+Whether this is true is especially significant if the work can be
+linked without the Library, or if the work is itself a library.  The
+threshold for this to be true is not precisely defined by law.
+
+  If such an object file uses only numerical parameters, data
+structure layouts and accessors, and small macros and small inline
+functions (ten lines or less in length), then the use of the object
+file is unrestricted, regardless of whether it is legally a derivative
+work.  (Executables containing this object code plus portions of the
+Library will still fall under Section 6.)
+
+  Otherwise, if the work is a derivative of the Library, you may
+distribute the object code for the work under the terms of Section 6.
+Any executables containing that work also fall under Section 6,
+whether or not they are linked directly with the Library itself.
+
+  6. As an exception to the Sections above, you may also combine or
+link a "work that uses the Library" with the Library to produce a
+work containing portions of the Library, and distribute that work
+under terms of your choice, provided that the terms permit
+modification of the work for the customer's own use and reverse
+engineering for debugging such modifications.
+
+  You must give prominent notice with each copy of the work that the
+Library is used in it and that the Library and its use are covered by
+this License.  You must supply a copy of this License.  If the work
+during execution displays copyright notices, you must include the
+copyright notice for the Library among them, as well as a reference
+directing the user to the copy of this License.  Also, you must do one
+of these things:
+
+    a) Accompany the work with the complete corresponding
+    machine-readable source code for the Library including whatever
+    changes were used in the work (which must be distributed under
+    Sections 1 and 2 above); and, if the work is an executable linked
+    with the Library, with the complete machine-readable "work that
+    uses the Library", as object code and/or source code, so that the
+    user can modify the Library and then relink to produce a modified
+    executable containing the modified Library.  (It is understood
+    that the user who changes the contents of definitions files in the
+    Library will not necessarily be able to recompile the application
+    to use the modified definitions.)
+
+    b) Use a suitable shared library mechanism for linking with the
+    Library.  A suitable mechanism is one that (1) uses at run time a
+    copy of the library already present on the user's computer system,
+    rather than copying library functions into the executable, and (2)
+    will operate properly with a modified version of the library, if
+    the user installs one, as long as the modified version is
+    interface-compatible with the version that the work was made with.
+
+    c) Accompany the work with a written offer, valid for at
+    least three years, to give the same user the materials
+    specified in Subsection 6a, above, for a charge no more
+    than the cost of performing this distribution.
+
+    d) If distribution of the work is made by offering access to copy
+    from a designated place, offer equivalent access to copy the above
+    specified materials from the same place.
+
+    e) Verify that the user has already received a copy of these
+    materials or that you have already sent this user a copy.
+
+  For an executable, the required form of the "work that uses the
+Library" must include any data and utility programs needed for
+reproducing the executable from it.  However, as a special exception,
+the materials to be distributed need not include anything that is
+normally distributed (in either source or binary form) with the major
+components (compiler, kernel, and so on) of the operating system on
+which the executable runs, unless that component itself accompanies
+the executable.
+
+  It may happen that this requirement contradicts the license
+restrictions of other proprietary libraries that do not normally
+accompany the operating system.  Such a contradiction means you cannot
+use both them and the Library together in an executable that you
+distribute.
+
+  7. You may place library facilities that are a work based on the
+Library side-by-side in a single library together with other library
+facilities not covered by this License, and distribute such a combined
+library, provided that the separate distribution of the work based on
+the Library and of the other library facilities is otherwise
+permitted, and provided that you do these two things:
+
+    a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities.  This must be distributed under the terms of the
+    Sections above.
+
+    b) Give prominent notice with the combined library of the fact
+    that part of it is a work based on the Library, and explaining
+    where to find the accompanying uncombined form of the same work.
+
+  8. You may not copy, modify, sublicense, link with, or distribute
+the Library except as expressly provided under this License.  Any
+attempt otherwise to copy, modify, sublicense, link with, or
+distribute the Library is void, and will automatically terminate your
+rights under this License.  However, parties who have received copies,
+or rights, from you under this License will not have their licenses
+terminated so long as such parties remain in full compliance.
+
+  9. You are not required to accept this License, since you have not
+signed it.  However, nothing else grants you permission to modify or
+distribute the Library or its derivative works.  These actions are
+prohibited by law if you do not accept this License.  Therefore, by
+modifying or distributing the Library (or any work based on the
+Library), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Library or works based on it.
+
+  10. Each time you redistribute the Library (or any work based on the
+Library), the recipient automatically receives a license from the
+original licensor to copy, distribute, link with or modify the Library
+subject to these terms and conditions.  You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties with
+this License.
+
+  11. If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues),
+conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot
+distribute so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you
+may not distribute the Library at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Library by
+all those who receive copies directly or indirectly through you, then
+the only way you could satisfy both it and this License would be to
+refrain entirely from distribution of the Library.
+
+If any portion of this section is held invalid or unenforceable under any
+particular circumstance, the balance of the section is intended to apply,
+and the section as a whole is intended to apply in other circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system which is
+implemented by public license practices.  Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+  12. If the distribution and/or use of the Library is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Library under this License may add
+an explicit geographical distribution limitation excluding those countries,
+so that distribution is permitted only in or among countries not thus
+excluded.  In such case, this License incorporates the limitation as if
+written in the body of this License.
+
+  13. The Free Software Foundation may publish revised and/or new
+versions of the Lesser General Public License from time to time.
+Such new versions will be similar in spirit to the present version,
+but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Library
+specifies a version number of this License which applies to it and
+"any later version", you have the option of following the terms and
+conditions either of that version or of any later version published by
+the Free Software Foundation.  If the Library does not specify a
+license version number, you may choose any version ever published by
+the Free Software Foundation.
+
+  14. If you wish to incorporate parts of the Library into other free
+programs whose distribution conditions are incompatible with these,
+write to the author to ask for permission.  For software which is
+copyrighted by the Free Software Foundation, write to the Free
+Software Foundation; we sometimes make exceptions for this.  Our
+decision will be guided by the two goals of preserving the free status
+of all derivatives of our free software and of promoting the sharing
+and reuse of software generally.
+
+                            NO WARRANTY
+
+  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES.
+
+                     END OF TERMS AND CONDITIONS
+
+           How to Apply These Terms to Your New Libraries
+
+  If you develop a new library, and you want it to be of the greatest
+possible use to the public, we recommend making it free software that
+everyone can redistribute and change.  You can do so by permitting
+redistribution under these terms (or, alternatively, under the terms of the
+ordinary General Public License).
+
+  To apply these terms, attach the following notices to the library.  It is
+safest to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the library's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This library is free software; you can redistribute it and/or
+    modify it under the terms of the GNU Lesser General Public
+    License as published by the Free Software Foundation; either
+    version 2.1 of the License, or (at your option) any later version.
+
+    This library is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+    Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public
+    License along with this library; if not, write to the Free Software
+    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
+    USA
+
+Also add information on how to contact you by electronic and paper mail.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the library, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the
+  library `Frob' (a library for tweaking knobs) written by James Random
+  Hacker.
+
+  <signature of Ty Coon>, 1 April 1990
+  Ty Coon, President of Vice
+
+That's all there is to it!
```

### Comparing `mariadb-1.1.6/PKG-INFO` & `mariadb-1.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 2.1
-Name: mariadb
-Version: 1.1.6
-Summary: Python MariaDB extension
-Home-page: https://www.github.com/mariadb-corporation/mariadb-connector-python
-Author: Georg Richter
-License: LGPL 2.1
-Project-URL: Bug Tracker, https://jira.mariadb.org/
-Project-URL: Documentation, https://mariadb-corporation.github.io/mariadb-connector-python/
-Project-URL: Source Code, https://www.github.com/mariadb-corporation/mariadb-connector-python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <a href="http://mariadb.com/">
-    <img src="https://mariadb.com/kb/static/images/logo-2018-black.png">
-  </a>
-</p>
-
-# MariaDB Connector/Python
-
-[![License (LGPL version 2.1)][licence-image]](LICENSE)
-[![Python 3.7][python-image]][python-url]
-[![Build Status](https://travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)](https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
-<a href="https://scan.coverity.com/projects/mariadb-connector-python">
-  <img alt="Coverity Scan Build Status"
-       src="https://scan.coverity.com/projects/21386/badge.svg"/>
-</a>
-
-MariaDB Connector/Python enables python programs to access MariaDB and MySQL databases, using an API
-which is compliant with the Python DB API 2.0 (PEP-249). It is written in C and uses MariaDB Connector/C
-client library for client server communication.
-
-## License
-
-MariaDB Connector/Python is licensed under the LGPL 2.1
-
-## Source code
-
-MariaDB Connector/Python source code is hosted on [Github](https://github.com/mariadb-corporation/mariadb-connector-python)
-
-## Documentation
-
-MariaDB Connector/Python documentation can be found on [Github Pages](https://mariadb-corporation.github.io/mariadb-connector-python/)
-
-## Bugs
-
-Bugs and feature requests should be filed in the [MariaDB bug ticket system](https://jira.mariadb.org/)
-
-
-[licence-image]:https://img.shields.io/badge/license-GNU%20LGPL%20version%202.1-green.svg?style=flat-square
-[python-image]:https://img.shields.io/badge/python-3.7-blue.svg
-[python-url]:https://www.python.org/downloads/release/python-370/
+Metadata-Version: 2.1
+Name: mariadb
+Version: 1.1.7
+Summary: Python MariaDB extension
+Home-page: https://www.github.com/mariadb-corporation/mariadb-connector-python
+Author: Georg Richter
+License: LGPL 2.1
+Project-URL: Bug Tracker, https://jira.mariadb.org/
+Project-URL: Documentation, https://mariadb-corporation.github.io/mariadb-connector-python/
+Project-URL: Source Code, https://www.github.com/mariadb-corporation/mariadb-connector-python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Topic :: Database
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <a href="http://mariadb.com/">
+    <img src="https://mariadb.com/kb/static/images/logo-2018-black.png">
+  </a>
+</p>
+
+# MariaDB Connector/Python
+
+[![License (LGPL version 2.1)][licence-image]](LICENSE)
+[![Python 3.7][python-image]][python-url]
+[![Build Status](https://travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)](https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
+<a href="https://scan.coverity.com/projects/mariadb-connector-python">
+  <img alt="Coverity Scan Build Status"
+       src="https://scan.coverity.com/projects/21386/badge.svg"/>
+</a>
+
+MariaDB Connector/Python enables python programs to access MariaDB and MySQL databases, using an API
+which is compliant with the Python DB API 2.0 (PEP-249). It is written in C and uses MariaDB Connector/C
+client library for client server communication.
+
+## License
+
+MariaDB Connector/Python is licensed under the LGPL 2.1
+
+## Source code
+
+MariaDB Connector/Python source code is hosted on [Github](https://github.com/mariadb-corporation/mariadb-connector-python)
+
+## Documentation
+
+MariaDB Connector/Python documentation can be found on [Github Pages](https://mariadb-corporation.github.io/mariadb-connector-python/)
+
+## Bugs
+
+Bugs and feature requests should be filed in the [MariaDB bug ticket system](https://jira.mariadb.org/)
+
+
+[licence-image]:https://img.shields.io/badge/license-GNU%20LGPL%20version%202.1-green.svg?style=flat-square
+[python-image]:https://img.shields.io/badge/python-3.7-blue.svg
+[python-url]:https://www.python.org/downloads/release/python-370/
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: mariadb Version: 1.1.6 Summary: Python MariaDB
+Metadata-Version: 2.1 Name: mariadb Version: 1.1.7 Summary: Python MariaDB
 extension Home-page: https://www.github.com/mariadb-corporation/mariadb-
 connector-python Author: Georg Richter License: LGPL 2.1 Project-URL: Bug
 Tracker, https://jira.mariadb.org/ Project-URL: Documentation, https://mariadb-
 corporation.github.io/mariadb-connector-python/ Project-URL: Source Code,
 https://www.github.com/mariadb-corporation/mariadb-connector-python Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: MacOS X Classifier: Environment :: Win32 (MS
 Windows) Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v2 or later (LGPLv2+) Classifier: Programming Language :: C Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: MacOS Classifier: Operating System :: POSIX Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Topic ::
-Database Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Database Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
           [https://mariadb.com/kb/static/images/logo-2018-black.png]
 # MariaDB Connector/Python [![License (LGPL version 2.1)][licence-image]]
 (LICENSE) [![Python 3.7][python-image]][python-url] [![Build Status](https://
 travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)]
 (https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
 [Coverity_Scan_Build_Status] MariaDB Connector/Python enables python programs
```

### Comparing `mariadb-1.1.6/README.md` & `mariadb-1.1.7/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-<p align="center">
-  <a href="http://mariadb.com/">
-    <img src="https://mariadb.com/kb/static/images/logo-2018-black.png">
-  </a>
-</p>
-
-# MariaDB Connector/Python
-
-[![License (LGPL version 2.1)][licence-image]](LICENSE)
-[![Python 3.7][python-image]][python-url]
-[![Build Status](https://travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)](https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
-<a href="https://scan.coverity.com/projects/mariadb-connector-python">
-  <img alt="Coverity Scan Build Status"
-       src="https://scan.coverity.com/projects/21386/badge.svg"/>
-</a>
-
-MariaDB Connector/Python enables python programs to access MariaDB and MySQL databases, using an API
-which is compliant with the Python DB API 2.0 (PEP-249). It is written in C and uses MariaDB Connector/C
-client library for client server communication.
-
-## License
-
-MariaDB Connector/Python is licensed under the LGPL 2.1
-
-## Source code
-
-MariaDB Connector/Python source code is hosted on [Github](https://github.com/mariadb-corporation/mariadb-connector-python)
-
-## Documentation
-
-MariaDB Connector/Python documentation can be found on [Github Pages](https://mariadb-corporation.github.io/mariadb-connector-python/)
-
-## Bugs
-
-Bugs and feature requests should be filed in the [MariaDB bug ticket system](https://jira.mariadb.org/)
-
-
-[licence-image]:https://img.shields.io/badge/license-GNU%20LGPL%20version%202.1-green.svg?style=flat-square
-[python-image]:https://img.shields.io/badge/python-3.7-blue.svg
-[python-url]:https://www.python.org/downloads/release/python-370/
+<p align="center">
+  <a href="http://mariadb.com/">
+    <img src="https://mariadb.com/kb/static/images/logo-2018-black.png">
+  </a>
+</p>
+
+# MariaDB Connector/Python
+
+[![License (LGPL version 2.1)][licence-image]](LICENSE)
+[![Python 3.7][python-image]][python-url]
+[![Build Status](https://travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)](https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
+<a href="https://scan.coverity.com/projects/mariadb-connector-python">
+  <img alt="Coverity Scan Build Status"
+       src="https://scan.coverity.com/projects/21386/badge.svg"/>
+</a>
+
+MariaDB Connector/Python enables python programs to access MariaDB and MySQL databases, using an API
+which is compliant with the Python DB API 2.0 (PEP-249). It is written in C and uses MariaDB Connector/C
+client library for client server communication.
+
+## License
+
+MariaDB Connector/Python is licensed under the LGPL 2.1
+
+## Source code
+
+MariaDB Connector/Python source code is hosted on [Github](https://github.com/mariadb-corporation/mariadb-connector-python)
+
+## Documentation
+
+MariaDB Connector/Python documentation can be found on [Github Pages](https://mariadb-corporation.github.io/mariadb-connector-python/)
+
+## Bugs
+
+Bugs and feature requests should be filed in the [MariaDB bug ticket system](https://jira.mariadb.org/)
+
+
+[licence-image]:https://img.shields.io/badge/license-GNU%20LGPL%20version%202.1-green.svg?style=flat-square
+[python-image]:https://img.shields.io/badge/python-3.7-blue.svg
+[python-url]:https://www.python.org/downloads/release/python-370/
```

### Comparing `mariadb-1.1.6/include/docs/connection.h` & `mariadb-1.1.7/include/docs/connection.h`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-/************************************************************************************
-    Copyright (C) 2019 Georg Richter and MariaDB Corporation AB
-
-   This library is free software; you can redistribute it and/or
-   modify it under the terms of the GNU Library General Public
-   License as published by the Free Software Foundation; either
-   version 2 of the License, or (at your option) any later version.
-
-   This library is distributed in the hope that it will be useful,
-   but WITHOUT ANY WARRANTY; without even the implied warranty of
-   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-   Library General Public License for more details.
-
-   You should have received a copy of the GNU Library General Public
-   License along with this library; if not see <http://www.gnu.org/licenses>
-   or write to the Free Software Foundation, Inc.,
-   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
-*************************************************************************************/
-PyDoc_STRVAR(
-  connection_connect__doc__,
-  __connect__doc__
-);
-
-PyDoc_STRVAR(
-  connection__doc__,
-  "The Connection class is used to open and manage a connection to a\n"
-  "MariaDB or compatible database server"
-);
-
-PyDoc_STRVAR(
-  connection_dump_debug_info__doc__,
-  "dump_debug_info()\n"
-  "--\n"
-  "\n"
-  "This function is designed to be executed by an user with the SUPER privilege\n"
-  "and is used to dump server status information into the log for the MariaDB\n"
-  "Server relating to the connection."
-);
-
-PyDoc_STRVAR(
-  connection_close__doc__,
-  "close()\n"
-  "--\n"
-  "\n"
-  "Close the connection now (rather than whenever .__del__() is called).\n\n"
-  "The connection will be unusable from this point forward; an Error\n"
-  "(or subclass) exception will be raised if any operation is attempted\n"
-  "with the connection. The same applies to all cursor objects trying to\n"
-  "use the connection.\n\n"
-  "Note that closing a connection without committing the changes first\n"
-  "will cause an implicit rollback to be performed."
-);
-
-PyDoc_STRVAR(
-  connection_change_user__doc__,
-  "change_user(user: str, password: str, database: str)\n"
-  "--\n"
-  "\n"
-  "Changes the user and default database of the current connection\n\n"
-  "Parameters:\n"
-  "  - user: user name\n"
-  "  - password: password\n"
-  "  - database: name of default database\n\n"
-  "In order to successfully change users a valid username and password\n"
-  "parameters must be provided and that user must have sufficient\n"
-  "permissions to access the desired database. If for any reason\n"
-  "authorization fails an exception will be raised and the current user\n"
-  "authentication will remain."
-);
-
-PyDoc_STRVAR(
-  connection_reconnect__doc__,
-  "reconnect()\n"
-  "--\n"
-  "\n"
-  "tries to reconnect to a server in case the connection died due to timeout\n"
-  "or other errors. It uses the same credentials which were specified in\n"
-  "connect() method."
-);
-
-PyDoc_STRVAR(
-  connection_reset__doc__,
-  "reset()\n"
-  "--\n"
-  "\n"
-  "Resets the current connection and clears session state and pending\n"
-  "results. Open cursors will become invalid and cannot be used anymore."
-);
-
-PyDoc_STRVAR(
-  connection_escape_string__doc__,
-  "escape_string(statement)\n"
-  "--\n"
-  "\n"
-  "Parameters:\n"
-  "statement: string\n\n"
-  "This function is used to create a legal SQL string that you can use in\n"
-  "an SQL statement. The given string is encoded to an escaped SQL string."
-);
-
-/* ok */
-PyDoc_STRVAR(
-  connection_ping__doc__, 
-  "ping()\n"
-  "--\n"
-  "\n"
-  "Checks if the connection to the database server is still available.\n\n"
-  "If auto reconnect was set to true, an attempt will be made to reconnect\n"
-  "to the database server in case the connection\n"
-  "was lost\n\n"
-  "If the connection is not available an InterfaceError will be raised."
-);
-
-PyDoc_STRVAR(
-  connection_auto_reconnect__doc__,
-  "(read/write)\n\n"
-  "Enable or disable automatic reconnection to the server if the connection\n"
-  "is found to have been lost.\n\n"
-  "When enabled, client tries to reconnect to a database server in case\n"
-  "the connection to a database server died due to timeout or other errors."
-);
-
-PyDoc_STRVAR(
-  connection_warnings__doc__,
-  "Returns the number of warnings from the last executed statement, or zero\n"
-  "if there are no warnings."
-);
+/************************************************************************************
+    Copyright (C) 2019 Georg Richter and MariaDB Corporation AB
+
+   This library is free software; you can redistribute it and/or
+   modify it under the terms of the GNU Library General Public
+   License as published by the Free Software Foundation; either
+   version 2 of the License, or (at your option) any later version.
+
+   This library is distributed in the hope that it will be useful,
+   but WITHOUT ANY WARRANTY; without even the implied warranty of
+   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+   Library General Public License for more details.
+
+   You should have received a copy of the GNU Library General Public
+   License along with this library; if not see <http://www.gnu.org/licenses>
+   or write to the Free Software Foundation, Inc.,
+   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+*************************************************************************************/
+PyDoc_STRVAR(
+  connection_connect__doc__,
+  __connect__doc__
+);
+
+PyDoc_STRVAR(
+  connection__doc__,
+  "The Connection class is used to open and manage a connection to a\n"
+  "MariaDB or compatible database server"
+);
+
+PyDoc_STRVAR(
+  connection_dump_debug_info__doc__,
+  "dump_debug_info()\n"
+  "--\n"
+  "\n"
+  "This function is designed to be executed by an user with the SUPER privilege\n"
+  "and is used to dump server status information into the log for the MariaDB\n"
+  "Server relating to the connection."
+);
+
+PyDoc_STRVAR(
+  connection_close__doc__,
+  "close()\n"
+  "--\n"
+  "\n"
+  "Close the connection now (rather than whenever .__del__() is called).\n\n"
+  "The connection will be unusable from this point forward; an Error\n"
+  "(or subclass) exception will be raised if any operation is attempted\n"
+  "with the connection. The same applies to all cursor objects trying to\n"
+  "use the connection.\n\n"
+  "Note that closing a connection without committing the changes first\n"
+  "will cause an implicit rollback to be performed."
+);
+
+PyDoc_STRVAR(
+  connection_change_user__doc__,
+  "change_user(user: str, password: str, database: str)\n"
+  "--\n"
+  "\n"
+  "Changes the user and default database of the current connection\n\n"
+  "Parameters:\n"
+  "  - user: user name\n"
+  "  - password: password\n"
+  "  - database: name of default database\n\n"
+  "In order to successfully change users a valid username and password\n"
+  "parameters must be provided and that user must have sufficient\n"
+  "permissions to access the desired database. If for any reason\n"
+  "authorization fails an exception will be raised and the current user\n"
+  "authentication will remain."
+);
+
+PyDoc_STRVAR(
+  connection_reconnect__doc__,
+  "reconnect()\n"
+  "--\n"
+  "\n"
+  "tries to reconnect to a server in case the connection died due to timeout\n"
+  "or other errors. It uses the same credentials which were specified in\n"
+  "connect() method."
+);
+
+PyDoc_STRVAR(
+  connection_reset__doc__,
+  "reset()\n"
+  "--\n"
+  "\n"
+  "Resets the current connection and clears session state and pending\n"
+  "results. Open cursors will become invalid and cannot be used anymore."
+);
+
+PyDoc_STRVAR(
+  connection_escape_string__doc__,
+  "escape_string(statement)\n"
+  "--\n"
+  "\n"
+  "Parameters:\n"
+  "statement: string\n\n"
+  "This function is used to create a legal SQL string that you can use in\n"
+  "an SQL statement. The given string is encoded to an escaped SQL string."
+);
+
+/* ok */
+PyDoc_STRVAR(
+  connection_ping__doc__, 
+  "ping()\n"
+  "--\n"
+  "\n"
+  "Checks if the connection to the database server is still available.\n\n"
+  "If auto reconnect was set to true, an attempt will be made to reconnect\n"
+  "to the database server in case the connection\n"
+  "was lost\n\n"
+  "If the connection is not available an InterfaceError will be raised."
+);
+
+PyDoc_STRVAR(
+  connection_auto_reconnect__doc__,
+  "(read/write)\n\n"
+  "Enable or disable automatic reconnection to the server if the connection\n"
+  "is found to have been lost.\n\n"
+  "When enabled, client tries to reconnect to a database server in case\n"
+  "the connection to a database server died due to timeout or other errors."
+);
+
+PyDoc_STRVAR(
+  connection_warnings__doc__,
+  "Returns the number of warnings from the last executed statement, or zero\n"
+  "if there are no warnings."
+);
```

### Comparing `mariadb-1.1.6/include/docs/exception.h` & `mariadb-1.1.7/include/docs/exception.h`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-/*****************************************************************************
-   Copyright (C) 2020 Georg Richter and MariaDB Corporation AB
-
-   This library is free software; you can redistribute it and/or
-   modify it under the terms of the GNU Library General Public
-   License as published by the Free Software Foundation; either
-   version 2 of the License, or (at your option) any later version.
-
-   This library is distributed in the hope that it will be useful,
-   but WITHOUT ANY WARRANTY; without even the implied warranty of
-   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-   Library General Public License for more details.
-
-   You should have received a copy of the GNU Library General Public
-   License along with this library; if not see <http://www.gnu.org/licenses>
-   or write to the Free Software Foundation, Inc.,
-   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
-******************************************************************************/
-
-PyDoc_STRVAR(
-    exception_interface__doc__,
-    "Exception raised for errors that are related to the database interface "\
-    "rather than the database itself"
-);
-
-PyDoc_STRVAR(
-    exception_warning__doc__,
-    "Exception raised for important warnings like data truncations "\
-    "while inserting, etc"
-);
-
-PyDoc_STRVAR(
-    exception_database__doc__,
-   "Exception raised for errors that are related to the database"
-);
-
-PyDoc_STRVAR(
-    exception_data__doc__,
-    "Exception raised for errors that are due to problems with the "\
-    "processed data like division by zero, numeric value out of range, etc."
-);
-
-PyDoc_STRVAR(
-    exception_pool__doc__,
-    "Exception raised for errors related to ConnectionPool class."
-);
-
-PyDoc_STRVAR(
-    exception_operational__doc__,
-    "Exception raised for errors that are related to the database's "\
-    "operation and not necessarily under the control of the programmer."
-);
-
-PyDoc_STRVAR(
-    exception_integrity__doc__,
-    "Exception raised when the relational integrity of the database "\
-    "is affected, e.g. a foreign key check fails"
-);
-
-PyDoc_STRVAR(
-    exception_internal__doc__,
-    "Exception raised when the database encounters an internal error, "\
-    "e.g. the cursor is not valid anymore";
-);
-
-PyDoc_STRVAR(
-    exception_programming__doc__,
-    "Exception raised for programming errors, e.g. table not found or "\
-    "already exists, syntax error in the SQL statement"
-);
-
-PyDoc_STRVAR(
-    exception_notsupported__doc__,
-    "Exception raised in case a method or database API was used which is "\
-    "not supported by the database"
-);
+/*****************************************************************************
+   Copyright (C) 2020 Georg Richter and MariaDB Corporation AB
+
+   This library is free software; you can redistribute it and/or
+   modify it under the terms of the GNU Library General Public
+   License as published by the Free Software Foundation; either
+   version 2 of the License, or (at your option) any later version.
+
+   This library is distributed in the hope that it will be useful,
+   but WITHOUT ANY WARRANTY; without even the implied warranty of
+   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+   Library General Public License for more details.
+
+   You should have received a copy of the GNU Library General Public
+   License along with this library; if not see <http://www.gnu.org/licenses>
+   or write to the Free Software Foundation, Inc.,
+   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+******************************************************************************/
+
+PyDoc_STRVAR(
+    exception_interface__doc__,
+    "Exception raised for errors that are related to the database interface "\
+    "rather than the database itself"
+);
+
+PyDoc_STRVAR(
+    exception_warning__doc__,
+    "Exception raised for important warnings like data truncations "\
+    "while inserting, etc"
+);
+
+PyDoc_STRVAR(
+    exception_database__doc__,
+   "Exception raised for errors that are related to the database"
+);
+
+PyDoc_STRVAR(
+    exception_data__doc__,
+    "Exception raised for errors that are due to problems with the "\
+    "processed data like division by zero, numeric value out of range, etc."
+);
+
+PyDoc_STRVAR(
+    exception_pool__doc__,
+    "Exception raised for errors related to ConnectionPool class."
+);
+
+PyDoc_STRVAR(
+    exception_operational__doc__,
+    "Exception raised for errors that are related to the database's "\
+    "operation and not necessarily under the control of the programmer."
+);
+
+PyDoc_STRVAR(
+    exception_integrity__doc__,
+    "Exception raised when the relational integrity of the database "\
+    "is affected, e.g. a foreign key check fails"
+);
+
+PyDoc_STRVAR(
+    exception_internal__doc__,
+    "Exception raised when the database encounters an internal error, "\
+    "e.g. the cursor is not valid anymore";
+);
+
+PyDoc_STRVAR(
+    exception_programming__doc__,
+    "Exception raised for programming errors, e.g. table not found or "\
+    "already exists, syntax error in the SQL statement"
+);
+
+PyDoc_STRVAR(
+    exception_notsupported__doc__,
+    "Exception raised in case a method or database API was used which is "\
+    "not supported by the database"
+);
```

### Comparing `mariadb-1.1.6/include/mariadb_python.h` & `mariadb-1.1.7/include/mariadb_python.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,773 +1,774 @@
-/******************************************************************************
-    Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
-
-   This library is free software; you can redistribute it and/or
-   modify it under the terms of the GNU Library General Public
-   License as published by the Free Software Foundation; either
-   version 2 of the License, or (at your option) any later version.
-
-   This library is distributed in the hope that it will be useful,
-   but WITHOUT ANY WARRANTY; without even the implied warranty of
-   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-   Library General Public License for more details.
-
-   You should have received a copy of the GNU Library General Public
-   License along with this library; if not see <http://www.gnu.org/licenses>
-   or write to the Free Software Foundation, Inc.,
-   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
-******************************************************************************/
-#define PY_SSIZE_T_CLEAN
-
-#include "Python.h"
-#include "bytesobject.h"
-#include "structmember.h"
-#include "structseq.h"
-#include <stdarg.h>
-#include <stdint.h>
-#include <mysql.h>
-#include <errmsg.h>
-#include <mysqld_error.h>
-#include <time.h>
-#include <docs/common.h>
-#include <limits.h>
-
-#define CHECK_TYPE(obj, type) \
-(Py_TYPE((obj)) == type || PyType_IsSubtype(Py_TYPE((obj)), type))
-
-#if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_TYPE)
-static inline void _Py_SET_TYPE(PyObject *ob, PyTypeObject *type)
-{ ob->ob_type = type; }
-#define Py_SET_TYPE(ob, type) _Py_SET_TYPE((PyObject*)(ob), type)
-#endif
-
-#if defined(_WIN32)
-#include <config_win.h>
-#include <windows.h>
-#ifdef _MSC_VER
-typedef SSIZE_T ssize_t;
-#endif
-typedef CRITICAL_SECTION pthread_mutex_t;
-#define pthread_mutex_init(A,B)  InitializeCriticalSection(A)
-#define pthread_mutex_lock(A)	 (EnterCriticalSection(A),0)
-#define pthread_mutex_unlock(A)  LeaveCriticalSection(A)
-#define pthread_mutex_destroy(A) DeleteCriticalSection(A)
-#define pthread_self() GetCurrentThreadId()
-#include <malloc.h>
-#else
-#include <pthread.h>
-#include <limits.h>
-#endif /* defined(_WIN32) */
-
-
-#ifndef MIN
-#define MIN(a,b) (a) < (b) ? (a) : (b)
-#endif
-
-#ifndef MAX
-#define MAX(a,b) (a) > (b) ? (a) : (b)
-#endif
-
-#if !defined(__GNUC__) && !defined(__clang__)
-#define __attribute__(A)
-#endif
-
-#ifdef _WIN32
-int clock_gettime(int dummy, struct timespec *ct);
-#define CLOCK_MONOTONIC_RAW 1
-#endif
-
-#define REQUIRED_CC_VERSION 30103
-
-#if MARIADB_PACKAGE_VERSION_ID < REQUIRED_CC_VERSION
-#error Minimum required version of MariaDB Connector/C is 3.1.3
-#endif
-
-#if defined(_WIN32) && defined(_MSVC)
-#ifndef L64
-#define L64(x) x##i64
-#endif
-#else
-#ifndef L64
-#define L64(x) x##LL
-#endif /* L64 */
-#endif /* _WIN32 */
-
-#define STRINGIFY(n) #n
-#define TOSTRING(n) STRINGIFY(n)
-
-#define PY_MARIADB_VERSION TOSTRING(PY_MARIADB_MAJOR_VERSION) "." \
-        TOSTRING(PY_MARIADB_MINOR_VERSION) "." TOSTRING(PY_MARIADB_PATCH_VERSION)
-
-#define MAX_TPC_XID_SIZE 64
-#define POOL_DEFAULT_SIZE 5
-
-/* Placeholder for missing documentation */
-#define MISSING_DOC NULL
-
-/* Magic constant for checking dynamic columns */
-#define PYTHON_DYNCOL_VALUE 0xA378BD8E
-
-typedef struct st_lex_str {
-    char *str;
-    size_t length;
-} MrdbString;
-
-enum enum_binary_command {
-    SQL_NONE= 0,
-    SQL_INSERT,
-    SQL_UPDATE,
-    SQL_REPLACE,
-    SQL_DELETE,
-    SQL_CALL,
-    SQL_DO,
-    SQL_SELECT,
-    SQL_OTHER=255
-};
-
-enum enum_extended_field_type
-{
-  EXT_TYPE_NONE=0,
-  EXT_TYPE_JSON=1
-};
-
-enum enum_result_format
-{
-    RESULT_TUPLE= 0,
-    RESULT_NAMED_TUPLE,
-    RESULT_DICTIONARY
-};
-
-enum enum_dyncol_type
-{
-    DYNCOL_LIST= 1,
-    DYNCOL_TUPLE,
-    DYNCOL_SET,
-    DYNCOL_DICT,
-    DYNCOL_ODICT,
-    DYNCOL_LAST
-};
-
-enum enum_tpc_state
-{
-    TPC_STATE_NONE= 0,
-    TPC_STATE_XID,
-    TPC_STATE_PREPARE
-};
-
-enum enum_paramstyle
-{
-    NONE= 0,
-    QMARK= 1,
-    FORMAT= 2,
-    PYFORMAT= 3
-};
-
-typedef struct st_parser {
-    MrdbString statement;
-    MrdbString *keys;
-    uint8_t in_literal[3];
-    uint8_t in_comment;
-    uint8_t in_values;
-    uint8_t is_insert;
-    uint8_t comment_eol;
-    uint32_t param_count;
-    uint32_t key_count;
-    char* value_ofs;
-    PyObject *param_list;
-    enum enum_paramstyle paramstyle;
-    enum enum_binary_command command;
-    MYSQL *mysql;
-} MrdbParser;
-
-/* PEP-249: Connection object */
-typedef struct {
-    PyObject_HEAD
-    PyThreadState *thread_state;
-    MYSQL *mysql;
-    int open;
-    uint8_t is_buffered;
-    uint8_t is_closed;
-    enum enum_tpc_state tpc_state;
-    char xid[150]; /* large enough, to hold 2 * MAX_TPC_XID size + integer value */
-    PyObject *dsn; /* always null */
-    const char *host;
-/*    const char *tls_cipher;
-    const char *tls_version;
-    const char *unix_socket;
-    int port;
-    const char *charset;
-    const char *collation; */
-    uint8_t inuse;
-    uint8_t status;
-    uint8_t asynchronous;
-    struct timespec last_used;
-    unsigned long thread_id;
-    char *server_info;
-    uint8_t closed;
-#if MARIADB_PACKAGE_VERSION_ID > 30301
-    PyObject *status_callback;
-#endif
-    PyObject *last_executed_stmt;
-    PyObject *converter;
-} MrdbConnection;
-
-typedef struct {
-    enum enum_field_types type;
-    PyObject *Value;
-    uint8_t indicator;
-} Mariadb_Value;
-
-/* Parameter info for cursor.executemany()
-   operations */
-typedef struct {
-    enum enum_field_types type;
-    size_t bits; /* for PyLong Object */
-    PyTypeObject *ob_type;
-    uint8_t has_indicator;
-} MrdbParamInfo;
-
-typedef struct {
-    PyObject *value;
-    char indicator;
-    enum enum_field_types type;
-    size_t length;
-    uint8_t free_me;
-    void *buffer;
-    unsigned char num[8];
-    MYSQL_TIME tm;
-} MrdbParamValue;
-
-typedef struct {
-    char *statement;
-    Py_ssize_t statement_len;
-    enum enum_paramstyle paramstyle;
-    enum enum_binary_command command;
-    uint32_t paramcount;
-    uint8_t is_text;
-    PyObject *paramlist;
-    PyObject *keys;
-} MrdbParseInfo;
-
-/* PEP-249: Cursor object */
-typedef struct {
-    PyObject_HEAD
-    MrdbConnection *connection;
-    MYSQL_STMT *stmt;
-    MYSQL_RES *result;
-    PyObject *data;
-    uint32_t array_size;
-    uint32_t row_array_size; /* for fetch many */
-    MrdbParamInfo *paraminfo;
-    MrdbParamValue *value;
-    MYSQL_BIND *params;
-    MYSQL_BIND *bind;
-    MYSQL_FIELD *fields;
-    char *statement;
-    size_t statement_len;
-    PyObject **values;
-    PyStructSequence_Field *sequence_fields;
-    PyTypeObject *sequence_type;
-    MrdbParseInfo parseinfo;
-    unsigned long prefetch_rows;
-    unsigned long cursor_type;
-    int64_t affected_rows;
-    uint32_t field_count;
-    int64_t row_count;
-    uint64_t lastrow_id;
-    unsigned long row_number;
-    enum enum_result_format result_format;
-    uint8_t is_prepared;
-    char is_buffered;
-    uint8_t fetched;
-    uint8_t closed;
-    uint8_t reprepare;
-    enum enum_paramstyle paramstyle;
-} MrdbCursor;
-
-typedef struct
-{
-    PyObject_HEAD
-} Mariadb_Fieldinfo;
-
-typedef struct {
-    ps_field_fetch_func func;
-    int pack_len;
-    unsigned long max_len;
-} Mariadb_Conversion;
-
-extern char *dsn_keys[];
-
-/* Exceptions */
-extern PyObject *Mariadb_InterfaceError;
-extern PyObject *Mariadb_Error;
-extern PyObject *Mariadb_DatabaseError;
-extern PyObject *Mariadb_DataError;
-extern PyObject *Mariadb_PoolError;
-extern PyObject *Mariadb_OperationalError;
-extern PyObject *Mariadb_IntegrityError;
-extern PyObject *Mariadb_InternalError;
-extern PyObject *Mariadb_ProgrammingError;
-extern PyObject *Mariadb_NotSupportedError;
-extern PyObject *Mariadb_Warning;
-
-extern PyObject *decimal_module,
-                *decimal_type;
-
-/* Object types */
-extern PyTypeObject MrdbPool_Type;
-extern PyTypeObject Mariadb_Fieldinfo_Type;
-extern PyTypeObject MrdbConnection_Type;
-extern PyTypeObject MrdbCursor_Type;
-
-int Mariadb_traverse(PyObject *self,
-    visitproc visit,
-    void *arg);
-
-/* Function prototypes */
-void
-mariadb_throw_exception(void *handle,
-    PyObject *execption_type,
-    int8_t is_statement,
-    const char *message,
-    ...);
-
-enum enum_extended_field_type mariadb_extended_field_type(const MYSQL_FIELD *field);
-
-PyObject *
-MrdbConnection_ping(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_kill(MrdbConnection *self, PyObject *args);
-
-PyObject *
-MrdbConnection_reconnect(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_reset(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_autocommit(MrdbConnection *self, PyObject *args);
-
-PyObject *
-MrdbConnection_change_user(MrdbConnection *self, PyObject *args);
-
-PyObject
-*MrdbConnection_rollback(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_commit(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_close(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_connect( PyObject *self,PyObject *args,	PyObject *kwargs);
-
-void
-MrdbConnection_SetAttributes(MrdbConnection *self);
-
-/* TPC methods */
-PyObject *
-MrdbConnection_xid(MrdbConnection *self, PyObject *args);
-
-PyObject *
-MrdbConnection_tpc_begin(MrdbConnection *self, PyObject *args);
-
-PyObject *
-MrdbConnection_tpc_commit(MrdbConnection *self, PyObject *args);
-
-PyObject *
-MrdbConnection_tpc_rollback(MrdbConnection *self, PyObject *args);
-
-PyObject *
-MrdbConnection_tpc_prepare(MrdbConnection *self);
-
-PyObject *
-MrdbConnection_tpc_recover(MrdbConnection *self);
-
-/* codecs prototypes  */
-uint8_t
-mariadb_check_bulk_parameters(MrdbCursor *self, PyObject *data);
-
-uint8_t
-mariadb_check_execute_parameters(MrdbCursor *self, PyObject *data);
-
-uint8_t
-mariadb_param_update(void *data, MYSQL_BIND *bind, uint32_t row_nr);
-
-/* parser prototypes */
-MrdbParser *
-MrdbParser_init(MYSQL *mysql, const char *statement, size_t length);
-
-void
-MrdbParser_end(MrdbParser *p);
-
-uint8_t
-MrdbParser_parse(MrdbParser *p, uint8_t is_batch, char *errmsg, size_t errmsg_len);
-
-/* Global defines */
-
-
-#define MARIADB_PY_APILEVEL "2.0"
-#define MARIADB_PY_PARAMSTYLE "qmark"
-#define MARIADB_PY_THREADSAFETY 1
-
-#define MAX_POOL_SIZE 64
-
-#define TIMEDIFF(a,b)\
-  ((a).tv_sec * (uint64_t)1E09 + (a).tv_nsec) -\
-  ((b).tv_sec * (uint64_t)1E09 + (b).tv_nsec)
-
-/* Helper macros */
-
-#define MrdbIndicator_Check(a)\
-      (PyObject_HasAttrString(a, "indicator"))
-
-#define MARIADB_CHECK_CONNECTION(connection, ret)\
-    if (!(connection) || !(connection)->mysql)\
-    {\
-        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0, \
-           "Invalid connection or not connected");\
-        return (ret);\
-    }
-
-#define MARIADB_CHECK_TPC(connection)\
-  if (connection->tpc_state == TPC_STATE_NONE)\
-  {\
-      mariadb_throw_exception(connection->mysql, Mariadb_ProgrammingError, 0,\
-          "Transaction not started");\
-      return NULL;\
-  }
-
-#define MARIADB_FREE_MEM(a)\
-    if (a)\
-    {\
-        PyMem_RawFree((a));\
-        (a)= NULL;\
-    }
-
-#define MARIADB_CHECK_STMT(cursor)\
-    if (!cursor->connection->mysql || cursor->closed)\
-    {\
-       (cursor)->closed= 1;\
-        mariadb_throw_exception(cursor->stmt, Mariadb_ProgrammingError, 1,\
-      "Invalid cursor or not connected");\
-    }
-
-
-
-// #define pooling_keywords "pool_name", "pool_size", "reset_session", "idle_timeout", "acquire_timeout"
-#define connection_keywords "dsn", "host", "user", "password", "database", "port", "socket",\
-  "connect_timeout", "read_timeout", "write_timeout",\
-"local_infile", "compress", "init_command",\
-"default_file", "default_group",\
-"ssl_key", "ssl_ca", "ssl_cert", "ssl_crl",\
-"ssl_cipher", "ssl_capath", "ssl_crlpath",\
-"ssl_verify_cert", "ssl",\
-"client_flags", "charset"
-
-/* MariaDB protocol macros */
-#define int1store(T,A) *((int8_t*) (T)) = (A)
-#define uint1korr(A)   (*(((uint8_t*)(A))))
-#if defined(__i386__) || defined(_WIN32)
-#define sint2korr(A)	(*((int16_t *) (A)))
-#define sint3korr(A)	((int32_t) ((((unsigned char) (A)[2]) & 128) ? \
-      (((uint32_t) 255L << 24) | \
-       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
-       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
-       ((uint32_t) (unsigned char) (A)[0])) : \
-       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
-       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
-       ((uint32_t) (unsigned char) (A)[0])))
-#define sint4korr(A)	(*((long *) (A)))
-#define uint2korr(A)	(*((uint16_t *) (A)))
-#if defined(HAVE_purify) && !defined(_WIN32)
-#define uint3korr(A)	(uint32_t) (((uint32_t) ((unsigned char) (A)[0])) +\
-    (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
-    (((uint32_t) ((unsigned char) (A)[2])) << 16))
-#else
-          /*
-             ATTENTION !
-
-             Please, note, uint3korr reads 4 bytes (not 3) !
-             It means, that you have to provide enough allocated space !
-           */
-#define uint3korr(A)	(long) (*((unsigned int *) (A)) & 0xFFFFFF)
-#endif /* HAVE_purify && !_WIN32 */
-#define uint4korr(A)	(*((uint32_t *) (A)))
-#define uint5korr(A)	((unsigned long long)(((uint32_t) ((unsigned char) (A)[0])) +\
-      (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
-      (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
-      (((uint32_t) ((unsigned char) (A)[3])) << 24)) +\
-      (((unsigned long long) ((unsigned char) (A)[4])) << 32))
-#define uint6korr(A)	((unsigned long long)(((uint32_t)    ((unsigned char) (A)[0]))          + \
-      (((uint32_t)    ((unsigned char) (A)[1])) << 8)   + \
-      (((uint32_t)    ((unsigned char) (A)[2])) << 16)  + \
-      (((uint32_t)    ((unsigned char) (A)[3])) << 24)) + \
-      (((unsigned long long) ((unsigned char) (A)[4])) << 32) +       \
-      (((unsigned long long) ((unsigned char) (A)[5])) << 40))
-#define uint8_tkorr(A)	(*((unsigned long long *) (A)))
-#define sint8korr(A)	(*((long long *) (A)))
-#define int2store(T,A)	*((uint16_t*) (T))= (uint16_t) (A)
-#define int3store(T,A)  do { *(T)=  (unsigned char) ((A));\
-  *(T+1)=(unsigned char) (((uint) (A) >> 8));\
-  *(T+2)=(unsigned char) (((A) >> 16)); } while (0)
-#define int4store(T,A)	*((long *) (T))= (long) (A)
-#define int5store(T,A)  do { *(T)= (unsigned char)((A));\
-  *((T)+1)=(unsigned char) (((A) >> 8));\
-  *((T)+2)=(unsigned char) (((A) >> 16));\
-  *((T)+3)=(unsigned char) (((A) >> 24)); \
-  *((T)+4)=(unsigned char) (((A) >> 32)); } while(0)
-#define int6store(T,A)  do { *(T)=    (unsigned char)((A));          \
-  *((T)+1)=(unsigned char) (((A) >> 8));  \
-  *((T)+2)=(unsigned char) (((A) >> 16)); \
-  *((T)+3)=(unsigned char) (((A) >> 24)); \
-  *((T)+4)=(unsigned char) (((A) >> 32)); \
-  *((T)+5)=(unsigned char) (((A) >> 40)); } while(0)
-#define int8store(T,A)	*((unsigned long long *) (T))= (unsigned long long) (A)
-
-          typedef union {
-            double v;
-            long m[2];
-          } doubleget_union;
-#define doubleget(V,M)	\
-  do { doubleget_union _tmp; \
-    _tmp.m[0] = *((long*)(M)); \
-    _tmp.m[1] = *(((long*) (M))+1); \
-    (V) = _tmp.v; } while(0)
-#define doublestore(T,V) do { *((long *) T) = ((doubleget_union *)&V)->m[0]; \
-  *(((long *) T)+1) = ((doubleget_union *)&V)->m[1]; \
-} while (0)
-#define float4get(V,M)   do { *((float *) &(V)) = *((float*) (M)); } while(0)
-#define float8get(V,M)   doubleget((V),(M))
-#define float4store(V,M) memcpy((unsigned char*) V,(unsigned char*) (&M),sizeof(float))
-#define floatstore(T,V)  memcpy((unsigned char*)(T), (unsigned char*)(&V),sizeof(float))
-#define floatget(V,M)    memcpy((unsigned char*) &V,(unsigned char*) (M),sizeof(float))
-#define float8store(V,M) doublestore((V),(M))
-#else
-
-/*
-   We're here if it's not a IA-32 architecture (Win32 and UNIX IA-32 defines
-   were done before)
- */
-#define sint2korr(A)	(int16_t) (((int16_t) ((unsigned char) (A)[0])) +\
-    ((int16_t) ((int16_t) (A)[1]) << 8))
-#define sint3korr(A)	((int32_t) ((((unsigned char) (A)[2]) & 128) ? \
-      (((uint32_t) 255L << 24) | \
-       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
-       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
-       ((uint32_t) (unsigned char) (A)[0])) : \
-       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
-       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
-       ((uint32_t) (unsigned char) (A)[0])))
-#define sint4korr(A)	(int32_t) (((int32_t) ((unsigned char) (A)[0])) +\
-    (((int32_t) ((unsigned char) (A)[1]) << 8)) +\
-    (((int32_t) ((unsigned char) (A)[2]) << 16)) +\
-    (((int32_t) ((int16_t) (A)[3]) << 24)))
-#define sint8korr(A)	(long long) uint8korr(A)
-#define uint2korr(A)	(uint16_t) (((uint16_t) ((unsigned char) (A)[0])) +\
-    ((uint16_t) ((unsigned char) (A)[1]) << 8))
-#define uint3korr(A)	(uint32_t) (((uint32_t) ((unsigned char) (A)[0])) +\
-    (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
-    (((uint32_t) ((unsigned char) (A)[2])) << 16))
-#define uint4korr(A)	(uint32_t) (((uint32_t) ((unsigned char) (A)[0])) +\
-    (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
-    (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
-    (((uint32_t) ((unsigned char) (A)[3])) << 24))
-#define uint5korr(A)	((unsigned long long)(((uint32_t) ((unsigned char) (A)[0])) +\
-      (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
-      (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
-      (((uint32_t) ((unsigned char) (A)[3])) << 24)) +\
-      (((unsigned long long) ((unsigned char) (A)[4])) << 32))
-#define uint6korr(A)	((unsigned long long)(((uint32_t)    ((unsigned char) (A)[0]))          + \
-      (((uint32_t)    ((unsigned char) (A)[1])) << 8)   + \
-      (((uint32_t)    ((unsigned char) (A)[2])) << 16)  + \
-      (((uint32_t)    ((unsigned char) (A)[3])) << 24)) + \
-      (((unsigned long long) ((unsigned char) (A)[4])) << 32) +       \
-      (((unsigned long long) ((unsigned char) (A)[5])) << 40))
-#define uint8korr(A)	((unsigned long long)(((uint32_t) ((unsigned char) (A)[0])) +\
-      (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
-      (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
-      (((uint32_t) ((unsigned char) (A)[3])) << 24)) +\
-      (((unsigned long long) (((uint32_t) ((unsigned char) (A)[4])) +\
-                              (((uint32_t) ((unsigned char) (A)[5])) << 8) +\
-                              (((uint32_t) ((unsigned char) (A)[6])) << 16) +\
-                              (((uint32_t) ((unsigned char) (A)[7])) << 24))) <<\
-                              32))
-#define int2store(T,A)       do { uint def_temp= (uint) (A) ;\
-  *((unsigned char*) (T))=  (unsigned char)(def_temp); \
-  *((unsigned char*) (T)+1)=(unsigned char)((def_temp >> 8)); \
-} while(0)
-#define int3store(T,A)       do { /*lint -save -e734 */\
-  *((unsigned char*)(T))=(unsigned char) ((A));\
-  *((unsigned char*) (T)+1)=(unsigned char) (((A) >> 8));\
-  *((unsigned char*)(T)+2)=(unsigned char) (((A) >> 16)); \
-  /*lint -restore */} while(0)
-#define int4store(T,A)       do { *((char *)(T))=(char) ((A));\
-  *(((char *)(T))+1)=(char) (((A) >> 8));\
-  *(((char *)(T))+2)=(char) (((A) >> 16));\
-  *(((char *)(T))+3)=(char) (((A) >> 24)); } while(0)
-#define int5store(T,A)       do { *((char *)(T))=     (char)((A));  \
-  *(((char *)(T))+1)= (char)(((A) >> 8)); \
-  *(((char *)(T))+2)= (char)(((A) >> 16)); \
-  *(((char *)(T))+3)= (char)(((A) >> 24)); \
-  *(((char *)(T))+4)= (char)(((A) >> 32)); \
-} while(0)
-#define int6store(T,A)       do { *((char *)(T))=     (char)((A)); \
-  *(((char *)(T))+1)= (char)(((A) >> 8)); \
-  *(((char *)(T))+2)= (char)(((A) >> 16)); \
-  *(((char *)(T))+3)= (char)(((A) >> 24)); \
-  *(((char *)(T))+4)= (char)(((A) >> 32)); \
-  *(((char *)(T))+5)= (char)(((A) >> 40)); \
-} while(0)
-#define int8store(T,A)       do { uint def_temp= (uint) (A), def_temp2= (uint) ((A) >> 32); \
-  int4store((T),def_temp); \
-  int4store((T+4),def_temp2); } while(0)
-#ifdef WORDS_BIGENDIAN
-#define float4store(T,A) do { *(T)= ((unsigned char *) &A)[3];\
-  *((T)+1)=(char) ((unsigned char *) &A)[2];\
-  *((T)+2)=(char) ((unsigned char *) &A)[1];\
-  *((T)+3)=(char) ((unsigned char *) &A)[0]; } while(0)
-
-#define float4get(V,M)   do { float def_temp;\
-  ((unsigned char*) &def_temp)[0]=(M)[3];\
-  ((unsigned char*) &def_temp)[1]=(M)[2];\
-  ((unsigned char*) &def_temp)[2]=(M)[1];\
-  ((unsigned char*) &def_temp)[3]=(M)[0];\
-  (V)=def_temp; } while(0)
-#define float8store(T,V) do { *(T)= ((unsigned char *) &V)[7];\
-  *((T)+1)=(char) ((unsigned char *) &V)[6];\
-  *((T)+2)=(char) ((unsigned char *) &V)[5];\
-  *((T)+3)=(char) ((unsigned char *) &V)[4];\
-  *((T)+4)=(char) ((unsigned char *) &V)[3];\
-  *((T)+5)=(char) ((unsigned char *) &V)[2];\
-  *((T)+6)=(char) ((unsigned char *) &V)[1];\
-  *((T)+7)=(char) ((unsigned char *) &V)[0]; } while(0)
-
-#define float8get(V,M)   do { double def_temp;\
-  ((unsigned char*) &def_temp)[0]=(M)[7];\
-  ((unsigned char*) &def_temp)[1]=(M)[6];\
-  ((unsigned char*) &def_temp)[2]=(M)[5];\
-  ((unsigned char*) &def_temp)[3]=(M)[4];\
-  ((unsigned char*) &def_temp)[4]=(M)[3];\
-  ((unsigned char*) &def_temp)[5]=(M)[2];\
-  ((unsigned char*) &def_temp)[6]=(M)[1];\
-  ((unsigned char*) &def_temp)[7]=(M)[0];\
-  (V) = def_temp; } while(0)
-#else
-#define float4get(V,M)   memcpy(&V, (M), sizeof(float))
-#define float4store(V,M) memcpy(V, (&M), sizeof(float))
-
-#if defined(__FLOAT_WORD_ORDER) && (__FLOAT_WORD_ORDER == __BIG_ENDIAN)
-#define doublestore(T,V) do { *(((char*)T)+0)=(char) ((unsigned char *) &V)[4];\
-  *(((char*)T)+1)=(char) ((unsigned char *) &V)[5];\
-  *(((char*)T)+2)=(char) ((unsigned char *) &V)[6];\
-  *(((char*)T)+3)=(char) ((unsigned char *) &V)[7];\
-  *(((char*)T)+4)=(char) ((unsigned char *) &V)[0];\
-  *(((char*)T)+5)=(char) ((unsigned char *) &V)[1];\
-  *(((char*)T)+6)=(char) ((unsigned char *) &V)[2];\
-  *(((char*)T)+7)=(char) ((unsigned char *) &V)[3]; }\
-          while(0)
-#define doubleget(V,M)   do { double def_temp;\
-  ((unsigned char*) &def_temp)[0]=(M)[4];\
-  ((unsigned char*) &def_temp)[1]=(M)[5];\
-  ((unsigned char*) &def_temp)[2]=(M)[6];\
-  ((unsigned char*) &def_temp)[3]=(M)[7];\
-  ((unsigned char*) &def_temp)[4]=(M)[0];\
-  ((unsigned char*) &def_temp)[5]=(M)[1];\
-  ((unsigned char*) &def_temp)[6]=(M)[2];\
-  ((unsigned char*) &def_temp)[7]=(M)[3];\
-  (V) = def_temp; } while(0)
-#endif /* __FLOAT_WORD_ORDER */
-
-#define float8get(V,M)   doubleget((V),(M))
-#define float8store(V,M) doublestore((V),(M))
-#endif /* WORDS_BIGENDIAN */
-
-#ifdef HAVE_BIGENDIAN
-
-#define ushortget(V,M)  do { V = (uint16_t) (((uint16_t) ((unsigned char) (M)[1]))+\
-    ((uint16_t) ((uint16_t) (M)[0]) << 8)); } while(0)
-#define shortget(V,M)   do { V = (short) (((short) ((unsigned char) (M)[1]))+\
-    ((short) ((short) (M)[0]) << 8)); } while(0)
-#define longget(V,M)    do { int32 def_temp;\
-  ((unsigned char*) &def_temp)[0]=(M)[0];\
-  ((unsigned char*) &def_temp)[1]=(M)[1];\
-  ((unsigned char*) &def_temp)[2]=(M)[2];\
-  ((unsigned char*) &def_temp)[3]=(M)[3];\
-  (V)=def_temp; } while(0)
-#define ulongget(V,M)   do { uint32 def_temp;\
-  ((unsigned char*) &def_temp)[0]=(M)[0];\
-  ((unsigned char*) &def_temp)[1]=(M)[1];\
-  ((unsigned char*) &def_temp)[2]=(M)[2];\
-  ((unsigned char*) &def_temp)[3]=(M)[3];\
-  (V)=def_temp; } while(0)
-#define shortstore(T,A) do { uint def_temp=(uint) (A) ;\
-  *(((char*)T)+1)=(char)(def_temp); \
-  *(((char*)T)+0)=(char)(def_temp >> 8); } while(0)
-#define longstore(T,A)  do { *(((char*)T)+3)=((A));\
-  *(((char*)T)+2)=(((A) >> 8));\
-  *(((char*)T)+1)=(((A) >> 16));\
-  *(((char*)T)+0)=(((A) >> 24)); } while(0)
-
-#define floatget(V,M)    memcpy(&V, (M), sizeof(float))
-#define floatstore(T,V)  memcpy((T), (void*) (&V), sizeof(float))
-#define doubleget(V,M)	 memcpy(&V, (M), sizeof(double))
-#define doublestore(T,V) memcpy((T), (void *) &V, sizeof(double))
-#define longlongget(V,M) memcpy(&V, (M), sizeof(unsigned long long))
-#define longlongstore(T,V) memcpy((T), &V, sizeof(unsigned long long))
-
-#else
-
-#define ushortget(V,M)	do { V = uint2korr(M); } while(0)
-#define shortget(V,M)	do { V = sint2korr(M); } while(0)
-#define longget(V,M)	do { V = sint4korr(M); } while(0)
-#define ulongget(V,M)   do { V = uint4korr(M); } while(0)
-#define shortstore(T,V) int2store(T,V)
-#define longstore(T,V)	int4store(T,V)
-#ifndef floatstore
-#define floatstore(T,V)  memcpy((T), (void *) (&V), sizeof(float))
-#define floatget(V,M)    memcpy(&V, (M), sizeof(float))
-#endif
-#ifndef doubleget
-#define doubleget(V,M)	 memcpy(&V, (M), sizeof(double))
-#define doublestore(T,V) memcpy((T), (void *) &V, sizeof(double))
-#endif /* doubleget */
-#define longlongget(V,M) memcpy(&V, (M), sizeof(unsigned long long))
-#define longlongstore(T,V) memcpy((T), &V, sizeof(unsigned long long))
-
-#endif /* WORDS_BIGENDIAN */
-
-
-#endif /* __i386__ OR _WIN32 */
-
-/* Due to callback functions we cannot use PY_BEGIN/END_ALLOW_THREADS */
-
-#define MARIADB_BEGIN_ALLOW_THREADS(obj)\
-{\
-  (obj)->thread_state= PyEval_SaveThread();\
-}
-
-#define MARIADB_END_ALLOW_THREADS(obj)\
-if ((obj)->thread_state)\
-{\
-    PyEval_RestoreThread((obj)->thread_state);\
-    (obj)->thread_state= NULL;\
-}
-
-#define MARIADB_UNBLOCK_THREADS(obj)\
-{\
-    if ((obj)->thread_state)\
-    {\
-        _save= (obj)->thread_state;\
-        PyEval_RestoreThread(_save);\
-        (obj)->thread_state= NULL;\
-    }\
-}
-
-#define MARIADB_BLOCK_THREADS(obj)\
-    if (_save)\
-    {\
-        (obj)->thread_state= PyEval_SaveThread();\
-        _save= NULL;\
-    }
+/******************************************************************************
+    Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
+
+   This library is free software; you can redistribute it and/or
+   modify it under the terms of the GNU Library General Public
+   License as published by the Free Software Foundation; either
+   version 2 of the License, or (at your option) any later version.
+
+   This library is distributed in the hope that it will be useful,
+   but WITHOUT ANY WARRANTY; without even the implied warranty of
+   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+   Library General Public License for more details.
+
+   You should have received a copy of the GNU Library General Public
+   License along with this library; if not see <http://www.gnu.org/licenses>
+   or write to the Free Software Foundation, Inc.,
+   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+******************************************************************************/
+#define PY_SSIZE_T_CLEAN
+
+#include "Python.h"
+#include "bytesobject.h"
+#include "structmember.h"
+#include "structseq.h"
+#include <stdarg.h>
+#include <stdint.h>
+#include <mysql.h>
+#include <errmsg.h>
+#include <mysqld_error.h>
+#include <time.h>
+#include <docs/common.h>
+#include <limits.h>
+
+#define CHECK_TYPE(obj, type) \
+(Py_TYPE((obj)) == type || PyType_IsSubtype(Py_TYPE((obj)), type))
+
+#if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_TYPE)
+static inline void _Py_SET_TYPE(PyObject *ob, PyTypeObject *type)
+{ ob->ob_type = type; }
+#define Py_SET_TYPE(ob, type) _Py_SET_TYPE((PyObject*)(ob), type)
+#endif
+
+#if defined(_WIN32)
+#include <config_win.h>
+#include <windows.h>
+#ifdef _MSC_VER
+typedef SSIZE_T ssize_t;
+#endif
+typedef CRITICAL_SECTION pthread_mutex_t;
+#define pthread_mutex_init(A,B)  InitializeCriticalSection(A)
+#define pthread_mutex_lock(A)	 (EnterCriticalSection(A),0)
+#define pthread_mutex_unlock(A)  LeaveCriticalSection(A)
+#define pthread_mutex_destroy(A) DeleteCriticalSection(A)
+#define pthread_self() GetCurrentThreadId()
+#include <malloc.h>
+#else
+#include <pthread.h>
+#include <limits.h>
+#endif /* defined(_WIN32) */
+
+
+#ifndef MIN
+#define MIN(a,b) (a) < (b) ? (a) : (b)
+#endif
+
+#ifndef MAX
+#define MAX(a,b) (a) > (b) ? (a) : (b)
+#endif
+
+#if !defined(__GNUC__) && !defined(__clang__)
+#define __attribute__(A)
+#endif
+
+#ifdef _WIN32
+int clock_gettime(int dummy, struct timespec *ct);
+#define CLOCK_MONOTONIC_RAW 1
+#endif
+
+#define REQUIRED_CC_VERSION 30103
+
+#if MARIADB_PACKAGE_VERSION_ID < REQUIRED_CC_VERSION
+#error Minimum required version of MariaDB Connector/C is 3.1.3
+#endif
+
+#if defined(_WIN32) && defined(_MSVC)
+#ifndef L64
+#define L64(x) x##i64
+#endif
+#else
+#ifndef L64
+#define L64(x) x##LL
+#endif /* L64 */
+#endif /* _WIN32 */
+
+#define STRINGIFY(n) #n
+#define TOSTRING(n) STRINGIFY(n)
+
+#define PY_MARIADB_VERSION TOSTRING(PY_MARIADB_MAJOR_VERSION) "." \
+        TOSTRING(PY_MARIADB_MINOR_VERSION) "." TOSTRING(PY_MARIADB_PATCH_VERSION)
+
+#define MAX_TPC_XID_SIZE 64
+#define POOL_DEFAULT_SIZE 5
+
+/* Placeholder for missing documentation */
+#define MISSING_DOC NULL
+
+/* Magic constant for checking dynamic columns */
+#define PYTHON_DYNCOL_VALUE 0xA378BD8E
+
+typedef struct st_lex_str {
+    char *str;
+    size_t length;
+} MrdbString;
+
+enum enum_binary_command {
+    SQL_NONE= 0,
+    SQL_INSERT,
+    SQL_UPDATE,
+    SQL_REPLACE,
+    SQL_DELETE,
+    SQL_CALL,
+    SQL_DO,
+    SQL_SELECT,
+    SQL_OTHER=255
+};
+
+enum enum_extended_field_type
+{
+  EXT_TYPE_NONE=0,
+  EXT_TYPE_JSON=1
+};
+
+enum enum_result_format
+{
+    RESULT_TUPLE= 0,
+    RESULT_NAMED_TUPLE,
+    RESULT_DICTIONARY
+};
+
+enum enum_dyncol_type
+{
+    DYNCOL_LIST= 1,
+    DYNCOL_TUPLE,
+    DYNCOL_SET,
+    DYNCOL_DICT,
+    DYNCOL_ODICT,
+    DYNCOL_LAST
+};
+
+enum enum_tpc_state
+{
+    TPC_STATE_NONE= 0,
+    TPC_STATE_XID,
+    TPC_STATE_PREPARE
+};
+
+enum enum_paramstyle
+{
+    NONE= 0,
+    QMARK= 1,
+    FORMAT= 2,
+    PYFORMAT= 3
+};
+
+typedef struct st_parser {
+    MrdbString statement;
+    MrdbString *keys;
+    uint8_t in_literal[3];
+    uint8_t in_comment;
+    uint8_t in_values;
+    uint8_t is_insert;
+    uint8_t comment_eol;
+    uint32_t param_count;
+    uint32_t key_count;
+    char* value_ofs;
+    PyObject *param_list;
+    enum enum_paramstyle paramstyle;
+    enum enum_binary_command command;
+    MYSQL *mysql;
+} MrdbParser;
+
+/* PEP-249: Connection object */
+typedef struct {
+    PyObject_HEAD
+    PyThreadState *thread_state;
+    MYSQL *mysql;
+    int open;
+    uint8_t is_buffered;
+    uint8_t is_closed;
+    enum enum_tpc_state tpc_state;
+    char xid[150]; /* large enough, to hold 2 * MAX_TPC_XID size + integer value */
+    PyObject *dsn; /* always null */
+    const char *host;
+/*    const char *tls_cipher;
+    const char *tls_version;
+    const char *unix_socket;
+    int port;
+    const char *charset;
+    const char *collation; */
+    uint8_t inuse;
+    uint8_t status;
+    uint8_t asynchronous;
+    struct timespec last_used;
+    unsigned long thread_id;
+    char *server_info;
+    uint8_t closed;
+#if MARIADB_PACKAGE_VERSION_ID > 30301
+    PyObject *status_callback;
+#endif
+    PyObject *last_executed_stmt;
+    PyObject *converter;
+} MrdbConnection;
+
+typedef struct {
+    enum enum_field_types type;
+    PyObject *Value;
+    uint8_t indicator;
+} Mariadb_Value;
+
+/* Parameter info for cursor.executemany()
+   operations */
+typedef struct {
+    enum enum_field_types type;
+    size_t bits; /* for PyLong Object */
+    PyTypeObject *ob_type;
+    uint8_t has_indicator;
+} MrdbParamInfo;
+
+typedef struct {
+    PyObject *value;
+    char indicator;
+    enum enum_field_types type;
+    size_t length;
+    uint8_t free_me;
+    void *buffer;
+    unsigned char num[8];
+    MYSQL_TIME tm;
+} MrdbParamValue;
+
+typedef struct {
+    char *statement;
+    Py_ssize_t statement_len;
+    enum enum_paramstyle paramstyle;
+    enum enum_binary_command command;
+    uint32_t paramcount;
+    uint8_t is_text;
+    PyObject *paramlist;
+    PyObject *keys;
+} MrdbParseInfo;
+
+/* PEP-249: Cursor object */
+typedef struct {
+    PyObject_HEAD
+    MrdbConnection *connection;
+    MYSQL_STMT *stmt;
+    MYSQL_RES *result;
+    PyObject *data;
+    uint32_t array_size;
+    uint32_t row_array_size; /* for fetch many */
+    MrdbParamInfo *paraminfo;
+    MrdbParamValue *value;
+    MYSQL_BIND *params;
+    MYSQL_BIND *bind;
+    MYSQL_FIELD *fields;
+    char *statement;
+    size_t statement_len;
+    PyObject **values;
+    PyStructSequence_Field *sequence_fields;
+    PyTypeObject *sequence_type;
+    MrdbParseInfo parseinfo;
+    unsigned long prefetch_rows;
+    unsigned long cursor_type;
+    int64_t affected_rows;
+    uint32_t field_count;
+    int64_t row_count;
+    uint64_t lastrow_id;
+    unsigned long row_number;
+    enum enum_result_format result_format;
+    uint8_t is_prepared;
+    char is_buffered;
+    uint8_t fetched;
+    uint8_t closed;
+    uint8_t reprepare;
+    enum enum_paramstyle paramstyle;
+} MrdbCursor;
+
+typedef struct
+{
+    PyObject_HEAD
+} Mariadb_Fieldinfo;
+
+typedef struct {
+    ps_field_fetch_func func;
+    int pack_len;
+    unsigned long max_len;
+} Mariadb_Conversion;
+
+extern char *dsn_keys[];
+
+/* Exceptions */
+extern PyObject *Mariadb_InterfaceError;
+extern PyObject *Mariadb_Error;
+extern PyObject *Mariadb_DatabaseError;
+extern PyObject *Mariadb_DataError;
+extern PyObject *Mariadb_PoolError;
+extern PyObject *Mariadb_OperationalError;
+extern PyObject *Mariadb_IntegrityError;
+extern PyObject *Mariadb_InternalError;
+extern PyObject *Mariadb_ProgrammingError;
+extern PyObject *Mariadb_NotSupportedError;
+extern PyObject *Mariadb_Warning;
+
+extern PyObject *decimal_module,
+                *decimal_type;
+
+/* Object types */
+extern PyTypeObject MrdbPool_Type;
+extern PyTypeObject Mariadb_Fieldinfo_Type;
+extern PyTypeObject MrdbConnection_Type;
+extern PyTypeObject MrdbCursor_Type;
+
+PyObject *ListOrTuple_GetItem(PyObject *obj, Py_ssize_t index);
+int Mariadb_traverse(PyObject *self,
+    visitproc visit,
+    void *arg);
+
+/* Function prototypes */
+void
+mariadb_throw_exception(void *handle,
+    PyObject *execption_type,
+    int8_t is_statement,
+    const char *message,
+    ...);
+
+enum enum_extended_field_type mariadb_extended_field_type(const MYSQL_FIELD *field);
+
+PyObject *
+MrdbConnection_ping(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_kill(MrdbConnection *self, PyObject *args);
+
+PyObject *
+MrdbConnection_reconnect(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_reset(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_autocommit(MrdbConnection *self, PyObject *args);
+
+PyObject *
+MrdbConnection_change_user(MrdbConnection *self, PyObject *args);
+
+PyObject
+*MrdbConnection_rollback(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_commit(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_close(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_connect( PyObject *self,PyObject *args,	PyObject *kwargs);
+
+void
+MrdbConnection_SetAttributes(MrdbConnection *self);
+
+/* TPC methods */
+PyObject *
+MrdbConnection_xid(MrdbConnection *self, PyObject *args);
+
+PyObject *
+MrdbConnection_tpc_begin(MrdbConnection *self, PyObject *args);
+
+PyObject *
+MrdbConnection_tpc_commit(MrdbConnection *self, PyObject *args);
+
+PyObject *
+MrdbConnection_tpc_rollback(MrdbConnection *self, PyObject *args);
+
+PyObject *
+MrdbConnection_tpc_prepare(MrdbConnection *self);
+
+PyObject *
+MrdbConnection_tpc_recover(MrdbConnection *self);
+
+/* codecs prototypes  */
+uint8_t
+mariadb_check_bulk_parameters(MrdbCursor *self, PyObject *data);
+
+uint8_t
+mariadb_check_execute_parameters(MrdbCursor *self, PyObject *data);
+
+uint8_t
+mariadb_param_update(void *data, MYSQL_BIND *bind, uint32_t row_nr);
+
+/* parser prototypes */
+MrdbParser *
+MrdbParser_init(MYSQL *mysql, const char *statement, size_t length);
+
+void
+MrdbParser_end(MrdbParser *p);
+
+uint8_t
+MrdbParser_parse(MrdbParser *p, uint8_t is_batch, char *errmsg, size_t errmsg_len);
+
+/* Global defines */
+
+
+#define MARIADB_PY_APILEVEL "2.0"
+#define MARIADB_PY_PARAMSTYLE "qmark"
+#define MARIADB_PY_THREADSAFETY 1
+
+#define MAX_POOL_SIZE 64
+
+#define TIMEDIFF(a,b)\
+  ((a).tv_sec * (uint64_t)1E09 + (a).tv_nsec) -\
+  ((b).tv_sec * (uint64_t)1E09 + (b).tv_nsec)
+
+/* Helper macros */
+
+#define MrdbIndicator_Check(a)\
+      (PyObject_HasAttrString(a, "indicator"))
+
+#define MARIADB_CHECK_CONNECTION(connection, ret)\
+    if (!(connection) || !(connection)->mysql)\
+    {\
+        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0, \
+           "Invalid connection or not connected");\
+        return (ret);\
+    }
+
+#define MARIADB_CHECK_TPC(connection)\
+  if (connection->tpc_state == TPC_STATE_NONE)\
+  {\
+      mariadb_throw_exception(connection->mysql, Mariadb_ProgrammingError, 0,\
+          "Transaction not started");\
+      return NULL;\
+  }
+
+#define MARIADB_FREE_MEM(a)\
+    if (a)\
+    {\
+        PyMem_RawFree((a));\
+        (a)= NULL;\
+    }
+
+#define MARIADB_CHECK_STMT(cursor)\
+    if (!cursor->connection->mysql || cursor->closed)\
+    {\
+       (cursor)->closed= 1;\
+        mariadb_throw_exception(cursor->stmt, Mariadb_ProgrammingError, 1,\
+      "Invalid cursor or not connected");\
+    }
+
+
+
+// #define pooling_keywords "pool_name", "pool_size", "reset_session", "idle_timeout", "acquire_timeout"
+#define connection_keywords "dsn", "host", "user", "password", "database", "port", "socket",\
+  "connect_timeout", "read_timeout", "write_timeout",\
+"local_infile", "compress", "init_command",\
+"default_file", "default_group",\
+"ssl_key", "ssl_ca", "ssl_cert", "ssl_crl",\
+"ssl_cipher", "ssl_capath", "ssl_crlpath",\
+"ssl_verify_cert", "ssl",\
+"client_flags", "charset"
+
+/* MariaDB protocol macros */
+#define int1store(T,A) *((int8_t*) (T)) = (A)
+#define uint1korr(A)   (*(((uint8_t*)(A))))
+#if defined(__i386__) || defined(_WIN32)
+#define sint2korr(A)	(*((int16_t *) (A)))
+#define sint3korr(A)	((int32_t) ((((unsigned char) (A)[2]) & 128) ? \
+      (((uint32_t) 255L << 24) | \
+       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
+       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
+       ((uint32_t) (unsigned char) (A)[0])) : \
+       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
+       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
+       ((uint32_t) (unsigned char) (A)[0])))
+#define sint4korr(A)	(*((long *) (A)))
+#define uint2korr(A)	(*((uint16_t *) (A)))
+#if defined(HAVE_purify) && !defined(_WIN32)
+#define uint3korr(A)	(uint32_t) (((uint32_t) ((unsigned char) (A)[0])) +\
+    (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
+    (((uint32_t) ((unsigned char) (A)[2])) << 16))
+#else
+          /*
+             ATTENTION !
+
+             Please, note, uint3korr reads 4 bytes (not 3) !
+             It means, that you have to provide enough allocated space !
+           */
+#define uint3korr(A)	(long) (*((unsigned int *) (A)) & 0xFFFFFF)
+#endif /* HAVE_purify && !_WIN32 */
+#define uint4korr(A)	(*((uint32_t *) (A)))
+#define uint5korr(A)	((unsigned long long)(((uint32_t) ((unsigned char) (A)[0])) +\
+      (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
+      (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
+      (((uint32_t) ((unsigned char) (A)[3])) << 24)) +\
+      (((unsigned long long) ((unsigned char) (A)[4])) << 32))
+#define uint6korr(A)	((unsigned long long)(((uint32_t)    ((unsigned char) (A)[0]))          + \
+      (((uint32_t)    ((unsigned char) (A)[1])) << 8)   + \
+      (((uint32_t)    ((unsigned char) (A)[2])) << 16)  + \
+      (((uint32_t)    ((unsigned char) (A)[3])) << 24)) + \
+      (((unsigned long long) ((unsigned char) (A)[4])) << 32) +       \
+      (((unsigned long long) ((unsigned char) (A)[5])) << 40))
+#define uint8_tkorr(A)	(*((unsigned long long *) (A)))
+#define sint8korr(A)	(*((long long *) (A)))
+#define int2store(T,A)	*((uint16_t*) (T))= (uint16_t) (A)
+#define int3store(T,A)  do { *(T)=  (unsigned char) ((A));\
+  *(T+1)=(unsigned char) (((uint) (A) >> 8));\
+  *(T+2)=(unsigned char) (((A) >> 16)); } while (0)
+#define int4store(T,A)	*((long *) (T))= (long) (A)
+#define int5store(T,A)  do { *(T)= (unsigned char)((A));\
+  *((T)+1)=(unsigned char) (((A) >> 8));\
+  *((T)+2)=(unsigned char) (((A) >> 16));\
+  *((T)+3)=(unsigned char) (((A) >> 24)); \
+  *((T)+4)=(unsigned char) (((A) >> 32)); } while(0)
+#define int6store(T,A)  do { *(T)=    (unsigned char)((A));          \
+  *((T)+1)=(unsigned char) (((A) >> 8));  \
+  *((T)+2)=(unsigned char) (((A) >> 16)); \
+  *((T)+3)=(unsigned char) (((A) >> 24)); \
+  *((T)+4)=(unsigned char) (((A) >> 32)); \
+  *((T)+5)=(unsigned char) (((A) >> 40)); } while(0)
+#define int8store(T,A)	*((unsigned long long *) (T))= (unsigned long long) (A)
+
+          typedef union {
+            double v;
+            long m[2];
+          } doubleget_union;
+#define doubleget(V,M)	\
+  do { doubleget_union _tmp; \
+    _tmp.m[0] = *((long*)(M)); \
+    _tmp.m[1] = *(((long*) (M))+1); \
+    (V) = _tmp.v; } while(0)
+#define doublestore(T,V) do { *((long *) T) = ((doubleget_union *)&V)->m[0]; \
+  *(((long *) T)+1) = ((doubleget_union *)&V)->m[1]; \
+} while (0)
+#define float4get(V,M)   do { *((float *) &(V)) = *((float*) (M)); } while(0)
+#define float8get(V,M)   doubleget((V),(M))
+#define float4store(V,M) memcpy((unsigned char*) V,(unsigned char*) (&M),sizeof(float))
+#define floatstore(T,V)  memcpy((unsigned char*)(T), (unsigned char*)(&V),sizeof(float))
+#define floatget(V,M)    memcpy((unsigned char*) &V,(unsigned char*) (M),sizeof(float))
+#define float8store(V,M) doublestore((V),(M))
+#else
+
+/*
+   We're here if it's not a IA-32 architecture (Win32 and UNIX IA-32 defines
+   were done before)
+ */
+#define sint2korr(A)	(int16_t) (((int16_t) ((unsigned char) (A)[0])) +\
+    ((int16_t) ((int16_t) (A)[1]) << 8))
+#define sint3korr(A)	((int32_t) ((((unsigned char) (A)[2]) & 128) ? \
+      (((uint32_t) 255L << 24) | \
+       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
+       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
+       ((uint32_t) (unsigned char) (A)[0])) : \
+       (((uint32_t) (unsigned char) (A)[2]) << 16) |\
+       (((uint32_t) (unsigned char) (A)[1]) << 8) | \
+       ((uint32_t) (unsigned char) (A)[0])))
+#define sint4korr(A)	(int32_t) (((int32_t) ((unsigned char) (A)[0])) +\
+    (((int32_t) ((unsigned char) (A)[1]) << 8)) +\
+    (((int32_t) ((unsigned char) (A)[2]) << 16)) +\
+    (((int32_t) ((int16_t) (A)[3]) << 24)))
+#define sint8korr(A)	(long long) uint8korr(A)
+#define uint2korr(A)	(uint16_t) (((uint16_t) ((unsigned char) (A)[0])) +\
+    ((uint16_t) ((unsigned char) (A)[1]) << 8))
+#define uint3korr(A)	(uint32_t) (((uint32_t) ((unsigned char) (A)[0])) +\
+    (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
+    (((uint32_t) ((unsigned char) (A)[2])) << 16))
+#define uint4korr(A)	(uint32_t) (((uint32_t) ((unsigned char) (A)[0])) +\
+    (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
+    (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
+    (((uint32_t) ((unsigned char) (A)[3])) << 24))
+#define uint5korr(A)	((unsigned long long)(((uint32_t) ((unsigned char) (A)[0])) +\
+      (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
+      (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
+      (((uint32_t) ((unsigned char) (A)[3])) << 24)) +\
+      (((unsigned long long) ((unsigned char) (A)[4])) << 32))
+#define uint6korr(A)	((unsigned long long)(((uint32_t)    ((unsigned char) (A)[0]))          + \
+      (((uint32_t)    ((unsigned char) (A)[1])) << 8)   + \
+      (((uint32_t)    ((unsigned char) (A)[2])) << 16)  + \
+      (((uint32_t)    ((unsigned char) (A)[3])) << 24)) + \
+      (((unsigned long long) ((unsigned char) (A)[4])) << 32) +       \
+      (((unsigned long long) ((unsigned char) (A)[5])) << 40))
+#define uint8korr(A)	((unsigned long long)(((uint32_t) ((unsigned char) (A)[0])) +\
+      (((uint32_t) ((unsigned char) (A)[1])) << 8) +\
+      (((uint32_t) ((unsigned char) (A)[2])) << 16) +\
+      (((uint32_t) ((unsigned char) (A)[3])) << 24)) +\
+      (((unsigned long long) (((uint32_t) ((unsigned char) (A)[4])) +\
+                              (((uint32_t) ((unsigned char) (A)[5])) << 8) +\
+                              (((uint32_t) ((unsigned char) (A)[6])) << 16) +\
+                              (((uint32_t) ((unsigned char) (A)[7])) << 24))) <<\
+                              32))
+#define int2store(T,A)       do { uint def_temp= (uint) (A) ;\
+  *((unsigned char*) (T))=  (unsigned char)(def_temp); \
+  *((unsigned char*) (T)+1)=(unsigned char)((def_temp >> 8)); \
+} while(0)
+#define int3store(T,A)       do { /*lint -save -e734 */\
+  *((unsigned char*)(T))=(unsigned char) ((A));\
+  *((unsigned char*) (T)+1)=(unsigned char) (((A) >> 8));\
+  *((unsigned char*)(T)+2)=(unsigned char) (((A) >> 16)); \
+  /*lint -restore */} while(0)
+#define int4store(T,A)       do { *((char *)(T))=(char) ((A));\
+  *(((char *)(T))+1)=(char) (((A) >> 8));\
+  *(((char *)(T))+2)=(char) (((A) >> 16));\
+  *(((char *)(T))+3)=(char) (((A) >> 24)); } while(0)
+#define int5store(T,A)       do { *((char *)(T))=     (char)((A));  \
+  *(((char *)(T))+1)= (char)(((A) >> 8)); \
+  *(((char *)(T))+2)= (char)(((A) >> 16)); \
+  *(((char *)(T))+3)= (char)(((A) >> 24)); \
+  *(((char *)(T))+4)= (char)(((A) >> 32)); \
+} while(0)
+#define int6store(T,A)       do { *((char *)(T))=     (char)((A)); \
+  *(((char *)(T))+1)= (char)(((A) >> 8)); \
+  *(((char *)(T))+2)= (char)(((A) >> 16)); \
+  *(((char *)(T))+3)= (char)(((A) >> 24)); \
+  *(((char *)(T))+4)= (char)(((A) >> 32)); \
+  *(((char *)(T))+5)= (char)(((A) >> 40)); \
+} while(0)
+#define int8store(T,A)       do { uint def_temp= (uint) (A), def_temp2= (uint) ((A) >> 32); \
+  int4store((T),def_temp); \
+  int4store((T+4),def_temp2); } while(0)
+#ifdef WORDS_BIGENDIAN
+#define float4store(T,A) do { *(T)= ((unsigned char *) &A)[3];\
+  *((T)+1)=(char) ((unsigned char *) &A)[2];\
+  *((T)+2)=(char) ((unsigned char *) &A)[1];\
+  *((T)+3)=(char) ((unsigned char *) &A)[0]; } while(0)
+
+#define float4get(V,M)   do { float def_temp;\
+  ((unsigned char*) &def_temp)[0]=(M)[3];\
+  ((unsigned char*) &def_temp)[1]=(M)[2];\
+  ((unsigned char*) &def_temp)[2]=(M)[1];\
+  ((unsigned char*) &def_temp)[3]=(M)[0];\
+  (V)=def_temp; } while(0)
+#define float8store(T,V) do { *(T)= ((unsigned char *) &V)[7];\
+  *((T)+1)=(char) ((unsigned char *) &V)[6];\
+  *((T)+2)=(char) ((unsigned char *) &V)[5];\
+  *((T)+3)=(char) ((unsigned char *) &V)[4];\
+  *((T)+4)=(char) ((unsigned char *) &V)[3];\
+  *((T)+5)=(char) ((unsigned char *) &V)[2];\
+  *((T)+6)=(char) ((unsigned char *) &V)[1];\
+  *((T)+7)=(char) ((unsigned char *) &V)[0]; } while(0)
+
+#define float8get(V,M)   do { double def_temp;\
+  ((unsigned char*) &def_temp)[0]=(M)[7];\
+  ((unsigned char*) &def_temp)[1]=(M)[6];\
+  ((unsigned char*) &def_temp)[2]=(M)[5];\
+  ((unsigned char*) &def_temp)[3]=(M)[4];\
+  ((unsigned char*) &def_temp)[4]=(M)[3];\
+  ((unsigned char*) &def_temp)[5]=(M)[2];\
+  ((unsigned char*) &def_temp)[6]=(M)[1];\
+  ((unsigned char*) &def_temp)[7]=(M)[0];\
+  (V) = def_temp; } while(0)
+#else
+#define float4get(V,M)   memcpy(&V, (M), sizeof(float))
+#define float4store(V,M) memcpy(V, (&M), sizeof(float))
+
+#if defined(__FLOAT_WORD_ORDER) && (__FLOAT_WORD_ORDER == __BIG_ENDIAN)
+#define doublestore(T,V) do { *(((char*)T)+0)=(char) ((unsigned char *) &V)[4];\
+  *(((char*)T)+1)=(char) ((unsigned char *) &V)[5];\
+  *(((char*)T)+2)=(char) ((unsigned char *) &V)[6];\
+  *(((char*)T)+3)=(char) ((unsigned char *) &V)[7];\
+  *(((char*)T)+4)=(char) ((unsigned char *) &V)[0];\
+  *(((char*)T)+5)=(char) ((unsigned char *) &V)[1];\
+  *(((char*)T)+6)=(char) ((unsigned char *) &V)[2];\
+  *(((char*)T)+7)=(char) ((unsigned char *) &V)[3]; }\
+          while(0)
+#define doubleget(V,M)   do { double def_temp;\
+  ((unsigned char*) &def_temp)[0]=(M)[4];\
+  ((unsigned char*) &def_temp)[1]=(M)[5];\
+  ((unsigned char*) &def_temp)[2]=(M)[6];\
+  ((unsigned char*) &def_temp)[3]=(M)[7];\
+  ((unsigned char*) &def_temp)[4]=(M)[0];\
+  ((unsigned char*) &def_temp)[5]=(M)[1];\
+  ((unsigned char*) &def_temp)[6]=(M)[2];\
+  ((unsigned char*) &def_temp)[7]=(M)[3];\
+  (V) = def_temp; } while(0)
+#endif /* __FLOAT_WORD_ORDER */
+
+#define float8get(V,M)   doubleget((V),(M))
+#define float8store(V,M) doublestore((V),(M))
+#endif /* WORDS_BIGENDIAN */
+
+#ifdef HAVE_BIGENDIAN
+
+#define ushortget(V,M)  do { V = (uint16_t) (((uint16_t) ((unsigned char) (M)[1]))+\
+    ((uint16_t) ((uint16_t) (M)[0]) << 8)); } while(0)
+#define shortget(V,M)   do { V = (short) (((short) ((unsigned char) (M)[1]))+\
+    ((short) ((short) (M)[0]) << 8)); } while(0)
+#define longget(V,M)    do { int32 def_temp;\
+  ((unsigned char*) &def_temp)[0]=(M)[0];\
+  ((unsigned char*) &def_temp)[1]=(M)[1];\
+  ((unsigned char*) &def_temp)[2]=(M)[2];\
+  ((unsigned char*) &def_temp)[3]=(M)[3];\
+  (V)=def_temp; } while(0)
+#define ulongget(V,M)   do { uint32 def_temp;\
+  ((unsigned char*) &def_temp)[0]=(M)[0];\
+  ((unsigned char*) &def_temp)[1]=(M)[1];\
+  ((unsigned char*) &def_temp)[2]=(M)[2];\
+  ((unsigned char*) &def_temp)[3]=(M)[3];\
+  (V)=def_temp; } while(0)
+#define shortstore(T,A) do { uint def_temp=(uint) (A) ;\
+  *(((char*)T)+1)=(char)(def_temp); \
+  *(((char*)T)+0)=(char)(def_temp >> 8); } while(0)
+#define longstore(T,A)  do { *(((char*)T)+3)=((A));\
+  *(((char*)T)+2)=(((A) >> 8));\
+  *(((char*)T)+1)=(((A) >> 16));\
+  *(((char*)T)+0)=(((A) >> 24)); } while(0)
+
+#define floatget(V,M)    memcpy(&V, (M), sizeof(float))
+#define floatstore(T,V)  memcpy((T), (void*) (&V), sizeof(float))
+#define doubleget(V,M)	 memcpy(&V, (M), sizeof(double))
+#define doublestore(T,V) memcpy((T), (void *) &V, sizeof(double))
+#define longlongget(V,M) memcpy(&V, (M), sizeof(unsigned long long))
+#define longlongstore(T,V) memcpy((T), &V, sizeof(unsigned long long))
+
+#else
+
+#define ushortget(V,M)	do { V = uint2korr(M); } while(0)
+#define shortget(V,M)	do { V = sint2korr(M); } while(0)
+#define longget(V,M)	do { V = sint4korr(M); } while(0)
+#define ulongget(V,M)   do { V = uint4korr(M); } while(0)
+#define shortstore(T,V) int2store(T,V)
+#define longstore(T,V)	int4store(T,V)
+#ifndef floatstore
+#define floatstore(T,V)  memcpy((T), (void *) (&V), sizeof(float))
+#define floatget(V,M)    memcpy(&V, (M), sizeof(float))
+#endif
+#ifndef doubleget
+#define doubleget(V,M)	 memcpy(&V, (M), sizeof(double))
+#define doublestore(T,V) memcpy((T), (void *) &V, sizeof(double))
+#endif /* doubleget */
+#define longlongget(V,M) memcpy(&V, (M), sizeof(unsigned long long))
+#define longlongstore(T,V) memcpy((T), &V, sizeof(unsigned long long))
+
+#endif /* WORDS_BIGENDIAN */
+
+
+#endif /* __i386__ OR _WIN32 */
+
+/* Due to callback functions we cannot use PY_BEGIN/END_ALLOW_THREADS */
+
+#define MARIADB_BEGIN_ALLOW_THREADS(obj)\
+{\
+  (obj)->thread_state= PyEval_SaveThread();\
+}
+
+#define MARIADB_END_ALLOW_THREADS(obj)\
+if ((obj)->thread_state)\
+{\
+    PyEval_RestoreThread((obj)->thread_state);\
+    (obj)->thread_state= NULL;\
+}
+
+#define MARIADB_UNBLOCK_THREADS(obj)\
+{\
+    if ((obj)->thread_state)\
+    {\
+        _save= (obj)->thread_state;\
+        PyEval_RestoreThread(_save);\
+        (obj)->thread_state= NULL;\
+    }\
+}
+
+#define MARIADB_BLOCK_THREADS(obj)\
+    if (_save)\
+    {\
+        (obj)->thread_state= PyEval_SaveThread();\
+        _save= NULL;\
+    }
```

### Comparing `mariadb-1.1.6/mariadb/connectionpool.py` & `mariadb-1.1.7/mariadb/connectionpool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,307 +1,308 @@
-#
-# Copyright (C) 2020-2021 Georg Richter and MariaDB Corporation AB
-
-# This library is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Library General Public
-# License as published by the Free Software Foundation; either
-# version 2 of the License, or (at your option) any later version.
-
-# This library is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# Library General Public License for more details.
-
-# You should have received a copy of the GNU Library General Public
-# License along with this library; if not see <http://www.gnu.org/licenses>
-# or write to the Free Software Foundation, Inc.,
-# 51 Franklin St., Fifth Floor, Boston, MA 02110, USA
-#
-
-import mariadb
-import _thread
-import time
-
-from mariadb.constants import STATUS
-
-MAX_POOL_SIZE = 64
-
-
-class ConnectionPool(object):
-    """
-    Class defining a pool of database connections
-
-    MariaDB Connector/Python supports simple connection pooling.
-    A connection pool holds a number of open connections and handles
-    thread safety when providing connections to threads.
-
-    The size of a connection pool is configurable at creation time,
-    but cannot be changed afterwards. The maximum size of a connection
-    pool is limited to 64 connections.
-
-    Keyword Arguments:
-
-        * pool_name (str) -- Name of connection pool
-
-        * pool_size (int)=5 -- Size of pool. If not specified default value
-          of 5 will be used. Maximum allowed number is 64.
-
-        * pool_reset_connection (bool)=True -- Will reset the connection before
-          returning it to the pool.  Default value is True.
-
-        * pool_validation_interval (int)=500 -- Specifies the validation
-          interval in milliseconds after which the status of a connection
-          requested from the pool is checked.
-          The default values is 500 milliseconds, a value of 0 means that
-          the status will always be checked.
-          (Added in version 1.1.6)
-    """
-
-    def __init__(self, *args, **kwargs):
-        """
-        Creates a connection pool class
-
-        :param str pool_name:
-            Name of connection pool
-
-        :param int pool_size:
-            Size of pool. If not specified default value of 5 will be used.
-            Maximum allowed number is 64.
-
-        :param bool pool_reset_connection:
-            Will reset the connection before returning it to the pool.
-            Default value is True.
-        """
-        self._connections_free = []
-        self._connections_used = []
-        self._pool_args = {}
-        self._conn_args = {}
-        self._lock_pool = _thread.RLock()
-        self.__closed = 0
-
-        key_words = ["pool_name", "pool_size", "pool_reset_connection",
-                     "pool_validation_interval"]
-
-        # check if pool_name was provided
-        if kwargs and "pool_name" in kwargs:
-
-            # check if pool_name already exists
-            if kwargs["pool_name"] in mariadb._CONNECTION_POOLS:
-                raise mariadb.ProgrammingError("Pool '%s' already exists"
-                                               % kwargs["pool_name"])
-        else:
-            raise mariadb.ProgrammingError("No pool name specified")
-
-        # save pool keyword arguments
-        self._pool_args["name"] = kwargs.get("pool_name")
-        self._pool_args["size"] = int(kwargs.get("pool_size", 5))
-        self._pool_args["reset_connection"] = \
-            bool(kwargs.get("pool_reset_connection", True))
-        self._pool_args["validation_interval"] = \
-            int(kwargs.get("pool_validation_interval", 500))
-
-        # validate pool size (must be in range between 1 and MAX_POOL_SIZE)
-        if not (0 < self._pool_args["size"] <= MAX_POOL_SIZE):
-            raise mariadb.ProgrammingError("Pool size must be in range of "
-                                           "1 and %s" % MAX_POOL_SIZE)
-
-        # store pool and connection arguments
-        self._conn_args = kwargs.copy()
-        for key in key_words:
-            if key in self._conn_args:
-                del self._conn_args[key]
-
-        if len(self._conn_args) > 0:
-            with self._lock_pool:
-                # fill connection pool
-                for i in range(0, self._pool_args["size"]):
-                    try:
-                        connection = mariadb.Connection(**self._conn_args)
-                    except mariadb.Error:
-                        # if an error occurred, close all connections
-                        # and raise exception
-                        for j in range(0, len(self._connections_free)):
-                            try:
-                                self._connections_free[j].close()
-                            except mariadb.Error:
-                                # connect failed, so we are not
-                                # interested in errors
-                                # from close() method
-                                pass
-                            del self._connections_free[j]
-                        raise
-                    self.add_connection(connection)
-
-        # store connection pool in _CONNECTION_POOLS
-        mariadb._CONNECTION_POOLS[self._pool_args["name"]] = self
-
-    def _replace_connection(self, connection):
-        """
-        Removes the given connection and adds a new connection.
-        """
-
-        if connection:
-            if connection in self._connections_free:
-                x = self._connections_free.index(connection)
-                del self._connections_free[x]
-            elif connection in self._connections_used:
-                x = self._connections_used.index(connection)
-                del self._connections_used[x]
-
-            connection._Connection__pool = None
-            connection.close()
-        return self.add_connection()
-
-    def __repr__(self):
-        if (self.__closed):
-            return "<mariadb.connectionPool.ConnectionPool object (closed) "\
-                   "at %s>" % (hex(id(self)),)
-        else:
-            return "<mariadb.connectionPool.ConnectionPool object (name=%s) "\
-                   "at %s>" % (self.pool_name, hex(id(self)))
-
-    def add_connection(self, connection=None):
-        """
-        Adds a connection object to the connection pool.
-
-        In case that the pool doesn’t have a free slot or is not configured
-        a PoolError exception will be raised.
-        """
-
-        if not self._conn_args:
-            raise mariadb.PoolError("Couldn't get configuration for pool %s" %
-                                    self._pool_args["name"])
-
-        if (connection is not None and
-                not isinstance(connection, mariadb.connections.Connection)):
-            raise mariadb.ProgrammingError("Passed parameter is not a "
-                                           "connection object")
-
-        if connection is None and len(self._conn_args) == 0:
-            raise mariadb.PoolError("Can't get configuration for pool %s" %
-                                    self._pool_args["name"])
-
-        total = len(self._connections_free + self._connections_used)
-        if total >= self._pool_args["size"]:
-            raise mariadb.PoolError("Can't add connection to pool %s: "
-                                    "No free slot available (%s)." %
-                                    (self._pool_args["name"],
-                                     total))
-
-        with self._lock_pool:
-            if connection is None:
-                connection = mariadb.Connection(**self._conn_args)
-
-            connection._Connection__pool = self
-            connection.__last_used = time.perf_counter_ns()
-            self._connections_free.append(connection)
-            return connection
-
-    def get_connection(self):
-        """
-        Returns a connection from the connection pool or raises a PoolError
-        exception if a connection is not available.
-        """
-
-        conn = None
-
-        with self._lock_pool:
-            for i in range(0, len(self._connections_free)):
-                conn = self._connections_free[i]
-                dt = (time.perf_counter_ns() - conn.__last_used) / 1000000
-                if dt > self._pool_args["validation_interval"]:
-                    try:
-                        conn.ping()
-                    except mariadb.Error:
-                        conn = self._replace_connection(conn)
-                        if not conn:
-                            continue
-
-                conn._used += 1
-                self._connections_used.append(conn)
-                del self._connections_free[i]
-                return conn
-
-        return None
-
-    def _close_connection(self, connection):
-        """
-        Returns connection to the pool. Internally used
-        by connection object.
-        """
-        with self._lock_pool:
-
-            try:
-                if self._pool_args["reset_connection"]:
-                    connection.reset()
-                elif connection.server_status & STATUS.IN_TRANS:
-                    connection.rollback()
-            except mariadb.Error:
-                self._replace_connection(connection)
-
-            if connection:
-                if connection in self._connections_used:
-                    x = self._connections_used.index(connection)
-                    del self._connections_used[x]
-                    connection.__last_used = time.perf_counter_ns()
-                    self._connections_free.append(connection)
-
-    def set_config(self, **kwargs):
-        """
-        Sets the connection configuration for the connection pool.
-        For valid connection arguments check the mariadb.connect() method.
-
-        Note: This method doesn't create connections in the pool.
-        To fill the pool one has to use add_connection() ḿethod.
-        """
-
-        self._conn_args = kwargs
-
-    def close(self):
-        """Closes connection pool and all connections."""
-        try:
-            for c in (self._connections_free + self._connections_used):
-                c._Connection__pool = None
-                c.close()
-        finally:
-            self._connections_free = None
-            self._connections_used = None
-            del mariadb._CONNECTION_POOLS[self._pool_args["name"]]
-
-    @property
-    def pool_name(self):
-        """Returns the name of the connection pool."""
-
-        return self._pool_args["name"]
-
-    @property
-    def pool_size(self):
-        """Returns the size of the connection pool."""
-
-        return self._pool_args["size"]
-
-    @property
-    def max_size(self):
-        "Returns the maximum size for connection pools."""
-
-        return MAX_POOL_SIZE
-
-    @property
-    def connection_count(self):
-        "Returns the number of connections in connection pool."""
-
-        try:
-            return len(self._connections_free + self._connections_used)
-        except Exception:
-            return 0
-
-    @property
-    def pool_reset_connection(self):
-        """
-        If set to true, the connection will be reset on both client and server
-        side after .close() method was called
-        """
-        return self._pool_args["reset_connection"]
-
-    @pool_reset_connection.setter
-    def pool_reset_connection(self, reset):
-        self._pool_args["reset_connection"] = reset
+#
+# Copyright (C) 2020-2021 Georg Richter and MariaDB Corporation AB
+
+# This library is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Library General Public
+# License as published by the Free Software Foundation; either
+# version 2 of the License, or (at your option) any later version.
+
+# This library is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Library General Public License for more details.
+
+# You should have received a copy of the GNU Library General Public
+# License along with this library; if not see <http://www.gnu.org/licenses>
+# or write to the Free Software Foundation, Inc.,
+# 51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+#
+
+import mariadb
+import _thread
+import time
+
+from mariadb.constants import STATUS
+
+MAX_POOL_SIZE = 64
+
+
+class ConnectionPool(object):
+    """
+    Class defining a pool of database connections
+
+    MariaDB Connector/Python supports simple connection pooling.
+    A connection pool holds a number of open connections and handles
+    thread safety when providing connections to threads.
+
+    The size of a connection pool is configurable at creation time,
+    but cannot be changed afterwards. The maximum size of a connection
+    pool is limited to 64 connections.
+
+    Keyword Arguments:
+
+        * pool_name (str) -- Name of connection pool
+
+        * pool_size (int)=5 -- Size of pool. If not specified default value
+          of 5 will be used. Maximum allowed number is 64.
+
+        * pool_reset_connection (bool)=True -- Will reset the connection before
+          returning it to the pool.  Default value is True.
+
+        * pool_validation_interval (int)=500 -- Specifies the validation
+          interval in milliseconds after which the status of a connection
+          requested from the pool is checked.
+          The default values is 500 milliseconds, a value of 0 means that
+          the status will always be checked.
+          (Added in version 1.1.6)
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Creates a connection pool class
+
+        :param str pool_name:
+            Name of connection pool
+
+        :param int pool_size:
+            Size of pool. If not specified default value of 5 will be used.
+            Maximum allowed number is 64.
+
+        :param bool pool_reset_connection:
+            Will reset the connection before returning it to the pool.
+            Default value is True.
+        """
+        self._connections_free = []
+        self._connections_used = []
+        self._pool_args = {}
+        self._conn_args = {}
+        self._lock_pool = _thread.RLock()
+        self.__closed = 0
+
+        key_words = ["pool_name", "pool_size", "pool_reset_connection",
+                     "pool_validation_interval"]
+
+        # check if pool_name was provided
+        if kwargs and "pool_name" in kwargs:
+
+            # check if pool_name already exists
+            if kwargs["pool_name"] in mariadb._CONNECTION_POOLS:
+                raise mariadb.ProgrammingError("Pool '%s' already exists"
+                                               % kwargs["pool_name"])
+        else:
+            raise mariadb.ProgrammingError("No pool name specified")
+
+        # save pool keyword arguments
+        self._pool_args["name"] = kwargs.get("pool_name")
+        self._pool_args["size"] = int(kwargs.get("pool_size", 5))
+        self._pool_args["reset_connection"] = \
+            bool(kwargs.get("pool_reset_connection", True))
+        self._pool_args["validation_interval"] = \
+            int(kwargs.get("pool_validation_interval", 500))
+
+        # validate pool size (must be in range between 1 and MAX_POOL_SIZE)
+        if not (0 < self._pool_args["size"] <= MAX_POOL_SIZE):
+            raise mariadb.ProgrammingError("Pool size must be in range of "
+                                           "1 and %s" % MAX_POOL_SIZE)
+
+        # store pool and connection arguments
+        self._conn_args = kwargs.copy()
+        for key in key_words:
+            if key in self._conn_args:
+                del self._conn_args[key]
+
+        if len(self._conn_args) > 0:
+            with self._lock_pool:
+                # fill connection pool
+                for i in range(0, self._pool_args["size"]):
+                    try:
+                        connection = mariadb.Connection(**self._conn_args)
+                    except mariadb.Error:
+                        # if an error occurred, close all connections
+                        # and raise exception
+                        for j in range(0, len(self._connections_free)):
+                            try:
+                                self._connections_free[j].close()
+                            except mariadb.Error:
+                                # connect failed, so we are not
+                                # interested in errors
+                                # from close() method
+                                pass
+                            del self._connections_free[j]
+                        raise
+                    self.add_connection(connection)
+
+        # store connection pool in _CONNECTION_POOLS
+        mariadb._CONNECTION_POOLS[self._pool_args["name"]] = self
+
+    def _replace_connection(self, connection):
+        """
+        Removes the given connection and adds a new connection.
+        """
+
+        if connection:
+            if connection in self._connections_free:
+                x = self._connections_free.index(connection)
+                del self._connections_free[x]
+            elif connection in self._connections_used:
+                x = self._connections_used.index(connection)
+                del self._connections_used[x]
+
+            connection._Connection__pool = None
+            connection.close()
+        return self.add_connection()
+
+    def __repr__(self):
+        if (self.__closed):
+            return "<mariadb.connectionPool.ConnectionPool object (closed) "\
+                   "at %s>" % (hex(id(self)),)
+        else:
+            return "<mariadb.connectionPool.ConnectionPool object (name=%s) "\
+                   "at %s>" % (self.pool_name, hex(id(self)))
+
+    def add_connection(self, connection=None):
+        """
+        Adds a connection object to the connection pool.
+
+        In case that the pool doesn’t have a free slot or is not configured
+        a PoolError exception will be raised.
+        """
+
+        if not self._conn_args:
+            raise mariadb.PoolError("Couldn't get configuration for pool %s" %
+                                    self._pool_args["name"])
+
+        if (connection is not None and
+                not isinstance(connection, mariadb.connections.Connection)):
+            raise mariadb.ProgrammingError("Passed parameter is not a "
+                                           "connection object")
+
+        if connection is None and len(self._conn_args) == 0:
+            raise mariadb.PoolError("Can't get configuration for pool %s" %
+                                    self._pool_args["name"])
+
+        total = len(self._connections_free + self._connections_used)
+        if total >= self._pool_args["size"]:
+            raise mariadb.PoolError("Can't add connection to pool %s: "
+                                    "No free slot available (%s)." %
+                                    (self._pool_args["name"],
+                                     total))
+
+        with self._lock_pool:
+            if connection is None:
+                connection = mariadb.Connection(**self._conn_args)
+
+            connection._Connection__pool = self
+            connection.__last_used = time.perf_counter_ns()
+            self._connections_free.append(connection)
+            return connection
+
+    def get_connection(self):
+        """
+        Returns a connection from the connection pool or raises a PoolError
+        exception if a connection is not available.
+        """
+
+        conn = None
+
+        with self._lock_pool:
+            for i in range(0, len(self._connections_free)):
+                conn = self._connections_free[i]
+                dt = (time.perf_counter_ns() - conn.__last_used) / 1000000
+                if dt > self._pool_args["validation_interval"]:
+                    try:
+                        conn.ping()
+                    except mariadb.Error:
+                        conn = self._replace_connection(conn)
+                        if not conn:
+                            continue
+
+                conn._used += 1
+                self._connections_used.append(conn)
+                idx = self._connections_free.index(conn)
+                del self._connections_free[idx]
+                return conn
+
+        raise mariadb.PoolError("No connection available")
+
+    def _close_connection(self, connection):
+        """
+        Returns connection to the pool. Internally used
+        by connection object.
+        """
+        with self._lock_pool:
+
+            try:
+                if self._pool_args["reset_connection"]:
+                    connection.reset()
+                elif connection.server_status & STATUS.IN_TRANS:
+                    connection.rollback()
+            except mariadb.Error:
+                self._replace_connection(connection)
+
+            if connection:
+                if connection in self._connections_used:
+                    x = self._connections_used.index(connection)
+                    del self._connections_used[x]
+                    connection.__last_used = time.perf_counter_ns()
+                    self._connections_free.append(connection)
+
+    def set_config(self, **kwargs):
+        """
+        Sets the connection configuration for the connection pool.
+        For valid connection arguments check the mariadb.connect() method.
+
+        Note: This method doesn't create connections in the pool.
+        To fill the pool one has to use add_connection() ḿethod.
+        """
+
+        self._conn_args = kwargs
+
+    def close(self):
+        """Closes connection pool and all connections."""
+        try:
+            for c in (self._connections_free + self._connections_used):
+                c._Connection__pool = None
+                c.close()
+        finally:
+            self._connections_free = None
+            self._connections_used = None
+            del mariadb._CONNECTION_POOLS[self._pool_args["name"]]
+
+    @property
+    def pool_name(self):
+        """Returns the name of the connection pool."""
+
+        return self._pool_args["name"]
+
+    @property
+    def pool_size(self):
+        """Returns the size of the connection pool."""
+
+        return self._pool_args["size"]
+
+    @property
+    def max_size(self):
+        "Returns the maximum size for connection pools."""
+
+        return MAX_POOL_SIZE
+
+    @property
+    def connection_count(self):
+        "Returns the number of connections in connection pool."""
+
+        try:
+            return len(self._connections_free + self._connections_used)
+        except Exception:
+            return 0
+
+    @property
+    def pool_reset_connection(self):
+        """
+        If set to true, the connection will be reset on both client and server
+        side after .close() method was called
+        """
+        return self._pool_args["reset_connection"]
+
+    @pool_reset_connection.setter
+    def pool_reset_connection(self, reset):
+        self._pool_args["reset_connection"] = reset
```

### Comparing `mariadb-1.1.6/mariadb/connections.py` & `mariadb-1.1.7/mariadb/cursors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,689 +1,561 @@
-#
-# Copyright (C) 2020-2021 Georg Richter and MariaDB Corporation AB
-
-# This library is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Library General Public
-# License as published by the Free Software Foundation; either
-# version 2 of the License, or (at your option) any later version.
-
-# This library is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# Library General Public License for more details.
-
-# You should have received a copy of the GNU Library General Public
-# License along with this library; if not see <http://www.gnu.org/licenses>
-# or write to the Free Software Foundation, Inc.,
-# 51 Franklin St., Fifth Floor, Boston, MA 02110, USA
-#
-
-import mariadb
-import socket
-import mariadb.cursors
-
-from mariadb.constants import STATUS, TPC_STATE, INFO
-from packaging import version
-
-_DEFAULT_CHARSET = "utf8mb4"
-_DEFAULT_COLLATION = "utf8mb4_general_ci"
-_MAX_TPC_XID_SIZE = 64
-
-
-class Connection(mariadb._mariadb.connection):
-    """
-    MariaDB Connector/Python Connection Object
-
-    Handles the connection to a MariaDB or MySQL database server.
-    It encapsulates a database session.
-
-    Connections are created using the method mariadb.connect()
-    """
-
-    def _check_closed(self):
-        if self._closed:
-            raise mariadb.ProgrammingError("Invalid connection or "
-                                           "not connected")
-
-    def __init__(self, *args, **kwargs):
-        """
-        Establishes a connection to a database server and returns a connection
-        object.
-        """
-
-        self._socket = None
-        self._used = 0
-        self._last_executed_statement = None
-        self._socket = None
-        self.__pool = None
-        self.__last_used = 0
-        self.tpc_state = TPC_STATE.NONE
-        self._xid = None
-
-        autocommit = kwargs.pop("autocommit", False)
-        reconnect = kwargs.pop("reconnect", False)
-        self._converter = kwargs.pop("converter", None)
-
-        # if host contains a connection string or multiple hosts,
-        # we need to check if it's supported by Connector/C
-        if "host" in kwargs:
-            host = kwargs.get("host")
-            if version.Version(mariadb.mariadbapi_version) <\
-               version.Version('3.3.0') and ',' in host:
-                raise mariadb.ProgrammingError("Host failover list requires "
-                                               "MariaDB Connector/C 3.3.0 "
-                                               "or newer")
-
-        # compatibility feature: if SSL is provided as a dictionary,
-        # we will map it's content
-        if "ssl" in kwargs and not isinstance(kwargs["ssl"], bool):
-            ssl = kwargs.pop("ssl", None)
-            for key in ["ca", "cert", "capath", "key", "cipher"]:
-                if key in ssl:
-                    kwargs["ssl_%s" % key] = ssl[key]
-            kwargs["ssl"] = True
-
-        super().__init__(*args, **kwargs)
-        self.autocommit = autocommit
-        self.auto_reconnect = reconnect
-
-    def cursor(self, cursorclass=mariadb.cursors.Cursor, **kwargs):
-        """
-        Returns a new cursor object for the current connection.
-
-        If no cursorclass was specified, a cursor with default mariadb.Cursor
-        class will be created.
-
-        Optional keyword parameters:
-
-        - buffered = True
-          If set to False the result will be unbuffered, which means before
-          executing another statement with the same connection the entire
-          result set must be fetched.
-          Please note that the default was False for MariaDB Connector/Python
-          versions < 1.1.0.
-
-        - dictionary = False
-          Return fetch values as dictionary.
-
-        - named_tuple = False
-          Return fetch values as named tuple. This feature exists for
-          compatibility reasons and should be avoided due to possible
-          inconsistency.
-
-        - cursor_type = CURSOR_TYPE.NONE
-          If cursor_type is set to CURSOR_TYPE.READ_ONLY, a cursor is opened
-          for the statement invoked with cursors execute() method.
-
-        - prepared = False
-          When set to True cursor will remain in prepared state after the first
-          execute() method was called. Further calls to execute() method will
-          ignore the sql statement.
-
-        - binary = False
-          Always execute statement in MariaDB client/server binary protocol.
-
-        In versions prior to 1.1.0 results were unbuffered by default,
-        which means before executing another statement with the same
-        connection the entire result set must be fetched.
-
-        fetch* methods of the cursor class by default return result set values
-        as a tuple, unless named_tuple or dictionary was specified.
-        The latter one exists for compatibility reasons and should be avoided
-        due to possible inconsistency in case two or more fields in a result
-        set have the same name.
-
-        If cursor_type is set to CURSOR_TYPE.READ_ONLY, a cursor is opened for
-        the statement invoked with cursors execute() method.
-        """
-        self._check_closed()
-        cursor = cursorclass(self, **kwargs)
-        if not isinstance(cursor, mariadb._mariadb.cursor):
-            raise mariadb.ProgrammingError("%s is not an instance of "
-                                           "mariadb.cursor" % cursor)
-        return cursor
-
-    def close(self):
-        self._check_closed()
-        if self._Connection__pool:
-            self._Connection__pool._close_connection(self)
-        else:
-            super().close()
-
-    def __enter__(self):
-        self._check_closed()
-        "Returns a copy of the connection."
-
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self._check_closed()
-        "Closes connection."
-
-        self.close()
-
-    def commit(self):
-        """
-        Commit any pending transaction to the database.
-        """
-
-        self._check_closed()
-        if self.tpc_state > TPC_STATE.NONE:
-            raise mariadb.ProgrammingError("commit() is not allowed if "
-                                           "a TPC transaction is active")
-        self._execute_command("COMMIT")
-        self._read_response()
-
-    def rollback(self):
-        """
-        Causes the database to roll back to the start of any pending
-        transaction
-
-        Closing a connection without committing the changes first will
-        cause an implicit rollback to be performed.
-        Note that rollback() will not work as expected if autocommit mode
-        was set to True or the storage engine does not support transactions."
-        """
-
-        self._check_closed()
-        if self.tpc_state > TPC_STATE.NONE:
-            raise mariadb.ProgrammingError("rollback() is not allowed if a "
-                                           "TPC transaction is active")
-        self._execute_command("ROLLBACK")
-        self._read_response()
-
-    def kill(self, id: int):
-        """
-        This function is used to ask the server to kill a database connection
-        specified by the processid parameter.
-
-        The connection id can be be retrieved by SHOW PROCESSLIST sql command.
-        """
-
-        self._check_closed()
-        if not isinstance(id, int):
-            raise mariadb.ProgrammingError("id must be of type int.")
-        stmt = "KILL %s" % id
-        self._execute_command(stmt)
-        self._read_response()
-
-    def begin(self):
-        """
-        Start a new transaction which can be committed by .commit() method,
-        or cancelled by .rollback() method.
-        """
-        self._check_closed()
-        self._execute_command("BEGIN")
-        self._read_response()
-
-    def select_db(self, new_db: str):
-        """
-        Gets the default database for the current connection.
-
-        The default database can also be obtained or changed by database
-        attribute.
-        """
-
-        self._check_closed()
-        self.database = new_db
-
-    def get_server_version(self):
-        """
-        Returns a tuple representing the version of the connected server in
-        the following format: (MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
-        """
-
-        return self.server_version_info
-
-    def show_warnings(self):
-        """
-        Shows error, warning and note messages from last executed command.
-        """
-
-        self._check_closed()
-        if (not self.warnings):
-            return None
-
-        cursor = self.cursor()
-        cursor.execute("SHOW WARNINGS")
-        ret = cursor.fetchall()
-        del cursor
-        return ret
-
-    class xid(tuple):
-        """
-        xid(format_id: int, global_transaction_id: str, branch_qualifier: str)
-
-        Creates a transaction ID object suitable for passing to the .tpc_*()
-        methods of this connection.
-
-        Parameters:
-
-        - format_id: Format id. If not set default value `0` will be used.
-
-        - global_transaction_id: Global transaction qualifier, which must be
-          unique. The maximum length of the global transaction id is
-          limited to 64 characters.
-
-        - branch_qualifier: Branch qualifier which represents a local
-          transaction identifier. The maximum length of the branch qualifier
-          is limited to 64 characters.
-
-        """
-        def __new__(self, format_id, transaction_id, branch_qualifier):
-            if not isinstance(format_id, int):
-                raise mariadb.ProgrammingError("argument 1 must be int, "
-                                               "not %s",
-                                               type(format_id).__name__)
-            if not isinstance(transaction_id, str):
-                raise mariadb.ProgrammingError("argument 2 must be str, "
-                                               "not %s",
-                                               type(transaction_id).__mane__)
-            if not isinstance(branch_qualifier, str):
-                raise mariadb.ProgrammingError("argument 3 must be str, "
-                                               "not %s",
-                                               type(transaction_id).__name__)
-            if len(transaction_id) > _MAX_TPC_XID_SIZE:
-                raise mariadb.ProgrammingError("Maximum length of "
-                                               "transaction_id exceeded.")
-            if len(branch_qualifier) > _MAX_TPC_XID_SIZE:
-                raise mariadb.ProgrammingError("Maximum length of "
-                                               "branch_qualifier exceeded.")
-            if format_id == 0:
-                format_id = 1
-            return super().__new__(self, (format_id,
-                                          transaction_id,
-                                          branch_qualifier))
-
-    def tpc_begin(self, xid):
-        """
-        Parameter:
-          xid: xid object which was created by .xid() method of connection
-               class
-
-        Begins a TPC transaction with the given transaction ID xid.
-
-        This method should be called outside of a transaction
-        (i.e. nothing may have executed since the last .commit()
-        or .rollback()).
-        Furthermore, it is an error to call .commit() or .rollback() within
-        the TPC transaction. A ProgrammingError is raised, if the application
-        calls .commit() or .rollback() during an active TPC transaction.
-        """
-
-        self._check_closed()
-        if type(xid).__name__ != "xid":
-            raise mariadb.ProgrammingError("argument 1 must be xid "
-                                           "not %s", type(xid).__name__)
-        stmt = "XA BEGIN '%s','%s',%s" % (xid[1], xid[2], xid[0])
-        try:
-            self._execute_command(stmt)
-            self._read_response()
-        except mariadb.Error:
-            raise
-        self.tpc_state = TPC_STATE.XID
-        self._xid = xid
-
-    def tpc_commit(self, xid=None):
-        """
-        Optional parameter:"
-        xid: xid object which was created by .xid() method of connection class.
-
-        When called with no arguments, .tpc_commit() commits a TPC transaction
-        previously prepared with .tpc_prepare().
-
-        If .tpc_commit() is called prior to .tpc_prepare(), a single phase
-        commit is performed. A transaction manager may choose to do this if
-        only a single resource is participating in the global transaction.
-        When called with a transaction ID xid, the database commits the given
-        transaction. If an invalid transaction ID is provided,
-        a ProgrammingError will be raised.
-        This form should be called outside of a transaction, and
-        is intended for use in recovery."
-        """
-
-        self._check_closed()
-        if not xid:
-            xid = self._xid
-
-        if self.tpc_state == TPC_STATE.NONE:
-            raise mariadb.ProgrammingError("Transaction not started.")
-        if xid is None and self.tpc_state != TPC_STATE.PREPARE:
-            raise mariadb.ProgrammingError("Transaction is not prepared.")
-        if xid and type(xid).__name__ != "xid":
-            raise mariadb.ProgrammingError("argument 1 must be xid "
-                                           "not %s" % type(xid).__name__)
-
-        if self.tpc_state < TPC_STATE.PREPARE:
-            stmt = "XA END '%s','%s',%s" % (xid[1], xid[2], xid[0])
-            self._execute_command(stmt)
-            try:
-                self._read_response()
-            except mariadb.Error:
-                self._xid = None
-                self.tpc_state = TPC_STATE.NONE
-                raise
-
-        stmt = "XA COMMIT '%s','%s',%s" % (xid[1], xid[2], xid[0])
-        if self.tpc_state < TPC_STATE.PREPARE:
-            stmt = stmt + " ONE PHASE"
-        try:
-            self._execute_command(stmt)
-            self._read_response()
-        except mariadb.Error:
-            self._xid = None
-            self.tpc_state = TPC_STATE.NONE
-            raise
-
-        # cleanup
-        self._xid = None
-        self.tpc_state = TPC_STATE.NONE
-
-    def tpc_prepare(self):
-        """
-        Performs the first phase of a transaction started with .tpc_begin().
-        A ProgrammingError will be raised if this method was called outside of
-        a TPC transaction.
-
-        After calling .tpc_prepare(), no statements can be executed until
-        .tpc_commit() or .tpc_rollback() have been called.
-        """
-
-        self._check_closed()
-        if self.tpc_state == TPC_STATE.NONE:
-            raise mariadb.ProgrammingError("Transaction not started.")
-        if self.tpc_state == TPC_STATE.PREPARE:
-            raise mariadb.ProgrammingError("Transaction is already in "
-                                           "prepared state.")
-
-        xid = self._xid
-        stmt = "XA END '%s','%s',%s" % (xid[1], xid[2], xid[0])
-        try:
-            self._execute_command(stmt)
-            self._read_response()
-        except mariadb.Error:
-            self._xid = None
-            self.tpc_state = TPC_STATE.NONE
-            raise
-
-        stmt = "XA PREPARE '%s','%s',%s" % (xid[1], xid[2], xid[0])
-        try:
-            self._execute_command(stmt)
-            self._read_response()
-        except mariadb.Error:
-            self._xid = None
-            self.tpc_state = TPC_STATE.NONE
-            raise
-
-        self.tpc_state = TPC_STATE.PREPARE
-
-    def tpc_rollback(self, xid=None):
-        """
-        Parameter:
-           xid: xid object which was created by .xid() method of connection
-                class
-
-        Performs the first phase of a transaction started with .tpc_begin().
-        A ProgrammingError will be raised if this method outside of a TPC
-        transaction.
-
-        After calling .tpc_prepare(), no statements can be executed until
-        .tpc_commit() or .tpc_rollback() have been called.
-        """
-
-        self._check_closed()
-        if self.tpc_state == TPC_STATE.NONE:
-            raise mariadb.ProgrammingError("Transaction not started.")
-        if xid and type(xid).__name__ != "xid":
-            raise mariadb.ProgrammingError("argument 1 must be xid "
-                                           "not %s" % type(xid).__name__)
-
-        if not xid:
-            xid = self._xid
-
-        if self.tpc_state < TPC_STATE.PREPARE:
-            stmt = "XA END '%s','%s',%s" % (xid[1], xid[2], xid[0])
-            self._execute_command(stmt)
-            try:
-                self._read_response()
-            except mariadb.Error:
-                self._xid = None
-                self.tpc_state = TPC_STATE.NONE
-                raise
-
-        stmt = "XA ROLLBACK '%s','%s',%s" % (xid[1], xid[2], xid[0])
-        try:
-            self._execute_command(stmt)
-            self._read_response()
-        except mariadb.Error:
-            self._xid = None
-            self.tpc_state = TPC_STATE.NONE
-            raise
-
-        self.tpc_state = TPC_STATE.PREPARE
-
-    def tpc_recover(self):
-        """
-        Returns a list of pending transaction IDs suitable for use with
-        tpc_commit(xid) or .tpc_rollback(xid).
-        """
-
-        self._check_closed()
-        cursor = self.cursor()
-        cursor.execute("XA RECOVER")
-        result = cursor.fetchall()
-        del cursor
-        return result
-
-    @property
-    def database(self):
-        """Get default database for connection."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.SCHEMA)
-
-    @database.setter
-    def database(self, schema):
-        """Set default database."""
-        self._check_closed()
-
-        try:
-            self._execute_command("USE %s" % str(schema))
-            self._read_response()
-        except mariadb.Error:
-            raise
-
-    @property
-    def user(self):
-        """
-        Returns the user name for the current connection or empty
-        string if it can't be determined, e.g. when using socket
-        authentication.
-        """
-        self._check_closed()
-
-        return self._mariadb_get_info(INFO.USER)
-
-    @property
-    def character_set(self):
-        """
-        Client character set.
-
-        For MariaDB Connector/Python it is always utf8mb4.
-        """
-
-        return _DEFAULT_CHARSET
-
-    @property
-    def client_capabilities(self):
-        """Client capability flags."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.CLIENT_CAPABILITIES)
-
-    @property
-    def server_capabilities(self):
-        """Server capability flags."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.SERVER_CAPABILITIES)
-
-    @property
-    def extended_server_capabilities(self):
-        """
-        Extended server capability flags (only for MariaDB
-        database servers).
-        """
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.EXTENDED_SERVER_CAPABILITIES)
-
-    @property
-    def server_port(self):
-        """
-        Database server TCP/IP port. This value will be 0 in case of a unix
-        socket connection.
-        """
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.PORT)
-
-    @property
-    def unix_socket(self):
-        """Unix socket name."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.UNIX_SOCKET)
-
-    @property
-    def server_name(self):
-        """Name or IP address of database server."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.HOST)
-
-    @property
-    def collation(self):
-        """Client character set collation"""
-
-        return _DEFAULT_COLLATION
-
-    @property
-    def server_info(self):
-        """Server version in alphanumerical format (str)"""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.SERVER_VERSION)
-
-    @property
-    def tls_cipher(self):
-        """TLS cipher suite if a secure connection is used."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.SSL_CIPHER)
-
-    @property
-    def tls_version(self):
-        """TLS protocol version if a secure connection is used."""
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.TLS_VERSION)
-
-    @property
-    def server_status(self):
-        """
-        Return server status flags
-        """
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.SERVER_STATUS)
-
-    @property
-    def server_version(self):
-        """
-        Server version in numerical format.
-
-        The form of the version number is
-        VERSION_MAJOR * 10000 + VERSION_MINOR * 100 + VERSION_PATCH
-        """
-
-        self._check_closed()
-        return self._mariadb_get_info(INFO.SERVER_VERSION_ID)
-
-    @property
-    def server_version_info(self):
-        """
-        Returns numeric version of connected database server in tuple format.
-        """
-
-        self._check_closed()
-        version = self.server_version
-        return (int(version / 10000),
-                int((version % 10000) / 100),
-                version % 100)
-
-    @property
-    def autocommit(self):
-        """
-        Toggles autocommit mode on or off for the current database connection.
-
-        Autocommit mode only affects operations on transactional table types.
-        Be aware that rollback() will not work, if autocommit mode was switched
-        on.
-
-        By default autocommit mode is set to False."
-        """
-
-        self._check_closed()
-        return bool(self.server_status & STATUS.AUTOCOMMIT)
-
-    @autocommit.setter
-    def autocommit(self, mode):
-        self._check_closed()
-        if bool(mode) == self.autocommit:
-            return
-        try:
-            self._execute_command("SET AUTOCOMMIT=%s" % int(mode))
-            self._read_response()
-        except mariadb.Error:
-            raise
-
-    @property
-    def socket(self):
-        """Returns the socket used for database connection"""
-
-        fno = self._get_socket()
-        if not self._socket:
-            self._socket = socket.socket(fileno=fno)
-        # in case of a possible reconnect, file descriptor has changed
-        elif fno != self._socket.fileno():
-            self._socket = socket.socket(fileno=fno)
-        return self._socket
-
-    @property
-    def open(self):
-        """
-        Returns true if the connection is alive.
-
-        A ping command will be send to the server for this purpose,
-        which means this function might fail if there are still
-        non processed pending result sets.
-        """
-
-        self._check_closed()
-        try:
-            self.ping()
-        except mariadb.Error:
-            return False
-        return True
-
-    # Aliases
-    character_set_name = character_set
-
-    @property
-    def thread_id(self):
-        """
-        Alias for connection_id
-        """
-
-        self._check_closed()
-        return self.connection_id
+#
+# Copyright (C) 2020-2021 Georg Richter and MariaDB Corporation AB
+
+# This library is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Library General Public
+# License as published by the Free Software Foundation; either
+# version 2 of the License, or (at your option) any later version.
+
+# This library is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Library General Public License for more details.
+
+# You should have received a copy of the GNU Library General Public
+# License along with this library; if not see <http://www.gnu.org/licenses>
+# or write to the Free Software Foundation, Inc.,
+# 51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+#
+
+import mariadb
+import datetime
+from numbers import Number
+from mariadb.constants import CURSOR, STATUS, CAPABILITY, INDICATOR
+from typing import Sequence
+
+PARAMSTYLE_QMARK = 1
+PARAMSTYLE_FORMAT = 2
+PARAMSTYLE_PYFORMAT = 3
+
+ROWS_ALL = -1
+
+RESULT_TUPLE = 0
+RESULT_NAMEDTUPLE = 1
+RESULT_DICTIONARY = 2
+
+# Command types
+SQL_NONE = 0,
+SQL_INSERT = 1
+SQL_UPDATE = 2
+SQL_REPLACE = 3
+SQL_DELETE = 4
+SQL_CALL = 5
+SQL_DO = 6
+SQL_SELECT = 7
+SQL_OTHER = 255
+
+ROWS_EOF = -1
+
+
+class Cursor(mariadb._mariadb.cursor):
+    """
+    MariaDB Connector/Python Cursor Object
+    """
+
+    def check_closed(self):
+        if self.closed:
+            self._connection._check_closed()
+            raise mariadb.ProgrammingError("Cursor is closed")
+
+    def __init__(self, connection, **kwargs):
+        """
+        initialization
+        """
+        self._bulk = False
+        self._dictionary = False
+        self._named_tuple = False
+        self._connection = connection
+        self._resulttype = RESULT_TUPLE
+        self._description = None
+        self._transformed_statement = None
+        self._prepared = False
+        self._prev_stmt = None
+        self._force_binary = None
+        self._rowcount = 0
+        self.buffered = True
+        self._parseinfo = None
+        self._data = None
+
+        if not connection:
+            raise mariadb.ProgrammingError("Invalid or no connection provided")
+
+        # parse keywords
+        if kwargs:
+            rtype = kwargs.pop("named_tuple", False)
+            if rtype:
+                self._resulttype = RESULT_NAMEDTUPLE
+            else:
+                rtype = kwargs.pop("dictionary", False)
+                if rtype:
+                    self._resulttype = RESULT_DICTIONARY
+            buffered = kwargs.pop("buffered", True)
+            self.buffered = buffered
+            self._prepared = kwargs.pop("prepared", False)
+            self._force_binary = kwargs.pop("binary", False)
+            self._cursor_type = kwargs.pop("cursor_type", 0)
+
+        # call initialization of main class
+        super().__init__(connection, **kwargs)
+
+    def _substitute_parameters(self):
+        """
+        Internal use only.
+
+        When running in text protocol, this method will replace placeholders
+        by supplied values.
+
+        For values which aren't numbers, strings or bytes string representation
+        will be used.
+        """
+
+        new_stmt = self.statement.encode("utf8")
+        replace_diff = 0
+        if self._paramlist:
+            for i in range(0, len(self._paramlist)):
+                extra_bytes = 0
+                if self._paramstyle == PARAMSTYLE_PYFORMAT:
+                    val = self._data[self._keys[i]]
+                else:
+                    val = self._data[i]
+                if val is None:
+                    replace = "NULL"
+                else:
+                    if isinstance(val, INDICATOR.MrdbIndicator):
+                        if val == INDICATOR.NULL:
+                            replace = "NULL"
+                        if val == INDICATOR.DEFAULT:
+                            replace = "DEFAULT"
+                    elif isinstance(val, Number):
+                        replace = val.__str__()
+                    else:
+                        if isinstance(val, (bytes, bytearray)):
+                            replace = "\"%s\"" % self.connection.escape_string(
+                                val.decode(encoding='latin1'))
+                        else:
+                            replace = "\"%s\"" % self.connection.escape_string(
+                                val.__str__())
+                            extra_bytes = len(replace.encode("utf-8")) -\
+                                len(replace)
+                ofs = self._paramlist[i] + replace_diff
+
+                new_stmt = new_stmt[:ofs] + replace.__str__().encode("utf8") +\
+                    new_stmt[ofs+1:]
+                replace_diff += len(replace) - 1 + extra_bytes
+        return new_stmt
+
+    def _check_execute_params(self):
+        # check data format
+        if self._paramstyle in (PARAMSTYLE_QMARK, PARAMSTYLE_FORMAT):
+            if not isinstance(self._data, (tuple, list)):
+                raise mariadb.ProgrammingError("Data argument must be "
+                                               "Tuple or List")
+
+        if self._paramstyle == PARAMSTYLE_PYFORMAT:
+            if not isinstance(self._data, dict):
+                raise mariadb.ProgrammingError("Data argument must be "
+                                               "Dictionary")
+            for i in range(0, len(self._keys)):
+                if self._keys[i] not in self._data:
+                    raise mariadb.ProgrammingError("Dictionary doesn't contain"
+                                                   " key '%s'" % self._keys[i])
+        else:
+            # check if number of place holders matches the number of
+            # supplied elements in data tuple
+            if self._paramlist and (
+               (not self._data and len(self._paramlist) > 0) or
+               (len(self._data) != len(self._paramlist))):
+                raise mariadb.ProgrammingError(
+                    "statement (%s) doesn't match the number of data elements"
+                    " (%s)." % (len(self._paramlist), len(self._data)))
+
+    def callproc(self, sp: str, data: Sequence = ()):
+        """
+        Executes a stored procedure sp. The data sequence must contain an
+        entry for each parameter the procedure expects.
+
+        Input/Output or Output parameters have to be retrieved by .fetch
+        methods, the .sp_outparams attribute indicates if the result set
+        contains output parameters.
+
+        Arguments:
+            - sp: Name of stored procedure.
+            - data: Optional sequence containing data for placeholder
+                    substitution.
+        """
+
+        self.check_closed()
+
+        # create statement
+        params = ""
+        if data and len(data):
+            params = ("?," * len(data))[:-1]
+        statement = "CALL %s(%s)" % (sp, params)
+        self._rowcount = 0
+        self.execute(statement, data)
+
+    def _parse_execute(self, statement: str, data=(), is_bulk=False):
+        """
+        For internal use
+
+        Parses SQL statement and checks parameters.
+        """
+
+        if not statement:
+            raise mariadb.ProgrammingError("empty statement")
+
+        # parse statement
+        if self.statement != statement or is_bulk and not self._bulk:
+            super()._parse(statement)
+            self._prev_stmt = statement
+            self._reprepare = True
+        else:
+            self._reprepare = False
+
+        self._transformed_statement = self.statement
+
+        if self._cursor_type == CURSOR.READ_ONLY:
+            self._text = False
+
+        self._data = data
+
+        self._check_execute_params()
+
+    def nextset(self):
+        """
+        Will make the cursor skip to the next available result set,
+        discarding any remaining rows from the current set.
+        """
+
+        self.check_closed()
+        return super()._nextset()
+
+    def execute(self, statement: str, data: Sequence = (), buffered=None):
+        """
+        Prepare and execute a SQL statement.
+
+        Parameters may be provided as sequence or mapping and will be bound
+        to variables in the operation. Variables are specified as question
+        marks (paramstyle ='qmark'), however for compatibility reasons MariaDB
+        Connector/Python also supports the 'format' and 'pyformat' paramstyles
+        with the restriction, that different paramstyles can't be mixed within
+        a statement.
+
+        A reference to the operation will be retained by the cursor.
+        If the cursor was created with attribute prepared =True the statement
+        string for following execute operations will be ignored.
+        This is most effective for algorithms where the same operation is used,
+        but different parameters are bound to it (many times).
+
+        By default execute() method generates an buffered result unless the
+        optional parameter buffered was set to False or the cursor was
+        generated as an unbuffered cursor.
+        """
+
+        self.check_closed()
+
+        self.connection._last_executed_statement = statement
+
+        # Parse statement
+        do_parse = True
+        self._rowcount = 0
+
+        if buffered is not None:
+            self.buffered = buffered
+
+        # clear pending result sets
+        if self.field_count:
+            self._clear_result()
+
+        # if we have a prepared cursor, we have to set statement
+        # to previous statement and don't need to parse
+        if self._prepared and self.statement:
+            statement = self.statement
+            do_parse = False
+
+        # parse statement and check param style
+        if do_parse:
+            self._parse_execute(statement, (data))
+
+        self._description = None
+
+        # CONPY-218: Allow None as replacement for empty tuple
+        data = data or ()
+
+        if len(data):
+            self._data = data
+        else:
+            self._data = None
+            # If statement doesn't contain parameters we force to run in text
+            # mode, unless a server side cursor or stored procedure will be
+            # executed.
+            if self._command != SQL_CALL and self._cursor_type == 0:
+                self._text = True
+
+        if self._force_binary:
+            self._text = False
+
+        # if one of the provided parameters has byte or datetime value,
+        # we don't use text protocol
+        if data and self._check_text_types() == True:
+            self._text = False
+
+        if self._text:
+            # in text mode we need to substitute parameters
+            # and store transformed statement
+            if (self.paramcount > 0):
+                self._transformed_statement = self._substitute_parameters()
+            else:
+                self._transformed_statement = self.statement
+
+            self._execute_text(self._transformed_statement)
+            self._readresponse()
+        else:
+            self._data = data
+            self._execute_binary()
+
+        self._initresult()
+        self._bulk = 0
+
+    def executemany(self, statement, parameters):
+        """
+        Prepare a database operation (INSERT,UPDATE,REPLACE or DELETE
+        statement) and execute it against all parameter found in sequence.
+
+        Exactly behaves like .execute() but accepts a list of tuples, where
+        each tuple represents data of a row within a table.
+        .executemany() only supports DML (insert, update, delete) statements.
+
+        If the SQL statement contains a RETURNING clause, executemany()
+        returns a result set containing the values for columns listed in the
+        RETURNING clause.
+        """
+        self.check_closed()
+
+        if not parameters or not len(parameters):
+            raise mariadb.ProgrammingError("No data provided")
+
+        self.connection._last_executed_statement = statement
+
+        # clear pending results
+        if self.field_count:
+            self._clear_result()
+
+        # If the server doesn't support bulk operations, we need to emulate
+        # by looping
+        # TODO: insert/replace statements are not optimized yet
+        #       rowcount updating
+        if not (self.connection.extended_server_capabilities &
+                (CAPABILITY.BULK_OPERATIONS >> 32)):
+            count = 0
+            for row in parameters:
+                self.execute(statement, row)
+                count += self.rowcount
+            self._rowcount = count
+        else:
+            # parse statement
+            self._parse_execute(statement, parameters[0], is_bulk=True)
+            self._data = parameters
+            self.is_text = False
+            self._rowcount = 0
+            self._execute_bulk()
+            self._bulk = 1
+
+    def _fetch_row(self):
+        """
+        Internal use only
+
+        fetches row and converts values, if connection has a converter.
+        """
+        self.check_closed()
+
+        # if there is no result set, PEP-249 requires to raise an
+        # exception
+        if not self.field_count:
+            raise mariadb.ProgrammingError("Cursor doesn't have a result set")
+        return super().fetchone()
+
+    def close(self):
+        """
+        Closes the cursor.
+
+        If the cursor has pending or unread results, .close() will cancel them
+        so that further operations using the same connection can be executed.
+
+        The cursor will be unusable from this point forward; an Error
+        (or subclass) exception will be raised if any operation is attempted
+        with the cursor."
+        """
+
+        # CONPY-231: fix memory leak
+        if self._data:
+            del self._data
+
+        if not self.connection._closed:
+            super().close()
+
+    def fetchone(self):
+        """
+        Fetch the next row of a query result set, returning a single sequence,
+        or None if no more data is available.
+
+        An exception will be raised if the previous call to execute() didn't
+        produce a result set or execute() wasn't called before.
+        """
+        self.check_closed()
+
+        row = self._fetch_row()
+        return row
+
+    def fetchmany(self, size: int = 0):
+        """
+        Fetch the next set of rows of a query result, returning a sequence
+        of sequences (e.g. a list of tuples). An empty sequence is returned
+        when no more rows are available.
+
+        The number of rows to fetch per call is specified by the parameter.
+        If it is not given, the cursor's arraysize determines the number
+        of rows to be fetched. The method should try to fetch as many rows
+        as indicated by the size parameter.
+        If this is not possible due to the specified number of rows not being
+        available, fewer rows may be returned.
+
+        An exception will be raised if the previous call to execute() didn't
+        produce a result set or execute() wasn't called before.
+        """
+        self.check_closed()
+
+        if size == 0:
+            size = self.arraysize
+
+        return super().fetchrows(size)
+
+    def fetchall(self):
+        """
+        Fetch all remaining rows of a query result, returning them as a
+        sequence of sequences (e.g. a list of tuples).
+
+        An exception will be raised if the previous call to execute() didn't
+        produce a result set or execute() wasn't called before.
+        """
+        self.check_closed()
+        return super().fetchrows(ROWS_EOF)
+
+    def __iter__(self):
+        return iter(self.fetchone, None)
+
+    def scroll(self, value: int, mode="relative"):
+        """
+        Scroll the cursor in the result set to a new position according to
+        mode.
+
+        If mode is "relative" (default), value is taken as offset to the
+        current position in the result set, if set to absolute, value states
+        an absolute target position.
+        """
+
+        if self.field_count == 0:
+            raise mariadb.ProgrammingError("Cursor doesn't have a result set")
+
+        if not self.buffered:
+            raise mariadb.ProgrammingError("This method is available only "
+                                           "for cursors with a buffered "
+                                           "result set.")
+
+        if mode != "absolute" and mode != "relative":
+            raise mariadb.ProgrammingError("Invalid or unknown scroll "
+                                           "mode specified.")
+
+        if value == 0 and mode != "absolute":
+            raise mariadb.ProgrammingError("Invalid position value 0.")
+
+        if mode == "relative":
+            if self.rownumber + value < 0 or \
+               self.rownumber + value > self.rowcount:
+                raise mariadb.ProgrammingError("Position value "
+                                               "is out of range.")
+            new_pos = self.rownumber + value
+        else:
+            if value < 0 or value >= self.rowcount:
+                raise mariadb.ProgrammingError("Position value "
+                                               "is out of range.")
+            new_pos = value
+
+        self._seek(new_pos)
+        self._rownumber = new_pos
+
+    def setinputsizes(self, size: int):
+        """
+        Required by PEP-249. Does nothing in MariaDB Connector/Python
+        """
+
+        return
+
+    def setoutputsize(self, size: int):
+        """
+        Required by PEP-249. Does nothing in MariaDB Connector/Python
+        """
+
+        return
+
+    def __enter__(self):
+        """Returns a copy of the cursor."""
+
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        """Closes cursor."""
+        self.close()
+
+    @property
+    def rowcount(self):
+        """
+        This read-only attribute specifies the number of rows that the last\
+        execute*() produced (for DQL statements like SELECT) or affected
+        (for DML statements like UPDATE or INSERT).
+        The return value is -1 in case no .execute*() has been performed
+        on the cursor or the rowcount of the last operation  cannot be
+        determined by the interface.
+        """
+        self.check_closed()
+        if self._rowcount > 0:
+            return self._rowcount
+        return super().rowcount
+
+    @property
+    def sp_outparams(self):
+        """
+        Indicates if the current result set contains in out or out parameter
+        from a previous executed stored procedure
+        """
+        self.check_closed()
+
+        return bool(self.connection.server_status & STATUS.PS_OUT_PARAMS)
+
+    @property
+    def lastrowid(self):
+        """
+        Returns the ID generated by a query on a table with a column having
+        the AUTO_INCREMENT attribute or the value for the last usage of
+        LAST_INSERT_ID().
+
+        If the last query wasn't an INSERT or UPDATE
+        statement or if the modified table does not have a column with the
+        AUTO_INCREMENT attribute and LAST_INSERT_ID was not used, the returned
+        value will be zero
+        """
+        self.check_closed()
+
+        id = self.insert_id
+        if id > 0:
+            return id
+        return None
+
+    @property
+    def connection(self):
+        """
+        Read-Only attribute which returns the reference to the connection
+        object on which the cursor was created.
+        """
+        self.check_closed()
+
+        return self._connection
```

### Comparing `mariadb-1.1.6/mariadb/constants/CAPABILITY.py` & `mariadb-1.1.7/mariadb/constants/CAPABILITY.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-'''
-MariaDB capability flags.
-
-These flags are used to check the capabilities both of a MariaDB server
-or the client applicaion.
-
-Capability flags are defined in module *mariadb.constants.CAPABILIY*
-
-'''
-
-MYSQL = 1          # MariaDB
-LONG_PASSWORD = 1  # MySQL
-FOUND_ROWS = 2
-LONG_FLAG = 4
-CONNECT_WITH_DB = 8
-NO_SCHEMA = 16
-COMPRESS = 32
-LOCAL_FILES = 128
-IGNORE_SPACE = 256
-INTERACTIVE = 1024
-SSL = 2048
-TRANSACTIONS = 8192
-SECURE_CONNECTION = 32768
-MULTI_STATEMENTS = 1 << 16
-MULTI_RESULTS = 1 << 17
-PS_MULTI_RESULTS = 1 << 18
-PLUGIN_AUTH = 1 << 19
-CONNECT_ATTRS = 1 << 20
-CAN_HANDLE_EXPIRED_PASSWORDS = 1 < 22
-SESSION_TRACKING = 1 << 23
-SSL_VERIFY_SERVER_CERT = 1 << 30
-REMEMBER_OPTIONS = 1 << 31
-
-# MariaDB specific capabilities
-PROGRESS = 1 << 32
-BULK_OPERATIONS = 1 << 34
-EXTENDED_METADATA = 1 << 35
-CACHE_METDATA = 1 << 36
+'''
+MariaDB capability flags.
+
+These flags are used to check the capabilities both of a MariaDB server
+or the client applicaion.
+
+Capability flags are defined in module *mariadb.constants.CAPABILIY*
+
+'''
+
+MYSQL = 1          # MariaDB
+LONG_PASSWORD = 1  # MySQL
+FOUND_ROWS = 2
+LONG_FLAG = 4
+CONNECT_WITH_DB = 8
+NO_SCHEMA = 16
+COMPRESS = 32
+LOCAL_FILES = 128
+IGNORE_SPACE = 256
+INTERACTIVE = 1024
+SSL = 2048
+TRANSACTIONS = 8192
+SECURE_CONNECTION = 32768
+MULTI_STATEMENTS = 1 << 16
+MULTI_RESULTS = 1 << 17
+PS_MULTI_RESULTS = 1 << 18
+PLUGIN_AUTH = 1 << 19
+CONNECT_ATTRS = 1 << 20
+CAN_HANDLE_EXPIRED_PASSWORDS = 1 < 22
+SESSION_TRACKING = 1 << 23
+SSL_VERIFY_SERVER_CERT = 1 << 30
+REMEMBER_OPTIONS = 1 << 31
+
+# MariaDB specific capabilities
+PROGRESS = 1 << 32
+BULK_OPERATIONS = 1 << 34
+EXTENDED_METADATA = 1 << 35
+CACHE_METDATA = 1 << 36
```

### Comparing `mariadb-1.1.6/mariadb/constants/CLIENT.py` & `mariadb-1.1.7/mariadb/constants/CLIENT.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-'''
-MariaDB capability flags.
-
-These flags are used to check the capabilities both of a MariaDB server
-or the client applicaion.
-
-Capability flags are defined in module *mariadb.constants.CLIENT*
-
-'''
-
-MYSQL = 1          # MariaDB
-LONG_PASSWORD = 1  # MySQL
-FOUND_ROWS = 2
-LONG_FLAG = 4
-CONNECT_WITH_DB = 8
-NO_SCHEMA = 16
-COMPRESS = 32
-LOCAL_FILES = 128
-IGNORE_SPACE = 256
-INTERACTIVE = 1024
-SSL = 2048
-TRANSACTIONS = 8192
-SECURE_CONNECTION = 32768
-MULTI_STATEMENTS = 1 << 16
-MULTI_RESULTS = 1 << 17
-PS_MULTI_RESULTS = 1 << 18
-PLUGIN_AUTH = 1 << 19
-CONNECT_ATTRS = 1 << 20
-CAN_HANDLE_EXPIRED_PASSWORDS = 1 < 22
-SESSION_TRACKING = 1 << 23
-SSL_VERIFY_SERVER_CERT = 1 << 30
-REMEMBER_OPTIONS = 1 << 31
-
-# MariaDB specific capabilities
-PROGRESS = 1 << 32
-BULK_OPERATIONS = 1 << 34
-EXTENDED_METADATA = 1 << 35
-CACHE_METDATA = 1 << 36
+'''
+MariaDB capability flags.
+
+These flags are used to check the capabilities both of a MariaDB server
+or the client applicaion.
+
+Capability flags are defined in module *mariadb.constants.CLIENT*
+
+'''
+
+MYSQL = 1          # MariaDB
+LONG_PASSWORD = 1  # MySQL
+FOUND_ROWS = 2
+LONG_FLAG = 4
+CONNECT_WITH_DB = 8
+NO_SCHEMA = 16
+COMPRESS = 32
+LOCAL_FILES = 128
+IGNORE_SPACE = 256
+INTERACTIVE = 1024
+SSL = 2048
+TRANSACTIONS = 8192
+SECURE_CONNECTION = 32768
+MULTI_STATEMENTS = 1 << 16
+MULTI_RESULTS = 1 << 17
+PS_MULTI_RESULTS = 1 << 18
+PLUGIN_AUTH = 1 << 19
+CONNECT_ATTRS = 1 << 20
+CAN_HANDLE_EXPIRED_PASSWORDS = 1 < 22
+SESSION_TRACKING = 1 << 23
+SSL_VERIFY_SERVER_CERT = 1 << 30
+REMEMBER_OPTIONS = 1 << 31
+
+# MariaDB specific capabilities
+PROGRESS = 1 << 32
+BULK_OPERATIONS = 1 << 34
+EXTENDED_METADATA = 1 << 35
+CACHE_METDATA = 1 << 36
```

### Comparing `mariadb-1.1.6/mariadb/constants/ERR.py` & `mariadb-1.1.7/mariadb/constants/ERR.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1254 +1,1254 @@
-# Autogenerated file. Please do not edit!
-
-
-ER_ERROR_FIRST = 1000
-ER_HASHCHK = 1000
-ER_NISAMCHK = 1001
-ER_NO = 1002
-ER_YES = 1003
-ER_CANT_CREATE_FILE = 1004
-ER_CANT_CREATE_TABLE = 1005
-ER_CANT_CREATE_DB = 1006
-ER_DB_CREATE_EXISTS = 1007
-ER_DB_DROP_EXISTS = 1008
-ER_DB_DROP_DELETE = 1009
-ER_DB_DROP_RMDIR = 1010
-ER_CANT_DELETE_FILE = 1011
-ER_CANT_FIND_SYSTEM_REC = 1012
-ER_CANT_GET_STAT = 1013
-ER_CANT_GET_WD = 1014
-ER_CANT_LOCK = 1015
-ER_CANT_OPEN_FILE = 1016
-ER_FILE_NOT_FOUND = 1017
-ER_CANT_READ_DIR = 1018
-ER_CANT_SET_WD = 1019
-ER_CHECKREAD = 1020
-ER_DISK_FULL = 1021
-ER_DUP_KEY = 1022
-ER_ERROR_ON_CLOSE = 1023
-ER_ERROR_ON_READ = 1024
-ER_ERROR_ON_RENAME = 1025
-ER_ERROR_ON_WRITE = 1026
-ER_FILE_USED = 1027
-ER_FILSORT_ABORT = 1028
-ER_FORM_NOT_FOUND = 1029
-ER_GET_ERRNO = 1030
-ER_ILLEGAL_HA = 1031
-ER_KEY_NOT_FOUND = 1032
-ER_NOT_FORM_FILE = 1033
-ER_NOT_KEYFILE = 1034
-ER_OLD_KEYFILE = 1035
-ER_OPEN_AS_READONLY = 1036
-ER_OUTOFMEMORY = 1037
-ER_OUT_OF_SORTMEMORY = 1038
-ER_UNEXPECTED_EOF = 1039
-ER_CON_COUNT_ERROR = 1040
-ER_OUT_OF_RESOURCES = 1041
-ER_BAD_HOST_ERROR = 1042
-ER_HANDSHAKE_ERROR = 1043
-ER_DBACCESS_DENIED_ERROR = 1044
-ER_ACCESS_DENIED_ERROR = 1045
-ER_NO_DB_ERROR = 1046
-ER_UNKNOWN_COM_ERROR = 1047
-ER_BAD_NULL_ERROR = 1048
-ER_BAD_DB_ERROR = 1049
-ER_TABLE_EXISTS_ERROR = 1050
-ER_BAD_TABLE_ERROR = 1051
-ER_NON_UNIQ_ERROR = 1052
-ER_SERVER_SHUTDOWN = 1053
-ER_BAD_FIELD_ERROR = 1054
-ER_WRONG_FIELD_WITH_GROUP = 1055
-ER_WRONG_GROUP_FIELD = 1056
-ER_WRONG_SUM_SELECT = 1057
-ER_WRONG_VALUE_COUNT = 1058
-ER_TOO_LONG_IDENT = 1059
-ER_DUP_FIELDNAME = 1060
-ER_DUP_KEYNAME = 1061
-ER_DUP_ENTRY = 1062
-ER_WRONG_FIELD_SPEC = 1063
-ER_PARSE_ERROR = 1064
-ER_EMPTY_QUERY = 1065
-ER_NONUNIQ_TABLE = 1066
-ER_INVALID_DEFAULT = 1067
-ER_MULTIPLE_PRI_KEY = 1068
-ER_TOO_MANY_KEYS = 1069
-ER_TOO_MANY_KEY_PARTS = 1070
-ER_TOO_LONG_KEY = 1071
-ER_KEY_COLUMN_DOES_NOT_EXIST = 1072
-ER_BLOB_USED_AS_KEY = 1073
-ER_TOO_BIG_FIELDLENGTH = 1074
-ER_WRONG_AUTO_KEY = 1075
-ER_BINLOG_CANT_DELETE_GTID_DOMAIN = 1076
-ER_NORMAL_SHUTDOWN = 1077
-ER_GOT_SIGNAL = 1078
-ER_SHUTDOWN_COMPLETE = 1079
-ER_FORCING_CLOSE = 1080
-ER_IPSOCK_ERROR = 1081
-ER_NO_SUCH_INDEX = 1082
-ER_WRONG_FIELD_TERMINATORS = 1083
-ER_BLOBS_AND_NO_TERMINATED = 1084
-ER_TEXTFILE_NOT_READABLE = 1085
-ER_FILE_EXISTS_ERROR = 1086
-ER_LOAD_INFO = 1087
-ER_ALTER_INFO = 1088
-ER_WRONG_SUB_KEY = 1089
-ER_CANT_REMOVE_ALL_FIELDS = 1090
-ER_CANT_DROP_FIELD_OR_KEY = 1091
-ER_INSERT_INFO = 1092
-ER_UPDATE_TABLE_USED = 1093
-ER_NO_SUCH_THREAD = 1094
-ER_KILL_DENIED_ERROR = 1095
-ER_NO_TABLES_USED = 1096
-ER_TOO_BIG_SET = 1097
-ER_NO_UNIQUE_LOGFILE = 1098
-ER_TABLE_NOT_LOCKED_FOR_WRITE = 1099
-ER_TABLE_NOT_LOCKED = 1100
-ER_WRONG_DB_NAME = 1102
-ER_WRONG_TABLE_NAME = 1103
-ER_TOO_BIG_SELECT = 1104
-ER_UNKNOWN_ERROR = 1105
-ER_UNKNOWN_PROCEDURE = 1106
-ER_WRONG_PARAMCOUNT_TO_PROCEDURE = 1107
-ER_WRONG_PARAMETERS_TO_PROCEDURE = 1108
-ER_UNKNOWN_TABLE = 1109
-ER_FIELD_SPECIFIED_TWICE = 1110
-ER_INVALID_GROUP_FUNC_USE = 1111
-ER_UNSUPPORTED_EXTENSION = 1112
-ER_TABLE_MUST_HAVE_COLUMNS = 1113
-ER_RECORD_FILE_FULL = 1114
-ER_UNKNOWN_CHARACTER_SET = 1115
-ER_TOO_MANY_TABLES = 1116
-ER_TOO_MANY_FIELDS = 1117
-ER_TOO_BIG_ROWSIZE = 1118
-ER_STACK_OVERRUN = 1119
-ER_WRONG_OUTER_JOIN = 1120
-ER_NULL_COLUMN_IN_INDEX = 1121
-ER_CANT_FIND_UDF = 1122
-ER_CANT_INITIALIZE_UDF = 1123
-ER_UDF_NO_PATHS = 1124
-ER_UDF_EXISTS = 1125
-ER_CANT_OPEN_LIBRARY = 1126
-ER_CANT_FIND_DL_ENTRY = 1127
-ER_FUNCTION_NOT_DEFINED = 1128
-ER_HOST_IS_BLOCKED = 1129
-ER_HOST_NOT_PRIVILEGED = 1130
-ER_PASSWORD_ANONYMOUS_USER = 1131
-ER_PASSWORD_NOT_ALLOWED = 1132
-ER_PASSWORD_NO_MATCH = 1133
-ER_UPDATE_INFO = 1134
-ER_CANT_CREATE_THREAD = 1135
-ER_WRONG_VALUE_COUNT_ON_ROW = 1136
-ER_CANT_REOPEN_TABLE = 1137
-ER_INVALID_USE_OF_NULL = 1138
-ER_REGEXP_ERROR = 1139
-ER_MIX_OF_GROUP_FUNC_AND_FIELDS = 1140
-ER_NONEXISTING_GRANT = 1141
-ER_TABLEACCESS_DENIED_ERROR = 1142
-ER_COLUMNACCESS_DENIED_ERROR = 1143
-ER_ILLEGAL_GRANT_FOR_TABLE = 1144
-ER_GRANT_WRONG_HOST_OR_USER = 1145
-ER_NO_SUCH_TABLE = 1146
-ER_NONEXISTING_TABLE_GRANT = 1147
-ER_NOT_ALLOWED_COMMAND = 1148
-ER_SYNTAX_ERROR = 1149
-ER_DELAYED_CANT_CHANGE_LOCK = 1150
-ER_TOO_MANY_DELAYED_THREADS = 1151
-ER_ABORTING_CONNECTION = 1152
-ER_NET_PACKET_TOO_LARGE = 1153
-ER_NET_READ_ERROR_FROM_PIPE = 1154
-ER_NET_FCNTL_ERROR = 1155
-ER_NET_PACKETS_OUT_OF_ORDER = 1156
-ER_NET_UNCOMPRESS_ERROR = 1157
-ER_NET_READ_ERROR = 1158
-ER_NET_READ_INTERRUPTED = 1159
-ER_NET_ERROR_ON_WRITE = 1160
-ER_NET_WRITE_INTERRUPTED = 1161
-ER_TOO_LONG_STRING = 1162
-ER_TABLE_CANT_HANDLE_BLOB = 1163
-ER_TABLE_CANT_HANDLE_AUTO_INCREMENT = 1164
-ER_DELAYED_INSERT_TABLE_LOCKED = 1165
-ER_WRONG_COLUMN_NAME = 1166
-ER_WRONG_KEY_COLUMN = 1167
-ER_WRONG_MRG_TABLE = 1168
-ER_DUP_UNIQUE = 1169
-ER_BLOB_KEY_WITHOUT_LENGTH = 1170
-ER_PRIMARY_CANT_HAVE_NULL = 1171
-ER_TOO_MANY_ROWS = 1172
-ER_REQUIRES_PRIMARY_KEY = 1173
-ER_NO_RAID_COMPILED = 1174
-ER_UPDATE_WITHOUT_KEY_IN_SAFE_MODE = 1175
-ER_KEY_DOES_NOT_EXISTS = 1176
-ER_CHECK_NO_SUCH_TABLE = 1177
-ER_CHECK_NOT_IMPLEMENTED = 1178
-ER_CANT_DO_THIS_DURING_AN_TRANSACTION = 1179
-ER_ERROR_DURING_COMMIT = 1180
-ER_ERROR_DURING_ROLLBACK = 1181
-ER_ERROR_DURING_FLUSH_LOGS = 1182
-ER_ERROR_DURING_CHECKPOINT = 1183
-ER_NEW_ABORTING_CONNECTION = 1184
-ER_FLUSH_MASTER_BINLOG_CLOSED = 1186
-ER_INDEX_REBUILD = 1187
-ER_MASTER = 1188
-ER_MASTER_NET_READ = 1189
-ER_MASTER_NET_WRITE = 1190
-ER_FT_MATCHING_KEY_NOT_FOUND = 1191
-ER_LOCK_OR_ACTIVE_TRANSACTION = 1192
-ER_UNKNOWN_SYSTEM_VARIABLE = 1193
-ER_CRASHED_ON_USAGE = 1194
-ER_CRASHED_ON_REPAIR = 1195
-ER_WARNING_NOT_COMPLETE_ROLLBACK = 1196
-ER_TRANS_CACHE_FULL = 1197
-ER_SLAVE_MUST_STOP = 1198
-ER_SLAVE_NOT_RUNNING = 1199
-ER_BAD_SLAVE = 1200
-ER_MASTER_INFO = 1201
-ER_SLAVE_THREAD = 1202
-ER_TOO_MANY_USER_CONNECTIONS = 1203
-ER_SET_CONSTANTS_ONLY = 1204
-ER_LOCK_WAIT_TIMEOUT = 1205
-ER_LOCK_TABLE_FULL = 1206
-ER_READ_ONLY_TRANSACTION = 1207
-ER_DROP_DB_WITH_READ_LOCK = 1208
-ER_CREATE_DB_WITH_READ_LOCK = 1209
-ER_WRONG_ARGUMENTS = 1210
-ER_NO_PERMISSION_TO_CREATE_USER = 1211
-ER_UNION_TABLES_IN_DIFFERENT_DIR = 1212
-ER_LOCK_DEADLOCK = 1213
-ER_TABLE_CANT_HANDLE_FT = 1214
-ER_CANNOT_ADD_FOREIGN = 1215
-ER_NO_REFERENCED_ROW = 1216
-ER_ROW_IS_REFERENCED = 1217
-ER_CONNECT_TO_MASTER = 1218
-ER_QUERY_ON_MASTER = 1219
-ER_ERROR_WHEN_EXECUTING_COMMAND = 1220
-ER_WRONG_USAGE = 1221
-ER_WRONG_NUMBER_OF_COLUMNS_IN_SELECT = 1222
-ER_CANT_UPDATE_WITH_READLOCK = 1223
-ER_MIXING_NOT_ALLOWED = 1224
-ER_DUP_ARGUMENT = 1225
-ER_USER_LIMIT_REACHED = 1226
-ER_SPECIFIC_ACCESS_DENIED_ERROR = 1227
-ER_LOCAL_VARIABLE = 1228
-ER_GLOBAL_VARIABLE = 1229
-ER_NO_DEFAULT = 1230
-ER_WRONG_VALUE_FOR_VAR = 1231
-ER_WRONG_TYPE_FOR_VAR = 1232
-ER_VAR_CANT_BE_READ = 1233
-ER_CANT_USE_OPTION_HERE = 1234
-ER_NOT_SUPPORTED_YET = 1235
-ER_MASTER_FATAL_ERROR_READING_BINLOG = 1236
-ER_SLAVE_IGNORED_TABLE = 1237
-ER_INCORRECT_GLOBAL_LOCAL_VAR = 1238
-ER_WRONG_FK_DEF = 1239
-ER_KEY_REF_DO_NOT_MATCH_TABLE_REF = 1240
-ER_OPERAND_COLUMNS = 1241
-ER_SUBQUERY_NO_1_ROW = 1242
-ER_UNKNOWN_STMT_HANDLER = 1243
-ER_CORRUPT_HELP_DB = 1244
-ER_CYCLIC_REFERENCE = 1245
-ER_AUTO_CONVERT = 1246
-ER_ILLEGAL_REFERENCE = 1247
-ER_DERIVED_MUST_HAVE_ALIAS = 1248
-ER_SELECT_REDUCED = 1249
-ER_TABLENAME_NOT_ALLOWED_HERE = 1250
-ER_NOT_SUPPORTED_AUTH_MODE = 1251
-ER_SPATIAL_CANT_HAVE_NULL = 1252
-ER_COLLATION_CHARSET_MISMATCH = 1253
-ER_SLAVE_WAS_RUNNING = 1254
-ER_SLAVE_WAS_NOT_RUNNING = 1255
-ER_TOO_BIG_FOR_UNCOMPRESS = 1256
-ER_ZLIB_Z_MEM_ERROR = 1257
-ER_ZLIB_Z_BUF_ERROR = 1258
-ER_ZLIB_Z_DATA_ERROR = 1259
-ER_CUT_VALUE_GROUP_CONCAT = 1260
-ER_WARN_TOO_FEW_RECORDS = 1261
-ER_WARN_TOO_MANY_RECORDS = 1262
-ER_WARN_NULL_TO_NOTNULL = 1263
-ER_WARN_DATA_OUT_OF_RANGE = 1264
-WARN_DATA_TRUNCATED = 1265
-ER_WARN_USING_OTHER_HANDLER = 1266
-ER_CANT_AGGREGATE_2COLLATIONS = 1267
-ER_DROP_USER = 1268
-ER_REVOKE_GRANTS = 1269
-ER_CANT_AGGREGATE_3COLLATIONS = 1270
-ER_CANT_AGGREGATE_NCOLLATIONS = 1271
-ER_VARIABLE_IS_NOT_STRUCT = 1272
-ER_UNKNOWN_COLLATION = 1273
-ER_SLAVE_IGNORED_SSL_PARAMS = 1274
-ER_SERVER_IS_IN_SECURE_AUTH_MODE = 1275
-ER_WARN_FIELD_RESOLVED = 1276
-ER_BAD_SLAVE_UNTIL_COND = 1277
-ER_MISSING_SKIP_SLAVE = 1278
-ER_UNTIL_COND_IGNORED = 1279
-ER_WRONG_NAME_FOR_INDEX = 1280
-ER_WRONG_NAME_FOR_CATALOG = 1281
-ER_WARN_QC_RESIZE = 1282
-ER_BAD_FT_COLUMN = 1283
-ER_UNKNOWN_KEY_CACHE = 1284
-ER_WARN_HOSTNAME_WONT_WORK = 1285
-ER_UNKNOWN_STORAGE_ENGINE = 1286
-ER_WARN_DEPRECATED_SYNTAX = 1287
-ER_NON_UPDATABLE_TABLE = 1288
-ER_FEATURE_DISABLED = 1289
-ER_OPTION_PREVENTS_STATEMENT = 1290
-ER_DUPLICATED_VALUE_IN_TYPE = 1291
-ER_TRUNCATED_WRONG_VALUE = 1292
-ER_TOO_MUCH_AUTO_TIMESTAMP_COLS = 1293
-ER_INVALID_ON_UPDATE = 1294
-ER_UNSUPPORTED_PS = 1295
-ER_GET_ERRMSG = 1296
-ER_GET_TEMPORARY_ERRMSG = 1297
-ER_UNKNOWN_TIME_ZONE = 1298
-ER_WARN_INVALID_TIMESTAMP = 1299
-ER_INVALID_CHARACTER_STRING = 1300
-ER_WARN_ALLOWED_PACKET_OVERFLOWED = 1301
-ER_CONFLICTING_DECLARATIONS = 1302
-ER_SP_NO_RECURSIVE_CREATE = 1303
-ER_SP_ALREADY_EXISTS = 1304
-ER_SP_DOES_NOT_EXIST = 1305
-ER_SP_DROP_FAILED = 1306
-ER_SP_STORE_FAILED = 1307
-ER_SP_LILABEL_MISMATCH = 1308
-ER_SP_LABEL_REDEFINE = 1309
-ER_SP_LABEL_MISMATCH = 1310
-ER_SP_UNINIT_VAR = 1311
-ER_SP_BADSELECT = 1312
-ER_SP_BADRETURN = 1313
-ER_SP_BADSTATEMENT = 1314
-ER_UPDATE_LOG_DEPRECATED_IGNORED = 1315
-ER_UPDATE_LOG_DEPRECATED_TRANSLATED = 1316
-ER_QUERY_INTERRUPTED = 1317
-ER_SP_WRONG_NO_OF_ARGS = 1318
-ER_SP_COND_MISMATCH = 1319
-ER_SP_NORETURN = 1320
-ER_SP_NORETURNEND = 1321
-ER_SP_BAD_CURSOR_QUERY = 1322
-ER_SP_BAD_CURSOR_SELECT = 1323
-ER_SP_CURSOR_MISMATCH = 1324
-ER_SP_CURSOR_ALREADY_OPEN = 1325
-ER_SP_CURSOR_NOT_OPEN = 1326
-ER_SP_UNDECLARED_VAR = 1327
-ER_SP_WRONG_NO_OF_FETCH_ARGS = 1328
-ER_SP_FETCH_NO_DATA = 1329
-ER_SP_DUP_PARAM = 1330
-ER_SP_DUP_VAR = 1331
-ER_SP_DUP_COND = 1332
-ER_SP_DUP_CURS = 1333
-ER_SP_CANT_ALTER = 1334
-ER_SP_SUBSELECT_NYI = 1335
-ER_STMT_NOT_ALLOWED_IN_SF_OR_TRG = 1336
-ER_SP_VARCOND_AFTER_CURSHNDLR = 1337
-ER_SP_CURSOR_AFTER_HANDLER = 1338
-ER_SP_CASE_NOT_FOUND = 1339
-ER_FPARSER_TOO_BIG_FILE = 1340
-ER_FPARSER_BAD_HEADER = 1341
-ER_FPARSER_EOF_IN_COMMENT = 1342
-ER_FPARSER_ERROR_IN_PARAMETER = 1343
-ER_FPARSER_EOF_IN_UNKNOWN_PARAMETER = 1344
-ER_VIEW_NO_EXPLAIN = 1345
-ER_FRM_UNKNOWN_TYPE = 1346
-ER_WRONG_OBJECT = 1347
-ER_NONUPDATEABLE_COLUMN = 1348
-ER_VIEW_SELECT_DERIVED = 1349
-ER_VIEW_SELECT_CLAUSE = 1350
-ER_VIEW_SELECT_VARIABLE = 1351
-ER_VIEW_SELECT_TMPTABLE = 1352
-ER_VIEW_WRONG_LIST = 1353
-ER_WARN_VIEW_MERGE = 1354
-ER_WARN_VIEW_WITHOUT_KEY = 1355
-ER_VIEW_INVALID = 1356
-ER_SP_NO_DROP_SP = 1357
-ER_SP_GOTO_IN_HNDLR = 1358
-ER_TRG_ALREADY_EXISTS = 1359
-ER_TRG_DOES_NOT_EXIST = 1360
-ER_TRG_ON_VIEW_OR_TEMP_TABLE = 1361
-ER_TRG_CANT_CHANGE_ROW = 1362
-ER_TRG_NO_SUCH_ROW_IN_TRG = 1363
-ER_NO_DEFAULT_FOR_FIELD = 1364
-ER_DIVISION_BY_ZERO = 1365
-ER_TRUNCATED_WRONG_VALUE_FOR_FIELD = 1366
-ER_ILLEGAL_VALUE_FOR_TYPE = 1367
-ER_VIEW_NONUPD_CHECK = 1368
-ER_VIEW_CHECK_FAILED = 1369
-ER_PROCACCESS_DENIED_ERROR = 1370
-ER_RELAY_LOG_FAIL = 1371
-ER_PASSWD_LENGTH = 1372
-ER_UNKNOWN_TARGET_BINLOG = 1373
-ER_IO_ERR_LOG_INDEX_READ = 1374
-ER_BINLOG_PURGE_PROHIBITED = 1375
-ER_FSEEK_FAIL = 1376
-ER_BINLOG_PURGE_FATAL_ERR = 1377
-ER_LOG_IN_USE = 1378
-ER_LOG_PURGE_UNKNOWN_ERR = 1379
-ER_RELAY_LOG_INIT = 1380
-ER_NO_BINARY_LOGGING = 1381
-ER_RESERVED_SYNTAX = 1382
-ER_WSAS_FAILED = 1383
-ER_DIFF_GROUPS_PROC = 1384
-ER_NO_GROUP_FOR_PROC = 1385
-ER_ORDER_WITH_PROC = 1386
-ER_LOGGING_PROHIBIT_CHANGING_OF = 1387
-ER_NO_FILE_MAPPING = 1388
-ER_WRONG_MAGIC = 1389
-ER_PS_MANY_PARAM = 1390
-ER_KEY_PART_0 = 1391
-ER_VIEW_CHECKSUM = 1392
-ER_VIEW_MULTIUPDATE = 1393
-ER_VIEW_NO_INSERT_FIELD_LIST = 1394
-ER_VIEW_DELETE_MERGE_VIEW = 1395
-ER_CANNOT_USER = 1396
-ER_XAER_NOTA = 1397
-ER_XAER_INVAL = 1398
-ER_XAER_RMFAIL = 1399
-ER_XAER_OUTSIDE = 1400
-ER_XAER_RMERR = 1401
-ER_XA_RBROLLBACK = 1402
-ER_NONEXISTING_PROC_GRANT = 1403
-ER_PROC_AUTO_GRANT_FAIL = 1404
-ER_PROC_AUTO_REVOKE_FAIL = 1405
-ER_DATA_TOO_LONG = 1406
-ER_SP_BAD_SQLSTATE = 1407
-ER_STARTUP = 1408
-ER_LOAD_FROM_FIXED_SIZE_ROWS_TO_VAR = 1409
-ER_CANT_CREATE_USER_WITH_GRANT = 1410
-ER_WRONG_VALUE_FOR_TYPE = 1411
-ER_TABLE_DEF_CHANGED = 1412
-ER_SP_DUP_HANDLER = 1413
-ER_SP_NOT_VAR_ARG = 1414
-ER_SP_NO_RETSET = 1415
-ER_CANT_CREATE_GEOMETRY_OBJECT = 1416
-ER_FAILED_ROUTINE_BREAK_BINLOG = 1417
-ER_BINLOG_UNSAFE_ROUTINE = 1418
-ER_BINLOG_CREATE_ROUTINE_NEED_SUPER = 1419
-ER_EXEC_STMT_WITH_OPEN_CURSOR = 1420
-ER_STMT_HAS_NO_OPEN_CURSOR = 1421
-ER_COMMIT_NOT_ALLOWED_IN_SF_OR_TRG = 1422
-ER_NO_DEFAULT_FOR_VIEW_FIELD = 1423
-ER_SP_NO_RECURSION = 1424
-ER_TOO_BIG_SCALE = 1425
-ER_TOO_BIG_PRECISION = 1426
-ER_M_BIGGER_THAN_D = 1427
-ER_WRONG_LOCK_OF_SYSTEM_TABLE = 1428
-ER_CONNECT_TO_FOREIGN_DATA_SOURCE = 1429
-ER_QUERY_ON_FOREIGN_DATA_SOURCE = 1430
-ER_FOREIGN_DATA_SOURCE_DOESNT_EXIST = 1431
-ER_FOREIGN_DATA_STRING_INVALID_CANT_CREATE = 1432
-ER_FOREIGN_DATA_STRING_INVALID = 1433
-ER_CANT_CREATE_FEDERATED_TABLE = 1434
-ER_TRG_IN_WRONG_SCHEMA = 1435
-ER_STACK_OVERRUN_NEED_MORE = 1436
-ER_TOO_LONG_BODY = 1437
-ER_WARN_CANT_DROP_DEFAULT_KEYCACHE = 1438
-ER_TOO_BIG_DISPLAYWIDTH = 1439
-ER_XAER_DUPID = 1440
-ER_DATETIME_FUNCTION_OVERFLOW = 1441
-ER_CANT_UPDATE_USED_TABLE_IN_SF_OR_TRG = 1442
-ER_VIEW_PREVENT_UPDATE = 1443
-ER_PS_NO_RECURSION = 1444
-ER_SP_CANT_SET_AUTOCOMMIT = 1445
-ER_MALFORMED_DEFINER = 1446
-ER_VIEW_FRM_NO_USER = 1447
-ER_VIEW_OTHER_USER = 1448
-ER_NO_SUCH_USER = 1449
-ER_FORBID_SCHEMA_CHANGE = 1450
-ER_ROW_IS_REFERENCED_2 = 1451
-ER_NO_REFERENCED_ROW_2 = 1452
-ER_SP_BAD_VAR_SHADOW = 1453
-ER_TRG_NO_DEFINER = 1454
-ER_OLD_FILE_FORMAT = 1455
-ER_SP_RECURSION_LIMIT = 1456
-ER_SP_PROC_TABLE_CORRUPT = 1457
-ER_SP_WRONG_NAME = 1458
-ER_TABLE_NEEDS_UPGRADE = 1459
-ER_SP_NO_AGGREGATE = 1460
-ER_MAX_PREPARED_STMT_COUNT_REACHED = 1461
-ER_VIEW_RECURSIVE = 1462
-ER_NON_GROUPING_FIELD_USED = 1463
-ER_TABLE_CANT_HANDLE_SPKEYS = 1464
-ER_NO_TRIGGERS_ON_SYSTEM_SCHEMA = 1465
-ER_REMOVED_SPACES = 1466
-ER_AUTOINC_READ_FAILED = 1467
-ER_USERNAME = 1468
-ER_HOSTNAME = 1469
-ER_WRONG_STRING_LENGTH = 1470
-ER_NON_INSERTABLE_TABLE = 1471
-ER_ADMIN_WRONG_MRG_TABLE = 1472
-ER_TOO_HIGH_LEVEL_OF_NESTING_FOR_SELECT = 1473
-ER_NAME_BECOMES_EMPTY = 1474
-ER_AMBIGUOUS_FIELD_TERM = 1475
-ER_FOREIGN_SERVER_EXISTS = 1476
-ER_FOREIGN_SERVER_DOESNT_EXIST = 1477
-ER_ILLEGAL_HA_CREATE_OPTION = 1478
-ER_PARTITION_REQUIRES_VALUES_ERROR = 1479
-ER_PARTITION_WRONG_VALUES_ERROR = 1480
-ER_PARTITION_MAXVALUE_ERROR = 1481
-ER_PARTITION_SUBPARTITION_ERROR = 1482
-ER_PARTITION_SUBPART_MIX_ERROR = 1483
-ER_PARTITION_WRONG_NO_PART_ERROR = 1484
-ER_PARTITION_WRONG_NO_SUBPART_ERROR = 1485
-ER_WRONG_EXPR_IN_PARTITION_FUNC_ERROR = 1486
-ER_NOT_CONSTANT_EXPRESSION = 1487
-ER_FIELD_NOT_FOUND_PART_ERROR = 1488
-ER_LIST_OF_FIELDS_ONLY_IN_HASH_ERROR = 1489
-ER_INCONSISTENT_PARTITION_INFO_ERROR = 1490
-ER_PARTITION_FUNC_NOT_ALLOWED_ERROR = 1491
-ER_PARTITIONS_MUST_BE_DEFINED_ERROR = 1492
-ER_RANGE_NOT_INCREASING_ERROR = 1493
-ER_INCONSISTENT_TYPE_OF_FUNCTIONS_ERROR = 1494
-ER_MULTIPLE_DEF_CONST_IN_LIST_PART_ERROR = 1495
-ER_PARTITION_ENTRY_ERROR = 1496
-ER_MIX_HANDLER_ERROR = 1497
-ER_PARTITION_NOT_DEFINED_ERROR = 1498
-ER_TOO_MANY_PARTITIONS_ERROR = 1499
-ER_SUBPARTITION_ERROR = 1500
-ER_CANT_CREATE_HANDLER_FILE = 1501
-ER_BLOB_FIELD_IN_PART_FUNC_ERROR = 1502
-ER_UNIQUE_KEY_NEED_ALL_FIELDS_IN_PF = 1503
-ER_NO_PARTS_ERROR = 1504
-ER_PARTITION_MGMT_ON_NONPARTITIONED = 1505
-ER_FEATURE_NOT_SUPPORTED_WITH_PARTITIONING = 1506
-ER_PARTITION_DOES_NOT_EXIST = 1507
-ER_DROP_LAST_PARTITION = 1508
-ER_COALESCE_ONLY_ON_HASH_PARTITION = 1509
-ER_REORG_HASH_ONLY_ON_SAME_NO = 1510
-ER_REORG_NO_PARAM_ERROR = 1511
-ER_ONLY_ON_RANGE_LIST_PARTITION = 1512
-ER_ADD_PARTITION_SUBPART_ERROR = 1513
-ER_ADD_PARTITION_NO_NEW_PARTITION = 1514
-ER_COALESCE_PARTITION_NO_PARTITION = 1515
-ER_REORG_PARTITION_NOT_EXIST = 1516
-ER_SAME_NAME_PARTITION = 1517
-ER_NO_BINLOG_ERROR = 1518
-ER_CONSECUTIVE_REORG_PARTITIONS = 1519
-ER_REORG_OUTSIDE_RANGE = 1520
-ER_PARTITION_FUNCTION_FAILURE = 1521
-ER_PART_STATE_ERROR = 1522
-ER_LIMITED_PART_RANGE = 1523
-ER_PLUGIN_IS_NOT_LOADED = 1524
-ER_WRONG_VALUE = 1525
-ER_NO_PARTITION_FOR_GIVEN_VALUE = 1526
-ER_FILEGROUP_OPTION_ONLY_ONCE = 1527
-ER_CREATE_FILEGROUP_FAILED = 1528
-ER_DROP_FILEGROUP_FAILED = 1529
-ER_TABLESPACE_AUTO_EXTEND_ERROR = 1530
-ER_WRONG_SIZE_NUMBER = 1531
-ER_SIZE_OVERFLOW_ERROR = 1532
-ER_ALTER_FILEGROUP_FAILED = 1533
-ER_BINLOG_ROW_LOGGING_FAILED = 1534
-ER_BINLOG_ROW_WRONG_TABLE_DEF = 1535
-ER_BINLOG_ROW_RBR_TO_SBR = 1536
-ER_EVENT_ALREADY_EXISTS = 1537
-ER_EVENT_STORE_FAILED = 1538
-ER_EVENT_DOES_NOT_EXIST = 1539
-ER_EVENT_CANT_ALTER = 1540
-ER_EVENT_DROP_FAILED = 1541
-ER_EVENT_INTERVAL_NOT_POSITIVE_OR_TOO_BIG = 1542
-ER_EVENT_ENDS_BEFORE_STARTS = 1543
-ER_EVENT_EXEC_TIME_IN_THE_PAST = 1544
-ER_EVENT_OPEN_TABLE_FAILED = 1545
-ER_EVENT_NEITHER_M_EXPR_NOR_M_AT = 1546
-ER_EVENT_CANNOT_DELETE = 1549
-ER_EVENT_COMPILE_ERROR = 1550
-ER_EVENT_SAME_NAME = 1551
-ER_EVENT_DATA_TOO_LONG = 1552
-ER_DROP_INDEX_FK = 1553
-ER_WARN_DEPRECATED_SYNTAX_WITH_VER = 1554
-ER_CANT_WRITE_LOCK_LOG_TABLE = 1555
-ER_CANT_LOCK_LOG_TABLE = 1556
-ER_COL_COUNT_DOESNT_MATCH_PLEASE_UPDATE = 1558
-ER_TEMP_TABLE_PREVENTS_SWITCH_OUT_OF_RBR = 1559
-ER_STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1560
-ER_PARTITION_NO_TEMPORARY = 1562
-ER_PARTITION_CONST_DOMAIN_ERROR = 1563
-ER_PARTITION_FUNCTION_IS_NOT_ALLOWED = 1564
-ER_DDL_LOG_ERROR = 1565
-ER_NULL_IN_VALUES_LESS_THAN = 1566
-ER_WRONG_PARTITION_NAME = 1567
-ER_CANT_CHANGE_TX_CHARACTERISTICS = 1568
-ER_DUP_ENTRY_AUTOINCREMENT_CASE = 1569
-ER_EVENT_MODIFY_QUEUE_ERROR = 1570
-ER_EVENT_SET_VAR_ERROR = 1571
-ER_PARTITION_MERGE_ERROR = 1572
-ER_CANT_ACTIVATE_LOG = 1573
-ER_RBR_NOT_AVAILABLE = 1574
-ER_BASE64_DECODE_ERROR = 1575
-ER_EVENT_RECURSION_FORBIDDEN = 1576
-ER_EVENTS_DB_ERROR = 1577
-ER_ONLY_INTEGERS_ALLOWED = 1578
-ER_UNSUPORTED_LOG_ENGINE = 1579
-ER_BAD_LOG_STATEMENT = 1580
-ER_CANT_RENAME_LOG_TABLE = 1581
-ER_WRONG_PARAMCOUNT_TO_NATIVE_FCT = 1582
-ER_WRONG_PARAMETERS_TO_NATIVE_FCT = 1583
-ER_WRONG_PARAMETERS_TO_STORED_FCT = 1584
-ER_NATIVE_FCT_NAME_COLLISION = 1585
-ER_DUP_ENTRY_WITH_KEY_NAME = 1586
-ER_BINLOG_PURGE_EMFILE = 1587
-ER_EVENT_CANNOT_CREATE_IN_THE_PAST = 1588
-ER_EVENT_CANNOT_ALTER_IN_THE_PAST = 1589
-ER_SLAVE_INCIDENT = 1590
-ER_NO_PARTITION_FOR_GIVEN_VALUE_SILENT = 1591
-ER_BINLOG_UNSAFE_STATEMENT = 1592
-ER_SLAVE_FATAL_ERROR = 1593
-ER_SLAVE_RELAY_LOG_READ_FAILURE = 1594
-ER_SLAVE_RELAY_LOG_WRITE_FAILURE = 1595
-ER_SLAVE_CREATE_EVENT_FAILURE = 1596
-ER_SLAVE_MASTER_COM_FAILURE = 1597
-ER_BINLOG_LOGGING_IMPOSSIBLE = 1598
-ER_VIEW_NO_CREATION_CTX = 1599
-ER_VIEW_INVALID_CREATION_CTX = 1600
-ER_SR_INVALID_CREATION_CTX = 1601
-ER_TRG_CORRUPTED_FILE = 1602
-ER_TRG_NO_CREATION_CTX = 1603
-ER_TRG_INVALID_CREATION_CTX = 1604
-ER_EVENT_INVALID_CREATION_CTX = 1605
-ER_TRG_CANT_OPEN_TABLE = 1606
-ER_CANT_CREATE_SROUTINE = 1607
-ER_NO_FORMAT_DESCRIPTION_EVENT_BEFORE_BINLOG_STATEMENT = 1609
-ER_SLAVE_CORRUPT_EVENT = 1610
-ER_LOAD_DATA_INVALID_COLUMN = 1611
-ER_LOG_PURGE_NO_FILE = 1612
-ER_XA_RBTIMEOUT = 1613
-ER_XA_RBDEADLOCK = 1614
-ER_NEED_REPREPARE = 1615
-ER_DELAYED_NOT_SUPPORTED = 1616
-WARN_NO_MASTER_INFO = 1617
-WARN_OPTION_IGNORED = 1618
-ER_PLUGIN_DELETE_BUILTIN = 1619
-WARN_PLUGIN_BUSY = 1620
-ER_VARIABLE_IS_READONLY = 1621
-ER_WARN_ENGINE_TRANSACTION_ROLLBACK = 1622
-ER_SLAVE_HEARTBEAT_FAILURE = 1623
-ER_SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE = 1624
-ER_CONFLICT_FN_PARSE_ERROR = 1626
-ER_EXCEPTIONS_WRITE_ERROR = 1627
-ER_TOO_LONG_TABLE_COMMENT = 1628
-ER_TOO_LONG_FIELD_COMMENT = 1629
-ER_FUNC_INEXISTENT_NAME_COLLISION = 1630
-ER_DATABASE_NAME = 1631
-ER_TABLE_NAME = 1632
-ER_PARTITION_NAME = 1633
-ER_SUBPARTITION_NAME = 1634
-ER_TEMPORARY_NAME = 1635
-ER_RENAMED_NAME = 1636
-ER_TOO_MANY_CONCURRENT_TRXS = 1637
-WARN_NON_ASCII_SEPARATOR_NOT_IMPLEMENTED = 1638
-ER_DEBUG_SYNC_TIMEOUT = 1639
-ER_DEBUG_SYNC_HIT_LIMIT = 1640
-ER_DUP_SIGNAL_SET = 1641
-ER_SIGNAL_WARN = 1642
-ER_SIGNAL_NOT_FOUND = 1643
-ER_SIGNAL_EXCEPTION = 1644
-ER_RESIGNAL_WITHOUT_ACTIVE_HANDLER = 1645
-ER_SIGNAL_BAD_CONDITION_TYPE = 1646
-WARN_COND_ITEM_TRUNCATED = 1647
-ER_COND_ITEM_TOO_LONG = 1648
-ER_UNKNOWN_LOCALE = 1649
-ER_SLAVE_IGNORE_SERVER_IDS = 1650
-ER_QUERY_CACHE_DISABLED = 1651
-ER_SAME_NAME_PARTITION_FIELD = 1652
-ER_PARTITION_COLUMN_LIST_ERROR = 1653
-ER_WRONG_TYPE_COLUMN_VALUE_ERROR = 1654
-ER_TOO_MANY_PARTITION_FUNC_FIELDS_ERROR = 1655
-ER_MAXVALUE_IN_VALUES_IN = 1656
-ER_TOO_MANY_VALUES_ERROR = 1657
-ER_ROW_SINGLE_PARTITION_FIELD_ERROR = 1658
-ER_FIELD_TYPE_NOT_ALLOWED_AS_PARTITION_FIELD = 1659
-ER_PARTITION_FIELDS_TOO_LONG = 1660
-ER_BINLOG_ROW_ENGINE_AND_STMT_ENGINE = 1661
-ER_BINLOG_ROW_MODE_AND_STMT_ENGINE = 1662
-ER_BINLOG_UNSAFE_AND_STMT_ENGINE = 1663
-ER_BINLOG_ROW_INJECTION_AND_STMT_ENGINE = 1664
-ER_BINLOG_STMT_MODE_AND_ROW_ENGINE = 1665
-ER_BINLOG_ROW_INJECTION_AND_STMT_MODE = 1666
-ER_BINLOG_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1667
-ER_BINLOG_UNSAFE_LIMIT = 1668
-ER_BINLOG_UNSAFE_INSERT_DELAYED = 1669
-ER_BINLOG_UNSAFE_SYSTEM_TABLE = 1670
-ER_BINLOG_UNSAFE_AUTOINC_COLUMNS = 1671
-ER_BINLOG_UNSAFE_UDF = 1672
-ER_BINLOG_UNSAFE_SYSTEM_VARIABLE = 1673
-ER_BINLOG_UNSAFE_SYSTEM_FUNCTION = 1674
-ER_BINLOG_UNSAFE_NONTRANS_AFTER_TRANS = 1675
-ER_MESSAGE_AND_STATEMENT = 1676
-ER_SLAVE_CONVERSION_FAILED = 1677
-ER_SLAVE_CANT_CREATE_CONVERSION = 1678
-ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1679
-ER_PATH_LENGTH = 1680
-ER_WARN_DEPRECATED_SYNTAX_NO_REPLACEMENT = 1681
-ER_WRONG_NATIVE_TABLE_STRUCTURE = 1682
-ER_WRONG_PERFSCHEMA_USAGE = 1683
-ER_WARN_I_S_SKIPPED_TABLE = 1684
-ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1685
-ER_STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1686
-ER_SPATIAL_MUST_HAVE_GEOM_COL = 1687
-ER_TOO_LONG_INDEX_COMMENT = 1688
-ER_LOCK_ABORTED = 1689
-ER_DATA_OUT_OF_RANGE = 1690
-ER_WRONG_SPVAR_TYPE_IN_LIMIT = 1691
-ER_BINLOG_UNSAFE_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1692
-ER_BINLOG_UNSAFE_MIXED_STATEMENT = 1693
-ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1694
-ER_STORED_FUNCTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1695
-ER_FAILED_READ_FROM_PAR_FILE = 1696
-ER_VALUES_IS_NOT_INT_TYPE_ERROR = 1697
-ER_ACCESS_DENIED_NO_PASSWORD_ERROR = 1698
-ER_SET_PASSWORD_AUTH_PLUGIN = 1699
-ER_GRANT_PLUGIN_USER_EXISTS = 1700
-ER_TRUNCATE_ILLEGAL_FK = 1701
-ER_PLUGIN_IS_PERMANENT = 1702
-ER_SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MIN = 1703
-ER_SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MAX = 1704
-ER_STMT_CACHE_FULL = 1705
-ER_MULTI_UPDATE_KEY_CONFLICT = 1706
-ER_TABLE_NEEDS_REBUILD = 1707
-WARN_OPTION_BELOW_LIMIT = 1708
-ER_INDEX_COLUMN_TOO_LONG = 1709
-ER_ERROR_IN_TRIGGER_BODY = 1710
-ER_ERROR_IN_UNKNOWN_TRIGGER_BODY = 1711
-ER_INDEX_CORRUPT = 1712
-ER_UNDO_RECORD_TOO_BIG = 1713
-ER_BINLOG_UNSAFE_INSERT_IGNORE_SELECT = 1714
-ER_BINLOG_UNSAFE_INSERT_SELECT_UPDATE = 1715
-ER_BINLOG_UNSAFE_REPLACE_SELECT = 1716
-ER_BINLOG_UNSAFE_CREATE_IGNORE_SELECT = 1717
-ER_BINLOG_UNSAFE_CREATE_REPLACE_SELECT = 1718
-ER_BINLOG_UNSAFE_UPDATE_IGNORE = 1719
-ER_BINLOG_UNSAFE_WRITE_AUTOINC_SELECT = 1722
-ER_BINLOG_UNSAFE_CREATE_SELECT_AUTOINC = 1723
-ER_BINLOG_UNSAFE_INSERT_TWO_KEYS = 1724
-ER_VERS_NOT_ALLOWED = 1726
-ER_BINLOG_UNSAFE_AUTOINC_NOT_FIRST = 1727
-ER_CANNOT_LOAD_FROM_TABLE_V2 = 1728
-ER_MASTER_DELAY_VALUE_OUT_OF_RANGE = 1729
-ER_ONLY_FD_AND_RBR_EVENTS_ALLOWED_IN_BINLOG_STATEMENT = 1730
-ER_PARTITION_EXCHANGE_DIFFERENT_OPTION = 1731
-ER_PARTITION_EXCHANGE_PART_TABLE = 1732
-ER_PARTITION_EXCHANGE_TEMP_TABLE = 1733
-ER_PARTITION_INSTEAD_OF_SUBPARTITION = 1734
-ER_UNKNOWN_PARTITION = 1735
-ER_TABLES_DIFFERENT_METADATA = 1736
-ER_ROW_DOES_NOT_MATCH_PARTITION = 1737
-ER_BINLOG_CACHE_SIZE_GREATER_THAN_MAX = 1738
-ER_WARN_INDEX_NOT_APPLICABLE = 1739
-ER_PARTITION_EXCHANGE_FOREIGN_KEY = 1740
-ER_NO_SUCH_KEY_VALUE = 1741
-ER_VALUE_TOO_LONG = 1742
-ER_NETWORK_READ_EVENT_CHECKSUM_FAILURE = 1743
-ER_BINLOG_READ_EVENT_CHECKSUM_FAILURE = 1744
-ER_BINLOG_STMT_CACHE_SIZE_GREATER_THAN_MAX = 1745
-ER_CANT_UPDATE_TABLE_IN_CREATE_TABLE_SELECT = 1746
-ER_PARTITION_CLAUSE_ON_NONPARTITIONED = 1747
-ER_ROW_DOES_NOT_MATCH_GIVEN_PARTITION_SET = 1748
-ER_CHANGE_RPL_INFO_REPOSITORY_FAILURE = 1750
-ER_WARNING_NOT_COMPLETE_ROLLBACK_WITH_CREATED_TEMP_TABLE = 1751
-ER_WARNING_NOT_COMPLETE_ROLLBACK_WITH_DROPPED_TEMP_TABLE = 1752
-ER_MTS_FEATURE_IS_NOT_SUPPORTED = 1753
-ER_MTS_UPDATED_DBS_GREATER_MAX = 1754
-ER_MTS_CANT_PARALLEL = 1755
-ER_MTS_INCONSISTENT_DATA = 1756
-ER_FULLTEXT_NOT_SUPPORTED_WITH_PARTITIONING = 1757
-ER_DA_INVALID_CONDITION_NUMBER = 1758
-ER_INSECURE_PLAIN_TEXT = 1759
-ER_INSECURE_CHANGE_MASTER = 1760
-ER_FOREIGN_DUPLICATE_KEY_WITH_CHILD_INFO = 1761
-ER_FOREIGN_DUPLICATE_KEY_WITHOUT_CHILD_INFO = 1762
-ER_SQLTHREAD_WITH_SECURE_SLAVE = 1763
-ER_TABLE_HAS_NO_FT = 1764
-ER_VARIABLE_NOT_SETTABLE_IN_SF_OR_TRIGGER = 1765
-ER_VARIABLE_NOT_SETTABLE_IN_TRANSACTION = 1766
-ER_GTID_NEXT_IS_NOT_IN_GTID_NEXT_LIST = 1767
-ER_CANT_CHANGE_GTID_NEXT_IN_TRANSACTION_WHEN_GTID_NEXT_LIST_IS_NULL = 1768
-ER_SET_STATEMENT_CANNOT_INVOKE_FUNCTION = 1769
-ER_GTID_NEXT_CANT_BE_AUTOMATIC_IF_GTID_NEXT_LIST_IS_NON_NULL = 1770
-ER_SKIPPING_LOGGED_TRANSACTION = 1771
-ER_MALFORMED_GTID_SET_SPECIFICATION = 1772
-ER_MALFORMED_GTID_SET_ENCODING = 1773
-ER_MALFORMED_GTID_SPECIFICATION = 1774
-ER_GNO_EXHAUSTED = 1775
-ER_BAD_SLAVE_AUTO_POSITION = 1776
-ER_AUTO_POSITION_REQUIRES_GTID_MODE_ON = 1777
-ER_CANT_DO_IMPLICIT_COMMIT_IN_TRX_WHEN_GTID_NEXT_IS_SET = 1778
-ER_GTID_MODE_2_OR_3_REQUIRES_ENFORCE_GTID_CONSISTENCY_ON = 1779
-ER_GTID_MODE_REQUIRES_BINLOG = 1780
-ER_CANT_SET_GTID_NEXT_TO_GTID_WHEN_GTID_MODE_IS_OFF = 1781
-ER_CANT_SET_GTID_NEXT_TO_ANONYMOUS_WHEN_GTID_MODE_IS_ON = 1782
-ER_CANT_SET_GTID_NEXT_LIST_TO_NON_NULL_WHEN_GTID_MODE_IS_OFF = 1783
-ER_FOUND_GTID_EVENT_WHEN_GTID_MODE_IS_OFF = 1784
-ER_GTID_UNSAFE_NON_TRANSACTIONAL_TABLE = 1785
-ER_GTID_UNSAFE_CREATE_SELECT = 1786
-ER_GTID_UNSAFE_CREATE_DROP_TEMPORARY_TABLE_IN_TRANSACTION = 1787
-ER_GTID_MODE_CAN_ONLY_CHANGE_ONE_STEP_AT_A_TIME = 1788
-ER_MASTER_HAS_PURGED_REQUIRED_GTIDS = 1789
-ER_CANT_SET_GTID_NEXT_WHEN_OWNING_GTID = 1790
-ER_UNKNOWN_EXPLAIN_FORMAT = 1791
-ER_CANT_EXECUTE_IN_READ_ONLY_TRANSACTION = 1792
-ER_TOO_LONG_TABLE_PARTITION_COMMENT = 1793
-ER_SLAVE_CONFIGURATION = 1794
-ER_INNODB_FT_LIMIT = 1795
-ER_INNODB_NO_FT_TEMP_TABLE = 1796
-ER_INNODB_FT_WRONG_DOCID_COLUMN = 1797
-ER_INNODB_FT_WRONG_DOCID_INDEX = 1798
-ER_INNODB_ONLINE_LOG_TOO_BIG = 1799
-ER_UNKNOWN_ALTER_ALGORITHM = 1800
-ER_UNKNOWN_ALTER_LOCK = 1801
-ER_MTS_CHANGE_MASTER_CANT_RUN_WITH_GAPS = 1802
-ER_MTS_RECOVERY_FAILURE = 1803
-ER_MTS_RESET_WORKERS = 1804
-ER_COL_COUNT_DOESNT_MATCH_CORRUPTED_V2 = 1805
-ER_SLAVE_SILENT_RETRY_TRANSACTION = 1806
-ER_TABLE_SCHEMA_MISMATCH = 1808
-ER_TABLE_IN_SYSTEM_TABLESPACE = 1809
-ER_IO_READ_ERROR = 1810
-ER_IO_WRITE_ERROR = 1811
-ER_TABLESPACE_MISSING = 1812
-ER_TABLESPACE_EXISTS = 1813
-ER_TABLESPACE_DISCARDED = 1814
-ER_INTERNAL_ERROR = 1815
-ER_INNODB_IMPORT_ERROR = 1816
-ER_INNODB_INDEX_CORRUPT = 1817
-ER_INVALID_YEAR_COLUMN_LENGTH = 1818
-ER_NOT_VALID_PASSWORD = 1819
-ER_MUST_CHANGE_PASSWORD = 1820
-ER_FK_NO_INDEX_CHILD = 1821
-ER_FK_NO_INDEX_PARENT = 1822
-ER_FK_FAIL_ADD_SYSTEM = 1823
-ER_FK_CANNOT_OPEN_PARENT = 1824
-ER_FK_INCORRECT_OPTION = 1825
-ER_DUP_CONSTRAINT_NAME = 1826
-ER_PASSWORD_FORMAT = 1827
-ER_FK_COLUMN_CANNOT_DROP = 1828
-ER_FK_COLUMN_CANNOT_DROP_CHILD = 1829
-ER_FK_COLUMN_NOT_NULL = 1830
-ER_DUP_INDEX = 1831
-ER_FK_COLUMN_CANNOT_CHANGE = 1832
-ER_FK_COLUMN_CANNOT_CHANGE_CHILD = 1833
-ER_FK_CANNOT_DELETE_PARENT = 1834
-ER_MALFORMED_PACKET = 1835
-ER_READ_ONLY_MODE = 1836
-ER_GTID_NEXT_TYPE_UNDEFINED_GROUP = 1837
-ER_VARIABLE_NOT_SETTABLE_IN_SP = 1838
-ER_CANT_SET_GTID_PURGED_WHEN_GTID_MODE_IS_OFF = 1839
-ER_CANT_SET_GTID_PURGED_WHEN_GTID_EXECUTED_IS_NOT_EMPTY = 1840
-ER_CANT_SET_GTID_PURGED_WHEN_OWNED_GTIDS_IS_NOT_EMPTY = 1841
-ER_GTID_PURGED_WAS_CHANGED = 1842
-ER_GTID_EXECUTED_WAS_CHANGED = 1843
-ER_BINLOG_STMT_MODE_AND_NO_REPL_TABLES = 1844
-ER_ALTER_OPERATION_NOT_SUPPORTED = 1845
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON = 1846
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_COPY = 1847
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_PARTITION = 1848
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_RENAME = 1849
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_COLUMN_TYPE = 1850
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_CHECK = 1851
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_IGNORE = 1852
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_NOPK = 1853
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_AUTOINC = 1854
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_HIDDEN_FTS = 1855
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_CHANGE_FTS = 1856
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_FTS = 1857
-ER_SQL_SLAVE_SKIP_COUNTER_NOT_SETTABLE_IN_GTID_MODE = 1858
-ER_DUP_UNKNOWN_IN_INDEX = 1859
-ER_IDENT_CAUSES_TOO_LONG_PATH = 1860
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_NOT_NULL = 1861
-ER_MUST_CHANGE_PASSWORD_LOGIN = 1862
-ER_ROW_IN_WRONG_PARTITION = 1863
-ER_MTS_EVENT_BIGGER_PENDING_JOBS_SIZE_MAX = 1864
-ER_INNODB_NO_FT_USES_PARSER = 1865
-ER_BINLOG_LOGICAL_CORRUPTION = 1866
-ER_WARN_PURGE_LOG_IN_USE = 1867
-ER_WARN_PURGE_LOG_IS_ACTIVE = 1868
-ER_AUTO_INCREMENT_CONFLICT = 1869
-WARN_ON_BLOCKHOLE_IN_RBR = 1870
-ER_SLAVE_MI_INIT_REPOSITORY = 1871
-ER_SLAVE_RLI_INIT_REPOSITORY = 1872
-ER_ACCESS_DENIED_CHANGE_USER_ERROR = 1873
-ER_INNODB_READ_ONLY = 1874
-ER_STOP_SLAVE_SQL_THREAD_TIMEOUT = 1875
-ER_STOP_SLAVE_IO_THREAD_TIMEOUT = 1876
-ER_TABLE_CORRUPT = 1877
-ER_TEMP_FILE_WRITE_FAILURE = 1878
-ER_INNODB_FT_AUX_NOT_HEX_ID = 1879
-ER_LAST_MYSQL_ERROR_MESSAGE = 1880
-ER_ERROR_LAST_SECTION_1 = 1880
-ER_ERROR_FIRST_SECTION_2 = 1900
-ER_GENERATED_COLUMN_FUNCTION_IS_NOT_ALLOWED = 1901
-ER_PRIMARY_KEY_BASED_ON_GENERATED_COLUMN = 1903
-ER_KEY_BASED_ON_GENERATED_VIRTUAL_COLUMN = 1904
-ER_WRONG_FK_OPTION_FOR_GENERATED_COLUMN = 1905
-ER_WARNING_NON_DEFAULT_VALUE_FOR_GENERATED_COLUMN = 1906
-ER_UNSUPPORTED_ACTION_ON_GENERATED_COLUMN = 1907
-ER_UNSUPPORTED_ENGINE_FOR_GENERATED_COLUMNS = 1910
-ER_UNKNOWN_OPTION = 1911
-ER_BAD_OPTION_VALUE = 1912
-ER_DATA_OVERFLOW = 1916
-ER_DATA_TRUNCATED = 1917
-ER_BAD_DATA = 1918
-ER_DYN_COL_WRONG_FORMAT = 1919
-ER_DYN_COL_IMPLEMENTATION_LIMIT = 1920
-ER_DYN_COL_DATA = 1921
-ER_DYN_COL_WRONG_CHARSET = 1922
-ER_ILLEGAL_SUBQUERY_OPTIMIZER_SWITCHES = 1923
-ER_QUERY_CACHE_IS_DISABLED = 1924
-ER_QUERY_CACHE_IS_GLOBALY_DISABLED = 1925
-ER_VIEW_ORDERBY_IGNORED = 1926
-ER_CONNECTION_KILLED = 1927
-ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_SKIP_REPLICATION = 1929
-ER_STORED_FUNCTION_PREVENTS_SWITCH_SKIP_REPLICATION = 1930
-ER_QUERY_EXCEEDED_ROWS_EXAMINED_LIMIT = 1931
-ER_NO_SUCH_TABLE_IN_ENGINE = 1932
-ER_TARGET_NOT_EXPLAINABLE = 1933
-ER_CONNECTION_ALREADY_EXISTS = 1934
-ER_MASTER_LOG_PREFIX = 1935
-ER_CANT_START_STOP_SLAVE = 1936
-ER_SLAVE_STARTED = 1937
-ER_SLAVE_STOPPED = 1938
-ER_SQL_DISCOVER_ERROR = 1939
-ER_FAILED_GTID_STATE_INIT = 1940
-ER_INCORRECT_GTID_STATE = 1941
-ER_CANNOT_UPDATE_GTID_STATE = 1942
-ER_DUPLICATE_GTID_DOMAIN = 1943
-ER_GTID_OPEN_TABLE_FAILED = 1944
-ER_GTID_POSITION_NOT_FOUND_IN_BINLOG = 1945
-ER_CANNOT_LOAD_SLAVE_GTID_STATE = 1946
-ER_MASTER_GTID_POS_CONFLICTS_WITH_BINLOG = 1947
-ER_MASTER_GTID_POS_MISSING_DOMAIN = 1948
-ER_UNTIL_REQUIRES_USING_GTID = 1949
-ER_GTID_STRICT_OUT_OF_ORDER = 1950
-ER_GTID_START_FROM_BINLOG_HOLE = 1951
-ER_SLAVE_UNEXPECTED_MASTER_SWITCH = 1952
-ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_GTID_DOMAIN_ID_SEQ_NO = 1953
-ER_STORED_FUNCTION_PREVENTS_SWITCH_GTID_DOMAIN_ID_SEQ_NO = 1954
-ER_GTID_POSITION_NOT_FOUND_IN_BINLOG2 = 1955
-ER_BINLOG_MUST_BE_EMPTY = 1956
-ER_NO_SUCH_QUERY = 1957
-ER_BAD_BASE64_DATA = 1958
-ER_INVALID_ROLE = 1959
-ER_INVALID_CURRENT_USER = 1960
-ER_CANNOT_GRANT_ROLE = 1961
-ER_CANNOT_REVOKE_ROLE = 1962
-ER_CHANGE_SLAVE_PARALLEL_THREADS_ACTIVE = 1963
-ER_PRIOR_COMMIT_FAILED = 1964
-ER_IT_IS_A_VIEW = 1965
-ER_SLAVE_SKIP_NOT_IN_GTID = 1966
-ER_TABLE_DEFINITION_TOO_BIG = 1967
-ER_PLUGIN_INSTALLED = 1968
-ER_STATEMENT_TIMEOUT = 1969
-ER_SUBQUERIES_NOT_SUPPORTED = 1970
-ER_SET_STATEMENT_NOT_SUPPORTED = 1971
-ER_USER_CREATE_EXISTS = 1973
-ER_USER_DROP_EXISTS = 1974
-ER_ROLE_CREATE_EXISTS = 1975
-ER_ROLE_DROP_EXISTS = 1976
-ER_CANNOT_CONVERT_CHARACTER = 1977
-ER_INVALID_DEFAULT_VALUE_FOR_FIELD = 1978
-ER_KILL_QUERY_DENIED_ERROR = 1979
-ER_NO_EIS_FOR_FIELD = 1980
-ER_WARN_AGGFUNC_DEPENDENCE = 1981
-WARN_INNODB_PARTITION_OPTION_IGNORED = 1982
-ER_ERROR_LAST_SECTION_2 = 1982
-ER_ERROR_FIRST_SECTION_3 = 2000
-ER_ERROR_LAST_SECTION_3 = 2000
-ER_ERROR_FIRST_SECTION_4 = 3000
-ER_FILE_CORRUPT = 3000
-ER_ERROR_ON_MASTER = 3001
-ER_INCONSISTENT_ERROR = 3002
-ER_STORAGE_ENGINE_NOT_LOADED = 3003
-ER_GET_STACKED_DA_WITHOUT_ACTIVE_HANDLER = 3004
-ER_WARN_LEGACY_SYNTAX_CONVERTED = 3005
-ER_BINLOG_UNSAFE_FULLTEXT_PLUGIN = 3006
-ER_CANNOT_DISCARD_TEMPORARY_TABLE = 3007
-ER_FK_DEPTH_EXCEEDED = 3008
-ER_COL_COUNT_DOESNT_MATCH_PLEASE_UPDATE_V2 = 3009
-ER_WARN_TRIGGER_DOESNT_HAVE_CREATED = 3010
-ER_REFERENCED_TRG_DOES_NOT_EXIST_MYSQL = 3011
-ER_EXPLAIN_NOT_SUPPORTED = 3012
-ER_INVALID_FIELD_SIZE = 3013
-ER_MISSING_HA_CREATE_OPTION = 3014
-ER_ENGINE_OUT_OF_MEMORY = 3015
-ER_PASSWORD_EXPIRE_ANONYMOUS_USER = 3016
-ER_SLAVE_SQL_THREAD_MUST_STOP = 3017
-ER_NO_FT_MATERIALIZED_SUBQUERY = 3018
-ER_INNODB_UNDO_LOG_FULL = 3019
-ER_INVALID_ARGUMENT_FOR_LOGARITHM = 3020
-ER_SLAVE_CHANNEL_IO_THREAD_MUST_STOP = 3021
-ER_WARN_OPEN_TEMP_TABLES_MUST_BE_ZERO = 3022
-ER_WARN_ONLY_MASTER_LOG_FILE_NO_POS = 3023
-ER_QUERY_TIMEOUT = 3024
-ER_NON_RO_SELECT_DISABLE_TIMER = 3025
-ER_DUP_LIST_ENTRY = 3026
-ER_SQL_MODE_NO_EFFECT = 3027
-ER_AGGREGATE_ORDER_FOR_UNION = 3028
-ER_AGGREGATE_ORDER_NON_AGG_QUERY = 3029
-ER_SLAVE_WORKER_STOPPED_PREVIOUS_THD_ERROR = 3030
-ER_DONT_SUPPORT_SLAVE_PRESERVE_COMMIT_ORDER = 3031
-ER_SERVER_OFFLINE_MODE = 3032
-ER_GIS_DIFFERENT_SRIDS = 3033
-ER_GIS_UNSUPPORTED_ARGUMENT = 3034
-ER_GIS_UNKNOWN_ERROR = 3035
-ER_GIS_UNKNOWN_EXCEPTION = 3036
-ER_GIS_INVALID_DATA = 3037
-ER_BOOST_GEOMETRY_EMPTY_INPUT_EXCEPTION = 3038
-ER_BOOST_GEOMETRY_CENTROID_EXCEPTION = 3039
-ER_BOOST_GEOMETRY_OVERLAY_INVALID_INPUT_EXCEPTION = 3040
-ER_BOOST_GEOMETRY_TURN_INFO_EXCEPTION = 3041
-ER_BOOST_GEOMETRY_SELF_INTERSECTION_POINT_EXCEPTION = 3042
-ER_BOOST_GEOMETRY_UNKNOWN_EXCEPTION = 3043
-ER_STD_BAD_ALLOC_ERROR = 3044
-ER_STD_DOMAIN_ERROR = 3045
-ER_STD_LENGTH_ERROR = 3046
-ER_STD_INVALID_ARGUMENT = 3047
-ER_STD_OUT_OF_RANGE_ERROR = 3048
-ER_STD_OVERFLOW_ERROR = 3049
-ER_STD_RANGE_ERROR = 3050
-ER_STD_UNDERFLOW_ERROR = 3051
-ER_STD_LOGIC_ERROR = 3052
-ER_STD_RUNTIME_ERROR = 3053
-ER_STD_UNKNOWN_EXCEPTION = 3054
-ER_GIS_DATA_WRONG_ENDIANESS = 3055
-ER_CHANGE_MASTER_PASSWORD_LENGTH = 3056
-ER_USER_LOCK_WRONG_NAME = 3057
-ER_USER_LOCK_DEADLOCK = 3058
-ER_REPLACE_INACCESSIBLE_ROWS = 3059
-ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_GIS = 3060
-ER_ERROR_LAST_SECTION_4 = 3060
-ER_ERROR_FIRST_SECTION_5 = 4000
-ER_WITH_COL_WRONG_LIST = 4002
-ER_TOO_MANY_DEFINITIONS_IN_WITH_CLAUSE = 4003
-ER_DUP_QUERY_NAME = 4004
-ER_RECURSIVE_WITHOUT_ANCHORS = 4005
-ER_UNACCEPTABLE_MUTUAL_RECURSION = 4006
-ER_REF_TO_RECURSIVE_WITH_TABLE_IN_DERIVED = 4007
-ER_NOT_STANDARD_COMPLIANT_RECURSIVE = 4008
-ER_WRONG_WINDOW_SPEC_NAME = 4009
-ER_DUP_WINDOW_NAME = 4010
-ER_PARTITION_LIST_IN_REFERENCING_WINDOW_SPEC = 4011
-ER_ORDER_LIST_IN_REFERENCING_WINDOW_SPEC = 4012
-ER_WINDOW_FRAME_IN_REFERENCED_WINDOW_SPEC = 4013
-ER_BAD_COMBINATION_OF_WINDOW_FRAME_BOUND_SPECS = 4014
-ER_WRONG_PLACEMENT_OF_WINDOW_FUNCTION = 4015
-ER_WINDOW_FUNCTION_IN_WINDOW_SPEC = 4016
-ER_NOT_ALLOWED_WINDOW_FRAME = 4017
-ER_NO_ORDER_LIST_IN_WINDOW_SPEC = 4018
-ER_RANGE_FRAME_NEEDS_SIMPLE_ORDERBY = 4019
-ER_WRONG_TYPE_FOR_ROWS_FRAME = 4020
-ER_WRONG_TYPE_FOR_RANGE_FRAME = 4021
-ER_FRAME_EXCLUSION_NOT_SUPPORTED = 4022
-ER_WINDOW_FUNCTION_DONT_HAVE_FRAME = 4023
-ER_INVALID_NTILE_ARGUMENT = 4024
-ER_CONSTRAINT_FAILED = 4025
-ER_EXPRESSION_IS_TOO_BIG = 4026
-ER_ERROR_EVALUATING_EXPRESSION = 4027
-ER_CALCULATING_DEFAULT_VALUE = 4028
-ER_EXPRESSION_REFERS_TO_UNINIT_FIELD = 4029
-ER_PARTITION_DEFAULT_ERROR = 4030
-ER_REFERENCED_TRG_DOES_NOT_EXIST = 4031
-ER_INVALID_DEFAULT_PARAM = 4032
-ER_BINLOG_NON_SUPPORTED_BULK = 4033
-ER_BINLOG_UNCOMPRESS_ERROR = 4034
-ER_JSON_BAD_CHR = 4035
-ER_JSON_NOT_JSON_CHR = 4036
-ER_JSON_EOS = 4037
-ER_JSON_SYNTAX = 4038
-ER_JSON_ESCAPING = 4039
-ER_JSON_DEPTH = 4040
-ER_JSON_PATH_EOS = 4041
-ER_JSON_PATH_SYNTAX = 4042
-ER_JSON_PATH_DEPTH = 4043
-ER_JSON_PATH_NO_WILDCARD = 4044
-ER_JSON_PATH_ARRAY = 4045
-ER_JSON_ONE_OR_ALL = 4046
-ER_UNSUPPORTED_COMPRESSED_TABLE = 4047
-ER_GEOJSON_INCORRECT = 4048
-ER_GEOJSON_TOO_FEW_POINTS = 4049
-ER_GEOJSON_NOT_CLOSED = 4050
-ER_JSON_PATH_EMPTY = 4051
-ER_SLAVE_SAME_ID = 4052
-ER_FLASHBACK_NOT_SUPPORTED = 4053
-ER_KEYS_OUT_OF_ORDER = 4054
-ER_OVERLAPPING_KEYS = 4055
-ER_REQUIRE_ROW_BINLOG_FORMAT = 4056
-ER_ISOLATION_MODE_NOT_SUPPORTED = 4057
-ER_ON_DUPLICATE_DISABLED = 4058
-ER_UPDATES_WITH_CONSISTENT_SNAPSHOT = 4059
-ER_ROLLBACK_ONLY = 4060
-ER_ROLLBACK_TO_SAVEPOINT = 4061
-ER_ISOLATION_LEVEL_WITH_CONSISTENT_SNAPSHOT = 4062
-ER_UNSUPPORTED_COLLATION = 4063
-ER_METADATA_INCONSISTENCY = 4064
-ER_CF_DIFFERENT = 4065
-ER_RDB_TTL_DURATION_FORMAT = 4066
-ER_RDB_STATUS_GENERAL = 4067
-ER_RDB_STATUS_MSG = 4068
-ER_RDB_TTL_UNSUPPORTED = 4069
-ER_RDB_TTL_COL_FORMAT = 4070
-ER_PER_INDEX_CF_DEPRECATED = 4071
-ER_KEY_CREATE_DURING_ALTER = 4072
-ER_SK_POPULATE_DURING_ALTER = 4073
-ER_SUM_FUNC_WITH_WINDOW_FUNC_AS_ARG = 4074
-ER_NET_OK_PACKET_TOO_LARGE = 4075
-ER_GEOJSON_EMPTY_COORDINATES = 4076
-ER_MYROCKS_CANT_NOPAD_COLLATION = 4077
-ER_ILLEGAL_PARAMETER_DATA_TYPES2_FOR_OPERATION = 4078
-ER_ILLEGAL_PARAMETER_DATA_TYPE_FOR_OPERATION = 4079
-ER_WRONG_PARAMCOUNT_TO_CURSOR = 4080
-ER_UNKNOWN_STRUCTURED_VARIABLE = 4081
-ER_ROW_VARIABLE_DOES_NOT_HAVE_FIELD = 4082
-ER_END_IDENTIFIER_DOES_NOT_MATCH = 4083
-ER_SEQUENCE_RUN_OUT = 4084
-ER_SEQUENCE_INVALID_DATA = 4085
-ER_SEQUENCE_INVALID_TABLE_STRUCTURE = 4086
-ER_SEQUENCE_ACCESS_ERROR = 4087
-ER_SEQUENCE_BINLOG_FORMAT = 4088
-ER_NOT_SEQUENCE = 4089
-ER_NOT_SEQUENCE2 = 4090
-ER_UNKNOWN_SEQUENCES = 4091
-ER_UNKNOWN_VIEW = 4092
-ER_WRONG_INSERT_INTO_SEQUENCE = 4093
-ER_SP_STACK_TRACE = 4094
-ER_PACKAGE_ROUTINE_IN_SPEC_NOT_DEFINED_IN_BODY = 4095
-ER_PACKAGE_ROUTINE_FORWARD_DECLARATION_NOT_DEFINED = 4096
-ER_COMPRESSED_COLUMN_USED_AS_KEY = 4097
-ER_UNKNOWN_COMPRESSION_METHOD = 4098
-ER_WRONG_NUMBER_OF_VALUES_IN_TVC = 4099
-ER_FIELD_REFERENCE_IN_TVC = 4100
-ER_WRONG_TYPE_FOR_PERCENTILE_FUNC = 4101
-ER_ARGUMENT_NOT_CONSTANT = 4102
-ER_ARGUMENT_OUT_OF_RANGE = 4103
-ER_WRONG_TYPE_OF_ARGUMENT = 4104
-ER_NOT_AGGREGATE_FUNCTION = 4105
-ER_INVALID_AGGREGATE_FUNCTION = 4106
-ER_INVALID_VALUE_TO_LIMIT = 4107
-ER_INVISIBLE_NOT_NULL_WITHOUT_DEFAULT = 4108
-ER_UPDATE_INFO_WITH_SYSTEM_VERSIONING = 4109
-ER_VERS_FIELD_WRONG_TYPE = 4110
-ER_VERS_ENGINE_UNSUPPORTED = 4111
-ER_PARTITION_WRONG_TYPE = 4113
-WARN_VERS_PART_FULL = 4114
-WARN_VERS_PARAMETERS = 4115
-ER_VERS_DROP_PARTITION_INTERVAL = 4116
-WARN_VERS_PART_NON_HISTORICAL = 4118
-ER_VERS_ALTER_NOT_ALLOWED = 4119
-ER_VERS_ALTER_ENGINE_PROHIBITED = 4120
-ER_VERS_RANGE_PROHIBITED = 4121
-ER_CONFLICTING_FOR_SYSTEM_TIME = 4122
-ER_VERS_TABLE_MUST_HAVE_COLUMNS = 4123
-ER_VERS_NOT_VERSIONED = 4124
-ER_MISSING = 4125
-ER_VERS_PERIOD_COLUMNS = 4126
-ER_PART_WRONG_VALUE = 4127
-ER_VERS_WRONG_PARTS = 4128
-ER_VERS_NO_TRX_ID = 4129
-ER_VERS_ALTER_SYSTEM_FIELD = 4130
-ER_DROP_VERSIONING_SYSTEM_TIME_PARTITION = 4131
-ER_VERS_DB_NOT_SUPPORTED = 4132
-ER_VERS_TRT_IS_DISABLED = 4133
-ER_VERS_DUPLICATE_ROW_START_END = 4134
-ER_VERS_ALREADY_VERSIONED = 4135
-ER_VERS_NOT_SUPPORTED = 4137
-ER_VERS_TRX_PART_HISTORIC_ROW_NOT_SUPPORTED = 4138
-ER_INDEX_FILE_FULL = 4139
-ER_UPDATED_COLUMN_ONLY_ONCE = 4140
-ER_EMPTY_ROW_IN_TVC = 4141
-ER_VERS_QUERY_IN_PARTITION = 4142
-ER_KEY_DOESNT_SUPPORT = 4143
-ER_ALTER_OPERATION_TABLE_OPTIONS_NEED_REBUILD = 4144
-ER_BACKUP_LOCK_IS_ACTIVE = 4145
-ER_BACKUP_NOT_RUNNING = 4146
-ER_BACKUP_WRONG_STAGE = 4147
-ER_BACKUP_STAGE_FAILED = 4148
-ER_BACKUP_UNKNOWN_STAGE = 4149
-ER_USER_IS_BLOCKED = 4150
-ER_ACCOUNT_HAS_BEEN_LOCKED = 4151
-ER_PERIOD_TEMPORARY_NOT_ALLOWED = 4152
-ER_PERIOD_TYPES_MISMATCH = 4153
-ER_MORE_THAN_ONE_PERIOD = 4154
-ER_PERIOD_FIELD_WRONG_ATTRIBUTES = 4155
-ER_PERIOD_NOT_FOUND = 4156
-ER_PERIOD_COLUMNS_UPDATED = 4157
-ER_PERIOD_CONSTRAINT_DROP = 4158
-ER_TOO_LONG_KEYPART = 4159
-ER_TOO_LONG_DATABASE_COMMENT = 4160
-ER_UNKNOWN_DATA_TYPE = 4161
-ER_UNKNOWN_OPERATOR = 4162
-ER_WARN_HISTORY_ROW_START_TIME = 4163
-ER_PART_STARTS_BEYOND_INTERVAL = 4164
-ER_GALERA_REPLICATION_NOT_SUPPORTED = 4165
-ER_LOAD_INFILE_CAPABILITY_DISABLED = 4166
-ER_NO_SECURE_TRANSPORTS_CONFIGURED = 4167
-ER_SLAVE_IGNORED_SHARED_TABLE = 4168
-ER_NO_AUTOINCREMENT_WITH_UNIQUE = 4169
-ER_KEY_CONTAINS_PERIOD_FIELDS = 4170
-ER_KEY_CANT_HAVE_WITHOUT_OVERLAPS = 4171
-ER_NOT_ALLOWED_IN_THIS_CONTEXT = 4172
-ER_DATA_WAS_COMMITED_UNDER_ROLLBACK = 4173
-ER_PK_INDEX_CANT_BE_IGNORED = 4174
-ER_BINLOG_UNSAFE_SKIP_LOCKED = 4175
-ER_JSON_TABLE_ERROR_ON_FIELD = 4176
-ER_JSON_TABLE_ALIAS_REQUIRED = 4177
-ER_JSON_TABLE_SCALAR_EXPECTED = 4178
-ER_JSON_TABLE_MULTIPLE_MATCHES = 4179
-ER_WITH_TIES_NEEDS_ORDER = 4180
-ER_REMOVED_ORPHAN_TRIGGER = 4181
-ER_STORAGE_ENGINE_DISABLED = 4182
-WARN_SFORMAT_ERROR = 4183
-ER_PARTITION_CONVERT_SUBPARTITIONED = 4184
-ER_PROVIDER_NOT_LOADED = 4185
-ER_JSON_HISTOGRAM_PARSE_FAILED = 4186
-ER_SF_OUT_INOUT_ARG_NOT_ALLOWED = 4187
-ER_INCONSISTENT_SLAVE_TEMP_TABLE = 4188
-CR_UNKNOWN_ERROR = 2000
-CR_SOCKET_CREATE_ERROR = 2001
-CR_CONNECTION_ERROR = 2002
-CR_CONN_HOST_ERROR = 2003
-CR_IPSOCK_ERROR = 2004
-CR_UNKNOWN_HOST = 2005
-CR_SERVER_GONE_ERROR = 2006
-CR_VERSION_ERROR = 2007
-CR_OUT_OF_MEMORY = 2008
-CR_WRONG_HOST_INFO = 2009
-CR_LOCALHOST_CONNECTION = 2010
-CR_TCP_CONNECTION = 2011
-CR_SERVER_HANDSHAKE_ERR = 2012
-CR_SERVER_LOST = 2013
-CR_COMMANDS_OUT_OF_SYNC = 2014
-CR_NAMEDPIPE_CONNECTION = 2015
-CR_NAMEDPIPEWAIT_ERROR = 2016
-CR_NAMEDPIPEOPEN_ERROR = 2017
-CR_NAMEDPIPESETSTATE_ERROR = 2018
-CR_CANT_READ_CHARSET = 2019
-CR_NET_PACKET_TOO_LARGE = 2020
-CR_SSL_CONNECTION_ERROR = 2026
-CR_MALFORMED_PACKET = 2027
-CR_NO_PREPARE_STMT = 2030
-CR_PARAMS_NOT_BOUND = 2031
-CR_INVALID_PARAMETER_NO = 2034
-CR_INVALID_BUFFER_USE = 2035
-CR_UNSUPPORTED_PARAM_TYPE = 2036
-CR_SHARED_MEMORY_CONNECTION = 2037
-CR_SHARED_MEMORY_CONNECT_ERROR = 2038
-CR_CONN_UNKNOWN_PROTOCOL = 2047
-CR_SECURE_AUTH = 2049
-CR_NO_DATA = 2051
-CR_NO_STMT_METADATA = 2052
-CR_NOT_IMPLEMENTED = 2054
-CR_SERVER_LOST_EXTENDED = 2055
-CR_STMT_CLOSED = 2056
-CR_NEW_STMT_METADATA = 2057
-CR_ALREADY_CONNECTED = 2058
-CR_AUTH_PLUGIN_CANNOT_LOAD = 2059
-CR_DUPLICATE_CONNECTION_ATTR = 2060
-CR_AUTH_PLUGIN_ERR = 2061
-CR_EVENT_CREATE_FAILED = 5000
-CR_BIND_ADDR_FAILED = 5001
-CR_ASYNC_NOT_SUPPORTED = 5002
-CR_FUNCTION_NOT_SUPPORTED = 5003
-CR_FILE_NOT_FOUND = 5004
-CR_FILE_READ = 5005
-CR_BULK_WITHOUT_PARAMETERS = 5006
-CR_INVALID_STMT = 5007
-CR_VERSION_MISMATCH = 5008
-CR_INVALID_PARAMETER = 5009
-CR_PLUGIN_NOT_ALLOWED = 5010
-CR_CONNSTR_PARSE_ERROR = 5011
-CR_ERR_LOAD_PLUGIN = 5012
+# Autogenerated file. Please do not edit!
+
+
+ER_ERROR_FIRST = 1000
+ER_HASHCHK = 1000
+ER_NISAMCHK = 1001
+ER_NO = 1002
+ER_YES = 1003
+ER_CANT_CREATE_FILE = 1004
+ER_CANT_CREATE_TABLE = 1005
+ER_CANT_CREATE_DB = 1006
+ER_DB_CREATE_EXISTS = 1007
+ER_DB_DROP_EXISTS = 1008
+ER_DB_DROP_DELETE = 1009
+ER_DB_DROP_RMDIR = 1010
+ER_CANT_DELETE_FILE = 1011
+ER_CANT_FIND_SYSTEM_REC = 1012
+ER_CANT_GET_STAT = 1013
+ER_CANT_GET_WD = 1014
+ER_CANT_LOCK = 1015
+ER_CANT_OPEN_FILE = 1016
+ER_FILE_NOT_FOUND = 1017
+ER_CANT_READ_DIR = 1018
+ER_CANT_SET_WD = 1019
+ER_CHECKREAD = 1020
+ER_DISK_FULL = 1021
+ER_DUP_KEY = 1022
+ER_ERROR_ON_CLOSE = 1023
+ER_ERROR_ON_READ = 1024
+ER_ERROR_ON_RENAME = 1025
+ER_ERROR_ON_WRITE = 1026
+ER_FILE_USED = 1027
+ER_FILSORT_ABORT = 1028
+ER_FORM_NOT_FOUND = 1029
+ER_GET_ERRNO = 1030
+ER_ILLEGAL_HA = 1031
+ER_KEY_NOT_FOUND = 1032
+ER_NOT_FORM_FILE = 1033
+ER_NOT_KEYFILE = 1034
+ER_OLD_KEYFILE = 1035
+ER_OPEN_AS_READONLY = 1036
+ER_OUTOFMEMORY = 1037
+ER_OUT_OF_SORTMEMORY = 1038
+ER_UNEXPECTED_EOF = 1039
+ER_CON_COUNT_ERROR = 1040
+ER_OUT_OF_RESOURCES = 1041
+ER_BAD_HOST_ERROR = 1042
+ER_HANDSHAKE_ERROR = 1043
+ER_DBACCESS_DENIED_ERROR = 1044
+ER_ACCESS_DENIED_ERROR = 1045
+ER_NO_DB_ERROR = 1046
+ER_UNKNOWN_COM_ERROR = 1047
+ER_BAD_NULL_ERROR = 1048
+ER_BAD_DB_ERROR = 1049
+ER_TABLE_EXISTS_ERROR = 1050
+ER_BAD_TABLE_ERROR = 1051
+ER_NON_UNIQ_ERROR = 1052
+ER_SERVER_SHUTDOWN = 1053
+ER_BAD_FIELD_ERROR = 1054
+ER_WRONG_FIELD_WITH_GROUP = 1055
+ER_WRONG_GROUP_FIELD = 1056
+ER_WRONG_SUM_SELECT = 1057
+ER_WRONG_VALUE_COUNT = 1058
+ER_TOO_LONG_IDENT = 1059
+ER_DUP_FIELDNAME = 1060
+ER_DUP_KEYNAME = 1061
+ER_DUP_ENTRY = 1062
+ER_WRONG_FIELD_SPEC = 1063
+ER_PARSE_ERROR = 1064
+ER_EMPTY_QUERY = 1065
+ER_NONUNIQ_TABLE = 1066
+ER_INVALID_DEFAULT = 1067
+ER_MULTIPLE_PRI_KEY = 1068
+ER_TOO_MANY_KEYS = 1069
+ER_TOO_MANY_KEY_PARTS = 1070
+ER_TOO_LONG_KEY = 1071
+ER_KEY_COLUMN_DOES_NOT_EXIST = 1072
+ER_BLOB_USED_AS_KEY = 1073
+ER_TOO_BIG_FIELDLENGTH = 1074
+ER_WRONG_AUTO_KEY = 1075
+ER_BINLOG_CANT_DELETE_GTID_DOMAIN = 1076
+ER_NORMAL_SHUTDOWN = 1077
+ER_GOT_SIGNAL = 1078
+ER_SHUTDOWN_COMPLETE = 1079
+ER_FORCING_CLOSE = 1080
+ER_IPSOCK_ERROR = 1081
+ER_NO_SUCH_INDEX = 1082
+ER_WRONG_FIELD_TERMINATORS = 1083
+ER_BLOBS_AND_NO_TERMINATED = 1084
+ER_TEXTFILE_NOT_READABLE = 1085
+ER_FILE_EXISTS_ERROR = 1086
+ER_LOAD_INFO = 1087
+ER_ALTER_INFO = 1088
+ER_WRONG_SUB_KEY = 1089
+ER_CANT_REMOVE_ALL_FIELDS = 1090
+ER_CANT_DROP_FIELD_OR_KEY = 1091
+ER_INSERT_INFO = 1092
+ER_UPDATE_TABLE_USED = 1093
+ER_NO_SUCH_THREAD = 1094
+ER_KILL_DENIED_ERROR = 1095
+ER_NO_TABLES_USED = 1096
+ER_TOO_BIG_SET = 1097
+ER_NO_UNIQUE_LOGFILE = 1098
+ER_TABLE_NOT_LOCKED_FOR_WRITE = 1099
+ER_TABLE_NOT_LOCKED = 1100
+ER_WRONG_DB_NAME = 1102
+ER_WRONG_TABLE_NAME = 1103
+ER_TOO_BIG_SELECT = 1104
+ER_UNKNOWN_ERROR = 1105
+ER_UNKNOWN_PROCEDURE = 1106
+ER_WRONG_PARAMCOUNT_TO_PROCEDURE = 1107
+ER_WRONG_PARAMETERS_TO_PROCEDURE = 1108
+ER_UNKNOWN_TABLE = 1109
+ER_FIELD_SPECIFIED_TWICE = 1110
+ER_INVALID_GROUP_FUNC_USE = 1111
+ER_UNSUPPORTED_EXTENSION = 1112
+ER_TABLE_MUST_HAVE_COLUMNS = 1113
+ER_RECORD_FILE_FULL = 1114
+ER_UNKNOWN_CHARACTER_SET = 1115
+ER_TOO_MANY_TABLES = 1116
+ER_TOO_MANY_FIELDS = 1117
+ER_TOO_BIG_ROWSIZE = 1118
+ER_STACK_OVERRUN = 1119
+ER_WRONG_OUTER_JOIN = 1120
+ER_NULL_COLUMN_IN_INDEX = 1121
+ER_CANT_FIND_UDF = 1122
+ER_CANT_INITIALIZE_UDF = 1123
+ER_UDF_NO_PATHS = 1124
+ER_UDF_EXISTS = 1125
+ER_CANT_OPEN_LIBRARY = 1126
+ER_CANT_FIND_DL_ENTRY = 1127
+ER_FUNCTION_NOT_DEFINED = 1128
+ER_HOST_IS_BLOCKED = 1129
+ER_HOST_NOT_PRIVILEGED = 1130
+ER_PASSWORD_ANONYMOUS_USER = 1131
+ER_PASSWORD_NOT_ALLOWED = 1132
+ER_PASSWORD_NO_MATCH = 1133
+ER_UPDATE_INFO = 1134
+ER_CANT_CREATE_THREAD = 1135
+ER_WRONG_VALUE_COUNT_ON_ROW = 1136
+ER_CANT_REOPEN_TABLE = 1137
+ER_INVALID_USE_OF_NULL = 1138
+ER_REGEXP_ERROR = 1139
+ER_MIX_OF_GROUP_FUNC_AND_FIELDS = 1140
+ER_NONEXISTING_GRANT = 1141
+ER_TABLEACCESS_DENIED_ERROR = 1142
+ER_COLUMNACCESS_DENIED_ERROR = 1143
+ER_ILLEGAL_GRANT_FOR_TABLE = 1144
+ER_GRANT_WRONG_HOST_OR_USER = 1145
+ER_NO_SUCH_TABLE = 1146
+ER_NONEXISTING_TABLE_GRANT = 1147
+ER_NOT_ALLOWED_COMMAND = 1148
+ER_SYNTAX_ERROR = 1149
+ER_DELAYED_CANT_CHANGE_LOCK = 1150
+ER_TOO_MANY_DELAYED_THREADS = 1151
+ER_ABORTING_CONNECTION = 1152
+ER_NET_PACKET_TOO_LARGE = 1153
+ER_NET_READ_ERROR_FROM_PIPE = 1154
+ER_NET_FCNTL_ERROR = 1155
+ER_NET_PACKETS_OUT_OF_ORDER = 1156
+ER_NET_UNCOMPRESS_ERROR = 1157
+ER_NET_READ_ERROR = 1158
+ER_NET_READ_INTERRUPTED = 1159
+ER_NET_ERROR_ON_WRITE = 1160
+ER_NET_WRITE_INTERRUPTED = 1161
+ER_TOO_LONG_STRING = 1162
+ER_TABLE_CANT_HANDLE_BLOB = 1163
+ER_TABLE_CANT_HANDLE_AUTO_INCREMENT = 1164
+ER_DELAYED_INSERT_TABLE_LOCKED = 1165
+ER_WRONG_COLUMN_NAME = 1166
+ER_WRONG_KEY_COLUMN = 1167
+ER_WRONG_MRG_TABLE = 1168
+ER_DUP_UNIQUE = 1169
+ER_BLOB_KEY_WITHOUT_LENGTH = 1170
+ER_PRIMARY_CANT_HAVE_NULL = 1171
+ER_TOO_MANY_ROWS = 1172
+ER_REQUIRES_PRIMARY_KEY = 1173
+ER_NO_RAID_COMPILED = 1174
+ER_UPDATE_WITHOUT_KEY_IN_SAFE_MODE = 1175
+ER_KEY_DOES_NOT_EXISTS = 1176
+ER_CHECK_NO_SUCH_TABLE = 1177
+ER_CHECK_NOT_IMPLEMENTED = 1178
+ER_CANT_DO_THIS_DURING_AN_TRANSACTION = 1179
+ER_ERROR_DURING_COMMIT = 1180
+ER_ERROR_DURING_ROLLBACK = 1181
+ER_ERROR_DURING_FLUSH_LOGS = 1182
+ER_ERROR_DURING_CHECKPOINT = 1183
+ER_NEW_ABORTING_CONNECTION = 1184
+ER_FLUSH_MASTER_BINLOG_CLOSED = 1186
+ER_INDEX_REBUILD = 1187
+ER_MASTER = 1188
+ER_MASTER_NET_READ = 1189
+ER_MASTER_NET_WRITE = 1190
+ER_FT_MATCHING_KEY_NOT_FOUND = 1191
+ER_LOCK_OR_ACTIVE_TRANSACTION = 1192
+ER_UNKNOWN_SYSTEM_VARIABLE = 1193
+ER_CRASHED_ON_USAGE = 1194
+ER_CRASHED_ON_REPAIR = 1195
+ER_WARNING_NOT_COMPLETE_ROLLBACK = 1196
+ER_TRANS_CACHE_FULL = 1197
+ER_SLAVE_MUST_STOP = 1198
+ER_SLAVE_NOT_RUNNING = 1199
+ER_BAD_SLAVE = 1200
+ER_MASTER_INFO = 1201
+ER_SLAVE_THREAD = 1202
+ER_TOO_MANY_USER_CONNECTIONS = 1203
+ER_SET_CONSTANTS_ONLY = 1204
+ER_LOCK_WAIT_TIMEOUT = 1205
+ER_LOCK_TABLE_FULL = 1206
+ER_READ_ONLY_TRANSACTION = 1207
+ER_DROP_DB_WITH_READ_LOCK = 1208
+ER_CREATE_DB_WITH_READ_LOCK = 1209
+ER_WRONG_ARGUMENTS = 1210
+ER_NO_PERMISSION_TO_CREATE_USER = 1211
+ER_UNION_TABLES_IN_DIFFERENT_DIR = 1212
+ER_LOCK_DEADLOCK = 1213
+ER_TABLE_CANT_HANDLE_FT = 1214
+ER_CANNOT_ADD_FOREIGN = 1215
+ER_NO_REFERENCED_ROW = 1216
+ER_ROW_IS_REFERENCED = 1217
+ER_CONNECT_TO_MASTER = 1218
+ER_QUERY_ON_MASTER = 1219
+ER_ERROR_WHEN_EXECUTING_COMMAND = 1220
+ER_WRONG_USAGE = 1221
+ER_WRONG_NUMBER_OF_COLUMNS_IN_SELECT = 1222
+ER_CANT_UPDATE_WITH_READLOCK = 1223
+ER_MIXING_NOT_ALLOWED = 1224
+ER_DUP_ARGUMENT = 1225
+ER_USER_LIMIT_REACHED = 1226
+ER_SPECIFIC_ACCESS_DENIED_ERROR = 1227
+ER_LOCAL_VARIABLE = 1228
+ER_GLOBAL_VARIABLE = 1229
+ER_NO_DEFAULT = 1230
+ER_WRONG_VALUE_FOR_VAR = 1231
+ER_WRONG_TYPE_FOR_VAR = 1232
+ER_VAR_CANT_BE_READ = 1233
+ER_CANT_USE_OPTION_HERE = 1234
+ER_NOT_SUPPORTED_YET = 1235
+ER_MASTER_FATAL_ERROR_READING_BINLOG = 1236
+ER_SLAVE_IGNORED_TABLE = 1237
+ER_INCORRECT_GLOBAL_LOCAL_VAR = 1238
+ER_WRONG_FK_DEF = 1239
+ER_KEY_REF_DO_NOT_MATCH_TABLE_REF = 1240
+ER_OPERAND_COLUMNS = 1241
+ER_SUBQUERY_NO_1_ROW = 1242
+ER_UNKNOWN_STMT_HANDLER = 1243
+ER_CORRUPT_HELP_DB = 1244
+ER_CYCLIC_REFERENCE = 1245
+ER_AUTO_CONVERT = 1246
+ER_ILLEGAL_REFERENCE = 1247
+ER_DERIVED_MUST_HAVE_ALIAS = 1248
+ER_SELECT_REDUCED = 1249
+ER_TABLENAME_NOT_ALLOWED_HERE = 1250
+ER_NOT_SUPPORTED_AUTH_MODE = 1251
+ER_SPATIAL_CANT_HAVE_NULL = 1252
+ER_COLLATION_CHARSET_MISMATCH = 1253
+ER_SLAVE_WAS_RUNNING = 1254
+ER_SLAVE_WAS_NOT_RUNNING = 1255
+ER_TOO_BIG_FOR_UNCOMPRESS = 1256
+ER_ZLIB_Z_MEM_ERROR = 1257
+ER_ZLIB_Z_BUF_ERROR = 1258
+ER_ZLIB_Z_DATA_ERROR = 1259
+ER_CUT_VALUE_GROUP_CONCAT = 1260
+ER_WARN_TOO_FEW_RECORDS = 1261
+ER_WARN_TOO_MANY_RECORDS = 1262
+ER_WARN_NULL_TO_NOTNULL = 1263
+ER_WARN_DATA_OUT_OF_RANGE = 1264
+WARN_DATA_TRUNCATED = 1265
+ER_WARN_USING_OTHER_HANDLER = 1266
+ER_CANT_AGGREGATE_2COLLATIONS = 1267
+ER_DROP_USER = 1268
+ER_REVOKE_GRANTS = 1269
+ER_CANT_AGGREGATE_3COLLATIONS = 1270
+ER_CANT_AGGREGATE_NCOLLATIONS = 1271
+ER_VARIABLE_IS_NOT_STRUCT = 1272
+ER_UNKNOWN_COLLATION = 1273
+ER_SLAVE_IGNORED_SSL_PARAMS = 1274
+ER_SERVER_IS_IN_SECURE_AUTH_MODE = 1275
+ER_WARN_FIELD_RESOLVED = 1276
+ER_BAD_SLAVE_UNTIL_COND = 1277
+ER_MISSING_SKIP_SLAVE = 1278
+ER_UNTIL_COND_IGNORED = 1279
+ER_WRONG_NAME_FOR_INDEX = 1280
+ER_WRONG_NAME_FOR_CATALOG = 1281
+ER_WARN_QC_RESIZE = 1282
+ER_BAD_FT_COLUMN = 1283
+ER_UNKNOWN_KEY_CACHE = 1284
+ER_WARN_HOSTNAME_WONT_WORK = 1285
+ER_UNKNOWN_STORAGE_ENGINE = 1286
+ER_WARN_DEPRECATED_SYNTAX = 1287
+ER_NON_UPDATABLE_TABLE = 1288
+ER_FEATURE_DISABLED = 1289
+ER_OPTION_PREVENTS_STATEMENT = 1290
+ER_DUPLICATED_VALUE_IN_TYPE = 1291
+ER_TRUNCATED_WRONG_VALUE = 1292
+ER_TOO_MUCH_AUTO_TIMESTAMP_COLS = 1293
+ER_INVALID_ON_UPDATE = 1294
+ER_UNSUPPORTED_PS = 1295
+ER_GET_ERRMSG = 1296
+ER_GET_TEMPORARY_ERRMSG = 1297
+ER_UNKNOWN_TIME_ZONE = 1298
+ER_WARN_INVALID_TIMESTAMP = 1299
+ER_INVALID_CHARACTER_STRING = 1300
+ER_WARN_ALLOWED_PACKET_OVERFLOWED = 1301
+ER_CONFLICTING_DECLARATIONS = 1302
+ER_SP_NO_RECURSIVE_CREATE = 1303
+ER_SP_ALREADY_EXISTS = 1304
+ER_SP_DOES_NOT_EXIST = 1305
+ER_SP_DROP_FAILED = 1306
+ER_SP_STORE_FAILED = 1307
+ER_SP_LILABEL_MISMATCH = 1308
+ER_SP_LABEL_REDEFINE = 1309
+ER_SP_LABEL_MISMATCH = 1310
+ER_SP_UNINIT_VAR = 1311
+ER_SP_BADSELECT = 1312
+ER_SP_BADRETURN = 1313
+ER_SP_BADSTATEMENT = 1314
+ER_UPDATE_LOG_DEPRECATED_IGNORED = 1315
+ER_UPDATE_LOG_DEPRECATED_TRANSLATED = 1316
+ER_QUERY_INTERRUPTED = 1317
+ER_SP_WRONG_NO_OF_ARGS = 1318
+ER_SP_COND_MISMATCH = 1319
+ER_SP_NORETURN = 1320
+ER_SP_NORETURNEND = 1321
+ER_SP_BAD_CURSOR_QUERY = 1322
+ER_SP_BAD_CURSOR_SELECT = 1323
+ER_SP_CURSOR_MISMATCH = 1324
+ER_SP_CURSOR_ALREADY_OPEN = 1325
+ER_SP_CURSOR_NOT_OPEN = 1326
+ER_SP_UNDECLARED_VAR = 1327
+ER_SP_WRONG_NO_OF_FETCH_ARGS = 1328
+ER_SP_FETCH_NO_DATA = 1329
+ER_SP_DUP_PARAM = 1330
+ER_SP_DUP_VAR = 1331
+ER_SP_DUP_COND = 1332
+ER_SP_DUP_CURS = 1333
+ER_SP_CANT_ALTER = 1334
+ER_SP_SUBSELECT_NYI = 1335
+ER_STMT_NOT_ALLOWED_IN_SF_OR_TRG = 1336
+ER_SP_VARCOND_AFTER_CURSHNDLR = 1337
+ER_SP_CURSOR_AFTER_HANDLER = 1338
+ER_SP_CASE_NOT_FOUND = 1339
+ER_FPARSER_TOO_BIG_FILE = 1340
+ER_FPARSER_BAD_HEADER = 1341
+ER_FPARSER_EOF_IN_COMMENT = 1342
+ER_FPARSER_ERROR_IN_PARAMETER = 1343
+ER_FPARSER_EOF_IN_UNKNOWN_PARAMETER = 1344
+ER_VIEW_NO_EXPLAIN = 1345
+ER_FRM_UNKNOWN_TYPE = 1346
+ER_WRONG_OBJECT = 1347
+ER_NONUPDATEABLE_COLUMN = 1348
+ER_VIEW_SELECT_DERIVED = 1349
+ER_VIEW_SELECT_CLAUSE = 1350
+ER_VIEW_SELECT_VARIABLE = 1351
+ER_VIEW_SELECT_TMPTABLE = 1352
+ER_VIEW_WRONG_LIST = 1353
+ER_WARN_VIEW_MERGE = 1354
+ER_WARN_VIEW_WITHOUT_KEY = 1355
+ER_VIEW_INVALID = 1356
+ER_SP_NO_DROP_SP = 1357
+ER_SP_GOTO_IN_HNDLR = 1358
+ER_TRG_ALREADY_EXISTS = 1359
+ER_TRG_DOES_NOT_EXIST = 1360
+ER_TRG_ON_VIEW_OR_TEMP_TABLE = 1361
+ER_TRG_CANT_CHANGE_ROW = 1362
+ER_TRG_NO_SUCH_ROW_IN_TRG = 1363
+ER_NO_DEFAULT_FOR_FIELD = 1364
+ER_DIVISION_BY_ZERO = 1365
+ER_TRUNCATED_WRONG_VALUE_FOR_FIELD = 1366
+ER_ILLEGAL_VALUE_FOR_TYPE = 1367
+ER_VIEW_NONUPD_CHECK = 1368
+ER_VIEW_CHECK_FAILED = 1369
+ER_PROCACCESS_DENIED_ERROR = 1370
+ER_RELAY_LOG_FAIL = 1371
+ER_PASSWD_LENGTH = 1372
+ER_UNKNOWN_TARGET_BINLOG = 1373
+ER_IO_ERR_LOG_INDEX_READ = 1374
+ER_BINLOG_PURGE_PROHIBITED = 1375
+ER_FSEEK_FAIL = 1376
+ER_BINLOG_PURGE_FATAL_ERR = 1377
+ER_LOG_IN_USE = 1378
+ER_LOG_PURGE_UNKNOWN_ERR = 1379
+ER_RELAY_LOG_INIT = 1380
+ER_NO_BINARY_LOGGING = 1381
+ER_RESERVED_SYNTAX = 1382
+ER_WSAS_FAILED = 1383
+ER_DIFF_GROUPS_PROC = 1384
+ER_NO_GROUP_FOR_PROC = 1385
+ER_ORDER_WITH_PROC = 1386
+ER_LOGGING_PROHIBIT_CHANGING_OF = 1387
+ER_NO_FILE_MAPPING = 1388
+ER_WRONG_MAGIC = 1389
+ER_PS_MANY_PARAM = 1390
+ER_KEY_PART_0 = 1391
+ER_VIEW_CHECKSUM = 1392
+ER_VIEW_MULTIUPDATE = 1393
+ER_VIEW_NO_INSERT_FIELD_LIST = 1394
+ER_VIEW_DELETE_MERGE_VIEW = 1395
+ER_CANNOT_USER = 1396
+ER_XAER_NOTA = 1397
+ER_XAER_INVAL = 1398
+ER_XAER_RMFAIL = 1399
+ER_XAER_OUTSIDE = 1400
+ER_XAER_RMERR = 1401
+ER_XA_RBROLLBACK = 1402
+ER_NONEXISTING_PROC_GRANT = 1403
+ER_PROC_AUTO_GRANT_FAIL = 1404
+ER_PROC_AUTO_REVOKE_FAIL = 1405
+ER_DATA_TOO_LONG = 1406
+ER_SP_BAD_SQLSTATE = 1407
+ER_STARTUP = 1408
+ER_LOAD_FROM_FIXED_SIZE_ROWS_TO_VAR = 1409
+ER_CANT_CREATE_USER_WITH_GRANT = 1410
+ER_WRONG_VALUE_FOR_TYPE = 1411
+ER_TABLE_DEF_CHANGED = 1412
+ER_SP_DUP_HANDLER = 1413
+ER_SP_NOT_VAR_ARG = 1414
+ER_SP_NO_RETSET = 1415
+ER_CANT_CREATE_GEOMETRY_OBJECT = 1416
+ER_FAILED_ROUTINE_BREAK_BINLOG = 1417
+ER_BINLOG_UNSAFE_ROUTINE = 1418
+ER_BINLOG_CREATE_ROUTINE_NEED_SUPER = 1419
+ER_EXEC_STMT_WITH_OPEN_CURSOR = 1420
+ER_STMT_HAS_NO_OPEN_CURSOR = 1421
+ER_COMMIT_NOT_ALLOWED_IN_SF_OR_TRG = 1422
+ER_NO_DEFAULT_FOR_VIEW_FIELD = 1423
+ER_SP_NO_RECURSION = 1424
+ER_TOO_BIG_SCALE = 1425
+ER_TOO_BIG_PRECISION = 1426
+ER_M_BIGGER_THAN_D = 1427
+ER_WRONG_LOCK_OF_SYSTEM_TABLE = 1428
+ER_CONNECT_TO_FOREIGN_DATA_SOURCE = 1429
+ER_QUERY_ON_FOREIGN_DATA_SOURCE = 1430
+ER_FOREIGN_DATA_SOURCE_DOESNT_EXIST = 1431
+ER_FOREIGN_DATA_STRING_INVALID_CANT_CREATE = 1432
+ER_FOREIGN_DATA_STRING_INVALID = 1433
+ER_CANT_CREATE_FEDERATED_TABLE = 1434
+ER_TRG_IN_WRONG_SCHEMA = 1435
+ER_STACK_OVERRUN_NEED_MORE = 1436
+ER_TOO_LONG_BODY = 1437
+ER_WARN_CANT_DROP_DEFAULT_KEYCACHE = 1438
+ER_TOO_BIG_DISPLAYWIDTH = 1439
+ER_XAER_DUPID = 1440
+ER_DATETIME_FUNCTION_OVERFLOW = 1441
+ER_CANT_UPDATE_USED_TABLE_IN_SF_OR_TRG = 1442
+ER_VIEW_PREVENT_UPDATE = 1443
+ER_PS_NO_RECURSION = 1444
+ER_SP_CANT_SET_AUTOCOMMIT = 1445
+ER_MALFORMED_DEFINER = 1446
+ER_VIEW_FRM_NO_USER = 1447
+ER_VIEW_OTHER_USER = 1448
+ER_NO_SUCH_USER = 1449
+ER_FORBID_SCHEMA_CHANGE = 1450
+ER_ROW_IS_REFERENCED_2 = 1451
+ER_NO_REFERENCED_ROW_2 = 1452
+ER_SP_BAD_VAR_SHADOW = 1453
+ER_TRG_NO_DEFINER = 1454
+ER_OLD_FILE_FORMAT = 1455
+ER_SP_RECURSION_LIMIT = 1456
+ER_SP_PROC_TABLE_CORRUPT = 1457
+ER_SP_WRONG_NAME = 1458
+ER_TABLE_NEEDS_UPGRADE = 1459
+ER_SP_NO_AGGREGATE = 1460
+ER_MAX_PREPARED_STMT_COUNT_REACHED = 1461
+ER_VIEW_RECURSIVE = 1462
+ER_NON_GROUPING_FIELD_USED = 1463
+ER_TABLE_CANT_HANDLE_SPKEYS = 1464
+ER_NO_TRIGGERS_ON_SYSTEM_SCHEMA = 1465
+ER_REMOVED_SPACES = 1466
+ER_AUTOINC_READ_FAILED = 1467
+ER_USERNAME = 1468
+ER_HOSTNAME = 1469
+ER_WRONG_STRING_LENGTH = 1470
+ER_NON_INSERTABLE_TABLE = 1471
+ER_ADMIN_WRONG_MRG_TABLE = 1472
+ER_TOO_HIGH_LEVEL_OF_NESTING_FOR_SELECT = 1473
+ER_NAME_BECOMES_EMPTY = 1474
+ER_AMBIGUOUS_FIELD_TERM = 1475
+ER_FOREIGN_SERVER_EXISTS = 1476
+ER_FOREIGN_SERVER_DOESNT_EXIST = 1477
+ER_ILLEGAL_HA_CREATE_OPTION = 1478
+ER_PARTITION_REQUIRES_VALUES_ERROR = 1479
+ER_PARTITION_WRONG_VALUES_ERROR = 1480
+ER_PARTITION_MAXVALUE_ERROR = 1481
+ER_PARTITION_SUBPARTITION_ERROR = 1482
+ER_PARTITION_SUBPART_MIX_ERROR = 1483
+ER_PARTITION_WRONG_NO_PART_ERROR = 1484
+ER_PARTITION_WRONG_NO_SUBPART_ERROR = 1485
+ER_WRONG_EXPR_IN_PARTITION_FUNC_ERROR = 1486
+ER_NOT_CONSTANT_EXPRESSION = 1487
+ER_FIELD_NOT_FOUND_PART_ERROR = 1488
+ER_LIST_OF_FIELDS_ONLY_IN_HASH_ERROR = 1489
+ER_INCONSISTENT_PARTITION_INFO_ERROR = 1490
+ER_PARTITION_FUNC_NOT_ALLOWED_ERROR = 1491
+ER_PARTITIONS_MUST_BE_DEFINED_ERROR = 1492
+ER_RANGE_NOT_INCREASING_ERROR = 1493
+ER_INCONSISTENT_TYPE_OF_FUNCTIONS_ERROR = 1494
+ER_MULTIPLE_DEF_CONST_IN_LIST_PART_ERROR = 1495
+ER_PARTITION_ENTRY_ERROR = 1496
+ER_MIX_HANDLER_ERROR = 1497
+ER_PARTITION_NOT_DEFINED_ERROR = 1498
+ER_TOO_MANY_PARTITIONS_ERROR = 1499
+ER_SUBPARTITION_ERROR = 1500
+ER_CANT_CREATE_HANDLER_FILE = 1501
+ER_BLOB_FIELD_IN_PART_FUNC_ERROR = 1502
+ER_UNIQUE_KEY_NEED_ALL_FIELDS_IN_PF = 1503
+ER_NO_PARTS_ERROR = 1504
+ER_PARTITION_MGMT_ON_NONPARTITIONED = 1505
+ER_FEATURE_NOT_SUPPORTED_WITH_PARTITIONING = 1506
+ER_PARTITION_DOES_NOT_EXIST = 1507
+ER_DROP_LAST_PARTITION = 1508
+ER_COALESCE_ONLY_ON_HASH_PARTITION = 1509
+ER_REORG_HASH_ONLY_ON_SAME_NO = 1510
+ER_REORG_NO_PARAM_ERROR = 1511
+ER_ONLY_ON_RANGE_LIST_PARTITION = 1512
+ER_ADD_PARTITION_SUBPART_ERROR = 1513
+ER_ADD_PARTITION_NO_NEW_PARTITION = 1514
+ER_COALESCE_PARTITION_NO_PARTITION = 1515
+ER_REORG_PARTITION_NOT_EXIST = 1516
+ER_SAME_NAME_PARTITION = 1517
+ER_NO_BINLOG_ERROR = 1518
+ER_CONSECUTIVE_REORG_PARTITIONS = 1519
+ER_REORG_OUTSIDE_RANGE = 1520
+ER_PARTITION_FUNCTION_FAILURE = 1521
+ER_PART_STATE_ERROR = 1522
+ER_LIMITED_PART_RANGE = 1523
+ER_PLUGIN_IS_NOT_LOADED = 1524
+ER_WRONG_VALUE = 1525
+ER_NO_PARTITION_FOR_GIVEN_VALUE = 1526
+ER_FILEGROUP_OPTION_ONLY_ONCE = 1527
+ER_CREATE_FILEGROUP_FAILED = 1528
+ER_DROP_FILEGROUP_FAILED = 1529
+ER_TABLESPACE_AUTO_EXTEND_ERROR = 1530
+ER_WRONG_SIZE_NUMBER = 1531
+ER_SIZE_OVERFLOW_ERROR = 1532
+ER_ALTER_FILEGROUP_FAILED = 1533
+ER_BINLOG_ROW_LOGGING_FAILED = 1534
+ER_BINLOG_ROW_WRONG_TABLE_DEF = 1535
+ER_BINLOG_ROW_RBR_TO_SBR = 1536
+ER_EVENT_ALREADY_EXISTS = 1537
+ER_EVENT_STORE_FAILED = 1538
+ER_EVENT_DOES_NOT_EXIST = 1539
+ER_EVENT_CANT_ALTER = 1540
+ER_EVENT_DROP_FAILED = 1541
+ER_EVENT_INTERVAL_NOT_POSITIVE_OR_TOO_BIG = 1542
+ER_EVENT_ENDS_BEFORE_STARTS = 1543
+ER_EVENT_EXEC_TIME_IN_THE_PAST = 1544
+ER_EVENT_OPEN_TABLE_FAILED = 1545
+ER_EVENT_NEITHER_M_EXPR_NOR_M_AT = 1546
+ER_EVENT_CANNOT_DELETE = 1549
+ER_EVENT_COMPILE_ERROR = 1550
+ER_EVENT_SAME_NAME = 1551
+ER_EVENT_DATA_TOO_LONG = 1552
+ER_DROP_INDEX_FK = 1553
+ER_WARN_DEPRECATED_SYNTAX_WITH_VER = 1554
+ER_CANT_WRITE_LOCK_LOG_TABLE = 1555
+ER_CANT_LOCK_LOG_TABLE = 1556
+ER_COL_COUNT_DOESNT_MATCH_PLEASE_UPDATE = 1558
+ER_TEMP_TABLE_PREVENTS_SWITCH_OUT_OF_RBR = 1559
+ER_STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1560
+ER_PARTITION_NO_TEMPORARY = 1562
+ER_PARTITION_CONST_DOMAIN_ERROR = 1563
+ER_PARTITION_FUNCTION_IS_NOT_ALLOWED = 1564
+ER_DDL_LOG_ERROR = 1565
+ER_NULL_IN_VALUES_LESS_THAN = 1566
+ER_WRONG_PARTITION_NAME = 1567
+ER_CANT_CHANGE_TX_CHARACTERISTICS = 1568
+ER_DUP_ENTRY_AUTOINCREMENT_CASE = 1569
+ER_EVENT_MODIFY_QUEUE_ERROR = 1570
+ER_EVENT_SET_VAR_ERROR = 1571
+ER_PARTITION_MERGE_ERROR = 1572
+ER_CANT_ACTIVATE_LOG = 1573
+ER_RBR_NOT_AVAILABLE = 1574
+ER_BASE64_DECODE_ERROR = 1575
+ER_EVENT_RECURSION_FORBIDDEN = 1576
+ER_EVENTS_DB_ERROR = 1577
+ER_ONLY_INTEGERS_ALLOWED = 1578
+ER_UNSUPORTED_LOG_ENGINE = 1579
+ER_BAD_LOG_STATEMENT = 1580
+ER_CANT_RENAME_LOG_TABLE = 1581
+ER_WRONG_PARAMCOUNT_TO_NATIVE_FCT = 1582
+ER_WRONG_PARAMETERS_TO_NATIVE_FCT = 1583
+ER_WRONG_PARAMETERS_TO_STORED_FCT = 1584
+ER_NATIVE_FCT_NAME_COLLISION = 1585
+ER_DUP_ENTRY_WITH_KEY_NAME = 1586
+ER_BINLOG_PURGE_EMFILE = 1587
+ER_EVENT_CANNOT_CREATE_IN_THE_PAST = 1588
+ER_EVENT_CANNOT_ALTER_IN_THE_PAST = 1589
+ER_SLAVE_INCIDENT = 1590
+ER_NO_PARTITION_FOR_GIVEN_VALUE_SILENT = 1591
+ER_BINLOG_UNSAFE_STATEMENT = 1592
+ER_SLAVE_FATAL_ERROR = 1593
+ER_SLAVE_RELAY_LOG_READ_FAILURE = 1594
+ER_SLAVE_RELAY_LOG_WRITE_FAILURE = 1595
+ER_SLAVE_CREATE_EVENT_FAILURE = 1596
+ER_SLAVE_MASTER_COM_FAILURE = 1597
+ER_BINLOG_LOGGING_IMPOSSIBLE = 1598
+ER_VIEW_NO_CREATION_CTX = 1599
+ER_VIEW_INVALID_CREATION_CTX = 1600
+ER_SR_INVALID_CREATION_CTX = 1601
+ER_TRG_CORRUPTED_FILE = 1602
+ER_TRG_NO_CREATION_CTX = 1603
+ER_TRG_INVALID_CREATION_CTX = 1604
+ER_EVENT_INVALID_CREATION_CTX = 1605
+ER_TRG_CANT_OPEN_TABLE = 1606
+ER_CANT_CREATE_SROUTINE = 1607
+ER_NO_FORMAT_DESCRIPTION_EVENT_BEFORE_BINLOG_STATEMENT = 1609
+ER_SLAVE_CORRUPT_EVENT = 1610
+ER_LOAD_DATA_INVALID_COLUMN = 1611
+ER_LOG_PURGE_NO_FILE = 1612
+ER_XA_RBTIMEOUT = 1613
+ER_XA_RBDEADLOCK = 1614
+ER_NEED_REPREPARE = 1615
+ER_DELAYED_NOT_SUPPORTED = 1616
+WARN_NO_MASTER_INFO = 1617
+WARN_OPTION_IGNORED = 1618
+ER_PLUGIN_DELETE_BUILTIN = 1619
+WARN_PLUGIN_BUSY = 1620
+ER_VARIABLE_IS_READONLY = 1621
+ER_WARN_ENGINE_TRANSACTION_ROLLBACK = 1622
+ER_SLAVE_HEARTBEAT_FAILURE = 1623
+ER_SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE = 1624
+ER_CONFLICT_FN_PARSE_ERROR = 1626
+ER_EXCEPTIONS_WRITE_ERROR = 1627
+ER_TOO_LONG_TABLE_COMMENT = 1628
+ER_TOO_LONG_FIELD_COMMENT = 1629
+ER_FUNC_INEXISTENT_NAME_COLLISION = 1630
+ER_DATABASE_NAME = 1631
+ER_TABLE_NAME = 1632
+ER_PARTITION_NAME = 1633
+ER_SUBPARTITION_NAME = 1634
+ER_TEMPORARY_NAME = 1635
+ER_RENAMED_NAME = 1636
+ER_TOO_MANY_CONCURRENT_TRXS = 1637
+WARN_NON_ASCII_SEPARATOR_NOT_IMPLEMENTED = 1638
+ER_DEBUG_SYNC_TIMEOUT = 1639
+ER_DEBUG_SYNC_HIT_LIMIT = 1640
+ER_DUP_SIGNAL_SET = 1641
+ER_SIGNAL_WARN = 1642
+ER_SIGNAL_NOT_FOUND = 1643
+ER_SIGNAL_EXCEPTION = 1644
+ER_RESIGNAL_WITHOUT_ACTIVE_HANDLER = 1645
+ER_SIGNAL_BAD_CONDITION_TYPE = 1646
+WARN_COND_ITEM_TRUNCATED = 1647
+ER_COND_ITEM_TOO_LONG = 1648
+ER_UNKNOWN_LOCALE = 1649
+ER_SLAVE_IGNORE_SERVER_IDS = 1650
+ER_QUERY_CACHE_DISABLED = 1651
+ER_SAME_NAME_PARTITION_FIELD = 1652
+ER_PARTITION_COLUMN_LIST_ERROR = 1653
+ER_WRONG_TYPE_COLUMN_VALUE_ERROR = 1654
+ER_TOO_MANY_PARTITION_FUNC_FIELDS_ERROR = 1655
+ER_MAXVALUE_IN_VALUES_IN = 1656
+ER_TOO_MANY_VALUES_ERROR = 1657
+ER_ROW_SINGLE_PARTITION_FIELD_ERROR = 1658
+ER_FIELD_TYPE_NOT_ALLOWED_AS_PARTITION_FIELD = 1659
+ER_PARTITION_FIELDS_TOO_LONG = 1660
+ER_BINLOG_ROW_ENGINE_AND_STMT_ENGINE = 1661
+ER_BINLOG_ROW_MODE_AND_STMT_ENGINE = 1662
+ER_BINLOG_UNSAFE_AND_STMT_ENGINE = 1663
+ER_BINLOG_ROW_INJECTION_AND_STMT_ENGINE = 1664
+ER_BINLOG_STMT_MODE_AND_ROW_ENGINE = 1665
+ER_BINLOG_ROW_INJECTION_AND_STMT_MODE = 1666
+ER_BINLOG_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1667
+ER_BINLOG_UNSAFE_LIMIT = 1668
+ER_BINLOG_UNSAFE_INSERT_DELAYED = 1669
+ER_BINLOG_UNSAFE_SYSTEM_TABLE = 1670
+ER_BINLOG_UNSAFE_AUTOINC_COLUMNS = 1671
+ER_BINLOG_UNSAFE_UDF = 1672
+ER_BINLOG_UNSAFE_SYSTEM_VARIABLE = 1673
+ER_BINLOG_UNSAFE_SYSTEM_FUNCTION = 1674
+ER_BINLOG_UNSAFE_NONTRANS_AFTER_TRANS = 1675
+ER_MESSAGE_AND_STATEMENT = 1676
+ER_SLAVE_CONVERSION_FAILED = 1677
+ER_SLAVE_CANT_CREATE_CONVERSION = 1678
+ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1679
+ER_PATH_LENGTH = 1680
+ER_WARN_DEPRECATED_SYNTAX_NO_REPLACEMENT = 1681
+ER_WRONG_NATIVE_TABLE_STRUCTURE = 1682
+ER_WRONG_PERFSCHEMA_USAGE = 1683
+ER_WARN_I_S_SKIPPED_TABLE = 1684
+ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1685
+ER_STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1686
+ER_SPATIAL_MUST_HAVE_GEOM_COL = 1687
+ER_TOO_LONG_INDEX_COMMENT = 1688
+ER_LOCK_ABORTED = 1689
+ER_DATA_OUT_OF_RANGE = 1690
+ER_WRONG_SPVAR_TYPE_IN_LIMIT = 1691
+ER_BINLOG_UNSAFE_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1692
+ER_BINLOG_UNSAFE_MIXED_STATEMENT = 1693
+ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1694
+ER_STORED_FUNCTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1695
+ER_FAILED_READ_FROM_PAR_FILE = 1696
+ER_VALUES_IS_NOT_INT_TYPE_ERROR = 1697
+ER_ACCESS_DENIED_NO_PASSWORD_ERROR = 1698
+ER_SET_PASSWORD_AUTH_PLUGIN = 1699
+ER_GRANT_PLUGIN_USER_EXISTS = 1700
+ER_TRUNCATE_ILLEGAL_FK = 1701
+ER_PLUGIN_IS_PERMANENT = 1702
+ER_SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MIN = 1703
+ER_SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MAX = 1704
+ER_STMT_CACHE_FULL = 1705
+ER_MULTI_UPDATE_KEY_CONFLICT = 1706
+ER_TABLE_NEEDS_REBUILD = 1707
+WARN_OPTION_BELOW_LIMIT = 1708
+ER_INDEX_COLUMN_TOO_LONG = 1709
+ER_ERROR_IN_TRIGGER_BODY = 1710
+ER_ERROR_IN_UNKNOWN_TRIGGER_BODY = 1711
+ER_INDEX_CORRUPT = 1712
+ER_UNDO_RECORD_TOO_BIG = 1713
+ER_BINLOG_UNSAFE_INSERT_IGNORE_SELECT = 1714
+ER_BINLOG_UNSAFE_INSERT_SELECT_UPDATE = 1715
+ER_BINLOG_UNSAFE_REPLACE_SELECT = 1716
+ER_BINLOG_UNSAFE_CREATE_IGNORE_SELECT = 1717
+ER_BINLOG_UNSAFE_CREATE_REPLACE_SELECT = 1718
+ER_BINLOG_UNSAFE_UPDATE_IGNORE = 1719
+ER_BINLOG_UNSAFE_WRITE_AUTOINC_SELECT = 1722
+ER_BINLOG_UNSAFE_CREATE_SELECT_AUTOINC = 1723
+ER_BINLOG_UNSAFE_INSERT_TWO_KEYS = 1724
+ER_VERS_NOT_ALLOWED = 1726
+ER_BINLOG_UNSAFE_AUTOINC_NOT_FIRST = 1727
+ER_CANNOT_LOAD_FROM_TABLE_V2 = 1728
+ER_MASTER_DELAY_VALUE_OUT_OF_RANGE = 1729
+ER_ONLY_FD_AND_RBR_EVENTS_ALLOWED_IN_BINLOG_STATEMENT = 1730
+ER_PARTITION_EXCHANGE_DIFFERENT_OPTION = 1731
+ER_PARTITION_EXCHANGE_PART_TABLE = 1732
+ER_PARTITION_EXCHANGE_TEMP_TABLE = 1733
+ER_PARTITION_INSTEAD_OF_SUBPARTITION = 1734
+ER_UNKNOWN_PARTITION = 1735
+ER_TABLES_DIFFERENT_METADATA = 1736
+ER_ROW_DOES_NOT_MATCH_PARTITION = 1737
+ER_BINLOG_CACHE_SIZE_GREATER_THAN_MAX = 1738
+ER_WARN_INDEX_NOT_APPLICABLE = 1739
+ER_PARTITION_EXCHANGE_FOREIGN_KEY = 1740
+ER_NO_SUCH_KEY_VALUE = 1741
+ER_VALUE_TOO_LONG = 1742
+ER_NETWORK_READ_EVENT_CHECKSUM_FAILURE = 1743
+ER_BINLOG_READ_EVENT_CHECKSUM_FAILURE = 1744
+ER_BINLOG_STMT_CACHE_SIZE_GREATER_THAN_MAX = 1745
+ER_CANT_UPDATE_TABLE_IN_CREATE_TABLE_SELECT = 1746
+ER_PARTITION_CLAUSE_ON_NONPARTITIONED = 1747
+ER_ROW_DOES_NOT_MATCH_GIVEN_PARTITION_SET = 1748
+ER_CHANGE_RPL_INFO_REPOSITORY_FAILURE = 1750
+ER_WARNING_NOT_COMPLETE_ROLLBACK_WITH_CREATED_TEMP_TABLE = 1751
+ER_WARNING_NOT_COMPLETE_ROLLBACK_WITH_DROPPED_TEMP_TABLE = 1752
+ER_MTS_FEATURE_IS_NOT_SUPPORTED = 1753
+ER_MTS_UPDATED_DBS_GREATER_MAX = 1754
+ER_MTS_CANT_PARALLEL = 1755
+ER_MTS_INCONSISTENT_DATA = 1756
+ER_FULLTEXT_NOT_SUPPORTED_WITH_PARTITIONING = 1757
+ER_DA_INVALID_CONDITION_NUMBER = 1758
+ER_INSECURE_PLAIN_TEXT = 1759
+ER_INSECURE_CHANGE_MASTER = 1760
+ER_FOREIGN_DUPLICATE_KEY_WITH_CHILD_INFO = 1761
+ER_FOREIGN_DUPLICATE_KEY_WITHOUT_CHILD_INFO = 1762
+ER_SQLTHREAD_WITH_SECURE_SLAVE = 1763
+ER_TABLE_HAS_NO_FT = 1764
+ER_VARIABLE_NOT_SETTABLE_IN_SF_OR_TRIGGER = 1765
+ER_VARIABLE_NOT_SETTABLE_IN_TRANSACTION = 1766
+ER_GTID_NEXT_IS_NOT_IN_GTID_NEXT_LIST = 1767
+ER_CANT_CHANGE_GTID_NEXT_IN_TRANSACTION_WHEN_GTID_NEXT_LIST_IS_NULL = 1768
+ER_SET_STATEMENT_CANNOT_INVOKE_FUNCTION = 1769
+ER_GTID_NEXT_CANT_BE_AUTOMATIC_IF_GTID_NEXT_LIST_IS_NON_NULL = 1770
+ER_SKIPPING_LOGGED_TRANSACTION = 1771
+ER_MALFORMED_GTID_SET_SPECIFICATION = 1772
+ER_MALFORMED_GTID_SET_ENCODING = 1773
+ER_MALFORMED_GTID_SPECIFICATION = 1774
+ER_GNO_EXHAUSTED = 1775
+ER_BAD_SLAVE_AUTO_POSITION = 1776
+ER_AUTO_POSITION_REQUIRES_GTID_MODE_ON = 1777
+ER_CANT_DO_IMPLICIT_COMMIT_IN_TRX_WHEN_GTID_NEXT_IS_SET = 1778
+ER_GTID_MODE_2_OR_3_REQUIRES_ENFORCE_GTID_CONSISTENCY_ON = 1779
+ER_GTID_MODE_REQUIRES_BINLOG = 1780
+ER_CANT_SET_GTID_NEXT_TO_GTID_WHEN_GTID_MODE_IS_OFF = 1781
+ER_CANT_SET_GTID_NEXT_TO_ANONYMOUS_WHEN_GTID_MODE_IS_ON = 1782
+ER_CANT_SET_GTID_NEXT_LIST_TO_NON_NULL_WHEN_GTID_MODE_IS_OFF = 1783
+ER_FOUND_GTID_EVENT_WHEN_GTID_MODE_IS_OFF = 1784
+ER_GTID_UNSAFE_NON_TRANSACTIONAL_TABLE = 1785
+ER_GTID_UNSAFE_CREATE_SELECT = 1786
+ER_GTID_UNSAFE_CREATE_DROP_TEMPORARY_TABLE_IN_TRANSACTION = 1787
+ER_GTID_MODE_CAN_ONLY_CHANGE_ONE_STEP_AT_A_TIME = 1788
+ER_MASTER_HAS_PURGED_REQUIRED_GTIDS = 1789
+ER_CANT_SET_GTID_NEXT_WHEN_OWNING_GTID = 1790
+ER_UNKNOWN_EXPLAIN_FORMAT = 1791
+ER_CANT_EXECUTE_IN_READ_ONLY_TRANSACTION = 1792
+ER_TOO_LONG_TABLE_PARTITION_COMMENT = 1793
+ER_SLAVE_CONFIGURATION = 1794
+ER_INNODB_FT_LIMIT = 1795
+ER_INNODB_NO_FT_TEMP_TABLE = 1796
+ER_INNODB_FT_WRONG_DOCID_COLUMN = 1797
+ER_INNODB_FT_WRONG_DOCID_INDEX = 1798
+ER_INNODB_ONLINE_LOG_TOO_BIG = 1799
+ER_UNKNOWN_ALTER_ALGORITHM = 1800
+ER_UNKNOWN_ALTER_LOCK = 1801
+ER_MTS_CHANGE_MASTER_CANT_RUN_WITH_GAPS = 1802
+ER_MTS_RECOVERY_FAILURE = 1803
+ER_MTS_RESET_WORKERS = 1804
+ER_COL_COUNT_DOESNT_MATCH_CORRUPTED_V2 = 1805
+ER_SLAVE_SILENT_RETRY_TRANSACTION = 1806
+ER_TABLE_SCHEMA_MISMATCH = 1808
+ER_TABLE_IN_SYSTEM_TABLESPACE = 1809
+ER_IO_READ_ERROR = 1810
+ER_IO_WRITE_ERROR = 1811
+ER_TABLESPACE_MISSING = 1812
+ER_TABLESPACE_EXISTS = 1813
+ER_TABLESPACE_DISCARDED = 1814
+ER_INTERNAL_ERROR = 1815
+ER_INNODB_IMPORT_ERROR = 1816
+ER_INNODB_INDEX_CORRUPT = 1817
+ER_INVALID_YEAR_COLUMN_LENGTH = 1818
+ER_NOT_VALID_PASSWORD = 1819
+ER_MUST_CHANGE_PASSWORD = 1820
+ER_FK_NO_INDEX_CHILD = 1821
+ER_FK_NO_INDEX_PARENT = 1822
+ER_FK_FAIL_ADD_SYSTEM = 1823
+ER_FK_CANNOT_OPEN_PARENT = 1824
+ER_FK_INCORRECT_OPTION = 1825
+ER_DUP_CONSTRAINT_NAME = 1826
+ER_PASSWORD_FORMAT = 1827
+ER_FK_COLUMN_CANNOT_DROP = 1828
+ER_FK_COLUMN_CANNOT_DROP_CHILD = 1829
+ER_FK_COLUMN_NOT_NULL = 1830
+ER_DUP_INDEX = 1831
+ER_FK_COLUMN_CANNOT_CHANGE = 1832
+ER_FK_COLUMN_CANNOT_CHANGE_CHILD = 1833
+ER_FK_CANNOT_DELETE_PARENT = 1834
+ER_MALFORMED_PACKET = 1835
+ER_READ_ONLY_MODE = 1836
+ER_GTID_NEXT_TYPE_UNDEFINED_GROUP = 1837
+ER_VARIABLE_NOT_SETTABLE_IN_SP = 1838
+ER_CANT_SET_GTID_PURGED_WHEN_GTID_MODE_IS_OFF = 1839
+ER_CANT_SET_GTID_PURGED_WHEN_GTID_EXECUTED_IS_NOT_EMPTY = 1840
+ER_CANT_SET_GTID_PURGED_WHEN_OWNED_GTIDS_IS_NOT_EMPTY = 1841
+ER_GTID_PURGED_WAS_CHANGED = 1842
+ER_GTID_EXECUTED_WAS_CHANGED = 1843
+ER_BINLOG_STMT_MODE_AND_NO_REPL_TABLES = 1844
+ER_ALTER_OPERATION_NOT_SUPPORTED = 1845
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON = 1846
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_COPY = 1847
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_PARTITION = 1848
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_RENAME = 1849
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_COLUMN_TYPE = 1850
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_CHECK = 1851
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_IGNORE = 1852
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_NOPK = 1853
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_AUTOINC = 1854
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_HIDDEN_FTS = 1855
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_CHANGE_FTS = 1856
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_FTS = 1857
+ER_SQL_SLAVE_SKIP_COUNTER_NOT_SETTABLE_IN_GTID_MODE = 1858
+ER_DUP_UNKNOWN_IN_INDEX = 1859
+ER_IDENT_CAUSES_TOO_LONG_PATH = 1860
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_NOT_NULL = 1861
+ER_MUST_CHANGE_PASSWORD_LOGIN = 1862
+ER_ROW_IN_WRONG_PARTITION = 1863
+ER_MTS_EVENT_BIGGER_PENDING_JOBS_SIZE_MAX = 1864
+ER_INNODB_NO_FT_USES_PARSER = 1865
+ER_BINLOG_LOGICAL_CORRUPTION = 1866
+ER_WARN_PURGE_LOG_IN_USE = 1867
+ER_WARN_PURGE_LOG_IS_ACTIVE = 1868
+ER_AUTO_INCREMENT_CONFLICT = 1869
+WARN_ON_BLOCKHOLE_IN_RBR = 1870
+ER_SLAVE_MI_INIT_REPOSITORY = 1871
+ER_SLAVE_RLI_INIT_REPOSITORY = 1872
+ER_ACCESS_DENIED_CHANGE_USER_ERROR = 1873
+ER_INNODB_READ_ONLY = 1874
+ER_STOP_SLAVE_SQL_THREAD_TIMEOUT = 1875
+ER_STOP_SLAVE_IO_THREAD_TIMEOUT = 1876
+ER_TABLE_CORRUPT = 1877
+ER_TEMP_FILE_WRITE_FAILURE = 1878
+ER_INNODB_FT_AUX_NOT_HEX_ID = 1879
+ER_LAST_MYSQL_ERROR_MESSAGE = 1880
+ER_ERROR_LAST_SECTION_1 = 1880
+ER_ERROR_FIRST_SECTION_2 = 1900
+ER_GENERATED_COLUMN_FUNCTION_IS_NOT_ALLOWED = 1901
+ER_PRIMARY_KEY_BASED_ON_GENERATED_COLUMN = 1903
+ER_KEY_BASED_ON_GENERATED_VIRTUAL_COLUMN = 1904
+ER_WRONG_FK_OPTION_FOR_GENERATED_COLUMN = 1905
+ER_WARNING_NON_DEFAULT_VALUE_FOR_GENERATED_COLUMN = 1906
+ER_UNSUPPORTED_ACTION_ON_GENERATED_COLUMN = 1907
+ER_UNSUPPORTED_ENGINE_FOR_GENERATED_COLUMNS = 1910
+ER_UNKNOWN_OPTION = 1911
+ER_BAD_OPTION_VALUE = 1912
+ER_DATA_OVERFLOW = 1916
+ER_DATA_TRUNCATED = 1917
+ER_BAD_DATA = 1918
+ER_DYN_COL_WRONG_FORMAT = 1919
+ER_DYN_COL_IMPLEMENTATION_LIMIT = 1920
+ER_DYN_COL_DATA = 1921
+ER_DYN_COL_WRONG_CHARSET = 1922
+ER_ILLEGAL_SUBQUERY_OPTIMIZER_SWITCHES = 1923
+ER_QUERY_CACHE_IS_DISABLED = 1924
+ER_QUERY_CACHE_IS_GLOBALY_DISABLED = 1925
+ER_VIEW_ORDERBY_IGNORED = 1926
+ER_CONNECTION_KILLED = 1927
+ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_SKIP_REPLICATION = 1929
+ER_STORED_FUNCTION_PREVENTS_SWITCH_SKIP_REPLICATION = 1930
+ER_QUERY_EXCEEDED_ROWS_EXAMINED_LIMIT = 1931
+ER_NO_SUCH_TABLE_IN_ENGINE = 1932
+ER_TARGET_NOT_EXPLAINABLE = 1933
+ER_CONNECTION_ALREADY_EXISTS = 1934
+ER_MASTER_LOG_PREFIX = 1935
+ER_CANT_START_STOP_SLAVE = 1936
+ER_SLAVE_STARTED = 1937
+ER_SLAVE_STOPPED = 1938
+ER_SQL_DISCOVER_ERROR = 1939
+ER_FAILED_GTID_STATE_INIT = 1940
+ER_INCORRECT_GTID_STATE = 1941
+ER_CANNOT_UPDATE_GTID_STATE = 1942
+ER_DUPLICATE_GTID_DOMAIN = 1943
+ER_GTID_OPEN_TABLE_FAILED = 1944
+ER_GTID_POSITION_NOT_FOUND_IN_BINLOG = 1945
+ER_CANNOT_LOAD_SLAVE_GTID_STATE = 1946
+ER_MASTER_GTID_POS_CONFLICTS_WITH_BINLOG = 1947
+ER_MASTER_GTID_POS_MISSING_DOMAIN = 1948
+ER_UNTIL_REQUIRES_USING_GTID = 1949
+ER_GTID_STRICT_OUT_OF_ORDER = 1950
+ER_GTID_START_FROM_BINLOG_HOLE = 1951
+ER_SLAVE_UNEXPECTED_MASTER_SWITCH = 1952
+ER_INSIDE_TRANSACTION_PREVENTS_SWITCH_GTID_DOMAIN_ID_SEQ_NO = 1953
+ER_STORED_FUNCTION_PREVENTS_SWITCH_GTID_DOMAIN_ID_SEQ_NO = 1954
+ER_GTID_POSITION_NOT_FOUND_IN_BINLOG2 = 1955
+ER_BINLOG_MUST_BE_EMPTY = 1956
+ER_NO_SUCH_QUERY = 1957
+ER_BAD_BASE64_DATA = 1958
+ER_INVALID_ROLE = 1959
+ER_INVALID_CURRENT_USER = 1960
+ER_CANNOT_GRANT_ROLE = 1961
+ER_CANNOT_REVOKE_ROLE = 1962
+ER_CHANGE_SLAVE_PARALLEL_THREADS_ACTIVE = 1963
+ER_PRIOR_COMMIT_FAILED = 1964
+ER_IT_IS_A_VIEW = 1965
+ER_SLAVE_SKIP_NOT_IN_GTID = 1966
+ER_TABLE_DEFINITION_TOO_BIG = 1967
+ER_PLUGIN_INSTALLED = 1968
+ER_STATEMENT_TIMEOUT = 1969
+ER_SUBQUERIES_NOT_SUPPORTED = 1970
+ER_SET_STATEMENT_NOT_SUPPORTED = 1971
+ER_USER_CREATE_EXISTS = 1973
+ER_USER_DROP_EXISTS = 1974
+ER_ROLE_CREATE_EXISTS = 1975
+ER_ROLE_DROP_EXISTS = 1976
+ER_CANNOT_CONVERT_CHARACTER = 1977
+ER_INVALID_DEFAULT_VALUE_FOR_FIELD = 1978
+ER_KILL_QUERY_DENIED_ERROR = 1979
+ER_NO_EIS_FOR_FIELD = 1980
+ER_WARN_AGGFUNC_DEPENDENCE = 1981
+WARN_INNODB_PARTITION_OPTION_IGNORED = 1982
+ER_ERROR_LAST_SECTION_2 = 1982
+ER_ERROR_FIRST_SECTION_3 = 2000
+ER_ERROR_LAST_SECTION_3 = 2000
+ER_ERROR_FIRST_SECTION_4 = 3000
+ER_FILE_CORRUPT = 3000
+ER_ERROR_ON_MASTER = 3001
+ER_INCONSISTENT_ERROR = 3002
+ER_STORAGE_ENGINE_NOT_LOADED = 3003
+ER_GET_STACKED_DA_WITHOUT_ACTIVE_HANDLER = 3004
+ER_WARN_LEGACY_SYNTAX_CONVERTED = 3005
+ER_BINLOG_UNSAFE_FULLTEXT_PLUGIN = 3006
+ER_CANNOT_DISCARD_TEMPORARY_TABLE = 3007
+ER_FK_DEPTH_EXCEEDED = 3008
+ER_COL_COUNT_DOESNT_MATCH_PLEASE_UPDATE_V2 = 3009
+ER_WARN_TRIGGER_DOESNT_HAVE_CREATED = 3010
+ER_REFERENCED_TRG_DOES_NOT_EXIST_MYSQL = 3011
+ER_EXPLAIN_NOT_SUPPORTED = 3012
+ER_INVALID_FIELD_SIZE = 3013
+ER_MISSING_HA_CREATE_OPTION = 3014
+ER_ENGINE_OUT_OF_MEMORY = 3015
+ER_PASSWORD_EXPIRE_ANONYMOUS_USER = 3016
+ER_SLAVE_SQL_THREAD_MUST_STOP = 3017
+ER_NO_FT_MATERIALIZED_SUBQUERY = 3018
+ER_INNODB_UNDO_LOG_FULL = 3019
+ER_INVALID_ARGUMENT_FOR_LOGARITHM = 3020
+ER_SLAVE_CHANNEL_IO_THREAD_MUST_STOP = 3021
+ER_WARN_OPEN_TEMP_TABLES_MUST_BE_ZERO = 3022
+ER_WARN_ONLY_MASTER_LOG_FILE_NO_POS = 3023
+ER_QUERY_TIMEOUT = 3024
+ER_NON_RO_SELECT_DISABLE_TIMER = 3025
+ER_DUP_LIST_ENTRY = 3026
+ER_SQL_MODE_NO_EFFECT = 3027
+ER_AGGREGATE_ORDER_FOR_UNION = 3028
+ER_AGGREGATE_ORDER_NON_AGG_QUERY = 3029
+ER_SLAVE_WORKER_STOPPED_PREVIOUS_THD_ERROR = 3030
+ER_DONT_SUPPORT_SLAVE_PRESERVE_COMMIT_ORDER = 3031
+ER_SERVER_OFFLINE_MODE = 3032
+ER_GIS_DIFFERENT_SRIDS = 3033
+ER_GIS_UNSUPPORTED_ARGUMENT = 3034
+ER_GIS_UNKNOWN_ERROR = 3035
+ER_GIS_UNKNOWN_EXCEPTION = 3036
+ER_GIS_INVALID_DATA = 3037
+ER_BOOST_GEOMETRY_EMPTY_INPUT_EXCEPTION = 3038
+ER_BOOST_GEOMETRY_CENTROID_EXCEPTION = 3039
+ER_BOOST_GEOMETRY_OVERLAY_INVALID_INPUT_EXCEPTION = 3040
+ER_BOOST_GEOMETRY_TURN_INFO_EXCEPTION = 3041
+ER_BOOST_GEOMETRY_SELF_INTERSECTION_POINT_EXCEPTION = 3042
+ER_BOOST_GEOMETRY_UNKNOWN_EXCEPTION = 3043
+ER_STD_BAD_ALLOC_ERROR = 3044
+ER_STD_DOMAIN_ERROR = 3045
+ER_STD_LENGTH_ERROR = 3046
+ER_STD_INVALID_ARGUMENT = 3047
+ER_STD_OUT_OF_RANGE_ERROR = 3048
+ER_STD_OVERFLOW_ERROR = 3049
+ER_STD_RANGE_ERROR = 3050
+ER_STD_UNDERFLOW_ERROR = 3051
+ER_STD_LOGIC_ERROR = 3052
+ER_STD_RUNTIME_ERROR = 3053
+ER_STD_UNKNOWN_EXCEPTION = 3054
+ER_GIS_DATA_WRONG_ENDIANESS = 3055
+ER_CHANGE_MASTER_PASSWORD_LENGTH = 3056
+ER_USER_LOCK_WRONG_NAME = 3057
+ER_USER_LOCK_DEADLOCK = 3058
+ER_REPLACE_INACCESSIBLE_ROWS = 3059
+ER_ALTER_OPERATION_NOT_SUPPORTED_REASON_GIS = 3060
+ER_ERROR_LAST_SECTION_4 = 3060
+ER_ERROR_FIRST_SECTION_5 = 4000
+ER_WITH_COL_WRONG_LIST = 4002
+ER_TOO_MANY_DEFINITIONS_IN_WITH_CLAUSE = 4003
+ER_DUP_QUERY_NAME = 4004
+ER_RECURSIVE_WITHOUT_ANCHORS = 4005
+ER_UNACCEPTABLE_MUTUAL_RECURSION = 4006
+ER_REF_TO_RECURSIVE_WITH_TABLE_IN_DERIVED = 4007
+ER_NOT_STANDARD_COMPLIANT_RECURSIVE = 4008
+ER_WRONG_WINDOW_SPEC_NAME = 4009
+ER_DUP_WINDOW_NAME = 4010
+ER_PARTITION_LIST_IN_REFERENCING_WINDOW_SPEC = 4011
+ER_ORDER_LIST_IN_REFERENCING_WINDOW_SPEC = 4012
+ER_WINDOW_FRAME_IN_REFERENCED_WINDOW_SPEC = 4013
+ER_BAD_COMBINATION_OF_WINDOW_FRAME_BOUND_SPECS = 4014
+ER_WRONG_PLACEMENT_OF_WINDOW_FUNCTION = 4015
+ER_WINDOW_FUNCTION_IN_WINDOW_SPEC = 4016
+ER_NOT_ALLOWED_WINDOW_FRAME = 4017
+ER_NO_ORDER_LIST_IN_WINDOW_SPEC = 4018
+ER_RANGE_FRAME_NEEDS_SIMPLE_ORDERBY = 4019
+ER_WRONG_TYPE_FOR_ROWS_FRAME = 4020
+ER_WRONG_TYPE_FOR_RANGE_FRAME = 4021
+ER_FRAME_EXCLUSION_NOT_SUPPORTED = 4022
+ER_WINDOW_FUNCTION_DONT_HAVE_FRAME = 4023
+ER_INVALID_NTILE_ARGUMENT = 4024
+ER_CONSTRAINT_FAILED = 4025
+ER_EXPRESSION_IS_TOO_BIG = 4026
+ER_ERROR_EVALUATING_EXPRESSION = 4027
+ER_CALCULATING_DEFAULT_VALUE = 4028
+ER_EXPRESSION_REFERS_TO_UNINIT_FIELD = 4029
+ER_PARTITION_DEFAULT_ERROR = 4030
+ER_REFERENCED_TRG_DOES_NOT_EXIST = 4031
+ER_INVALID_DEFAULT_PARAM = 4032
+ER_BINLOG_NON_SUPPORTED_BULK = 4033
+ER_BINLOG_UNCOMPRESS_ERROR = 4034
+ER_JSON_BAD_CHR = 4035
+ER_JSON_NOT_JSON_CHR = 4036
+ER_JSON_EOS = 4037
+ER_JSON_SYNTAX = 4038
+ER_JSON_ESCAPING = 4039
+ER_JSON_DEPTH = 4040
+ER_JSON_PATH_EOS = 4041
+ER_JSON_PATH_SYNTAX = 4042
+ER_JSON_PATH_DEPTH = 4043
+ER_JSON_PATH_NO_WILDCARD = 4044
+ER_JSON_PATH_ARRAY = 4045
+ER_JSON_ONE_OR_ALL = 4046
+ER_UNSUPPORTED_COMPRESSED_TABLE = 4047
+ER_GEOJSON_INCORRECT = 4048
+ER_GEOJSON_TOO_FEW_POINTS = 4049
+ER_GEOJSON_NOT_CLOSED = 4050
+ER_JSON_PATH_EMPTY = 4051
+ER_SLAVE_SAME_ID = 4052
+ER_FLASHBACK_NOT_SUPPORTED = 4053
+ER_KEYS_OUT_OF_ORDER = 4054
+ER_OVERLAPPING_KEYS = 4055
+ER_REQUIRE_ROW_BINLOG_FORMAT = 4056
+ER_ISOLATION_MODE_NOT_SUPPORTED = 4057
+ER_ON_DUPLICATE_DISABLED = 4058
+ER_UPDATES_WITH_CONSISTENT_SNAPSHOT = 4059
+ER_ROLLBACK_ONLY = 4060
+ER_ROLLBACK_TO_SAVEPOINT = 4061
+ER_ISOLATION_LEVEL_WITH_CONSISTENT_SNAPSHOT = 4062
+ER_UNSUPPORTED_COLLATION = 4063
+ER_METADATA_INCONSISTENCY = 4064
+ER_CF_DIFFERENT = 4065
+ER_RDB_TTL_DURATION_FORMAT = 4066
+ER_RDB_STATUS_GENERAL = 4067
+ER_RDB_STATUS_MSG = 4068
+ER_RDB_TTL_UNSUPPORTED = 4069
+ER_RDB_TTL_COL_FORMAT = 4070
+ER_PER_INDEX_CF_DEPRECATED = 4071
+ER_KEY_CREATE_DURING_ALTER = 4072
+ER_SK_POPULATE_DURING_ALTER = 4073
+ER_SUM_FUNC_WITH_WINDOW_FUNC_AS_ARG = 4074
+ER_NET_OK_PACKET_TOO_LARGE = 4075
+ER_GEOJSON_EMPTY_COORDINATES = 4076
+ER_MYROCKS_CANT_NOPAD_COLLATION = 4077
+ER_ILLEGAL_PARAMETER_DATA_TYPES2_FOR_OPERATION = 4078
+ER_ILLEGAL_PARAMETER_DATA_TYPE_FOR_OPERATION = 4079
+ER_WRONG_PARAMCOUNT_TO_CURSOR = 4080
+ER_UNKNOWN_STRUCTURED_VARIABLE = 4081
+ER_ROW_VARIABLE_DOES_NOT_HAVE_FIELD = 4082
+ER_END_IDENTIFIER_DOES_NOT_MATCH = 4083
+ER_SEQUENCE_RUN_OUT = 4084
+ER_SEQUENCE_INVALID_DATA = 4085
+ER_SEQUENCE_INVALID_TABLE_STRUCTURE = 4086
+ER_SEQUENCE_ACCESS_ERROR = 4087
+ER_SEQUENCE_BINLOG_FORMAT = 4088
+ER_NOT_SEQUENCE = 4089
+ER_NOT_SEQUENCE2 = 4090
+ER_UNKNOWN_SEQUENCES = 4091
+ER_UNKNOWN_VIEW = 4092
+ER_WRONG_INSERT_INTO_SEQUENCE = 4093
+ER_SP_STACK_TRACE = 4094
+ER_PACKAGE_ROUTINE_IN_SPEC_NOT_DEFINED_IN_BODY = 4095
+ER_PACKAGE_ROUTINE_FORWARD_DECLARATION_NOT_DEFINED = 4096
+ER_COMPRESSED_COLUMN_USED_AS_KEY = 4097
+ER_UNKNOWN_COMPRESSION_METHOD = 4098
+ER_WRONG_NUMBER_OF_VALUES_IN_TVC = 4099
+ER_FIELD_REFERENCE_IN_TVC = 4100
+ER_WRONG_TYPE_FOR_PERCENTILE_FUNC = 4101
+ER_ARGUMENT_NOT_CONSTANT = 4102
+ER_ARGUMENT_OUT_OF_RANGE = 4103
+ER_WRONG_TYPE_OF_ARGUMENT = 4104
+ER_NOT_AGGREGATE_FUNCTION = 4105
+ER_INVALID_AGGREGATE_FUNCTION = 4106
+ER_INVALID_VALUE_TO_LIMIT = 4107
+ER_INVISIBLE_NOT_NULL_WITHOUT_DEFAULT = 4108
+ER_UPDATE_INFO_WITH_SYSTEM_VERSIONING = 4109
+ER_VERS_FIELD_WRONG_TYPE = 4110
+ER_VERS_ENGINE_UNSUPPORTED = 4111
+ER_PARTITION_WRONG_TYPE = 4113
+WARN_VERS_PART_FULL = 4114
+WARN_VERS_PARAMETERS = 4115
+ER_VERS_DROP_PARTITION_INTERVAL = 4116
+WARN_VERS_PART_NON_HISTORICAL = 4118
+ER_VERS_ALTER_NOT_ALLOWED = 4119
+ER_VERS_ALTER_ENGINE_PROHIBITED = 4120
+ER_VERS_RANGE_PROHIBITED = 4121
+ER_CONFLICTING_FOR_SYSTEM_TIME = 4122
+ER_VERS_TABLE_MUST_HAVE_COLUMNS = 4123
+ER_VERS_NOT_VERSIONED = 4124
+ER_MISSING = 4125
+ER_VERS_PERIOD_COLUMNS = 4126
+ER_PART_WRONG_VALUE = 4127
+ER_VERS_WRONG_PARTS = 4128
+ER_VERS_NO_TRX_ID = 4129
+ER_VERS_ALTER_SYSTEM_FIELD = 4130
+ER_DROP_VERSIONING_SYSTEM_TIME_PARTITION = 4131
+ER_VERS_DB_NOT_SUPPORTED = 4132
+ER_VERS_TRT_IS_DISABLED = 4133
+ER_VERS_DUPLICATE_ROW_START_END = 4134
+ER_VERS_ALREADY_VERSIONED = 4135
+ER_VERS_NOT_SUPPORTED = 4137
+ER_VERS_TRX_PART_HISTORIC_ROW_NOT_SUPPORTED = 4138
+ER_INDEX_FILE_FULL = 4139
+ER_UPDATED_COLUMN_ONLY_ONCE = 4140
+ER_EMPTY_ROW_IN_TVC = 4141
+ER_VERS_QUERY_IN_PARTITION = 4142
+ER_KEY_DOESNT_SUPPORT = 4143
+ER_ALTER_OPERATION_TABLE_OPTIONS_NEED_REBUILD = 4144
+ER_BACKUP_LOCK_IS_ACTIVE = 4145
+ER_BACKUP_NOT_RUNNING = 4146
+ER_BACKUP_WRONG_STAGE = 4147
+ER_BACKUP_STAGE_FAILED = 4148
+ER_BACKUP_UNKNOWN_STAGE = 4149
+ER_USER_IS_BLOCKED = 4150
+ER_ACCOUNT_HAS_BEEN_LOCKED = 4151
+ER_PERIOD_TEMPORARY_NOT_ALLOWED = 4152
+ER_PERIOD_TYPES_MISMATCH = 4153
+ER_MORE_THAN_ONE_PERIOD = 4154
+ER_PERIOD_FIELD_WRONG_ATTRIBUTES = 4155
+ER_PERIOD_NOT_FOUND = 4156
+ER_PERIOD_COLUMNS_UPDATED = 4157
+ER_PERIOD_CONSTRAINT_DROP = 4158
+ER_TOO_LONG_KEYPART = 4159
+ER_TOO_LONG_DATABASE_COMMENT = 4160
+ER_UNKNOWN_DATA_TYPE = 4161
+ER_UNKNOWN_OPERATOR = 4162
+ER_WARN_HISTORY_ROW_START_TIME = 4163
+ER_PART_STARTS_BEYOND_INTERVAL = 4164
+ER_GALERA_REPLICATION_NOT_SUPPORTED = 4165
+ER_LOAD_INFILE_CAPABILITY_DISABLED = 4166
+ER_NO_SECURE_TRANSPORTS_CONFIGURED = 4167
+ER_SLAVE_IGNORED_SHARED_TABLE = 4168
+ER_NO_AUTOINCREMENT_WITH_UNIQUE = 4169
+ER_KEY_CONTAINS_PERIOD_FIELDS = 4170
+ER_KEY_CANT_HAVE_WITHOUT_OVERLAPS = 4171
+ER_NOT_ALLOWED_IN_THIS_CONTEXT = 4172
+ER_DATA_WAS_COMMITED_UNDER_ROLLBACK = 4173
+ER_PK_INDEX_CANT_BE_IGNORED = 4174
+ER_BINLOG_UNSAFE_SKIP_LOCKED = 4175
+ER_JSON_TABLE_ERROR_ON_FIELD = 4176
+ER_JSON_TABLE_ALIAS_REQUIRED = 4177
+ER_JSON_TABLE_SCALAR_EXPECTED = 4178
+ER_JSON_TABLE_MULTIPLE_MATCHES = 4179
+ER_WITH_TIES_NEEDS_ORDER = 4180
+ER_REMOVED_ORPHAN_TRIGGER = 4181
+ER_STORAGE_ENGINE_DISABLED = 4182
+WARN_SFORMAT_ERROR = 4183
+ER_PARTITION_CONVERT_SUBPARTITIONED = 4184
+ER_PROVIDER_NOT_LOADED = 4185
+ER_JSON_HISTOGRAM_PARSE_FAILED = 4186
+ER_SF_OUT_INOUT_ARG_NOT_ALLOWED = 4187
+ER_INCONSISTENT_SLAVE_TEMP_TABLE = 4188
+CR_UNKNOWN_ERROR = 2000
+CR_SOCKET_CREATE_ERROR = 2001
+CR_CONNECTION_ERROR = 2002
+CR_CONN_HOST_ERROR = 2003
+CR_IPSOCK_ERROR = 2004
+CR_UNKNOWN_HOST = 2005
+CR_SERVER_GONE_ERROR = 2006
+CR_VERSION_ERROR = 2007
+CR_OUT_OF_MEMORY = 2008
+CR_WRONG_HOST_INFO = 2009
+CR_LOCALHOST_CONNECTION = 2010
+CR_TCP_CONNECTION = 2011
+CR_SERVER_HANDSHAKE_ERR = 2012
+CR_SERVER_LOST = 2013
+CR_COMMANDS_OUT_OF_SYNC = 2014
+CR_NAMEDPIPE_CONNECTION = 2015
+CR_NAMEDPIPEWAIT_ERROR = 2016
+CR_NAMEDPIPEOPEN_ERROR = 2017
+CR_NAMEDPIPESETSTATE_ERROR = 2018
+CR_CANT_READ_CHARSET = 2019
+CR_NET_PACKET_TOO_LARGE = 2020
+CR_SSL_CONNECTION_ERROR = 2026
+CR_MALFORMED_PACKET = 2027
+CR_NO_PREPARE_STMT = 2030
+CR_PARAMS_NOT_BOUND = 2031
+CR_INVALID_PARAMETER_NO = 2034
+CR_INVALID_BUFFER_USE = 2035
+CR_UNSUPPORTED_PARAM_TYPE = 2036
+CR_SHARED_MEMORY_CONNECTION = 2037
+CR_SHARED_MEMORY_CONNECT_ERROR = 2038
+CR_CONN_UNKNOWN_PROTOCOL = 2047
+CR_SECURE_AUTH = 2049
+CR_NO_DATA = 2051
+CR_NO_STMT_METADATA = 2052
+CR_NOT_IMPLEMENTED = 2054
+CR_SERVER_LOST_EXTENDED = 2055
+CR_STMT_CLOSED = 2056
+CR_NEW_STMT_METADATA = 2057
+CR_ALREADY_CONNECTED = 2058
+CR_AUTH_PLUGIN_CANNOT_LOAD = 2059
+CR_DUPLICATE_CONNECTION_ATTR = 2060
+CR_AUTH_PLUGIN_ERR = 2061
+CR_EVENT_CREATE_FAILED = 5000
+CR_BIND_ADDR_FAILED = 5001
+CR_ASYNC_NOT_SUPPORTED = 5002
+CR_FUNCTION_NOT_SUPPORTED = 5003
+CR_FILE_NOT_FOUND = 5004
+CR_FILE_READ = 5005
+CR_BULK_WITHOUT_PARAMETERS = 5006
+CR_INVALID_STMT = 5007
+CR_VERSION_MISMATCH = 5008
+CR_INVALID_PARAMETER = 5009
+CR_PLUGIN_NOT_ALLOWED = 5010
+CR_CONNSTR_PARSE_ERROR = 5011
+CR_ERR_LOAD_PLUGIN = 5012
```

### Comparing `mariadb-1.1.6/mariadb/constants/FIELD_TYPE.py` & `mariadb-1.1.7/mariadb/constants/FIELD_TYPE.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""
-MariaDB FIELD_TYPE Constants
-
-These constants represent the field types supported by MariaDB.
-The field type is returned as second element of cursor description attribute.
-
-Field types are defined in module *mariadb.constants.FIELD_TYPE*
-"""
-
-DECIMAL = 0
-TINY = 1
-SHORT = 2
-LONG = 3
-FLOAT = 4
-DOUBLE = 5
-NULL = 6
-TIMESTAMP = 7
-LONGLONG = 8
-INT24 = 9
-DATE = 10
-TIME = 11
-DATETIME = 12
-YEAR = 13
-NEWDATE = 14
-VARCHAR = 15
-BIT = 16
-TIMESTAMP2 = 17
-DATETIME2 = 18
-TIME2 = 19
-JSON = 245
-NEWDECIMAL = 246
-ENUM = 247
-SET = 248
-TINY_BLOB = 249
-MEDIUM_BLOB = 250
-LONG_BLOB = 251
-BLOB = 252
-VAR_STRING = 253
-STRING = 254
-GEOMETRY = 255
+"""
+MariaDB FIELD_TYPE Constants
+
+These constants represent the field types supported by MariaDB.
+The field type is returned as second element of cursor description attribute.
+
+Field types are defined in module *mariadb.constants.FIELD_TYPE*
+"""
+
+DECIMAL = 0
+TINY = 1
+SHORT = 2
+LONG = 3
+FLOAT = 4
+DOUBLE = 5
+NULL = 6
+TIMESTAMP = 7
+LONGLONG = 8
+INT24 = 9
+DATE = 10
+TIME = 11
+DATETIME = 12
+YEAR = 13
+NEWDATE = 14
+VARCHAR = 15
+BIT = 16
+TIMESTAMP2 = 17
+DATETIME2 = 18
+TIME2 = 19
+JSON = 245
+NEWDECIMAL = 246
+ENUM = 247
+SET = 248
+TINY_BLOB = 249
+MEDIUM_BLOB = 250
+LONG_BLOB = 251
+BLOB = 252
+VAR_STRING = 253
+STRING = 254
+GEOMETRY = 255
```

### Comparing `mariadb-1.1.6/mariadb/constants/INFO.py` & `mariadb-1.1.7/mariadb/constants/INFO.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""
-Constants for _get_info method of MariadB connection object
-"""
-
-CHARSET_ID = 0
-CHARSET_NAME = 1
-CLIENT_ERRORS = 2
-CLIENT_VERSION = 3
-CLIENT_VERSION_ID = 4
-ASYNC_TIMEOUT = 5
-ASYNC_TIMEOUT_MS = 6
-CHARSET_INFO = 7
-ERROR = 8
-ERROR_ID = 9
-HOST = 10
-INFO = 11
-PORT = 12
-PROTOCOL_VERSION_ID = 13
-PVIO_TYPE = 14
-SCHEMA = 15
-SERVER_TYPE = 16
-SERVER_VERSION = 17
-SERVER_VERSION_ID = 18
-SOCKET = 19
-SQLSTATE = 20
-SSL_CIPHER = 21
-TLS_LIBRARY = 22
-TLS_VERSION = 23
-TLS_VERSION_ID = 24
-TYPE = 25
-UNIX_SOCKET = 26
-USER = 27
-MAX_ALLOWED_PACKET = 28
-NET_BUFFER_LENGTH = 29
-SERVER_STATUS = 30
-SERVER_CAPABILITIES = 31
-EXTENDED_SERVER_CAPABILITIES = 32
-CLIENT_CAPABILITIES = 33
-BYTES_READ = 34
-BYTES_SENT = 35
+"""
+Constants for _get_info method of MariadB connection object
+"""
+
+CHARSET_ID = 0
+CHARSET_NAME = 1
+CLIENT_ERRORS = 2
+CLIENT_VERSION = 3
+CLIENT_VERSION_ID = 4
+ASYNC_TIMEOUT = 5
+ASYNC_TIMEOUT_MS = 6
+CHARSET_INFO = 7
+ERROR = 8
+ERROR_ID = 9
+HOST = 10
+INFO = 11
+PORT = 12
+PROTOCOL_VERSION_ID = 13
+PVIO_TYPE = 14
+SCHEMA = 15
+SERVER_TYPE = 16
+SERVER_VERSION = 17
+SERVER_VERSION_ID = 18
+SOCKET = 19
+SQLSTATE = 20
+SSL_CIPHER = 21
+TLS_LIBRARY = 22
+TLS_VERSION = 23
+TLS_VERSION_ID = 24
+TYPE = 25
+UNIX_SOCKET = 26
+USER = 27
+MAX_ALLOWED_PACKET = 28
+NET_BUFFER_LENGTH = 29
+SERVER_STATUS = 30
+SERVER_CAPABILITIES = 31
+EXTENDED_SERVER_CAPABILITIES = 32
+CLIENT_CAPABILITIES = 33
+BYTES_READ = 34
+BYTES_SENT = 35
```

### Comparing `mariadb-1.1.6/mariadb/field.py` & `mariadb-1.1.7/mariadb/field.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from mariadb.constants import FIELD_TYPE, FIELD_FLAG
-
-field_types = {FIELD_TYPE.DECIMAL: "DECIMAL",
-               FIELD_TYPE.TINY:  "TINY",
-               FIELD_TYPE.SHORT: "SHORT",
-               FIELD_TYPE.LONG: "LONG",
-               FIELD_TYPE.FLOAT: "FLOAT",
-               FIELD_TYPE.DOUBLE: "DOUBLE",
-               FIELD_TYPE.NULL: "NULL",
-               FIELD_TYPE.TIMESTAMP: "TIMESTAMP",
-               FIELD_TYPE.LONGLONG: "LONGLONG",
-               FIELD_TYPE.INT24: "INT24",
-               FIELD_TYPE.DATE: "DATE",
-               FIELD_TYPE.TIME: "TIME",
-               FIELD_TYPE.DATETIME: "DATETIME",
-               FIELD_TYPE.YEAR: "YEAR",
-               FIELD_TYPE.NEWDATE: "NEWDATE",
-               FIELD_TYPE.VARCHAR: "VARCHAR",
-               FIELD_TYPE.BIT: "BIT",
-               FIELD_TYPE.JSON: "JSON",
-               FIELD_TYPE.NEWDECIMAL: "NEWDECIMAL",
-               FIELD_TYPE.ENUM: "ENUM",
-               FIELD_TYPE.SET: "SET",
-               FIELD_TYPE.TINY_BLOB: "TINY_BLOB",
-               FIELD_TYPE.MEDIUM_BLOB: "MEDIUM_BLOB",
-               FIELD_TYPE.LONG_BLOB: "LONG_BLOB",
-               FIELD_TYPE.BLOB: "BLOB",
-               FIELD_TYPE.VAR_STRING: "VAR_STRING",
-               FIELD_TYPE.STRING: "STRING",
-               FIELD_TYPE.GEOMETRY: "GEOMETRY"}
-
-field_flags = {FIELD_FLAG.NOT_NULL: "NOT_NULL",
-               FIELD_FLAG.PRIMARY_KEY: "PRIMARY_KEY",
-               FIELD_FLAG.UNIQUE_KEY: "UNIQUE_KEY",
-               FIELD_FLAG.MULTIPLE_KEY: "PART_KEY",
-               FIELD_FLAG.BLOB: "BLOB",
-               FIELD_FLAG.UNSIGNED: "UNSIGNED",
-               FIELD_FLAG.ZEROFILL: "ZEROFILL",
-               FIELD_FLAG.BINARY: "BINARY",
-               FIELD_FLAG.ENUM: "NUMERIC",
-               FIELD_FLAG.AUTO_INCREMENT: "AUTO_INCREMENT",
-               FIELD_FLAG.TIMESTAMP: "TIMESTAMP",
-               FIELD_FLAG.SET: "SET",
-               FIELD_FLAG.NO_DEFAULT: "NO_DEFAULT",
-               FIELD_FLAG.ON_UPDATE_NOW: "UPDATE_TIMESTAMP",
-               FIELD_FLAG.NUMERIC: "NUMERIC"}
-
-
-class fieldinfo():
-
-    def type(self, description):
-        if description[1] in field_types:
-            return field_types[description[1]]
-        return None
-
-    def flag(self, description):
-        flags = [field_flags[f] for f in field_flags.keys()
-                 if description[7] & f]
-        return " | ".join(flags)
+from mariadb.constants import FIELD_TYPE, FIELD_FLAG
+
+field_types = {FIELD_TYPE.DECIMAL: "DECIMAL",
+               FIELD_TYPE.TINY:  "TINY",
+               FIELD_TYPE.SHORT: "SHORT",
+               FIELD_TYPE.LONG: "LONG",
+               FIELD_TYPE.FLOAT: "FLOAT",
+               FIELD_TYPE.DOUBLE: "DOUBLE",
+               FIELD_TYPE.NULL: "NULL",
+               FIELD_TYPE.TIMESTAMP: "TIMESTAMP",
+               FIELD_TYPE.LONGLONG: "LONGLONG",
+               FIELD_TYPE.INT24: "INT24",
+               FIELD_TYPE.DATE: "DATE",
+               FIELD_TYPE.TIME: "TIME",
+               FIELD_TYPE.DATETIME: "DATETIME",
+               FIELD_TYPE.YEAR: "YEAR",
+               FIELD_TYPE.NEWDATE: "NEWDATE",
+               FIELD_TYPE.VARCHAR: "VARCHAR",
+               FIELD_TYPE.BIT: "BIT",
+               FIELD_TYPE.JSON: "JSON",
+               FIELD_TYPE.NEWDECIMAL: "NEWDECIMAL",
+               FIELD_TYPE.ENUM: "ENUM",
+               FIELD_TYPE.SET: "SET",
+               FIELD_TYPE.TINY_BLOB: "TINY_BLOB",
+               FIELD_TYPE.MEDIUM_BLOB: "MEDIUM_BLOB",
+               FIELD_TYPE.LONG_BLOB: "LONG_BLOB",
+               FIELD_TYPE.BLOB: "BLOB",
+               FIELD_TYPE.VAR_STRING: "VAR_STRING",
+               FIELD_TYPE.STRING: "STRING",
+               FIELD_TYPE.GEOMETRY: "GEOMETRY"}
+
+field_flags = {FIELD_FLAG.NOT_NULL: "NOT_NULL",
+               FIELD_FLAG.PRIMARY_KEY: "PRIMARY_KEY",
+               FIELD_FLAG.UNIQUE_KEY: "UNIQUE_KEY",
+               FIELD_FLAG.MULTIPLE_KEY: "PART_KEY",
+               FIELD_FLAG.BLOB: "BLOB",
+               FIELD_FLAG.UNSIGNED: "UNSIGNED",
+               FIELD_FLAG.ZEROFILL: "ZEROFILL",
+               FIELD_FLAG.BINARY: "BINARY",
+               FIELD_FLAG.ENUM: "NUMERIC",
+               FIELD_FLAG.AUTO_INCREMENT: "AUTO_INCREMENT",
+               FIELD_FLAG.TIMESTAMP: "TIMESTAMP",
+               FIELD_FLAG.SET: "SET",
+               FIELD_FLAG.NO_DEFAULT: "NO_DEFAULT",
+               FIELD_FLAG.ON_UPDATE_NOW: "UPDATE_TIMESTAMP",
+               FIELD_FLAG.NUMERIC: "NUMERIC"}
+
+
+class fieldinfo():
+
+    def type(self, description):
+        if description[1] in field_types:
+            return field_types[description[1]]
+        return None
+
+    def flag(self, description):
+        flags = [field_flags[f] for f in field_flags.keys()
+                 if description[7] & f]
+        return " | ".join(flags)
```

### Comparing `mariadb-1.1.6/mariadb/mariadb.c` & `mariadb-1.1.7/mariadb/mariadb.c`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-/******************************************************************************
-  Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
-
-  This library is free software; you can redistribute it and/or
-  modify it under the terms of the GNU Library General Public
-  License as published by the Free Software Foundation; either
-  version 2 of the License, or (at your option) any later version.
-
-  This library is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-  Library General Public License for more details.
-
-  You should have received a copy of the GNU Library General Public
-  License along with this library; if not see <http://www.gnu.org/licenses>
-  or write to the Free Software Foundation, Inc.,
-  51 Franklin St., Fifth Floor, Boston, MA 02110, USA
- ******************************************************************************/
-#define MARIADB_CONNECTION
-
-#include "mariadb_python.h"
-#include "docs/module.h"
-#include "docs/exception.h"
-#include <structmember.h>
-#include <datetime.h>
-
-extern int codecs_datetime_init(void);
-
-PyObject *decimal_module= NULL,
-         *decimal_type= NULL,
-         *socket_module= NULL,
-         *indicator_module= NULL;
-extern uint16_t max_pool_size;
-
-int
-Mariadb_traverse(PyObject *self,
-                 visitproc visit,
-                 void *arg)
-{
-    return 0;
-}
-
-static PyMethodDef
-Mariadb_Methods[] =
-{
-    /* PEP-249: mandatory */
-    {"connect", (PyCFunction)MrdbConnection_connect,
-        METH_VARARGS | METH_KEYWORDS,
-        module_connect__doc__},
-    /* Todo: add methods for api functions which don't require
-       a connection */
-    {NULL} /* always last */
-};
-
-/* MariaDB module definition */
-static struct PyModuleDef 
-mariadb_module= {
-    PyModuleDef_HEAD_INIT,
-    "_mariadb",
-    "MariaDB Connector for Python",
-    -1,
-    Mariadb_Methods
-};
-
-static int mariadb_datetime_init(void)
-{
-    PyDateTime_IMPORT;
-
-    if (!PyDateTimeAPI) {
-        PyErr_SetString(PyExc_ImportError, "DateTimeAPI initialization failed");
-        return 1;
-    }
-    return 0;
-}
-
-static void mariadb_add_exception(PyObject *module,
-        PyObject **exception,
-        const char *exception_name,
-        PyObject *base_exception,
-        const char *doc,
-        const char *object_name)
-{
-    *exception= PyErr_NewExceptionWithDoc(exception_name,
-            doc,
-            Mariadb_Error,
-            NULL);
-
-    Py_INCREF(*exception);
-    PyModule_AddObject(module, object_name, *exception);
-}
-
-/* MariaDB module initialization function */
-PyMODINIT_FUNC PyInit__mariadb(void)
-{
-    PyObject *module= PyModule_Create(&mariadb_module);
-
-    /* check if client library is compatible */
-    if (mysql_get_client_version() < MARIADB_PACKAGE_VERSION_ID)
-    {
-      char errmsg[255];
-
-      snprintf(errmsg, 254, "MariaDB Connector/Python was build with MariaDB Connector/C %s, "
-               "while the loaded MariaDB Connector/C library has version %s.",
-               MARIADB_PACKAGE_VERSION, mysql_get_client_info());
-      PyErr_SetString(PyExc_ImportError, errmsg);
-      goto error;
-    }
-
-    /* Initialize DateTimeAPI */
-    if (mariadb_datetime_init() ||
-        codecs_datetime_init())
-    {
-        goto error;
-    }
-
-    Py_SET_TYPE(&MrdbConnection_Type, &PyType_Type);
-    if (PyType_Ready(&MrdbConnection_Type) == -1)
-    {
-        goto error;
-    }
-
-    /* Import Decimal support (CONPY-49) */
-    if (!(decimal_module= PyImport_ImportModule("decimal")) ||
-        !(decimal_type= PyObject_GetAttr(decimal_module, PyUnicode_FromString("Decimal"))))
-    {
-        goto error;
-    }
-
-    if (!(socket_module= PyImport_ImportModule("socket")))
-    {
-        goto error;
-    }
-
-    Py_SET_TYPE(&MrdbCursor_Type, &PyType_Type);
-    if (PyType_Ready(&MrdbCursor_Type) == -1)
-    {
-        goto error;
-    }
-    PyModule_AddObject(module, "cursor", (PyObject *)&MrdbCursor_Type);
-
-    /* optional (MariaDB specific) globals */
-    PyModule_AddObject(module, "mariadbapi_version",
-                       PyUnicode_FromString(mysql_get_client_info()));
-
-    Mariadb_Error= PyErr_NewException("mariadb.Error",
-            PyExc_Exception,
-            NULL);
-    Py_INCREF(Mariadb_Error);
-    PyModule_AddObject(module, "Error", Mariadb_Error);
-
-    mariadb_add_exception(module, &Mariadb_InterfaceError,
-            "mariadb.InterfaceError", Mariadb_Error,
-            exception_interface__doc__, "InterfaceError");
-    mariadb_add_exception(module, &Mariadb_DatabaseError,
-            "mariadb.DatabaseError", Mariadb_Error,
-            exception_database__doc__, "DatabaseError");
-    mariadb_add_exception(module, &Mariadb_OperationalError,
-            "mariadb.OperationalError", Mariadb_Error,
-            exception_operational__doc__, "OperationalError");
-    mariadb_add_exception(module, &Mariadb_Warning,
-            "mariadb.Warning", NULL, exception_warning__doc__, "Warning");
-    mariadb_add_exception(module, &Mariadb_IntegrityError,
-            "mariadb.IntegrityError", Mariadb_Error,
-            exception_integrity__doc__, "IntegrityError");
-    mariadb_add_exception(module, &Mariadb_InternalError,
-            "mariadb.InternalError", Mariadb_Error,
-            exception_internal__doc__, "InternalError");
-    mariadb_add_exception(module, &Mariadb_ProgrammingError,
-            "mariadb.ProgrammingError", Mariadb_Error,
-            exception_programming__doc__, "ProgrammingError");
-    mariadb_add_exception(module, &Mariadb_NotSupportedError,
-            "mariadb.NotSupportedError", Mariadb_Error,
-            exception_notsupported__doc__, "NotSupportedError");
-    mariadb_add_exception(module, &Mariadb_DataError,
-            "mariadb.DataError", Mariadb_DatabaseError,
-            exception_data__doc__, "DataError");
-    mariadb_add_exception(module, &Mariadb_PoolError,
-            "mariadb.PoolError", Mariadb_Error,
-            exception_pool__doc__, "PoolError");
-
-    Py_INCREF(&MrdbConnection_Type);
-    PyModule_AddObject(module, "connection", (PyObject *)&MrdbConnection_Type);
-
-    return module;
-error:
-    if (PyErr_Occurred())
-    {
-        return NULL;
-    }
-    PyErr_SetString(PyExc_ImportError, "Mariadb module initialization failed.");
-    return NULL;
-}
+/******************************************************************************
+  Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
+
+  This library is free software; you can redistribute it and/or
+  modify it under the terms of the GNU Library General Public
+  License as published by the Free Software Foundation; either
+  version 2 of the License, or (at your option) any later version.
+
+  This library is distributed in the hope that it will be useful,
+  but WITHOUT ANY WARRANTY; without even the implied warranty of
+  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+  Library General Public License for more details.
+
+  You should have received a copy of the GNU Library General Public
+  License along with this library; if not see <http://www.gnu.org/licenses>
+  or write to the Free Software Foundation, Inc.,
+  51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+ ******************************************************************************/
+#define MARIADB_CONNECTION
+
+#include "mariadb_python.h"
+#include "docs/module.h"
+#include "docs/exception.h"
+#include <structmember.h>
+#include <datetime.h>
+
+extern int codecs_datetime_init(void);
+
+PyObject *decimal_module= NULL,
+         *decimal_type= NULL,
+         *socket_module= NULL,
+         *indicator_module= NULL;
+extern uint16_t max_pool_size;
+
+int
+Mariadb_traverse(PyObject *self,
+                 visitproc visit,
+                 void *arg)
+{
+    return 0;
+}
+
+static PyMethodDef
+Mariadb_Methods[] =
+{
+    /* PEP-249: mandatory */
+    {"connect", (PyCFunction)MrdbConnection_connect,
+        METH_VARARGS | METH_KEYWORDS,
+        module_connect__doc__},
+    /* Todo: add methods for api functions which don't require
+       a connection */
+    {NULL} /* always last */
+};
+
+/* MariaDB module definition */
+static struct PyModuleDef 
+mariadb_module= {
+    PyModuleDef_HEAD_INIT,
+    "_mariadb",
+    "MariaDB Connector for Python",
+    -1,
+    Mariadb_Methods
+};
+
+static int mariadb_datetime_init(void)
+{
+    PyDateTime_IMPORT;
+
+    if (!PyDateTimeAPI) {
+        PyErr_SetString(PyExc_ImportError, "DateTimeAPI initialization failed");
+        return 1;
+    }
+    return 0;
+}
+
+static void mariadb_add_exception(PyObject *module,
+        PyObject **exception,
+        const char *exception_name,
+        PyObject *base_exception,
+        const char *doc,
+        const char *object_name)
+{
+    *exception= PyErr_NewExceptionWithDoc(exception_name,
+            doc,
+            Mariadb_Error,
+            NULL);
+
+    Py_INCREF(*exception);
+    PyModule_AddObject(module, object_name, *exception);
+}
+
+/* MariaDB module initialization function */
+PyMODINIT_FUNC PyInit__mariadb(void)
+{
+    PyObject *module= PyModule_Create(&mariadb_module);
+
+    /* check if client library is compatible */
+    if (mysql_get_client_version() < MARIADB_PACKAGE_VERSION_ID)
+    {
+      char errmsg[255];
+
+      snprintf(errmsg, 254, "MariaDB Connector/Python was build with MariaDB Connector/C %s, "
+               "while the loaded MariaDB Connector/C library has version %s.",
+               MARIADB_PACKAGE_VERSION, mysql_get_client_info());
+      PyErr_SetString(PyExc_ImportError, errmsg);
+      goto error;
+    }
+
+    /* Initialize DateTimeAPI */
+    if (mariadb_datetime_init() ||
+        codecs_datetime_init())
+    {
+        goto error;
+    }
+
+    Py_SET_TYPE(&MrdbConnection_Type, &PyType_Type);
+    if (PyType_Ready(&MrdbConnection_Type) == -1)
+    {
+        goto error;
+    }
+
+    /* Import Decimal support (CONPY-49) */
+    if (!(decimal_module= PyImport_ImportModule("decimal")) ||
+        !(decimal_type= PyObject_GetAttr(decimal_module, PyUnicode_FromString("Decimal"))))
+    {
+        goto error;
+    }
+
+    if (!(socket_module= PyImport_ImportModule("socket")))
+    {
+        goto error;
+    }
+
+    Py_SET_TYPE(&MrdbCursor_Type, &PyType_Type);
+    if (PyType_Ready(&MrdbCursor_Type) == -1)
+    {
+        goto error;
+    }
+    PyModule_AddObject(module, "cursor", (PyObject *)&MrdbCursor_Type);
+
+    /* optional (MariaDB specific) globals */
+    PyModule_AddObject(module, "mariadbapi_version",
+                       PyUnicode_FromString(mysql_get_client_info()));
+
+    Mariadb_Error= PyErr_NewException("mariadb.Error",
+            PyExc_Exception,
+            NULL);
+    Py_INCREF(Mariadb_Error);
+    PyModule_AddObject(module, "Error", Mariadb_Error);
+
+    mariadb_add_exception(module, &Mariadb_InterfaceError,
+            "mariadb.InterfaceError", Mariadb_Error,
+            exception_interface__doc__, "InterfaceError");
+    mariadb_add_exception(module, &Mariadb_DatabaseError,
+            "mariadb.DatabaseError", Mariadb_Error,
+            exception_database__doc__, "DatabaseError");
+    mariadb_add_exception(module, &Mariadb_OperationalError,
+            "mariadb.OperationalError", Mariadb_Error,
+            exception_operational__doc__, "OperationalError");
+    mariadb_add_exception(module, &Mariadb_Warning,
+            "mariadb.Warning", NULL, exception_warning__doc__, "Warning");
+    mariadb_add_exception(module, &Mariadb_IntegrityError,
+            "mariadb.IntegrityError", Mariadb_Error,
+            exception_integrity__doc__, "IntegrityError");
+    mariadb_add_exception(module, &Mariadb_InternalError,
+            "mariadb.InternalError", Mariadb_Error,
+            exception_internal__doc__, "InternalError");
+    mariadb_add_exception(module, &Mariadb_ProgrammingError,
+            "mariadb.ProgrammingError", Mariadb_Error,
+            exception_programming__doc__, "ProgrammingError");
+    mariadb_add_exception(module, &Mariadb_NotSupportedError,
+            "mariadb.NotSupportedError", Mariadb_Error,
+            exception_notsupported__doc__, "NotSupportedError");
+    mariadb_add_exception(module, &Mariadb_DataError,
+            "mariadb.DataError", Mariadb_DatabaseError,
+            exception_data__doc__, "DataError");
+    mariadb_add_exception(module, &Mariadb_PoolError,
+            "mariadb.PoolError", Mariadb_Error,
+            exception_pool__doc__, "PoolError");
+
+    Py_INCREF(&MrdbConnection_Type);
+    PyModule_AddObject(module, "connection", (PyObject *)&MrdbConnection_Type);
+
+    return module;
+error:
+    if (PyErr_Occurred())
+    {
+        return NULL;
+    }
+    PyErr_SetString(PyExc_ImportError, "Mariadb module initialization failed.");
+    return NULL;
+}
```

### Comparing `mariadb-1.1.6/mariadb/mariadb_codecs.c` & `mariadb-1.1.7/mariadb/mariadb_codecs.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,1487 +1,1497 @@
-/*****************************************************************************
-  Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
-
-  This library is free software; you can redistribute it and/or
-  modify it under the terms of the GNU Library General Public
-  License as published by the Free Software Foundation; either
-  version 2 of the License, or (at your option) any later version.
-
-  This library is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-  Library General Public License for more details.
-
-  You should have received a copy of the GNU Library General Public
-  License along with this library; if not see <http://www.gnu.org/licenses>
-  or write to the Free Software Foundation, Inc.,
-  51 Franklin St., Fifth Floor, Boston, MA 02110, USA
- ****************************************************************************/
-#include "mariadb_python.h"
-#include <datetime.h>
-
-#define CHARSET_BINARY 63
-
-#define IS_DECIMAL_TYPE(type) \
-((type) == MYSQL_TYPE_NEWDECIMAL || (type) == MYSQL_TYPE_DOUBLE || (type) == MYSQL_TYPE_FLOAT)
-
-long MrdbIndicator_AsLong(PyObject *column)
-{
-  PyObject *pyLong= PyObject_GetAttrString(column, "indicator");
-  return PyLong_AsLong(pyLong);
-}
-
-int codecs_datetime_init(void)
-{
-    PyDateTime_IMPORT;
-
-    if (!PyDateTimeAPI) {
-        PyErr_SetString(PyExc_ImportError, "DateTimeAPI initialization failed");
-        return 1;
-    }
-    return 0;
-}
-
-enum enum_extended_field_type mariadb_extended_field_type(const MYSQL_FIELD *field)
-{
-#if MARIADB_PACKAGE_VERSION_ID > 30107
-    MARIADB_CONST_STRING str;
-
-    if (!mariadb_field_attr(&str, field, MARIADB_FIELD_ATTR_FORMAT_NAME))
-    {
-      if (str.length == 4 && !strncmp(str.str, "json", 4))
-          return EXT_TYPE_JSON;
-    }
-#endif
-    return EXT_TYPE_NONE;
-}
-
-/*
-   converts a Python date/time/datetime object to MYSQL_TIME
-*/
-static void
-mariadb_pydate_to_tm(enum enum_field_types type,
-                     PyObject *obj,
-                     MYSQL_TIME *tm)
-{
-    memset(tm, 0, sizeof(MYSQL_TIME));
-    if (type == MYSQL_TYPE_TIME ||
-            type == MYSQL_TYPE_DATETIME)
-    {
-        uint8_t is_time= PyTime_CheckExact(obj);
-        tm->hour= is_time ? PyDateTime_TIME_GET_HOUR(obj) :
-            PyDateTime_DATE_GET_HOUR(obj);
-        tm->minute= is_time ? PyDateTime_TIME_GET_MINUTE(obj) :
-            PyDateTime_DATE_GET_MINUTE(obj);
-        tm->second= is_time ? PyDateTime_TIME_GET_SECOND(obj) :
-            PyDateTime_DATE_GET_SECOND(obj);
-        tm->second_part= is_time ? PyDateTime_TIME_GET_MICROSECOND(obj) :
-            PyDateTime_DATE_GET_MICROSECOND(obj);
-        if (type == MYSQL_TYPE_TIME)
-        {
-            tm->time_type= MYSQL_TIMESTAMP_TIME;
-            return;
-        }
-    }
-    if (type == MYSQL_TYPE_DATE ||
-            type == MYSQL_TYPE_DATETIME)
-    {
-        tm->year= PyDateTime_GET_YEAR(obj);
-        tm->month= PyDateTime_GET_MONTH(obj);
-        tm->day= PyDateTime_GET_DAY(obj);
-        if (type == MYSQL_TYPE_DATE)
-            tm->time_type= MYSQL_TIMESTAMP_DATE;
-        else
-            tm->time_type= MYSQL_TIMESTAMP_DATETIME;
-    }
-}
-
-static void
-mariadb_pydelta_to_tm(PyObject *obj, MYSQL_TIME *tm)
-{
-  int remain= 0, total_seconds= 0;
-
-  memset(tm, 0, sizeof(MYSQL_TIME));
-  tm->second_part= ((PyDateTime_Delta *)obj)->microseconds;
-  tm->neg= ((PyDateTime_Delta *)obj)->days < 0;
-
-  /* todo: there must be a function obj->total_seconds() */
-  total_seconds= abs(((PyDateTime_Delta *)obj)->days * 3600 * 24 + ((PyDateTime_Delta *)obj)->seconds);
-
-  if (tm->second_part && tm->neg)
-  {
-    total_seconds-= 1;
-    tm->second_part= 1000000 - tm->second_part;
-  }
-
-  tm->hour= total_seconds / 3600;
-  remain= total_seconds % 3600;
-  tm->minute= remain / 60;
-  tm->second= remain % 60;
-}
-
-static unsigned long long my_strtoull(const char *str, size_t len, const char **end, int *err)
-{
-  unsigned long long val = 0;
-  const char *p = str;
-  const char *end_str = p + len;
-
-  for (; p < end_str; p++)
-  {
-    if (*p < '0' || *p > '9')
-      break;
-
-    if (val > ULLONG_MAX /10 || val*10 > ULLONG_MAX - (*p - '0'))
-    {
-      *err = ERANGE;
-      break;
-    }
-    val = val * 10 + *p -'0';
-  }
-
-  if (p == str)
-    /* Did not parse anything.*/
-    *err = ERANGE;
-
-  *end = p;
-  return val;
-}
-
-/*
-  strtoui() version, that works for non-null terminated strings
-*/
-static unsigned int my_strtoui(const char *str, size_t len, const char **end, int *err)
-{
-  unsigned long long ull = my_strtoull(str, len, end, err);
-  if (ull > UINT_MAX)
-    *err = ERANGE;
-  return (unsigned int)ull;
-}
-
-/*
-  Parse time, in MySQL format.
-
-  the input string needs is in form "hour:minute:second[.fraction]"
-  hour, minute and second can have leading zeroes or not,
-  they are not necessarily 2 chars.
-
-  Hour must be < 838, minute < 60, second < 60
-  Only 6 places of fraction are considered, the value is truncated after 6 places.
-*/
-static const unsigned int frac_mul[] = { 1000000,100000,10000,1000,100,10 };
-
-static int parse_time(const char *str, size_t length, const char **end_ptr, MYSQL_TIME *tm)
-{
-  int err= 0;
-  const char *p = str;
-  const char *end = str + length;
-  size_t frac_len;
-  int ret=1;
-
-  tm->hour = my_strtoui(p, end-p, &p, &err);
-  if (err || tm->hour > 838 || p == end || *p != ':' )
-    goto end;
-
-  p++;
-  tm->minute = my_strtoui(p, end-p, &p, &err);
-  if (err || tm->minute > 59 || p == end || *p != ':')
-    goto end;
-
-  p++;
-  tm->second = my_strtoui(p, end-p, &p, &err);
-  if (err || tm->second > 59)
-    goto end;
-
-  ret = 0;
-  tm->second_part = 0;
-
-  if (p == end)
-    goto end;
-
-  /* Check for fractional part*/
-  if (*p != '.')
-    goto end;
-
-  p++;
-  frac_len = MIN(6,end-p);
-
-  tm->second_part = my_strtoui(p, frac_len, &p, &err);
-  if (err)
-    goto end;
-
-  if (frac_len < 6)
-    tm->second_part *= frac_mul[frac_len];
-
-  ret = 0;
-
-  /* Consume whole fractional part, even after 6 digits.*/
-  p += frac_len;
-  while(p < *end_ptr)
-  {
-    if (*p < '0' || *p > '9')
-      break;
-    p++;
-  }
-end:
-  *end_ptr = p;
-  return ret;
-}
-
-static uint8_t check_date(uint16_t year, uint8_t month, uint8_t day)
-{
-  uint8_t is_leap= 0;
-
-  if (year < 1 || year > 9999)
-      return 0;
-  if (month < 1 || month > 12)
-      return 0;
-  if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
-      is_leap= 1;
-  if (month == 2)
-  {
-    if (is_leap && day > 29)
-        return 0;
-    if (!is_leap && day > 28)
-        return 0;
-  }
-  if ((month == 4 || month == 6 || month == 9 || month == 11) && day > 30)
-      return 0;
-  return 1;
-}
-
-static uint8_t check_time(MYSQL_TIME *tm)
-{
-  if (tm->hour > 838)
-      return 0;
-  if (tm->minute < 0 || tm->minute > 59)
-      return 0;
-  if (tm->second < 0 || tm->second > 59)
-      return 0;
-  if (tm->second_part < 0 || tm->second_part > 999999)
-      return 0;
-  return 1;
-}
-
-
-/*
-  Parse date, in MySQL format.
-
-  The input string needs is in form "year-month-day"
-  year, month and day can have leading zeroes or not,
-  they do not have fixed length.
-
-  Year must be < 10000, month < 12, day < 32
-
-  Years with 2 digits, are converted to values 1970-2069 according to 
-  usual rules:
-
-  00-69 is converted to 2000-2069.
-  70-99 is converted to 1970-1999.
-*/
-static int parse_date(const char *str, size_t length, const char **end_ptr, MYSQL_TIME *tm)
-{
-  int err = 0;
-  const char *p = str;
-  const char *end = str + length;
-  int ret = 1;
-
-  tm->year = my_strtoui(p, end - p, &p, &err);
-  if (err || tm->year > 9999 || p == end || *p != '-')
-    goto end;
-
-  if (p - str == 2) // 2-digit year
-    tm->year += (tm->year >= 70) ? 1900 : 2000;
-
-  p++;
-  tm->month = my_strtoui(p,end -p, &p, &err);
-  if (err || tm->month > 12 || p == end || *p != '-')
-    goto end;
-
-  p++;
-  tm->day = my_strtoui(p, end -p , &p, &err);
-  if (err || tm->day > 31)
-    goto end;
-
-  ret = 0;
-
-end:
-  *end_ptr = p;
-  return ret;
-}
-
-int Py_str_to_TIME(const char *str, size_t length, MYSQL_TIME *tm)
-{
-  const char *p = str;
-  const char *end = str + length;
-  int is_time = 0;
-
-  if (!p)
-    goto error;
-
-  while (p < end && isspace(*p))
-    p++;
-  while (p < end && isspace(end[-1]))
-    end--;
-
-  if (end -p < 5)
-    goto error;
-
-  if (*p == '-')
-  {
-    tm->neg = 1;
-    /* Only TIME can't be negative.*/
-    is_time = 1;
-    p++;
-  }
-  else
-  {
-    int i;
-    tm->neg = 0;
-    /*
-      Date parsing (in server) accepts leading zeroes, thus position of the delimiters
-      is not fixed. Scan the string to find out what we need to parse.
-    */
-    for (i = 1; p + i < end; i++)
-    {
-      if(p[i] == '-' || p [i] == ':')
-      {
-        is_time = p[i] == ':';
-        break;
-      }
-    }
-  }
-
-  if (is_time)
-  {
-    if (parse_time(p, end - p, &p, tm))
-      goto error;
-    
-    tm->year = tm->month = tm->day = 0;
-    tm->time_type = MYSQL_TIMESTAMP_TIME;
-    return 0;
-  }
-
-  if (parse_date(p, end - p, &p, tm))
-    goto error;
-
-  if (p == end || p[0] != ' ')
-  {
-    tm->hour = tm->minute = tm->second = tm->second_part = 0;
-    tm->time_type = MYSQL_TIMESTAMP_DATE;
-    return 0;
-  }
-
-  /* Skip space. */
-  p++;
-  if (parse_time(p, end - p, &p, tm))
-    goto error;
-
-  /* In DATETIME, hours must be < 24.*/
-  if (tm->hour > 23)
-   goto error;
-
-  tm->time_type = MYSQL_TIMESTAMP_DATETIME;
-  return 0;
-
-error:
-  memset(tm, 0, sizeof(*tm));
-  tm->time_type = MYSQL_TIMESTAMP_ERROR;
-  return 1;
-}
-
-static PyObject *Mrdb_GetTimeDelta(MYSQL_TIME *tm)
-{
-    int days, hour, minute, second, second_part;
- 
-    hour= (tm->neg) ? -1 * tm->hour : tm->hour;
-    minute= (tm->neg) ? -1 * tm->minute : tm->minute;
-    second= (tm->neg) ? -1 * tm->second : tm->second;
-    second_part= (tm->neg) ? -1 * tm->second_part : tm->second_part;
-
-    days= hour / 24;
-    hour= hour % 24;
-    second= hour * 3600 + minute * 60 + second;
-    
-    return PyDelta_FromDSU(days, second, second_part);
-}
-
-static PyObject *ma_convert_value(MrdbCursor *self,
-                                  enum enum_field_types type,
-                                  PyObject *value)
-{
-    PyObject *key= PyLong_FromLongLong(type);
-    PyObject *func;
-    PyObject *new_value= NULL;
-
-    if (!self->connection->converter)
-        return NULL;
-
-    if ((func= PyDict_GetItem(self->connection->converter, key)) &&
-            PyCallable_Check(func))
-    {
-        PyObject *arglist= PyTuple_New(1);
-        PyTuple_SetItem(arglist, 0, value);
-        new_value= PyObject_CallObject(func, arglist);
-    }
-    return new_value;
-}
- 
-void
-field_fetch_fromtext(MrdbCursor *self, char *data, unsigned int column)
-{
-    MYSQL_TIME tm;
-    unsigned long *length;
-    enum enum_extended_field_type ext_type= mariadb_extended_field_type(&self->fields[column]);
-    uint16_t type= self->fields[column].type;
-
-    if (!data)
-      type= MYSQL_TYPE_NULL;
-
-    length= mysql_fetch_lengths(self->result);
-
-    switch (type)
-    {
-        case MYSQL_TYPE_NULL:
-            Py_INCREF(Py_None);
-            self->values[column]= Py_None;
-            break;
-        case MYSQL_TYPE_TINY:
-        case MYSQL_TYPE_SHORT:
-        case MYSQL_TYPE_YEAR:
-        case MYSQL_TYPE_INT24:
-        case MYSQL_TYPE_LONG:
-        case MYSQL_TYPE_LONGLONG:
-            self->values[column]= PyLong_FromString(data, NULL, 0);
-            break;
-        case MYSQL_TYPE_FLOAT:  
-        case MYSQL_TYPE_DOUBLE: 
-        {
-            double d= atof(data);
-            self->values[column]= PyFloat_FromDouble(d);
-            break;
-        }
-        case MYSQL_TYPE_TIME:
-        case MYSQL_TYPE_DATE:
-        case MYSQL_TYPE_DATETIME:
-        case MYSQL_TYPE_TIMESTAMP:
-            memset(&tm, 0, sizeof(MYSQL_TIME));
-            Py_str_to_TIME(data, strlen(data), &tm);
-            if (self->fields[column].type == MYSQL_TYPE_TIME)
-            {
-                if (check_time(&tm))
-                {
-                      self->values[column]= Mrdb_GetTimeDelta(&tm);
-                }
-                else {
-                    Py_INCREF(Py_None);
-                    self->values[column]= Py_None;
-                }
-            } else if (self->fields[column].type == MYSQL_TYPE_DATE)
-            {
-                if (check_date(tm.year, tm.month, tm.day))
-                {
-                    self->values[column]= PyDate_FromDate(tm.year, tm.month, tm.day);
-                }
-                else {
-                    Py_INCREF(Py_None);
-                    self->values[column]= Py_None;
-                }
-            } else 
-            {
-                if (check_date(tm.year, tm.month, tm.day) &&
-                    check_time(&tm))
-                {
-                    self->values[column]= PyDateTime_FromDateAndTime(tm.year, tm.month,
-                               tm.day, tm.hour, tm.minute, tm.second, tm.second_part);
-                }
-                else {
-                    Py_INCREF(Py_None);
-                    self->values[column]= Py_None;
-                }
-            }
-            break;
-        case MYSQL_TYPE_TINY_BLOB:
-        case MYSQL_TYPE_MEDIUM_BLOB:
-        case MYSQL_TYPE_BLOB:
-        case MYSQL_TYPE_LONG_BLOB:
-        case MYSQL_TYPE_GEOMETRY:
-        case MYSQL_TYPE_BIT:
-            if (length[column] > self->fields[column].max_length)
-            {
-                self->fields[column].max_length= length[column];
-            }
-            if (self->fields[column].charsetnr== CHARSET_BINARY &&
-                ext_type != EXT_TYPE_JSON)
-            {
-                self->values[column]= 
-                       PyBytes_FromStringAndSize((const char *)data,
-                                                 (Py_ssize_t)length[column]);
-            }
-            else {
-                self->values[column]= 
-                    PyUnicode_FromStringAndSize((const char *)data, 
-                                                (Py_ssize_t)length[column]);
-            }
-            break;
-        case MYSQL_TYPE_NEWDECIMAL:
-        {
-            PyObject *decimal;
-            decimal= PyObject_CallFunction(decimal_type, "s", (const char *)data);
-            self->values[column]= decimal;
-            break;
-        }
-        case MYSQL_TYPE_STRING:
-        case MYSQL_TYPE_VAR_STRING:
-        case MYSQL_TYPE_JSON:
-        case MYSQL_TYPE_VARCHAR:
-        case MYSQL_TYPE_DECIMAL:
-        case MYSQL_TYPE_SET:
-        case MYSQL_TYPE_ENUM:
-        {
-            unsigned long len;
-            if ( self->fields[column].charsetnr == CHARSET_BINARY)
-            {
-                self->values[column]=
-                        PyBytes_FromStringAndSize((const char *)data,
-                                                       (Py_ssize_t)length[column]);
-                len= (unsigned long)length[column];
-            } else {
-                self->values[column]=
-                    PyUnicode_FromStringAndSize((const char *)data,
-                                                (Py_ssize_t)length[column]);
-                len= (unsigned long)PyUnicode_GET_LENGTH(self->values[column]);
-            }
-            if (len > self->fields[column].max_length)
-            {
-                self->fields[column].max_length= len;
-            }
-            break;
-        }
-        default:
-            break;
-    }
-        /* check if values need to be converted */
-    if (self->connection->converter)
-    {
-        PyObject *val;
-        enum enum_field_types type;
-
-        if (ext_type == EXT_TYPE_JSON)
-          type= MYSQL_TYPE_JSON;
-        else
-          type= self->fields[column].type;
-
-        if ((val= ma_convert_value(self, type, self->values[column])))
-            self->values[column]= val;
-    }
-} 
-
-/* field_fetch_callback
-   This function was previously registered with mysql_stmt_attr_set and
-   STMT_ATTR_FIELD_FETCH_CALLBACK parameter. Instead of filling a bind 
-   buffer MariaDB Connector/C sends raw data in row for the specified column.
-   In case of a NULL value row ptr will be NULL.
-
-   The cursor handle was also previously registered with mysql_stmt_attr_set
-   and STMT_ATTR_USER_DATA parameter and will be passed in data variable.
-*/
-
-void
-field_fetch_callback(void *data, unsigned int column, unsigned char **row)
-{
-    MrdbCursor *self= (MrdbCursor *)data;
-    enum enum_extended_field_type ext_type= mariadb_extended_field_type(&self->fields[column]);
-
-    if (!row)
-    {
-        Py_INCREF(Py_None);
-        self->values[column]= Py_None;
-        return;
-    }
-    switch(self->fields[column].type) {
-        case MYSQL_TYPE_NULL:
-            Py_INCREF(Py_None);
-            self->values[column]= Py_None;
-            break;
-        case MYSQL_TYPE_TINY:
-            self->values[column]= (self->fields[column].flags &
-                 UNSIGNED_FLAG) ?
-                PyLong_FromUnsignedLong((unsigned long)*row[0]) :
-                PyLong_FromLong((long)*row[0]);
-            *row+= 1;
-            break;
-        case MYSQL_TYPE_SHORT:
-        case MYSQL_TYPE_YEAR:
-            self->values[column]=
-                (self->fields[column].flags & UNSIGNED_FLAG) ?
-                PyLong_FromUnsignedLong((unsigned long)uint2korr(*row)) :
-                PyLong_FromLong((long)sint2korr(*row));
-            *row+= 2;
-            break;
-        case MYSQL_TYPE_INT24:
-            self->values[column]= 
-                (self->fields[column].flags & UNSIGNED_FLAG) ?
-                PyLong_FromUnsignedLong((unsigned long)uint3korr(*row)) :
-                PyLong_FromLong((long)sint3korr(*row));
-            *row+= 4;
-            break;
-        case MYSQL_TYPE_LONG:
-            self->values[column]=
-                (self->fields[column].flags & UNSIGNED_FLAG) ?
-                PyLong_FromUnsignedLong((unsigned long)uint4korr(*row)) :
-                PyLong_FromLong((long)sint4korr(*row));
-            *row+= 4;
-            break;
-        case MYSQL_TYPE_LONGLONG:
-            {
-                long long l= sint8korr(*row);
-                self->values[column]=
-                   (self->fields[column].flags & UNSIGNED_FLAG) ?
-                    PyLong_FromUnsignedLongLong((unsigned long long)l) :
-                    PyLong_FromLongLong(l);
-                *row+= 8;
-                break;
-            }
-        case MYSQL_TYPE_FLOAT:
-            {
-                float f;
-                float4get(f, *row);
-                self->values[column]= PyFloat_FromDouble((double)f);
-                *row+= 4;
-                break;
-            }
-        case MYSQL_TYPE_DOUBLE:
-            {
-                double d;
-                float8get(d, *row);
-                self->values[column]= PyFloat_FromDouble(d);
-                *row+= 8;
-                break;
-            }
-        case MYSQL_TYPE_DATETIME:
-        case MYSQL_TYPE_TIMESTAMP:
-            {
-                uint8_t len= 0;
-                int year= 0, month= 0, day= 0,
-                    hour= 0, minute= 0, second= 0, second_part= 0;
-
-                len= (uint8_t)mysql_net_field_length(row);
-                if (!len)
-                {
-                    self->values[column]= PyDateTime_FromDateAndTime(0,0,0,0,0,0,0);
-                    break;
-                }
-                year= uint2korr(*row);
-                month= uint1korr(*row + 2);
-                day= uint1korr(*row + 3);
-                if (len > 4)
-                {
-                    hour= uint1korr(*row + 4);
-                    minute= uint1korr(*row + 5);
-                    second= uint1korr(*row + 6);
-                }
-                if (len == 11)
-                    second_part= uint4korr(*row + 7);
-                self->values[column]= PyDateTime_FromDateAndTime(year, month, 
-                    day, hour, minute, second, second_part);
-                *row+= len;
-                break;
-            }
-        case MYSQL_TYPE_DATE:
-            {
-                uint8_t len= 0;
-                int year, month, day;
-
-                len= (uint8_t)mysql_net_field_length(row);
-
-                if (!len)
-                {
-                    self->values[column]= PyDate_FromDate(0,0,0);
-                    break;
-                }
-                year= uint2korr(*row);
-                month= uint1korr(*row + 2);
-                day= uint1korr(*row + 3);
-                self->values[column]= PyDate_FromDate(year, month, day);
-                *row+= len;
-                break;
-            }
-        case MYSQL_TYPE_TIME:
-            {
-                uint8_t len= 0;
-                MYSQL_TIME tm;
-                memset(&tm, 0, sizeof(MYSQL_TIME));
-
-                len= (uint8_t)mysql_net_field_length(row);
-                if (!len)
-                {
-                    self->values[column]= Mrdb_GetTimeDelta(&tm);
-                    break;
-                }
-                tm.neg= uint1korr(*row);
-                tm.day= uint4korr(*row + 1);
-                tm.hour= uint1korr(*row + 5);
-                tm.minute= uint1korr(*row + 6);
-                tm.second= uint1korr(*row + 7);
-                if (len > 8)
-                    tm.second_part= uint4korr(*row + 8);
-                if (tm.day)
-                    tm.hour+= (tm.day * 24);
-                self->values[column]= Mrdb_GetTimeDelta(&tm);
-                *row+= len;
-                break;
-            }
-        case MYSQL_TYPE_TINY_BLOB:
-        case MYSQL_TYPE_MEDIUM_BLOB:
-        case MYSQL_TYPE_BLOB:
-        case MYSQL_TYPE_LONG_BLOB:
-        case MYSQL_TYPE_BIT:
-            {
-                unsigned long length= mysql_net_field_length(row);
-                if (length > self->fields[column].max_length)
-                    self->fields[column].max_length= length;
-                if (self->fields[column].charsetnr == CHARSET_BINARY &&
-                    ext_type != EXT_TYPE_JSON)
-                {
-                    self->values[column]= 
-                            PyBytes_FromStringAndSize((const char *)*row, 
-                                                       (Py_ssize_t)length);
-                }
-                else {
-                    self->values[column]=
-                        PyUnicode_FromStringAndSize((const char *)*row, 
-                                                    (Py_ssize_t)length);
-                }
-                *row+= length;
-                break;
-            }
-        case MYSQL_TYPE_NEWDECIMAL:
-            {
-                unsigned long length= mysql_net_field_length(row);
-
-                if (length > 0)
-                {
-                    char *tmp= alloca(length + 1);
-                    memcpy(tmp, (const char *)*row, length);
-                    tmp[length]= 0;
-                    self->values[column]= PyObject_CallFunction(decimal_type, "s", tmp);
-                } else {
-                    self->values[column]= PyObject_CallFunction(decimal_type, "s", "0");
-                }
-                *row+= length;
-                break;
-            }
-        case MYSQL_TYPE_GEOMETRY:
-        case MYSQL_TYPE_STRING:
-        case MYSQL_TYPE_VAR_STRING:
-        case MYSQL_TYPE_JSON:
-        case MYSQL_TYPE_VARCHAR:
-        case MYSQL_TYPE_DECIMAL:
-        case MYSQL_TYPE_SET:
-        case MYSQL_TYPE_ENUM:
-        {
-            unsigned long length;
-            unsigned long utf8len;
-            length= mysql_net_field_length(row);
-
-            if ((self->fields[column].flags & BINARY_FLAG ||
-                self->fields[column].charsetnr == CHARSET_BINARY))
-            {
-                self->values[column]=
-                        PyBytes_FromStringAndSize((const char *)*row,
-                                                   (Py_ssize_t)length);
-                if (length > self->fields[column].max_length)
-                    self->fields[column].max_length= length;
-            } else {
-                 self->values[column]= 
-                 PyUnicode_FromStringAndSize((const char *)*row,
-                                             (Py_ssize_t)length);
-                 utf8len= (unsigned long)PyUnicode_GET_LENGTH(self->values[column]);
-                 if (utf8len > self->fields[column].max_length)
-                    self->fields[column].max_length= utf8len;
-            }
-            *row+= length;
-        }
-        default:
-            break;
-    }
-    /* check if values need to be converted */
-    if (self->connection->converter)
-    {
-        PyObject *val;
-        enum enum_field_types type;
-
-        if (ext_type == EXT_TYPE_JSON)
-          type= MYSQL_TYPE_JSON;
-        else
-          type= self->fields[column].type;
-
-        if ((val= ma_convert_value(self, type, self->values[column])))
-            self->values[column]= val;
-    }
-}
-/* 
-   mariadb_get_column_info
-   This function analyzes the Python object and calculates the corresponding
-   MYSQL_TYPE, unsigned flag or NULL values and stores the information in
-   MrdbParamInfo pointer.
- */
-static uint8_t 
-mariadb_get_column_info(PyObject *obj, MrdbParamInfo *paraminfo)
-{
-    if (obj == NULL)
-    {
-        paraminfo->type= MYSQL_TYPE_NULL;
-        return 0;
-    }
-
-    if (CHECK_TYPE(obj, &PyLong_Type))
-    {
-        size_t b= _PyLong_NumBits(obj);
-        if (b > paraminfo->bits)
-            paraminfo->bits= b;
-        paraminfo->type= MYSQL_TYPE_LONGLONG;
-        return 0;
-    } else if (CHECK_TYPE(obj, &PyBool_Type)) {
-        paraminfo->type= MYSQL_TYPE_TINY;
-        return 0;
-    } else if (CHECK_TYPE(obj, &PyFloat_Type)) {
-        paraminfo->type= MYSQL_TYPE_DOUBLE;
-        return 0;
-    } else if (CHECK_TYPE(obj, &PyBytes_Type)) {
-        paraminfo->type= MYSQL_TYPE_LONG_BLOB;
-        return 0;
-    } else if (PyDate_CheckExact(obj)) {
-        paraminfo->type= MYSQL_TYPE_DATE;
-        return 0;
-    } else if (PyTime_CheckExact(obj) ||
-               PyDelta_CheckExact(obj)) {
-        paraminfo->type= MYSQL_TYPE_TIME;
-        return 0;
-    } else if (PyDateTime_CheckExact(obj)) {
-        paraminfo->type= MYSQL_TYPE_DATETIME;
-        return 0;
-   } else if (CHECK_TYPE(obj, &PyUnicode_Type)) {
-        paraminfo->type= MYSQL_TYPE_VAR_STRING;
-        return 0;
-    } else if (obj == Py_None) {
-        paraminfo->type= MYSQL_TYPE_NULL;
-        return 0;
-    } else if (!strcmp(Py_TYPE(obj)->tp_name, "decimal.Decimal") || !strcmp(Py_TYPE(obj)->tp_name, "Decimal")) {
-        /* CONPY-49: C-API has no correspondent data type for DECIMAL column type,
-           so we need to convert decimal.Decimal Object to string during callback */
-        paraminfo->type= MYSQL_TYPE_NEWDECIMAL;
-        return 0;
-    }
-    else {
-        /* If Object has string representation, we will use string representation */ 
-        /* no corresponding object, return error  */
-        return 2;
-    }
-
-    return 1;
-}
-
-static PyObject *ListOrTuple_GetItem(PyObject *obj, Py_ssize_t index)
-{
-    if (CHECK_TYPE(obj, &PyList_Type))
-    {
-        return PyList_GetItem(obj, index);
-    } else if (CHECK_TYPE(obj, &PyTuple_Type))
-    {
-        return PyTuple_GetItem(obj, index);
-    }
-    /* this should never happen, since the type was checked before */
-    return NULL;
-}
-
-/* 
-
-   mariadb_get_parameter()
-   @brief   Returns a bulk parameter which was passed to
-   cursor.executemany() or a parameter which was
-   passed to cursor.execute()
-
-   @param   self[in]         Cursor
-   @param   row_nr[in]       row number
-   @paran   column_nr[in]    column number
-   @param   paran[in][out]   bulk parameter pointer
-
-   @return  0 on success, 1 on error
- */
-static uint8_t 
-mariadb_get_parameter(MrdbCursor *self,
-                      uint8_t is_bulk,
-                      uint32_t row_nr,
-                      uint32_t column_nr,
-                      MrdbParamValue *param)
-{
-    PyObject *row= NULL,
-             *column= NULL;
-    uint8_t rc= 1;
-    long caps;
-
-    mariadb_get_infov(self->connection->mysql,
-                      MARIADB_CONNECTION_EXTENDED_SERVER_CAPABILITIES, &caps);
-
-    if (is_bulk)
-    {
-        /* check if row_nr and column_nr are in the range from
-           0 to (value - 1) */
-        if (row_nr > (self->array_size - 1) ||
-                column_nr > (self->parseinfo.paramcount - 1))
-        {
-            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
-                    "Can't access data at row %d, column %d",
-                     row_nr + 1, column_nr + 1);
-            goto end;
-        }
-
-        if (!(row= ListOrTuple_GetItem(self->data, row_nr)))
-        {
-            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
-                    "Can't access row number %d", row_nr + 1);
-            goto end;
-        }
-    }
-    else
-        row= self->data;
-
-    if (self->parseinfo.paramstyle != PYFORMAT)
-    {
-        if (!(column= ListOrTuple_GetItem(row, column_nr)))
-        {
-            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
-                    "Can't access column number %d at row %d",
-                     column_nr + 1, row_nr + 1);
-            goto end;
-        }
-    } else
-    {
-        PyObject *key;
-
-        key= PyTuple_GetItem(self->parseinfo.keys, column_nr);
-        if (!PyDict_Contains(row, key))
-        {
-            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
-                    "Can't find key in parameter data");
-            goto end;
-        }
-        column= PyDict_GetItem(row, key);
-    }
-
-    /* check if an indicator was passed */
-    if (MrdbIndicator_Check(column))
-    {
-        if (!(caps & (MARIADB_CLIENT_STMT_BULK_OPERATIONS >> 32)))
-        {
-            mariadb_throw_exception(NULL, Mariadb_NotSupportedError, 0,
-                    "MariaDB %s doesn't support indicator variables. "\
-                    "Required version is 10.2.6 or newer",
-                    mysql_get_server_info(self->stmt->mysql));
-            goto end;
-        }
-        param->indicator= (uint8_t)MrdbIndicator_AsLong(column);
-        param->value= NULL; /* you can't have both indicator and value */
-    } else if (column == Py_None) {
-        param->value= NULL;
-        if (caps &
-            (MARIADB_CLIENT_STMT_BULK_OPERATIONS >> 32))
-        {
-            param->indicator= STMT_INDICATOR_NULL;
-        }
-    } 
-    else {
-        param->value= column;
-        param->indicator= STMT_INDICATOR_NONE;
-    }
-    rc= 0;
-end:
-    return rc;
-}
-
-/* 
-   mariadb_get_parameter_info
-   mariadb_get_parameter_info fills the MYSQL_BIND structure
-   with correct field_types for the Python objects.
-
-   In case of a bulk operation (executemany()) we will also optimize
-   the field type (e.g. by checking maxbit size for a PyLong).
-   If the types in this column differ we will return an error.
-*/
-static uint8_t 
-mariadb_get_parameter_info(MrdbCursor *self,
-                           MYSQL_BIND *param,
-                           uint32_t column_nr)
-{
-    uint32_t i, bits= 0;
-    MrdbParamValue paramvalue;
-    MrdbParamInfo pinfo;
-
-    param->is_unsigned= 0;
-    paramvalue.indicator= 0;
-
-    if (!self->array_size)
-    {
-        uint8_t rc;
-        memset(&pinfo, 0, sizeof(MrdbParamInfo));
-        if (mariadb_get_parameter(self, 0, 0, column_nr, &paramvalue))
-            return 1;
-        if ((rc= mariadb_get_column_info(paramvalue.value, &pinfo)))
-        {
-            if (rc == 1)
-            {
-                mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
-                    "Can't retrieve column information for parameter %d",
-                     column_nr);
-            }
-            if (rc == 2)
-            {
-                mariadb_throw_exception(NULL, Mariadb_NotSupportedError, 0,
-                    "Data type '%s' in column %d not supported in MariaDB Connector/Python",
-                     Py_TYPE(paramvalue.value)->tp_name, column_nr);
-            }
-       
-            return 1;
-        }
-        param->buffer_type= pinfo.type;
-        bits= (uint32_t)pinfo.bits;
-    }
-    else for (i=0; i < self->array_size; i++)
-    {
-        if (mariadb_get_parameter(self, 1, i, column_nr, &paramvalue))
-            return 1;
-        memset(&pinfo, 0, sizeof(MrdbParamInfo));
-        if (mariadb_get_column_info(paramvalue.value, &pinfo) && !paramvalue.indicator)
-        {
-            mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
-                    "Invalid parameter type at row %d, column %d",
-                    i+1, column_nr + 1);
-            return 1;
-        }
-
-        if (pinfo.type == MYSQL_TYPE_LONGLONG)
-        {
-            if (pinfo.bits > bits)
-            {
-                bits= (uint32_t)pinfo.bits;
-            }
-        }
-
-        if (!param->buffer_type ||
-                param->buffer_type == MYSQL_TYPE_NULL)
-        {
-            param->buffer_type= pinfo.type;
-        }
-        else {
-            /* except for NULL the parameter types must match */
-            if (param->buffer_type != pinfo.type &&
-                    pinfo.type != MYSQL_TYPE_NULL &&
-                    !paramvalue.indicator)
-            {
-                if ((param->buffer_type == MYSQL_TYPE_TINY ||
-                     param->buffer_type == MYSQL_TYPE_SHORT ||
-                     param->buffer_type == MYSQL_TYPE_LONG) &&
-                        pinfo.type == MYSQL_TYPE_LONGLONG)
-                    break;
-                if (IS_DECIMAL_TYPE(pinfo.type) &&
-                    IS_DECIMAL_TYPE(param->buffer_type))
-                {
-                    param->buffer_type= MYSQL_TYPE_NEWDECIMAL;
-                    break;
-                }
-                mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
-                        "Invalid parameter type at row %d, column %d",
-                        i+1, column_nr + 1);
-                return 1;
-            }
-        }
-    }
-    /* check the bit size for long types and set the appropriate
-       field type */
-    if (param->buffer_type == MYSQL_TYPE_LONGLONG)
-    {
-        if ((bits <= 8 && param->is_unsigned) || bits < 8)
-        {
-            param->buffer_type= MYSQL_TYPE_TINY;
-        }
-        else if ((bits <= 16 && param->is_unsigned) || bits < 16) {
-            param->buffer_type= MYSQL_TYPE_SHORT;
-        }
-        else if ((bits <= 32 && param->is_unsigned) || bits < 32) {
-            param->buffer_type= MYSQL_TYPE_LONG;
-        }
-        else {
-            param->buffer_type= MYSQL_TYPE_LONGLONG;
-        }
-    }
-    return 0;
-}
-
-static Py_ssize_t ListOrTuple_Size(PyObject *obj)
-{
-    if (CHECK_TYPE(obj, &PyList_Type))
-    {
-        return PyList_Size(obj);
-    } else if (CHECK_TYPE(obj, &PyTuple_Type))
-    {
-        return PyTuple_Size(obj);
-    }
-    /* this should never happen, since the type was checked before */
-    return 0;
-}
-
-/* mariadb_check_bulk_parameters
-   This function validates the specified bulk parameters and
-   translates the field types to MYSQL_TYPE_*.
- */
-uint8_t 
-mariadb_check_bulk_parameters(MrdbCursor *self,
-                              PyObject *data)
-{
-    uint32_t i;
-
-    if (!CHECK_TYPE((data), &PyList_Type) &&
-        !CHECK_TYPE(data, &PyTuple_Type))
-    {
-        mariadb_throw_exception(self->stmt, Mariadb_InterfaceError, 1, 
-                "Data must be passed as sequence (Tuple or List)");
-        return 1;
-    }
-
-    if (!(self->array_size= (uint32_t)ListOrTuple_Size(data)))
-    {
-        mariadb_throw_exception(self->stmt, Mariadb_InterfaceError, 1, 
-                "Empty parameter list. At least one row must be specified");
-        return 1;
-    }
-
-    for (i=0; i < self->array_size; i++)
-    {
-        PyObject *obj= ListOrTuple_GetItem(data, i);
-        if (self->parseinfo.paramstyle != PYFORMAT &&
-                (!CHECK_TYPE(obj, &PyTuple_Type) &&
-                 !CHECK_TYPE(obj, &PyList_Type)))
-        {
-            mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
-                    "Invalid parameter type in row %d. "\
-                    " (Row data must be provided as tuple(s))", i+1);
-            return 1;
-        }
-        if (self->parseinfo.paramstyle == PYFORMAT &&
-                !CHECK_TYPE(obj, &PyDict_Type))
-        {
-            mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
-                    "Invalid parameter type in row %d. "\
-                    " (Row data must be provided as dict)", i+1);
-            return 1;
-        }
-
-        if (!self->parseinfo.paramcount ||
-                (self->parseinfo.paramstyle != PYFORMAT && 
-                 self->parseinfo.paramcount != ListOrTuple_Size(obj)))
-        {
-            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 1, 
-                    "Invalid number of parameters in row %d", i+1);
-            return 1;
-        }
-    }
-
-    if (!self->is_prepared &&
-            !(self->params= PyMem_RawCalloc(self->parseinfo.paramcount,
-                                            sizeof(MYSQL_BIND))))
-    {
-        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
-                "Not enough memory (tried to allocated %lld bytes)",
-                self->parseinfo.paramcount * sizeof(MYSQL_BIND));
-        goto error;
-    }
-
-    if (!(self->value= PyMem_RawCalloc(self->parseinfo.paramcount, 
-                                       sizeof(MrdbParamValue))))
-    {
-        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
-                "Not enough memory (tried to allocated %lld bytes)",
-                self->parseinfo.paramcount * sizeof(MrdbParamValue));
-        goto error;
-    }
-
-    for (i=0; i < self->parseinfo.paramcount; i++)
-    {
-        if (mariadb_get_parameter_info(self, &self->params[i], i))
-            goto error;
-    }
-    return 0;
-error:
-    MARIADB_FREE_MEM(self->paraminfo);
-    MARIADB_FREE_MEM(self->value);
-    return 1;
-}
-
-uint8_t
-mariadb_check_execute_parameters(MrdbCursor *self,
-                                 PyObject *data)
-{
-    uint32_t i;
-
-    if (!self->parseinfo.paramcount)
-    {
-        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
-                "Invalid number of parameters");
-        goto error;
-    }
-
-    if (!self->params &&
-            !(self->params= PyMem_RawCalloc(self->parseinfo.paramcount, sizeof(MYSQL_BIND))))
-    {
-        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
-                "Not enough memory (tried to allocated %lld bytes)",
-                self->parseinfo.paramcount * sizeof(MYSQL_BIND));
-        goto error;
-    }
-
-    if (!self->value &&
-       !(self->value= PyMem_RawCalloc(self->parseinfo.paramcount, sizeof(MrdbParamValue))))
-    {
-        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
-                "Not enough memory (tried to allocated %lld bytes)",
-                self->parseinfo.paramcount * sizeof(MrdbParamValue));
-        goto error;
-    }
-
-    for (i=0; i < self->parseinfo.paramcount; i++)
-    {
-        if (mariadb_get_parameter_info(self, &self->params[i], i))
-        {
-            goto error;
-        }
-    }
-    return 0;
-error:
-    MARIADB_FREE_MEM(self->paraminfo);
-    MARIADB_FREE_MEM(self->value);
-    return 1;
-}
-
-/* 
-  mariadb_param_to_bind()
-
-  @brief Set the current value for the specified bind buffer
-
-  @param self       cursor
-  @param bind[in]   bind structure
-  @param value[in]  current column value
-
-  @return 0 on success, otherwise error
- */
-static uint8_t 
-mariadb_param_to_bind(MrdbCursor *self,
-                      MYSQL_BIND *bind,
-                      MrdbParamValue *value)
-{
-    uint8_t rc= 0;
-    uint8_t is_negative= 0;
-
-    if (value->indicator > 0)
-    {
-        bind->u.indicator[0]= value->indicator;
-        goto end;
-    }
-
-    if (!value->value)
-    {
-      bind->buffer_type= MYSQL_TYPE_NULL;
-    } else {
-      if (IS_NUM(bind->buffer_type))
-      {
-          bind->buffer= value->num;
-      }
-
-      if (CHECK_TYPE(value->value, &PyLong_Type))
-      {
-          if (_PyLong_Sign(value->value) < 0)
-              is_negative= 1;
-      }
-    }
-
-    switch(bind->buffer_type)
-    {
-        case MYSQL_TYPE_TINY:
-            if (!is_negative)
-            {
-                if ((value->num[0]= (uint8_t)PyLong_AsUnsignedLong(value->value)) > 0x7F)
-                    bind->is_unsigned= 1;
-            }
-            else {
-                value->num[0]= (int8_t)PyLong_AsLong(value->value);
-            }
-            break;
-        case MYSQL_TYPE_SHORT:
-            if (!is_negative)
-            {
-                if ((*(uint16_t *)&value->num= (uint16_t)PyLong_AsUnsignedLong(value->value)) > 0x7FFF)
-                    bind->is_unsigned= 1;
-            }
-            else {
-                *(int16_t *)&value->num= (int16_t)PyLong_AsLong(value->value);
-            }
-            break;
-        case MYSQL_TYPE_LONG:
-            if (!is_negative)
-            {
-                if ((*(uint32_t *)&value->num= (uint32_t)PyLong_AsUnsignedLong(value->value)) > 0x7FFFFFFF)
-                    bind->is_unsigned= 1;
-            }
-            else {
-                *(int32_t *)&value->num= (int32_t)PyLong_AsLong(value->value);
-            }
-            break;
-        case MYSQL_TYPE_LONGLONG:
-            if (!is_negative)
-            {
-                if ((*(uint64_t *)value->num= (uint64_t)PyLong_AsUnsignedLongLong(value->value)) > 0x7FFFFFFFFFFFFFFF)
-                    bind->is_unsigned= 1;
-            }
-            else {
-                *(int64_t *)value->num= (int64_t)PyLong_AsLongLong(value->value);
-            }
-            break;
-        case MYSQL_TYPE_DOUBLE:
-            *(double *)value->num= (double)PyFloat_AsDouble(value->value);
-            break;
-        case MYSQL_TYPE_LONG_BLOB:
-            bind->buffer_length= (unsigned long)PyBytes_GET_SIZE(value->value);
-            bind->buffer= (void *) PyBytes_AS_STRING(value->value);
-            break;
-        case MYSQL_TYPE_DATE:
-        case MYSQL_TYPE_TIME:
-        case MYSQL_TYPE_DATETIME:
-            bind->buffer= &value->tm;
-            if (PyDelta_CheckExact(value->value))
-                mariadb_pydelta_to_tm(value->value, &value->tm);
-            else
-                mariadb_pydate_to_tm(bind->buffer_type, value->value, &value->tm);
-            break;
-        case MYSQL_TYPE_NEWDECIMAL:
-            {
-                Py_ssize_t len;
-                PyObject *obj= NULL;
-                char *p;
-
-                if (value->free_me)
-                    MARIADB_FREE_MEM(value->buffer);
-                if (!strcmp(Py_TYPE(value->value)->tp_name, "decimal.Decimal") ||
-                    !strcmp(Py_TYPE(value->value)->tp_name, "Decimal"))
-                {
-                    obj= PyObject_Str(value->value);
-                    p= (void *)PyUnicode_AsUTF8AndSize(obj, &len);
-                }
-                else
-                {
-                    obj= PyObject_Str(value->value);
-                    p= (void *)PyUnicode_AsUTF8AndSize(obj, &len);
-                }
-                bind->buffer= value->buffer= PyMem_RawCalloc(1, len);
-                memcpy(value->buffer, p, len);
-                value->free_me= 1;
-                bind->buffer_length= (unsigned long)len;
-                Py_DECREF(obj);
-            }
-            break;
-        case MYSQL_TYPE_VAR_STRING:
-            {
-                Py_ssize_t len;
-
-                bind->buffer= (void *)PyUnicode_AsUTF8AndSize(value->value, &len);
-                bind->buffer_length= (unsigned long)len;
-                break;
-            }
-        case MYSQL_TYPE_NULL:
-            break;
-        default:
-            rc= 1;
-    }
-end:
-    return rc;
-}
-
-/* 
-  mariadb_param_update()
-  @brief   Callback function which updates the bind structure's buffer and
-  length with data from the specified row number. This callback function
-  must be registered via api function mysql_stmt_attr_set
-  with STMT_ATTR_PARAM_CALLBACK option
-
-  @param   data[in]      A pointer to a MrdbCursor object which was passed
-  via mysql_stmt_attr_set before
-  data[in][out] An array of bind structures
-  data[in]      row number
-
-  @return  0 on success, otherwise error (=1)
-*/
-uint8_t
-mariadb_param_update(void *data, MYSQL_BIND *bind, uint32_t row_nr)
-{
-    MrdbCursor *self= (MrdbCursor *)data;
-    uint32_t i;
-    uint8_t rc= 1;
-
-    for (i=0; i < self->parseinfo.paramcount; i++)
-    {
-        if (mariadb_get_parameter(self, (self->array_size > 0), 
-                                 row_nr, i, &self->value[i]))
-        {
-            goto end;
-        }
-        if (self->value[i].indicator)
-        {
-            bind[i].u.indicator= &self->value[i].indicator;
-        }
-        if (self->value[i].indicator < 1)
-        {
-            if (mariadb_param_to_bind(self, &bind[i], &self->value[i]))
-            {
-                goto end;
-            }
-        }
-    }
-    rc= 0;
-end:
-    return rc;
-}
-
-#ifdef _WIN32
-
-/* windows equivalent for clock_gettime.
-   Code based on https://stackoverflow.com/questions/5404277/porting-clock-gettime-to-windows
- */
-
-static uint8_t g_first_time = 1;
-static LARGE_INTEGER g_counts_per_sec;
-
-int clock_gettime(int dummy, struct timespec *ct)
-{
-    LARGE_INTEGER count;
-
-    if (g_first_time)
-    {
-        g_first_time = 0;
-
-        if (0 == QueryPerformanceFrequency(&g_counts_per_sec))
-        {
-            g_counts_per_sec.QuadPart = 0;
-        }
-    }
-
-    if ((NULL == ct) || (g_counts_per_sec.QuadPart <= 0) ||
-            (0 == QueryPerformanceCounter(&count)))
-    {
-        return -1;
-    }
-
-    ct->tv_sec = count.QuadPart / g_counts_per_sec.QuadPart;
-    ct->tv_nsec = (long)(((count.QuadPart % g_counts_per_sec.QuadPart) * 1E09) / g_counts_per_sec.QuadPart);
-
-    return 0;
-}
-
-#endif
+/*****************************************************************************
+  Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
+
+  This library is free software; you can redistribute it and/or
+  modify it under the terms of the GNU Library General Public
+  License as published by the Free Software Foundation; either
+  version 2 of the License, or (at your option) any later version.
+
+  This library is distributed in the hope that it will be useful,
+  but WITHOUT ANY WARRANTY; without even the implied warranty of
+  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+  Library General Public License for more details.
+
+  You should have received a copy of the GNU Library General Public
+  License along with this library; if not see <http://www.gnu.org/licenses>
+  or write to the Free Software Foundation, Inc.,
+  51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+ ****************************************************************************/
+#include "mariadb_python.h"
+#include <datetime.h>
+
+#define CHARSET_BINARY 63
+
+#define IS_DECIMAL_TYPE(type) \
+((type) == MYSQL_TYPE_NEWDECIMAL || (type) == MYSQL_TYPE_DOUBLE || (type) == MYSQL_TYPE_FLOAT)
+
+long MrdbIndicator_AsLong(PyObject *column)
+{
+  PyObject *pyLong= PyObject_GetAttrString(column, "indicator");
+  return PyLong_AsLong(pyLong);
+}
+
+int codecs_datetime_init(void)
+{
+    PyDateTime_IMPORT;
+
+    if (!PyDateTimeAPI) {
+        PyErr_SetString(PyExc_ImportError, "DateTimeAPI initialization failed");
+        return 1;
+    }
+    return 0;
+}
+
+enum enum_extended_field_type mariadb_extended_field_type(const MYSQL_FIELD *field)
+{
+#if MARIADB_PACKAGE_VERSION_ID > 30107
+    MARIADB_CONST_STRING str;
+
+    if (!mariadb_field_attr(&str, field, MARIADB_FIELD_ATTR_FORMAT_NAME))
+    {
+      if (str.length == 4 && !strncmp(str.str, "json", 4))
+          return EXT_TYPE_JSON;
+    }
+#endif
+    return EXT_TYPE_NONE;
+}
+
+/*
+   converts a Python date/time/datetime object to MYSQL_TIME
+*/
+static void
+mariadb_pydate_to_tm(enum enum_field_types type,
+                     PyObject *obj,
+                     MYSQL_TIME *tm)
+{
+    memset(tm, 0, sizeof(MYSQL_TIME));
+    if (type == MYSQL_TYPE_TIME ||
+            type == MYSQL_TYPE_DATETIME)
+    {
+        uint8_t is_time= PyTime_CheckExact(obj);
+        tm->hour= is_time ? PyDateTime_TIME_GET_HOUR(obj) :
+            PyDateTime_DATE_GET_HOUR(obj);
+        tm->minute= is_time ? PyDateTime_TIME_GET_MINUTE(obj) :
+            PyDateTime_DATE_GET_MINUTE(obj);
+        tm->second= is_time ? PyDateTime_TIME_GET_SECOND(obj) :
+            PyDateTime_DATE_GET_SECOND(obj);
+        tm->second_part= is_time ? PyDateTime_TIME_GET_MICROSECOND(obj) :
+            PyDateTime_DATE_GET_MICROSECOND(obj);
+        if (type == MYSQL_TYPE_TIME)
+        {
+            tm->time_type= MYSQL_TIMESTAMP_TIME;
+            return;
+        }
+    }
+    if (type == MYSQL_TYPE_DATE ||
+            type == MYSQL_TYPE_DATETIME)
+    {
+        tm->year= PyDateTime_GET_YEAR(obj);
+        tm->month= PyDateTime_GET_MONTH(obj);
+        tm->day= PyDateTime_GET_DAY(obj);
+        if (type == MYSQL_TYPE_DATE)
+            tm->time_type= MYSQL_TIMESTAMP_DATE;
+        else
+            tm->time_type= MYSQL_TIMESTAMP_DATETIME;
+    }
+}
+
+static void
+mariadb_pydelta_to_tm(PyObject *obj, MYSQL_TIME *tm)
+{
+  int remain= 0, total_seconds= 0;
+
+  memset(tm, 0, sizeof(MYSQL_TIME));
+  tm->second_part= ((PyDateTime_Delta *)obj)->microseconds;
+  tm->neg= ((PyDateTime_Delta *)obj)->days < 0;
+
+  /* todo: there must be a function obj->total_seconds() */
+  total_seconds= abs(((PyDateTime_Delta *)obj)->days * 3600 * 24 + ((PyDateTime_Delta *)obj)->seconds);
+
+  if (tm->second_part && tm->neg)
+  {
+    total_seconds-= 1;
+    tm->second_part= 1000000 - tm->second_part;
+  }
+
+  tm->hour= total_seconds / 3600;
+  remain= total_seconds % 3600;
+  tm->minute= remain / 60;
+  tm->second= remain % 60;
+}
+
+static unsigned long long my_strtoull(const char *str, size_t len, const char **end, int *err)
+{
+  unsigned long long val = 0;
+  const char *p = str;
+  const char *end_str = p + len;
+
+  for (; p < end_str; p++)
+  {
+    if (*p < '0' || *p > '9')
+      break;
+
+    if (val > ULLONG_MAX /10 || val*10 > ULLONG_MAX - (*p - '0'))
+    {
+      *err = ERANGE;
+      break;
+    }
+    val = val * 10 + *p -'0';
+  }
+
+  if (p == str)
+    /* Did not parse anything.*/
+    *err = ERANGE;
+
+  *end = p;
+  return val;
+}
+
+/*
+  strtoui() version, that works for non-null terminated strings
+*/
+static unsigned int my_strtoui(const char *str, size_t len, const char **end, int *err)
+{
+  unsigned long long ull = my_strtoull(str, len, end, err);
+  if (ull > UINT_MAX)
+    *err = ERANGE;
+  return (unsigned int)ull;
+}
+
+/*
+  Parse time, in MySQL format.
+
+  the input string needs is in form "hour:minute:second[.fraction]"
+  hour, minute and second can have leading zeroes or not,
+  they are not necessarily 2 chars.
+
+  Hour must be < 838, minute < 60, second < 60
+  Only 6 places of fraction are considered, the value is truncated after 6 places.
+*/
+static const unsigned int frac_mul[] = { 1000000,100000,10000,1000,100,10 };
+
+static int parse_time(const char *str, size_t length, const char **end_ptr, MYSQL_TIME *tm)
+{
+  int err= 0;
+  const char *p = str;
+  const char *end = str + length;
+  size_t frac_len;
+  int ret=1;
+
+  tm->hour = my_strtoui(p, end-p, &p, &err);
+  if (err || tm->hour > 838 || p == end || *p != ':' )
+    goto end;
+
+  p++;
+  tm->minute = my_strtoui(p, end-p, &p, &err);
+  if (err || tm->minute > 59 || p == end || *p != ':')
+    goto end;
+
+  p++;
+  tm->second = my_strtoui(p, end-p, &p, &err);
+  if (err || tm->second > 59)
+    goto end;
+
+  ret = 0;
+  tm->second_part = 0;
+
+  if (p == end)
+    goto end;
+
+  /* Check for fractional part*/
+  if (*p != '.')
+    goto end;
+
+  p++;
+  frac_len = MIN(6,end-p);
+
+  tm->second_part = my_strtoui(p, frac_len, &p, &err);
+  if (err)
+    goto end;
+
+  if (frac_len < 6)
+    tm->second_part *= frac_mul[frac_len];
+
+  ret = 0;
+
+  /* Consume whole fractional part, even after 6 digits.*/
+  p += frac_len;
+  while(p < *end_ptr)
+  {
+    if (*p < '0' || *p > '9')
+      break;
+    p++;
+  }
+end:
+  *end_ptr = p;
+  return ret;
+}
+
+static uint8_t check_date(uint16_t year, uint8_t month, uint8_t day)
+{
+  uint8_t is_leap= 0;
+
+  if (year < 1 || year > 9999)
+      return 0;
+  if (month < 1 || month > 12)
+      return 0;
+  if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
+      is_leap= 1;
+  if (month == 2)
+  {
+    if (is_leap && day > 29)
+        return 0;
+    if (!is_leap && day > 28)
+        return 0;
+  }
+  if ((month == 4 || month == 6 || month == 9 || month == 11) && day > 30)
+      return 0;
+  return 1;
+}
+
+static uint8_t check_time(MYSQL_TIME *tm)
+{
+  if (tm->hour > 838)
+      return 0;
+  if (tm->minute < 0 || tm->minute > 59)
+      return 0;
+  if (tm->second < 0 || tm->second > 59)
+      return 0;
+  if (tm->second_part < 0 || tm->second_part > 999999)
+      return 0;
+  return 1;
+}
+
+
+/*
+  Parse date, in MySQL format.
+
+  The input string needs is in form "year-month-day"
+  year, month and day can have leading zeroes or not,
+  they do not have fixed length.
+
+  Year must be < 10000, month < 12, day < 32
+
+  Years with 2 digits, are converted to values 1970-2069 according to 
+  usual rules:
+
+  00-69 is converted to 2000-2069.
+  70-99 is converted to 1970-1999.
+*/
+static int parse_date(const char *str, size_t length, const char **end_ptr, MYSQL_TIME *tm)
+{
+  int err = 0;
+  const char *p = str;
+  const char *end = str + length;
+  int ret = 1;
+
+  tm->year = my_strtoui(p, end - p, &p, &err);
+  if (err || tm->year > 9999 || p == end || *p != '-')
+    goto end;
+
+  if (p - str == 2) // 2-digit year
+    tm->year += (tm->year >= 70) ? 1900 : 2000;
+
+  p++;
+  tm->month = my_strtoui(p,end -p, &p, &err);
+  if (err || tm->month > 12 || p == end || *p != '-')
+    goto end;
+
+  p++;
+  tm->day = my_strtoui(p, end -p , &p, &err);
+  if (err || tm->day > 31)
+    goto end;
+
+  ret = 0;
+
+end:
+  *end_ptr = p;
+  return ret;
+}
+
+int Py_str_to_TIME(const char *str, size_t length, MYSQL_TIME *tm)
+{
+  const char *p = str;
+  const char *end = str + length;
+  int is_time = 0;
+
+  if (!p)
+    goto error;
+
+  while (p < end && isspace(*p))
+    p++;
+  while (p < end && isspace(end[-1]))
+    end--;
+
+  if (end -p < 5)
+    goto error;
+
+  if (*p == '-')
+  {
+    tm->neg = 1;
+    /* Only TIME can't be negative.*/
+    is_time = 1;
+    p++;
+  }
+  else
+  {
+    int i;
+    tm->neg = 0;
+    /*
+      Date parsing (in server) accepts leading zeroes, thus position of the delimiters
+      is not fixed. Scan the string to find out what we need to parse.
+    */
+    for (i = 1; p + i < end; i++)
+    {
+      if(p[i] == '-' || p [i] == ':')
+      {
+        is_time = p[i] == ':';
+        break;
+      }
+    }
+  }
+
+  if (is_time)
+  {
+    if (parse_time(p, end - p, &p, tm))
+      goto error;
+    
+    tm->year = tm->month = tm->day = 0;
+    tm->time_type = MYSQL_TIMESTAMP_TIME;
+    return 0;
+  }
+
+  if (parse_date(p, end - p, &p, tm))
+    goto error;
+
+  if (p == end || p[0] != ' ')
+  {
+    tm->hour = tm->minute = tm->second = tm->second_part = 0;
+    tm->time_type = MYSQL_TIMESTAMP_DATE;
+    return 0;
+  }
+
+  /* Skip space. */
+  p++;
+  if (parse_time(p, end - p, &p, tm))
+    goto error;
+
+  /* In DATETIME, hours must be < 24.*/
+  if (tm->hour > 23)
+   goto error;
+
+  tm->time_type = MYSQL_TIMESTAMP_DATETIME;
+  return 0;
+
+error:
+  memset(tm, 0, sizeof(*tm));
+  tm->time_type = MYSQL_TIMESTAMP_ERROR;
+  return 1;
+}
+
+static PyObject *Mrdb_GetTimeDelta(MYSQL_TIME *tm)
+{
+    int days, hour, minute, second, second_part;
+ 
+    hour= (tm->neg) ? -1 * tm->hour : tm->hour;
+    minute= (tm->neg) ? -1 * tm->minute : tm->minute;
+    second= (tm->neg) ? -1 * tm->second : tm->second;
+    second_part= (tm->neg) ? -1 * tm->second_part : tm->second_part;
+
+    days= hour / 24;
+    hour= hour % 24;
+    second= hour * 3600 + minute * 60 + second;
+    
+    return PyDelta_FromDSU(days, second, second_part);
+}
+
+static PyObject *ma_convert_value(MrdbCursor *self,
+                                  enum enum_field_types type,
+                                  PyObject *value)
+{
+    PyObject *key= PyLong_FromLongLong(type);
+    PyObject *func;
+    PyObject *new_value= NULL;
+
+    if (!self->connection->converter)
+        return NULL;
+
+    if ((func= PyDict_GetItem(self->connection->converter, key)) &&
+            PyCallable_Check(func))
+    {
+        PyObject *arglist= PyTuple_New(1);
+        PyTuple_SetItem(arglist, 0, value);
+        new_value= PyObject_CallObject(func, arglist);
+    }
+    return new_value;
+}
+ 
+void
+field_fetch_fromtext(MrdbCursor *self, char *data, unsigned int column)
+{
+    MYSQL_TIME tm;
+    unsigned long *length;
+    enum enum_extended_field_type ext_type= mariadb_extended_field_type(&self->fields[column]);
+    uint16_t type= self->fields[column].type;
+
+    if (!data)
+      type= MYSQL_TYPE_NULL;
+
+    length= mysql_fetch_lengths(self->result);
+
+    switch (type)
+    {
+        case MYSQL_TYPE_NULL:
+            Py_INCREF(Py_None);
+            self->values[column]= Py_None;
+            break;
+        case MYSQL_TYPE_TINY:
+        case MYSQL_TYPE_SHORT:
+        case MYSQL_TYPE_YEAR:
+        case MYSQL_TYPE_INT24:
+        case MYSQL_TYPE_LONG:
+        case MYSQL_TYPE_LONGLONG:
+        {
+            char *p= data;
+
+            /* CONPY-258: remove leading zero's */
+            if (strlen(p) > 1)
+            {
+                while (*p && *p == '0')
+                p++;
+            }
+            self->values[column]= PyLong_FromString(p, NULL, 0);
+            break;
+        }
+        case MYSQL_TYPE_FLOAT:  
+        case MYSQL_TYPE_DOUBLE: 
+        {
+            double d= atof(data);
+            self->values[column]= PyFloat_FromDouble(d);
+            break;
+        }
+        case MYSQL_TYPE_TIME:
+        case MYSQL_TYPE_DATE:
+        case MYSQL_TYPE_DATETIME:
+        case MYSQL_TYPE_TIMESTAMP:
+            memset(&tm, 0, sizeof(MYSQL_TIME));
+            Py_str_to_TIME(data, strlen(data), &tm);
+            if (self->fields[column].type == MYSQL_TYPE_TIME)
+            {
+                if (check_time(&tm))
+                {
+                      self->values[column]= Mrdb_GetTimeDelta(&tm);
+                }
+                else {
+                    Py_INCREF(Py_None);
+                    self->values[column]= Py_None;
+                }
+            } else if (self->fields[column].type == MYSQL_TYPE_DATE)
+            {
+                if (check_date(tm.year, tm.month, tm.day))
+                {
+                    self->values[column]= PyDate_FromDate(tm.year, tm.month, tm.day);
+                }
+                else {
+                    Py_INCREF(Py_None);
+                    self->values[column]= Py_None;
+                }
+            } else 
+            {
+                if (check_date(tm.year, tm.month, tm.day) &&
+                    check_time(&tm))
+                {
+                    self->values[column]= PyDateTime_FromDateAndTime(tm.year, tm.month,
+                               tm.day, tm.hour, tm.minute, tm.second, tm.second_part);
+                }
+                else {
+                    Py_INCREF(Py_None);
+                    self->values[column]= Py_None;
+                }
+            }
+            break;
+        case MYSQL_TYPE_TINY_BLOB:
+        case MYSQL_TYPE_MEDIUM_BLOB:
+        case MYSQL_TYPE_BLOB:
+        case MYSQL_TYPE_LONG_BLOB:
+        case MYSQL_TYPE_GEOMETRY:
+        case MYSQL_TYPE_BIT:
+            if (length[column] > self->fields[column].max_length)
+            {
+                self->fields[column].max_length= length[column];
+            }
+            if (self->fields[column].charsetnr== CHARSET_BINARY &&
+                ext_type != EXT_TYPE_JSON)
+            {
+                self->values[column]= 
+                       PyBytes_FromStringAndSize((const char *)data,
+                                                 (Py_ssize_t)length[column]);
+            }
+            else {
+                self->values[column]= 
+                    PyUnicode_FromStringAndSize((const char *)data, 
+                                                (Py_ssize_t)length[column]);
+            }
+            break;
+        case MYSQL_TYPE_NEWDECIMAL:
+        {
+            PyObject *decimal;
+            decimal= PyObject_CallFunction(decimal_type, "s", (const char *)data);
+            self->values[column]= decimal;
+            break;
+        }
+        case MYSQL_TYPE_STRING:
+        case MYSQL_TYPE_VAR_STRING:
+        case MYSQL_TYPE_JSON:
+        case MYSQL_TYPE_VARCHAR:
+        case MYSQL_TYPE_DECIMAL:
+        case MYSQL_TYPE_SET:
+        case MYSQL_TYPE_ENUM:
+        {
+            unsigned long len;
+            if ( self->fields[column].charsetnr == CHARSET_BINARY)
+            {
+                self->values[column]=
+                        PyBytes_FromStringAndSize((const char *)data,
+                                                       (Py_ssize_t)length[column]);
+                len= (unsigned long)length[column];
+            } else {
+                self->values[column]=
+                    PyUnicode_FromStringAndSize((const char *)data,
+                                                (Py_ssize_t)length[column]);
+                len= (unsigned long)PyUnicode_GET_LENGTH(self->values[column]);
+            }
+            if (len > self->fields[column].max_length)
+            {
+                self->fields[column].max_length= len;
+            }
+            break;
+        }
+        default:
+            break;
+    }
+        /* check if values need to be converted */
+    if (self->connection->converter)
+    {
+        PyObject *val;
+        enum enum_field_types type;
+
+        if (ext_type == EXT_TYPE_JSON)
+          type= MYSQL_TYPE_JSON;
+        else
+          type= self->fields[column].type;
+
+        if ((val= ma_convert_value(self, type, self->values[column])))
+            self->values[column]= val;
+    }
+} 
+
+/* field_fetch_callback
+   This function was previously registered with mysql_stmt_attr_set and
+   STMT_ATTR_FIELD_FETCH_CALLBACK parameter. Instead of filling a bind 
+   buffer MariaDB Connector/C sends raw data in row for the specified column.
+   In case of a NULL value row ptr will be NULL.
+
+   The cursor handle was also previously registered with mysql_stmt_attr_set
+   and STMT_ATTR_USER_DATA parameter and will be passed in data variable.
+*/
+
+void
+field_fetch_callback(void *data, unsigned int column, unsigned char **row)
+{
+    MrdbCursor *self= (MrdbCursor *)data;
+    enum enum_extended_field_type ext_type= mariadb_extended_field_type(&self->fields[column]);
+
+    if (!row)
+    {
+        Py_INCREF(Py_None);
+        self->values[column]= Py_None;
+        return;
+    }
+    switch(self->fields[column].type) {
+        case MYSQL_TYPE_NULL:
+            Py_INCREF(Py_None);
+            self->values[column]= Py_None;
+            break;
+        case MYSQL_TYPE_TINY:
+            self->values[column]= (self->fields[column].flags &
+                 UNSIGNED_FLAG) ?
+                PyLong_FromUnsignedLong((unsigned long)*row[0]) :
+                PyLong_FromLong((long)*row[0]);
+            *row+= 1;
+            break;
+        case MYSQL_TYPE_SHORT:
+        case MYSQL_TYPE_YEAR:
+            self->values[column]=
+                (self->fields[column].flags & UNSIGNED_FLAG) ?
+                PyLong_FromUnsignedLong((unsigned long)uint2korr(*row)) :
+                PyLong_FromLong((long)sint2korr(*row));
+            *row+= 2;
+            break;
+        case MYSQL_TYPE_INT24:
+            self->values[column]= 
+                (self->fields[column].flags & UNSIGNED_FLAG) ?
+                PyLong_FromUnsignedLong((unsigned long)uint3korr(*row)) :
+                PyLong_FromLong((long)sint3korr(*row));
+            *row+= 4;
+            break;
+        case MYSQL_TYPE_LONG:
+            self->values[column]=
+                (self->fields[column].flags & UNSIGNED_FLAG) ?
+                PyLong_FromUnsignedLong((unsigned long)uint4korr(*row)) :
+                PyLong_FromLong((long)sint4korr(*row));
+            *row+= 4;
+            break;
+        case MYSQL_TYPE_LONGLONG:
+            {
+                long long l= sint8korr(*row);
+                self->values[column]=
+                   (self->fields[column].flags & UNSIGNED_FLAG) ?
+                    PyLong_FromUnsignedLongLong((unsigned long long)l) :
+                    PyLong_FromLongLong(l);
+                *row+= 8;
+                break;
+            }
+        case MYSQL_TYPE_FLOAT:
+            {
+                float f;
+                float4get(f, *row);
+                self->values[column]= PyFloat_FromDouble((double)f);
+                *row+= 4;
+                break;
+            }
+        case MYSQL_TYPE_DOUBLE:
+            {
+                double d;
+                float8get(d, *row);
+                self->values[column]= PyFloat_FromDouble(d);
+                *row+= 8;
+                break;
+            }
+        case MYSQL_TYPE_DATETIME:
+        case MYSQL_TYPE_TIMESTAMP:
+            {
+                uint8_t len= 0;
+                int year= 0, month= 0, day= 0,
+                    hour= 0, minute= 0, second= 0, second_part= 0;
+
+                len= (uint8_t)mysql_net_field_length(row);
+                if (!len)
+                {
+                    self->values[column]= PyDateTime_FromDateAndTime(0,0,0,0,0,0,0);
+                    break;
+                }
+                year= uint2korr(*row);
+                month= uint1korr(*row + 2);
+                day= uint1korr(*row + 3);
+                if (len > 4)
+                {
+                    hour= uint1korr(*row + 4);
+                    minute= uint1korr(*row + 5);
+                    second= uint1korr(*row + 6);
+                }
+                if (len == 11)
+                    second_part= uint4korr(*row + 7);
+                self->values[column]= PyDateTime_FromDateAndTime(year, month, 
+                    day, hour, minute, second, second_part);
+                *row+= len;
+                break;
+            }
+        case MYSQL_TYPE_DATE:
+            {
+                uint8_t len= 0;
+                int year, month, day;
+
+                len= (uint8_t)mysql_net_field_length(row);
+
+                if (!len)
+                {
+                    self->values[column]= PyDate_FromDate(0,0,0);
+                    break;
+                }
+                year= uint2korr(*row);
+                month= uint1korr(*row + 2);
+                day= uint1korr(*row + 3);
+                self->values[column]= PyDate_FromDate(year, month, day);
+                *row+= len;
+                break;
+            }
+        case MYSQL_TYPE_TIME:
+            {
+                uint8_t len= 0;
+                MYSQL_TIME tm;
+                memset(&tm, 0, sizeof(MYSQL_TIME));
+
+                len= (uint8_t)mysql_net_field_length(row);
+                if (!len)
+                {
+                    self->values[column]= Mrdb_GetTimeDelta(&tm);
+                    break;
+                }
+                tm.neg= uint1korr(*row);
+                tm.day= uint4korr(*row + 1);
+                tm.hour= uint1korr(*row + 5);
+                tm.minute= uint1korr(*row + 6);
+                tm.second= uint1korr(*row + 7);
+                if (len > 8)
+                    tm.second_part= uint4korr(*row + 8);
+                if (tm.day)
+                    tm.hour+= (tm.day * 24);
+                self->values[column]= Mrdb_GetTimeDelta(&tm);
+                *row+= len;
+                break;
+            }
+        case MYSQL_TYPE_TINY_BLOB:
+        case MYSQL_TYPE_MEDIUM_BLOB:
+        case MYSQL_TYPE_BLOB:
+        case MYSQL_TYPE_LONG_BLOB:
+        case MYSQL_TYPE_BIT:
+            {
+                unsigned long length= mysql_net_field_length(row);
+                if (length > self->fields[column].max_length)
+                    self->fields[column].max_length= length;
+                if (self->fields[column].charsetnr == CHARSET_BINARY &&
+                    ext_type != EXT_TYPE_JSON)
+                {
+                    self->values[column]= 
+                            PyBytes_FromStringAndSize((const char *)*row, 
+                                                       (Py_ssize_t)length);
+                }
+                else {
+                    self->values[column]=
+                        PyUnicode_FromStringAndSize((const char *)*row, 
+                                                    (Py_ssize_t)length);
+                }
+                *row+= length;
+                break;
+            }
+        case MYSQL_TYPE_NEWDECIMAL:
+            {
+                unsigned long length= mysql_net_field_length(row);
+
+                if (length > 0)
+                {
+                    char *tmp= alloca(length + 1);
+                    memcpy(tmp, (const char *)*row, length);
+                    tmp[length]= 0;
+                    self->values[column]= PyObject_CallFunction(decimal_type, "s", tmp);
+                } else {
+                    self->values[column]= PyObject_CallFunction(decimal_type, "s", "0");
+                }
+                *row+= length;
+                break;
+            }
+        case MYSQL_TYPE_GEOMETRY:
+        case MYSQL_TYPE_STRING:
+        case MYSQL_TYPE_VAR_STRING:
+        case MYSQL_TYPE_JSON:
+        case MYSQL_TYPE_VARCHAR:
+        case MYSQL_TYPE_DECIMAL:
+        case MYSQL_TYPE_SET:
+        case MYSQL_TYPE_ENUM:
+        {
+            unsigned long length;
+            unsigned long utf8len;
+            length= mysql_net_field_length(row);
+
+            if ((self->fields[column].flags & BINARY_FLAG ||
+                self->fields[column].charsetnr == CHARSET_BINARY))
+            {
+                self->values[column]=
+                        PyBytes_FromStringAndSize((const char *)*row,
+                                                   (Py_ssize_t)length);
+                if (length > self->fields[column].max_length)
+                    self->fields[column].max_length= length;
+            } else {
+                 self->values[column]= 
+                 PyUnicode_FromStringAndSize((const char *)*row,
+                                             (Py_ssize_t)length);
+                 utf8len= (unsigned long)PyUnicode_GET_LENGTH(self->values[column]);
+                 if (utf8len > self->fields[column].max_length)
+                    self->fields[column].max_length= utf8len;
+            }
+            *row+= length;
+        }
+        default:
+            break;
+    }
+    /* check if values need to be converted */
+    if (self->connection->converter)
+    {
+        PyObject *val;
+        enum enum_field_types type;
+
+        if (ext_type == EXT_TYPE_JSON)
+          type= MYSQL_TYPE_JSON;
+        else
+          type= self->fields[column].type;
+
+        if ((val= ma_convert_value(self, type, self->values[column])))
+            self->values[column]= val;
+    }
+}
+/* 
+   mariadb_get_column_info
+   This function analyzes the Python object and calculates the corresponding
+   MYSQL_TYPE, unsigned flag or NULL values and stores the information in
+   MrdbParamInfo pointer.
+ */
+static uint8_t 
+mariadb_get_column_info(PyObject *obj, MrdbParamInfo *paraminfo)
+{
+    if (obj == NULL)
+    {
+        paraminfo->type= MYSQL_TYPE_NULL;
+        return 0;
+    }
+
+    if (CHECK_TYPE(obj, &PyLong_Type))
+    {
+        size_t b= _PyLong_NumBits(obj);
+        if (b > paraminfo->bits)
+            paraminfo->bits= b;
+        paraminfo->type= MYSQL_TYPE_LONGLONG;
+        return 0;
+    } else if (CHECK_TYPE(obj, &PyBool_Type)) {
+        paraminfo->type= MYSQL_TYPE_TINY;
+        return 0;
+    } else if (CHECK_TYPE(obj, &PyFloat_Type)) {
+        paraminfo->type= MYSQL_TYPE_DOUBLE;
+        return 0;
+    } else if (CHECK_TYPE(obj, &PyBytes_Type)) {
+        paraminfo->type= MYSQL_TYPE_LONG_BLOB;
+        return 0;
+    } else if (PyDate_CheckExact(obj)) {
+        paraminfo->type= MYSQL_TYPE_DATE;
+        return 0;
+    } else if (PyTime_CheckExact(obj) ||
+               PyDelta_CheckExact(obj)) {
+        paraminfo->type= MYSQL_TYPE_TIME;
+        return 0;
+    } else if (PyDateTime_CheckExact(obj)) {
+        paraminfo->type= MYSQL_TYPE_DATETIME;
+        return 0;
+   } else if (CHECK_TYPE(obj, &PyUnicode_Type)) {
+        paraminfo->type= MYSQL_TYPE_VAR_STRING;
+        return 0;
+    } else if (obj == Py_None) {
+        paraminfo->type= MYSQL_TYPE_NULL;
+        return 0;
+    } else if (!strcmp(Py_TYPE(obj)->tp_name, "decimal.Decimal") || !strcmp(Py_TYPE(obj)->tp_name, "Decimal")) {
+        /* CONPY-49: C-API has no correspondent data type for DECIMAL column type,
+           so we need to convert decimal.Decimal Object to string during callback */
+        paraminfo->type= MYSQL_TYPE_NEWDECIMAL;
+        return 0;
+    }
+    else {
+        /* If Object has string representation, we will use string representation */ 
+        /* no corresponding object, return error  */
+        return 2;
+    }
+
+    return 1;
+}
+
+PyObject *ListOrTuple_GetItem(PyObject *obj, Py_ssize_t index)
+{
+    if (CHECK_TYPE(obj, &PyList_Type))
+    {
+        return PyList_GetItem(obj, index);
+    } else if (CHECK_TYPE(obj, &PyTuple_Type))
+    {
+        return PyTuple_GetItem(obj, index);
+    }
+    /* this should never happen, since the type was checked before */
+    return NULL;
+}
+
+/* 
+
+   mariadb_get_parameter()
+   @brief   Returns a bulk parameter which was passed to
+   cursor.executemany() or a parameter which was
+   passed to cursor.execute()
+
+   @param   self[in]         Cursor
+   @param   row_nr[in]       row number
+   @paran   column_nr[in]    column number
+   @param   paran[in][out]   bulk parameter pointer
+
+   @return  0 on success, 1 on error
+ */
+static uint8_t 
+mariadb_get_parameter(MrdbCursor *self,
+                      uint8_t is_bulk,
+                      uint32_t row_nr,
+                      uint32_t column_nr,
+                      MrdbParamValue *param)
+{
+    PyObject *row= NULL,
+             *column= NULL;
+    uint8_t rc= 1;
+    long caps;
+
+    mariadb_get_infov(self->connection->mysql,
+                      MARIADB_CONNECTION_EXTENDED_SERVER_CAPABILITIES, &caps);
+
+    if (is_bulk)
+    {
+        /* check if row_nr and column_nr are in the range from
+           0 to (value - 1) */
+        if (row_nr > (self->array_size - 1) ||
+                column_nr > (self->parseinfo.paramcount - 1))
+        {
+            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
+                    "Can't access data at row %d, column %d",
+                     row_nr + 1, column_nr + 1);
+            goto end;
+        }
+
+        if (!(row= ListOrTuple_GetItem(self->data, row_nr)))
+        {
+            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
+                    "Can't access row number %d", row_nr + 1);
+            goto end;
+        }
+    }
+    else
+        row= self->data;
+
+    if (self->parseinfo.paramstyle != PYFORMAT)
+    {
+        if (!(column= ListOrTuple_GetItem(row, column_nr)))
+        {
+            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
+                    "Can't access column number %d at row %d",
+                     column_nr + 1, row_nr + 1);
+            goto end;
+        }
+    } else
+    {
+        PyObject *key;
+
+        key= PyTuple_GetItem(self->parseinfo.keys, column_nr);
+        if (!PyDict_Contains(row, key))
+        {
+            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 0,
+                    "Can't find key in parameter data");
+            goto end;
+        }
+        column= PyDict_GetItem(row, key);
+    }
+
+    /* check if an indicator was passed */
+    if (MrdbIndicator_Check(column))
+    {
+        if (!(caps & (MARIADB_CLIENT_STMT_BULK_OPERATIONS >> 32)))
+        {
+            mariadb_throw_exception(NULL, Mariadb_NotSupportedError, 0,
+                    "MariaDB %s doesn't support indicator variables. "\
+                    "Required version is 10.2.6 or newer",
+                    mysql_get_server_info(self->stmt->mysql));
+            goto end;
+        }
+        param->indicator= (uint8_t)MrdbIndicator_AsLong(column);
+        param->value= NULL; /* you can't have both indicator and value */
+    } else if (column == Py_None) {
+        param->value= NULL;
+        if (caps &
+            (MARIADB_CLIENT_STMT_BULK_OPERATIONS >> 32))
+        {
+            param->indicator= STMT_INDICATOR_NULL;
+        }
+    } 
+    else {
+        param->value= column;
+        param->indicator= STMT_INDICATOR_NONE;
+    }
+    rc= 0;
+end:
+    return rc;
+}
+
+/* 
+   mariadb_get_parameter_info
+   mariadb_get_parameter_info fills the MYSQL_BIND structure
+   with correct field_types for the Python objects.
+
+   In case of a bulk operation (executemany()) we will also optimize
+   the field type (e.g. by checking maxbit size for a PyLong).
+   If the types in this column differ we will return an error.
+*/
+static uint8_t 
+mariadb_get_parameter_info(MrdbCursor *self,
+                           MYSQL_BIND *param,
+                           uint32_t column_nr)
+{
+    uint32_t i, bits= 0;
+    MrdbParamValue paramvalue;
+    MrdbParamInfo pinfo;
+
+    param->is_unsigned= 0;
+    paramvalue.indicator= 0;
+
+    if (!self->array_size)
+    {
+        uint8_t rc;
+        memset(&pinfo, 0, sizeof(MrdbParamInfo));
+        if (mariadb_get_parameter(self, 0, 0, column_nr, &paramvalue))
+            return 1;
+        if ((rc= mariadb_get_column_info(paramvalue.value, &pinfo)))
+        {
+            if (rc == 1)
+            {
+                mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
+                    "Can't retrieve column information for parameter %d",
+                     column_nr);
+            }
+            if (rc == 2)
+            {
+                mariadb_throw_exception(NULL, Mariadb_NotSupportedError, 0,
+                    "Data type '%s' in column %d not supported in MariaDB Connector/Python",
+                     Py_TYPE(paramvalue.value)->tp_name, column_nr);
+            }
+       
+            return 1;
+        }
+        param->buffer_type= pinfo.type;
+        bits= (uint32_t)pinfo.bits;
+    }
+    else for (i=0; i < self->array_size; i++)
+    {
+        if (mariadb_get_parameter(self, 1, i, column_nr, &paramvalue))
+            return 1;
+        memset(&pinfo, 0, sizeof(MrdbParamInfo));
+        if (mariadb_get_column_info(paramvalue.value, &pinfo) && !paramvalue.indicator)
+        {
+            mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
+                    "Invalid parameter type at row %d, column %d",
+                    i+1, column_nr + 1);
+            return 1;
+        }
+
+        if (pinfo.type == MYSQL_TYPE_LONGLONG)
+        {
+            if (pinfo.bits > bits)
+            {
+                bits= (uint32_t)pinfo.bits;
+            }
+        }
+
+        if (!param->buffer_type ||
+                param->buffer_type == MYSQL_TYPE_NULL)
+        {
+            param->buffer_type= pinfo.type;
+        }
+        else {
+            /* except for NULL the parameter types must match */
+            if (param->buffer_type != pinfo.type &&
+                    pinfo.type != MYSQL_TYPE_NULL &&
+                    !paramvalue.indicator)
+            {
+                if ((param->buffer_type == MYSQL_TYPE_TINY ||
+                     param->buffer_type == MYSQL_TYPE_SHORT ||
+                     param->buffer_type == MYSQL_TYPE_LONG) &&
+                        pinfo.type == MYSQL_TYPE_LONGLONG)
+                    break;
+                if (IS_DECIMAL_TYPE(pinfo.type) &&
+                    IS_DECIMAL_TYPE(param->buffer_type))
+                {
+                    param->buffer_type= MYSQL_TYPE_NEWDECIMAL;
+                    break;
+                }
+                mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
+                        "Invalid parameter type at row %d, column %d",
+                        i+1, column_nr + 1);
+                return 1;
+            }
+        }
+    }
+    /* check the bit size for long types and set the appropriate
+       field type */
+    if (param->buffer_type == MYSQL_TYPE_LONGLONG)
+    {
+        if ((bits <= 8 && param->is_unsigned) || bits < 8)
+        {
+            param->buffer_type= MYSQL_TYPE_TINY;
+        }
+        else if ((bits <= 16 && param->is_unsigned) || bits < 16) {
+            param->buffer_type= MYSQL_TYPE_SHORT;
+        }
+        else if ((bits <= 32 && param->is_unsigned) || bits < 32) {
+            param->buffer_type= MYSQL_TYPE_LONG;
+        }
+        else {
+            param->buffer_type= MYSQL_TYPE_LONGLONG;
+        }
+    }
+    return 0;
+}
+
+static Py_ssize_t ListOrTuple_Size(PyObject *obj)
+{
+    if (CHECK_TYPE(obj, &PyList_Type))
+    {
+        return PyList_Size(obj);
+    } else if (CHECK_TYPE(obj, &PyTuple_Type))
+    {
+        return PyTuple_Size(obj);
+    }
+    /* this should never happen, since the type was checked before */
+    return 0;
+}
+
+/* mariadb_check_bulk_parameters
+   This function validates the specified bulk parameters and
+   translates the field types to MYSQL_TYPE_*.
+ */
+uint8_t 
+mariadb_check_bulk_parameters(MrdbCursor *self,
+                              PyObject *data)
+{
+    uint32_t i;
+
+    if (!CHECK_TYPE((data), &PyList_Type) &&
+        !CHECK_TYPE(data, &PyTuple_Type))
+    {
+        mariadb_throw_exception(self->stmt, Mariadb_InterfaceError, 1, 
+                "Data must be passed as sequence (Tuple or List)");
+        return 1;
+    }
+
+    if (!(self->array_size= (uint32_t)ListOrTuple_Size(data)))
+    {
+        mariadb_throw_exception(self->stmt, Mariadb_InterfaceError, 1, 
+                "Empty parameter list. At least one row must be specified");
+        return 1;
+    }
+
+    for (i=0; i < self->array_size; i++)
+    {
+        PyObject *obj= ListOrTuple_GetItem(data, i);
+        if (self->parseinfo.paramstyle != PYFORMAT &&
+                (!CHECK_TYPE(obj, &PyTuple_Type) &&
+                 !CHECK_TYPE(obj, &PyList_Type)))
+        {
+            mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
+                    "Invalid parameter type in row %d. "\
+                    " (Row data must be provided as tuple(s))", i+1);
+            return 1;
+        }
+        if (self->parseinfo.paramstyle == PYFORMAT &&
+                !CHECK_TYPE(obj, &PyDict_Type))
+        {
+            mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
+                    "Invalid parameter type in row %d. "\
+                    " (Row data must be provided as dict)", i+1);
+            return 1;
+        }
+
+        if (!self->parseinfo.paramcount ||
+                (self->parseinfo.paramstyle != PYFORMAT && 
+                 self->parseinfo.paramcount != ListOrTuple_Size(obj)))
+        {
+            mariadb_throw_exception(self->stmt, Mariadb_ProgrammingError, 1, 
+                    "Invalid number of parameters in row %d", i+1);
+            return 1;
+        }
+    }
+
+    if (!self->is_prepared &&
+            !(self->params= PyMem_RawCalloc(self->parseinfo.paramcount,
+                                            sizeof(MYSQL_BIND))))
+    {
+        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
+                "Not enough memory (tried to allocated %lld bytes)",
+                self->parseinfo.paramcount * sizeof(MYSQL_BIND));
+        goto error;
+    }
+
+    if (!(self->value= PyMem_RawCalloc(self->parseinfo.paramcount, 
+                                       sizeof(MrdbParamValue))))
+    {
+        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
+                "Not enough memory (tried to allocated %lld bytes)",
+                self->parseinfo.paramcount * sizeof(MrdbParamValue));
+        goto error;
+    }
+
+    for (i=0; i < self->parseinfo.paramcount; i++)
+    {
+        if (mariadb_get_parameter_info(self, &self->params[i], i))
+            goto error;
+    }
+    return 0;
+error:
+    MARIADB_FREE_MEM(self->paraminfo);
+    MARIADB_FREE_MEM(self->value);
+    return 1;
+}
+
+uint8_t
+mariadb_check_execute_parameters(MrdbCursor *self,
+                                 PyObject *data)
+{
+    uint32_t i;
+
+    if (!self->parseinfo.paramcount)
+    {
+        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 0,
+                "Invalid number of parameters");
+        goto error;
+    }
+
+    if (!self->params &&
+            !(self->params= PyMem_RawCalloc(self->parseinfo.paramcount, sizeof(MYSQL_BIND))))
+    {
+        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
+                "Not enough memory (tried to allocated %lld bytes)",
+                self->parseinfo.paramcount * sizeof(MYSQL_BIND));
+        goto error;
+    }
+
+    if (!self->value &&
+       !(self->value= PyMem_RawCalloc(self->parseinfo.paramcount, sizeof(MrdbParamValue))))
+    {
+        mariadb_throw_exception(NULL, Mariadb_InterfaceError, 0,
+                "Not enough memory (tried to allocated %lld bytes)",
+                self->parseinfo.paramcount * sizeof(MrdbParamValue));
+        goto error;
+    }
+
+    for (i=0; i < self->parseinfo.paramcount; i++)
+    {
+        if (mariadb_get_parameter_info(self, &self->params[i], i))
+        {
+            goto error;
+        }
+    }
+    return 0;
+error:
+    MARIADB_FREE_MEM(self->paraminfo);
+    MARIADB_FREE_MEM(self->value);
+    return 1;
+}
+
+/* 
+  mariadb_param_to_bind()
+
+  @brief Set the current value for the specified bind buffer
+
+  @param self       cursor
+  @param bind[in]   bind structure
+  @param value[in]  current column value
+
+  @return 0 on success, otherwise error
+ */
+static uint8_t 
+mariadb_param_to_bind(MrdbCursor *self,
+                      MYSQL_BIND *bind,
+                      MrdbParamValue *value)
+{
+    uint8_t rc= 0;
+    uint8_t is_negative= 0;
+
+    if (value->indicator > 0)
+    {
+        bind->u.indicator[0]= value->indicator;
+        goto end;
+    }
+
+    if (!value->value)
+    {
+      bind->buffer_type= MYSQL_TYPE_NULL;
+    } else {
+      if (IS_NUM(bind->buffer_type))
+      {
+          bind->buffer= value->num;
+      }
+
+      if (CHECK_TYPE(value->value, &PyLong_Type))
+      {
+          if (_PyLong_Sign(value->value) < 0)
+              is_negative= 1;
+      }
+    }
+
+    switch(bind->buffer_type)
+    {
+        case MYSQL_TYPE_TINY:
+            if (!is_negative)
+            {
+                if ((value->num[0]= (uint8_t)PyLong_AsUnsignedLong(value->value)) > 0x7F)
+                    bind->is_unsigned= 1;
+            }
+            else {
+                value->num[0]= (int8_t)PyLong_AsLong(value->value);
+            }
+            break;
+        case MYSQL_TYPE_SHORT:
+            if (!is_negative)
+            {
+                if ((*(uint16_t *)&value->num= (uint16_t)PyLong_AsUnsignedLong(value->value)) > 0x7FFF)
+                    bind->is_unsigned= 1;
+            }
+            else {
+                *(int16_t *)&value->num= (int16_t)PyLong_AsLong(value->value);
+            }
+            break;
+        case MYSQL_TYPE_LONG:
+            if (!is_negative)
+            {
+                if ((*(uint32_t *)&value->num= (uint32_t)PyLong_AsUnsignedLong(value->value)) > 0x7FFFFFFF)
+                    bind->is_unsigned= 1;
+            }
+            else {
+                *(int32_t *)&value->num= (int32_t)PyLong_AsLong(value->value);
+            }
+            break;
+        case MYSQL_TYPE_LONGLONG:
+            if (!is_negative)
+            {
+                if ((*(uint64_t *)value->num= (uint64_t)PyLong_AsUnsignedLongLong(value->value)) > 0x7FFFFFFFFFFFFFFF)
+                    bind->is_unsigned= 1;
+            }
+            else {
+                *(int64_t *)value->num= (int64_t)PyLong_AsLongLong(value->value);
+            }
+            break;
+        case MYSQL_TYPE_DOUBLE:
+            *(double *)value->num= (double)PyFloat_AsDouble(value->value);
+            break;
+        case MYSQL_TYPE_LONG_BLOB:
+            bind->buffer_length= (unsigned long)PyBytes_GET_SIZE(value->value);
+            bind->buffer= (void *) PyBytes_AS_STRING(value->value);
+            break;
+        case MYSQL_TYPE_DATE:
+        case MYSQL_TYPE_TIME:
+        case MYSQL_TYPE_DATETIME:
+            bind->buffer= &value->tm;
+            if (PyDelta_CheckExact(value->value))
+                mariadb_pydelta_to_tm(value->value, &value->tm);
+            else
+                mariadb_pydate_to_tm(bind->buffer_type, value->value, &value->tm);
+            break;
+        case MYSQL_TYPE_NEWDECIMAL:
+            {
+                Py_ssize_t len;
+                PyObject *obj= NULL;
+                char *p;
+
+                if (value->free_me)
+                    MARIADB_FREE_MEM(value->buffer);
+                if (!strcmp(Py_TYPE(value->value)->tp_name, "decimal.Decimal") ||
+                    !strcmp(Py_TYPE(value->value)->tp_name, "Decimal"))
+                {
+                    obj= PyObject_Str(value->value);
+                    p= (void *)PyUnicode_AsUTF8AndSize(obj, &len);
+                }
+                else
+                {
+                    obj= PyObject_Str(value->value);
+                    p= (void *)PyUnicode_AsUTF8AndSize(obj, &len);
+                }
+                bind->buffer= value->buffer= PyMem_RawCalloc(1, len);
+                memcpy(value->buffer, p, len);
+                value->free_me= 1;
+                bind->buffer_length= (unsigned long)len;
+                Py_DECREF(obj);
+            }
+            break;
+        case MYSQL_TYPE_VAR_STRING:
+            {
+                Py_ssize_t len;
+
+                bind->buffer= (void *)PyUnicode_AsUTF8AndSize(value->value, &len);
+                bind->buffer_length= (unsigned long)len;
+                break;
+            }
+        case MYSQL_TYPE_NULL:
+            break;
+        default:
+            rc= 1;
+    }
+end:
+    return rc;
+}
+
+/* 
+  mariadb_param_update()
+  @brief   Callback function which updates the bind structure's buffer and
+  length with data from the specified row number. This callback function
+  must be registered via api function mysql_stmt_attr_set
+  with STMT_ATTR_PARAM_CALLBACK option
+
+  @param   data[in]      A pointer to a MrdbCursor object which was passed
+  via mysql_stmt_attr_set before
+  data[in][out] An array of bind structures
+  data[in]      row number
+
+  @return  0 on success, otherwise error (=1)
+*/
+uint8_t
+mariadb_param_update(void *data, MYSQL_BIND *bind, uint32_t row_nr)
+{
+    MrdbCursor *self= (MrdbCursor *)data;
+    uint32_t i;
+    uint8_t rc= 1;
+
+    for (i=0; i < self->parseinfo.paramcount; i++)
+    {
+        if (mariadb_get_parameter(self, (self->array_size > 0), 
+                                 row_nr, i, &self->value[i]))
+        {
+            goto end;
+        }
+        if (self->value[i].indicator)
+        {
+            bind[i].u.indicator= &self->value[i].indicator;
+        }
+        if (self->value[i].indicator < 1)
+        {
+            if (mariadb_param_to_bind(self, &bind[i], &self->value[i]))
+            {
+                goto end;
+            }
+        }
+    }
+    rc= 0;
+end:
+    return rc;
+}
+
+#ifdef _WIN32
+
+/* windows equivalent for clock_gettime.
+   Code based on https://stackoverflow.com/questions/5404277/porting-clock-gettime-to-windows
+ */
+
+static uint8_t g_first_time = 1;
+static LARGE_INTEGER g_counts_per_sec;
+
+int clock_gettime(int dummy, struct timespec *ct)
+{
+    LARGE_INTEGER count;
+
+    if (g_first_time)
+    {
+        g_first_time = 0;
+
+        if (0 == QueryPerformanceFrequency(&g_counts_per_sec))
+        {
+            g_counts_per_sec.QuadPart = 0;
+        }
+    }
+
+    if ((NULL == ct) || (g_counts_per_sec.QuadPart <= 0) ||
+            (0 == QueryPerformanceCounter(&count)))
+    {
+        return -1;
+    }
+
+    ct->tv_sec = count.QuadPart / g_counts_per_sec.QuadPart;
+    ct->tv_nsec = (long)(((count.QuadPart % g_counts_per_sec.QuadPart) * 1E09) / g_counts_per_sec.QuadPart);
+
+    return 0;
+}
+
+#endif
```

### Comparing `mariadb-1.1.6/mariadb/mariadb_connection.c` & `mariadb-1.1.7/mariadb/mariadb_connection.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,929 +1,935 @@
-/*****************************************************************************
-  Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
-
-  This library is free software; you can redistribute it and/or
-  modify it under the terms of the GNU Library General Public
-  License as published by the Free Software Foundation; either
-  version 2 of the License, or (at your option) any later version.
-
-  This library is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-  Library General Public License for more details.
-
-  You should have received a copy of the GNU Library General Public
-  License along with this library; if not see <http://www.gnu.org/licenses>
-  or write to the Free Software Foundation, Inc.,
-  51 Franklin St., Fifth Floor, Boston, MA 02110, USA
- *****************************************************************************/
-
-#include "mariadb_python.h"
-#include "docs/connection.h"
-#include "docs/exception.h"
-
-#define MADB_SET_OPTION(m,o,v)\
-if (mysql_optionsv((m), (o), (v)))\
-{\
-    mariadb_throw_exception(self->mysql, NULL, 0, NULL);\
-    return -1;\
-}
-
-char *dsn_keys[]= {
-    "dsn", "host", "user", "password", "database", "port", "unix_socket",
-    "connect_timeout", "read_timeout", "write_timeout",
-    "local_infile", "compress", "init_command",
-    "default_file", "default_group",
-    "ssl_key", "ssl_ca", "ssl_cert", "ssl_crl",
-    "ssl_cipher", "ssl_capath", "ssl_crlpath",
-    "ssl_verify_cert", "ssl",
-    "client_flag", "pool_name", "pool_size", 
-    "pool_reset_connection", "plugin_dir",
-    "username", "db", "passwd",
-    "status_callback",
-    NULL
-};
-
-const char *mariadb_default_charset= "utf8mb4";
-const char *mariadb_default_collation= "utf8mb4_general_ci";
-
-void
-MrdbConnection_dealloc(MrdbConnection *self);
-
-static PyObject *
-MrdbConnection_exception(PyObject *self, void *closure);
-
-#define GETTER_EXCEPTION(name, exception, doc)\
-{ name,MrdbConnection_exception, NULL, doc, &exception }
-
-static PyObject *
-MrdbConnection_getreconnect(MrdbConnection *self, void *closure);
-
-static int
-MrdbConnection_setreconnect(MrdbConnection *self, PyObject *args,
-                            void *closure);
-static PyObject *
-MrdbConnection_escape_string(MrdbConnection *self, PyObject *args);
-
-static PyObject *
-MrdbConnection_getinfo(MrdbConnection *self, PyObject *args);
-
-static PyObject *
-MrdbConnection_dump_debug_info(MrdbConnection *self);
-
-static PyObject *
-MrdbConnection_warnings(MrdbConnection *self);
-
-static PyObject *
-MrdbConnection_executecommand(MrdbConnection *self,
-                             PyObject *args);
-
-static PyObject *
-MrdbConnection_readresponse(MrdbConnection *self);
-
-static PyObject
-*MrdbConnection_socket(MrdbConnection *self);
-
-static PyGetSetDef
-MrdbConnection_sets[]=
-{
-    {"auto_reconnect", (getter)MrdbConnection_getreconnect,
-        (setter)MrdbConnection_setreconnect,
-        connection_auto_reconnect__doc__, NULL},
-    {"warnings", (getter)MrdbConnection_warnings, NULL,
-        connection_warnings__doc__, NULL},
-    GETTER_EXCEPTION("Error", Mariadb_Error, ""),
-    GETTER_EXCEPTION("Warning", Mariadb_Warning, exception_warning__doc__),
-    GETTER_EXCEPTION("InterfaceError", Mariadb_InterfaceError, exception_interface__doc__),
-    GETTER_EXCEPTION("ProgrammingError", Mariadb_ProgrammingError, exception_programming__doc__),
-    GETTER_EXCEPTION("IntegrityError", Mariadb_IntegrityError, exception_integrity__doc__),
-    GETTER_EXCEPTION("DatabaseError", Mariadb_DatabaseError, exception_database__doc__),
-    GETTER_EXCEPTION("NotSupportedError", Mariadb_NotSupportedError, exception_notsupported__doc__),
-    GETTER_EXCEPTION("InternalError", Mariadb_InternalError, exception_internal__doc__),
-    GETTER_EXCEPTION("OperationalError", Mariadb_OperationalError, exception_operational__doc__),
-    GETTER_EXCEPTION("PoolError", Mariadb_PoolError, exception_pool__doc__),
-    GETTER_EXCEPTION("DataError", Mariadb_DataError, exception_data__doc__),
-    {NULL}
-};
-
-static PyMethodDef
-MrdbConnection_Methods[] =
-{
-    /* PEP-249 methods */
-    {"close", (PyCFunction)MrdbConnection_close,
-        METH_NOARGS,
-        connection_close__doc__},
-    {"connect", (PyCFunction)MrdbConnection_connect,
-        METH_VARARGS | METH_KEYWORDS,
-        connection_connect__doc__},
-    /* additional methods */
-    { "ping",
-        (PyCFunction)MrdbConnection_ping,
-        METH_NOARGS,
-        connection_ping__doc__
-    },
-    { "change_user",
-        (PyCFunction)MrdbConnection_change_user,
-        METH_VARARGS,
-        connection_change_user__doc__
-    },
-    { "reconnect",
-        (PyCFunction)MrdbConnection_reconnect,
-        METH_NOARGS,
-        connection_reconnect__doc__
-    },
-    { "reset",
-        (PyCFunction)MrdbConnection_reset,
-        METH_NOARGS,
-        connection_reset__doc__,
-    },
-    { "escape_string",
-        (PyCFunction)MrdbConnection_escape_string,
-        METH_VARARGS,
-        connection_escape_string__doc__
-    },
-    { "dump_debug_info",
-       (PyCFunction)MrdbConnection_dump_debug_info,
-       METH_NOARGS,
-       connection_dump_debug_info__doc__
-    },
-    /* Internal methods */
-    { "_execute_command", 
-      (PyCFunction)MrdbConnection_executecommand,
-      METH_VARARGS,
-      "For internal use only"},
-    {"_read_response", (PyCFunction)MrdbConnection_readresponse,
-      METH_NOARGS,
-      "For internal use only"},
-    {"_mariadb_get_info", (PyCFunction)MrdbConnection_getinfo,
-      METH_VARARGS,
-      "For internal use only"},
-    {"_get_socket", (PyCFunction)MrdbConnection_socket,
-      METH_NOARGS,
-      "For internal use only"},
-    {NULL} /* always last */
-};
-
-static struct
-PyMemberDef MrdbConnection_Members[] =
-{
-    {"connection_id",
-        T_LONG,
-        offsetof(MrdbConnection, thread_id),
-        READONLY,
-        "Id of current connection."},
-    {"dsn",
-        T_OBJECT,
-        offsetof(MrdbConnection, dsn),
-        READONLY,
-        "Data source name (dsn)"},
-    {"_closed",
-        T_BOOL,
-        offsetof(MrdbConnection, closed),
-        READONLY,
-        "Indicates if connection was closed"},
-    {"_converter",
-        T_OBJECT,
-        offsetof(MrdbConnection, converter),
-        0,
-        "Conversion dictionary"},
-    {NULL} /* always last */
-};
-#if MARIADB_PACKAGE_VERSION_ID > 30301
-void MrdbConnection_process_status_info(void *data, enum enum_mariadb_status_info type, ...)
-{
-  va_list ap;
-  PyThreadState *_save= NULL;
-  MrdbConnection *self= (MrdbConnection *)data;
-  PyObject *dict= NULL;
-  PyObject *dict_key= NULL, *dict_val= NULL;
-  va_start(ap, type);
-
-  if (self->status_callback) {
-    if (type == STATUS_TYPE)
-    {
-      unsigned int server_status= va_arg(ap, int);
-      
-      MARIADB_UNBLOCK_THREADS(self);
-      dict_key= PyUnicode_FromString("server_status");
-      dict_val= PyLong_FromLong(server_status);
-      dict= PyDict_New();
-      PyDict_SetItem(dict, dict_key, dict_val);
-      Py_DECREF(dict_key);
-      Py_DECREF(dict_val);
-      PyObject_CallFunction(self->status_callback, "OO", (PyObject *)data, dict);
-      MARIADB_BLOCK_THREADS(self);
-    }
-  }
-  if (type == SESSION_TRACK_TYPE)
-  {
-    enum enum_session_state_type track_type= va_arg(ap, enum enum_session_state_type);
-
-    MARIADB_UNBLOCK_THREADS(self);
-
-    if (self->status_callback) {
-      switch (track_type) {
-        case SESSION_TRACK_SCHEMA:
-          dict_key= PyUnicode_FromString("schema");
-          break;
-        case SESSION_TRACK_STATE_CHANGE:
-          dict_key= PyUnicode_FromString("state_change");
-          break;
-        default:
-          break;
-      }
-    }
-
-    if (dict_key)
-    {
-      MARIADB_CONST_STRING *val= va_arg(ap, MARIADB_CONST_STRING *);
-      dict_val= PyUnicode_FromStringAndSize(val->str, val->length);
-      dict= PyDict_New();
-      PyDict_SetItem(dict, dict_key, dict_val);
-      Py_DECREF(dict_key);
-      Py_DECREF(dict_val);
-      PyObject_CallFunction(self->status_callback, "OO", (PyObject *)data, dict);
-    }
-
-    if (track_type == SESSION_TRACK_SYSTEM_VARIABLES)
-    {
-      MARIADB_CONST_STRING *key= va_arg(ap, MARIADB_CONST_STRING *);
-      MARIADB_CONST_STRING *val= va_arg(ap, MARIADB_CONST_STRING *);
-
-      if (!strncmp(key->str, "character_set_client", key->length) &&
-           strncmp(val->str, "utf8mb4", val->length))
-      {
-        /* mariadb_throw_exception (PyUnicode_FormatV)
-           doesn't support string with length,
-           so we need a temporary variable */
-        char charset[128];
-
-        memcpy(charset, val->str, val->length);
-        charset[val->length]= 0;
-        va_end(ap);
-        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
-                "Character set '%s' is not supported", charset);
-      }
-      if (self->status_callback)
-      {
-        dict_key= PyUnicode_FromStringAndSize(key->str, key->length);
-        dict_val= PyUnicode_FromStringAndSize(val->str, val->length);
-        dict= PyDict_New();
-        PyDict_SetItem(dict, dict_key, dict_val);
-        Py_DECREF(dict_key);
-        Py_DECREF(dict_val);
-        PyObject_CallFunction(self->status_callback, "OO", (PyObject *)data, dict);
-      }
-    }
-    MARIADB_BLOCK_THREADS(self);
-  }
-  va_end(ap);
-} 
-#endif
-
-static int
-MrdbConnection_Initialize(MrdbConnection *self,
-        PyObject *args,
-        PyObject *dsnargs)
-{
-    uint8_t has_error= 1;
-    char *dsn= NULL, *host=NULL, *user= NULL, *password= NULL, *schema= NULL,
-         *socket= NULL, *init_command= NULL, *default_file= NULL,
-         *default_group= NULL,
-         *ssl_key= NULL, *ssl_cert= NULL, *ssl_ca= NULL, *ssl_capath= NULL,
-         *ssl_crl= NULL, *ssl_crlpath= NULL, *ssl_cipher= NULL,
-         *plugin_dir= NULL;
-    char *pool_name= 0;
-    uint32_t pool_size= 0;
-    uint8_t ssl_enforce= 0;
-    uint8_t reset_session= 1;
-    unsigned int client_flags= 0, port= 0;
-    unsigned int local_infile= 0xFF;
-    unsigned int connect_timeout=0, read_timeout=0, write_timeout=0,
-                 compress= 0, ssl_verify_cert= 0;
-    PyObject *status_callback= NULL;
-
-    if (!PyArg_ParseTupleAndKeywords(args, dsnargs,
-                "|zzzzziziiibbzzzzzzzzzzibizibzzzzO:connect",
-                dsn_keys,
-                &dsn, &host, &user, &password, &schema, &port, &socket,
-                &connect_timeout, &read_timeout, &write_timeout,
-                &local_infile, &compress, &init_command,
-                &default_file, &default_group,
-                &ssl_key, &ssl_ca, &ssl_cert, &ssl_crl,
-                &ssl_cipher, &ssl_capath, &ssl_crlpath,
-                &ssl_verify_cert, &ssl_enforce,
-                &client_flags, &pool_name, &pool_size,
-                &reset_session, &plugin_dir,
-                &user, &schema, &password, &status_callback))
-    {
-        return -1;
-    }
-
-    if (dsn)
-    {
-        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
-                "dsn keyword is not supported");
-        return -1;
-    }
-
-#if MARIADB_PACKAGE_VERSION_ID < 30302
-    if (status_callback)
-      {
-        /* status callback requires C/C 3.3.2 */
-        PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "status_callback support requires MariaDB Connector/C >= 3.3.2 "\
-                                                  "(found version %s)", mysql_get_client_info());
-    }
-#else
-    self->status_callback= status_callback;
-#endif
-
-    if (!(self->mysql= mysql_init(NULL)))
-    {
-        mariadb_throw_exception(self->mysql, Mariadb_OperationalError, 1,
-            "Can't allocate memory for connection");
-        return -1;
-    }
-
-#if MARIADB_PACKAGE_VERSION_ID > 30301
-   if (mysql_optionsv(self->mysql, MARIADB_OPT_STATUS_CALLBACK, MrdbConnection_process_status_info, self))
-   {
-     /* Generate a warning, not an error - this will allow to run the module if Connector/C installation
-        was overwritten */
-      PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "MariaDB Connector/Python was build with MariaDB Connector/C version %s "\
-                                             "but loaded Connector/C library has version %s", MARIADB_PACKAGE_VERSION,
-                                             mysql_get_client_info());
-   }
-#endif
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-
-    if (mysql_options(self->mysql, MYSQL_SET_CHARSET_NAME, mariadb_default_charset))
-       goto end;
-
-    if (local_infile != 0xFF)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_LOCAL_INFILE, &local_infile))
-          goto end;
-    }
-
-    if (compress)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_COMPRESS, "1"))
-          goto end;
-    }
-
-    if (init_command)
-    {
-        if (mysql_options(self->mysql, MYSQL_INIT_COMMAND, init_command))
-          goto end;
-    }
-
-    if (plugin_dir) {
-        if (mysql_options(self->mysql, MYSQL_PLUGIN_DIR, plugin_dir))
-          goto end;
-    } else {
-#if defined(DEFAULT_PLUGINS_SUBDIR)
-      if (mysql_options(self->mysql, MYSQL_PLUGIN_DIR, DEFAULT_PLUGINS_SUBDIR))
-        goto end;
-#endif
-    }
-
-    /* read defaults from configuration file(s) */
-    if (default_file)
-    {
-        if (mysql_options(self->mysql, MYSQL_READ_DEFAULT_FILE, default_file))
-          goto end;
-    }
-    if (default_group)
-    {
-        if (mysql_options(self->mysql, MYSQL_READ_DEFAULT_GROUP, default_group))
-          goto end;
-    }
-
-    /* set timeouts */
-    if (connect_timeout)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_CONNECT_TIMEOUT, &connect_timeout))
-          goto end;
-    }
-    if (read_timeout)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_READ_TIMEOUT, &read_timeout))
-          goto end;
-    }
-    if (write_timeout)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_WRITE_TIMEOUT, &write_timeout))
-          goto end;
-    }
-
-    /* set TLS/SSL options */
-    if (ssl_enforce || ssl_key || ssl_ca || ssl_cert || ssl_capath || ssl_cipher)
-        mysql_ssl_set(self->mysql, (const char *)ssl_key,
-                (const char *)ssl_cert,
-                (const char *)ssl_ca,
-                (const char *)ssl_capath,
-                (const char *)ssl_cipher);
-    if (ssl_crl)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_SSL_CRL, ssl_crl))
-          goto end;
-    }
-    if (ssl_crlpath)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_SSL_CRLPATH, ssl_crlpath))
-          goto end;
-    }
-    if (ssl_verify_cert)
-    {
-        if (mysql_options(self->mysql, MYSQL_OPT_SSL_VERIFY_SERVER_CERT, (unsigned char *) &ssl_verify_cert))
-          goto end;
-    }
-
-    mysql_real_connect(self->mysql, host, user, password, schema, port,
-            socket, client_flags);
-   
-    if (mysql_errno(self->mysql))
-    {
-        goto end;
-    }
-
-    self->thread_id= mysql_thread_id(self->mysql);
-    mariadb_get_infov(self->mysql, MARIADB_CONNECTION_HOST, (void *)&self->host);
-
-    has_error= 0;
-end:
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (has_error)
-    {
-          mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-          return -1;
-    }
-
-    if (PyErr_Occurred())
-        return -1;
-
-    return 0;
-}
-
-static int MrdbConnection_traverse(
-        MrdbConnection *self,
-        visitproc visit,
-        void *arg)
-{
-    return 0;
-}
-
-static PyObject *MrdbConnection_repr(MrdbConnection *self)
-{
-    char cobj_repr[384];
-
-    if (!self->closed)
-        snprintf(cobj_repr, 384, "<mariadb.connection connected to '%s' at %p>",
-                self->host, self);
-    else
-        snprintf(cobj_repr, 384, "<mariadb.connection (closed) at %p>",
-                self);
-    return PyUnicode_FromString(cobj_repr);
-}
-
-PyTypeObject MrdbConnection_Type = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "mariadb.connection",
-    sizeof(MrdbConnection),
-    0,
-    (destructor)MrdbConnection_dealloc, /* tp_dealloc */
-    0, /*tp_print*/
-    0, /* tp_getattr */
-    0, /* tp_setattr */
-    0, /* PyAsyncMethods* */
-    (reprfunc)MrdbConnection_repr, /* tp_repr */
-
-    /* Method suites for standard classes */
-
-    0, /* (PyNumberMethods *) tp_as_number */
-    0, /* (PySequenceMethods *) tp_as_sequence */
-    0, /* (PyMappingMethods *) tp_as_mapping */
-
-    /* More standard operations (here for binary compatibility) */
-
-    0, /* (hashfunc) tp_hash */
-    0, /* (ternaryfunc) tp_call */
-    0, /* (reprfunc) tp_str */
-    0, /* tp_getattro */
-    0, /* tp_setattro */
-
-    /* Functions to access object as input/output buffer */
-    0, /* (PyBufferProcs *) tp_as_buffer */
-
-    /* (tp_flags) Flags to define presence of optional/expanded features */
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-    connection__doc__, /* tp_doc Documentation string */
-
-    /* call function for all accessible objects */
-    (traverseproc)MrdbConnection_traverse, /* tp_traverse */
-
-    /* delete references to contained objects */
-    0, /* tp_clear */
-
-    /* rich comparisons */
-    0, /* (richcmpfunc) tp_richcompare */
-
-    /* weak reference enabler */
-    0, /* (long) tp_weaklistoffset */
-
-    /* Iterators */
-    0, /* (getiterfunc) tp_iter */
-    0, /* (iternextfunc) tp_iternext */
-
-    /* Attribute descriptor and subclassing stuff */
-    (struct PyMethodDef *)MrdbConnection_Methods, /* tp_methods */
-    (struct PyMemberDef *)MrdbConnection_Members, /* tp_members */
-    MrdbConnection_sets, /* (struct getsetlist *) tp_getset; */
-    0, /* (struct _typeobject *) tp_base; */
-    0, /* (PyObject *) tp_dict */
-    0, /* (descrgetfunc) tp_descr_get */
-    0, /* (descrsetfunc) tp_descr_set */
-    0, /* (long) tp_dictoffset */
-    (initproc)MrdbConnection_Initialize, /* tp_init */
-    PyType_GenericAlloc, //NULL, /* tp_alloc */
-    PyType_GenericNew, //NULL, /* tp_new */
-    NULL, /* tp_free Low-level free-memory routine */ 
-    0, /* (PyObject *) tp_bases */
-    0, /* (PyObject *) tp_mro method resolution order */
-    0, /* (PyObject *) tp_defined */
-};
-
-PyObject *
-MrdbConnection_connect(
-        PyObject *self,
-        PyObject *args,
-        PyObject *kwargs)
-{
-    MrdbConnection *c;
-
-    if (!(c= (MrdbConnection *)PyType_GenericAlloc(&MrdbConnection_Type, 1)))
-        return NULL;
-
-    if (MrdbConnection_Initialize(c, args, kwargs))
-    {
-        Py_DECREF(c);
-        return NULL;
-    }
-    return (PyObject *) c;
-}
-
-/* destructor of MariaDB Connection object */
-void MrdbConnection_dealloc(MrdbConnection *self)
-{
-    if (self)
-    {
-        if (self->mysql)
-        {
-            MARIADB_BEGIN_ALLOW_THREADS(self)
-            mysql_close(self->mysql);
-            MARIADB_END_ALLOW_THREADS(self)
-            self->mysql= NULL;
-        }
-        Py_TYPE(self)->tp_free((PyObject*)self);
-    }
-}
-
-static PyObject *
-MrdbConnection_executecommand(MrdbConnection *self,
-                             PyObject *args)
-{
-  char *cmd;
-  int rc;
-
-  MARIADB_CHECK_CONNECTION(self, NULL);
-  if (!PyArg_ParseTuple(args, "s", &cmd))
-    return NULL;
-
-  MARIADB_BEGIN_ALLOW_THREADS(self);
-  rc= mysql_send_query(self->mysql, cmd, (long)strlen(cmd));
-  MARIADB_END_ALLOW_THREADS(self);
-
-  if (rc)
-  {
-      mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-      return NULL;
-  }
-  Py_RETURN_NONE;
-}
-
-PyObject *MrdbConnection_close(MrdbConnection *self)
-{
-    MARIADB_CHECK_CONNECTION(self, NULL);
-    /* Todo: check if all the cursor stuff is deleted (when using prepared
-       statements this should be handled in mysql_close) */
-
-    MARIADB_BEGIN_ALLOW_THREADS(self)
-    mysql_close(self->mysql);
-    MARIADB_END_ALLOW_THREADS(self)
-    self->mysql= NULL;
-    self->closed= 1;
-    Py_RETURN_NONE;
-}
-
-static PyObject *
-MrdbConnection_exception(PyObject *self, void *closure)
-{
-    PyObject *exception = *(PyObject **)closure;
-
-    Py_INCREF(exception);
-    return exception;
-}
-
-/* {{{ MrdbConnection_ping */
-PyObject *MrdbConnection_ping(MrdbConnection *self)
-{
-    int rc;
-
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-    rc= mysql_ping(self->mysql);
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (rc) {
-        mariadb_throw_exception(self->mysql, Mariadb_InterfaceError, 0, NULL);
-        return NULL;
-    }
-
-    /* in case a reconnect occurred, we need to obtain new thread_id */
-    self->thread_id= mysql_thread_id(self->mysql);
-
-    Py_RETURN_NONE;
-}
-/* }}} */
-
-/* {{{ MrdbConnection_change_user */
-PyObject *MrdbConnection_change_user(MrdbConnection *self,
-        PyObject *args)
-{
-    const char *user= NULL,
-          *password= NULL,
-          *database= NULL;
-    int rc= 0;
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    if (!PyArg_ParseTuple(args, "sss", &user, &password, &database))
-        return NULL;
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-    rc= mysql_change_user(self->mysql, user, password, database);
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (rc)
-    {
-        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-        return NULL;
-    }
-    Py_RETURN_NONE;
-}
-/* }}} */
-
-/* {{{ MrdbConnection_getreconnect */
-static PyObject *MrdbConnection_getreconnect(MrdbConnection *self,
-        void *closure)
-{
-    uint8_t reconnect= 0;
-
-    if (self->mysql) {
-        mysql_get_option(self->mysql, MYSQL_OPT_RECONNECT, &reconnect);
-    }
-
-    if (reconnect) {
-        Py_RETURN_TRUE;
-    }
-
-    Py_RETURN_FALSE;
-}
-/* }}} */
-
-/* MrdbConnection_setreconnect */
-static int MrdbConnection_setreconnect(MrdbConnection *self,
-        PyObject *args,
-        void *closure)
-{
-    uint8_t reconnect;
-
-    if (!self->mysql) {
-        return 0;
-    }
-
-    if (!args || !CHECK_TYPE(args, &PyBool_Type)) {
-        PyErr_SetString(PyExc_TypeError, "Argument must be boolean");
-        return -1;
-    }
-
-    reconnect= PyObject_IsTrue(args);
-    mysql_optionsv(self->mysql, MYSQL_OPT_RECONNECT, &reconnect);
-    return 0;
-}
-/* }}} */
-
-static PyObject *
-MrdbConnection_getinfo(MrdbConnection *self, PyObject *args)
-{
-    union {
-        char *str;
-        uint64_t num;
-        uint8_t b;
-    } val;
-
-    uint32_t option;
-
-    if (!PyArg_ParseTuple(args, "i", &option))
-          return NULL;
-
-    memset(&val, 0, sizeof(val));
-
-    if (mariadb_get_infov(self->mysql, option, &val))
-    {
-        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
-                                "Parameter option not supported");
-        return NULL;
-    }
-
-    switch (option) {
-      case MARIADB_CONNECTION_UNIX_SOCKET:
-      case MARIADB_CONNECTION_USER:
-      case MARIADB_CHARSET_NAME: 
-      case MARIADB_TLS_LIBRARY:
-      case MARIADB_CLIENT_VERSION:
-      case MARIADB_CONNECTION_HOST:
-      case MARIADB_CONNECTION_INFO:
-      case MARIADB_CONNECTION_SCHEMA:
-      case MARIADB_CONNECTION_SQLSTATE:
-      case MARIADB_CONNECTION_SOCKET:
-      case MARIADB_CONNECTION_SSL_CIPHER:
-      case MARIADB_CONNECTION_TLS_VERSION:
-      case MARIADB_CONNECTION_SERVER_VERSION:
-        return PyUnicode_FromString(val.str ? val.str : "");
-        break;
-
-      case MARIADB_CHARSET_ID:
-      case MARIADB_CLIENT_VERSION_ID:
-      case MARIADB_CONNECTION_ASYNC_TIMEOUT:
-      case MARIADB_CONNECTION_ASYNC_TIMEOUT_MS:
-      case MARIADB_CONNECTION_PORT:
-      case MARIADB_CONNECTION_PROTOCOL_VERSION_ID:
-      case MARIADB_CONNECTION_SERVER_TYPE:
-      case MARIADB_CONNECTION_SERVER_VERSION_ID:
-      case MARIADB_CONNECTION_TLS_VERSION_ID:
-      case MARIADB_MAX_ALLOWED_PACKET:
-      case MARIADB_NET_BUFFER_LENGTH:
-      case MARIADB_CONNECTION_SERVER_STATUS:
-      case MARIADB_CONNECTION_SERVER_CAPABILITIES:
-      case MARIADB_CONNECTION_EXTENDED_SERVER_CAPABILITIES:
-      case MARIADB_CONNECTION_CLIENT_CAPABILITIES:
-#ifdef MARIADB_CONNECTION_BYTES_READ
-      case MARIADB_CONNECTION_BYTES_READ:
-      case MARIADB_CONNECTION_BYTES_SENT:
-#endif
-        return PyLong_FromLong((long)val.num);
-        break;
-      default:
-        Py_RETURN_NONE;
-    }
-}
-
-/* {{{ MrdbConnection_reconnect */
-PyObject *MrdbConnection_reconnect(MrdbConnection *self)
-{
-    int rc;
-    uint8_t reconnect= 1;
-    uint8_t save_reconnect;
-
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    mysql_get_option(self->mysql, MYSQL_OPT_RECONNECT, &save_reconnect);
-    /* coverity[copy_paste_error] */
-    if (!save_reconnect)
-        mysql_optionsv(self->mysql, MYSQL_OPT_RECONNECT, &reconnect);
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-    rc= mariadb_reconnect(self->mysql);
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (!save_reconnect)
-        mysql_optionsv(self->mysql, MYSQL_OPT_RECONNECT, &save_reconnect);
-
-    if (rc)
-    {
-        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-        return NULL;
-    }
-    /* get capabilities */
-    self->thread_id= mysql_thread_id(self->mysql);
-    Py_RETURN_NONE;
-}
-/* }}} */
-
-/* {{{ MrdbConnection_reset */
-PyObject *MrdbConnection_reset(MrdbConnection *self)
-{
-    int rc;
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-    rc= mysql_reset_connection(self->mysql);
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (rc)
-    {
-        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-        return NULL;
-    }
-    Py_RETURN_NONE;
-}
-/* }}} */
-
-/* {{{ MrdbConnection_warnings */
-static PyObject *MrdbConnection_warnings(MrdbConnection *self)
-{
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    return PyLong_FromLong((long)mysql_warning_count(self->mysql));
-}
-/* }}} */
-
-/* {{{ MrdbConnection_escape_string */
-static PyObject *MrdbConnection_escape_string(MrdbConnection *self,
-        PyObject *args)
-{
-    PyObject *string= NULL,
-             *new_string= NULL;
-    size_t from_length, to_length;
-    char *from, *to;
-
-    /* escaping depends on the server status, so we need a valid
-       connection */
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    if (!PyArg_ParseTuple(args, "O!", &PyUnicode_Type, &string))
-        return NULL;
-
-    from= (char *)PyUnicode_AsUTF8AndSize(string, (Py_ssize_t *)&from_length);
-    if (!(to= (char *)PyMem_RawCalloc(1, from_length * 2 + 1)))
-    {
-        return NULL;
-    }
-    to_length= mysql_real_escape_string(self->mysql, to, from, (unsigned long)from_length);
-    new_string= PyUnicode_FromStringAndSize(to, to_length);
-    PyMem_Free(to);
-    return new_string;
-}
-/* }}} */
-
-static PyObject *
-MrdbConnection_dump_debug_info(MrdbConnection *self)
-{
-    int rc;
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-    rc= mysql_dump_debug_info(self->mysql);
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (rc)
-    {
-        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-        return NULL;
-    }
-    Py_RETURN_NONE;
-}
-
-static PyObject *MrdbConnection_readresponse(MrdbConnection *self)
-{
-    int rc;
-
-    MARIADB_BEGIN_ALLOW_THREADS(self);
-    rc= self->mysql->methods->db_read_query_result(self->mysql);
-    MARIADB_END_ALLOW_THREADS(self);
-
-    if (rc)
-    {
-        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
-        return NULL;
-    }
-    Py_RETURN_NONE;
-}
-
-static PyObject *MrdbConnection_socket(MrdbConnection *self)
-{
-    MARIADB_CHECK_CONNECTION(self, NULL);
-
-    return PyLong_FromLong((unsigned long)mysql_get_socket(self->mysql));
-}
-
-/* vim: set tabstop=4 */
-/* vim: set shiftwidth=4 */
-/* vim: set expandtab */
-/* vim: set foldmethod=indent */
-/* vim: set foldnestmax=10 */
-/* vim: set nofoldenable */
-/* vim: set foldlevel=2 */
+/*****************************************************************************
+  Copyright (C) 2018-2020 Georg Richter and MariaDB Corporation AB
+
+  This library is free software; you can redistribute it and/or
+  modify it under the terms of the GNU Library General Public
+  License as published by the Free Software Foundation; either
+  version 2 of the License, or (at your option) any later version.
+
+  This library is distributed in the hope that it will be useful,
+  but WITHOUT ANY WARRANTY; without even the implied warranty of
+  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+  Library General Public License for more details.
+
+  You should have received a copy of the GNU Library General Public
+  License along with this library; if not see <http://www.gnu.org/licenses>
+  or write to the Free Software Foundation, Inc.,
+  51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+ *****************************************************************************/
+
+#include "mariadb_python.h"
+#include "docs/connection.h"
+#include "docs/exception.h"
+
+#define MADB_SET_OPTION(m,o,v)\
+if (mysql_optionsv((m), (o), (v)))\
+{\
+    mariadb_throw_exception(self->mysql, NULL, 0, NULL);\
+    return -1;\
+}
+
+char *dsn_keys[]= {
+    "dsn", "host", "user", "password", "database", "port", "unix_socket",
+    "connect_timeout", "read_timeout", "write_timeout",
+    "local_infile", "compress", "init_command",
+    "default_file", "default_group",
+    "ssl_key", "ssl_ca", "ssl_cert", "ssl_crl",
+    "ssl_cipher", "ssl_capath", "ssl_crlpath",
+    "ssl_verify_cert", "ssl",
+    "client_flag", "pool_name", "pool_size", 
+    "pool_reset_connection", "plugin_dir",
+    "username", "db", "passwd",
+    "status_callback", "tls_version",
+    NULL
+};
+
+const char *mariadb_default_charset= "utf8mb4";
+const char *mariadb_default_collation= "utf8mb4_general_ci";
+
+void
+MrdbConnection_dealloc(MrdbConnection *self);
+
+static PyObject *
+MrdbConnection_exception(PyObject *self, void *closure);
+
+#define GETTER_EXCEPTION(name, exception, doc)\
+{ name,MrdbConnection_exception, NULL, doc, &exception }
+
+static PyObject *
+MrdbConnection_getreconnect(MrdbConnection *self, void *closure);
+
+static int
+MrdbConnection_setreconnect(MrdbConnection *self, PyObject *args,
+                            void *closure);
+static PyObject *
+MrdbConnection_escape_string(MrdbConnection *self, PyObject *args);
+
+static PyObject *
+MrdbConnection_getinfo(MrdbConnection *self, PyObject *args);
+
+static PyObject *
+MrdbConnection_dump_debug_info(MrdbConnection *self);
+
+static PyObject *
+MrdbConnection_warnings(MrdbConnection *self);
+
+static PyObject *
+MrdbConnection_executecommand(MrdbConnection *self,
+                             PyObject *args);
+
+static PyObject *
+MrdbConnection_readresponse(MrdbConnection *self);
+
+static PyObject
+*MrdbConnection_socket(MrdbConnection *self);
+
+static PyGetSetDef
+MrdbConnection_sets[]=
+{
+    {"auto_reconnect", (getter)MrdbConnection_getreconnect,
+        (setter)MrdbConnection_setreconnect,
+        connection_auto_reconnect__doc__, NULL},
+    {"warnings", (getter)MrdbConnection_warnings, NULL,
+        connection_warnings__doc__, NULL},
+    GETTER_EXCEPTION("Error", Mariadb_Error, ""),
+    GETTER_EXCEPTION("Warning", Mariadb_Warning, exception_warning__doc__),
+    GETTER_EXCEPTION("InterfaceError", Mariadb_InterfaceError, exception_interface__doc__),
+    GETTER_EXCEPTION("ProgrammingError", Mariadb_ProgrammingError, exception_programming__doc__),
+    GETTER_EXCEPTION("IntegrityError", Mariadb_IntegrityError, exception_integrity__doc__),
+    GETTER_EXCEPTION("DatabaseError", Mariadb_DatabaseError, exception_database__doc__),
+    GETTER_EXCEPTION("NotSupportedError", Mariadb_NotSupportedError, exception_notsupported__doc__),
+    GETTER_EXCEPTION("InternalError", Mariadb_InternalError, exception_internal__doc__),
+    GETTER_EXCEPTION("OperationalError", Mariadb_OperationalError, exception_operational__doc__),
+    GETTER_EXCEPTION("PoolError", Mariadb_PoolError, exception_pool__doc__),
+    GETTER_EXCEPTION("DataError", Mariadb_DataError, exception_data__doc__),
+    {NULL}
+};
+
+static PyMethodDef
+MrdbConnection_Methods[] =
+{
+    /* PEP-249 methods */
+    {"close", (PyCFunction)MrdbConnection_close,
+        METH_NOARGS,
+        connection_close__doc__},
+    {"connect", (PyCFunction)MrdbConnection_connect,
+        METH_VARARGS | METH_KEYWORDS,
+        connection_connect__doc__},
+    /* additional methods */
+    { "ping",
+        (PyCFunction)MrdbConnection_ping,
+        METH_NOARGS,
+        connection_ping__doc__
+    },
+    { "change_user",
+        (PyCFunction)MrdbConnection_change_user,
+        METH_VARARGS,
+        connection_change_user__doc__
+    },
+    { "reconnect",
+        (PyCFunction)MrdbConnection_reconnect,
+        METH_NOARGS,
+        connection_reconnect__doc__
+    },
+    { "reset",
+        (PyCFunction)MrdbConnection_reset,
+        METH_NOARGS,
+        connection_reset__doc__,
+    },
+    { "escape_string",
+        (PyCFunction)MrdbConnection_escape_string,
+        METH_VARARGS,
+        connection_escape_string__doc__
+    },
+    { "dump_debug_info",
+       (PyCFunction)MrdbConnection_dump_debug_info,
+       METH_NOARGS,
+       connection_dump_debug_info__doc__
+    },
+    /* Internal methods */
+    { "_execute_command", 
+      (PyCFunction)MrdbConnection_executecommand,
+      METH_VARARGS,
+      "For internal use only"},
+    {"_read_response", (PyCFunction)MrdbConnection_readresponse,
+      METH_NOARGS,
+      "For internal use only"},
+    {"_mariadb_get_info", (PyCFunction)MrdbConnection_getinfo,
+      METH_VARARGS,
+      "For internal use only"},
+    {"_get_socket", (PyCFunction)MrdbConnection_socket,
+      METH_NOARGS,
+      "For internal use only"},
+    {NULL} /* always last */
+};
+
+static struct
+PyMemberDef MrdbConnection_Members[] =
+{
+    {"connection_id",
+        T_LONG,
+        offsetof(MrdbConnection, thread_id),
+        READONLY,
+        "Id of current connection."},
+    {"dsn",
+        T_OBJECT,
+        offsetof(MrdbConnection, dsn),
+        READONLY,
+        "Data source name (dsn)"},
+    {"_closed",
+        T_BOOL,
+        offsetof(MrdbConnection, closed),
+        READONLY,
+        "Indicates if connection was closed"},
+    {"_converter",
+        T_OBJECT,
+        offsetof(MrdbConnection, converter),
+        0,
+        "Conversion dictionary"},
+    {NULL} /* always last */
+};
+#if MARIADB_PACKAGE_VERSION_ID > 30301
+void MrdbConnection_process_status_info(void *data, enum enum_mariadb_status_info type, ...)
+{
+  va_list ap;
+  PyThreadState *_save= NULL;
+  MrdbConnection *self= (MrdbConnection *)data;
+  PyObject *dict= NULL;
+  PyObject *dict_key= NULL, *dict_val= NULL;
+  va_start(ap, type);
+
+  if (self->status_callback) {
+    if (type == STATUS_TYPE)
+    {
+      unsigned int server_status= va_arg(ap, int);
+      
+      MARIADB_UNBLOCK_THREADS(self);
+      dict_key= PyUnicode_FromString("server_status");
+      dict_val= PyLong_FromLong(server_status);
+      dict= PyDict_New();
+      PyDict_SetItem(dict, dict_key, dict_val);
+      Py_DECREF(dict_key);
+      Py_DECREF(dict_val);
+      PyObject_CallFunction(self->status_callback, "OO", (PyObject *)data, dict);
+      MARIADB_BLOCK_THREADS(self);
+    }
+  }
+  if (type == SESSION_TRACK_TYPE)
+  {
+    enum enum_session_state_type track_type= va_arg(ap, enum enum_session_state_type);
+
+    MARIADB_UNBLOCK_THREADS(self);
+
+    if (self->status_callback) {
+      switch (track_type) {
+        case SESSION_TRACK_SCHEMA:
+          dict_key= PyUnicode_FromString("schema");
+          break;
+        case SESSION_TRACK_STATE_CHANGE:
+          dict_key= PyUnicode_FromString("state_change");
+          break;
+        default:
+          break;
+      }
+    }
+
+    if (dict_key)
+    {
+      MARIADB_CONST_STRING *val= va_arg(ap, MARIADB_CONST_STRING *);
+      dict_val= PyUnicode_FromStringAndSize(val->str, val->length);
+      dict= PyDict_New();
+      PyDict_SetItem(dict, dict_key, dict_val);
+      Py_DECREF(dict_key);
+      Py_DECREF(dict_val);
+      PyObject_CallFunction(self->status_callback, "OO", (PyObject *)data, dict);
+    }
+
+    if (track_type == SESSION_TRACK_SYSTEM_VARIABLES)
+    {
+      MARIADB_CONST_STRING *key= va_arg(ap, MARIADB_CONST_STRING *);
+      MARIADB_CONST_STRING *val= va_arg(ap, MARIADB_CONST_STRING *);
+
+      if (!strncmp(key->str, "character_set_client", key->length) &&
+           strncmp(val->str, "utf8mb4", val->length))
+      {
+        /* mariadb_throw_exception (PyUnicode_FormatV)
+           doesn't support string with length,
+           so we need a temporary variable */
+        char charset[128];
+
+        memcpy(charset, val->str, val->length);
+        charset[val->length]= 0;
+        va_end(ap);
+        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
+                "Character set '%s' is not supported", charset);
+      }
+      if (self->status_callback)
+      {
+        dict_key= PyUnicode_FromStringAndSize(key->str, key->length);
+        dict_val= PyUnicode_FromStringAndSize(val->str, val->length);
+        dict= PyDict_New();
+        PyDict_SetItem(dict, dict_key, dict_val);
+        Py_DECREF(dict_key);
+        Py_DECREF(dict_val);
+        PyObject_CallFunction(self->status_callback, "OO", (PyObject *)data, dict);
+      }
+    }
+    MARIADB_BLOCK_THREADS(self);
+  }
+  va_end(ap);
+} 
+#endif
+
+static int
+MrdbConnection_Initialize(MrdbConnection *self,
+        PyObject *args,
+        PyObject *dsnargs)
+{
+    uint8_t has_error= 1;
+    char *dsn= NULL, *host=NULL, *user= NULL, *password= NULL, *schema= NULL,
+         *socket= NULL, *init_command= NULL, *default_file= NULL,
+         *default_group= NULL,
+         *ssl_key= NULL, *ssl_cert= NULL, *ssl_ca= NULL, *ssl_capath= NULL,
+         *ssl_crl= NULL, *ssl_crlpath= NULL, *ssl_cipher= NULL,
+         *plugin_dir= NULL, *tls_version= NULL;
+    char *pool_name= 0;
+    uint32_t pool_size= 0;
+    uint8_t ssl_enforce= 0;
+    uint8_t reset_session= 1;
+    unsigned int client_flags= 0, port= 0;
+    unsigned int local_infile= 0xFF;
+    unsigned int connect_timeout=0, read_timeout=0, write_timeout=0,
+                 compress= 0, ssl_verify_cert= 0;
+    PyObject *status_callback= NULL;
+
+    if (!PyArg_ParseTupleAndKeywords(args, dsnargs,
+                "|zzzzziziiibbzzzzzzzzzzibizibzzzzOz:connect",
+                dsn_keys,
+                &dsn, &host, &user, &password, &schema, &port, &socket,
+                &connect_timeout, &read_timeout, &write_timeout,
+                &local_infile, &compress, &init_command,
+                &default_file, &default_group,
+                &ssl_key, &ssl_ca, &ssl_cert, &ssl_crl,
+                &ssl_cipher, &ssl_capath, &ssl_crlpath,
+                &ssl_verify_cert, &ssl_enforce,
+                &client_flags, &pool_name, &pool_size,
+                &reset_session, &plugin_dir,
+                &user, &schema, &password, &status_callback,
+                &tls_version))
+    {
+        return -1;
+    }
+
+    if (dsn)
+    {
+        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
+                "dsn keyword is not supported");
+        return -1;
+    }
+
+#if MARIADB_PACKAGE_VERSION_ID < 30302
+    if (status_callback)
+      {
+        /* status callback requires C/C 3.3.2 */
+        PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "status_callback support requires MariaDB Connector/C >= 3.3.2 "\
+                                                  "(found version %s)", mysql_get_client_info());
+    }
+#else
+    self->status_callback= status_callback;
+#endif
+
+    if (!(self->mysql= mysql_init(NULL)))
+    {
+        mariadb_throw_exception(self->mysql, Mariadb_OperationalError, 1,
+            "Can't allocate memory for connection");
+        return -1;
+    }
+
+#if MARIADB_PACKAGE_VERSION_ID > 30301
+   if (mysql_optionsv(self->mysql, MARIADB_OPT_STATUS_CALLBACK, MrdbConnection_process_status_info, self))
+   {
+     /* Generate a warning, not an error - this will allow to run the module if Connector/C installation
+        was overwritten */
+      PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "MariaDB Connector/Python was build with MariaDB Connector/C version %s "\
+                                             "but loaded Connector/C library has version %s", MARIADB_PACKAGE_VERSION,
+                                             mysql_get_client_info());
+   }
+#endif
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+
+    if (mysql_options(self->mysql, MYSQL_SET_CHARSET_NAME, mariadb_default_charset))
+       goto end;
+
+    if (local_infile != 0xFF)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_LOCAL_INFILE, &local_infile))
+          goto end;
+    }
+
+    if (compress)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_COMPRESS, "1"))
+          goto end;
+    }
+
+    if (init_command)
+    {
+        if (mysql_options(self->mysql, MYSQL_INIT_COMMAND, init_command))
+          goto end;
+    }
+
+    if (plugin_dir) {
+        if (mysql_options(self->mysql, MYSQL_PLUGIN_DIR, plugin_dir))
+          goto end;
+    } else {
+#if defined(DEFAULT_PLUGINS_SUBDIR)
+      if (mysql_options(self->mysql, MYSQL_PLUGIN_DIR, DEFAULT_PLUGINS_SUBDIR))
+        goto end;
+#endif
+    }
+
+    /* read defaults from configuration file(s) */
+    if (default_file)
+    {
+        if (mysql_options(self->mysql, MYSQL_READ_DEFAULT_FILE, default_file))
+          goto end;
+    }
+    if (default_group)
+    {
+        if (mysql_options(self->mysql, MYSQL_READ_DEFAULT_GROUP, default_group))
+          goto end;
+    }
+
+    /* set timeouts */
+    if (connect_timeout)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_CONNECT_TIMEOUT, &connect_timeout))
+          goto end;
+    }
+    if (read_timeout)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_READ_TIMEOUT, &read_timeout))
+          goto end;
+    }
+    if (write_timeout)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_WRITE_TIMEOUT, &write_timeout))
+          goto end;
+    }
+
+    /* set TLS/SSL options */
+    if (ssl_enforce || ssl_key || ssl_ca || ssl_cert || ssl_capath || ssl_cipher || tls_version)
+        mysql_ssl_set(self->mysql, (const char *)ssl_key,
+                (const char *)ssl_cert,
+                (const char *)ssl_ca,
+                (const char *)ssl_capath,
+                (const char *)ssl_cipher);
+    if (ssl_crl)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_SSL_CRL, ssl_crl))
+          goto end;
+    }
+    if (ssl_crlpath)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_SSL_CRLPATH, ssl_crlpath))
+          goto end;
+    }
+    if (ssl_verify_cert)
+    {
+        if (mysql_options(self->mysql, MYSQL_OPT_SSL_VERIFY_SERVER_CERT, (unsigned char *) &ssl_verify_cert))
+          goto end;
+    }
+    if (tls_version)
+    {
+        if (mysql_options(self->mysql, MARIADB_OPT_TLS_VERSION, tls_version))
+          goto end;
+    }
+
+    mysql_real_connect(self->mysql, host, user, password, schema, port,
+            socket, client_flags);
+   
+    if (mysql_errno(self->mysql))
+    {
+        goto end;
+    }
+
+    self->thread_id= mysql_thread_id(self->mysql);
+    mariadb_get_infov(self->mysql, MARIADB_CONNECTION_HOST, (void *)&self->host);
+
+    has_error= 0;
+end:
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (has_error)
+    {
+          mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+          return -1;
+    }
+
+    if (PyErr_Occurred())
+        return -1;
+
+    return 0;
+}
+
+static int MrdbConnection_traverse(
+        MrdbConnection *self,
+        visitproc visit,
+        void *arg)
+{
+    return 0;
+}
+
+static PyObject *MrdbConnection_repr(MrdbConnection *self)
+{
+    char cobj_repr[384];
+
+    if (!self->closed)
+        snprintf(cobj_repr, 384, "<mariadb.connection connected to '%s' at %p>",
+                self->host, self);
+    else
+        snprintf(cobj_repr, 384, "<mariadb.connection (closed) at %p>",
+                self);
+    return PyUnicode_FromString(cobj_repr);
+}
+
+PyTypeObject MrdbConnection_Type = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "mariadb.connection",
+    sizeof(MrdbConnection),
+    0,
+    (destructor)MrdbConnection_dealloc, /* tp_dealloc */
+    0, /*tp_print*/
+    0, /* tp_getattr */
+    0, /* tp_setattr */
+    0, /* PyAsyncMethods* */
+    (reprfunc)MrdbConnection_repr, /* tp_repr */
+
+    /* Method suites for standard classes */
+
+    0, /* (PyNumberMethods *) tp_as_number */
+    0, /* (PySequenceMethods *) tp_as_sequence */
+    0, /* (PyMappingMethods *) tp_as_mapping */
+
+    /* More standard operations (here for binary compatibility) */
+
+    0, /* (hashfunc) tp_hash */
+    0, /* (ternaryfunc) tp_call */
+    0, /* (reprfunc) tp_str */
+    0, /* tp_getattro */
+    0, /* tp_setattro */
+
+    /* Functions to access object as input/output buffer */
+    0, /* (PyBufferProcs *) tp_as_buffer */
+
+    /* (tp_flags) Flags to define presence of optional/expanded features */
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    connection__doc__, /* tp_doc Documentation string */
+
+    /* call function for all accessible objects */
+    (traverseproc)MrdbConnection_traverse, /* tp_traverse */
+
+    /* delete references to contained objects */
+    0, /* tp_clear */
+
+    /* rich comparisons */
+    0, /* (richcmpfunc) tp_richcompare */
+
+    /* weak reference enabler */
+    0, /* (long) tp_weaklistoffset */
+
+    /* Iterators */
+    0, /* (getiterfunc) tp_iter */
+    0, /* (iternextfunc) tp_iternext */
+
+    /* Attribute descriptor and subclassing stuff */
+    (struct PyMethodDef *)MrdbConnection_Methods, /* tp_methods */
+    (struct PyMemberDef *)MrdbConnection_Members, /* tp_members */
+    MrdbConnection_sets, /* (struct getsetlist *) tp_getset; */
+    0, /* (struct _typeobject *) tp_base; */
+    0, /* (PyObject *) tp_dict */
+    0, /* (descrgetfunc) tp_descr_get */
+    0, /* (descrsetfunc) tp_descr_set */
+    0, /* (long) tp_dictoffset */
+    (initproc)MrdbConnection_Initialize, /* tp_init */
+    PyType_GenericAlloc, //NULL, /* tp_alloc */
+    PyType_GenericNew, //NULL, /* tp_new */
+    NULL, /* tp_free Low-level free-memory routine */ 
+    0, /* (PyObject *) tp_bases */
+    0, /* (PyObject *) tp_mro method resolution order */
+    0, /* (PyObject *) tp_defined */
+};
+
+PyObject *
+MrdbConnection_connect(
+        PyObject *self,
+        PyObject *args,
+        PyObject *kwargs)
+{
+    MrdbConnection *c;
+
+    if (!(c= (MrdbConnection *)PyType_GenericAlloc(&MrdbConnection_Type, 1)))
+        return NULL;
+
+    if (MrdbConnection_Initialize(c, args, kwargs))
+    {
+        Py_DECREF(c);
+        return NULL;
+    }
+    return (PyObject *) c;
+}
+
+/* destructor of MariaDB Connection object */
+void MrdbConnection_dealloc(MrdbConnection *self)
+{
+    if (self)
+    {
+        if (self->mysql)
+        {
+            MARIADB_BEGIN_ALLOW_THREADS(self)
+            mysql_close(self->mysql);
+            MARIADB_END_ALLOW_THREADS(self)
+            self->mysql= NULL;
+        }
+        Py_TYPE(self)->tp_free((PyObject*)self);
+    }
+}
+
+static PyObject *
+MrdbConnection_executecommand(MrdbConnection *self,
+                             PyObject *args)
+{
+  char *cmd;
+  int rc;
+
+  MARIADB_CHECK_CONNECTION(self, NULL);
+  if (!PyArg_ParseTuple(args, "s", &cmd))
+    return NULL;
+
+  MARIADB_BEGIN_ALLOW_THREADS(self);
+  rc= mysql_send_query(self->mysql, cmd, (long)strlen(cmd));
+  MARIADB_END_ALLOW_THREADS(self);
+
+  if (rc)
+  {
+      mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+      return NULL;
+  }
+  Py_RETURN_NONE;
+}
+
+PyObject *MrdbConnection_close(MrdbConnection *self)
+{
+    MARIADB_CHECK_CONNECTION(self, NULL);
+    /* Todo: check if all the cursor stuff is deleted (when using prepared
+       statements this should be handled in mysql_close) */
+
+    MARIADB_BEGIN_ALLOW_THREADS(self)
+    mysql_close(self->mysql);
+    MARIADB_END_ALLOW_THREADS(self)
+    self->mysql= NULL;
+    self->closed= 1;
+    Py_RETURN_NONE;
+}
+
+static PyObject *
+MrdbConnection_exception(PyObject *self, void *closure)
+{
+    PyObject *exception = *(PyObject **)closure;
+
+    Py_INCREF(exception);
+    return exception;
+}
+
+/* {{{ MrdbConnection_ping */
+PyObject *MrdbConnection_ping(MrdbConnection *self)
+{
+    int rc;
+
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+    rc= mysql_ping(self->mysql);
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (rc) {
+        mariadb_throw_exception(self->mysql, Mariadb_InterfaceError, 0, NULL);
+        return NULL;
+    }
+
+    /* in case a reconnect occurred, we need to obtain new thread_id */
+    self->thread_id= mysql_thread_id(self->mysql);
+
+    Py_RETURN_NONE;
+}
+/* }}} */
+
+/* {{{ MrdbConnection_change_user */
+PyObject *MrdbConnection_change_user(MrdbConnection *self,
+        PyObject *args)
+{
+    const char *user= NULL,
+          *password= NULL,
+          *database= NULL;
+    int rc= 0;
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    if (!PyArg_ParseTuple(args, "sss", &user, &password, &database))
+        return NULL;
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+    rc= mysql_change_user(self->mysql, user, password, database);
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (rc)
+    {
+        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+        return NULL;
+    }
+    Py_RETURN_NONE;
+}
+/* }}} */
+
+/* {{{ MrdbConnection_getreconnect */
+static PyObject *MrdbConnection_getreconnect(MrdbConnection *self,
+        void *closure)
+{
+    uint8_t reconnect= 0;
+
+    if (self->mysql) {
+        mysql_get_option(self->mysql, MYSQL_OPT_RECONNECT, &reconnect);
+    }
+
+    if (reconnect) {
+        Py_RETURN_TRUE;
+    }
+
+    Py_RETURN_FALSE;
+}
+/* }}} */
+
+/* MrdbConnection_setreconnect */
+static int MrdbConnection_setreconnect(MrdbConnection *self,
+        PyObject *args,
+        void *closure)
+{
+    uint8_t reconnect;
+
+    if (!self->mysql) {
+        return 0;
+    }
+
+    if (!args || !CHECK_TYPE(args, &PyBool_Type)) {
+        PyErr_SetString(PyExc_TypeError, "Argument must be boolean");
+        return -1;
+    }
+
+    reconnect= PyObject_IsTrue(args);
+    mysql_optionsv(self->mysql, MYSQL_OPT_RECONNECT, &reconnect);
+    return 0;
+}
+/* }}} */
+
+static PyObject *
+MrdbConnection_getinfo(MrdbConnection *self, PyObject *args)
+{
+    union {
+        char *str;
+        uint64_t num;
+        uint8_t b;
+    } val;
+
+    uint32_t option;
+
+    if (!PyArg_ParseTuple(args, "i", &option))
+          return NULL;
+
+    memset(&val, 0, sizeof(val));
+
+    if (mariadb_get_infov(self->mysql, option, &val))
+    {
+        mariadb_throw_exception(NULL, Mariadb_ProgrammingError, 1,
+                                "Parameter option not supported");
+        return NULL;
+    }
+
+    switch (option) {
+      case MARIADB_CONNECTION_UNIX_SOCKET:
+      case MARIADB_CONNECTION_USER:
+      case MARIADB_CHARSET_NAME: 
+      case MARIADB_TLS_LIBRARY:
+      case MARIADB_CLIENT_VERSION:
+      case MARIADB_CONNECTION_HOST:
+      case MARIADB_CONNECTION_INFO:
+      case MARIADB_CONNECTION_SCHEMA:
+      case MARIADB_CONNECTION_SQLSTATE:
+      case MARIADB_CONNECTION_SOCKET:
+      case MARIADB_CONNECTION_SSL_CIPHER:
+      case MARIADB_CONNECTION_TLS_VERSION:
+      case MARIADB_CONNECTION_SERVER_VERSION:
+        return PyUnicode_FromString(val.str ? val.str : "");
+        break;
+
+      case MARIADB_CHARSET_ID:
+      case MARIADB_CLIENT_VERSION_ID:
+      case MARIADB_CONNECTION_ASYNC_TIMEOUT:
+      case MARIADB_CONNECTION_ASYNC_TIMEOUT_MS:
+      case MARIADB_CONNECTION_PORT:
+      case MARIADB_CONNECTION_PROTOCOL_VERSION_ID:
+      case MARIADB_CONNECTION_SERVER_TYPE:
+      case MARIADB_CONNECTION_SERVER_VERSION_ID:
+      case MARIADB_CONNECTION_TLS_VERSION_ID:
+      case MARIADB_MAX_ALLOWED_PACKET:
+      case MARIADB_NET_BUFFER_LENGTH:
+      case MARIADB_CONNECTION_SERVER_STATUS:
+      case MARIADB_CONNECTION_SERVER_CAPABILITIES:
+      case MARIADB_CONNECTION_EXTENDED_SERVER_CAPABILITIES:
+      case MARIADB_CONNECTION_CLIENT_CAPABILITIES:
+#ifdef MARIADB_CONNECTION_BYTES_READ
+      case MARIADB_CONNECTION_BYTES_READ:
+      case MARIADB_CONNECTION_BYTES_SENT:
+#endif
+        return PyLong_FromLong((long)val.num);
+        break;
+      default:
+        Py_RETURN_NONE;
+    }
+}
+
+/* {{{ MrdbConnection_reconnect */
+PyObject *MrdbConnection_reconnect(MrdbConnection *self)
+{
+    int rc;
+    uint8_t reconnect= 1;
+    uint8_t save_reconnect;
+
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    mysql_get_option(self->mysql, MYSQL_OPT_RECONNECT, &save_reconnect);
+    /* coverity[copy_paste_error] */
+    if (!save_reconnect)
+        mysql_optionsv(self->mysql, MYSQL_OPT_RECONNECT, &reconnect);
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+    rc= mariadb_reconnect(self->mysql);
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (!save_reconnect)
+        mysql_optionsv(self->mysql, MYSQL_OPT_RECONNECT, &save_reconnect);
+
+    if (rc)
+    {
+        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+        return NULL;
+    }
+    /* get capabilities */
+    self->thread_id= mysql_thread_id(self->mysql);
+    Py_RETURN_NONE;
+}
+/* }}} */
+
+/* {{{ MrdbConnection_reset */
+PyObject *MrdbConnection_reset(MrdbConnection *self)
+{
+    int rc;
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+    rc= mysql_reset_connection(self->mysql);
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (rc)
+    {
+        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+        return NULL;
+    }
+    Py_RETURN_NONE;
+}
+/* }}} */
+
+/* {{{ MrdbConnection_warnings */
+static PyObject *MrdbConnection_warnings(MrdbConnection *self)
+{
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    return PyLong_FromLong((long)mysql_warning_count(self->mysql));
+}
+/* }}} */
+
+/* {{{ MrdbConnection_escape_string */
+static PyObject *MrdbConnection_escape_string(MrdbConnection *self,
+        PyObject *args)
+{
+    PyObject *string= NULL,
+             *new_string= NULL;
+    size_t from_length, to_length;
+    char *from, *to;
+
+    /* escaping depends on the server status, so we need a valid
+       connection */
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    if (!PyArg_ParseTuple(args, "O!", &PyUnicode_Type, &string))
+        return NULL;
+
+    from= (char *)PyUnicode_AsUTF8AndSize(string, (Py_ssize_t *)&from_length);
+    if (!(to= (char *)PyMem_RawCalloc(1, from_length * 2 + 1)))
+    {
+        return NULL;
+    }
+    to_length= mysql_real_escape_string(self->mysql, to, from, (unsigned long)from_length);
+    new_string= PyUnicode_FromStringAndSize(to, to_length);
+    PyMem_Free(to);
+    return new_string;
+}
+/* }}} */
+
+static PyObject *
+MrdbConnection_dump_debug_info(MrdbConnection *self)
+{
+    int rc;
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+    rc= mysql_dump_debug_info(self->mysql);
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (rc)
+    {
+        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+        return NULL;
+    }
+    Py_RETURN_NONE;
+}
+
+static PyObject *MrdbConnection_readresponse(MrdbConnection *self)
+{
+    int rc;
+
+    MARIADB_BEGIN_ALLOW_THREADS(self);
+    rc= self->mysql->methods->db_read_query_result(self->mysql);
+    MARIADB_END_ALLOW_THREADS(self);
+
+    if (rc)
+    {
+        mariadb_throw_exception(self->mysql, NULL, 0, NULL);
+        return NULL;
+    }
+    Py_RETURN_NONE;
+}
+
+static PyObject *MrdbConnection_socket(MrdbConnection *self)
+{
+    MARIADB_CHECK_CONNECTION(self, NULL);
+
+    return PyLong_FromLong((unsigned long)mysql_get_socket(self->mysql));
+}
+
+/* vim: set tabstop=4 */
+/* vim: set shiftwidth=4 */
+/* vim: set expandtab */
+/* vim: set foldmethod=indent */
+/* vim: set foldnestmax=10 */
+/* vim: set nofoldenable */
+/* vim: set foldlevel=2 */
```

### Comparing `mariadb-1.1.6/mariadb/mariadb_exception.c` & `mariadb-1.1.7/mariadb/mariadb_exception.c`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-/************************************************************************************
-    Copyright (C) 2018 Georg Richter and MariaDB Corporation AB
-
-   This library is free software; you can redistribute it and/or
-   modify it under the terms of the GNU Library General Public
-   License as published by the Free Software Foundation; either
-   version 2 of the License, or (at your option) any later version.
-
-   This library is distributed in the hope that it will be useful,
-   but WITHOUT ANY WARRANTY; without even the implied warranty of
-   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-   Library General Public License for more details.
-
-   You should have received a copy of the GNU Library General Public
-   License along with this library; if not see <http://www.gnu.org/licenses>
-   or write to the Free Software Foundation, Inc.,
-   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
-*************************************************************************************/
-
-#include <mariadb_python.h>
-#include <mysqld_error.h>
-
-/* Exceptions */
-PyObject *Mariadb_InterfaceError;
-PyObject *Mariadb_Error;
-PyObject *Mariadb_DatabaseError;
-PyObject *Mariadb_DataError;
-PyObject *Mariadb_PoolError;
-PyObject *Mariadb_OperationalError;
-PyObject *Mariadb_IntegrityError;
-PyObject *Mariadb_InternalError;
-PyObject *Mariadb_ProgrammingError;
-PyObject *Mariadb_NotSupportedError;
-PyObject *Mariadb_Warning;
-
-struct st_error_map {
-  char  sqlstate[3];
-  uint8_t type;
-};
-
-static PyObject *get_exception_type(int error_number)
-{
-  /* This list might be incomplete, special error values which are
-     not handled yet will be returned as Internal or Operational errors.
-     error codes are defined in errmsg.h (client errors) and mysqld_error.h
-     (server errors) */
-  switch (error_number) {
-  /* InterfaceError */
-  case 0:
-  case CR_SERVER_LOST:
-  case CR_SERVER_GONE_ERROR:
-  case CR_SERVER_HANDSHAKE_ERR:
-  case CR_IPSOCK_ERROR:
-  case CR_COMMANDS_OUT_OF_SYNC:
-      return Mariadb_InterfaceError;
-  /* DataError: Exception raised for errors that are due to problems with the processed
-     data like division by zero, numeric value out of range, etc */
-  case ER_DATA_TOO_LONG:
-  case ER_DATETIME_FUNCTION_OVERFLOW:
-  case ER_DIVISION_BY_ZERO:
-  case ER_NO_DEFAULT:
-  case ER_PRIMARY_CANT_HAVE_NULL:
-  case ER_WARN_DATA_OUT_OF_RANGE:
-  case WARN_DATA_TRUNCATED:
-      return Mariadb_DataError;
-
-  /* ProgrammingError: Exception raised for programming errors, e.g. table not found or 
-     already exists, syntax error in the SQL statement, wrong number of parameters specified, etc. */
-  case ER_EMPTY_QUERY:
-  case ER_CANT_DO_THIS_DURING_AN_TRANSACTION:
-  case ER_DB_CREATE_EXISTS:
-  case ER_FIELD_SPECIFIED_TWICE:
-  case ER_INVALID_GROUP_FUNC_USE:
-  case ER_NO_SUCH_INDEX:
-  case ER_NO_SUCH_KEY_VALUE:
-  case ER_NO_SUCH_TABLE:
-  case ER_NO_SUCH_USER:
-  case ER_PARSE_ERROR:
-  case ER_SYNTAX_ERROR:
-  case ER_TABLE_MUST_HAVE_COLUMNS:
-  case ER_UNSUPPORTED_EXTENSION:
-  case ER_WRONG_DB_NAME:
-  case ER_WRONG_TABLE_NAME:
-  case ER_BAD_DB_ERROR:
-      return Mariadb_ProgrammingError;
-
-  /* IntegrityError: Exception raised when the relational integrity of the database is affected,
-     e.g. a foreign key check fails */
-  case ER_CANNOT_ADD_FOREIGN:
-  case ER_DUP_ENTRY:
-  case ER_DUP_UNIQUE:
-  case ER_NO_DEFAULT_FOR_FIELD:
-  case ER_NO_REFERENCED_ROW:
-  case ER_NO_REFERENCED_ROW_2:
-  case ER_ROW_IS_REFERENCED:
-  case ER_ROW_IS_REFERENCED_2:
-  case ER_XAER_OUTSIDE:
-  case ER_XAER_RMERR:
-  case ER_BAD_NULL_ERROR:
-  case ER_DATA_OUT_OF_RANGE:
-  case ER_CONSTRAINT_FAILED:
-  case ER_DUP_CONSTRAINT_NAME:
-      return Mariadb_IntegrityError;
-  default:
-      /* MariaDB Error */
-      if (error_number >= 1000)
-          return Mariadb_OperationalError;
-      /* same behavior as in MySQLdb: we return an InternalError, in case of system errors */
-      return Mariadb_InternalError;
-  }
-
-  return NULL;
-}
-
-void mariadb_exception_connection_gone(PyObject *exception_type,
-                                  int error_no,
-                                  const char *message,
-                                  ...)
-{
-  va_list ap;
-  PyObject *ErrorMsg= 0;
-  PyObject *ErrorNo= 0;
-  PyObject *SqlState= 0;
-  PyObject *Exception= 0;
-
-  
-  ErrorNo= PyLong_FromLong(CR_UNKNOWN_ERROR);
-  SqlState= PyUnicode_FromString("HY000");
-  va_start(ap, message);
-  ErrorMsg= PyUnicode_FromFormatV(message, ap);
-  va_end(ap);
-
-  if (!(Exception= PyObject_CallFunctionObjArgs(exception_type, ErrorMsg, NULL)))
-  {
-    PyErr_SetString(PyExc_RuntimeError,
-                    "Failed to create exception");
-    return;
-  }
-
-  PyObject_SetAttr(Exception, PyUnicode_FromString("sqlstate"), SqlState);
-  PyObject_SetAttr(Exception, PyUnicode_FromString("errno"), ErrorNo);
-  PyObject_SetAttr(Exception, PyUnicode_FromString("errmsg"), ErrorMsg);
-  /* For MySQL Connector/Python compatibility */
-  PyObject_SetAttr(Exception, PyUnicode_FromString("msg"), ErrorMsg);
-  PyErr_SetObject(exception_type, Exception);
-  Py_XDECREF(ErrorMsg);
-  Py_XDECREF(ErrorNo);
-  Py_XDECREF(SqlState);
-}
-
-/**
- mariadb_throw_exception()
- @brief  raises an exception
-
- @param  handle[in]            a connection or statement handle
- @param  exception_type[in]    type of exception
- @param  handle_type[in]       -1 no handle (use error_no)
-                                0 MYSQL
-                                1 MYSQL_STMT
- @param  message[in]           Error message. If message is NULL, the error
-                               message will be retrieved from specified handle.
- @param  ... [in]              message parameter
-
- @return void
-
-*/
-void mariadb_throw_exception(void *handle,
-                             PyObject *exception_type,
-                             int8_t is_statement,
-                             const char *message,
-                             ...)
-{
-  va_list ap;
-  PyObject *ErrorMsg= 0;
-  PyObject *ErrorNo= 0;
-  PyObject *SqlState= 0;
-  PyObject *Exception= 0;
-
-  if (message)
-  {
-    ErrorNo= PyLong_FromLong(CR_UNKNOWN_ERROR);
-    SqlState= PyUnicode_FromString("HY000");
-    va_start(ap, message);
-    ErrorMsg= PyUnicode_FromFormatV(message, ap);
-    va_end(ap);
-  } else
-  {
-    exception_type= get_exception_type(is_statement ? mysql_stmt_errno((MYSQL_STMT*) handle) : mysql_errno((MYSQL *)handle));
-
-    if (!exception_type)
-      exception_type= Mariadb_DatabaseError;
- 
-    ErrorNo= PyLong_FromLong(is_statement ?
-                          mysql_stmt_errno((MYSQL_STMT *)handle) : mysql_errno((MYSQL *)handle));
-    ErrorMsg= PyUnicode_FromString(is_statement ?
-                        mysql_stmt_error((MYSQL_STMT *)handle) : mysql_error((MYSQL *)handle));
-    SqlState= PyUnicode_FromString(is_statement ?
-                        mysql_stmt_sqlstate((MYSQL_STMT *)handle) : mysql_sqlstate((MYSQL *)handle));
-  }
-
-  if (!(Exception= PyObject_CallFunctionObjArgs(exception_type, ErrorMsg, NULL)))
-  {
-    PyErr_SetString(PyExc_RuntimeError,
-                    "Failed to create exception");
-    return;
-  }
-
-  PyObject_SetAttr(Exception, PyUnicode_FromString("sqlstate"), SqlState);
-  PyObject_SetAttr(Exception, PyUnicode_FromString("errno"), ErrorNo);
-  PyObject_SetAttr(Exception, PyUnicode_FromString("errmsg"), ErrorMsg);
-  /* For MySQL Connector/Python compatibility */
-  PyObject_SetAttr(Exception, PyUnicode_FromString("msg"), ErrorMsg);
-  PyErr_SetObject(exception_type, Exception);
-  Py_XDECREF(ErrorMsg);
-  Py_XDECREF(ErrorNo);
-  Py_XDECREF(SqlState);
-}
-
-
-
+/************************************************************************************
+    Copyright (C) 2018 Georg Richter and MariaDB Corporation AB
+
+   This library is free software; you can redistribute it and/or
+   modify it under the terms of the GNU Library General Public
+   License as published by the Free Software Foundation; either
+   version 2 of the License, or (at your option) any later version.
+
+   This library is distributed in the hope that it will be useful,
+   but WITHOUT ANY WARRANTY; without even the implied warranty of
+   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+   Library General Public License for more details.
+
+   You should have received a copy of the GNU Library General Public
+   License along with this library; if not see <http://www.gnu.org/licenses>
+   or write to the Free Software Foundation, Inc.,
+   51 Franklin St., Fifth Floor, Boston, MA 02110, USA
+*************************************************************************************/
+
+#include <mariadb_python.h>
+#include <mysqld_error.h>
+
+/* Exceptions */
+PyObject *Mariadb_InterfaceError;
+PyObject *Mariadb_Error;
+PyObject *Mariadb_DatabaseError;
+PyObject *Mariadb_DataError;
+PyObject *Mariadb_PoolError;
+PyObject *Mariadb_OperationalError;
+PyObject *Mariadb_IntegrityError;
+PyObject *Mariadb_InternalError;
+PyObject *Mariadb_ProgrammingError;
+PyObject *Mariadb_NotSupportedError;
+PyObject *Mariadb_Warning;
+
+struct st_error_map {
+  char  sqlstate[3];
+  uint8_t type;
+};
+
+static PyObject *get_exception_type(int error_number)
+{
+  /* This list might be incomplete, special error values which are
+     not handled yet will be returned as Internal or Operational errors.
+     error codes are defined in errmsg.h (client errors) and mysqld_error.h
+     (server errors) */
+  switch (error_number) {
+  /* InterfaceError */
+  case 0:
+  case CR_SERVER_LOST:
+  case CR_SERVER_GONE_ERROR:
+  case CR_SERVER_HANDSHAKE_ERR:
+  case CR_IPSOCK_ERROR:
+  case CR_COMMANDS_OUT_OF_SYNC:
+      return Mariadb_InterfaceError;
+  /* DataError: Exception raised for errors that are due to problems with the processed
+     data like division by zero, numeric value out of range, etc */
+  case ER_DATA_TOO_LONG:
+  case ER_DATETIME_FUNCTION_OVERFLOW:
+  case ER_DIVISION_BY_ZERO:
+  case ER_NO_DEFAULT:
+  case ER_PRIMARY_CANT_HAVE_NULL:
+  case ER_WARN_DATA_OUT_OF_RANGE:
+  case WARN_DATA_TRUNCATED:
+      return Mariadb_DataError;
+
+  /* ProgrammingError: Exception raised for programming errors, e.g. table not found or 
+     already exists, syntax error in the SQL statement, wrong number of parameters specified, etc. */
+  case ER_EMPTY_QUERY:
+  case ER_CANT_DO_THIS_DURING_AN_TRANSACTION:
+  case ER_DB_CREATE_EXISTS:
+  case ER_FIELD_SPECIFIED_TWICE:
+  case ER_INVALID_GROUP_FUNC_USE:
+  case ER_NO_SUCH_INDEX:
+  case ER_NO_SUCH_KEY_VALUE:
+  case ER_NO_SUCH_TABLE:
+  case ER_NO_SUCH_USER:
+  case ER_PARSE_ERROR:
+  case ER_SYNTAX_ERROR:
+  case ER_TABLE_MUST_HAVE_COLUMNS:
+  case ER_UNSUPPORTED_EXTENSION:
+  case ER_WRONG_DB_NAME:
+  case ER_WRONG_TABLE_NAME:
+  case ER_BAD_DB_ERROR:
+      return Mariadb_ProgrammingError;
+
+  /* IntegrityError: Exception raised when the relational integrity of the database is affected,
+     e.g. a foreign key check fails */
+  case ER_CANNOT_ADD_FOREIGN:
+  case ER_DUP_ENTRY:
+  case ER_DUP_UNIQUE:
+  case ER_NO_DEFAULT_FOR_FIELD:
+  case ER_NO_REFERENCED_ROW:
+  case ER_NO_REFERENCED_ROW_2:
+  case ER_ROW_IS_REFERENCED:
+  case ER_ROW_IS_REFERENCED_2:
+  case ER_XAER_OUTSIDE:
+  case ER_XAER_RMERR:
+  case ER_BAD_NULL_ERROR:
+  case ER_DATA_OUT_OF_RANGE:
+  case ER_CONSTRAINT_FAILED:
+  case ER_DUP_CONSTRAINT_NAME:
+      return Mariadb_IntegrityError;
+  default:
+      /* MariaDB Error */
+      if (error_number >= 1000)
+          return Mariadb_OperationalError;
+      /* same behavior as in MySQLdb: we return an InternalError, in case of system errors */
+      return Mariadb_InternalError;
+  }
+
+  return NULL;
+}
+
+void mariadb_exception_connection_gone(PyObject *exception_type,
+                                  int error_no,
+                                  const char *message,
+                                  ...)
+{
+  va_list ap;
+  PyObject *ErrorMsg= 0;
+  PyObject *ErrorNo= 0;
+  PyObject *SqlState= 0;
+  PyObject *Exception= 0;
+
+  
+  ErrorNo= PyLong_FromLong(CR_UNKNOWN_ERROR);
+  SqlState= PyUnicode_FromString("HY000");
+  va_start(ap, message);
+  ErrorMsg= PyUnicode_FromFormatV(message, ap);
+  va_end(ap);
+
+  if (!(Exception= PyObject_CallFunctionObjArgs(exception_type, ErrorMsg, NULL)))
+  {
+    PyErr_SetString(PyExc_RuntimeError,
+                    "Failed to create exception");
+    return;
+  }
+
+  PyObject_SetAttr(Exception, PyUnicode_FromString("sqlstate"), SqlState);
+  PyObject_SetAttr(Exception, PyUnicode_FromString("errno"), ErrorNo);
+  PyObject_SetAttr(Exception, PyUnicode_FromString("errmsg"), ErrorMsg);
+  /* For MySQL Connector/Python compatibility */
+  PyObject_SetAttr(Exception, PyUnicode_FromString("msg"), ErrorMsg);
+  PyErr_SetObject(exception_type, Exception);
+  Py_XDECREF(ErrorMsg);
+  Py_XDECREF(ErrorNo);
+  Py_XDECREF(SqlState);
+}
+
+/**
+ mariadb_throw_exception()
+ @brief  raises an exception
+
+ @param  handle[in]            a connection or statement handle
+ @param  exception_type[in]    type of exception
+ @param  handle_type[in]       -1 no handle (use error_no)
+                                0 MYSQL
+                                1 MYSQL_STMT
+ @param  message[in]           Error message. If message is NULL, the error
+                               message will be retrieved from specified handle.
+ @param  ... [in]              message parameter
+
+ @return void
+
+*/
+void mariadb_throw_exception(void *handle,
+                             PyObject *exception_type,
+                             int8_t is_statement,
+                             const char *message,
+                             ...)
+{
+  va_list ap;
+  PyObject *ErrorMsg= 0;
+  PyObject *ErrorNo= 0;
+  PyObject *SqlState= 0;
+  PyObject *Exception= 0;
+
+  if (message)
+  {
+    ErrorNo= PyLong_FromLong(CR_UNKNOWN_ERROR);
+    SqlState= PyUnicode_FromString("HY000");
+    va_start(ap, message);
+    ErrorMsg= PyUnicode_FromFormatV(message, ap);
+    va_end(ap);
+  } else
+  {
+    exception_type= get_exception_type(is_statement ? mysql_stmt_errno((MYSQL_STMT*) handle) : mysql_errno((MYSQL *)handle));
+
+    if (!exception_type)
+      exception_type= Mariadb_DatabaseError;
+ 
+    ErrorNo= PyLong_FromLong(is_statement ?
+                          mysql_stmt_errno((MYSQL_STMT *)handle) : mysql_errno((MYSQL *)handle));
+    ErrorMsg= PyUnicode_FromString(is_statement ?
+                        mysql_stmt_error((MYSQL_STMT *)handle) : mysql_error((MYSQL *)handle));
+    SqlState= PyUnicode_FromString(is_statement ?
+                        mysql_stmt_sqlstate((MYSQL_STMT *)handle) : mysql_sqlstate((MYSQL *)handle));
+  }
+
+  if (!(Exception= PyObject_CallFunctionObjArgs(exception_type, ErrorMsg, NULL)))
+  {
+    PyErr_SetString(PyExc_RuntimeError,
+                    "Failed to create exception");
+    return;
+  }
+
+  PyObject_SetAttr(Exception, PyUnicode_FromString("sqlstate"), SqlState);
+  PyObject_SetAttr(Exception, PyUnicode_FromString("errno"), ErrorNo);
+  PyObject_SetAttr(Exception, PyUnicode_FromString("errmsg"), ErrorMsg);
+  /* For MySQL Connector/Python compatibility */
+  PyObject_SetAttr(Exception, PyUnicode_FromString("msg"), ErrorMsg);
+  PyErr_SetObject(exception_type, Exception);
+  Py_XDECREF(ErrorMsg);
+  Py_XDECREF(ErrorNo);
+  Py_XDECREF(SqlState);
+}
+
+
+
```

### Comparing `mariadb-1.1.6/mariadb.egg-info/PKG-INFO` & `mariadb-1.1.7/mariadb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 2.1
-Name: mariadb
-Version: 1.1.6
-Summary: Python MariaDB extension
-Home-page: https://www.github.com/mariadb-corporation/mariadb-connector-python
-Author: Georg Richter
-License: LGPL 2.1
-Project-URL: Bug Tracker, https://jira.mariadb.org/
-Project-URL: Documentation, https://mariadb-corporation.github.io/mariadb-connector-python/
-Project-URL: Source Code, https://www.github.com/mariadb-corporation/mariadb-connector-python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <a href="http://mariadb.com/">
-    <img src="https://mariadb.com/kb/static/images/logo-2018-black.png">
-  </a>
-</p>
-
-# MariaDB Connector/Python
-
-[![License (LGPL version 2.1)][licence-image]](LICENSE)
-[![Python 3.7][python-image]][python-url]
-[![Build Status](https://travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)](https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
-<a href="https://scan.coverity.com/projects/mariadb-connector-python">
-  <img alt="Coverity Scan Build Status"
-       src="https://scan.coverity.com/projects/21386/badge.svg"/>
-</a>
-
-MariaDB Connector/Python enables python programs to access MariaDB and MySQL databases, using an API
-which is compliant with the Python DB API 2.0 (PEP-249). It is written in C and uses MariaDB Connector/C
-client library for client server communication.
-
-## License
-
-MariaDB Connector/Python is licensed under the LGPL 2.1
-
-## Source code
-
-MariaDB Connector/Python source code is hosted on [Github](https://github.com/mariadb-corporation/mariadb-connector-python)
-
-## Documentation
-
-MariaDB Connector/Python documentation can be found on [Github Pages](https://mariadb-corporation.github.io/mariadb-connector-python/)
-
-## Bugs
-
-Bugs and feature requests should be filed in the [MariaDB bug ticket system](https://jira.mariadb.org/)
-
-
-[licence-image]:https://img.shields.io/badge/license-GNU%20LGPL%20version%202.1-green.svg?style=flat-square
-[python-image]:https://img.shields.io/badge/python-3.7-blue.svg
-[python-url]:https://www.python.org/downloads/release/python-370/
+Metadata-Version: 2.1
+Name: mariadb
+Version: 1.1.7
+Summary: Python MariaDB extension
+Home-page: https://www.github.com/mariadb-corporation/mariadb-connector-python
+Author: Georg Richter
+License: LGPL 2.1
+Project-URL: Bug Tracker, https://jira.mariadb.org/
+Project-URL: Documentation, https://mariadb-corporation.github.io/mariadb-connector-python/
+Project-URL: Source Code, https://www.github.com/mariadb-corporation/mariadb-connector-python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Topic :: Database
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <a href="http://mariadb.com/">
+    <img src="https://mariadb.com/kb/static/images/logo-2018-black.png">
+  </a>
+</p>
+
+# MariaDB Connector/Python
+
+[![License (LGPL version 2.1)][licence-image]](LICENSE)
+[![Python 3.7][python-image]][python-url]
+[![Build Status](https://travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)](https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
+<a href="https://scan.coverity.com/projects/mariadb-connector-python">
+  <img alt="Coverity Scan Build Status"
+       src="https://scan.coverity.com/projects/21386/badge.svg"/>
+</a>
+
+MariaDB Connector/Python enables python programs to access MariaDB and MySQL databases, using an API
+which is compliant with the Python DB API 2.0 (PEP-249). It is written in C and uses MariaDB Connector/C
+client library for client server communication.
+
+## License
+
+MariaDB Connector/Python is licensed under the LGPL 2.1
+
+## Source code
+
+MariaDB Connector/Python source code is hosted on [Github](https://github.com/mariadb-corporation/mariadb-connector-python)
+
+## Documentation
+
+MariaDB Connector/Python documentation can be found on [Github Pages](https://mariadb-corporation.github.io/mariadb-connector-python/)
+
+## Bugs
+
+Bugs and feature requests should be filed in the [MariaDB bug ticket system](https://jira.mariadb.org/)
+
+
+[licence-image]:https://img.shields.io/badge/license-GNU%20LGPL%20version%202.1-green.svg?style=flat-square
+[python-image]:https://img.shields.io/badge/python-3.7-blue.svg
+[python-url]:https://www.python.org/downloads/release/python-370/
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: mariadb Version: 1.1.6 Summary: Python MariaDB
+Metadata-Version: 2.1 Name: mariadb Version: 1.1.7 Summary: Python MariaDB
 extension Home-page: https://www.github.com/mariadb-corporation/mariadb-
 connector-python Author: Georg Richter License: LGPL 2.1 Project-URL: Bug
 Tracker, https://jira.mariadb.org/ Project-URL: Documentation, https://mariadb-
 corporation.github.io/mariadb-connector-python/ Project-URL: Source Code,
 https://www.github.com/mariadb-corporation/mariadb-connector-python Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: MacOS X Classifier: Environment :: Win32 (MS
 Windows) Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v2 or later (LGPLv2+) Classifier: Programming Language :: C Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: MacOS Classifier: Operating System :: POSIX Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Topic ::
-Database Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Database Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
           [https://mariadb.com/kb/static/images/logo-2018-black.png]
 # MariaDB Connector/Python [![License (LGPL version 2.1)][licence-image]]
 (LICENSE) [![Python 3.7][python-image]][python-url] [![Build Status](https://
 travis-ci.com/mariadb-corporation/mariadb-connector-python.svg?branch=1.1)]
 (https://app.travis-ci.com/mariadb-corporation/mariadb-connector-python)
 [Coverity_Scan_Build_Status] MariaDB Connector/Python enables python programs
```

### Comparing `mariadb-1.1.6/mariadb.egg-info/SOURCES.txt` & `mariadb-1.1.7/mariadb.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 mariadb_posix.py
 mariadb_windows.py
 pyproject.toml
 setup.py
 site.cfg
+include/config_win.h
 include/mariadb_python.h
 include/docs/common.h
 include/docs/connection.h
 include/docs/cursor.h
 include/docs/exception.h
 include/docs/module.h
 mariadb/__init__.py
```

### Comparing `mariadb-1.1.6/mariadb_posix.py` & `mariadb-1.1.7/mariadb_posix.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-#!/usr/bin/env python
-
-import subprocess
-from packaging import version
-import sys
-import os
-
-
-class MariaDBConfiguration():
-    lib_dirs = []
-    libs = []
-    version = []
-    includes = []
-    extra_objects = []
-    extra_compile_args = []
-    extra_link_args = []
-
-
-def mariadb_config(config, option):
-    from os import popen
-    file = popen("%s --%s" % (config, option))
-    data = file.read().strip().split()
-    rc = file.close()
-    if rc:
-        if rc / 256:
-            data = []
-        if rc / 256 > 1:
-            raise EnvironmentError(
-                """mariadb_config not found.
-
-This error typically indicates that MariaDB Connector/C, a dependency which
-must be preinstalled, is not found.
-If MariaDB Connector/C is not installed, see installation instructions
-If MariaDB Connector/C is installed, either set the environment variable
-MARIADB_CONFIG or edit the configuration file 'site.cfg' to set the
- 'mariadb_config' option to the file location of the mariadb_config utility.
-""")
-
-    return data
-
-
-def dequote(s):
-    if s[0] in "\"'" and s[0] == s[-1]:
-        s = s[1:-1]
-    return s
-
-
-def get_config(options):
-    required_version = "3.3.1"
-    static = options["link_static"]
-
-    try:
-        try:
-            config_prg = os.environ["MARIADB_CONFIG"]
-        except KeyError:
-            config_prg = options["mariadb_config"]
-        subprocess.call([config_prg, "--cc_version"])
-    except FileNotFoundError:
-        # using default from path
-        config_prg = "mariadb_config"
-
-    cc_version = mariadb_config(config_prg, "cc_version")
-    if version.Version(cc_version[0]) < version.Version(required_version):
-        print('MariaDB Connector/Python requires MariaDB Connector/C '
-              '>= %s, found version %s' % (required_version, cc_version[0]))
-        sys.exit(2)
-    cfg = MariaDBConfiguration()
-    cfg.version = cc_version[0]
-
-    plugindir = mariadb_config(config_prg, "plugindir")
-    libs = mariadb_config(config_prg, "libs")
-    extra_libs = mariadb_config(config_prg, "libs_sys")
-    cfg.lib_dirs = [dequote(i[2:]) for i in libs if i.startswith("-L")]
-
-    cfg.libs = [dequote(i[2:]) for i in libs if i.startswith("-l")]
-    includes = mariadb_config(config_prg, "include")
-    mariadb_includes = [dequote(i[2:]) for i in includes if i.startswith("-I")]
-    mariadb_includes.extend(["./include"])
-    if static.lower() == "on":
-        cfg.extra_link_args = ["-u mysql_ps_fetch_functions"]
-        cfg.extra_objects = ['{}/lib{}.a'.format(cfg.lib_dirs[0], lib)
-                             for lib in ["mariadbclient"]]
-        cfg.libs = [dequote(i[2:])
-                    for i in extra_libs if i.startswith("-l")]
-    cfg.includes = mariadb_includes
-    cfg.extra_compile_args = ["-DDEFAULT_PLUGINS_SUBDIR=\"%s\"" % plugindir[0]]
-    return cfg
+#!/usr/bin/env python
+
+import subprocess
+from packaging import version
+import sys
+import os
+
+
+class MariaDBConfiguration():
+    lib_dirs = []
+    libs = []
+    version = []
+    includes = []
+    extra_objects = []
+    extra_compile_args = []
+    extra_link_args = []
+
+
+def mariadb_config(config, option):
+    from os import popen
+    file = popen("%s --%s" % (config, option))
+    data = file.read().strip().split()
+    rc = file.close()
+    if rc:
+        if rc / 256:
+            data = []
+        if rc / 256 > 1:
+            raise EnvironmentError(
+                """mariadb_config not found.
+
+This error typically indicates that MariaDB Connector/C, a dependency which
+must be preinstalled, is not found.
+If MariaDB Connector/C is not installed, see installation instructions
+If MariaDB Connector/C is installed, either set the environment variable
+MARIADB_CONFIG or edit the configuration file 'site.cfg' to set the
+ 'mariadb_config' option to the file location of the mariadb_config utility.
+""")
+
+    return data
+
+
+def dequote(s):
+    if s[0] in "\"'" and s[0] == s[-1]:
+        s = s[1:-1]
+    return s
+
+
+def get_config(options):
+    required_version = "3.3.1"
+    static = options["link_static"]
+
+    try:
+        try:
+            config_prg = os.environ["MARIADB_CONFIG"]
+        except KeyError:
+            config_prg = options["mariadb_config"]
+        subprocess.call([config_prg, "--cc_version"])
+    except FileNotFoundError:
+        # using default from path
+        config_prg = "mariadb_config"
+
+    cc_version = mariadb_config(config_prg, "cc_version")
+    if version.Version(cc_version[0]) < version.Version(required_version):
+        print('MariaDB Connector/Python requires MariaDB Connector/C '
+              '>= %s, found version %s' % (required_version, cc_version[0]))
+        sys.exit(2)
+    cfg = MariaDBConfiguration()
+    cfg.version = cc_version[0]
+
+    plugindir = mariadb_config(config_prg, "plugindir")
+    libs = mariadb_config(config_prg, "libs")
+    extra_libs = mariadb_config(config_prg, "libs_sys")
+    cfg.lib_dirs = [dequote(i[2:]) for i in libs if i.startswith("-L")]
+
+    cfg.libs = [dequote(i[2:]) for i in libs if i.startswith("-l")]
+    includes = mariadb_config(config_prg, "include")
+    mariadb_includes = [dequote(i[2:]) for i in includes if i.startswith("-I")]
+    mariadb_includes.extend(["./include"])
+    if static.lower() == "on":
+        cfg.extra_link_args = ["-u mysql_ps_fetch_functions"]
+        cfg.extra_objects = ['{}/lib{}.a'.format(cfg.lib_dirs[0], lib)
+                             for lib in ["mariadbclient"]]
+        cfg.libs = [dequote(i[2:])
+                    for i in extra_libs if i.startswith("-l")]
+    cfg.includes = mariadb_includes
+    cfg.extra_compile_args = ["-DDEFAULT_PLUGINS_SUBDIR=\"%s\"" % plugindir[0]]
+    return cfg
```

### Comparing `mariadb-1.1.6/mariadb_windows.py` & `mariadb-1.1.7/mariadb_windows.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-#
-# Windows configuration
-#
-
-import os
-import platform
-import sys
-from packaging import version
-
-from winreg import ConnectRegistry, OpenKey, QueryValueEx,\
-    HKEY_LOCAL_MACHINE, KEY_READ, KEY_WOW64_64KEY
-
-
-class MariaDBConfiguration():
-    lib_dirs = []
-    libs = []
-    version = []
-    includes = []
-    extra_objects = []
-    extra_compile_args = []
-    extra_link_args = []
-
-
-def get_config(options):
-    static = options["link_static"]
-    mariadb_dir = options["install_dir"]
-    required_version = "3.2.4"
-
-    if not os.path.exists(mariadb_dir):
-        try:
-            mariadb_dir = os.environ["MARIADB_CC_INSTALL_DIR"]
-            cc_version = ["", ""]
-            print("using environment configuration " + mariadb_dir)
-        except KeyError:
-
-            try:
-                local_reg = ConnectRegistry(None, HKEY_LOCAL_MACHINE)
-                if platform.architecture()[0] == '32bit':
-                    connector_key = OpenKey(local_reg,
-                                            'SOFTWARE\\MariaDB Corporation\\'
-                                            'MariaDB Connector C')
-                else:
-                    connector_key = OpenKey(local_reg,
-                                            'SOFTWARE\\MariaDB Corporation\\'
-                                            'MariaDB Connector C 64-bit',
-                                            access=KEY_READ | KEY_WOW64_64KEY)
-                cc_version = QueryValueEx(connector_key, "Version")
-                if (version.Version(cc_version[0]) <
-                        version.Version(required_version)):
-                    print("MariaDB Connector/Python requires "
-                          "MariaDB Connector/C "
-                          ">= %s (found version: %s") \
-                          % (required_version, cc_version[0])
-                    sys.exit(2)
-                mariadb_dir = QueryValueEx(connector_key, "InstallDir")[0]
-
-            except Exception:
-                print("Could not find InstallationDir of MariaDB Connector/C. "
-                      "Please make sure MariaDB Connector/C is installed or "
-                      "specify the InstallationDir of MariaDB Connector/C by "
-                      "setting the environment variable "
-                      "MARIADB_CC_INSTALL_DIR.")
-                sys.exit(3)
-
-    print("Found MariaDB Connector/C in '%s'" % mariadb_dir)
-    cfg = MariaDBConfiguration()
-    cfg.includes = [".\\include", mariadb_dir + "\\include", mariadb_dir +
-                    "\\include\\mysql"]
-    cfg.lib_dirs = [mariadb_dir + "\\lib"]
-    cfg.libs = ["ws2_32", "advapi32", "kernel32", "shlwapi", "crypt32",
-                "secur32", "bcrypt"]
-    if static.lower() == "on" or static.lower() == "default":
-        cfg.libs.append("mariadbclient")
-    else:
-        print("dynamic")
-    cfg.extra_link_args = ["/NODEFAULTLIB:LIBCMT"]
-    cfg.extra_compile_args = ["/MD"]
-
-    f = open("./include/config_win.h", "w")
-    f.write("#define DEFAULT_PLUGINS_SUBDIR \"%s\\\\lib\\\\plugin\"" %
-            options["install_dir"].replace(""'\\', '\\\\'))
-    f.close()
-    return cfg
+#
+# Windows configuration
+#
+
+import os
+import platform
+import sys
+from packaging import version
+
+from winreg import ConnectRegistry, OpenKey, QueryValueEx,\
+    HKEY_LOCAL_MACHINE, KEY_READ, KEY_WOW64_64KEY
+
+
+class MariaDBConfiguration():
+    lib_dirs = []
+    libs = []
+    version = []
+    includes = []
+    extra_objects = []
+    extra_compile_args = []
+    extra_link_args = []
+
+
+def get_config(options):
+    static = options["link_static"]
+    mariadb_dir = options["install_dir"]
+    required_version = "3.2.4"
+
+    if not os.path.exists(mariadb_dir):
+        try:
+            mariadb_dir = os.environ["MARIADB_CC_INSTALL_DIR"]
+            cc_version = ["", ""]
+            print("using environment configuration " + mariadb_dir)
+        except KeyError:
+
+            try:
+                local_reg = ConnectRegistry(None, HKEY_LOCAL_MACHINE)
+                if platform.architecture()[0] == '32bit':
+                    connector_key = OpenKey(local_reg,
+                                            'SOFTWARE\\MariaDB Corporation\\'
+                                            'MariaDB Connector C')
+                else:
+                    connector_key = OpenKey(local_reg,
+                                            'SOFTWARE\\MariaDB Corporation\\'
+                                            'MariaDB Connector C 64-bit',
+                                            access=KEY_READ | KEY_WOW64_64KEY)
+                cc_version = QueryValueEx(connector_key, "Version")
+                if (version.Version(cc_version[0]) <
+                        version.Version(required_version)):
+                    print("MariaDB Connector/Python requires "
+                          "MariaDB Connector/C "
+                          ">= %s (found version: %s") \
+                          % (required_version, cc_version[0])
+                    sys.exit(2)
+                mariadb_dir = QueryValueEx(connector_key, "InstallDir")[0]
+
+            except Exception:
+                print("Could not find InstallationDir of MariaDB Connector/C. "
+                      "Please make sure MariaDB Connector/C is installed or "
+                      "specify the InstallationDir of MariaDB Connector/C by "
+                      "setting the environment variable "
+                      "MARIADB_CC_INSTALL_DIR.")
+                sys.exit(3)
+
+    print("Found MariaDB Connector/C in '%s'" % mariadb_dir)
+    cfg = MariaDBConfiguration()
+    cfg.includes = [".\\include", mariadb_dir + "\\include", mariadb_dir +
+                    "\\include\\mysql"]
+    cfg.lib_dirs = [mariadb_dir + "\\lib"]
+    cfg.libs = ["ws2_32", "advapi32", "kernel32", "shlwapi", "crypt32",
+                "secur32", "bcrypt"]
+    if static.lower() == "on" or static.lower() == "default":
+        cfg.libs.append("mariadbclient")
+    else:
+        print("dynamic")
+    cfg.extra_link_args = ["/NODEFAULTLIB:LIBCMT"]
+    cfg.extra_compile_args = ["/MD"]
+
+    f = open("./include/config_win.h", "w")
+    f.write("#define DEFAULT_PLUGINS_SUBDIR \"%s\\\\lib\\\\plugin\"" %
+            options["install_dir"].replace(""'\\', '\\\\'))
+    f.close()
+    return cfg
```

### Comparing `mariadb-1.1.6/setup.py` & `mariadb-1.1.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-#!/usr/bin/env python
-
-import os
-
-from setuptools import setup, Extension
-from configparser import ConfigParser
-
-# read the contents of your README file
-from os import path
-
-if os.name == "posix":
-    from mariadb_posix import get_config
-if os.name == "nt":
-    from mariadb_windows import get_config  # noqa: F811
-
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-define_macros = []
-
-# read settings from site.cfg
-c = ConfigParser()
-c.read(['site.cfg'])
-options = dict(c.items('cc_options'))
-
-cfg = get_config(options)
-
-PY_MARIADB_AUTHORS = "Georg Richter"
-
-PY_MARIADB_MAJOR_VERSION = 1
-PY_MARIADB_MINOR_VERSION = 1
-PY_MARIADB_PATCH_VERSION = 6
-PY_MARIADB_PRE_RELEASE_SEGMENT = None
-PY_MARIADB_PRE_RELEASE_NR = 0
-PY_MARIADB_POST_RELEASE_SEGMENT = None
-PY_MARIADB_POST_RELEASE_NR = 0
-
-PY_MARIADB_VERSION = "%s.%s.%s" % (PY_MARIADB_MAJOR_VERSION,
-                                   PY_MARIADB_MINOR_VERSION,
-                                   PY_MARIADB_PATCH_VERSION)
-
-if PY_MARIADB_POST_RELEASE_SEGMENT:
-    PY_MARIADB_VERSION += ".%s" % (PY_MARIADB_POST_RELEASE_SEGMENT +
-                                   PY_MARIADB_POST_RELEASE_NR)
-
-PY_MARIADB_VERSION_INFO = (PY_MARIADB_MAJOR_VERSION,
-                           PY_MARIADB_MINOR_VERSION,
-                           PY_MARIADB_PATCH_VERSION)
-
-if PY_MARIADB_PRE_RELEASE_SEGMENT:
-    PY_MARIADB_VERSION_INFO = PY_MARIADB_VERSION_INFO + (
-                                  PY_MARIADB_PRE_RELEASE_SEGMENT,
-                                  PY_MARIADB_PRE_RELEASE_NR)
-
-if PY_MARIADB_POST_RELEASE_SEGMENT:
-    PY_MARIADB_VERSION_INFO = PY_MARIADB_VERSION_INFO + (
-                                  PY_MARIADB_POST_RELEASE_SEGMENT,
-                                  PY_MARIADB_POST_RELEASE_NR)
-
-define_macros.append(("PY_MARIADB_MAJOR_VERSION", PY_MARIADB_MAJOR_VERSION))
-define_macros.append(("PY_MARIADB_MINOR_VERSION", PY_MARIADB_MINOR_VERSION))
-define_macros.append(("PY_MARIADB_PATCH_VERSION", PY_MARIADB_PATCH_VERSION))
-define_macros.append(("PY_MARIADB_PRE_RELEASE_SEGMENT", "\"%s\"" %
-                      PY_MARIADB_PRE_RELEASE_SEGMENT))
-define_macros.append(("PY_MARIADB_PRE_RELEASE_NR", "\"%s\"" %
-                      PY_MARIADB_PRE_RELEASE_NR))
-define_macros.append(("PY_MARIADB_POST_RELEASE_SEGMENT", "\"%s\"" %
-                      PY_MARIADB_POST_RELEASE_SEGMENT))
-define_macros.append(("PY_MARIADB_POST_RELEASE_NR", "\"%s\"" %
-                      PY_MARIADB_POST_RELEASE_NR))
-
-
-with open("mariadb/release_info.py", "w") as rel_info:
-    rel_info.write("__author__ = '%s'\n__version__ = '%s'\n__version_info__"
-                   " = %s\n" %
-                   (PY_MARIADB_AUTHORS, PY_MARIADB_VERSION,
-                    PY_MARIADB_VERSION_INFO))
-
-setup(name='mariadb',
-      version=PY_MARIADB_VERSION,
-      python_requires='>=3.7',
-      classifiers=[
-          'Development Status :: 5 - Production/Stable',
-          'Environment :: Console',
-          'Environment :: MacOS X',
-          'Environment :: Win32 (MS Windows)',
-          'License :: OSI Approved :: GNU Lesser General Public License'
-          ' v2 or later (LGPLv2+)',
-          'Programming Language :: C',
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10',
-          'Operating System :: Microsoft :: Windows',
-          'Operating System :: MacOS',
-          'Operating System :: POSIX',
-          'Intended Audience :: End Users/Desktop',
-          'Intended Audience :: Developers',
-          'Intended Audience :: System Administrators',
-          'Topic :: Database'
-      ],
-      description='Python MariaDB extension',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      author=PY_MARIADB_AUTHORS,
-      license='LGPL 2.1',
-      url='https://www.github.com/mariadb-corporation/'
-          'mariadb-connector-python',
-      project_urls={
-         "Bug Tracker": "https://jira.mariadb.org/",
-         "Documentation": "https://mariadb-corporation.github.io/"
-                          "mariadb-connector-python/",
-         "Source Code": "https://www.github.com/mariadb-corporation/"
-                        "mariadb-connector-python",
-      },
-      install_requires=['packaging'],
-      ext_modules=[Extension('mariadb._mariadb',
-                             ['mariadb/mariadb.c',
-                              'mariadb/mariadb_codecs.c',
-                              'mariadb/mariadb_connection.c',
-                              'mariadb/mariadb_cursor.c',
-                              'mariadb/mariadb_exception.c',
-                              'mariadb/mariadb_parser.c'],
-                             define_macros=define_macros,
-                             include_dirs=cfg.includes,
-                             library_dirs=cfg.lib_dirs,
-                             libraries=cfg.libs,
-                             extra_compile_args=cfg.extra_compile_args,
-                             extra_link_args=cfg.extra_link_args,
-                             extra_objects=cfg.extra_objects
-                             )],
-      py_modules=['mariadb.__init__',
-                  'mariadb.connectionpool',
-                  'mariadb.connections',
-                  'mariadb.constants.CAPABILITY',
-                  'mariadb.constants.CLIENT',
-                  'mariadb.constants.CURSOR',
-                  'mariadb.constants.ERR',
-                  'mariadb.constants.FIELD_FLAG',
-                  'mariadb.constants.FIELD_TYPE',
-                  'mariadb.constants.INDICATOR',
-                  'mariadb.constants.INFO',
-                  'mariadb.constants.STATUS',
-                  'mariadb.constants.TPC_STATE',
-                  'mariadb.cursors',
-                  'mariadb.dbapi20',
-                  'mariadb.field',
-                  'mariadb.release_info'])
+#!/usr/bin/env python
+
+import os
+
+from setuptools import setup, Extension
+from configparser import ConfigParser
+
+# read the contents of your README file
+from os import path
+
+if os.name == "posix":
+    from mariadb_posix import get_config
+if os.name == "nt":
+    from mariadb_windows import get_config  # noqa: F811
+
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+define_macros = []
+
+# read settings from site.cfg
+c = ConfigParser()
+c.read(['site.cfg'])
+options = dict(c.items('cc_options'))
+
+cfg = get_config(options)
+
+PY_MARIADB_AUTHORS = "Georg Richter"
+
+PY_MARIADB_MAJOR_VERSION = 1
+PY_MARIADB_MINOR_VERSION = 1
+PY_MARIADB_PATCH_VERSION = 7
+PY_MARIADB_PRE_RELEASE_SEGMENT = None
+PY_MARIADB_PRE_RELEASE_NR = 0
+PY_MARIADB_POST_RELEASE_SEGMENT = None
+PY_MARIADB_POST_RELEASE_NR = 0
+
+PY_MARIADB_VERSION = "%s.%s.%s" % (PY_MARIADB_MAJOR_VERSION,
+                                   PY_MARIADB_MINOR_VERSION,
+                                   PY_MARIADB_PATCH_VERSION)
+
+if PY_MARIADB_POST_RELEASE_SEGMENT:
+    PY_MARIADB_VERSION += ".%s" % (PY_MARIADB_POST_RELEASE_SEGMENT +
+                                   PY_MARIADB_POST_RELEASE_NR)
+
+PY_MARIADB_VERSION_INFO = (PY_MARIADB_MAJOR_VERSION,
+                           PY_MARIADB_MINOR_VERSION,
+                           PY_MARIADB_PATCH_VERSION)
+
+if PY_MARIADB_PRE_RELEASE_SEGMENT:
+    PY_MARIADB_VERSION_INFO = PY_MARIADB_VERSION_INFO + (
+                                  PY_MARIADB_PRE_RELEASE_SEGMENT,
+                                  PY_MARIADB_PRE_RELEASE_NR)
+
+if PY_MARIADB_POST_RELEASE_SEGMENT:
+    PY_MARIADB_VERSION_INFO = PY_MARIADB_VERSION_INFO + (
+                                  PY_MARIADB_POST_RELEASE_SEGMENT,
+                                  PY_MARIADB_POST_RELEASE_NR)
+
+define_macros.append(("PY_MARIADB_MAJOR_VERSION", PY_MARIADB_MAJOR_VERSION))
+define_macros.append(("PY_MARIADB_MINOR_VERSION", PY_MARIADB_MINOR_VERSION))
+define_macros.append(("PY_MARIADB_PATCH_VERSION", PY_MARIADB_PATCH_VERSION))
+define_macros.append(("PY_MARIADB_PRE_RELEASE_SEGMENT", "\"%s\"" %
+                      PY_MARIADB_PRE_RELEASE_SEGMENT))
+define_macros.append(("PY_MARIADB_PRE_RELEASE_NR", "\"%s\"" %
+                      PY_MARIADB_PRE_RELEASE_NR))
+define_macros.append(("PY_MARIADB_POST_RELEASE_SEGMENT", "\"%s\"" %
+                      PY_MARIADB_POST_RELEASE_SEGMENT))
+define_macros.append(("PY_MARIADB_POST_RELEASE_NR", "\"%s\"" %
+                      PY_MARIADB_POST_RELEASE_NR))
+
+
+with open("mariadb/release_info.py", "w") as rel_info:
+    rel_info.write("__author__ = '%s'\n__version__ = '%s'\n__version_info__"
+                   " = %s\n" %
+                   (PY_MARIADB_AUTHORS, PY_MARIADB_VERSION,
+                    PY_MARIADB_VERSION_INFO))
+
+setup(name='mariadb',
+      version=PY_MARIADB_VERSION,
+      python_requires='>=3.8',
+      classifiers=[
+          'Development Status :: 5 - Production/Stable',
+          'Environment :: Console',
+          'Environment :: MacOS X',
+          'Environment :: Win32 (MS Windows)',
+          'License :: OSI Approved :: GNU Lesser General Public License'
+          ' v2 or later (LGPLv2+)',
+          'Programming Language :: C',
+          'Programming Language :: Python',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
+          'Operating System :: Microsoft :: Windows',
+          'Operating System :: MacOS',
+          'Operating System :: POSIX',
+          'Intended Audience :: End Users/Desktop',
+          'Intended Audience :: Developers',
+          'Intended Audience :: System Administrators',
+          'Topic :: Database'
+      ],
+      description='Python MariaDB extension',
+      long_description=long_description,
+      long_description_content_type='text/markdown',
+      author=PY_MARIADB_AUTHORS,
+      license='LGPL 2.1',
+      url='https://www.github.com/mariadb-corporation/'
+          'mariadb-connector-python',
+      project_urls={
+         "Bug Tracker": "https://jira.mariadb.org/",
+         "Documentation": "https://mariadb-corporation.github.io/"
+                          "mariadb-connector-python/",
+         "Source Code": "https://www.github.com/mariadb-corporation/"
+                        "mariadb-connector-python",
+      },
+      install_requires=['packaging'],
+      ext_modules=[Extension('mariadb._mariadb',
+                             ['mariadb/mariadb.c',
+                              'mariadb/mariadb_codecs.c',
+                              'mariadb/mariadb_connection.c',
+                              'mariadb/mariadb_cursor.c',
+                              'mariadb/mariadb_exception.c',
+                              'mariadb/mariadb_parser.c'],
+                             define_macros=define_macros,
+                             include_dirs=cfg.includes,
+                             library_dirs=cfg.lib_dirs,
+                             libraries=cfg.libs,
+                             extra_compile_args=cfg.extra_compile_args,
+                             extra_link_args=cfg.extra_link_args,
+                             extra_objects=cfg.extra_objects
+                             )],
+      py_modules=['mariadb.__init__',
+                  'mariadb.connectionpool',
+                  'mariadb.connections',
+                  'mariadb.constants.CAPABILITY',
+                  'mariadb.constants.CLIENT',
+                  'mariadb.constants.CURSOR',
+                  'mariadb.constants.ERR',
+                  'mariadb.constants.FIELD_FLAG',
+                  'mariadb.constants.FIELD_TYPE',
+                  'mariadb.constants.INDICATOR',
+                  'mariadb.constants.INFO',
+                  'mariadb.constants.STATUS',
+                  'mariadb.constants.TPC_STATE',
+                  'mariadb.cursors',
+                  'mariadb.dbapi20',
+                  'mariadb.field',
+                  'mariadb.release_info'])
```

